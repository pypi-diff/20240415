# Comparing `tmp/redisea-1.2.33.tar.gz` & `tmp/redisea-1.2.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redisea-1.2.33.tar", last modified: Fri Dec 30 05:55:16 2022, max compression
+gzip compressed data, was "redisea-1.2.34.tar", last modified: Mon Apr 15 04:12:24 2024, max compression
```

## Comparing `redisea-1.2.33.tar` & `redisea-1.2.34.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 05:55:16.592154 redisea-1.2.33/
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1069 2022-12-30 05:35:33.000000 redisea-1.2.33/LICENSE
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1447 2022-12-30 05:55:16.592154 redisea-1.2.33/PKG-INFO
--rw-rw-r--   0 azazel    (1000) azazel    (1000)      903 2022-12-30 05:39:46.000000 redisea-1.2.33/README.md
-drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 05:55:16.592154 redisea-1.2.33/redisea/
--rw-rw-r--   0 azazel    (1000) azazel    (1000)      103 2022-12-30 05:35:33.000000 redisea-1.2.33/redisea/__init__.py
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     8764 2022-12-30 05:35:33.000000 redisea-1.2.33/redisea/redisea.py
-drwxrwxr-x   0 azazel    (1000) azazel    (1000)        0 2022-12-30 05:55:16.592154 redisea-1.2.33/redisea.egg-info/
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1447 2022-12-30 05:55:16.000000 redisea-1.2.33/redisea.egg-info/PKG-INFO
--rw-rw-r--   0 azazel    (1000) azazel    (1000)      253 2022-12-30 05:55:16.000000 redisea-1.2.33/redisea.egg-info/SOURCES.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)        1 2022-12-30 05:55:16.000000 redisea-1.2.33/redisea.egg-info/dependency_links.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)       57 2022-12-30 05:55:16.000000 redisea-1.2.33/redisea.egg-info/entry_points.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)       27 2022-12-30 05:55:16.000000 redisea-1.2.33/redisea.egg-info/requires.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)        8 2022-12-30 05:55:16.000000 redisea-1.2.33/redisea.egg-info/top_level.txt
--rw-rw-r--   0 azazel    (1000) azazel    (1000)       38 2022-12-30 05:55:16.592154 redisea-1.2.33/setup.cfg
--rw-rw-r--   0 azazel    (1000) azazel    (1000)     1114 2022-12-30 05:36:40.000000 redisea-1.2.33/setup.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:12:24.716356 redisea-1.2.34/
+-rw-r--r--   0 azazel     (501) staff       (20)     1076 2024-04-15 04:08:56.000000 redisea-1.2.34/LICENSE
+-rw-r--r--   0 azazel     (501) staff       (20)     1525 2024-04-15 04:12:24.716130 redisea-1.2.34/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      906 2024-04-15 04:10:10.000000 redisea-1.2.34/README.md
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:12:24.714756 redisea-1.2.34/redisea/
+-rw-r--r--   0 azazel     (501) staff       (20)      108 2024-04-15 04:10:15.000000 redisea-1.2.34/redisea/__init__.py
+-rw-r--r--   0 azazel     (501) staff       (20)     8773 2024-04-15 04:12:14.000000 redisea-1.2.34/redisea/redisea.py
+drwxr-xr-x   0 azazel     (501) staff       (20)        0 2024-04-15 04:12:24.715894 redisea-1.2.34/redisea.egg-info/
+-rw-r--r--   0 azazel     (501) staff       (20)     1525 2024-04-15 04:12:24.000000 redisea-1.2.34/redisea.egg-info/PKG-INFO
+-rw-r--r--   0 azazel     (501) staff       (20)      253 2024-04-15 04:12:24.000000 redisea-1.2.34/redisea.egg-info/SOURCES.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        1 2024-04-15 04:12:24.000000 redisea-1.2.34/redisea.egg-info/dependency_links.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       57 2024-04-15 04:12:24.000000 redisea-1.2.34/redisea.egg-info/entry_points.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       27 2024-04-15 04:12:24.000000 redisea-1.2.34/redisea.egg-info/requires.txt
+-rw-r--r--   0 azazel     (501) staff       (20)        8 2024-04-15 04:12:24.000000 redisea-1.2.34/redisea.egg-info/top_level.txt
+-rw-r--r--   0 azazel     (501) staff       (20)       38 2024-04-15 04:12:24.716399 redisea-1.2.34/setup.cfg
+-rw-r--r--   0 azazel     (501) staff       (20)     1123 2024-04-15 04:11:47.000000 redisea-1.2.34/setup.py
```

### Comparing `redisea-1.2.33/LICENSE` & `redisea-1.2.34/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 azazelm3dj3d
+Copyright (c) 2022-2024 battleoverflow
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `redisea-1.2.33/PKG-INFO` & `redisea-1.2.34/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: redisea
-Version: 1.2.33
+Version: 1.2.34
 Summary: RediSea is a Redis (in-memory database) communication framework used for dumping key/value information within the Redis server, real-time Redis database analysis, and much more.
-Home-page: https://github.com/azazelm3dj3d/RediSea
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/RediSea
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: redis
+Requires-Dist: prettytable
 
-<img src="https://raw.githubusercontent.com/azazelm3dj3d/RediSea/main/assets/redisea_banner_v3.png">
+<img src="https://raw.githubusercontent.com/battleoverflow/RediSea/main/assets/redisea_banner_v3.png">
 
 RediSea is a Redis (in-memory database) communication framework used for viewing Redis keys, dumping Redis keys, dumping key information about the Redis server, real-time Redis database analysis, and much more!
 
 Please note, this framework does work even if a Redis instance is not present. There is also an option for remotely connecting to a Redis instance.
 
 RediSea is available through pip:
 ```bash
```

### Comparing `redisea-1.2.33/redisea/redisea.py` & `redisea-1.2.34/redisea/redisea.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 
 """
-    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Owner: battleoverflow (https://github.com/battleoverflow)
     Project: RediSea
     License: MIT
 """
 
 import redis, time, sys, os, platform, argparse
 
 from subprocess import getoutput
 from prettytable import PrettyTable
 
 r = redis.Redis()
-author = 'azazelm3dj3d'
-version = '1.2.32'
+author = 'battleoverflow'
+version = '1.2.34'
 
 class RediSea:
 
     def banner(self):
         print("""
             ██████╗ ███████╗██████╗ ██╗███████╗███████╗ █████╗ 
             ██╔══██╗██╔════╝██╔══██╗██║██╔════╝██╔════╝██╔══██╗
@@ -181,19 +181,19 @@
                     print("b, banner    Displays our cool banner!")
                     print("i, info      Return general information about the Redis instance")
                     print("r, remote    Remotely connect to a Redis instance")
                     print("rt, realtime View Redis data update in real-time\n")
             
             except KeyboardInterrupt:
                 print("\n\nThank you for using RediSea!\n")
-                print(f"Author: {author} (https://github.com/azazelm3dj3d)")
+                print(f"Author: {author} (https://github.com/battleoverflow)")
                 print(f"Version: {version}")
                 time.sleep(0.2)
                 sys.exit(0)
 
     def main():
         rs = RediSea()
         rs.banner()
         rs.redis_comms()
 
 if __name__ == '__main__':
-    RediSea.main()
+    RediSea.main()
```

### Comparing `redisea-1.2.33/redisea.egg-info/PKG-INFO` & `redisea-1.2.34/redisea.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: redisea
-Version: 1.2.33
+Version: 1.2.34
 Summary: RediSea is a Redis (in-memory database) communication framework used for dumping key/value information within the Redis server, real-time Redis database analysis, and much more.
-Home-page: https://github.com/azazelm3dj3d/RediSea
-Author: azazelm3dj3d
+Home-page: https://github.com/battleoverflow/RediSea
+Author: battleoverflow
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: argparse
+Requires-Dist: redis
+Requires-Dist: prettytable
 
-<img src="https://raw.githubusercontent.com/azazelm3dj3d/RediSea/main/assets/redisea_banner_v3.png">
+<img src="https://raw.githubusercontent.com/battleoverflow/RediSea/main/assets/redisea_banner_v3.png">
 
 RediSea is a Redis (in-memory database) communication framework used for viewing Redis keys, dumping Redis keys, dumping key information about the Redis server, real-time Redis database analysis, and much more!
 
 Please note, this framework does work even if a Redis instance is not present. There is also an option for remotely connecting to a Redis instance.
 
 RediSea is available through pip:
 ```bash
```

### Comparing `redisea-1.2.33/setup.py` & `redisea-1.2.34/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
-    Owner: azazelm3dj3d (https://github.com/azazelm3dj3d)
+    Owner: battleoverflow (https://github.com/battleoverflow)
     Project: RediSea
     License: MIT
 """
 
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "redisea",
-    version = "1.2.33",
-    author = "azazelm3dj3d",
+    version = "1.2.34",
+    author = "battleoverflow",
     description = "RediSea is a Redis (in-memory database) communication framework used for dumping key/value information within the Redis server, real-time Redis database analysis, and much more.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/azazelm3dj3d/RediSea",
+    url = "https://github.com/battleoverflow/RediSea",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages = [
         "redisea"
@@ -31,8 +31,8 @@
         "prettytable"
     ],
     scripts=["redisea/redisea.py"],
     entry_points={
         'console_scripts': ["redisea=redisea.redisea:RediSea.main"]
     },
     python_requires = ">=3.6"
-)
+)
```

