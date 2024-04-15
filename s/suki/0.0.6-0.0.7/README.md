# Comparing `tmp/suki-0.0.6.tar.gz` & `tmp/suki-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suki-0.0.6.tar", last modified: Fri Dec 30 06:03:14 2022, max compression
+gzip compressed data, was "suki-0.0.7.tar", last modified: Mon Apr 15 04:15:46 2024, max compression
```

## Comparing `suki-0.0.6.tar` & `suki-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 06:03:14.272168 suki-0.0.6/
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1301 2022-12-30 05:59:38.000000 suki-0.0.6/LICENSE
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1637 2022-12-30 06:03:14.272168 suki-0.0.6/PKG-INFO
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1164 2022-12-30 05:59:38.000000 suki-0.0.6/README.md
--rw-rw-r--   0 azazel    (1000) azazel    (1000)       38 2022-12-30 06:03:14.272168 suki-0.0.6/setup.cfg
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1004 2022-12-30 05:59:48.000000 suki-0.0.6/setup.py
-drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 06:03:14.272168 suki-0.0.6/suki/
--rw-rw-r--   0 azazel    (1000) azazel    (1000)      109 2022-12-30 05:59:38.000000 suki-0.0.6/suki/__init__.py
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     4079 2022-12-30 06:02:00.000000 suki-0.0.6/suki/suki.py
-drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 06:03:14.272168 suki-0.0.6/suki.egg-info/
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1637 2022-12-30 06:03:14.000000 suki-0.0.6/suki.egg-info/PKG-INFO
--rw-rw-r--   0 azazel    (1000) azazel    (1000)      226 2022-12-30 06:03:14.000000 suki-0.0.6/suki.egg-info/SOURCES.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)        1 2022-12-30 06:03:14.000000 suki-0.0.6/suki.egg-info/dependency_links.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)       45 2022-12-30 06:03:14.000000 suki-0.0.6/suki.egg-info/entry_points.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)       14 2022-12-30 06:03:14.000000 suki-0.0.6/suki.egg-info/requires.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)        5 2022-12-30 06:03:14.000000 suki-0.0.6/suki.egg-info/top_level.txt
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:15:46.571962 suki-0.0.7/
+-rw-r--r--   0 azazel     (501) staff       (20)     1308 2024-04-15 04:14:21.000000 suki-0.0.7/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1687 2024-04-15 04:15:46.571698 suki-0.0.7/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     1167 2024-04-15 04:15:25.000000 suki-0.0.7/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-15 04:15:46.572008 suki-0.0.7/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1013 2024-04-15 04:15:09.000000 suki-0.0.7/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:15:46.570390 suki-0.0.7/suki/
+-rw-r--r--   0 azazel     (501) staff       (20)      114 2024-04-15 04:14:46.000000 suki-0.0.7/suki/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)     4090 2024-04-15 04:15:01.000000 suki-0.0.7/suki/suki.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:15:46.571413 suki-0.0.7/suki.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1687 2024-04-15 04:15:46.000000 suki-0.0.7/suki.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      226 2024-04-15 04:15:46.000000 suki-0.0.7/suki.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-15 04:15:46.000000 suki-0.0.7/suki.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       45 2024-04-15 04:15:46.000000 suki-0.0.7/suki.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       14 2024-04-15 04:15:46.000000 suki-0.0.7/suki.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        5 2024-04-15 04:15:46.000000 suki-0.0.7/suki.egg-info/top_level.txt
```

### Comparing `suki-0.0.6/LICENSE` & `suki-0.0.7/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2022, azazelm3dj3d
+Copyright (c) 2022-2024, battleoverflow
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `suki-0.0.6/PKG-INFO` & `suki-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: suki
-Version: 0.0.6
+Version: 0.0.7
 Summary: Suki is a Python symbolic link package manager created to make Python package management similar to node_modules.
-Home-page: https://github.com/azazelm3dj3d/suki
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/suki
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: faye
 
 # Suki
+
 Suki is a Python package manager created to make file organization more easily accessible. Suki uses symbolic links and `requirements.txt` to locate your site-packages, gather the information, and add the appropriate files in your current working directory under a special directory called `suki_pkgs`.
 
 This structure is similar to how to npm or yarn handle `node_modules` but allows the user to maintain and edit their packages without ever needing to leave their current working directory.
 
 You can install this CLI tool using pip:
 ```bash
 pip install suki
 ```
 
 ### Example
+
 At the moment, Suki only locates, aggregates, and links all of your project's site-packages. This is useful if you need to make alterations or monitor your site-packages in the local directory. All changes to the site-packages will immediately take effect in the installed packages (thanks to the symbolic link).
 ```bash
 suki -l
 ```
 
 You can also input the location of the required packages using the `-f` flag:
 ```bash
```

### Comparing `suki-0.0.6/README.md` & `suki-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Suki
+
 Suki is a Python package manager created to make file organization more easily accessible. Suki uses symbolic links and `requirements.txt` to locate your site-packages, gather the information, and add the appropriate files in your current working directory under a special directory called `suki_pkgs`.
 
 This structure is similar to how to npm or yarn handle `node_modules` but allows the user to maintain and edit their packages without ever needing to leave their current working directory.
 
 You can install this CLI tool using pip:
 ```bash
 pip install suki
 ```
 
 ### Example
+
 At the moment, Suki only locates, aggregates, and links all of your project's site-packages. This is useful if you need to make alterations or monitor your site-packages in the local directory. All changes to the site-packages will immediately take effect in the installed packages (thanks to the symbolic link).
 ```bash
 suki -l
 ```
 
 You can also input the location of the required packages using the `-f` flag:
 ```bash
 suki -l -f "/home/suki/packages/requirements.txt"
 ```
 
-One thing to remember, the `suki_pkgs` will be dumped in whatever directory you are currently working in.
+One thing to remember, the `suki_pkgs` will be dumped in whatever directory you are currently working in.
```

### Comparing `suki-0.0.6/suki/suki.py` & `suki-0.0.7/suki/suki.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Owner: battleoverflow (https://github.com/battleoverflow)
     Project: Suki
     License: BSD 2-Clause
 """
 
 import site, os, argparse, shutil
 
 # Check out Faye, it's also one of my libraries
@@ -28,16 +28,16 @@
         """
         🌸 Banner 🌸
         """
         
         print("-" * 26)
         print(f"🌸 (¬_¬) Suki | v{Suki.version()} 🌸")
         print("-" * 26)
-        print("Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)")
-        print("Source: https://github.com/azazelm3dj3d/suki")
+        print("Owner: battleoverflow (https://github.com/battleoverflow)")
+        print("Source: https://github.com/battleoverflow/suki")
         print("\n")
 
     def link():
         """
         The most powerful method powering Suki.
         This allows the user to create a local directory of a set of packages.
         """
@@ -100,8 +100,8 @@
             print(f"v{Suki.version()}")
 
         if args.link:
             Suki.banner()
             Suki.link()
 
 if __name__ == '__main__':
-    Suki.main()
+    Suki.main()
```

### Comparing `suki-0.0.6/suki.egg-info/PKG-INFO` & `suki-0.0.7/suki.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: suki
-Version: 0.0.6
+Version: 0.0.7
 Summary: Suki is a Python symbolic link package manager created to make Python package management similar to node_modules.
-Home-page: https://github.com/azazelm3dj3d/suki
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/suki
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: faye
 
 # Suki
+
 Suki is a Python package manager created to make file organization more easily accessible. Suki uses symbolic links and `requirements.txt` to locate your site-packages, gather the information, and add the appropriate files in your current working directory under a special directory called `suki_pkgs`.
 
 This structure is similar to how to npm or yarn handle `node_modules` but allows the user to maintain and edit their packages without ever needing to leave their current working directory.
 
 You can install this CLI tool using pip:
 ```bash
 pip install suki
 ```
 
 ### Example
+
 At the moment, Suki only locates, aggregates, and links all of your project's site-packages. This is useful if you need to make alterations or monitor your site-packages in the local directory. All changes to the site-packages will immediately take effect in the installed packages (thanks to the symbolic link).
 ```bash
 suki -l
 ```
 
 You can also input the location of the required packages using the `-f` flag:
 ```bash
```

