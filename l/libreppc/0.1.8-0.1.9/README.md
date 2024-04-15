# Comparing `tmp/libreppc-0.1.8.tar.gz` & `tmp/libreppc-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.8.tar", last modified: Mon Apr 15 05:24:22 2024, max compression
+gzip compressed data, was "libreppc-0.1.9.tar", last modified: Mon Apr 15 06:12:17 2024, max compression
```

## Comparing `libreppc-0.1.8.tar` & `libreppc-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.8/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.1.8/MANIFEST.in
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 05:24:22.080480 libreppc-0.1.8/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.8/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-15 05:23:55.000000 libreppc-0.1.8/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      786 2024-04-15 04:47:48.000000 libreppc-0.1.8/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     7253 2024-04-15 04:57:04.000000 libreppc-0.1.8/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc/static/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     3034 2024-04-15 05:09:28.000000 libreppc-0.1.8/libreppc/static/bloger.css
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2778 2024-04-15 05:22:36.000000 libreppc-0.1.8/libreppc/static/mastodon.css
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc/templates/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2987 2024-04-15 05:04:21.000000 libreppc-0.1.8/libreppc/templates/index.html
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2869 2024-04-15 05:04:41.000000 libreppc-0.1.8/libreppc/templates/post.html
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 05:24:22.080480 libreppc-0.1.8/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      375 2024-04-15 05:24:22.000000 libreppc-0.1.8/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-15 05:24:21.000000 libreppc-0.1.8/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-15 05:24:22.080480 libreppc-0.1.8/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1101 2024-04-15 03:53:26.000000 libreppc-0.1.8/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 06:12:17.098023 libreppc-0.1.9/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.9/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.1.9/MANIFEST.in
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 06:12:17.098023 libreppc-0.1.9/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.9/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 06:12:17.094690 libreppc-0.1.9/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-15 06:11:43.000000 libreppc-0.1.9/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      786 2024-04-15 04:47:48.000000 libreppc-0.1.9/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     7253 2024-04-15 04:57:04.000000 libreppc-0.1.9/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 06:12:17.098023 libreppc-0.1.9/libreppc/static/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     3185 2024-04-15 06:11:30.000000 libreppc-0.1.9/libreppc/static/bloger.css
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2778 2024-04-15 05:22:36.000000 libreppc-0.1.9/libreppc/static/mastodon.css
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 06:12:17.098023 libreppc-0.1.9/libreppc/templates/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2987 2024-04-15 05:04:21.000000 libreppc-0.1.9/libreppc/templates/index.html
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2869 2024-04-15 05:04:41.000000 libreppc-0.1.9/libreppc/templates/post.html
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 06:12:17.098023 libreppc-0.1.9/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 06:12:16.000000 libreppc-0.1.9/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      375 2024-04-15 06:12:17.000000 libreppc-0.1.9/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-15 06:12:16.000000 libreppc-0.1.9/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-15 06:12:16.000000 libreppc-0.1.9/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-15 06:12:16.000000 libreppc-0.1.9/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-15 06:12:17.098023 libreppc-0.1.9/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1101 2024-04-15 03:53:26.000000 libreppc-0.1.9/setup.py
```

### Comparing `libreppc-0.1.8/LICENSE` & `libreppc-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/PKG-INFO` & `libreppc-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.8/README.md` & `libreppc-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/libreppc/__main__.py` & `libreppc-0.1.9/libreppc/__main__.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/libreppc/libreppc.py` & `libreppc-0.1.9/libreppc/libreppc.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/libreppc/static/bloger.css` & `libreppc-0.1.9/libreppc/static/bloger.css`

 * *Files 8% similar despite different names*

```diff
@@ -183,24 +183,35 @@
 @media (max-width: 1280px) {
     .content {
         width: 60%;
         margin-left: 20%;
         margin-right: 20%;
     }
 
+    .profile {
+        width: 40%;
+    }
+
     .projects {
-        grid-template-columns: repeat(2, 1fr);
+        grid-template-columns: repeat(3, 1fr);
     }
 }
 
 @media (max-width: 720px) {
     .content {
-        width: 80%;
-        margin-left: 10%;
-        margin-right: 10%;
+        width: 90%;
+        margin-left: 5%;
+        margin-right: 5%;
+    }
+
+    .profile {
+        width: 95%;
+        float: none;
+        clear: all;
+        position: relative;
     }
 
     .projects {
-        grid-template-columns: repeat(1, 1fr);
+        grid-template-columns: repeat(4, 1fr);
     }
 }
```

### Comparing `libreppc-0.1.8/libreppc/static/mastodon.css` & `libreppc-0.1.9/libreppc/static/mastodon.css`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/libreppc/templates/index.html` & `libreppc-0.1.9/libreppc/templates/index.html`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/libreppc/templates/post.html` & `libreppc-0.1.9/libreppc/templates/post.html`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.8/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.9/libreppc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.8/setup.py` & `libreppc-0.1.9/setup.py`

 * *Files identical despite different names*

