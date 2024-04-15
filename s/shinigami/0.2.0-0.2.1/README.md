# Comparing `tmp/shinigami-0.2.0.tar.gz` & `tmp/shinigami-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shinigami-0.2.0.tar", last modified: Sun Jun 11 01:42:08 2023, max compression
+gzip compressed data, was "shinigami-0.2.1.tar", last modified: Mon Apr 15 05:54:56 2024, max compression
```

## Comparing `shinigami-0.2.0.tar` & `shinigami-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-11 01:42:08.109053 shinigami-0.2.0/
--rw-r--r--   0 azazel     (501) staff       (20)     1322 2023-06-11 01:36:19.000000 shinigami-0.2.0/LICENSE
--rw-r--r--   0 azazel     (501) staff       (20)     1362 2023-06-11 01:42:08.108912 shinigami-0.2.0/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      884 2023-06-11 01:38:18.000000 shinigami-0.2.0/README.md
--rw-r--r--   0 azazel     (501) staff       (20)       38 2023-06-11 01:42:08.109089 shinigami-0.2.0/setup.cfg
--rw-r--r--   0 azazel     (501) staff       (20)     1025 2023-06-11 01:36:19.000000 shinigami-0.2.0/setup.py
-drwxr-xr-x   0 azazel     (501) staff       (20)        0 2023-06-11 01:42:08.108729 shinigami-0.2.0/shinigami.egg-info/
--rw-r--r--   0 azazel     (501) staff       (20)     1362 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/PKG-INFO
--rw-r--r--   0 azazel     (501) staff       (20)      239 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/SOURCES.txt
--rw-r--r--   0 azazel     (501) staff       (20)        1 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/dependency_links.txt
--rw-r--r--   0 azazel     (501) staff       (20)       48 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/entry_points.txt
--rw-r--r--   0 azazel     (501) staff       (20)       14 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/requires.txt
--rw-r--r--   0 azazel     (501) staff       (20)       10 2023-06-11 01:42:08.000000 shinigami-0.2.0/shinigami.egg-info/top_level.txt
--rw-r--r--   0 azazel     (501) staff       (20)     6393 2023-06-11 01:41:44.000000 shinigami-0.2.0/shinigami.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 05:54:56.684154 shinigami-0.2.1/
+-rw-r--r--   0 azazel     (501) staff       (20)     1329 2024-04-15 05:53:58.000000 shinigami-0.2.1/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     2129 2024-04-15 05:54:56.683744 shinigami-0.2.1/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)     1602 2024-04-15 05:54:01.000000 shinigami-0.2.1/README.md
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-15 05:54:56.684241 shinigami-0.2.1/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1035 2024-04-15 05:54:10.000000 shinigami-0.2.1/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 05:54:56.683457 shinigami-0.2.1/shinigami.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     2129 2024-04-15 05:54:56.000000 shinigami-0.2.1/shinigami.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      239 2024-04-15 05:54:56.000000 shinigami-0.2.1/shinigami.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-15 05:54:56.000000 shinigami-0.2.1/shinigami.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       48 2024-04-15 05:54:56.000000 shinigami-0.2.1/shinigami.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       14 2024-04-15 05:54:56.000000 shinigami-0.2.1/shinigami.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       10 2024-04-15 05:54:56.000000 shinigami-0.2.1/shinigami.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)     6415 2024-04-15 05:54:24.000000 shinigami-0.2.1/shinigami.py
```

### Comparing `shinigami-0.2.0/LICENSE` & `shinigami-0.2.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 2-Clause License
 
-Copyright (c) 2022, azazelm3dj3d
+Copyright (c) 2022-2024, battleoverflow
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `shinigami-0.2.0/shinigami.py` & `shinigami-0.2.1/shinigami.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-    Project: Shinigami (https://github.com/shinigamilib/shinigami)
-    Author: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Project: Shinigami (https://github.com/battleoverflow/shinigami)
+    Author: battleoverflow (https://github.com/battleoverflow)
     License: BSD 2-Clause
 """
 
 import os, requests, sys
 import argparse
 
 # Logging library
@@ -34,17 +34,16 @@
 
     def generate_dockerfile(self):
         """
         Generate a Dockerfile in the current working directory
         """
         
         try:
-
             # Queries open source Dockerfile repository
-            docker_data = requests.get(f"https://raw.githubusercontent.com/shinigamilib/DockDB/main/DockDB/{self.lang_os}/{self.version}/Dockerfile")
+            docker_data = requests.get(f"https://raw.githubusercontent.com/battleoverflow/DockDB/main/DockDB/{self.lang_os}/{self.version}/Dockerfile")
 
             # Checks the status code for the repository connection
             if docker_data.status_code == 200:
                 with open("Dockerfile", "w") as f:
                     f.write(docker_data.text)
 
                 if self.verbose:
@@ -107,19 +106,19 @@
                 print(Faye.log(msg="Successfully removed Dockerfile", level="INFO", color=self.color))
             else:
                 pass
 
 class CLI:
     def run():
         parser = argparse.ArgumentParser()
-        parser.add_argument('-i', '--image', help="Docker image to generate", default=None, required=False)
-        parser.add_argument('-v', '--version', help="Version of the Docker image", default=None, required=False)
-        parser.add_argument('-b', '--build', help="Build the Dockerfile after generation", action='store_true', default=False, required=False)
-        parser.add_argument('-c', '--color', help="Generate a color output", action='store_true', default=False, required=False)
-        parser.add_argument('-rm', '--remove', help="Remove the Dockerfile in the current working directory", action='store_true', default=False, required=False)
+        parser.add_argument('-i',  '--image',   help="Docker image to generate", default=None, required=False)
+        parser.add_argument('-v',  '--version', help="Version of the Docker image", default=None, required=False)
+        parser.add_argument('-b',  '--build',   help="Build the Dockerfile after generation", action='store_true', default=False, required=False)
+        parser.add_argument('-c',  '--color',   help="Generate a color output", action='store_true', default=False, required=False)
+        parser.add_argument('-rm', '--remove',  help="Remove the Dockerfile in the current working directory", action='store_true', default=False, required=False)
         args = parser.parse_args()
 
         v = "0.2.0"
 
         banner = \
         f"""
          _____ _     _       _                       _   _____  _     _____ 
@@ -128,16 +127,16 @@
          `--. \ '_ \| | '_ \| |/ _` |/ _` | '_ ` _ \| | | |    | |     | |  
         /\__/ / | | | | | | | | (_| | (_| | | | | | | | | \__/\| |_____| |_ 
         \____/|_| |_|_|_| |_|_|\__, |\__,_|_| |_| |_|_|  \____/\_____/\___/ 
                                 __/ |                                       
                                |___/                                        
 
         Shinigami CLI | v{v}
-        Author: https://github.com/azazelm3dj3d
-        Learn more: https://github.com/shinigamilib/shinigami
+        Author: https://github.com/battleoverflow
+        Learn more: https://github.com/battleoverflow/shinigami
         """
 
         print(banner)
 
         if args.remove:
             return Shinigami().remove_dockerfile()
```

