# Comparing `tmp/easy_utils_dev-2.9.tar.gz` & `tmp/easy_utils_dev-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_utils_dev-2.9.tar", last modified: Mon Apr 15 06:13:06 2024, max compression
+gzip compressed data, was "easy_utils_dev-2.9.1.tar", last modified: Mon Apr 15 07:00:54 2024, max compression
```

## Comparing `easy_utils_dev-2.9.tar` & `easy_utils_dev-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 06:13:06.959288 easy_utils_dev-2.9/
--rw-rw-rw-   0        0        0      172 2024-04-15 06:13:06.953223 easy_utils_dev-2.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 06:13:06.885606 easy_utils_dev-2.9/easy_utils_dev/
--rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9/easy_utils_dev/EasySsh.py
--rw-rw-rw-   0        0        0     2837 2024-01-17 00:38:30.000000 easy_utils_dev-2.9/easy_utils_dev/Events.py
--rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9/easy_utils_dev/__init__.py
--rw-rw-rw-   0        0        0    15032 2024-04-07 14:58:42.000000 easy_utils_dev-2.9/easy_utils_dev/cplib.py
--rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9/easy_utils_dev/custom_env.py
--rw-rw-rw-   0        0        0     7412 2024-04-15 06:10:21.000000 easy_utils_dev-2.9/easy_utils_dev/debugger.py
--rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9/easy_utils_dev/encryptor.py
--rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9/easy_utils_dev/keycloakapi.py
--rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9/easy_utils_dev/lralib.py
--rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.9/easy_utils_dev/ne1830PSS.py
--rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9/easy_utils_dev/optics_utils.py
--rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9/easy_utils_dev/simple_sqlite.py
--rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9/easy_utils_dev/uiserver.py
--rw-rw-rw-   0        0        0     3144 2024-04-15 05:45:40.000000 easy_utils_dev-2.9/easy_utils_dev/utils.py
--rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9/easy_utils_dev/wsnoclib.py
--rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9/easy_utils_dev/wsselib.py
-drwxrwxrwx   0        0        0        0 2024-04-15 06:13:06.948120 easy_utils_dev-2.9/easy_utils_dev.egg-info/
--rw-rw-rw-   0        0        0      172 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      633 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 06:13:06.000000 easy_utils_dev-2.9/easy_utils_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 06:13:06.959722 easy_utils_dev-2.9/setup.cfg
--rw-rw-rw-   0        0        0      315 2024-04-15 06:13:03.000000 easy_utils_dev-2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:00:54.094744 easy_utils_dev-2.9.1/
+-rw-rw-rw-   0        0        0      174 2024-04-15 07:00:54.089733 easy_utils_dev-2.9.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 07:00:54.062961 easy_utils_dev-2.9.1/easy_utils_dev/
+-rw-rw-rw-   0        0        0     3186 2024-03-11 19:01:52.000000 easy_utils_dev-2.9.1/easy_utils_dev/EasySsh.py
+-rw-rw-rw-   0        0        0     2978 2024-04-15 06:57:41.000000 easy_utils_dev-2.9.1/easy_utils_dev/Events.py
+-rw-rw-rw-   0        0        0      389 2024-04-07 14:14:30.000000 easy_utils_dev-2.9.1/easy_utils_dev/__init__.py
+-rw-rw-rw-   0        0        0    15032 2024-04-07 14:58:42.000000 easy_utils_dev-2.9.1/easy_utils_dev/cplib.py
+-rw-rw-rw-   0        0        0     1530 2024-01-17 11:32:08.000000 easy_utils_dev-2.9.1/easy_utils_dev/custom_env.py
+-rw-rw-rw-   0        0        0     8577 2024-04-15 07:00:14.000000 easy_utils_dev-2.9.1/easy_utils_dev/debugger.py
+-rw-rw-rw-   0        0        0     2100 2024-01-16 23:20:29.000000 easy_utils_dev-2.9.1/easy_utils_dev/encryptor.py
+-rw-rw-rw-   0        0        0     7170 2024-04-05 20:43:02.000000 easy_utils_dev-2.9.1/easy_utils_dev/keycloakapi.py
+-rw-rw-rw-   0        0        0     7942 2024-04-07 14:50:44.000000 easy_utils_dev-2.9.1/easy_utils_dev/lralib.py
+-rw-rw-rw-   0        0        0    33425 2024-04-04 14:35:28.000000 easy_utils_dev-2.9.1/easy_utils_dev/ne1830PSS.py
+-rw-rw-rw-   0        0        0      968 2024-01-16 23:11:29.000000 easy_utils_dev-2.9.1/easy_utils_dev/optics_utils.py
+-rw-rw-rw-   0        0        0     4553 2024-01-17 11:25:31.000000 easy_utils_dev-2.9.1/easy_utils_dev/simple_sqlite.py
+-rw-rw-rw-   0        0        0     2176 2024-04-02 04:54:18.000000 easy_utils_dev-2.9.1/easy_utils_dev/uiserver.py
+-rw-rw-rw-   0        0        0     3144 2024-04-15 05:45:40.000000 easy_utils_dev-2.9.1/easy_utils_dev/utils.py
+-rw-rw-rw-   0        0        0     9538 2024-04-02 06:13:17.000000 easy_utils_dev-2.9.1/easy_utils_dev/wsnoclib.py
+-rw-rw-rw-   0        0        0     7984 2024-04-04 18:33:00.000000 easy_utils_dev-2.9.1/easy_utils_dev/wsselib.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:00:54.086737 easy_utils_dev-2.9.1/easy_utils_dev.egg-info/
+-rw-rw-rw-   0        0        0      174 2024-04-15 07:00:53.000000 easy_utils_dev-2.9.1/easy_utils_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      633 2024-04-15 07:00:53.000000 easy_utils_dev-2.9.1/easy_utils_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:00:53.000000 easy_utils_dev-2.9.1/easy_utils_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 07:00:53.000000 easy_utils_dev-2.9.1/easy_utils_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 07:00:53.000000 easy_utils_dev-2.9.1/easy_utils_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:00:54.095737 easy_utils_dev-2.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      317 2024-04-15 07:00:19.000000 easy_utils_dev-2.9.1/setup.py
```

### Comparing `easy_utils_dev-2.9/easy_utils_dev/EasySsh.py` & `easy_utils_dev-2.9.1/easy_utils_dev/EasySsh.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/Events.py` & `easy_utils_dev-2.9.1/easy_utils_dev/Events.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,19 @@
           # Global environment to store event emitters
         
         setupEnvironment( 'event_emitter' )
 
         env['event_emitter'][id] = self  # Register the event emitter in the global environment
         self.env = env['event_emitter'][id]  # Reference to the event emitter in the global environment
 
+    def isEventSubscribed(self, event):
+        if event in list(self.listeners.keys()) :
+            return True
+        return False
+
     def addEventListener(self, event, callback):
         """
         Adds an event listener for the specified event.
 
         Parameters:
         - event: Name of the event.
         - callback: Callback function to be executed when the event is triggered.
```

### Comparing `easy_utils_dev-2.9/easy_utils_dev/cplib.py` & `easy_utils_dev-2.9.1/easy_utils_dev/cplib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/custom_env.py` & `easy_utils_dev-2.9.1/easy_utils_dev/custom_env.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/debugger.py` & `easy_utils_dev-2.9.1/easy_utils_dev/debugger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging , os , inspect
 from datetime import datetime
 from logging.handlers import RotatingFileHandler
 from .utils import getRandomKey, convert_bytes_to_kb , convert_bytes_to_mb , convert_mb_to_bytes 
 from .custom_env import custom_env , setupEnvironment
 import json , glob
+from .Events import EventEmitter
 
 def setGlobalHomePath( path ) :
     env = custom_env()
     env['debugger_homepath'] = path
     if not os.path.exists( path ) :
         print(f'Warning: Provided path does not exist. Path is {path}')
 
@@ -16,41 +17,58 @@
     env['debugger_on_screen'] = on_screen
 
 class DEBUGGER:
     def __init__(self, name, level='info', onscreen=True,log_rotation=3,homePath=None,id=getRandomKey(9) , global_debugger=None,disable_log_write=False):
         env = custom_env()
         env['debugger_on_screen'] = True
         self.env = env
+        self.events = EventEmitter()
         self.logger = logging.getLogger(name)
         self.set_level(level)
         self.LOG_SIZE_THRESHOLD_IN_BYTES = 10 * 1024 * 1024
         self.BACKUP_COUNT = log_rotation
         self.homePath = homePath
         self.onScreen= onscreen
         self.id = id
         self.how_many_times_write= 0
         self.stream_service = None
         self.name = name
+        self.rotate_disabled=False
         self.log_iterations=0
         self.log_iterations_threshold = 200
         self.global_debugger = global_debugger
         self.type = "CUSTOM_DEBUGGER"
         setupEnvironment( 'debugger' )
         env['debugger'][id] = self
-        path = self.homepath(homePath)
         f = f"[%(asctime)s]-[{name}]-[%(levelname)s]: %(message)s"
-        formatter = logging.Formatter(f , datefmt='%Y-%m-%d %H:%M:%S' )
-        self._file_handler_class = file_handler = RotatingFileHandler(path ,  maxBytes=self.LOG_SIZE_THRESHOLD_IN_BYTES , backupCount=self.BACKUP_COUNT )
-        self.file_handler = file_handler.setFormatter(formatter)
-        self.logger.addHandler(file_handler)
+        self.formatter = logging.Formatter(f , datefmt='%Y-%m-%d %H:%M:%S' )
+        path = self.homepath(homePath)
+        self.file_handler_class = None
+        self.file_handler_class = self.createRotateFileHandler(path)
         self.logger.addFilter(self.on_log )
         self._disable_log_write = disable_log_write
         if onscreen : self.enable_print()
         elif not onscreen : self.disable_print()
 
+
+    def disable_rotate(self) :
+        self.rotate_disabled = True
+
+    def enable_rotate(self) :
+        self.rotate_disabled = False
+
+    def createRotateFileHandler( self , path ) :
+        old = self.file_handler_class 
+        if old :
+            self.logger.removeHandler(old)
+        file_handler = RotatingFileHandler(path ,  maxBytes=self.LOG_SIZE_THRESHOLD_IN_BYTES , backupCount=self.BACKUP_COUNT )
+        self.file_handler= file_handler.setFormatter(self.formatter)
+        self.logger.addHandler(file_handler)
+        return file_handler
+
     def update_log_iterantions_threshold(self,threshold : int ):
         '''
         set value when rotation should be checked. when every on_log function called.
         by default rotation will be checked every 200 on_log function call.
         '''
         self.log_iterations_threshold = threshold
 
@@ -60,14 +78,25 @@
         logger must be debugger class.
         '''
         if logger.type != 'CUSTOM_DEBUGGER' :
             raise Exception(f'Invalid logger type. must pass debugger class.')
         self.global_debugger = logger
 
 
+    def getStreamServiceUrlPath(self) :
+        return self.streampath
+
+    def getStreamService(self) :
+        return self.stream_service
+
+    def isStreamServiceAvailable(self) :
+        if self.stream_service :
+            return True
+        return False
+
     def addStreamService( self , socketio , streampath='/debugger/stream/log' ) :
         """
         This function takes a live socketio server. it emit the log message using default path which is /debugger/stream/log
         """
         self.stream_service = socketio
         self.streampath = streampath
         
@@ -85,37 +114,39 @@
         if handler.shouldRollover(record) :
             handler.doRollover()
             self.log_iterations = 0
 
     def on_log(self , record) :
         if not self._disable_log_write and not self.stream_service and not self.onScreen and not self.env['debugger_on_screen'] :
             return
-        if self.log_iterations > self.log_iterations_threshold :
-            self.manage_file_rotation(record)
-        else :
-            self.log_iterations += 1
+        if self.rotate_disabled :
+            if self.log_iterations > self.log_iterations_threshold:
+                self.manage_file_rotation(record)
+            else :
+                self.log_iterations += 1
         d = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
         l = f"[{d}] - [{self.name}] - [{record.levelname}]: {record.getMessage()}"
 
         if not self._disable_log_write :
             with open(self.homePath , 'a+') as f :
                 f.write(f"{l}\n")
-        if self.stream_service is not None :
-            self.stream_service.emit( self.streampath , json.dumps({
+        if self.isStreamServiceAvailable() :
+            self.stream_service.emit( self.getStreamServiceUrlPath() , json.dumps({
                 'message' : l ,
                 'level' : record.levelname ,
                 'msg' : record.getMessage(),
                 'date' : d ,
-                'id' : self.id
+                'id' : self.id,
+                'formate' : 'json'
             }))
         if self.onScreen and self.env['debugger_on_screen'] == True :
             print(l)
 
     def get_rotate_handler(self) :
-        return self._file_handler_class
+        return self.file_handler_class
             
     def change_log_size(self, size) -> bool:
         '''
         change the size of each log file rotation.
         default is 10M
         size should be passed as MB
         '''
@@ -144,15 +175,22 @@
     def enable_print(self) :
         self.onScreen = True
 
     def disable_print(self) : 
         self.onScreen = False
 
     def changeHomePath( self , path ) :
-        self.homePath = path
+        p = self.homepath(path)
+        self.file_handler_class = self.createRotateFileHandler(p)
+
+    def isGlobalDebuggerDefined(self) :
+        if self.global_debugger :
+            return True
+        else :
+            return False
 
     def set_level(self, level : str):
         if 'info' in level.lower() : lvl = logging.INFO
         elif 'warn' in level.lower() : lvl = logging.WARNING
         elif 'warning' in level.lower() : lvl = logging.WARNING
         elif 'critical' in level.lower() : lvl = logging.CRITICAL
         elif 'debug' in level.lower() : lvl = logging.DEBUG
@@ -161,29 +199,29 @@
         self.logger.setLevel(lvl)
 
     def get_logger(self) : 
         return self.logger
 
     def info(self, message):
         self.logger.info(message)
-        if self.global_debugger : 
+        if self.isGlobalDebuggerDefined() : 
             self.global_debugger.info(message)
 
     def debug(self, message):
         self.logger.debug(message)
-        if self.global_debugger : 
+        if self.isGlobalDebuggerDefined() : 
             self.global_debugger.debug(message)
 
     def warning(self, message):
         self.logger.warning(message)
-        if self.global_debugger : 
+        if self.isGlobalDebuggerDefined() : 
             self.global_debugger.warning(message)
 
     def error(self, message):
         self.logger.error(message)
-        if self.global_debugger : 
+        if self.isGlobalDebuggerDefined() : 
             self.global_debugger.error(message)
 
     def critical(self, message):
         self.logger.critical(message)
-        if self.global_debugger : 
+        if self.isGlobalDebuggerDefined() : 
             self.global_debugger.critical(message)
```

### Comparing `easy_utils_dev-2.9/easy_utils_dev/encryptor.py` & `easy_utils_dev-2.9.1/easy_utils_dev/encryptor.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/keycloakapi.py` & `easy_utils_dev-2.9.1/easy_utils_dev/keycloakapi.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/lralib.py` & `easy_utils_dev-2.9.1/easy_utils_dev/lralib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/ne1830PSS.py` & `easy_utils_dev-2.9.1/easy_utils_dev/ne1830PSS.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/optics_utils.py` & `easy_utils_dev-2.9.1/easy_utils_dev/optics_utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/simple_sqlite.py` & `easy_utils_dev-2.9.1/easy_utils_dev/simple_sqlite.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/uiserver.py` & `easy_utils_dev-2.9.1/easy_utils_dev/uiserver.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/utils.py` & `easy_utils_dev-2.9.1/easy_utils_dev/utils.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/wsnoclib.py` & `easy_utils_dev-2.9.1/easy_utils_dev/wsnoclib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev/wsselib.py` & `easy_utils_dev-2.9.1/easy_utils_dev/wsselib.py`

 * *Files identical despite different names*

### Comparing `easy_utils_dev-2.9/easy_utils_dev.egg-info/SOURCES.txt` & `easy_utils_dev-2.9.1/easy_utils_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

