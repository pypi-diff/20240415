# Comparing `tmp/emerald_hws-0.0.5.tar.gz` & `tmp/emerald_hws-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emerald_hws-0.0.5.tar", last modified: Sat Apr 13 04:11:13 2024, max compression
+gzip compressed data, was "emerald_hws-0.0.6.tar", last modified: Mon Apr 15 10:10:58 2024, max compression
```

## Comparing `emerald_hws-0.0.5.tar` & `emerald_hws-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.693664 emerald_hws-0.0.5/
--rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.5/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-13 04:11:13.692824 emerald_hws-0.0.5/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.5/README.md
--rw-r--r--   0 ross       (501) staff       (20)      824 2024-04-13 04:03:34.000000 emerald_hws-0.0.5/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-13 04:11:13.693904 emerald_hws-0.0.5/setup.cfg
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.686475 emerald_hws-0.0.5/src/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.688860 emerald_hws-0.0.5/src/emerald_hws/
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.690785 emerald_hws-0.0.5/src/emerald_hws/__assets__/
--rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.5/src/emerald_hws/__assets__/SFSRootCAG2.pem
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.5/src/emerald_hws/__init__.py
--rw-r--r--   0 ross       (501) staff       (20)    12069 2024-04-13 03:44:49.000000 emerald_hws-0.0.5/src/emerald_hws/emeraldhws.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-13 04:11:13.691599 emerald_hws-0.0.5/src/emerald_hws.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)       22 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-13 04:11:13.000000 emerald_hws-0.0.5/src/emerald_hws.egg-info/top_level.txt
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.355442 emerald_hws-0.0.6/
+-rw-r--r--   0 ross       (501) staff       (20)     1072 2024-01-24 10:16:13.000000 emerald_hws-0.0.6/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-15 10:10:58.354632 emerald_hws-0.0.6/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)       84 2024-01-24 10:15:13.000000 emerald_hws-0.0.6/README.md
+-rw-r--r--   0 ross       (501) staff       (20)      824 2024-04-15 10:10:04.000000 emerald_hws-0.0.6/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-15 10:10:58.355666 emerald_hws-0.0.6/setup.cfg
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.344481 emerald_hws-0.0.6/src/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.347910 emerald_hws-0.0.6/src/emerald_hws/
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.352689 emerald_hws-0.0.6/src/emerald_hws/__assets__/
+-rw-r--r--   0 ross       (501) staff       (20)     1424 2024-01-23 10:06:20.000000 emerald_hws-0.0.6/src/emerald_hws/__assets__/SFSRootCAG2.pem
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-01-24 10:24:29.000000 emerald_hws-0.0.6/src/emerald_hws/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)    12051 2024-04-15 10:07:58.000000 emerald_hws-0.0.6/src/emerald_hws/emeraldhws.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 10:10:58.353568 emerald_hws-0.0.6/src/emerald_hws.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)      694 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      327 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)       22 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       12 2024-04-15 10:10:58.000000 emerald_hws-0.0.6/src/emerald_hws.egg-info/top_level.txt
```

### Comparing `emerald_hws-0.0.5/LICENSE` & `emerald_hws-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.5/PKG-INFO` & `emerald_hws-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `emerald_hws-0.0.5/pyproject.toml` & `emerald_hws-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "emerald_hws"
-version = "0.0.5"
+version = "0.0.6"
 dependencies = [
   "boto3",
   "AWSIoTPythonSDK"
 ]
 authors = [
   { name="Ross Williamson", email="ross@inertia.net.nz" },
 ]
```

### Comparing `emerald_hws-0.0.5/src/emerald_hws/__assets__/SFSRootCAG2.pem` & `emerald_hws-0.0.6/src/emerald_hws/__assets__/SFSRootCAG2.pem`

 * *Files identical despite different names*

### Comparing `emerald_hws-0.0.5/src/emerald_hws/emeraldhws.py` & `emerald_hws-0.0.6/src/emerald_hws/emeraldhws.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         """
 
         self.email = email
         self.password = password
         self.token = ""
         self.properties = {}
         self.logger = logging.getLogger()
-        self.logger.setLevel(logging.DEBUG)
 
     def getLoginToken(self):
         """ Performs an API request to get a token from the API
         """
         url = "https://api.emerald-ems.com.au/api/v1/customer/sign-in"
 
         payload = {
@@ -118,15 +117,15 @@
         myAWSIoTMQTTClient.configureOfflinePublishQueueing(-1)  # Infinite offline Publish queueing
         myAWSIoTMQTTClient.configureDrainingFrequency(2)  # Draining: 2 Hz
         myAWSIoTMQTTClient.configureConnectDisconnectTimeout(10)  # 10 sec
         myAWSIoTMQTTClient.configureMQTTOperationTimeout(10)  # 10 sec
         myAWSIoTMQTTClient.onOffline = self.on_offline
         myAWSIoTMQTTClient.onOnline = self.on_online
         # Connect and subscribe to AWS IoT
-        myAWSIoTMQTTClient.connect()
+        myAWSIoTMQTTClient.connect(keepAliveIntervalSecond=60)
 
         self.myAWSIoTMQTTClient = myAWSIoTMQTTClient
 
     def mqttDecodeUpdate(self, topic, payload):
         """ Attempt to decode a received MQTT message and direct appropriately
         :param topic: MQTT topic
         :param payload: MQTT payload
```

### Comparing `emerald_hws-0.0.5/src/emerald_hws.egg-info/PKG-INFO` & `emerald_hws-0.0.6/src/emerald_hws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emerald_hws
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to manipulate and monitor Emerald Heat Pump Hot Water Systems
 Author-email: Ross Williamson <ross@inertia.net.nz>
 Project-URL: Homepage, https://github.com/ross-w/emerald_hws_py
 Project-URL: Bug Tracker, https://github.com/ross-w/emerald_hws_py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

