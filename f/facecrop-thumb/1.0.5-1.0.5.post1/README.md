# Comparing `tmp/facecrop-thumb-1.0.5.tar.gz` & `tmp/facecrop-thumb-1.0.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facecrop-thumb-1.0.5.tar", last modified: Sat Apr 13 05:30:55 2024, max compression
+gzip compressed data, was "facecrop-thumb-1.0.5.post1.tar", last modified: Mon Apr 15 06:17:01 2024, max compression
```

## Comparing `facecrop-thumb-1.0.5.tar` & `facecrop-thumb-1.0.5.post1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/facecrop_thumb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/thumbnail_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/facecrop_thumb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 05:30:55.000000 facecrop-thumb-1.0.5/facecrop_thumb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:30:55.100022 facecrop-thumb-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-13 05:30:47.000000 facecrop-thumb-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:17:01.158043 facecrop-thumb-1.0.5.post1/
+-rw-rw-rw-   0        0        0     1092 2024-04-12 11:58:00.000000 facecrop-thumb-1.0.5.post1/LICENSE
+-rw-rw-rw-   0        0        0     4237 2024-04-15 06:17:01.158043 facecrop-thumb-1.0.5.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     3207 2024-04-14 16:59:22.000000 facecrop-thumb-1.0.5.post1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 06:17:01.148015 facecrop-thumb-1.0.5.post1/facecrop_thumb/
+-rw-rw-rw-   0        0        0        0 2024-04-13 05:09:35.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-04-12 15:16:49.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/__main__.py
+-rw-rw-rw-   0        0        0      283 2024-04-12 10:33:36.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/face_detection.py
+-rw-rw-rw-   0        0        0      788 2024-04-12 10:33:30.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/image_processing.py
+-rw-rw-rw-   0        0        0     1860 2024-04-14 16:12:15.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/main.py
+-rw-rw-rw-   0        0        0     2461 2024-04-13 05:15:26.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/thumbnail_generation.py
+-rw-rw-rw-   0        0        0       27 2024-04-15 06:16:26.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 06:17:01.157039 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/
+-rw-rw-rw-   0        0        0     4237 2024-04-15 06:17:00.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      476 2024-04-15 06:17:00.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 06:17:00.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-04-15 06:17:00.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-15 06:17:00.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 06:17:00.000000 facecrop-thumb-1.0.5.post1/facecrop_thumb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       81 2024-04-15 06:17:01.160114 facecrop-thumb-1.0.5.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1441 2024-04-13 06:04:04.000000 facecrop-thumb-1.0.5.post1/setup.py
```

### Comparing `facecrop-thumb-1.0.5/LICENSE` & `facecrop-thumb-1.0.5.post1/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Vaibhav Shukla
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Vaibhav Shukla
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `facecrop-thumb-1.0.5/facecrop_thumb/image_processing.py` & `facecrop-thumb-1.0.5.post1/facecrop_thumb/image_processing.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# image_processing.py
-import cv2
-
-def crop_face_thumbnail(image, face_coords, margin=50, target_size=(74, 74)):
-    x, y, w, h = face_coords
-    x -= margin
-    y -= margin
-    w += 2 * margin
-    h += 2 * margin
-    x = max(0, x)
-    y = max(0, y)
-    w = min(w, image.shape[1])
-    h = min(h, image.shape[0])
-    aspect_ratio = w / h
-    if w > h:
-        thumbnail_height = int(target_size[1])
-        thumbnail_width = int(thumbnail_height * aspect_ratio)
-    else:
-        thumbnail_width = int(target_size[0])
-        thumbnail_height = int(thumbnail_width / aspect_ratio)
-    face_with_margin = image[y:y+h, x:x+w]
-    face_thumbnail = cv2.resize(face_with_margin, (thumbnail_width, thumbnail_height), interpolation=cv2.INTER_AREA)
-    return face_thumbnail
+# image_processing.py
+import cv2
+
+def crop_face_thumbnail(image, face_coords, margin=50, target_size=(74, 74)):
+    x, y, w, h = face_coords
+    x -= margin
+    y -= margin
+    w += 2 * margin
+    h += 2 * margin
+    x = max(0, x)
+    y = max(0, y)
+    w = min(w, image.shape[1])
+    h = min(h, image.shape[0])
+    aspect_ratio = w / h
+    if w > h:
+        thumbnail_height = int(target_size[1])
+        thumbnail_width = int(thumbnail_height * aspect_ratio)
+    else:
+        thumbnail_width = int(target_size[0])
+        thumbnail_height = int(thumbnail_width / aspect_ratio)
+    face_with_margin = image[y:y+h, x:x+w]
+    face_thumbnail = cv2.resize(face_with_margin, (thumbnail_width, thumbnail_height), interpolation=cv2.INTER_AREA)
+    return face_thumbnail
```

