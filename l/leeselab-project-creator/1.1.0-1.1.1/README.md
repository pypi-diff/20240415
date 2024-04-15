# Comparing `tmp/leeselab-project-creator-1.1.0.tar.gz` & `tmp/leeselab_project_creator-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leeselab-project-creator-1.1.0.tar", last modified: Fri Apr 12 06:15:57 2024, max compression
+gzip compressed data, was "leeselab_project_creator-1.1.1.tar", last modified: Mon Apr 15 08:19:50 2024, max compression
```

## Comparing `leeselab-project-creator-1.1.0.tar` & `leeselab_project_creator-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 06:15:57.124321 leeselab-project-creator-1.1.0/
--rw-rw-rw-   0        0        0     1092 2024-03-22 13:13:18.000000 leeselab-project-creator-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2753 2024-04-12 06:15:57.123324 leeselab-project-creator-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2140 2024-04-12 06:06:43.000000 leeselab-project-creator-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 06:15:57.115331 leeselab-project-creator-1.1.0/leeselab_project_creator/
--rw-rw-rw-   0        0        0        0 2024-03-22 13:13:18.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/__init__.py
--rw-rw-rw-   0        0        0     6518 2024-03-22 13:13:18.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/__main__.py
--rw-rw-rw-   0        0        0     6447 2024-04-12 06:10:40.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/generate_plate_layout.py
--rw-rw-rw-   0        0        0     8707 2024-04-12 06:10:07.000000 leeselab-project-creator-1.1.0/leeselab_project_creator/generate_worklist.py
-drwxrwxrwx   0        0        0        0 2024-04-12 06:15:57.123324 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/
--rw-rw-rw-   0        0        0     2753 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      486 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       59 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-04-12 06:15:57.000000 leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 06:15:57.124321 leeselab-project-creator-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2024-04-12 06:15:30.000000 leeselab-project-creator-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:50.966231 leeselab_project_creator-1.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-03-21 12:48:51.000000 leeselab_project_creator-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2753 2024-04-15 08:19:50.965231 leeselab_project_creator-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2140 2024-04-03 06:34:35.000000 leeselab_project_creator-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:50.952315 leeselab_project_creator-1.1.1/leeselab_project_creator/
+-rw-rw-rw-   0        0        0        0 2024-04-03 06:33:19.000000 leeselab_project_creator-1.1.1/leeselab_project_creator/__init__.py
+-rw-rw-rw-   0        0        0     6518 2024-04-03 06:33:22.000000 leeselab_project_creator-1.1.1/leeselab_project_creator/__main__.py
+-rw-rw-rw-   0        0        0     6447 2024-04-15 08:13:37.000000 leeselab_project_creator-1.1.1/leeselab_project_creator/generate_plate_layout.py
+-rw-rw-rw-   0        0        0     8707 2024-04-15 08:14:36.000000 leeselab_project_creator-1.1.1/leeselab_project_creator/generate_worklist.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:19:50.964228 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/
+-rw-rw-rw-   0        0        0     2753 2024-04-15 08:19:50.000000 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      486 2024-04-15 08:19:50.000000 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:19:50.000000 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-04-15 08:19:50.000000 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       59 2024-04-15 08:19:50.000000 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-04-15 08:19:50.000000 leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:19:50.966231 leeselab_project_creator-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2024-04-15 08:14:47.000000 leeselab_project_creator-1.1.1/setup.py
```

### Comparing `leeselab-project-creator-1.1.0/LICENSE` & `leeselab_project_creator-1.1.1/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `leeselab-project-creator-1.1.0/PKG-INFO` & `leeselab_project_creator-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeselab-project-creator
-Version: 1.1.0
+Version: 1.1.1
 Summary: The leeselab project creator.
 Home-page: https://github.com/DominikBuchner/BOLDigger-commandline
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leeselab-project-creator-1.1.0/README.md` & `leeselab_project_creator-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `leeselab-project-creator-1.1.0/leeselab_project_creator/__main__.py` & `leeselab_project_creator-1.1.1/leeselab_project_creator/__main__.py`

 * *Files identical despite different names*

### Comparing `leeselab-project-creator-1.1.0/leeselab_project_creator/generate_plate_layout.py` & `leeselab_project_creator-1.1.1/leeselab_project_creator/generate_plate_layout.py`

 * *Files identical despite different names*

### Comparing `leeselab-project-creator-1.1.0/leeselab_project_creator/generate_worklist.py` & `leeselab_project_creator-1.1.1/leeselab_project_creator/generate_worklist.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -111,32 +111,32 @@
     general_worklist["plate"] = plates
 
     # optimal primer order for maximizing library diversity
     optimal_primer_order = [
         1,
         5,
         9,
-        13,
-        17,
-        21,
         2,
         6,
         10,
-        14,
-        18,
-        22,
         3,
         7,
         11,
-        15,
-        19,
-        23,
         4,
         8,
         12,
+        13,
+        17,
+        21,
+        14,
+        18,
+        22,
+        15,
+        19,
+        23,
         16,
         20,
         24,
     ]
 
     # gather the worklists here
     worklists = []
```

### Comparing `leeselab-project-creator-1.1.0/leeselab_project_creator.egg-info/PKG-INFO` & `leeselab_project_creator-1.1.1/leeselab_project_creator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leeselab-project-creator
-Version: 1.1.0
+Version: 1.1.1
 Summary: The leeselab project creator.
 Home-page: https://github.com/DominikBuchner/BOLDigger-commandline
 Author: Dominik Buchner
 Author-email: dominik.buchner524@googlemail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leeselab-project-creator-1.1.0/setup.py` & `leeselab_project_creator-1.1.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="leeselab-project-creator",
-    version="1.1.0",
+    version="1.1.1",
     author="Dominik Buchner",
     author_email="dominik.buchner524@googlemail.com",
     description="The leeselab project creator.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/DominikBuchner/BOLDigger-commandline",
     packages=setuptools.find_packages(),
```

