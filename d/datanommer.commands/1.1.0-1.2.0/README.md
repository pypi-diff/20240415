# Comparing `tmp/datanommer_commands-1.1.0.tar.gz` & `tmp/datanommer_commands-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datanommer_commands-1.1.0.tar", max compression
+gzip compressed data, was "datanommer_commands-1.2.0.tar", max compression
```

## Comparing `datanommer_commands-1.1.0.tar` & `datanommer_commands-1.2.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_commands-1.1.0/LICENSE
--rw-r--r--   0        0        0      392 2021-07-05 15:27:34.000000 datanommer_commands-1.1.0/README.rst
--rw-r--r--   0        0        0     1734 2022-07-06 08:10:03.000000 datanommer_commands-1.1.0/config.toml.example
--rw-r--r--   0        0        0    12060 2022-07-06 08:10:03.000000 datanommer_commands-1.1.0/datanommer/commands/__init__.py
--rw-r--r--   0        0        0     3286 2023-09-22 07:24:59.659106 datanommer_commands-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       45 2022-01-17 12:04:04.000000 datanommer_commands-1.1.0/tests/conftest.py
--rw-r--r--   0        0        0    18962 2023-03-14 06:49:37.000000 datanommer_commands-1.1.0/tests/test_commands.py
--rw-r--r--   0        0        0      602 2023-06-13 07:21:27.000000 datanommer_commands-1.1.0/tox.ini
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 datanommer_commands-1.1.0/setup.py
--rw-r--r--   0        0        0     1109 1970-01-01 00:00:00.000000 datanommer_commands-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2021-07-05 15:27:34.000000 datanommer_commands-1.2.0/LICENSE
+-rw-r--r--   0        0        0      392 2021-07-05 15:27:34.000000 datanommer_commands-1.2.0/README.rst
+-rw-r--r--   0        0        0     1734 2022-07-06 08:10:03.000000 datanommer_commands-1.2.0/config.toml.example
+-rw-r--r--   0        0        0    11417 2024-04-15 09:57:21.426639 datanommer_commands-1.2.0/datanommer/commands/__init__.py
+-rw-r--r--   0        0        0     5020 2024-04-15 09:57:21.426639 datanommer_commands-1.2.0/datanommer/commands/extract_users.py
+-rw-r--r--   0        0        0     2321 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/conftest.py
+-rw-r--r--   0        0        0    18298 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/test_commands.py
+-rw-r--r--   0        0        0     5905 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/test_extract_users.py
+-rw-r--r--   0        0        0     1224 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tests/utils.py
+-rw-r--r--   0        0        0      633 2024-04-15 09:57:21.427639 datanommer_commands-1.2.0/tox.ini
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 datanommer_commands-1.2.0/PKG-INFO
```

### Comparing `datanommer_commands-1.1.0/LICENSE` & `datanommer_commands-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.1.0/config.toml.example` & `datanommer_commands-1.2.0/config.toml.example`

 * *Files identical despite different names*

### Comparing `datanommer_commands-1.1.0/datanommer/commands/__init__.py` & `datanommer_commands-1.2.0/datanommer/commands/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,38 +9,40 @@
 # This program is distributed in the hope that it will be useful, but WITHOUT
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 # details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
+import importlib.metadata
+import itertools
 import json
 import logging
 import time
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 
 import click
 from fedora_messaging import config as fedora_messaging_config
-from sqlalchemy import func
+from sqlalchemy import func, select
 
 import datanommer.models as m
 
 
+__version__ = importlib.metadata.version("datanommer.commands")
+
 log = logging.getLogger("datanommer")
 
 
 def get_config(config_path=None):
     if config_path:
         fedora_messaging_config.conf.load_config(config_path)
     conf = fedora_messaging_config.conf["consumer_config"]
     for key in ("datanommer_sqlalchemy_url", "alembic_ini"):
         if key not in conf:
-            raise click.ClickException(
-                f"{key} not defined in the fedora-messaging config"
-            )
+            raise click.ClickException(f"{key} not defined in the fedora-messaging config")
     return conf
 
 
 config_option = click.option(
     "-c",
     "--config",
     "config_path",
@@ -60,51 +62,47 @@
         alembic_ini=config["alembic_ini"],
         create=True,
     )
 
 
 @click.command()
 @config_option
-@click.option(
-    "--since", default=None, help="Only after datetime, ex 2013-02-14T08:05:59.87"
-)
-@click.option(
-    "--before", default=None, help="Only before datetime, ex 2013-02-14T08:05:59.87"
-)
+@click.option("--since", default=None, help="Only after datetime, ex 2013-02-14T08:05:59.87")
+@click.option("--before", default=None, help="Only before datetime, ex 2013-02-14T08:05:59.87")
 def dump(config_path, since, before):
     """Dump the contents of the datanommer database as JSON.
 
     You can also specify a timespan with the --since and --before arguments:
 
         $ datanommer-dump --before 2013-02-15 --since 2013-02-11T08:00:00 > datanommer-dump.json
     """
     config = get_config(config_path)
     m.init(
         config["datanommer_sqlalchemy_url"],
         alembic_ini=config["alembic_ini"],
     )
 
-    query = m.Message.query
+    query = select(m.Message)
     if before:
         try:
             before = datetime.fromisoformat(before)
-        except ValueError:
-            raise click.ClickException("Invalid date format")
+        except ValueError as e:
+            raise click.ClickException("Invalid date format") from e
 
-        query = query.filter(m.Message.timestamp <= before)
+        query = query.where(m.Message.timestamp <= before)
 
     if since:
         try:
             since = datetime.fromisoformat(since)
-        except ValueError:
-            raise click.ClickException("Invalid date format")
+        except ValueError as e:
+            raise click.ClickException("Invalid date format") from e
 
-        query = query.filter(m.Message.timestamp >= since)
+        query = query.where(m.Message.timestamp >= since)
 
-    results = [json.dumps(msg.as_fedora_message_dict()) for msg in query.all()]
+    results = [json.dumps(msg.as_fedora_message_dict()) for msg in m.session.scalars(query)]
     click.echo(f"[{','.join(results)}]")
 
 
 @click.command()
 @config_option
 @click.option("--topic", is_flag=True, help="Shows the stats per topic")
 @click.option(
@@ -153,56 +151,44 @@
     config = get_config(config_path)
     m.init(
         config["datanommer_sqlalchemy_url"],
         alembic_ini=config["alembic_ini"],
     )
 
     if topic:
+        query = select(m.Message.topic, func.count(m.Message.topic))
         if category:
-            query = m.session.query(
-                m.Message.topic, func.count(m.Message.topic)
-            ).filter(m.Message.category == category)
-        else:
-            query = m.session.query(m.Message.topic, func.count(m.Message.topic))
+            query = query.where(m.Message.category == category)
         query = query.group_by(m.Message.topic)
     else:
+        query = select(m.Message.category, func.count(m.Message.category))
         if category:
-            query = m.session.query(
-                m.Message.category, func.count(m.Message.category)
-            ).filter(m.Message.category == category)
-        else:
-            query = m.session.query(m.Message.category, func.count(m.Message.category))
+            query = query.where(m.Message.category == category)
         query = query.group_by(m.Message.category)
 
-    results = query.all()
+    results = m.session.execute(query).all()
 
     if topic:
         for topic, count in results:
             click.echo(f"{topic} has {count} entries")
     else:
         for category, count in results:
             click.echo(f"{category} has {count} entries")
 
 
 @click.command()
 @config_option
-@click.option(
-    "--topic", default=None, help="Show the latest for only a specific topic."
-)
-@click.option(
-    "--category", default=None, help="Show the latest for only a specific category."
-)
+@click.option("--topic", default=None, help="Show the latest for only a specific topic.")
+@click.option("--category", default=None, help="Show the latest for only a specific category.")
 @click.option(
     "--overall",
     is_flag=True,
     help="Show only the latest message out of all message types.",
 )
-@click.option(
-    "--timestamp", is_flag=True, help="Show only the timestamp of the message(s)."
-)
+@click.option("--timestamp", is_flag=True, help="Show only the timestamp of the message(s).")
 @click.option(
     "--timesince",
     is_flag=True,
     help="Show the number of seconds since the last message",
 )
 @click.option(
     "--human",
@@ -291,38 +277,33 @@
     config = get_config(config_path)
     m.init(
         config["datanommer_sqlalchemy_url"],
         alembic_ini=config["alembic_ini"],
     )
 
     if topic:
-        queries = [m.Message.query.filter(m.Message.topic == topic)]
+        queries = [select(m.Message).where(m.Message.topic == topic)]
 
     elif category:
-        queries = [m.Message.query.filter(m.Message.category == category)]
+        queries = [select(m.Message).where(m.Message.category == category)]
     elif not overall:
         # If no args..
-        categories = [
-            c[0]
-            for c in m.session.query(m.Message.category)
-            .distinct()
-            .order_by(m.Message.category)
-        ]
+        categories_query = select(m.Message.category).distinct().order_by(m.Message.category)
+        categories = m.session.scalars(categories_query)
         queries = [
-            m.Message.query.filter(m.Message.category == category)
-            for category in categories
+            select(m.Message).where(m.Message.category == category) for category in categories
         ]
     else:
         # Show only the single latest message, regardless of type.
-        queries = [m.Message.query]
+        queries = [select(m.Message)]
 
     # Only check messages from the last year to speed up queries
     a_year = timedelta(days=365)
-    earliest = datetime.utcnow() - a_year
-    queries = [q.filter(m.Message.timestamp > earliest) for q in queries]
+    earliest = datetime.now(tz=timezone.utc) - a_year
+    queries = [q.where(m.Message.timestamp > earliest) for q in queries]
 
     # Order and limit to the latest.
     queries = [q.order_by(m.Message.timestamp.desc()).limit(1) for q in queries]
 
     def formatter(key, val):
         if timestamp and human:
             return json.dumps(str(val.timestamp))
@@ -333,29 +314,11 @@
         elif timesince:
             timedelta = datetime.now() - val.timestamp
             return json.dumps(str((timedelta.days * 86400) + timedelta.seconds))
         else:
             return f'{{"{key}": {json.dumps(val.as_fedora_message_dict())}}}'
 
     results = []
-    for result in sum((query.all() for query in queries), []):
+    for result in itertools.chain.from_iterable(m.session.scalars(query) for query in queries):
         results.append(formatter(result.category, result))
 
     click.echo(f"[{','.join(results)}]")
-
-
-# Set the version
-try:  # pragma: no cover
-    import importlib.metadata
-
-    __version__ = importlib.metadata.version("datanommer.commands")
-except ImportError:  # pragma: no cover
-    try:
-        import pkg_resources
-
-        try:
-            __version__ = pkg_resources.get_distribution("datanommer.commands").version
-        except pkg_resources.DistributionNotFound:
-            # The app is not installed, but the flask dev server can run it nonetheless.
-            __version__ = None
-    except ImportError:
-        __version__ = None
```

### Comparing `datanommer_commands-1.1.0/tests/test_commands.py` & `datanommer_commands-1.2.0/tests/test_commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,67 +14,21 @@
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 import json
 import time
 from datetime import datetime, timedelta
 
 import pytest
-from bodhi.messages.schemas.update import UpdateCommentV1
 from click import ClickException
 from click.testing import CliRunner
-from fedora_messaging import message as fedora_message
 
 import datanommer.commands
 import datanommer.models as m
 
-
-def generate_message(
-    topic="org.fedoraproject.test.a.nice.message",
-    body={"encouragement": "You're doing great!"},
-    headers=None,
-):
-    return fedora_message.Message(topic=topic, body=body, headers=headers)
-
-
-def generate_bodhi_update_complete_message():
-    msg = UpdateCommentV1(
-        body={
-            "comment": {
-                "karma": -1,
-                "text": "text",
-                "timestamp": "2019-03-18 16:54:48",
-                "update": {
-                    "alias": "FEDORA-EPEL-2021-f2d195dada",
-                    "builds": [
-                        {"nvr": "abrt-addon-python3-2.1.11-50.el7"},
-                        {"nvr": "kernel-10.4.0-2.el7"},
-                    ],
-                    "status": "pending",
-                    "release": {"name": "F35"},
-                    "request": "testing",
-                    "user": {"name": "ryanlerch"},
-                },
-                "user": {"name": "dudemcpants"},
-            }
-        }
-    )
-    msg.topic = f"org.fedoraproject.stg.{msg.topic}"
-    return msg
-
-
-@pytest.fixture
-def mock_init(mocker):
-    mocker.patch("datanommer.commands.m.init")
-    mocker.patch.dict(
-        datanommer.commands.fedora_messaging_config.conf["consumer_config"],
-        {
-            "datanommer_sqlalchemy_url": "",
-            "alembic_ini": None,
-        },
-    )
+from .utils import generate_bodhi_update_complete_message, generate_message
 
 
 def test_get_datanommer_sqlalchemy_url_keyerror(mocker):
     mocker.patch.dict(
         datanommer.commands.fedora_messaging_config.conf["consumer_config"],
         {},
         clear=True,
@@ -84,17 +38,15 @@
 
 
 def test_get_datanommer_sqlalchemy_url_config(mocker):
     conf = {
         "datanommer_sqlalchemy_url": "",
         "alembic_ini": "/some/where",
     }
-    mocker.patch.dict(
-        datanommer.commands.fedora_messaging_config.conf["consumer_config"], conf
-    )
+    mocker.patch.dict(datanommer.commands.fedora_messaging_config.conf["consumer_config"], conf)
     load_config = mocker.patch(
         "datanommer.commands.fedora_messaging_config.conf.load_config",
     )
     datanommer.commands.get_config("some-path")
     load_config.assert_called_with("some-path")
 
 
@@ -106,22 +58,21 @@
             "datanommer_sqlalchemy_url": "TESTURL",
             "alembic_ini": "/some/where",
         },
     )
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.create, [])
+    assert result.exit_code == 0, result.output
 
     assert result.output == "Creating Datanommer database and tables\n"
-    mock_model_init.assert_called_once_with(
-        "TESTURL", alembic_ini="/some/where", create=True
-    )
+    mock_model_init.assert_called_once_with("TESTURL", alembic_ini="/some/where", create=True)
 
 
-def test_stats(datanommer_models, mock_init):
+def test_stats(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -133,20 +84,21 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.stats, [])
+    assert result.exit_code == 0, result.output
 
     assert "git has 2 entries" in result.output
     assert "fas has 1 entries" in result.output
 
 
-def test_stats_topics(datanommer_models, mock_init):
+def test_stats_topics(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -158,27 +110,22 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.stats, ["--topic"])
+    assert result.exit_code == 0, result.output
 
-    assert (
-        "org.fedoraproject.prod.git.receive.valgrind.master has 1 entries"
-        in result.output
-    )
+    assert "org.fedoraproject.prod.git.receive.valgrind.master has 1 entries" in result.output
     assert "org.fedoraproject.stg.fas.user.create has 1 entries" in result.output
-    assert (
-        "org.fedoraproject.prod.git.branch.valgrind.master has 1 entries"
-        in result.output
-    )
+    assert "org.fedoraproject.prod.git.branch.valgrind.master has 1 entries" in result.output
 
 
-def test_stats_category_topics(datanommer_models, mock_init):
+def test_stats_category_topics(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -190,27 +137,22 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.stats, ["--topic", "--category", "git"])
+    assert result.exit_code == 0, result.output
 
-    assert (
-        "org.fedoraproject.prod.git.receive.valgrind.master has 1 entries"
-        in result.output
-    )
+    assert "org.fedoraproject.prod.git.receive.valgrind.master has 1 entries" in result.output
     assert "org.fedoraproject.stg.fas.user.create has 1 entries" not in result.output
-    assert (
-        "org.fedoraproject.prod.git.branch.valgrind.master has 1 entries"
-        in result.output
-    )
+    assert "org.fedoraproject.prod.git.branch.valgrind.master has 1 entries" in result.output
 
 
-def test_stats_category(datanommer_models, mock_init):
+def test_stats_category(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -222,93 +164,87 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.stats, ["--category", "git"])
+    assert result.exit_code == 0, result.output
 
     assert result.output == "git has 2 entries\n"
 
 
-def test_dump(datanommer_models, mocker, mock_init):
+def test_dump(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     m.add(msg2)
 
     msg3 = generate_bodhi_update_complete_message()
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.dump, [])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
-    assert (
-        json_object[0]["topic"] == "org.fedoraproject.prod.git.branch.valgrind.master"
-    )
+    assert json_object[0]["topic"] == "org.fedoraproject.prod.git.branch.valgrind.master"
 
 
-def test_dump_before(datanommer_models, mocker, mock_init):
+def test_dump_before(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     msg1._properties.headers["sent-at"] = datetime(2013, 2, 14).isoformat()
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.prod.git.receive.valgrind.master")
     msg2._properties.headers["sent-at"] = datetime(2013, 2, 15).isoformat()
     m.add(msg2)
 
     msg3 = generate_message(topic="org.fedoraproject.prod.log.receive.valgrind.master")
     msg3._properties.headers["sent-at"] = datetime(2013, 2, 16, 8).isoformat()
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.dump, ["--before", "2013-02-16"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
-    assert (
-        json_object[0]["topic"] == "org.fedoraproject.prod.git.branch.valgrind.master"
-    )
-    assert (
-        json_object[1]["topic"] == "org.fedoraproject.prod.git.receive.valgrind.master"
-    )
+    assert json_object[0]["topic"] == "org.fedoraproject.prod.git.branch.valgrind.master"
+    assert json_object[1]["topic"] == "org.fedoraproject.prod.git.receive.valgrind.master"
     assert len(json_object) == 2
 
 
-def test_dump_since(datanommer_models, mocker, mock_init):
+def test_dump_since(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     msg1._properties.headers["sent-at"] = datetime(2013, 2, 14).isoformat()
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.prod.git.receive.valgrind.master")
     msg2._properties.headers["sent-at"] = datetime(2013, 2, 15).isoformat()
     m.add(msg2)
 
     msg3 = generate_message(topic="org.fedoraproject.prod.log.receive.valgrind.master")
     msg3._properties.headers["sent-at"] = datetime(2013, 2, 16, 8).isoformat()
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.dump, ["--since", "2013-02-14T08:00:00"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
-    assert (
-        json_object[0]["topic"] == "org.fedoraproject.prod.git.receive.valgrind.master"
-    )
-    assert (
-        json_object[1]["topic"] == "org.fedoraproject.prod.log.receive.valgrind.master"
-    )
+    assert json_object[0]["topic"] == "org.fedoraproject.prod.git.receive.valgrind.master"
+    assert json_object[1]["topic"] == "org.fedoraproject.prod.log.receive.valgrind.master"
     assert len(json_object) == 2
 
 
-def test_dump_timespan(datanommer_models, mocker, mock_init):
+def test_dump_timespan(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     msg1._properties.headers["sent-at"] = datetime(2013, 2, 14).isoformat()
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.prod.git.receive.valgrind.master")
     msg2._properties.headers["sent-at"] = datetime(2013, 2, 15).isoformat()
     m.add(msg2)
@@ -318,33 +254,34 @@
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(
         datanommer.commands.dump,
         ["--before", "2013-02-16", "--since", "2013-02-14T08:00:00"],
     )
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
-    assert (
-        json_object[0]["topic"] == "org.fedoraproject.prod.git.receive.valgrind.master"
-    )
+    assert json_object[0]["topic"] == "org.fedoraproject.prod.git.receive.valgrind.master"
     assert len(json_object) == 1
 
 
-def test_dump_invalid_dates(datanommer_models, mocker, mock_init):
+def test_dump_invalid_dates(datanommer_models, mock_config, mock_init):
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.dump, ["--before", "2013-02-16asdasd"])
+    assert result.exit_code > 0, result.output
     assert result.output == "Error: Invalid date format\n"
 
     result = runner.invoke(datanommer.commands.dump, ["--since", "2013-02-16asdasd"])
+    assert result.exit_code > 0, result.output
     assert result.output == "Error: Invalid date format\n"
 
 
-def test_latest_overall(datanommer_models, mock_init):
+def test_latest_overall(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -356,22 +293,23 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, ["--overall"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     assert json_object[0]["git"]["body"] == {"Message 3": "Message 3"}
     assert len(json_object) == 1
 
 
-def test_latest_topic(datanommer_models, mock_init):
+def test_latest_topic(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -385,22 +323,23 @@
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(
         datanommer.commands.latest, ["--topic", "org.fedoraproject.stg.fas.user.create"]
     )
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     assert json_object[0]["fas"]["body"] == {"Message 2": "Message 2"}
     assert len(json_object) == 1
 
 
-def test_latest_category(datanommer_models, mock_init):
+def test_latest_category(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     m.add(msg1)
 
     msg2 = generate_message(
@@ -412,55 +351,52 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, ["--category", "fas"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     assert json_object[0]["fas"]["body"] == {"Message 2": "Message 2"}
     assert len(json_object) == 1
 
 
-def test_latest_timestamp_human(datanommer_models, mocker, mock_init):
+def test_latest_timestamp_human(datanommer_models, mocker, mock_config, mock_init):
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     msg1._properties.headers["sent-at"] = datetime(2013, 2, 14).isoformat()
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.stg.fas.user.create")
-    msg2._properties.headers["sent-at"] = datetime(
-        2013, 2, 15, 15, 15, 15, 15
-    ).isoformat()
+    msg2._properties.headers["sent-at"] = datetime(2013, 2, 15, 15, 15, 15, 15).isoformat()
     m.add(msg2)
 
     msg3 = generate_message(topic="org.fedoraproject.prod.git.receive.valgrind.master")
-    msg3._properties.headers["sent-at"] = datetime(
-        2013, 2, 16, 16, 16, 16, 16
-    ).isoformat()
+    msg3._properties.headers["sent-at"] = datetime(2013, 2, 16, 16, 16, 16, 16).isoformat()
     m.add(msg3)
 
     # datanommer-latest defaults to the last year, so mock the
     # datetime calls to go back to 2013
     mock_dt = mocker.patch("datanommer.commands.datetime")
-    mock_dt.utcnow.return_value = datetime(2013, 3, 1)
     mock_dt.now.return_value = datetime(2013, 3, 1)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, ["--timestamp", "--human"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     assert json_object[1] == "2013-02-16 16:16:16.000016"
     assert json_object[0] == "2013-02-15 15:15:15.000015"
     assert len(json_object) == 2
 
 
-def test_latest_timestamp(datanommer_models, mocker, mock_init):
+def test_latest_timestamp(datanommer_models, mocker, mock_config, mock_init):
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     msg1._properties.headers["sent-at"] = datetime(2013, 2, 14).isoformat()
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.stg.fas.user.create")
     msg2._properties.headers["sent-at"] = datetime(2013, 2, 15).isoformat()
     m.add(msg2)
@@ -468,28 +404,28 @@
     msg3 = generate_message(topic="org.fedoraproject.prod.git.receive.valgrind.master")
     msg3._properties.headers["sent-at"] = datetime(2013, 2, 16).isoformat()
     m.add(msg3)
 
     # datanommer-latest defaults to the last year, so mock the
     # datetime calls to go back to 2013
     mock_dt = mocker.patch("datanommer.commands.datetime")
-    mock_dt.utcnow.return_value = datetime(2013, 3, 1)
     mock_dt.now.return_value = datetime(2013, 3, 1)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, ["--timestamp"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     assert json_object[1] == time.mktime(datetime(2013, 2, 16).timetuple())
     assert json_object[0] == time.mktime(datetime(2013, 2, 15).timetuple())
     assert len(json_object) == 2
 
 
-def test_latest_timesince(datanommer_models, mocker, mock_init):
+def test_latest_timesince(datanommer_models, mocker, mock_config, mock_init):
     now = datetime(2013, 3, 1)
 
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     time1 = now - timedelta(days=1)
     msg1._properties.headers["sent-at"] = time1.isoformat()
     m.add(msg1)
 
@@ -502,32 +438,35 @@
     time3 = now - timedelta(seconds=1)
     msg3._properties.headers["sent-at"] = time3.isoformat()
     m.add(msg3)
 
     # datanommer-latest defaults to the last year, so mock the
     # datetime calls to go back to 2013
     mock_dt = mocker.patch("datanommer.commands.datetime")
-    mock_dt.utcnow.return_value = now
     mock_dt.now.return_value = now
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, ["--timesince"])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     # allow .1 second to run test
     assert int(json_object[1]) <= 1.1
     assert int(json_object[1]) >= 1
     assert int(json_object[0]) <= 60.1
     assert int(json_object[0]) >= 60
     assert len(json_object) == 2
 
 
-def test_latest_timesince_human(datanommer_models, mock_init):
+def test_latest_timesince_human(datanommer_models, mock_config, mock_init, mocker):
     now = datetime.now()
+    # mocker.patch.object(datanommer.commands.datetime, "now", return_value=now)
+    patched_datetime = mocker.patch("datanommer.commands.datetime", mocker.Mock(wraps=datetime))
+    patched_datetime.now.return_value = now
 
     msg1 = generate_message(topic="org.fedoraproject.prod.git.branch.valgrind.master")
     time1 = now - timedelta(days=2)
     msg1._properties.headers["sent-at"] = time1.isoformat()
     m.add(msg1)
 
     msg2 = generate_message(topic="org.fedoraproject.stg.fas.user.create")
@@ -538,25 +477,20 @@
     msg3 = generate_message(topic="org.fedoraproject.prod.git.receive.valgrind.master")
     time3 = now - timedelta(seconds=1)
     msg3._properties.headers["sent-at"] = time3.isoformat()
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, ["--timesince", "--human"])
+    assert result.exit_code == 0, result.output
 
-    json_object = json.loads(result.output)
-
-    # cannot assert exact value because of time to run test
-    assert "day" not in json_object[1]
-    assert "0:00:01." in json_object[1]
-    assert "1 day in 0:00:00.", json_object[0]
-    assert len(json_object) == 2
+    assert json.loads(result.output) == ["1 day, 0:00:00", "0:00:01"]
 
 
-def test_latest(datanommer_models, mock_init):
+def test_latest(datanommer_models, mock_config, mock_init):
     msg1 = generate_message(
         topic="org.fedoraproject.prod.git.branch.valgrind.master",
         body={"Message 1": "Message 1"},
     )
     time1 = datetime.now() - timedelta(days=2)
     msg1._properties.headers["sent-at"] = time1.isoformat()
     m.add(msg1)
@@ -570,13 +504,14 @@
         topic="org.fedoraproject.prod.git.receive.valgrind.master",
         body={"Message 3": "Message 3"},
     )
     m.add(msg3)
 
     runner = CliRunner()
     result = runner.invoke(datanommer.commands.latest, [])
+    assert result.exit_code == 0, result.output
 
     json_object = json.loads(result.output)
 
     assert json_object[1]["git"]["body"] == {"Message 3": "Message 3"}
     assert json_object[0]["fas"]["body"] == {"Message 2": "Message 2"}
     assert len(json_object) == 2
```

### Comparing `datanommer_commands-1.1.0/tox.ini` & `datanommer_commands-1.2.0/tox.ini`

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

### Comparing `datanommer_commands-1.1.0/PKG-INFO` & `datanommer_commands-1.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
-Name: datanommer-commands
-Version: 1.1.0
+Name: datanommer.commands
+Version: 1.2.0
 Summary: Console commands for datanommer
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
 Project-URL: Repository, https://github.com/fedora-infra/datanommer
 Description-Content-Type: text/x-rst
 
 datanommer.commands
 ===================
```

