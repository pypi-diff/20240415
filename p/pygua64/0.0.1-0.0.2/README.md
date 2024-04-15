# Comparing `tmp/pygua64-0.0.1.tar.gz` & `tmp/pygua64-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/lizongying/IdeaProjects/pygua64/dist/tmpbrqqr_gy/pygua64-0.0.1.tar", last modified: Fri Dec 10 07:00:34 2021, max compression
+gzip compressed data, was "pygua64-0.0.2.tar", last modified: Mon Apr 15 19:32:51 2024, max compression
```

## Comparing `pygua64-0.0.1.tar` & `pygua64-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 lizongying   (501) staff       (20)        0 2021-12-10 07:00:34.307386 pygua64-0.0.1/
--rw-r--r--   0 lizongying   (501) staff       (20)     1066 2021-12-10 06:59:17.000000 pygua64-0.0.1/LICENSE
--rw-r--r--   0 lizongying   (501) staff       (20)      747 2021-12-10 07:00:34.307661 pygua64-0.0.1/PKG-INFO
--rw-r--r--   0 lizongying   (501) staff       (20)      239 2021-12-10 07:00:10.000000 pygua64-0.0.1/README.md
--rw-r--r--   0 lizongying   (501) staff       (20)      103 2021-12-10 06:11:46.000000 pygua64-0.0.1/pyproject.toml
--rw-r--r--   0 lizongying   (501) staff       (20)      596 2021-12-10 07:00:34.308880 pygua64-0.0.1/setup.cfg
-drwxr-xr-x   0 lizongying   (501) staff       (20)        0 2021-12-10 07:00:34.292492 pygua64-0.0.1/src/
-drwxr-xr-x   0 lizongying   (501) staff       (20)        0 2021-12-10 07:00:34.297390 pygua64-0.0.1/src/pygua64/
--rw-r--r--   0 lizongying   (501) staff       (20)       15 2021-12-10 04:43:04.000000 pygua64-0.0.1/src/pygua64/__init__.py
--rw-r--r--   0 lizongying   (501) staff       (20)     2208 2021-12-10 06:56:31.000000 pygua64-0.0.1/src/pygua64/gua64.py
-drwxr-xr-x   0 lizongying   (501) staff       (20)        0 2021-12-10 07:00:34.306411 pygua64-0.0.1/src/pygua64.egg-info/
--rw-r--r--   0 lizongying   (501) staff       (20)      747 2021-12-10 07:00:34.000000 pygua64-0.0.1/src/pygua64.egg-info/PKG-INFO
--rw-r--r--   0 lizongying   (501) staff       (20)      227 2021-12-10 07:00:34.000000 pygua64-0.0.1/src/pygua64.egg-info/SOURCES.txt
--rw-r--r--   0 lizongying   (501) staff       (20)        1 2021-12-10 07:00:34.000000 pygua64-0.0.1/src/pygua64.egg-info/dependency_links.txt
--rw-r--r--   0 lizongying   (501) staff       (20)        8 2021-12-10 07:00:34.000000 pygua64-0.0.1/src/pygua64.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:32:51.469637 pygua64-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-15 19:32:48.000000 pygua64-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-15 19:32:51.469637 pygua64-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-15 19:32:48.000000 pygua64-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 19:32:48.000000 pygua64-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-15 19:32:51.469637 pygua64-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:32:51.465637 pygua64-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:32:51.469637 pygua64-0.0.2/src/pygua64/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 19:32:48.000000 pygua64-0.0.2/src/pygua64/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-15 19:32:48.000000 pygua64-0.0.2/src/pygua64/gua64.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:32:51.469637 pygua64-0.0.2/src/pygua64.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-15 19:32:51.000000 pygua64-0.0.2/src/pygua64.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 19:32:51.000000 pygua64-0.0.2/src/pygua64.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:32:51.000000 pygua64-0.0.2/src/pygua64.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 19:32:51.000000 pygua64-0.0.2/src/pygua64.egg-info/top_level.txt
```

### Comparing `pygua64-0.0.1/LICENSE` & `pygua64-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygua64-0.0.1/PKG-INFO` & `pygua64-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 Metadata-Version: 2.1
 Name: pygua64
-Version: 0.0.1
-Summary: 64卦
+Version: 0.0.2
+Summary: 六十四卦编码，python实现。
 Home-page: https://github.com/lizongying/pygua64
 Author: Li ZongYing
 Author-email: lizongying@msn.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/lizongying/pygua64/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 64卦
+# 六十四卦编码
 
-代替base64
+六十四卦编码，python实现。
+如：“hello，世界”会编码为“䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒〇”。
+
+## all language
+
+* [golang](https://github.com/lizongying/go-gua64)
+* [js](https://github.com/lizongying/js-gua64)
+* [java](https://github.com/lizongying/java-gua64)
+* [php-gua64](https://github.com/lizongying/php-gua64)
+* [python](https://github.com/lizongying/pygua64)
+
+## install
+
+```
+pip install pygua64
+```
 
 ## example
 
 ```
 from pygua64 import gua64
 r = gua64.encode('hello，世界'.encode())
 print(r.decode())
 
-r = gua64.decode('䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒☯'.encode())
+r = gua64.decode('䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒〇'.encode())
 print(r.decode())
-```
 
+r = verify('䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒〇')
+print(r)
+```
```

### Comparing `pygua64-0.0.1/src/pygua64.egg-info/PKG-INFO` & `pygua64-0.0.2/src/pygua64.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 Metadata-Version: 2.1
 Name: pygua64
-Version: 0.0.1
-Summary: 64卦
+Version: 0.0.2
+Summary: 六十四卦编码，python实现。
 Home-page: https://github.com/lizongying/pygua64
 Author: Li ZongYing
 Author-email: lizongying@msn.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/lizongying/pygua64/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# 64卦
+# 六十四卦编码
 
-代替base64
+六十四卦编码，python实现。
+如：“hello，世界”会编码为“䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒〇”。
+
+## all language
+
+* [golang](https://github.com/lizongying/go-gua64)
+* [js](https://github.com/lizongying/js-gua64)
+* [java](https://github.com/lizongying/java-gua64)
+* [php-gua64](https://github.com/lizongying/php-gua64)
+* [python](https://github.com/lizongying/pygua64)
+
+## install
+
+```
+pip install pygua64
+```
 
 ## example
 
 ```
 from pygua64 import gua64
 r = gua64.encode('hello，世界'.encode())
 print(r.decode())
 
-r = gua64.decode('䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒☯'.encode())
+r = gua64.decode('䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒〇'.encode())
 print(r.decode())
-```
 
+r = verify('䷯䷬䷿䷶䷸䷬䷀䷌䷌䷎䷼䷲䷰䷳䷸䷘䷔䷭䷒〇')
+print(r)
+```
```

