# Comparing `tmp/libreppc-0.1.6.tar.gz` & `tmp/libreppc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.6.tar", last modified: Sun Apr 14 20:52:51 2024, max compression
+gzip compressed data, was "libreppc-0.1.7.tar", last modified: Mon Apr 15 03:56:20 2024, max compression
```

## Comparing `libreppc-0.1.6.tar` & `libreppc-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:52:51.850504 libreppc-0.1.6/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.6/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 20:52:51.850504 libreppc-0.1.6/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.6/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:52:51.850504 libreppc-0.1.6/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 20:52:26.000000 libreppc-0.1.6/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      783 2024-04-14 20:43:38.000000 libreppc-0.1.6/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     6340 2024-04-14 20:41:05.000000 libreppc-0.1.6/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 20:52:51.850504 libreppc-0.1.6/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 20:52:51.000000 libreppc-0.1.6/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 20:52:51.850504 libreppc-0.1.6/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.6/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.7/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       98 2024-04-15 03:54:05.000000 libreppc-0.1.7/MANIFEST.in
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 03:56:20.819943 libreppc-0.1.7/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.7/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-15 03:55:35.000000 libreppc-0.1.7/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      783 2024-04-14 20:43:38.000000 libreppc-0.1.7/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     6340 2024-04-14 20:41:05.000000 libreppc-0.1.7/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc/static/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2736 2024-04-14 20:52:00.000000 libreppc-0.1.7/libreppc/static/bloger.css
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2720 2024-04-14 20:51:42.000000 libreppc-0.1.7/libreppc/static/mastodon.css
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc/templates/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2706 2024-04-14 20:16:12.000000 libreppc-0.1.7/libreppc/templates/index.html
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2693 2024-04-14 20:38:07.000000 libreppc-0.1.7/libreppc/templates/post.html
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-15 03:56:20.819943 libreppc-0.1.7/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      375 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-15 03:56:20.000000 libreppc-0.1.7/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-15 03:56:20.819943 libreppc-0.1.7/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1101 2024-04-15 03:53:26.000000 libreppc-0.1.7/setup.py
```

### Comparing `libreppc-0.1.6/LICENSE` & `libreppc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.6/PKG-INFO` & `libreppc-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.6/README.md` & `libreppc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.6/libreppc/__main__.py` & `libreppc-0.1.7/libreppc/__main__.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.6/libreppc/libreppc.py` & `libreppc-0.1.7/libreppc/libreppc.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.6/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.7/libreppc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.6
+Version: 0.1.7
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.6/setup.py` & `libreppc-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     version=VERSION,
     author="loliconshik3",
     author_email="loliconshik3@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=packages,
+    include_package_data=True,
     install_requires=['flask', 'markdown', 'feedgen', 'pytz'], 
     keywords=['python', 'profile', 'html', 'css', 'markdown', 'profile page', 'page', 'site', 'personal page'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

