# Comparing `tmp/facialfinder-0.0.5.tar.gz` & `tmp/facialfinder-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facialfinder-0.0.5.tar", last modified: Mon Apr 15 12:26:59 2024, max compression
+gzip compressed data, was "facialfinder-0.0.6.tar", last modified: Mon Apr 15 14:05:03 2024, max compression
```

## Comparing `facialfinder-0.0.5.tar` & `facialfinder-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.200678 facialfinder-0.0.5/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     1069 2024-04-15 12:21:06.000000 facialfinder-0.0.5/LICENSE.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3622 2024-04-15 12:26:59.200500 facialfinder-0.0.5/PKG-INFO
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3192 2024-04-15 12:25:12.000000 facialfinder-0.0.5/README.md
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.199053 facialfinder-0.0.5/facialfinder/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       40 2024-04-15 12:21:35.000000 facialfinder-0.0.5/facialfinder/__init__.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      129 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/_path.py
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.199614 facialfinder-0.0.5/facialfinder/datasets/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)   930127 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/datasets/faces.xml
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3541 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/image.py
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     5140 2024-04-15 12:21:06.000000 facialfinder-0.0.5/facialfinder/video.py
-drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 12:26:59.200321 facialfinder-0.0.5/facialfinder.egg-info/
--rw-r--r--   0 god_of_programmers   (501) staff       (20)     3622 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/PKG-INFO
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      332 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/SOURCES.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/dependency_links.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       58 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/requires.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       13 2024-04-15 12:26:59.000000 facialfinder-0.0.5/facialfinder.egg-info/top_level.txt
--rw-r--r--   0 god_of_programmers   (501) staff       (20)       38 2024-04-15 12:26:59.200714 facialfinder-0.0.5/setup.cfg
--rw-r--r--   0 god_of_programmers   (501) staff       (20)      738 2024-04-15 12:26:56.000000 facialfinder-0.0.5/setup.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 14:05:03.128979 facialfinder-0.0.6/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     1069 2024-04-15 13:53:04.000000 facialfinder-0.0.6/LICENSE.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3860 2024-04-15 14:05:03.128801 facialfinder-0.0.6/PKG-INFO
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3430 2024-04-15 14:00:47.000000 facialfinder-0.0.6/README.md
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 14:05:03.127413 facialfinder-0.0.6/facialfinder/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       40 2024-04-15 13:53:04.000000 facialfinder-0.0.6/facialfinder/__init__.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      129 2024-04-15 13:53:04.000000 facialfinder-0.0.6/facialfinder/_path.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 14:05:03.127993 facialfinder-0.0.6/facialfinder/datasets/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)   930127 2024-04-15 13:53:04.000000 facialfinder-0.0.6/facialfinder/datasets/faces.xml
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3541 2024-04-15 13:53:04.000000 facialfinder-0.0.6/facialfinder/image.py
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     5140 2024-04-15 13:53:04.000000 facialfinder-0.0.6/facialfinder/video.py
+drwxr-xr-x   0 god_of_programmers   (501) staff       (20)        0 2024-04-15 14:05:03.128651 facialfinder-0.0.6/facialfinder.egg-info/
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)     3860 2024-04-15 14:05:03.000000 facialfinder-0.0.6/facialfinder.egg-info/PKG-INFO
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      332 2024-04-15 14:05:03.000000 facialfinder-0.0.6/facialfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)        1 2024-04-15 14:05:03.000000 facialfinder-0.0.6/facialfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       58 2024-04-15 14:05:03.000000 facialfinder-0.0.6/facialfinder.egg-info/requires.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       13 2024-04-15 14:05:03.000000 facialfinder-0.0.6/facialfinder.egg-info/top_level.txt
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)       38 2024-04-15 14:05:03.129023 facialfinder-0.0.6/setup.cfg
+-rw-r--r--   0 god_of_programmers   (501) staff       (20)      738 2024-04-15 14:05:01.000000 facialfinder-0.0.6/setup.py
```

### Comparing `facialfinder-0.0.5/LICENSE.txt` & `facialfinder-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.5/PKG-INFO` & `facialfinder-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: facialfinder
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple tool for Face Detection on Image or Video, realtime detection support.
 Home-page: https://github.com/Anonimous05/FacialFinder
 Author: Airas Tolonov
 Author-email: airastolonov05@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: progressbar2==4.4.2
 
-<center><h1>Face Detection with OpenCV</h1></center>
-<center><h4>Very simple tool for face detection on Image or Video</h4></center>
+<p align="center">
+    <kbd>
+        <img style="border-radius: 5px; height: 200px" src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/logo/200x200.png" alt="logo">
+    </kbd>
+    <h1 style="margin: 0" align="center">FacialFinder with OpenCV</h1>
+    <h4 style="margin: 0" align="center">Very simple tool for face detection on Image or Video</h4>
+</p>
 <h2>Services</h2>
 <ul> 
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li>
 <b>Instance Methods</b>
@@ -122,23 +127,23 @@
 <h2>Examples</h2>
 <ul>
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/img.png" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/img.png" alt="" width="600"/>
 <li><b>After Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.png" alt="" width="600">
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/detected_faces.png" alt="" width="600">
 </ul>
 </li>
 <li>
 <h3><b>VideoDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/vid.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/vid.gif" alt="" width="600"/>
 <li><b>After Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/detected_faces.gif" alt="" width="600"/>
 </ul>
 </li>
 </ul>
```

### Comparing `facialfinder-0.0.5/README.md` & `facialfinder-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-<center><h1>Face Detection with OpenCV</h1></center>
-<center><h4>Very simple tool for face detection on Image or Video</h4></center>
+<p align="center">
+    <kbd>
+        <img style="border-radius: 5px; height: 200px" src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/logo/200x200.png" alt="logo">
+    </kbd>
+    <h1 style="margin: 0" align="center">FacialFinder with OpenCV</h1>
+    <h4 style="margin: 0" align="center">Very simple tool for face detection on Image or Video</h4>
+</p>
 <h2>Services</h2>
 <ul> 
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li>
 <b>Instance Methods</b>
@@ -109,23 +114,23 @@
 <h2>Examples</h2>
 <ul>
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/img.png" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/img.png" alt="" width="600"/>
 <li><b>After Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.png" alt="" width="600">
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/detected_faces.png" alt="" width="600">
 </ul>
 </li>
 <li>
 <h3><b>VideoDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/vid.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/vid.gif" alt="" width="600"/>
 <li><b>After Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/detected_faces.gif" alt="" width="600"/>
 </ul>
 </li>
 </ul>
```

### Comparing `facialfinder-0.0.5/facialfinder/datasets/faces.xml` & `facialfinder-0.0.6/facialfinder/datasets/faces.xml`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.5/facialfinder/image.py` & `facialfinder-0.0.6/facialfinder/image.py`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.5/facialfinder/video.py` & `facialfinder-0.0.6/facialfinder/video.py`

 * *Files identical despite different names*

### Comparing `facialfinder-0.0.5/facialfinder.egg-info/PKG-INFO` & `facialfinder-0.0.6/facialfinder.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: facialfinder
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple tool for Face Detection on Image or Video, realtime detection support.
 Home-page: https://github.com/Anonimous05/FacialFinder
 Author: Airas Tolonov
 Author-email: airastolonov05@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy==1.26.4
 Requires-Dist: opencv-python==4.9.0.80
 Requires-Dist: progressbar2==4.4.2
 
-<center><h1>Face Detection with OpenCV</h1></center>
-<center><h4>Very simple tool for face detection on Image or Video</h4></center>
+<p align="center">
+    <kbd>
+        <img style="border-radius: 5px; height: 200px" src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/logo/200x200.png" alt="logo">
+    </kbd>
+    <h1 style="margin: 0" align="center">FacialFinder with OpenCV</h1>
+    <h4 style="margin: 0" align="center">Very simple tool for face detection on Image or Video</h4>
+</p>
 <h2>Services</h2>
 <ul> 
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li>
 <b>Instance Methods</b>
@@ -122,23 +127,23 @@
 <h2>Examples</h2>
 <ul>
 <li>
 <h3><b>ImageDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/img.png" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/img.png" alt="" width="600"/>
 <li><b>After Face Detection image</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.png" alt="" width="600">
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/detected_faces.png" alt="" width="600">
 </ul>
 </li>
 <li>
 <h3><b>VideoDetection</b></h3>
 <ul>
 <li><b>.detect()</b></li>
 <li><b>Before Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/vid.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/vid.gif" alt="" width="600"/>
 <li><b>After Face Detection video</b></li>
-<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/examples/static/examples/detected_faces.gif" alt="" width="600"/>
+<img src="https://raw.githubusercontent.com/Anonimous05/FacialFinder/static/static/examples/detected_faces.gif" alt="" width="600"/>
 </ul>
 </li>
 </ul>
```

### Comparing `facialfinder-0.0.5/setup.py` & `facialfinder-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 core_dir = Path(__file__).parent
 
 long_description = (core_dir / "README.md").read_text()
 
 setup(
     name="facialfinder",
-    version="0.0.5",
+    version="0.0.6",
     url="https://github.com/Anonimous05/FacialFinder",
     author="Airas Tolonov",
     author_email="airastolonov05@gmail.com",
     description="Simple tool for Face Detection on Image or Video, realtime detection support.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
```

