# Comparing `tmp/codeframe-0.5.5.tar.gz` & `tmp/codeframe-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeframe-0.5.5.tar", last modified: Mon Apr 15 09:09:21 2024, max compression
+gzip compressed data, was "codeframe-0.5.7.tar", last modified: Mon Apr 15 09:12:32 2024, max compression
```

## Comparing `codeframe-0.5.5.tar` & `codeframe-0.5.7.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 09:09:21.143255 codeframe-0.5.5/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     2025 2024-04-15 09:09:13.000000 codeframe-0.5.5/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.139254 codeframe-0.5.5/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 08:56:26.000000 codeframe-0.5.5/bin/codeframe
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-01-17 17:42:18.000000 codeframe-0.5.5/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10240 2024-04-09 08:16:32.000000 codeframe-0.5.5/codeframe/cmd_parser.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6895 2024-03-20 08:17:13.000000 codeframe-0.5.5/codeframe/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/codeframe/data/
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/codeframe/data/installation_files/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      461 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/.bumpversion.cfg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       83 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/.gitignore
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1845 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/README.org
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-19 15:01:37.000000 codeframe-0.5.5/codeframe/data/installation_files/__init__.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/codeframe/data/installation_files/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/bin/codeframe
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/bin_codeframe.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/codeframe/data/installation_files/codeframe/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/codeframe/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3944 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/distcheck.sh
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      291 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/requirements.txt
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-04-15 09:09:09.000000 codeframe-0.5.5/codeframe/data/installation_files/setup.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2024-03-19 14:47:38.000000 codeframe-0.5.5/codeframe/data/testing
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4075 2024-03-20 08:16:36.000000 codeframe-0.5.5/codeframe/df_table.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      633 2024-04-09 08:07:38.000000 codeframe-0.5.5/codeframe/fn_load.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9400 2024-04-15 09:00:33.000000 codeframe-0.5.5/codeframe/installation.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9460 2024-04-08 14:32:43.000000 codeframe-0.5.5/codeframe/interpreter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8898 2024-04-15 08:51:16.000000 codeframe-0.5.5/codeframe/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5127 2024-04-03 05:16:15.000000 codeframe-0.5.5/codeframe/mmapwr.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2897 2024-01-23 13:00:22.000000 codeframe-0.5.5/codeframe/topbar.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-15 09:09:20.000000 codeframe-0.5.5/codeframe/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:09:21.143255 codeframe-0.5.5/codeframe.egg-info/
--rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 09:09:20.000000 codeframe-0.5.5/codeframe.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      990 2024-04-15 09:09:21.000000 codeframe-0.5.5/codeframe.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-15 09:09:20.000000 codeframe-0.5.5/codeframe.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       76 2024-04-15 09:09:20.000000 codeframe-0.5.5/codeframe.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2024-04-15 09:09:20.000000 codeframe-0.5.5/codeframe.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-15 09:09:21.143255 codeframe-0.5.5/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-19 15:48:21.000000 codeframe-0.5.5/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.005637 codeframe-0.5.7/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 09:12:32.005637 codeframe-0.5.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     2025 2024-04-15 09:12:29.000000 codeframe-0.5.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.001637 codeframe-0.5.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 08:56:26.000000 codeframe-0.5.7/bin/codeframe
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.001637 codeframe-0.5.7/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-01-17 17:42:18.000000 codeframe-0.5.7/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    10240 2024-04-09 08:16:32.000000 codeframe-0.5.7/codeframe/cmd_parser.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6895 2024-03-20 08:17:13.000000 codeframe-0.5.7/codeframe/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.001637 codeframe-0.5.7/codeframe/data/
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.001637 codeframe-0.5.7/codeframe/data/installation_files/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      466 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/.bumpversion.cfg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       83 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/.gitignore
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1845 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/README.org
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-03-19 15:01:37.000000 codeframe-0.5.7/codeframe/data/installation_files/__init__.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.001637 codeframe-0.5.7/codeframe/data/installation_files/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/bin/codeframe
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    11703 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/bin_codeframe.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.005637 codeframe-0.5.7/codeframe/data/installation_files/codeframe/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      251 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/codeframe/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3944 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/distcheck.sh
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      291 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/requirements.txt
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-04-15 09:12:25.000000 codeframe-0.5.7/codeframe/data/installation_files/setup.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2024-03-19 14:47:38.000000 codeframe-0.5.7/codeframe/data/testing
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4075 2024-03-20 08:16:36.000000 codeframe-0.5.7/codeframe/df_table.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      633 2024-04-09 08:07:38.000000 codeframe-0.5.7/codeframe/fn_load.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9403 2024-04-15 09:10:40.000000 codeframe-0.5.7/codeframe/installation.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     9460 2024-04-08 14:32:43.000000 codeframe-0.5.7/codeframe/interpreter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     8898 2024-04-15 08:51:16.000000 codeframe-0.5.7/codeframe/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     5127 2024-04-03 05:16:15.000000 codeframe-0.5.7/codeframe/mmapwr.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2897 2024-01-23 13:00:22.000000 codeframe-0.5.7/codeframe/topbar.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2024-04-15 09:12:31.000000 codeframe-0.5.7/codeframe/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2024-04-15 09:12:32.005637 codeframe-0.5.7/codeframe.egg-info/
+-rw-r--r--   0 ojr       (1000) ojr       (1000)     2484 2024-04-15 09:12:31.000000 codeframe-0.5.7/codeframe.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      990 2024-04-15 09:12:31.000000 codeframe-0.5.7/codeframe.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2024-04-15 09:12:31.000000 codeframe-0.5.7/codeframe.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       76 2024-04-15 09:12:31.000000 codeframe-0.5.7/codeframe.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       10 2024-04-15 09:12:31.000000 codeframe-0.5.7/codeframe.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2024-04-15 09:12:32.005637 codeframe-0.5.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1861 2024-03-19 15:48:21.000000 codeframe-0.5.7/setup.py
```

### Comparing `codeframe-0.5.5/PKG-INFO` & `codeframe-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.5.5
+Version: 0.5.7
 Summary: Automatically created environment for python package
 Home-page: https://gitlab.com/jaromrax/codeframe
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `codeframe-0.5.5/README.md` & `codeframe-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/bin/codeframe` & `codeframe-0.5.7/bin/codeframe`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/cmd_parser.py` & `codeframe-0.5.7/codeframe/cmd_parser.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/config.py` & `codeframe-0.5.7/codeframe/config.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/data/installation_files/README.org` & `codeframe-0.5.7/codeframe/data/installation_files/README.org`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/data/installation_files/bin/codeframe` & `codeframe-0.5.7/codeframe/data/installation_files/bin/codeframe`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/data/installation_files/bin_codeframe.py` & `codeframe-0.5.7/codeframe/data/installation_files/bin_codeframe.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/data/installation_files/distcheck.sh` & `codeframe-0.5.7/codeframe/data/installation_files/distcheck.sh`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/data/installation_files/setup.py` & `codeframe-0.5.7/codeframe/data/installation_files/setup.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/df_table.py` & `codeframe-0.5.7/codeframe/df_table.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/fn_load.py` & `codeframe-0.5.7/codeframe/fn_load.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/installation.py` & `codeframe-0.5.7/codeframe/installation.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                'bin/codeframe','bin_codeframe','codeframe/__init__.py','mmapwr.py','interpreter.py']
 
 
     # softlink these modules from subdirectory
     #
     #  WHAT IS NEEDED TO SOFT LINK
     #
-    lnmod = ['version','key_enter','topbar','config','df_table', 'mmapwr.py','interpreter.py','cmd_parser']
+    lnmod = ['version','key_enter','topbar','config','df_table', 'mmapwr.py','interpreter.py','cmd_parser.py']
 
     # POSTINIT, create  also COPA = f"~/.config/{proj}/cfg.json"
     #init = ['git','test','config',f'ln bin/{name}']
 
 
     ## prepare the structure or check existing commands
     #
```

### Comparing `codeframe-0.5.5/codeframe/interpreter.py` & `codeframe-0.5.7/codeframe/interpreter.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/key_enter.py` & `codeframe-0.5.7/codeframe/key_enter.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/mmapwr.py` & `codeframe-0.5.7/codeframe/mmapwr.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe/topbar.py` & `codeframe-0.5.7/codeframe/topbar.py`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/codeframe.egg-info/PKG-INFO` & `codeframe-0.5.7/codeframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codeframe
-Version: 0.5.5
+Version: 0.5.7
 Summary: Automatically created environment for python package
 Home-page: https://gitlab.com/jaromrax/codeframe
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 Requires-Dist: fire
```

### Comparing `codeframe-0.5.5/codeframe.egg-info/SOURCES.txt` & `codeframe-0.5.7/codeframe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codeframe-0.5.5/setup.py` & `codeframe-0.5.7/setup.py`

 * *Files identical despite different names*

