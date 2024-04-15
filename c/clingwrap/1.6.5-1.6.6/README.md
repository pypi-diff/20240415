# Comparing `tmp/clingwrap-1.6.5.tar.gz` & `tmp/clingwrap-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clingwrap-1.6.5.tar", last modified: Fri Dec  8 21:29:48 2023, max compression
+gzip compressed data, was "clingwrap-1.6.6.tar", last modified: Mon Apr 15 01:16:47 2024, max compression
```

## Comparing `clingwrap-1.6.5.tar` & `clingwrap-1.6.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-12-08 21:29:48.973361 clingwrap-1.6.5/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2023-12-08 21:29:48.000000 clingwrap-1.6.5/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-02-15 08:01:11.000000 clingwrap-1.6.5/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3581 2023-12-08 21:29:48.973361 clingwrap-1.6.5/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2272 2022-02-15 08:01:11.000000 clingwrap-1.6.5/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-12-08 21:29:48.969355 clingwrap-1.6.5/clingwrap/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-02-15 08:01:11.000000 clingwrap-1.6.5/clingwrap/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6202 2022-09-23 02:46:16.000000 clingwrap-1.6.5/clingwrap/main.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-12-08 21:29:48.973361 clingwrap-1.6.5/clingwrap/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-02-15 08:01:11.000000 clingwrap-1.6.5/clingwrap/tests/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-12-08 21:29:48.973361 clingwrap-1.6.5/clingwrap.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3581 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      485 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       50 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       10 2023-12-08 21:29:48.000000 clingwrap-1.6.5/clingwrap.egg-info/top_level.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-12-08 21:29:48.973361 clingwrap-1.6.5/examples/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4047 2023-12-07 21:49:17.000000 clingwrap-1.6.5/examples/shakenfist-ci-failure.cwd
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2022-02-15 08:01:11.000000 clingwrap-1.6.5/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      115 2022-08-07 23:04:29.000000 clingwrap-1.6.5/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      716 2023-12-08 21:29:48.973361 clingwrap-1.6.5/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1108 2022-02-15 08:07:21.000000 clingwrap-1.6.5/setup.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:04:29.000000 clingwrap-1.6.5/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-12-08 21:29:48.973361 clingwrap-1.6.5/tools/
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2022-02-15 08:01:11.000000 clingwrap-1.6.5/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2022-02-15 08:01:11.000000 clingwrap-1.6.5/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-15 01:16:47.757625 clingwrap-1.6.6/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2024-04-15 01:16:47.000000 clingwrap-1.6.6/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-02-15 08:01:11.000000 clingwrap-1.6.6/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3581 2024-04-15 01:16:47.757625 clingwrap-1.6.6/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2272 2022-02-15 08:01:11.000000 clingwrap-1.6.6/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-15 01:16:47.753624 clingwrap-1.6.6/clingwrap/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-02-15 08:01:11.000000 clingwrap-1.6.6/clingwrap/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6202 2022-09-23 02:46:16.000000 clingwrap-1.6.6/clingwrap/main.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-15 01:16:47.757625 clingwrap-1.6.6/clingwrap/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-02-15 08:01:11.000000 clingwrap-1.6.6/clingwrap/tests/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-15 01:16:47.757625 clingwrap-1.6.6/clingwrap.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3581 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      485 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       50 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       10 2024-04-15 01:16:47.000000 clingwrap-1.6.6/clingwrap.egg-info/top_level.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-15 01:16:47.757625 clingwrap-1.6.6/examples/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4221 2024-04-06 21:05:47.000000 clingwrap-1.6.6/examples/shakenfist-ci-failure.cwd
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2022-02-15 08:01:11.000000 clingwrap-1.6.6/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      115 2022-08-07 23:04:29.000000 clingwrap-1.6.6/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      716 2024-04-15 01:16:47.757625 clingwrap-1.6.6/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1108 2022-02-15 08:07:21.000000 clingwrap-1.6.6/setup.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-07 23:04:29.000000 clingwrap-1.6.6/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2024-04-15 01:16:47.757625 clingwrap-1.6.6/tools/
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2022-02-15 08:01:11.000000 clingwrap-1.6.6/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2022-02-15 08:01:11.000000 clingwrap-1.6.6/tox.ini
```

### Comparing `clingwrap-1.6.5/LICENSE` & `clingwrap-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/PKG-INFO` & `clingwrap-1.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clingwrap
-Version: 1.6.5
+Version: 1.6.6
 Summary: clingwrap: wrap up CI artefacts and post them to Google Storage
 Home-page: https://shakenfist.com/clingwrap
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Clingwrap
         =========
```

### Comparing `clingwrap-1.6.5/README.md` & `clingwrap-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/clingwrap/main.py` & `clingwrap-1.6.6/clingwrap/main.py`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/clingwrap.egg-info/PKG-INFO` & `clingwrap-1.6.6/clingwrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clingwrap
-Version: 1.6.5
+Version: 1.6.6
 Summary: clingwrap: wrap up CI artefacts and post them to Google Storage
 Home-page: https://shakenfist.com/clingwrap
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Clingwrap
         =========
```

### Comparing `clingwrap-1.6.5/examples/shakenfist-ci-failure.cwd` & `clingwrap-1.6.6/examples/shakenfist-ci-failure.cwd`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     destination: etc/apparmor
     file: etc/apparmor
 
   - name: apparmor configuration directory
     destination: etc/apparmor.d
     directory: /etc/apparmor.d
 
+  - name: apache2 configuration
+    destination: etc/apache2
+    directory: /etc/apache2
+
+  - name: Shaken Fist configuration
+    destination: etc/sf
+    directory: /etc/sf
+
   - name: Installed system OS packages and versions
     destination: _commands/dpkg
     shell: dpkg -l
 
   - name: Installed system pip packages and versions
     destination: _commands/pip
     shell: pip3 freeze
```

### Comparing `clingwrap-1.6.5/release.sh` & `clingwrap-1.6.6/release.sh`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/setup.cfg` & `clingwrap-1.6.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/setup.py` & `clingwrap-1.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/tools/flake8wrap.sh` & `clingwrap-1.6.6/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `clingwrap-1.6.5/tox.ini` & `clingwrap-1.6.6/tox.ini`

 * *Files identical despite different names*

