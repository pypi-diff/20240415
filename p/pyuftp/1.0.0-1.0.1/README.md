# Comparing `tmp/pyuftp-1.0.0.tar.gz` & `tmp/pyuftp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuftp-1.0.0.tar", last modified: Wed Mar 13 08:42:40 2024, max compression
+gzip compressed data, was "pyuftp-1.0.1.tar", last modified: Mon Apr 15 11:16:01 2024, max compression
```

## Comparing `pyuftp-1.0.0.tar` & `pyuftp-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:42:40.560377 pyuftp-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-13 08:42:32.000000 pyuftp-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-13 08:42:40.560377 pyuftp-1.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2247 2024-03-13 08:42:32.000000 pyuftp-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:42:40.556377 pyuftp-1.0.0/extras/
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-13 08:42:32.000000 pyuftp-1.0.0/extras/pyuftp
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:42:40.560377 pyuftp-1.0.0/pyuftp/
--rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-13 08:42:40.560377 pyuftp-1.0.0/pyuftp/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13822 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/cp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/cryptutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/pconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/share.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/uftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-03-13 08:42:32.000000 pyuftp-1.0.0/pyuftp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 08:42:40.560377 pyuftp-1.0.0/pyuftp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-03-13 08:42:40.000000 pyuftp-1.0.0/pyuftp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-13 08:42:40.000000 pyuftp-1.0.0/pyuftp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 08:42:40.000000 pyuftp-1.0.0/pyuftp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-13 08:42:40.000000 pyuftp-1.0.0/pyuftp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-13 08:42:40.000000 pyuftp-1.0.0/pyuftp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-13 08:42:40.000000 pyuftp-1.0.0/pyuftp.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-03-13 08:42:40.560377 pyuftp-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-03-13 08:42:32.000000 pyuftp-1.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-03-13 08:42:32.000000 pyuftp-1.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:16:01.020058 pyuftp-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-15 11:15:49.000000 pyuftp-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-15 11:16:01.020058 pyuftp-1.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2247 2024-04-15 11:15:49.000000 pyuftp-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:16:01.016058 pyuftp-1.0.1/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-15 11:15:49.000000 pyuftp-1.0.1/extras/pyuftp
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:16:01.020058 pyuftp-1.0.1/pyuftp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       74 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 11:16:01.020058 pyuftp-1.0.1/pyuftp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10513 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14482 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13822 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/cp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/cryptutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/pconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/uftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-15 11:15:49.000000 pyuftp-1.0.1/pyuftp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:16:01.020058 pyuftp-1.0.1/pyuftp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-15 11:16:00.000000 pyuftp-1.0.1/pyuftp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-15 11:16:00.000000 pyuftp-1.0.1/pyuftp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:16:00.000000 pyuftp-1.0.1/pyuftp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 11:16:00.000000 pyuftp-1.0.1/pyuftp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 11:16:00.000000 pyuftp-1.0.1/pyuftp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 11:16:00.000000 pyuftp-1.0.1/pyuftp.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-15 11:16:01.020058 pyuftp-1.0.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1208 2024-04-15 11:15:49.000000 pyuftp-1.0.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-15 11:15:49.000000 pyuftp-1.0.1/versioneer.py
```

### Comparing `pyuftp-1.0.0/LICENSE` & `pyuftp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/PKG-INFO` & `pyuftp-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuftp
-Version: 1.0.0
+Version: 1.0.1
 Summary: UFTP (UNICORE FTP) commandline client
 Home-page: https://github.com/UNICORE-EU/pyuftp
 Author: Bernd Schuller
 Author-email: b.schuller@fz-juelich.de
 License: License :: OSI Approved :: BSD
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pyuftp-1.0.0/README.md` & `pyuftp-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/extras/pyuftp` & `pyuftp-1.0.1/extras/pyuftp`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/authenticate.py` & `pyuftp-1.0.1/pyuftp/authenticate.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/base.py` & `pyuftp-1.0.1/pyuftp/base.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/client.py` & `pyuftp-1.0.1/pyuftp/client.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/cp.py` & `pyuftp-1.0.1/pyuftp/cp.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/cryptutils.py` & `pyuftp-1.0.1/pyuftp/cryptutils.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/pconnector.py` & `pyuftp-1.0.1/pyuftp/pconnector.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/share.py` & `pyuftp-1.0.1/pyuftp/share.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp/uftp.py` & `pyuftp-1.0.1/pyuftp/uftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
         self.perm = ""
         self.is_dir = False
         if ls_line:
             tok = ls_line.strip().split(" ", 3)
             self.is_dir = tok[0].startswith("d")
             self.perm = tok[0]
             self.size = int(tok[1])
-            self.mtime= int(tok[2])
+            self.mtime= int(tok[2]) / 1000
             self.path = tok[3]
     
     def can_write(self):
         return "w" in self.perm
 
     def can_execute(self):
         return "x" in self.perm
```

### Comparing `pyuftp-1.0.0/pyuftp/utils.py` & `pyuftp-1.0.1/pyuftp/utils.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/pyuftp.egg-info/PKG-INFO` & `pyuftp-1.0.1/pyuftp.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuftp
-Version: 1.0.0
+Version: 1.0.1
 Summary: UFTP (UNICORE FTP) commandline client
 Home-page: https://github.com/UNICORE-EU/pyuftp
 Author: Bernd Schuller
 Author-email: b.schuller@fz-juelich.de
 License: License :: OSI Approved :: BSD
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pyuftp-1.0.0/setup.py` & `pyuftp-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyuftp-1.0.0/versioneer.py` & `pyuftp-1.0.1/versioneer.py`

 * *Files identical despite different names*

