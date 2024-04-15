# Comparing `tmp/monisha-0.0.44.tar.gz` & `tmp/monisha-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.44.tar", last modified: Sun Apr 14 05:24:30 2024, max compression
+gzip compressed data, was "monisha-0.0.45.tar", last modified: Sun Apr 14 05:42:39 2024, max compression
```

## Comparing `monisha-0.0.44.tar` & `monisha-0.0.45.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:30.000549 monisha-0.0.44/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-14 05:24:25.000000 monisha-0.0.44/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.992549 monisha-0.0.44/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.996549 monisha-0.0.44/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/functions/function14.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.996549 monisha-0.0.44/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 05:24:25.000000 monisha-0.0.44/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 05:24:29.996549 monisha-0.0.44/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 05:24:25.000000 monisha-0.0.44/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:24:29.996549 monisha-0.0.44/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 05:24:29.000000 monisha-0.0.44/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:24:30.000549 monisha-0.0.44/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-14 05:24:25.000000 monisha-0.0.44/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:42:39.556290 monisha-0.0.45/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-14 05:42:35.000000 monisha-0.0.45/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:42:39.552290 monisha-0.0.45/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:42:39.552290 monisha-0.0.45/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/functions/function14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:42:39.556290 monisha-0.0.45/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 05:42:35.000000 monisha-0.0.45/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 05:42:39.556290 monisha-0.0.45/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 05:42:35.000000 monisha-0.0.45/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:42:39.556290 monisha-0.0.45/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-14 05:42:39.000000 monisha-0.0.45/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 05:42:39.000000 monisha-0.0.45/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:42:39.000000 monisha-0.0.45/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:42:39.000000 monisha-0.0.45/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 05:42:39.000000 monisha-0.0.45/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:42:39.556290 monisha-0.0.45/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-14 05:42:35.000000 monisha-0.0.45/setup.py
```

### Comparing `monisha-0.0.44/LICENSE` & `monisha-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/__init__.py` & `monisha-0.0.45/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function01.py` & `monisha-0.0.45/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function02.py` & `monisha-0.0.45/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function03.py` & `monisha-0.0.45/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function04.py` & `monisha-0.0.45/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function06.py` & `monisha-0.0.45/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function07.py` & `monisha-0.0.45/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function10.py` & `monisha-0.0.45/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/Monisha/functions/function14.py` & `monisha-0.0.45/Monisha/functions/function14.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 from ..scripts.en import Scripted
 #===========================================================================
 
 async def CDirectory(dname=Folder.DATA07, fname=Scripted.DATA01):
     name01 = str(dname)
     name02 = str(fname)
     osemse = os.getcwd()
-    moonse = os.path.join(osemse, name01) + name02
+    rooted = Scripted.DATA01
+    moonse = os.path.join(osemse, name01, rooted) + name02
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
     return moonse
 
 #===========================================================================
 
 async def UDirectory(dname=Folder.DATA07, fname=Scripted.DATA01):
     name01 = str(dname)
     name02 = str(fname)
     osemse = os.getcwd()
+    rooted = Scripted.DATA01
     timeso = str(round(time.time()))
-    moonse = os.path.join(osemse, name01, timeso) + name02
+    moonse = os.path.join(osemse, name01, timeso, rooted) + name02
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
     return moonse
 
 #===========================================================================
 
 async def BDirectory(uid, dname=Folder.DATA07, fname=Scripted.DATA01):
     usered = str(uid)
     name01 = str(dname)
     name02 = str(fname)
     osemse = os.getcwd()
+    rooted = Scripted.DATA01
     timeso = str(round(time.time()))
-    moonse = os.path.join(osemse, name01, usered, timeso) + name02
+    moonse = os.path.join(osemse, name01, usered, timeso, rooted) + name02
     moonse if os.path.isdir(moonse) else os.makedirs(moonse)
     return moonse
 
 #===========================================================================
```

### Comparing `monisha-0.0.44/Monisha/scripts/es.py` & `monisha-0.0.45/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/PKG-INFO` & `monisha-0.0.45/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.44
+Version: 0.0.45
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.44 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.45 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `monisha-0.0.44/monisha.egg-info/PKG-INFO` & `monisha-0.0.45/monisha.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.44
+Version: 0.0.45
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.44 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.45 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `monisha-0.0.44/monisha.egg-info/SOURCES.txt` & `monisha-0.0.45/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.44/setup.py` & `monisha-0.0.45/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
     description='ㅤ',
-    version='0.0.44',
+    version='0.0.45',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.10',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     url='https://github.com/Clinton-Abraham',
```

