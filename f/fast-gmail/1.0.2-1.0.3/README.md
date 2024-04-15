# Comparing `tmp/fast_gmail-1.0.2.tar.gz` & `tmp/fast_gmail-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.2.tar", last modified: Mon Apr 15 08:42:07 2024, max compression
+gzip compressed data, was "fast_gmail-1.0.3.tar", last modified: Mon Apr 15 08:44:30 2024, max compression
```

## Comparing `fast_gmail-1.0.2.tar` & `fast_gmail-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:42:07.208335 fast_gmail-1.0.2/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.2/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14837 2024-04-15 08:42:07.208335 fast_gmail-1.0.2/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14077 2024-04-15 08:16:21.000000 fast_gmail-1.0.2/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:42:07.204335 fast_gmail-1.0.2/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       19 2024-04-15 08:40:47.000000 fast_gmail-1.0.2/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.2/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    19262 2024-04-15 07:00:58.000000 fast_gmail-1.0.2/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7199 2024-04-15 06:26:53.000000 fast_gmail-1.0.2/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25326 2024-04-15 06:27:25.000000 fast_gmail-1.0.2/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.2/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:42:07.204335 fast_gmail-1.0.2/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14837 2024-04-15 08:42:07.000000 fast_gmail-1.0.2/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-15 08:42:07.000000 fast_gmail-1.0.2/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-15 08:42:07.000000 fast_gmail-1.0.2/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-15 08:42:07.000000 fast_gmail-1.0.2/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-15 08:42:07.000000 fast_gmail-1.0.2/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-15 08:42:07.208335 fast_gmail-1.0.2/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1056 2024-04-15 08:40:59.000000 fast_gmail-1.0.2/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:44:30.504817 fast_gmail-1.0.3/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.3/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    14837 2024-04-15 08:44:30.504817 fast_gmail-1.0.3/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14077 2024-04-15 08:16:21.000000 fast_gmail-1.0.3/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:44:30.504817 fast_gmail-1.0.3/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.0.3/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.3/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    19262 2024-04-15 07:00:58.000000 fast_gmail-1.0.3/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7199 2024-04-15 06:26:53.000000 fast_gmail-1.0.3/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25326 2024-04-15 06:27:25.000000 fast_gmail-1.0.3/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.3/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:44:30.504817 fast_gmail-1.0.3/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    14837 2024-04-15 08:44:30.000000 fast_gmail-1.0.3/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-15 08:44:30.000000 fast_gmail-1.0.3/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-15 08:44:30.000000 fast_gmail-1.0.3/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-15 08:44:30.000000 fast_gmail-1.0.3/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-15 08:44:30.000000 fast_gmail-1.0.3/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-15 08:44:30.504817 fast_gmail-1.0.3/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1056 2024-04-15 08:44:23.000000 fast_gmail-1.0.3/setup.py
```

### Comparing `fast_gmail-1.0.2/LICENSE` & `fast_gmail-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.2/PKG-INFO` & `fast_gmail-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.2
+Version: 1.0.3
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.0.2/README.md` & `fast_gmail-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.2/fast_gmail/gmail.py` & `fast_gmail-1.0.3/fast_gmail/gmail.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.2/fast_gmail/helpers.py` & `fast_gmail-1.0.3/fast_gmail/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.2/fast_gmail/message.py` & `fast_gmail-1.0.3/fast_gmail/message.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.2/fast_gmail/search.py` & `fast_gmail-1.0.3/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.2/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.0.3/fast_gmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.2
+Version: 1.0.3
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.0.2/setup.py` & `fast_gmail-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.0.2",
+    version="1.0.3",
     description="GmailApi wrapper",
     long_description=long_descrition,  # Load description from README
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
```

