# Comparing `tmp/terminate_thread-0.0.1.tar.gz` & `tmp/terminate_thread-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terminate_thread-0.0.1.tar", last modified: Mon Apr 15 05:29:00 2024, max compression
+gzip compressed data, was "terminate_thread-0.0.2.tar", last modified: Mon Apr 15 06:16:18 2024, max compression
```

## Comparing `terminate_thread-0.0.1.tar` & `terminate_thread-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 05:29:00.362142 terminate_thread-0.0.1/
--rw-rw-rw-   0        0        0      794 2024-04-15 05:29:00.360606 terminate_thread-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-15 05:07:40.000000 terminate_thread-0.0.1/README.md
--rw-rw-rw-   0        0        0      755 2024-04-15 05:28:39.000000 terminate_thread-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 05:29:00.362754 terminate_thread-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 05:29:00.333503 terminate_thread-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-15 05:29:00.342766 terminate_thread-0.0.1/src/terminate_thread/
--rw-rw-rw-   0        0        0       70 2024-04-15 04:46:25.000000 terminate_thread-0.0.1/src/terminate_thread/__init__.py
--rw-rw-rw-   0        0        0     8704 2024-01-20 02:37:48.000000 terminate_thread-0.0.1/src/terminate_thread/libterminate.dll
--rw-rw-rw-   0        0        0    16152 2024-01-19 15:03:28.000000 terminate_thread-0.0.1/src/terminate_thread/libterminate.so
--rw-rw-rw-   0        0        0      717 2024-04-15 05:05:25.000000 terminate_thread-0.0.1/src/terminate_thread/terminate_thread.py
-drwxrwxrwx   0        0        0        0 2024-04-15 05:29:00.359615 terminate_thread-0.0.1/src/terminate_thread.egg-info/
--rw-rw-rw-   0        0        0      794 2024-04-15 05:29:00.000000 terminate_thread-0.0.1/src/terminate_thread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-15 05:29:00.000000 terminate_thread-0.0.1/src/terminate_thread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 05:29:00.000000 terminate_thread-0.0.1/src/terminate_thread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-15 05:29:00.000000 terminate_thread-0.0.1/src/terminate_thread.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 06:16:18.785111 terminate_thread-0.0.2/
+-rw-rw-rw-   0        0        0      827 2024-04-15 06:16:18.785111 terminate_thread-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2024-04-15 06:12:16.000000 terminate_thread-0.0.2/README.md
+-rw-rw-rw-   0        0        0      727 2024-04-15 06:15:47.000000 terminate_thread-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 06:16:18.785111 terminate_thread-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 06:16:18.738186 terminate_thread-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-15 06:16:18.769428 terminate_thread-0.0.2/src/terminate_thread/
+-rw-rw-rw-   0        0        0       81 2024-04-15 06:12:16.000000 terminate_thread-0.0.2/src/terminate_thread/__init__.py
+-rw-rw-rw-   0        0        0     8704 2024-04-15 06:12:16.000000 terminate_thread-0.0.2/src/terminate_thread/libterminate.dll
+-rw-rw-rw-   0        0        0    16152 2024-04-15 06:12:16.000000 terminate_thread-0.0.2/src/terminate_thread/libterminate.so
+-rw-rw-rw-   0        0        0     1127 2024-04-15 06:12:16.000000 terminate_thread-0.0.2/src/terminate_thread/terminate_thread.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:16:18.785111 terminate_thread-0.0.2/src/terminate_thread.egg-info/
+-rw-rw-rw-   0        0        0      827 2024-04-15 06:16:18.000000 terminate_thread-0.0.2/src/terminate_thread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-15 06:16:18.000000 terminate_thread-0.0.2/src/terminate_thread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:16:18.000000 terminate_thread-0.0.2/src/terminate_thread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-15 06:16:18.000000 terminate_thread-0.0.2/src/terminate_thread.egg-info/top_level.txt
```

### Comparing `terminate_thread-0.0.1/PKG-INFO` & `terminate_thread-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: terminate_thread
-Version: 0.0.1
+Version: 0.0.2
 Summary: terminate_thread
 Author-email: calm51 <calm51@protonmail.com>
 Project-URL: Homepage, https://github.com/calm51/terminate_thread
 Project-URL: Issues, https://github.com/calm51/terminate_thread/issues
 Keywords: terminate thread,kill thread,stop thread
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ```python3
 import threading
 import time
-from terminate_thread import terminate
+from terminate_thread import terminate, kill
 
 
 def thread_func1():
     n = 0
     while True:
         n += 1
         print(n, t)
         time.sleep(1)
 
 
 if __name__ == "__main__":
     t = threading.Thread(target=thread_func1, )
     t.start()
     time.sleep(2)
+
     terminate(t)
+    # or
+    kill(t)
+
     exit(0)
 
 
 ```
```

### Comparing `terminate_thread-0.0.1/src/terminate_thread/libterminate.dll` & `terminate_thread-0.0.2/src/terminate_thread/libterminate.dll`

 * *Files identical despite different names*

### Comparing `terminate_thread-0.0.1/src/terminate_thread/libterminate.so` & `terminate_thread-0.0.2/src/terminate_thread/libterminate.so`

 * *Files identical despite different names*

### Comparing `terminate_thread-0.0.1/src/terminate_thread/terminate_thread.py` & `terminate_thread-0.0.2/src/terminate_thread/terminate_thread.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,28 @@
 import ctypes
 import os
 import sys
 from threading import Thread
 
 
-def terminate(thread: Thread):
-    if thread.is_alive():
+def terminate(thread: Thread) -> None:
+    if isinstance(thread, Thread) and thread.is_alive():
         _lib.main(ctypes.c_longlong(thread._ident))
 
 
+def kill(thread: Thread) -> bool:
+    if isinstance(thread, Thread) and thread.is_alive():
+        # InterruptedError SystemExit
+        _ = ctypes.pythonapi.PyThreadState_SetAsyncExc(ctypes.c_long(thread._ident),
+                                                          ctypes.py_object(SystemExit)) == 1
+        if _: thread.join()
+        return _
+    return False
+
+
 def _find_lib():
     paths = [os.path.dirname(__file__),
              os.path.join(os.path.dirname(__file__), "terminate_thread", ),
              os.path.dirname(os.path.abspath(sys.argv[0])),
              os.getcwd(),
              ]
     for i in paths:
```

### Comparing `terminate_thread-0.0.1/src/terminate_thread.egg-info/PKG-INFO` & `terminate_thread-0.0.2/src/terminate_thread.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: terminate_thread
-Version: 0.0.1
+Version: 0.0.2
 Summary: terminate_thread
 Author-email: calm51 <calm51@protonmail.com>
 Project-URL: Homepage, https://github.com/calm51/terminate_thread
 Project-URL: Issues, https://github.com/calm51/terminate_thread/issues
 Keywords: terminate thread,kill thread,stop thread
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 ```python3
 import threading
 import time
-from terminate_thread import terminate
+from terminate_thread import terminate, kill
 
 
 def thread_func1():
     n = 0
     while True:
         n += 1
         print(n, t)
         time.sleep(1)
 
 
 if __name__ == "__main__":
     t = threading.Thread(target=thread_func1, )
     t.start()
     time.sleep(2)
+
     terminate(t)
+    # or
+    kill(t)
+
     exit(0)
 
 
 ```
```

