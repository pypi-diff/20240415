# Comparing `tmp/mqi_sspd_api-0.0.9.tar.gz` & `tmp/mqi_sspd_api-0.1.10.tar.gz`

## Comparing `mqi_sspd_api-0.0.9.tar` & `mqi_sspd_api-0.1.10.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/examples/__init__.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/examples/set_current.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/mqi/v1/__init__.py
--rw-r--r--   0        0        0     7236 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/mqi/v1/api.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/LICENSE
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/README.md
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 mqi_sspd_api-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/examples/__init__.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/examples/set_current.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/mqi/v1/__init__.py
+-rw-r--r--   0        0        0     7243 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/mqi/v1/api.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/LICENSE
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/README.md
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/pyproject.toml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 mqi_sspd_api-0.1.10/PKG-INFO
```

### Comparing `mqi_sspd_api-0.0.9/mqi/v1/api.py` & `mqi_sspd_api-0.1.10/mqi/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,18 +106,17 @@
           "__MESSAGE__": "message",
           "command": "allChannels",
           "id": "",
           "name": "",
           "value": "0"
         }
 
-				self.ws.send(json.dumps(data))
-				sleep(0.2)
+        self.ws.send(json.dumps(data))
+        sleep(0.2)
         print(self.ws.recv())
-
         return True
 
     """
     current_sweep will initiate a current sweep for the channel chosen
 
     @param arduino_id:int -- id of the arduino to select
     @param fr:float -- short for from, this is the current to start from (mA)
```

### Comparing `mqi_sspd_api-0.0.9/LICENSE` & `mqi_sspd_api-0.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `mqi_sspd_api-0.0.9/pyproject.toml` & `mqi_sspd_api-0.1.10/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "websocket-client", "rel"]
 build-backend = "hatchling.build"
 [project]
 dependencies = ['websocket-client', 'rel']
 name = "mqi_sspd_api"
-version = "0.0.9"
+version = "0.1.10"
 authors = [
   { name="Filip Zlatoidsky", email="fillatino@gmail.com" },
 ]
 description = "This is the official API of the MQI biasing box"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

