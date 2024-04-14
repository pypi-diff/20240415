# Comparing `tmp/robothub-2.5.7.tar.gz` & `tmp/robothub-2.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robothub-2.5.7.tar", last modified: Fri Apr 12 22:56:08 2024, max compression
+gzip compressed data, was "robothub-2.5.8.tar", last modified: Sun Apr 14 22:55:18 2024, max compression
```

## Comparing `robothub-2.5.7.tar` & `robothub-2.5.8.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-12 22:55:46.000000 robothub-2.5.7/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-12 22:55:46.000000 robothub-2.5.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-12 22:56:08.306031 robothub-2.5.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-12 22:55:46.000000 robothub-2.5.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 22:56:08.306031 robothub-2.5.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-12 22:55:46.000000 robothub-2.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.298031 robothub-2.5.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.302031 robothub-2.5.7/src/robothub/
--rwxr-xr-x   0 runner    (1001) docker     (127)      629 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/application.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/frame_buffer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/live_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/live_view_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.302031 robothub-2.5.7/src/robothub/replay/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/capture_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/captures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/replay_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    32613 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/replay_camera.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/replay/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/src/robothub/robothub_core_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_event_typechecks.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_stop_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/app.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/communicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/robothub_core_wrapper/streams.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-12 22:55:46.000000 robothub-2.5.7/src/robothub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/src/robothub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 22:56:08.000000 robothub-2.5.7/src/robothub.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:56:08.306031 robothub-2.5.7/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:55:46.000000 robothub-2.5.7/tests/test_callback.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:55:46.000000 robothub-2.5.7/tests/test_hub_camera.py
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:55:46.000000 robothub-2.5.7/tests/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1065 2024-04-14 22:55:02.000000 robothub-2.5.8/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (127)       35 2024-04-14 22:55:02.000000 robothub-2.5.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-14 22:55:18.251026 robothub-2.5.8/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)      942 2024-04-14 22:55:02.000000 robothub-2.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:55:18.251026 robothub-2.5.8/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1278 2024-04-14 22:55:02.000000 robothub-2.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.243026 robothub-2.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.247026 robothub-2.5.8/src/robothub/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      656 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5804 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9904 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/frame_buffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20074 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/live_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/live_view_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.247026 robothub-2.5.8/src/robothub/replay/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6151 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/capture_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/captures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/replay_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33998 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/replay_camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/replay/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/src/robothub/robothub_core_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_event_typechecks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_stop_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9383 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/app.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6437 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/communicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17407 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7115 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/robothub_core_wrapper/streams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-14 22:55:02.000000 robothub-2.5.8/src/robothub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/src/robothub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:55:18.000000 robothub-2.5.8/src/robothub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:18.251026 robothub-2.5.8/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:02.000000 robothub-2.5.8/tests/test_callback.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:02.000000 robothub-2.5.8/tests/test_hub_camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:55:02.000000 robothub-2.5.8/tests/test_manager.py
```

### Comparing `robothub-2.5.7/LICENSE` & `robothub-2.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/PKG-INFO` & `robothub-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.7
+Version: 2.5.8
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.7/README.md` & `robothub-2.5.8/README.md`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/setup.py` & `robothub-2.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 
 long_description = io.open('README.md', encoding='utf-8').read()
 
 setup(
     name='robothub',
-    version='2.5.7',
+    version='2.5.8',
     description='RobotHub integration library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.luxonis.com/',
     license='MIT',
     keywords='robothub camera robot hub connect agent depthai sdk',
     author='Luxonis',
```

### Comparing `robothub-2.5.7/src/robothub/__init__.py` & `robothub-2.5.8/src/robothub/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import robothub.decorators
 from robothub.application import *
 from robothub.events import *
 from robothub.frame_buffer import *
 from robothub.live_view import *
 from robothub.replay import *
 from robothub.utils import setup_logger
 
@@ -15,11 +16,11 @@
 
 # Import symbols from robothub_core and make them available under the robothub namespace
 try:
     import robothub_core as robothub
 except ImportError:
     import robothub.robothub_core_wrapper as robothub
 
-__version__ = "2.5.7"
+__version__ = "2.5.8"
 
 # Setup logging for the module
 # setup_logger(__name__)
```

### Comparing `robothub-2.5.7/src/robothub/application.py` & `robothub-2.5.8/src/robothub/application.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/events.py` & `robothub-2.5.8/src/robothub/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/frame_buffer.py` & `robothub-2.5.8/src/robothub/frame_buffer.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/live_view.py` & `robothub-2.5.8/src/robothub/live_view.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/live_view_utils.py` & `robothub-2.5.8/src/robothub/live_view_utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/replay/capture_manager.py` & `robothub-2.5.8/src/robothub/replay/capture_manager.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/replay/captures.py` & `robothub-2.5.8/src/robothub/replay/captures.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/replay/replay_camera.py` & `robothub-2.5.8/src/robothub/replay/replay_camera.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,21 +58,21 @@
     @abstractmethod
     def replay_is_running(self) -> bool:
         pass
 
 
 class ColorReplayCamera(ReplayCamera):
     def __init__(
-        self,
-        pipeline: dai.Pipeline,
-        fps: float,
-        src: str | List[str],
-        run_in_loop: bool = True,
-        start: Optional[int] = None,
-        end: Optional[int] = None,
+            self,
+            pipeline: dai.Pipeline,
+            fps: float,
+            src: str | List[str],
+            run_in_loop: bool = True,
+            start: Optional[int] = None,
+            end: Optional[int] = None,
     ):
         super().__init__()
         self.replay_camera_instances.append(self)
         self._stream_name: StreamName = StreamName(suffix=str(len(self.replay_camera_instances)))
 
         # NOTE(miha): Replay node inputs/outputs
         self._input_control: Optional[dai.Node.Input] = None
@@ -99,14 +99,16 @@
         self._run_in_loop = run_in_loop
         self._pipeline: dai.Pipeline = pipeline
 
         self._video_width: int = 1920
         self._video_height: int = 1080
         self._preview_width: int = 1280
         self._preview_height: int = 720
+        self._preview_crop_needed: Optional[bool] = None
+        self._preview_x_coords: Optional[tuple[int, int]] = None
         self._isp_width: int = 1920
         self._isp_height: int = 1080
         self._raw_width: int = 1280
         self._raw_height: int = 720
         self._still_width: int = 1280
         self._still_height: int = 720
         self._color_order: dai.ColorCameraProperties.ColorOrder = dai.ColorCameraProperties.ColorOrder.BGR
@@ -162,22 +164,39 @@
             self._still_queue = device.getInputQueue(name=self._stream_name.STILL)
         if self._preview is not None:
             self._preview_queue = device.getInputQueue(name=self._stream_name.PREVIEW)
 
         sequence_number = 0
         send_video_frames_start = time.time()
 
-        while rh.app_is_running and self.replay_is_running:
+        while rh.app_is_running() and self.replay_is_running:
             start = time.monotonic()
 
             # NOTE(miha): Returned frame is in BGR format
             frame = self._capture_manager.get_next_frame()
             if frame is None:
                 break
 
+            frame_h, frame_w = frame.shape[:2]
+            if self._isp_width > frame_w or self._isp_height > frame_h:
+                logging.error(f"ISP frame size ({self._isp_width}x{self._isp_height}) is bigger than source frame size ({frame_w}x{frame_h})."
+                              f" Setting ISP size to frame size.")
+                self._isp_width = frame_w
+                self._isp_height = frame_h
+            if self._raw_width > frame_w or self._raw_height > frame_h:
+                logging.error(f"RAW frame size ({self._raw_width}x{self._raw_height}) is bigger than source frame size ({frame_w}x{frame_h})."
+                              f" Setting RAW size to frame size.")
+                self._raw_width = frame_w
+                self._raw_height = frame_h
+            if self._video_width > frame_w or self._video_height > frame_h:
+                logging.error(f"VIDEO frame size ({self._video_width}x{self._video_height}) is bigger than source frame size ({frame_w}x{frame_h})."
+                              f" Setting VIDEO size to frame size.")
+                self._video_width = frame_w
+                self._video_height = frame_h
+
             timestamp: timedelta = timedelta(seconds=time.time() - send_video_frames_start)
 
             # NOTE(miha): Mock input control commands
             if self._input_control_queue is not None:
                 if self._input_control_queue.has():
                     ctrl: dai.CameraControl = self._input_control_queue.get()  # type: ignore
                     if ctrl.getCaptureStill():
@@ -191,77 +210,73 @@
                     width=self._raw_width,
                     height=self._raw_height,
                     type=dai.ImgFrame.Type.BGR888p,
                     sequence_number=sequence_number,
                     timestamp=timestamp,
                 )
                 self._raw_queue.send(raw_img_frame)
-
             if self._use_nv12_frame:
-                nv12_frame = BGR2YUV_NV12(frame)
+                isp_frame = cv2.resize(frame, (self._isp_width, self._isp_height))
+                isp_nv12_frame = BGR2YUV_NV12(isp_frame)
+                video_nv12_frame = None
                 if self._isp_queue is not None:
                     isp_img_frame = create_img_frame(
-                        data=nv12_frame,
+                        data=isp_nv12_frame,
                         width=self._isp_width,
                         height=self._isp_height,
                         type=dai.ImgFrame.Type.NV12,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
                     )
                     self._isp_queue.send(isp_img_frame)
                 if self._video_queue is not None:
+                    if self._video_width == self._isp_width and self._video_height == self._isp_height:
+                        video_nv12_frame = isp_nv12_frame
+                    else:
+                        video_frame = cv2.resize(frame, (self._video_width, self._video_height))
+                        video_nv12_frame = BGR2YUV_NV12(video_frame)
                     video_img_frame = create_img_frame(
-                        data=nv12_frame,
+                        data=video_nv12_frame,
                         width=self._video_width,
                         height=self._video_height,
                         type=dai.ImgFrame.Type.NV12,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
                     )
                     self._video_queue.send(video_img_frame)
                 if self._still_queue is not None and self._send_capture_still:
+                    if self._still_width == self._isp_width and self._still_height == self._isp_height:
+                        still_nv12_frame = isp_nv12_frame
+                    elif video_nv12_frame is not None and self._still_width == self._video_width and self._still_height == self._video_width:
+                        still_nv12_frame = video_nv12_frame
+                    else:
+                        still_frame = cv2.resize(frame, (self._still_width, self._still_height))
+                        still_nv12_frame = BGR2YUV_NV12(still_frame)
                     self._send_capture_still = False
                     video_img_frame = create_img_frame(
-                        data=nv12_frame,
+                        data=still_nv12_frame,
                         width=self._video_width,
                         height=self._video_height,
                         type=dai.ImgFrame.Type.NV12,
                         sequence_number=sequence_number,
                         timestamp=timestamp,
                     )
-                    self._still_queue.send(dai.ImgFrame())
+                    self._still_queue.send(video_img_frame)
 
             if self._preview_queue is not None:
-                preview_img_frame = create_img_frame(
-                    data=to_planar(frame, (self._preview_width, self._preview_height)),
-                    width=self._preview_width,
-                    height=self._preview_height,
-                    type=dai.ImgFrame.Type.BGR888p,
-                    sequence_number=sequence_number,
-                    timestamp=timestamp,
-                )
-                self._preview_queue.send(preview_img_frame)
+                preview_frame = frame
+                # crop when preview aspect ratio is different to video aspect ratio
+                if self._preview_crop_needed is None:
+                    self._find_if_preview_crop_needed()
+                if self._preview_crop_needed:
+                    if self._preview_x_coords is None:
+                        self._find_preview_crop_coords()
+                    preview_frame = frame[:, self._preview_x_coords[0]:self._preview_x_coords[1], :]
 
-            if self._isp_queue is not None:
-                self._isp_queue.send(dai.ImgFrame())
-            if self._video_queue is not None:
-                nv12_frame = BGR2YUV_NV12(frame)
-                video_img_frame = create_img_frame(
-                    data=nv12_frame,
-                    width=self._video_width,
-                    height=self._video_height,
-                    type=dai.ImgFrame.Type.NV12,
-                    sequence_number=sequence_number,
-                    timestamp=timestamp,
-                )
-                self._video_queue.send(video_img_frame)
-            if self._still_queue is not None:
-                self._still_queue.send(dai.ImgFrame())
-            if self._preview_queue is not None:
-                preview_frame = cv2.resize(frame, (self._preview_width, self._preview_height))
+                preview_frame = cv2.resize(preview_frame, (self._preview_width, self._preview_height))
                 preview_img_frame = create_img_frame(
                     data=to_planar(preview_frame, (self._preview_width, self._preview_height)),
                     width=self._preview_width,
                     height=self._preview_height,
                     type=dai.ImgFrame.Type.BGR888p,
                     sequence_number=sequence_number,
                     timestamp=timestamp,
@@ -291,14 +306,22 @@
             self._stop_event.set()
             self._thread.join()
 
     @property
     def replay_is_running(self) -> bool:
         return not self._stop_event.is_set()
 
+    def _find_if_preview_crop_needed(self):
+        self._preview_crop_needed = abs(self._video_width / self._video_height - self._preview_width / self._preview_height) > 0.1
+
+    def _find_preview_crop_coords(self):
+        new_width = self._video_height * self._preview_width // self._preview_height
+        x_middle = self._video_width // 2 + self._video_width % 2
+        self._preview_x_coords = (x_middle - new_width // 2, x_middle + new_width // 2 + new_width % 2)
+
     # NOTE(miha): Below are methods for ColorCamera class:
 
     def getBoardSocket(self) -> dai.CameraBoardSocket | None:
         return self._camera_socket
 
     def getCamId(self) -> int:
         raise NotImplementedError("This function is not yet implemented")
@@ -456,14 +479,16 @@
     def setPreviewKeepAspectRatio(self, keep: bool) -> None:
         raise NotImplementedError("This function is not yet implemented")
 
     def setPreviewNumFramesPool(self, arg0: int) -> None:
         raise NotImplementedError("This function is not yet implemented")
 
     def setPreviewSize(self, width: int, height: int) -> None:
+        if width > self._video_width or height > self._video_height:
+            raise ValueError(f"Preview size ({width}x{height}) is larger than video size ({self._video_width}x{self._video_height})")
         self.preview  # Ensures that 'preview' is inited (lazy loaded).
         self._preview_width = width
         self._preview_height = height
         self._nodes[self._stream_name.PREVIEW].setMaxDataSize(width * height * 3)
 
     # @overload
     # def setPreviewSize(self, width: int, height: int) -> None:
@@ -502,23 +527,15 @@
     def setVideoNumFramesPool(self, arg0: int) -> None:
         raise NotImplementedError("This function is not yet implemented")
 
     def setVideoSize(self, width: int, height: int) -> None:
         self.video  # Ensures that 'video' is inited (lazy loaded).
         self._video_width = width
         self._video_height = height
-        self._nodes[self._stream_name.VIDEO].setMaxDataSize(width * height * 3)
-
-    # @overload
-    # def setVideoSize(self, width: int, height: int) -> None:
-    #     raise NotImplementedError("This function is not yet implemented")
-    #
-    # @overload
-    # def setVideoSize(self, size: Tuple[int, int]) -> None:
-    #     raise NotImplementedError("This function is not yet implemented")
+        self._nodes[self._stream_name.VIDEO].setMaxDataSize(width * height * 3 // 2)
 
     def setWaitForConfigInput(self, wait: bool) -> None:
         raise NotImplementedError("This function is not yet implemented")
 
     @property
     def frameEvent(self) -> dai.Node.Output:
         raise NotImplementedError("This function is not yet implemented")
@@ -565,36 +582,24 @@
 
     @property
     def video(self) -> dai.Node.Output:
         if self._video is None:
             self._video = self._create_cam_output(self._pipeline, self._stream_name.VIDEO)
         return self._video
 
-    # @property
-    # def out(self) -> dai.Node.Output:
-    #     if self._out is None:
-    #         node_out = self._create_cam_output(self._pipeline, self._stream_name.GRAY)
-    #         manip = self._pipeline.createImageManip()
-    #         manip.setFrameType(dai.RawImgFrame.Type.RAW8)
-    #         manip.setResize(1280, 800)
-    #         manip.setKeepAspectRatio(False)
-    #         node_out.link(manip.inputImage)
-    #         self._out = manip.out
-    #     return self._out
-
 
 class MonoReplayCamera(ReplayCamera):
     def __init__(
-        self,
-        pipeline: dai.Pipeline,
-        fps: float,
-        src: str | List[str],
-        run_in_loop: bool = True,
-        start: Optional[int] = None,
-        end: Optional[int] = None,
+            self,
+            pipeline: dai.Pipeline,
+            fps: float,
+            src: str | List[str],
+            run_in_loop: bool = True,
+            start: Optional[int] = None,
+            end: Optional[int] = None,
     ):
         super().__init__()
         self.replay_camera_instances.append(self)
         self._stream_name: StreamName = StreamName(suffix=str(len(self.replay_camera_instances)))
 
         self._input_control: Optional[dai.Node.Input] = None
         self._raw: Optional[dai.Node.Output] = None
@@ -609,15 +614,15 @@
         self._end = start
         self._run_in_loop = run_in_loop
         self._pipeline: dai.Pipeline = pipeline
 
         self._raw_width: int = 1920
         self._raw_height: int = 1080
         self._out_width: int = 1280
-        self._out_height: int = 720
+        self._out_height: int = 800
         self._color_order: dai.ColorCameraProperties.ColorOrder = dai.ColorCameraProperties.ColorOrder.BGR
         self._interleaved = False
         self._camera_socket: dai.CameraBoardSocket | None = None
 
         self._stop_event = threading.Event()
         self._thread: Optional[threading.Thread] = None
 
@@ -652,15 +657,15 @@
             self._raw_queue = device.getInputQueue(name=self._stream_name.RAW)
         if self._out is not None:
             self._out_queue = device.getInputQueue(name=self._stream_name.GRAY)
 
         sequence_number = 0
         send_video_frames_start = time.time()
 
-        while rh.app_is_running and self.replay_is_running:
+        while rh.app_is_running() and self.replay_is_running:
             start = time.monotonic()
 
             # NOTE(miha): Returned frame is in BGR format
             frame = self._capture_manager.get_next_frame()
             if frame is None:
                 break
 
@@ -796,29 +801,24 @@
 
     @property
     def inputControl(self) -> dai.Node.Input:
         if self._input_control is None:
             self._input_control = self._create_cam_input(self._pipeline, self._stream_name.INPUT_CONTROL)
         return self._input_control
 
-    # @property
-    # def out(self) -> dai.Node.Output:
-    #     if self._out is None:
-    #         node_out = self._create_cam_output(self._pipeline, self._stream_name.GRAY)
-    #         manip = self._pipeline.createImageManip()
-    #         manip.setFrameType(dai.RawImgFrame.Type.RAW8)
-    #         manip.setResize(1280, 800)
-    #         manip.setKeepAspectRatio(False)
-    #         node_out.link(manip.inputImage)
-    #         self._out = manip.out
-    #     return self._out
     @property
     def out(self) -> dai.Node.Output:
         if self._out is None:
-            self._out = self._create_cam_output(self._pipeline, self._stream_name.GRAY)
+            node_out = self._create_cam_output(self._pipeline, self._stream_name.GRAY)
+            manip = self._pipeline.createImageManip()
+            manip.setFrameType(dai.RawImgFrame.Type.RAW8)
+            manip.setResize(self._out_width, self._out_height)
+            manip.setKeepAspectRatio(False)
+            node_out.link(manip.inputImage)
+            self._out = manip.out
         return self._out
 
     @property
     def raw(self) -> dai.Node.Output:
         if self._raw is None:
             self._raw = self._create_cam_output(self._pipeline, self._stream_name.RAW)
         return self._raw
```

### Comparing `robothub-2.5.7/src/robothub/replay/utils.py` & `robothub-2.5.8/src/robothub/replay/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/__init__.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/_event_typechecks.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/_event_typechecks.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/app.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/app.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/client.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/client.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/communicator.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/communicator.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/device.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/device.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/events.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/globals.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/globals.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/robothub_core_wrapper/streams.py` & `robothub-2.5.8/src/robothub/robothub_core_wrapper/streams.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub/utils.py` & `robothub-2.5.8/src/robothub/utils.py`

 * *Files identical despite different names*

### Comparing `robothub-2.5.7/src/robothub.egg-info/PKG-INFO` & `robothub-2.5.8/src/robothub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robothub
-Version: 2.5.7
+Version: 2.5.8
 Summary: RobotHub integration library
 Home-page: https://www.luxonis.com/
 Author: Luxonis
 Author-email: support@luxonis.com
 License: MIT
 Project-URL: Homepage, https://github.com/luxonis/robothub/
 Project-URL: Documentation, https://hub-docs.luxonis.com/
```

### Comparing `robothub-2.5.7/src/robothub.egg-info/SOURCES.txt` & `robothub-2.5.8/src/robothub.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/robothub/__init__.py
 src/robothub/application.py
+src/robothub/decorators.py
 src/robothub/events.py
 src/robothub/frame_buffer.py
 src/robothub/live_view.py
 src/robothub/live_view_utils.py
 src/robothub/types.py
 src/robothub/utils.py
 src/robothub.egg-info/PKG-INFO
```

