# Comparing `tmp/somnetics_seamless_utils-0.0.2.tar.gz` & `tmp/somnetics_seamless_utils-0.0.3.tar.gz`

## Comparing `somnetics_seamless_utils-0.0.2.tar` & `somnetics_seamless_utils-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/__init__.py
--rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/config.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/elastic.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/message.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/objectstore.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/requirements.txt
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/service.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/README.md
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/__init__.py
+-rw-r--r--   0        0        0     5939 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/config.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/elastic.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/message.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/objectstore.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/requirements.txt
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/service.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/LICENSE
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 somnetics_seamless_utils-0.0.3/PKG-INFO
```

### Comparing `somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/config.py` & `somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/config.py`

 * *Files identical despite different names*

### Comparing `somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/elastic.py` & `somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/elastic.py`

 * *Files identical despite different names*

### Comparing `somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/message.py` & `somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/message.py`

 * *Files identical despite different names*

### Comparing `somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/objectstore.py` & `somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/objectstore.py`

 * *Files identical despite different names*

### Comparing `somnetics_seamless_utils-0.0.2/src/somnetics_seamless_utils/service.py` & `somnetics_seamless_utils-0.0.3/src/somnetics_seamless_utils/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import sys
 import getopt
 import resource
 import logging
 import falcon
 from abc import abstractmethod, ABCMeta
 from wsgiref.simple_server import make_server
-from seamless.config import Config
-from seamless.message import MessageQueue
+from config import Config
+from message import MessageQueue
 
 class Service(object, metaclass=ABCMeta):
     # region members
 
     _interactive = False
     _config: Config = None
```

### Comparing `somnetics_seamless_utils-0.0.2/.gitignore` & `somnetics_seamless_utils-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `somnetics_seamless_utils-0.0.2/LICENSE` & `somnetics_seamless_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `somnetics_seamless_utils-0.0.2/pyproject.toml` & `somnetics_seamless_utils-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "somnetics_seamless_utils"
-version = "0.0.2"
+version = "0.0.3"
 
 authors = [
   { name="Bibhas Das", email="bibhas.das@somnetics.in" },
 ]
 
 description = "Seamless Framework Utility"
 
@@ -20,23 +20,25 @@
 
 install_requires = [
 	"pika>=1.3.2",
 	"falcon>=3.1.3",
 	"requests>=2.25.1",
 	"minio>=7.2.5",
 	"etcd3>=0.12.0",
+        "elasticsearch>=8.13.0",
 	"protobuf>=3.20.3"
 ]
 
 dependencies = [
 	"pika>=1.3.2",
 	"falcon>=3.1.3",
 	"requests>=2.25.1",
 	"minio>=7.2.5",
 	"etcd3>=0.12.0",
+        "elasticsearch>=8.13.0",
 	"protobuf>=3.20.3"
 ]
 
 test_requires = []
 
 [build-system]
 requires = ["hatchling"]
```

### Comparing `somnetics_seamless_utils-0.0.2/PKG-INFO` & `somnetics_seamless_utils-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.3
 Name: somnetics_seamless_utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: Seamless Framework Utility
 Project-URL: Homepage, https://github.com/bibhas-das-somnetics/seamless-utils
 Project-URL: Issues, https://github.com/bibhas-das-somnetics/seamless-utils/issues
 Author-email: Bibhas Das <bibhas.das@somnetics.in>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: elasticsearch>=8.13.0
 Requires-Dist: etcd3>=0.12.0
 Requires-Dist: falcon>=3.1.3
 Requires-Dist: minio>=7.2.5
 Requires-Dist: pika>=1.3.2
 Requires-Dist: protobuf>=3.20.3
 Requires-Dist: requests>=2.25.1
 Description-Content-Type: text/markdown
```

