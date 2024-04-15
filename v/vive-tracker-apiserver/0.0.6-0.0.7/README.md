# Comparing `tmp/vive-tracker-apiserver-0.0.6.tar.gz` & `tmp/vive-tracker-apiserver-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vive-tracker-apiserver/vive-tracker-apiserver/dist/.tmp-ama7mei_/vive-tracker-apiserver-0.0.6.tar", last modified: Fri May 12 11:58:00 2023, max compression
+gzip compressed data, was "/home/runner/work/vive-tracker-apiserver/vive-tracker-apiserver/dist/.tmp-fbsv462d/vive-tracker-apiserver-0.0.7.tar", last modified: Mon Apr 15 12:46:46 2024, max compression
```

## Comparing `vive-tracker-apiserver-0.0.6.tar` & `vive-tracker-apiserver-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/tests/test_minimal.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/tests/test_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/client/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/test_visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/common/
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/common/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/grpc/tracker_packet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/controller_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/tracker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13434 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/triad_openvr.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/udp_emitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/vr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 11:57:47.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/vr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 11:58:00.000000 vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/tests/test_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/tests/test_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7159 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/client/Client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/list_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/test_visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/common/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/common/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/grpc/tracker_packet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10711 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/controller_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/tracker_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13434 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/triad_openvr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/udp_emitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/vr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:36.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/vr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 12:46:46.000000 vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/top_level.txt
```

### Comparing `vive-tracker-apiserver-0.0.6/PKG-INFO` & `vive-tracker-apiserver-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vive-tracker-apiserver
-Version: 0.0.6
+Version: 0.0.7
 Summary: Vive Tracker APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Vive Tracker APIServer
```

### Comparing `vive-tracker-apiserver-0.0.6/README.md` & `vive-tracker-apiserver-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/setup.py` & `vive-tracker-apiserver-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./vive_tracker_apiserver.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="vive-tracker-apiserver",
-    version="0.0.6",
+    version="0.0.7",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="Vive Tracker APIServer",
     packages=find_packages() + ["vive_tracker_apiserver.third_party.triad_openvr." + pkg for pkg in find_packages('vive_tracker_apiserver.third_party.triad_openvr')] + [
         'vive_tracker_apiserver.third_party.triad_openvr'],
     python_requires=">=3.7",
     install_requires=requires,
```

### Comparing `vive-tracker-apiserver-0.0.6/tests/test_minimal.py` & `vive-tracker-apiserver-0.0.7/tests/test_minimal.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import time
 from vive_tracker_apiserver.client import Client
 
 def get_description(data):
     return str([f'id:{item.meta.uid} x: {item.pos_x:.2f} y: {item.pos_y:.2f} z: {item.pos_z:.2f}' for item in data.payload])
 
-def test_server():
+def test():
     endpoint = "localhost:8080"
 
     c = Client(endpoint)
     response = c.get_group()
     print("GetTrackerGroup client received: " + str(response))
 
     stream = c.open_group_stream()
@@ -21,8 +21,8 @@
                 time.sleep(0.05)
                 continue
             print('\r'+get_description(data), end="")
     except KeyboardInterrupt as e:
         stream.close()
 
 if __name__ == '__main__':
-    test_server()
+    test()
```

### Comparing `vive-tracker-apiserver-0.0.6/tests/test_tracker.py` & `vive-tracker-apiserver-0.0.7/tests/test_tracker.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 if len(sys.argv) == 1:
     interval = 1/250
 elif len(sys.argv) == 2:
     interval = 1/float(sys.argv[1])
 else:
     print("Invalid number of arguments")
     interval = False
-    
+
+print(list(v.devices.keys()))
 if interval:
     while(True):
         start = time.time()
         txt = ""
 
         res = v.devices["tracker_1"].get_pose_euler()
         if res is not None:
```

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/main.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/main.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/apiserver/server.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/apiserver/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -144,14 +144,49 @@
 
             else:
                 if meta['index'] > desired_index:
                     logger.warning('slow client operation detected')
                 last_index = meta['index']
                 yield create_tracker_single_packet(meta, payload)
 
+    def StartRecording(self,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        logger.info(f"StartRecording: {target}")
+        err = self.app.start_recording(tag=target.tag)
+        if err is not None:
+            return pb2.RecordingResponse(started=False, error=str(err))
+        else:
+            return pb2.RecordingResponse(started=True, error="")
+
+
+    def StopRecording(self,
+                      target,
+                      options=(),
+                      channel_credentials=None,
+                      call_credentials=None,
+                      insecure=False,
+                      compression=None,
+                      wait_for_ready=None,
+                      timeout=None,
+                      metadata=None):
+        logger.info(f"StopRecording: {target}")
+        err = self.app.stop_recording()
+        if err is not None:
+            return pb2.RecordingResponse(started=False, error=str(err))
+        else:
+            return pb2.RecordingResponse(started=True, error="")
+
     # def GetFIFOStatus(self, request: pb2.ForceGetFIFOStatusRequest, context):
     #     return pb2.ForceStatusResponse(status=self.app.fifo_status)
     #
     # def SetFIFOStatus(self, request: pb2.ForceSetFIFOStatusRequest, context):
     #     logger.info(f"SetFIFOStatus: {request}")
     #     if request.status:
     #         err = self.app.start_fifo()
```

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/client/Client.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/client/Client.py`

 * *Files 14% similar despite different names*

```diff
@@ -43,10 +43,20 @@
     def open_group_stream(self):
         return ClientStream(
             self.stub.GetTrackerGroupStream(
                 pb2.TrackerRequest(uid="")
             )
         )
 
+    def start_recording(self, tag: str):
+        return self.stub.StartRecording(
+            pb2.RecordingRequest(tag=tag)
+        )
+
+    def stop_recording(self):
+        return self.stub.StopRecording(
+            pb2.RecordingRequest(tag="")
+        )
+
 
 def get_client(endpoint: str) -> Client:
     return Client(endpoint)
```

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/configure.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/configure.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/test_server.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/test_server.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/cmd/test_visualize.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/cmd/test_visualize.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/common/Config.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/common/Config.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/grpc/tracker_packet_pb2.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/grpc/tracker_packet_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,25 +9,29 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14tracker_packet.proto\x12\x08protocol\"\x1d\n\x0eTrackerRequest\x12\x0b\n\x03uid\x18\x02 \x01(\t\"S\n\x13TrackerMetaResponse\x12\r\n\x05valid\x18\x01 \x01(\x08\x12\r\n\x05index\x18\x02 \x01(\x04\x12\x11\n\tsys_ts_ns\x18\x03 \x01(\x04\x12\x0b\n\x03uid\x18\x0b \x01(\t\"\xad\x01\n\x15TrackerSingleResponse\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.protocol.TrackerMetaResponse\x12\r\n\x05pos_x\x18\x04 \x01(\x01\x12\r\n\x05pos_y\x18\x05 \x01(\x01\x12\r\n\x05pos_z\x18\x06 \x01(\x01\x12\r\n\x05rot_w\x18\x07 \x01(\x01\x12\r\n\x05rot_x\x18\x08 \x01(\x01\x12\r\n\x05rot_y\x18\t \x01(\x01\x12\r\n\x05rot_z\x18\n \x01(\x01\"u\n\x14TrackerGroupResponse\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.protocol.TrackerMetaResponse\x12\x30\n\x07payload\x18\x02 \x03(\x0b\x32\x1f.protocol.TrackerSingleResponse2\xe0\x02\n\x0eTrackerService\x12M\n\x0fGetTrackerGroup\x12\x18.protocol.TrackerRequest\x1a\x1e.protocol.TrackerGroupResponse\"\x00\x12U\n\x15GetTrackerGroupStream\x12\x18.protocol.TrackerRequest\x1a\x1e.protocol.TrackerGroupResponse\"\x00\x30\x01\x12O\n\x10GetTrackerSingle\x12\x18.protocol.TrackerRequest\x1a\x1f.protocol.TrackerSingleResponse\"\x00\x12W\n\x16GetTrackerSingleStream\x12\x18.protocol.TrackerRequest\x1a\x1f.protocol.TrackerSingleResponse\"\x00\x30\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14tracker_packet.proto\x12\x08protocol\"\x1d\n\x0eTrackerRequest\x12\x0b\n\x03uid\x18\x01 \x01(\t\"\x1f\n\x10RecordingRequest\x12\x0b\n\x03tag\x18\x01 \x01(\t\"3\n\x11RecordingResponse\x12\x0f\n\x07started\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"S\n\x13TrackerMetaResponse\x12\r\n\x05valid\x18\x01 \x01(\x08\x12\r\n\x05index\x18\x02 \x01(\x04\x12\x11\n\tsys_ts_ns\x18\x03 \x01(\x04\x12\x0b\n\x03uid\x18\x04 \x01(\t\"\xad\x01\n\x15TrackerSingleResponse\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.protocol.TrackerMetaResponse\x12\r\n\x05pos_x\x18\x02 \x01(\x01\x12\r\n\x05pos_y\x18\x03 \x01(\x01\x12\r\n\x05pos_z\x18\x04 \x01(\x01\x12\r\n\x05rot_w\x18\x05 \x01(\x01\x12\r\n\x05rot_x\x18\x06 \x01(\x01\x12\r\n\x05rot_y\x18\x07 \x01(\x01\x12\r\n\x05rot_z\x18\x08 \x01(\x01\"u\n\x14TrackerGroupResponse\x12+\n\x04meta\x18\x01 \x01(\x0b\x32\x1d.protocol.TrackerMetaResponse\x12\x30\n\x07payload\x18\x02 \x03(\x0b\x32\x1f.protocol.TrackerSingleResponse2\xf9\x03\n\x0eTrackerService\x12M\n\x0fGetTrackerGroup\x12\x18.protocol.TrackerRequest\x1a\x1e.protocol.TrackerGroupResponse\"\x00\x12U\n\x15GetTrackerGroupStream\x12\x18.protocol.TrackerRequest\x1a\x1e.protocol.TrackerGroupResponse\"\x00\x30\x01\x12O\n\x10GetTrackerSingle\x12\x18.protocol.TrackerRequest\x1a\x1f.protocol.TrackerSingleResponse\"\x00\x12W\n\x16GetTrackerSingleStream\x12\x18.protocol.TrackerRequest\x1a\x1f.protocol.TrackerSingleResponse\"\x00\x30\x01\x12K\n\x0eStartRecording\x12\x1a.protocol.RecordingRequest\x1a\x1b.protocol.RecordingResponse\"\x00\x12J\n\rStopRecording\x12\x1a.protocol.RecordingRequest\x1a\x1b.protocol.RecordingResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tracker_packet_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _TRACKERREQUEST._serialized_start=34
   _TRACKERREQUEST._serialized_end=63
-  _TRACKERMETARESPONSE._serialized_start=65
-  _TRACKERMETARESPONSE._serialized_end=148
-  _TRACKERSINGLERESPONSE._serialized_start=151
-  _TRACKERSINGLERESPONSE._serialized_end=324
-  _TRACKERGROUPRESPONSE._serialized_start=326
-  _TRACKERGROUPRESPONSE._serialized_end=443
-  _TRACKERSERVICE._serialized_start=446
-  _TRACKERSERVICE._serialized_end=798
+  _RECORDINGREQUEST._serialized_start=65
+  _RECORDINGREQUEST._serialized_end=96
+  _RECORDINGRESPONSE._serialized_start=98
+  _RECORDINGRESPONSE._serialized_end=149
+  _TRACKERMETARESPONSE._serialized_start=151
+  _TRACKERMETARESPONSE._serialized_end=234
+  _TRACKERSINGLERESPONSE._serialized_start=237
+  _TRACKERSINGLERESPONSE._serialized_end=410
+  _TRACKERGROUPRESPONSE._serialized_start=412
+  _TRACKERGROUPRESPONSE._serialized_end=529
+  _TRACKERSERVICE._serialized_start=532
+  _TRACKERSERVICE._serialized_end=1037
 # @@protoc_insertion_point(module_scope)
```

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,24 @@
                 response_deserializer=tracker__packet__pb2.TrackerSingleResponse.FromString,
                 )
         self.GetTrackerSingleStream = channel.unary_stream(
                 '/protocol.TrackerService/GetTrackerSingleStream',
                 request_serializer=tracker__packet__pb2.TrackerRequest.SerializeToString,
                 response_deserializer=tracker__packet__pb2.TrackerSingleResponse.FromString,
                 )
+        self.StartRecording = channel.unary_unary(
+                '/protocol.TrackerService/StartRecording',
+                request_serializer=tracker__packet__pb2.RecordingRequest.SerializeToString,
+                response_deserializer=tracker__packet__pb2.RecordingResponse.FromString,
+                )
+        self.StopRecording = channel.unary_unary(
+                '/protocol.TrackerService/StopRecording',
+                request_serializer=tracker__packet__pb2.RecordingRequest.SerializeToString,
+                response_deserializer=tracker__packet__pb2.RecordingResponse.FromString,
+                )
 
 
 class TrackerServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetTrackerGroup(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -59,14 +69,26 @@
 
     def GetTrackerSingleStream(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def StartRecording(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def StopRecording(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_TrackerServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetTrackerGroup': grpc.unary_unary_rpc_method_handler(
                     servicer.GetTrackerGroup,
                     request_deserializer=tracker__packet__pb2.TrackerRequest.FromString,
                     response_serializer=tracker__packet__pb2.TrackerGroupResponse.SerializeToString,
@@ -82,14 +104,24 @@
                     response_serializer=tracker__packet__pb2.TrackerSingleResponse.SerializeToString,
             ),
             'GetTrackerSingleStream': grpc.unary_stream_rpc_method_handler(
                     servicer.GetTrackerSingleStream,
                     request_deserializer=tracker__packet__pb2.TrackerRequest.FromString,
                     response_serializer=tracker__packet__pb2.TrackerSingleResponse.SerializeToString,
             ),
+            'StartRecording': grpc.unary_unary_rpc_method_handler(
+                    servicer.StartRecording,
+                    request_deserializer=tracker__packet__pb2.RecordingRequest.FromString,
+                    response_serializer=tracker__packet__pb2.RecordingResponse.SerializeToString,
+            ),
+            'StopRecording': grpc.unary_unary_rpc_method_handler(
+                    servicer.StopRecording,
+                    request_deserializer=tracker__packet__pb2.RecordingRequest.FromString,
+                    response_serializer=tracker__packet__pb2.RecordingResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'protocol.TrackerService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -159,7 +191,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/protocol.TrackerService/GetTrackerSingleStream',
             tracker__packet__pb2.TrackerRequest.SerializeToString,
             tracker__packet__pb2.TrackerSingleResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def StartRecording(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/protocol.TrackerService/StartRecording',
+            tracker__packet__pb2.RecordingRequest.SerializeToString,
+            tracker__packet__pb2.RecordingResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def StopRecording(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/protocol.TrackerService/StopRecording',
+            tracker__packet__pb2.RecordingRequest.SerializeToString,
+            tracker__packet__pb2.RecordingResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/controller_test.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/controller_test.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/tracker_test.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/tracker_test.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/triad_openvr.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/triad_openvr.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver/third_party/triad_openvr/udp_emitter.py` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver/third_party/triad_openvr/udp_emitter.py`

 * *Files identical despite different names*

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/PKG-INFO` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vive-tracker-apiserver
-Version: 0.0.6
+Version: 0.0.7
 Summary: Vive Tracker APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Vive Tracker APIServer
```

### Comparing `vive-tracker-apiserver-0.0.6/vive_tracker_apiserver.egg-info/SOURCES.txt` & `vive-tracker-apiserver-0.0.7/vive_tracker_apiserver.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 tests/test_minimal.py
+tests/test_recording.py
 tests/test_tracker.py
 vive_tracker_apiserver/__init__.py
 vive_tracker_apiserver/__main__.py
 vive_tracker_apiserver.egg-info/PKG-INFO
 vive_tracker_apiserver.egg-info/SOURCES.txt
 vive_tracker_apiserver.egg-info/dependency_links.txt
 vive_tracker_apiserver.egg-info/requires.txt
@@ -13,18 +14,20 @@
 vive_tracker_apiserver/apiserver/app.py
 vive_tracker_apiserver/apiserver/main.py
 vive_tracker_apiserver/apiserver/server.py
 vive_tracker_apiserver/client/Client.py
 vive_tracker_apiserver/client/__init__.py
 vive_tracker_apiserver/cmd/__init__.py
 vive_tracker_apiserver/cmd/configure.py
+vive_tracker_apiserver/cmd/list_devices.py
 vive_tracker_apiserver/cmd/test_server.py
 vive_tracker_apiserver/cmd/test_visualize.py
 vive_tracker_apiserver/common/Config.py
 vive_tracker_apiserver/common/__init__.py
+vive_tracker_apiserver/common/functional.py
 vive_tracker_apiserver/grpc/__init__.py
 vive_tracker_apiserver/grpc/tracker_packet_pb2.py
 vive_tracker_apiserver/grpc/tracker_packet_pb2_grpc.py
 vive_tracker_apiserver/third_party/__init__.py
 vive_tracker_apiserver/third_party/triad_openvr/controller_test.py
 vive_tracker_apiserver/third_party/triad_openvr/tracker_test.py
 vive_tracker_apiserver/third_party/triad_openvr/triad_openvr.py
```

