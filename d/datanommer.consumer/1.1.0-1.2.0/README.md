# Comparing `tmp/datanommer_consumer-1.1.0.tar.gz` & `tmp/datanommer_consumer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanommer_consumer-1.1.0.tar", max compression
+gzip compressed data, was "datanommer_consumer-1.2.0.tar", max compression
```

## Comparing `datanommer_consumer-1.1.0.tar` & `datanommer_consumer-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_consumer-1.1.0/LICENSE
--rw-r--r--   0        0        0      311 2022-01-17 12:04:04.000000 datanommer_consumer-1.1.0/README.rst
--rw-r--r--   0        0        0     1957 2022-01-17 12:04:04.000000 datanommer_consumer-1.1.0/datanommer/consumer/__init__.py
--rw-r--r--   0        0        0     3086 2023-09-22 07:24:59.659106 datanommer_consumer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      736 2021-07-05 15:27:34.000000 datanommer_consumer-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_consumer-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0     2013 2022-01-17 12:04:04.000000 datanommer_consumer-1.1.0/tests/test_consumer.py
--rw-r--r--   0        0        0      602 2023-06-13 09:23:37.000000 datanommer_consumer-1.1.0/tox.ini
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 datanommer_consumer-1.1.0/setup.py
--rw-r--r--   0        0        0     1061 1970-01-01 00:00:00.000000 datanommer_consumer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_consumer-1.2.0/LICENSE
+-rw-r--r--   0        0        0      311 2022-01-17 12:04:04.000000 datanommer_consumer-1.2.0/README.rst
+-rw-r--r--   0        0        0     1515 2024-04-15 09:57:21.427639 datanommer_consumer-1.2.0/datanommer/consumer/__init__.py
+-rw-r--r--   0        0        0     1980 2024-04-15 09:57:21.427639 datanommer_consumer-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      736 2021-07-05 15:27:34.000000 datanommer_consumer-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_consumer-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     2059 2024-04-15 09:57:21.428639 datanommer_consumer-1.2.0/tests/test_consumer.py
+-rw-r--r--   0        0        0      633 2024-04-15 09:57:21.428639 datanommer_consumer-1.2.0/tox.ini
+-rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 datanommer_consumer-1.2.0/PKG-INFO
```

### Comparing `datanommer_consumer-1.1.0/LICENSE` & `datanommer_consumer-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datanommer_consumer-1.1.0/datanommer/consumer/__init__.py` & `datanommer_consumer-1.2.0/datanommer/consumer/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
+import importlib.metadata
 import logging
 
 from fedora_messaging import config
 
 import datanommer.models as m
 
 
+__version__ = importlib.metadata.version("datanommer.consumer")
+
+
 def get_datanommer_sqlalchemy_url():
     try:
         return config.conf["consumer_config"]["datanommer_sqlalchemy_url"]
-    except KeyError:
+    except KeyError as e:
         raise ValueError(
             "datanommer_sqlalchemy_url not defined in the fedora-messaging config"
-        )
+        ) from e
 
 
 log = logging.getLogger("datanommer-consumer")
 
 
 class Nommer:
     def __init__(self):
@@ -39,25 +43,7 @@
     def __call__(self, message):
         log.info("Nomming %r" % message)
         try:
             m.add(message)
         except Exception:
             m.session.rollback()
             raise
-
-
-# Set the version
-try:  # pragma: no cover
-    import importlib.metadata
-
-    __version__ = importlib.metadata.version("datanommer.consumer")
-except ImportError:  # pragma: no cover
-    try:
-        import pkg_resources
-
-        try:
-            __version__ = pkg_resources.get_distribution("datanommer.consumer").version
-        except pkg_resources.DistributionNotFound:
-            # The app is not installed, but the flask dev server can run it nonetheless.
-            __version__ = None
-    except ImportError:
-        __version__ = None
```

### Comparing `datanommer_consumer-1.1.0/tests/__init__.py` & `datanommer_consumer-1.2.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `datanommer_consumer-1.1.0/tests/test_consumer.py` & `datanommer_consumer-1.2.0/tests/test_consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 # details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import pytest
 from fedora_messaging import message
+from sqlalchemy import func, select
 
 import datanommer.consumer
-import datanommer.models
+import datanommer.models as dm
 
 
 @pytest.fixture
 def consumer(mocker):
     mock_get_url = mocker.patch("datanommer.consumer.get_datanommer_sqlalchemy_url")
     mock_get_url.return_value = "sqlite:///fake.db"
     return datanommer.consumer.Nommer()
@@ -32,25 +33,25 @@
     example_message = message.Message(
         topic="nice.message", body={"encouragement": "You're doing great!"}
     )
 
     consumer = datanommer.consumer.Nommer()
 
     consumer(example_message)
-    assert datanommer.models.Message.query.count() == 1
+    assert dm.session.scalar(select(func.count(dm.Message.id))) == 1
 
 
 def test_add_exception(datanommer_models, consumer, mocker):
     example_message = message.Message(
         topic="nice.message", body={"encouragement": "You're doing great!"}
     )
 
-    datanommer.models.add = mocker.Mock(side_effect=Exception("an exception"))
+    dm.add = mocker.Mock(side_effect=RuntimeError("an exception"))
     consumer = datanommer.consumer.Nommer()
-    with pytest.raises(Exception):
+    with pytest.raises(RuntimeError):
         consumer(example_message)
 
 
 def test_get_datanommer_sqlalchemy_url_keyerror(mocker):
     mocker.patch.dict(
         datanommer.consumer.config.conf["consumer_config"],
         {},
```

### Comparing `datanommer_consumer-1.1.0/tox.ini` & `datanommer_consumer-1.2.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 sitepackages = false
 skip_install = true
 # Use allowlist for poetry when poetry 1.2+ is more widespread
 # allowlist_externals =
 #     poetry
 deps =
     poetry>=1.2
+env =
+    SQLALCHEMY_WARN_20=1
 commands_pre =
     poetry install --all-extras
     poetry run {toxinidir}/../tools/install-models-as-editable.sh
 commands =
     poetry run pytest -c ../pyproject.toml {posargs}
 
 [testenv:licenses]
```

### Comparing `datanommer_consumer-1.1.0/PKG-INFO` & `datanommer_consumer-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: datanommer-consumer
-Version: 1.1.0
+Name: datanommer.consumer
+Version: 1.2.0
 Summary: Consumer for datanommer
 Home-page: https://github.com/fedora-infra/datanommer
 License: GPL-3.0-or-later
 Author: Fedora Infrastructure
 Author-email: admin@fedoraproject.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: datanommer.models (>=1.0.0,<2.0.0)
 Requires-Dist: fedora-messaging (>=2.1.0)
 Requires-Dist: psycopg2 (>=2.9.1,<3.0.0)
 Project-URL: Repository, https://github.com/fedora-infra/datanommer
 Description-Content-Type: text/x-rst
 
 datanommer.consumer
```

