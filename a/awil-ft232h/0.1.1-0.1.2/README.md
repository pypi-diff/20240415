# Comparing `tmp/awil_ft232h-0.1.1.tar.gz` & `tmp/awil_ft232h-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awil_ft232h-0.1.1.tar", last modified: Wed Apr 10 09:03:06 2024, max compression
+gzip compressed data, was "awil_ft232h-0.1.2.tar", last modified: Mon Apr 15 01:36:25 2024, max compression
```

## Comparing `awil_ft232h-0.1.1.tar` & `awil_ft232h-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 09:03:06.497658 awil_ft232h-0.1.1/
--rw-rw-rw-   0        0        0     1084 2024-04-09 04:08:59.000000 awil_ft232h-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      521 2024-04-10 09:03:06.497658 awil_ft232h-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-09 04:08:59.000000 awil_ft232h-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 09:03:06.485658 awil_ft232h-0.1.1/awil_ft232h/
--rw-rw-rw-   0        0        0       35 2024-04-09 04:08:59.000000 awil_ft232h-0.1.1/awil_ft232h/__init__.py
--rw-rw-rw-   0        0        0     3567 2024-04-10 08:41:32.000000 awil_ft232h-0.1.1/awil_ft232h/awil_ft232h.py
-drwxrwxrwx   0        0        0        0 2024-04-10 09:03:06.496658 awil_ft232h-0.1.1/awil_ft232h.egg-info/
--rw-rw-rw-   0        0        0      521 2024-04-10 09:03:06.000000 awil_ft232h-0.1.1/awil_ft232h.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-10 09:03:06.000000 awil_ft232h-0.1.1/awil_ft232h.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 09:03:06.000000 awil_ft232h-0.1.1/awil_ft232h.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-10 09:03:06.000000 awil_ft232h-0.1.1/awil_ft232h.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 09:03:06.000000 awil_ft232h-0.1.1/awil_ft232h.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-10 09:03:06.497658 awil_ft232h-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      395 2024-04-10 08:43:54.000000 awil_ft232h-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:36:25.342550 awil_ft232h-0.1.2/
+-rw-rw-rw-   0        0        0     1084 2024-04-09 04:08:59.000000 awil_ft232h-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      521 2024-04-15 01:36:25.341549 awil_ft232h-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2024-04-10 09:44:35.000000 awil_ft232h-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 01:36:25.327376 awil_ft232h-0.1.2/awil_ft232h/
+-rw-rw-rw-   0        0        0       35 2024-04-09 04:08:59.000000 awil_ft232h-0.1.2/awil_ft232h/__init__.py
+-rw-rw-rw-   0        0        0     2202 2024-04-12 10:18:32.000000 awil_ft232h-0.1.2/awil_ft232h/awil_ft232h.py
+drwxrwxrwx   0        0        0        0 2024-04-15 01:36:25.341549 awil_ft232h-0.1.2/awil_ft232h.egg-info/
+-rw-rw-rw-   0        0        0      521 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 01:36:25.000000 awil_ft232h-0.1.2/awil_ft232h.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 01:36:25.342550 awil_ft232h-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      395 2024-04-15 01:36:16.000000 awil_ft232h-0.1.2/setup.py
```

### Comparing `awil_ft232h-0.1.1/LICENSE` & `awil_ft232h-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awil_ft232h-0.1.1/PKG-INFO` & `awil_ft232h-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awil_ft232h
-Version: 0.1.1
+Version: 0.1.2
 Author: Noriki Mochizuki
 Author-email: noriki.mochizuki.mj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyftdi>=0.55
```

### Comparing `awil_ft232h-0.1.1/awil_ft232h.egg-info/PKG-INFO` & `awil_ft232h-0.1.2/awil_ft232h.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awil_ft232h
-Version: 0.1.1
+Version: 0.1.2
 Author: Noriki Mochizuki
 Author-email: noriki.mochizuki.mj@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyftdi>=0.55
```

