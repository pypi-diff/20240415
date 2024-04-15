# Comparing `tmp/remindmail-2024.3.15.1.tar.gz` & `tmp/remindmail-2024.4.14.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remindmail-2024.3.15.1.tar", last modified: Sat Mar 16 04:46:49 2024, max compression
+gzip compressed data, was "remindmail-2024.4.14.1.tar", last modified: Mon Apr 15 03:29:08 2024, max compression
```

## Comparing `remindmail-2024.3.15.1.tar` & `remindmail-2024.4.14.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-16 04:46:49.276525 remindmail-2024.3.15.1/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.3.15.1/LICENSE.md
--rw-r--r--   0 tyler     (1000) tyler     (1000)    15533 2024-03-16 04:46:49.276525 remindmail-2024.3.15.1/PKG-INFO
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    15183 2024-01-07 07:25:03.000000 remindmail-2024.3.15.1/README.md
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.3.15.1/pyproject.toml
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)      751 2024-03-16 04:46:49.276525 remindmail-2024.3.15.1/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-16 04:46:49.272525 remindmail-2024.3.15.1/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-16 04:46:49.272525 remindmail-2024.3.15.1/src/remind/
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.3.15.1/src/remind/__init__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     7980 2024-03-12 02:50:41.000000 remindmail-2024.3.15.1/src/remind/__main__.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     2405 2023-12-29 22:36:09.000000 remindmail-2024.3.15.1/src/remind/reminder.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    28459 2024-03-16 04:44:20.000000 remindmail-2024.3.15.1/src/remind/remindmail.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)    12881 2023-12-29 22:36:09.000000 remindmail-2024.3.15.1/src/remind/remindmail_utils.py
--rwxrwxr-x   0 tyler     (1000) tyler     (1000)     6501 2023-12-29 22:36:09.000000 remindmail-2024.3.15.1/src/remind/trello_manager.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-03-16 04:46:49.276525 remindmail-2024.3.15.1/src/remindmail.egg-info/
--rw-r--r--   0 tyler     (1000) tyler     (1000)    15533 2024-03-16 04:46:49.000000 remindmail-2024.3.15.1/src/remindmail.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      392 2024-03-16 04:46:49.000000 remindmail-2024.3.15.1/src/remindmail.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-03-16 04:46:49.000000 remindmail-2024.3.15.1/src/remindmail.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-03-16 04:46:49.000000 remindmail-2024.3.15.1/src/remindmail.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-03-16 04:46:49.000000 remindmail-2024.3.15.1/src/remindmail.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:29:08.197188 remindmail-2024.4.14.1/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     1070 2023-12-29 22:36:09.000000 remindmail-2024.4.14.1/LICENSE.md
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6183 2024-04-15 03:29:08.197188 remindmail-2024.4.14.1/PKG-INFO
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)     5822 2024-04-15 03:27:28.000000 remindmail-2024.4.14.1/README.md
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)       98 2023-12-29 22:36:09.000000 remindmail-2024.4.14.1/pyproject.toml
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)      762 2024-04-15 03:29:08.197188 remindmail-2024.4.14.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:29:08.197188 remindmail-2024.4.14.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:29:08.197188 remindmail-2024.4.14.1/src/remind/
+-rwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-12-29 22:36:09.000000 remindmail-2024.4.14.1/src/remind/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     2537 2024-04-14 21:39:06.000000 remindmail-2024.4.14.1/src/remind/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     1257 2024-04-15 02:56:19.000000 remindmail-2024.4.14.1/src/remind/error_handler.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11268 2024-04-15 02:01:56.000000 remindmail-2024.4.14.1/src/remind/query_manager.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     9889 2024-04-15 02:23:21.000000 remindmail-2024.4.14.1/src/remind/reminder.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    23906 2024-04-15 02:40:25.000000 remindmail-2024.4.14.1/src/remind/reminder_confirmation.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    17715 2024-04-15 02:13:45.000000 remindmail-2024.4.14.1/src/remind/reminder_manager.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-04-15 03:29:08.197188 remindmail-2024.4.14.1/src/remindmail.egg-info/
+-rw-r--r--   0 tyler     (1000) tyler     (1000)     6183 2024-04-15 03:29:08.000000 remindmail-2024.4.14.1/src/remindmail.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      430 2024-04-15 03:29:08.000000 remindmail-2024.4.14.1/src/remindmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-04-15 03:29:08.000000 remindmail-2024.4.14.1/src/remindmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       48 2024-04-15 03:29:08.000000 remindmail-2024.4.14.1/src/remindmail.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        7 2024-04-15 03:29:08.000000 remindmail-2024.4.14.1/src/remindmail.egg-info/top_level.txt
```

### Comparing `remindmail-2024.3.15.1/LICENSE.md` & `remindmail-2024.4.14.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `remindmail-2024.3.15.1/setup.cfg` & `remindmail-2024.4.14.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = remindmail
-version = 2024.03.15.1
+version = 2024.04.14.1
 author = Tyler Woodfin
-author_email = feedback@tyler.cloud
+author_email = feedback-remindmail@tyler.cloud
 description = Easily schedule reminders to be emailed
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/remindmail
 project_urls = 
 bug tracker = https://github.com/tylerjwoodfin/remindmail/issues
 py_modules = ["remind"]
```

