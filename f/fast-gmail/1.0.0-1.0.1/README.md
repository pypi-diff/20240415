# Comparing `tmp/fast_gmail-1.0.0.tar.gz` & `tmp/fast_gmail-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.0.0.tar", last modified: Mon Apr 15 08:11:04 2024, max compression
+gzip compressed data, was "fast_gmail-1.0.1.tar", last modified: Mon Apr 15 08:36:43 2024, max compression
```

## Comparing `fast_gmail-1.0.0.tar` & `fast_gmail-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:11:04.351646 fast_gmail-1.0.0/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.0/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14831 2024-04-15 08:11:04.351646 fast_gmail-1.0.0/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14071 2024-04-15 07:32:29.000000 fast_gmail-1.0.0/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:11:04.347646 fast_gmail-1.0.0/fast_gmail/
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:11:04.351646 fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    14831 2024-04-15 08:11:04.000000 fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      250 2024-04-15 08:11:04.000000 fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-15 08:11:04.000000 fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-15 08:11:04.000000 fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-15 08:11:04.000000 fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-15 08:11:04.351646 fast_gmail-1.0.0/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1125 2024-04-15 08:10:57.000000 fast_gmail-1.0.0/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:36:43.367196 fast_gmail-1.0.1/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.0.1/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    14837 2024-04-15 08:36:43.367196 fast_gmail-1.0.1/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14077 2024-04-15 08:16:21.000000 fast_gmail-1.0.1/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:36:43.363196 fast_gmail-1.0.1/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       16 2024-04-14 07:52:44.000000 fast_gmail-1.0.1/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.0.1/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    19262 2024-04-15 07:00:58.000000 fast_gmail-1.0.1/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7199 2024-04-15 06:26:53.000000 fast_gmail-1.0.1/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25326 2024-04-15 06:27:25.000000 fast_gmail-1.0.1/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.0.1/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-04-15 08:36:43.367196 fast_gmail-1.0.1/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    14837 2024-04-15 08:36:43.000000 fast_gmail-1.0.1/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-04-15 08:36:43.000000 fast_gmail-1.0.1/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-04-15 08:36:43.000000 fast_gmail-1.0.1/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-04-15 08:36:43.000000 fast_gmail-1.0.1/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-04-15 08:36:43.000000 fast_gmail-1.0.1/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-04-15 08:36:43.367196 fast_gmail-1.0.1/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1056 2024-04-15 08:36:30.000000 fast_gmail-1.0.1/setup.py
```

### Comparing `fast_gmail-1.0.0/LICENSE` & `fast_gmail-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.0.0/PKG-INFO` & `fast_gmail-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.0
+Version: 1.0.1
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
 Requires-Dist: typing-extensions==4.11.0
 
 # Fast-gmail a simple python wrapper for gmailapi
 
 [![PyPI Downloads](https://img.shields.io/pypi/dm/fast-gmail.svg?label=PyPI%20downloads)](
-https://pypi.org/project/fast-gmail/)
+https://pypi.org/project/fast-gmail/1.0.0/)
 
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
 - Filter messages
```

### Comparing `fast_gmail-1.0.0/README.md` & `fast_gmail-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Fast-gmail a simple python wrapper for gmailapi
 
 [![PyPI Downloads](https://img.shields.io/pypi/dm/fast-gmail.svg?label=PyPI%20downloads)](
-https://pypi.org/project/fast-gmail/)
+https://pypi.org/project/fast-gmail/1.0.0/)
 
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
 - Filter messages
```

### Comparing `fast_gmail-1.0.0/fast_gmail/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.0.1/fast_gmail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.0.0
+Version: 1.0.1
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 Requires-Dist: google-auth-httplib2==0.2.0
 Requires-Dist: google-auth-oauthlib==1.2.0
 Requires-Dist: typing-extensions==4.11.0
 
 # Fast-gmail a simple python wrapper for gmailapi
 
 [![PyPI Downloads](https://img.shields.io/pypi/dm/fast-gmail.svg?label=PyPI%20downloads)](
-https://pypi.org/project/fast-gmail/)
+https://pypi.org/project/fast-gmail/1.0.0/)
 
 ---
 ## Functionalities:
 - Send text/html messages
 - Send messages with signature & attachments
 - Get messages with pagination
 - Filter messages
```

