# Comparing `tmp/xdcheckin-2.0.5.tar.gz` & `tmp/xdcheckin-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdcheckin-2.0.5.tar", last modified: Sun Apr 14 13:14:21 2024, max compression
+gzip compressed data, was "xdcheckin-2.0.6.tar", last modified: Sun Apr 14 15:41:30 2024, max compression
```

## Comparing `xdcheckin-2.0.5.tar` & `xdcheckin-2.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.140514 xdcheckin-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 13:14:21.140514 xdcheckin-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:14:21.140514 xdcheckin-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.132514 xdcheckin-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/Xdcheckin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 13:14:21.000000 xdcheckin-2.0.5/src/Xdcheckin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/chaoxing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/core/xidian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/server/static/
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/activity.js
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/classroom.js
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/curriculum.js
--rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/g_classroom_urls.js
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/global.js
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/location.js
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/login.js
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/misc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/player.js
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/static/util.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/server/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/server/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:21.136514 xdcheckin-2.0.5/src/xdcheckin/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/util/chaoxing_captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-14 13:14:09.000000 xdcheckin-2.0.5/src/xdcheckin/util/encryption.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.450209 xdcheckin-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 15:41:30.450209 xdcheckin-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:41:30.450209 xdcheckin-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.442209 xdcheckin-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.446209 xdcheckin-2.0.6/src/Xdcheckin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-14 15:41:30.000000 xdcheckin-2.0.6/src/Xdcheckin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 15:41:30.000000 xdcheckin-2.0.6/src/Xdcheckin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:41:30.000000 xdcheckin-2.0.6/src/Xdcheckin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-14 15:41:30.000000 xdcheckin-2.0.6/src/Xdcheckin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-14 15:41:30.000000 xdcheckin-2.0.6/src/Xdcheckin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 15:41:30.000000 xdcheckin-2.0.6/src/Xdcheckin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.442209 xdcheckin-2.0.6/src/xdcheckin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.442209 xdcheckin-2.0.6/src/xdcheckin/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33581 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/core/chaoxing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/core/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/core/xidian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.446209 xdcheckin-2.0.6/src/xdcheckin/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11913 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.446209 xdcheckin-2.0.6/src/xdcheckin/server/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/activity.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/classroom.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/curriculum.js
+-rw-r--r--   0 runner    (1001) docker     (127)   249304 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/g_classroom_urls.js
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/global.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/location.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/login.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/misc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/player.js
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/static/util.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.446209 xdcheckin-2.0.6/src/xdcheckin/server/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/server/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:30.446209 xdcheckin-2.0.6/src/xdcheckin/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7171 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/util/chaoxing_captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-14 15:41:25.000000 xdcheckin-2.0.6/src/xdcheckin/util/encryption.py
```

### Comparing `xdcheckin-2.0.5/LICENSE` & `xdcheckin-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/PKG-INFO` & `xdcheckin-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.5
+Version: 2.0.6
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `xdcheckin-2.0.5/README.md` & `xdcheckin-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/pyproject.toml` & `xdcheckin-2.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Xdcheckin"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
 	{name = "Pairman", email = "pairmanxlr@gmail.com"}
 ]
 readme = "README.md"
 description = "Chaoxing Checkin Tool for XDU."
 license = {text = "GNU General Public License v3 (GPLv3)"}
 keywords = ["xdu", "xidian", "chaoxing", "livestream"]
```

### Comparing `xdcheckin-2.0.5/src/Xdcheckin.egg-info/PKG-INFO` & `xdcheckin-2.0.6/src/Xdcheckin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Xdcheckin
-Version: 2.0.5
+Version: 2.0.6
 Summary: Chaoxing Checkin Tool for XDU.
 Author-email: Pairman <pairmanxlr@gmail.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/Pairman/Xdcheckin
 Project-URL: Changelog, https://github.com/Pairman/Xdcheckin/blob/main/CHANGELOG.md
 Keywords: xdu,xidian,chaoxing,livestream
 Classifier: Framework :: Flask
```

### Comparing `xdcheckin-2.0.5/src/Xdcheckin.egg-info/SOURCES.txt` & `xdcheckin-2.0.6/src/Xdcheckin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/core/chaoxing.py` & `xdcheckin-2.0.6/src/xdcheckin/core/chaoxing.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/core/locations.py` & `xdcheckin-2.0.6/src/xdcheckin/core/locations.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/core/xidian.py` & `xdcheckin-2.0.6/src/xdcheckin/core/xidian.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/server.py` & `xdcheckin-2.0.6/src/xdcheckin/server/server.py`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/activity.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/activity.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/classroom.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/classroom.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/curriculum.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/curriculum.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/g_classroom_urls.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/g_classroom_urls.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/location.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/location.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/login.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/login.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/misc.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/misc.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/player.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/player.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/style.css` & `xdcheckin-2.0.6/src/xdcheckin/server/static/style.css`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/static/util.js` & `xdcheckin-2.0.6/src/xdcheckin/server/static/util.js`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/server/templates/index.html` & `xdcheckin-2.0.6/src/xdcheckin/server/templates/index.html`

 * *Files identical despite different names*

### Comparing `xdcheckin-2.0.5/src/xdcheckin/util/chaoxing_captcha.py` & `xdcheckin-2.0.6/src/xdcheckin/util/chaoxing_captcha.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,39 +15,50 @@
 def solve_captcha(big_img: None = None, small_img: None = None):
 	"""Slider CAPTCHA solver.
 	:param big_img: Background image with slider piece embedded.
 	:param small_img: Slider image vertically aligned with transparent padding.
 	:return: Slider offset.
 	"""
 	with small_img.convert("L") as img:
+		x_right = 0
+		flag_x = False
 		y_bottom = 0
-		f_init = False
+		flag_y = False
 		with img.point(lambda v: v > 0 and 255 or 0) as pt:
 			y_top = pt.height
 			for y in range(pt.height):
 				if pt.crop((0, y, pt.width, y + 1)).getbbox():
 					y_bottom = max(y, y_bottom)
 					y_top = min(y, y_top)
-					f_init = True
-				elif f_init:
+					flag_y = True
+				elif flag_y:
 					break
-		with img.crop((0, y_top, small_img.width, y_bottom + 1)) as img:
+			x_left = pt.width
+			for x in range(pt.width):
+				if pt.crop((x, y_top, x + 1, y_bottom + 1)).getbbox():
+					x_right = max(x, x_right)
+					x_left = min(x, x_left)
+					flag_x = True
+				elif flag_x:
+					break
+		with img.crop((x_left, y_top, x_right, y_bottom + 1)) as img:
 			template = img.getdata()
 	mean_tmp = sum(template) / len(template)
 	template = [v - mean_tmp for v in template]
+	maxncc = 0
 	maxx = 0
-	maxv = 0
 	with big_img.convert("L").crop(
-		(0, y_top, big_img.width, y_bottom + 1)
+		(x_left, y_top, big_img.width - small_img.width + x_right + 1, y_bottom + 1)
 	) as img:
-		for x in range(0, img.width - small_img.width + 1, 4):
+		for x in range(1, img.width - x_right + x_left, 2):
 			window = img.crop(
-				(x, 0, x + small_img.width, img.height)
+				(x, 0, x + x_right - x_left, img.height)
 			).getdata()
-			mean_wd = sum(window)
+			mean_wd = sum(window) / (x_right - x_left) / img.height
+			window = [w - mean_wd for w in window]
 			ncc = sum(
-				(u - mean_wd) * v
-				for u, v in zip(window, template)
-			) / sum(map(lambda v: (v - mean_wd) ** 2, window))
-			if ncc > maxv:
-				maxx, maxv = x, ncc
-	return maxx
+				w * t for w, t in zip(window, template)
+			) / sum(w ** 2 for w in window)
+			if ncc > maxncc:
+				maxncc = ncc
+				maxx = x
+	return maxx + 1
```

### Comparing `xdcheckin-2.0.5/src/xdcheckin/util/encryption.py` & `xdcheckin-2.0.6/src/xdcheckin/util/encryption.py`

 * *Files identical despite different names*

