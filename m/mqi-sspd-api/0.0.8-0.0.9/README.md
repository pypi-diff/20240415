# Comparing `tmp/mqi_sspd_api-0.0.8.tar.gz` & `tmp/mqi_sspd_api-0.0.9.tar.gz`

## Comparing `mqi_sspd_api-0.0.8.tar` & `mqi_sspd_api-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/examples/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/examples/set_current.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/mqi/v1/__init__.py
--rw-r--r--   0        0        0     7232 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/mqi/v1/api.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/examples/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/examples/set_current.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/mqi/v1/__init__.py
+-rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/mqi/v1/api.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/LICENSE
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/README.md
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/PKG-INFO
```

### Comparing `mqi_sspd_api-0.0.8/mqi/v1/api.py` & `mqi_sspd_api-0.0.9/mqi/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 "id": channel,
                 "name": "",
                 "value": "0"
 
         }
 
         self.ws.send(json.dumps(data))
-				sleep(0.2)
+        sleep(0.2)
         print(self.ws.recv())
 
         return True
 
     """
     get_resolution will return the resolution of the arduino
```

### Comparing `mqi_sspd_api-0.0.8/LICENSE` & `mqi_sspd_api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mqi_sspd_api-0.0.8/pyproject.toml` & `mqi_sspd_api-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "websocket-client", "rel"]
 build-backend = "hatchling.build"
 [project]
 dependencies = ['websocket-client', 'rel']
 name = "mqi_sspd_api"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Filip Zlatoidsky", email="fillatino@gmail.com" },
 ]
 description = "This is the official API of the MQI biasing box"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `mqi_sspd_api-0.0.8/PKG-INFO` & `mqi_sspd_api-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mqi_sspd_api
-Version: 0.0.8
+Version: 0.0.9
 Summary: This is the official API of the MQI biasing box
 Project-URL: Homepage, https://github.com/MQI-Software/mqi-api
 Project-URL: Issues, https://github.com/MQI-Software/mqi-api/issues
 Author-email: Filip Zlatoidsky <fillatino@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

