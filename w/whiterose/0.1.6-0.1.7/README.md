# Comparing `tmp/whiterose-0.1.6.tar.gz` & `tmp/whiterose-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiterose-0.1.6.tar", last modified: Thu Apr  7 03:20:57 2022, max compression
+gzip compressed data, was "whiterose-0.1.7.tar", last modified: Mon Apr 15 03:50:48 2024, max compression
```

## Comparing `whiterose-0.1.6.tar` & `whiterose-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-04-07 03:20:57.086313 whiterose-0.1.6/
--rw-r--r--   0 kali      (1000) kali      (1000)     1073 2022-04-07 02:19:43.000000 whiterose-0.1.6/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     1968 2022-04-07 03:20:57.086313 whiterose-0.1.6/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1429 2022-04-07 03:15:31.000000 whiterose-0.1.6/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       84 2022-04-07 03:12:57.000000 whiterose-0.1.6/pyproject.toml
--rw-r--r--   0 kali      (1000) kali      (1000)      627 2022-04-07 03:20:57.086313 whiterose-0.1.6/setup.cfg
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-04-07 03:20:57.082313 whiterose-0.1.6/src/
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-04-07 03:20:57.082313 whiterose-0.1.6/src/whiterose/
--rw-r--r--   0 kali      (1000) kali      (1000)        0 2022-04-07 03:18:41.000000 whiterose-0.1.6/src/whiterose/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1513 2022-04-07 03:19:59.000000 whiterose-0.1.6/src/whiterose/whiterose.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2022-04-07 03:20:57.086313 whiterose-0.1.6/src/whiterose.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     1968 2022-04-07 03:20:56.000000 whiterose-0.1.6/src/whiterose.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      243 2022-04-07 03:20:57.000000 whiterose-0.1.6/src/whiterose.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2022-04-07 03:20:56.000000 whiterose-0.1.6/src/whiterose.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       10 2022-04-07 03:20:56.000000 whiterose-0.1.6/src/whiterose.egg-info/top_level.txt
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 03:50:48.247995 whiterose-0.1.7/
+-rw-r--r--   0 azazel     (501) staff       (20)     1074 2024-04-15 03:50:12.000000 whiterose-0.1.7/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1712 2024-04-15 03:50:48.247729 whiterose-0.1.7/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     1174 2024-04-15 03:49:58.000000 whiterose-0.1.7/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-15 03:50:48.248042 whiterose-0.1.7/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1142 2024-04-15 03:48:53.000000 whiterose-0.1.7/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 03:50:48.247436 whiterose-0.1.7/whiterose.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1712 2024-04-15 03:50:48.000000 whiterose-0.1.7/whiterose.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      171 2024-04-15 03:50:48.000000 whiterose-0.1.7/whiterose.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-15 03:50:48.000000 whiterose-0.1.7/whiterose.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       10 2024-04-15 03:50:48.000000 whiterose-0.1.7/whiterose.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)     1514 2024-04-15 03:45:41.000000 whiterose-0.1.7/whiterose.py
```

### Comparing `whiterose-0.1.6/LICENSE` & `whiterose-0.1.7/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `whiterose-0.1.6/PKG-INFO` & `whiterose-0.1.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,72 @@
 Metadata-Version: 2.1
 Name: whiterose
-Version: 0.1.6
-Summary: Whiterose Timing Library
-Home-page: https://github.com/Hifumi1337/whiterose
-Author: Hifumi1337
-Author-email: hifumi1337@protonmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/Hifumi1337/whiterose/issues
-Platform: UNKNOWN
+Version: 0.1.7
+Summary: Whiterose is a pure Python library built to return the current time in real-time within a single stdout. This Python library does not require any external libraries.
+Home-page: https://github.com/battleoverflow/whiterose
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Whiterose
-Whiterose is a pure Python library built to return the current time in real-time within a single stdout. This Python library does not require any external libraries. This project is still in a semi-WIP state.
+Whiterose is a pure Python library built to return the current time in real-time within a single stdout. This Python library does not require any external libraries.
 
 ## Installation
 You can install this library via Pypi:
-```bash
-pip3 install whiterose
-```
 
-## Usage
-A script has been provided for testing the currently functionality of the library.
 ```bash
-$ python3 example.py
+pip3 install whiterose
 ```
 
 ### Options
 timer_s() - Time updates in real-time every second
 
 timer_m() - Time updates in real-time every minute
 
 timer_h() - Time updates in real-time every hour
 
 ## Examples
-You can call the library by using this syntax. This example will print the time to the console every second.
+
+You can call the library by using this syntax:
+
 ```python
-from whiterose.whiterose import Whiterose
+# This example will print the time to the console every second
+from whiterose import Whiterose
 
 wr = Whiterose()
 
 def one_s_timer():
-    wr.timer_s(1) # Real-time timer ever 1 second
+    wr.timer_s(1) # 1 second
 
 if __name__ == '__main__':
     one_s_timer()
 ```
 
-This example will print the time to the console every 4 seconds.
 ```python
-from whiterose.whiterose import Whiterose
+# This example will print the time to the console every 4 seconds
+from whiterose import Whiterose
 
 wr = Whiterose()
 
 def one_s_timer():
-    wr.timer_s(4) # Real-time timer ever 4 seconds
+    wr.timer_s(4) # 4 seconds
 
 if __name__ == '__main__':
     one_s_timer()
 ```
 
-This example will print the time to the console every 2 minutes.
 ```python
-from whiterose.whiterose import Whiterose
+# This example will print the time to the console every 2 minutes
+from whiterose import Whiterose
 
 wr = Whiterose()
 
 def one_m_timer():
-    wr.timer_m(2) # Real-time timer ever 2 minutes
+    wr.timer_m(2) # 2 minutes
 
 if __name__ == '__main__':
     one_m_timer()
 ```
-
```

### Comparing `whiterose-0.1.6/README.md` & `whiterose-0.1.7/whiterose.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,72 @@
+Metadata-Version: 2.1
+Name: whiterose
+Version: 0.1.7
+Summary: Whiterose is a pure Python library built to return the current time in real-time within a single stdout. This Python library does not require any external libraries.
+Home-page: https://github.com/battleoverflow/whiterose
+Author: battleoverflow
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Whiterose
-Whiterose is a pure Python library built to return the current time in real-time within a single stdout. This Python library does not require any external libraries. This project is still in a semi-WIP state.
+Whiterose is a pure Python library built to return the current time in real-time within a single stdout. This Python library does not require any external libraries.
 
 ## Installation
 You can install this library via Pypi:
-```bash
-pip3 install whiterose
-```
 
-## Usage
-A script has been provided for testing the currently functionality of the library.
 ```bash
-$ python3 example.py
+pip3 install whiterose
 ```
 
 ### Options
 timer_s() - Time updates in real-time every second
 
 timer_m() - Time updates in real-time every minute
 
 timer_h() - Time updates in real-time every hour
 
 ## Examples
-You can call the library by using this syntax. This example will print the time to the console every second.
+
+You can call the library by using this syntax:
+
 ```python
-from whiterose.whiterose import Whiterose
+# This example will print the time to the console every second
+from whiterose import Whiterose
 
 wr = Whiterose()
 
 def one_s_timer():
-    wr.timer_s(1) # Real-time timer ever 1 second
+    wr.timer_s(1) # 1 second
 
 if __name__ == '__main__':
     one_s_timer()
 ```
 
-This example will print the time to the console every 4 seconds.
 ```python
-from whiterose.whiterose import Whiterose
+# This example will print the time to the console every 4 seconds
+from whiterose import Whiterose
 
 wr = Whiterose()
 
 def one_s_timer():
-    wr.timer_s(4) # Real-time timer ever 4 seconds
+    wr.timer_s(4) # 4 seconds
 
 if __name__ == '__main__':
     one_s_timer()
 ```
 
-This example will print the time to the console every 2 minutes.
 ```python
-from whiterose.whiterose import Whiterose
+# This example will print the time to the console every 2 minutes
+from whiterose import Whiterose
 
 wr = Whiterose()
 
 def one_m_timer():
-    wr.timer_m(2) # Real-time timer ever 2 minutes
+    wr.timer_m(2) # 2 minutes
 
 if __name__ == '__main__':
     one_m_timer()
-```
+```
```

### Comparing `whiterose-0.1.6/src/whiterose/whiterose.py` & `whiterose-0.1.7/whiterose.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import time, os, platform
 from datetime import datetime
 
 ###############################################
 #                                             #
 #   Whiterose Timing Library                  #
-#   Author: Hifumi1337                        #
-#   GitHub: https://github.com/Hifumi1337     #
+#   Author: battleoverflow                    #
+#   GitHub: https://github.com/battleoverflow #
 #                                             #
 ###############################################
 
-VERSION = "0.1.6"
+VERSION = "0.1.7"
 
 class Whiterose:
 
     def timer_s(self, seconds):
 
         while True:
             time.sleep(seconds) # Number of seconds
@@ -51,8 +51,8 @@
             if platform.system() == 'Windows':
                 os.system('cls')
             else:
                 os.system("clear")
             
             timer = datetime.now().strftime("%I:%M:%S %p")
 
-            print(timer)
+            print(timer)
```

