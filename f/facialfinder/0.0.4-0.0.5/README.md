# Comparing `tmp/facialfinder-0.0.4.tar.gz` & `tmp/facialfinder-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facialfinder-0.0.4.tar", last modified: Fri Apr 12 22:18:35 2024, max compression
+gzip compressed data, was "facialfinder-0.0.5.tar", last modified: Mon Apr 15 12:26:59 2024, max compression
```

## Comparing `facialfinder-0.0.4.tar` & `facialfinder-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:18:35.364580 facialfinder-0.0.4/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     1069 2024-04-12 18:33:09.000000 facialfinder-0.0.4/LICENSE.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3610 2024-04-12 22:18:35.364397 facialfinder-0.0.4/PKG-INFO
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3180 2024-04-12 18:48:05.000000 facialfinder-0.0.4/README.md
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:18:35.361550 facialfinder-0.0.4/facialfinder/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-12 18:59:26.000000 facialfinder-0.0.4/facialfinder/__init__.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      129 2024-04-12 22:06:08.000000 facialfinder-0.0.4/facialfinder/_path.py
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:18:35.362215 facialfinder-0.0.4/facialfinder/datasets/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)   930127 2024-04-12 18:58:20.000000 facialfinder-0.0.4/facialfinder/datasets/faces.xml
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3541 2024-04-12 20:04:58.000000 facialfinder-0.0.4/facialfinder/image.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     5140 2024-04-12 20:04:58.000000 facialfinder-0.0.4/facialfinder/video.py
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-12 22:18:35.364204 facialfinder-0.0.4/facialfinder.egg-info/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3610 2024-04-12 22:18:35.000000 facialfinder-0.0.4/facialfinder.egg-info/PKG-INFO
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      332 2024-04-12 22:18:35.000000 facialfinder-0.0.4/facialfinder.egg-info/SOURCES.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-12 22:18:35.000000 facialfinder-0.0.4/facialfinder.egg-info/dependency_links.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       58 2024-04-12 22:18:35.000000 facialfinder-0.0.4/facialfinder.egg-info/requires.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       13 2024-04-12 22:18:35.000000 facialfinder-0.0.4/facialfinder.egg-info/top_level.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       38 2024-04-12 22:18:35.364615 facialfinder-0.0.4/setup.cfg
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      738 2024-04-12 22:18:30.000000 facialfinder-0.0.4/setup.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.200678 facialfinder-0.0.5/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     1069 2024-04-15 12:21:06.000000 facialfinder-0.0.5/LICENSE.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3622 2024-04-15 12:26:59.200500 facialfinder-0.0.5/PKG-INFO
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3192 2024-04-15 12:25:12.000000 facialfinder-0.0.5/README.md
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.199053 facialfinder-0.0.5/facialfinder/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       40 2024-04-15 12:21:35.000000 facialfinder-0.0.5/facialfinder/__init__.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      129 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/_path.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.199614 facialfinder-0.0.5/facialfinder/datasets/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)   930127 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/datasets/faces.xml
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3541 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/image.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     5140 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/video.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.200321 facialfinder-0.0.5/facialfinder.egg-info/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3622 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/PKG-INFO
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      332 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       58 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/requires.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       13 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/top_level.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       38 2024-04-15 12:26:59.200714 facialfinder-0.0.5/setup.cfg
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      738 2024-04-15 12:26:56.000000 facialfinder-0.0.5/setup.py
```

### Comparing `facialfinder-0.0.4/LICENSE.txt` & `facialfinder-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.4/PKG-INFO` & `facialfinder-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facialfinder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple tool for Face Detection on Image or Video, realtime detection support.
 Home-page: https://github.com/Anonimous05/FacialFinder
 Author: Airas Tolonov
 Author-email: airastolonov05@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy==1.26.4
@@ -122,23 +122,23 @@
 <h2>Examples</h2>
 <ul>
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/img.png" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/img.png" alt="" width="600"/>
 <li><b>After Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/detected_faces.png" alt="" width="600">
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.png" alt="" width="600">
 </ul>
 </li>
 <li>
 <h3><b>VideoDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/vid.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/vid.gif" alt="" width="600"/>
 <li><b>After Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/detected_faces.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.gif" alt="" width="600"/>
 </ul>
 </li>
 </ul>
```

### Comparing `facialfinder-0.0.4/README.md` & `facialfinder-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -109,23 +109,23 @@
 <h2>Examples</h2>
 <ul>
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/img.png" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/img.png" alt="" width="600"/>
 <li><b>After Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/detected_faces.png" alt="" width="600">
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.png" alt="" width="600">
 </ul>
 </li>
 <li>
 <h3><b>VideoDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/vid.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/vid.gif" alt="" width="600"/>
 <li><b>After Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/detected_faces.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.gif" alt="" width="600"/>
 </ul>
 </li>
 </ul>
```

### Comparing `facialfinder-0.0.4/facialfinder/datasets/faces.xml` & `facialfinder-0.0.5/facialfinder/datasets/faces.xml`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.4/facialfinder/image.py` & `facialfinder-0.0.5/facialfinder/image.py`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.4/facialfinder/video.py` & `facialfinder-0.0.5/facialfinder/video.py`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.4/facialfinder.egg-info/PKG-INFO` & `facialfinder-0.0.5/facialfinder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facialfinder
-Version: 0.0.4
+Version: 0.0.5
 Summary: Simple tool for Face Detection on Image or Video, realtime detection support.
 Home-page: https://github.com/Anonimous05/FacialFinder
 Author: Airas Tolonov
 Author-email: airastolonov05@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy==1.26.4
@@ -122,23 +122,23 @@
 <h2>Examples</h2>
 <ul>
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/img.png" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/img.png" alt="" width="600"/>
 <li><b>After Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/detected_faces.png" alt="" width="600">
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.png" alt="" width="600">
 </ul>
 </li>
 <li>
 <h3><b>VideoDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/vid.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/vid.gif" alt="" width="600"/>
 <li><b>After Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FaceDetection/main/static/examples/detected_faces.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.gif" alt="" width="600"/>
 </ul>
 </li>
 </ul>
```

### Comparing `facialfinder-0.0.4/setup.py` & `facialfinder-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 core_dir = Path(__file__).parent
 
 long_description = (core_dir / "README.md").read_text()
 
 setup(
     name="facialfinder",
-    version="0.0.4",
+    version="0.0.5",
     url="https://github.com/Anonimous05/FacialFinder",
     author="Airas Tolonov",
     author_email="airastolonov05@gmail.com",
     description="Simple tool for Face Detection on Image or Video, realtime detection support.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

