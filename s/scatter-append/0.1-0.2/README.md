# Comparing `tmp/scatter_append-0.1.tar.gz` & `tmp/scatter_append-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatter_append-0.1.tar", last modified: Mon Apr 15 04:40:15 2024, max compression
+gzip compressed data, was "scatter_append-0.2.tar", last modified: Mon Apr 15 05:32:00 2024, max compression
```

## Comparing `scatter_append-0.1.tar` & `scatter_append-0.2.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 04:40:15.871816 scatter_append-0.1/
--rw-r--r--   0 taco      (1000) taco      (1000)      390 2024-04-15 04:40:15.871816 scatter_append-0.1/PKG-INFO
-drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 04:40:15.867816 scatter_append-0.1/scatter_append/
--rw-rw-r--   0 taco      (1000) taco      (1000)       70 2024-04-15 04:35:42.000000 scatter_append-0.1/scatter_append/__init__.py
--rw-rw-r--   0 taco      (1000) taco      (1000)      640 2024-04-15 04:35:42.000000 scatter_append-0.1/scatter_append/scatter_append.py
-drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 04:40:15.867816 scatter_append-0.1/scatter_append.egg-info/
--rw-r--r--   0 taco      (1000) taco      (1000)      390 2024-04-15 04:40:15.000000 scatter_append-0.1/scatter_append.egg-info/PKG-INFO
--rw-rw-r--   0 taco      (1000) taco      (1000)      220 2024-04-15 04:40:15.000000 scatter_append-0.1/scatter_append.egg-info/SOURCES.txt
--rw-rw-r--   0 taco      (1000) taco      (1000)        1 2024-04-15 04:40:15.000000 scatter_append-0.1/scatter_append.egg-info/dependency_links.txt
--rw-rw-r--   0 taco      (1000) taco      (1000)       15 2024-04-15 04:40:15.000000 scatter_append-0.1/scatter_append.egg-info/top_level.txt
--rw-rw-r--   0 taco      (1000) taco      (1000)       38 2024-04-15 04:40:15.871816 scatter_append-0.1/setup.cfg
--rw-rw-r--   0 taco      (1000) taco      (1000)      514 2024-04-15 04:35:42.000000 scatter_append-0.1/setup.py
+drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 05:32:00.622969 scatter_append-0.2/
+-rw-r--r--   0 taco      (1000) taco      (1000)      390 2024-04-15 05:32:00.622969 scatter_append-0.2/PKG-INFO
+drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 05:32:00.622969 scatter_append-0.2/scatter_append/
+-rw-rw-r--   0 taco      (1000) taco      (1000)       70 2024-04-15 04:35:42.000000 scatter_append-0.2/scatter_append/__init__.py
+-rw-rw-r--   0 taco      (1000) taco      (1000)      740 2024-04-15 05:25:37.000000 scatter_append-0.2/scatter_append/scatter_append.py
+drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 05:32:00.622969 scatter_append-0.2/scatter_append.egg-info/
+-rw-r--r--   0 taco      (1000) taco      (1000)      390 2024-04-15 05:32:00.000000 scatter_append-0.2/scatter_append.egg-info/PKG-INFO
+-rw-rw-r--   0 taco      (1000) taco      (1000)      233 2024-04-15 05:32:00.000000 scatter_append-0.2/scatter_append.egg-info/SOURCES.txt
+-rw-rw-r--   0 taco      (1000) taco      (1000)        1 2024-04-15 05:32:00.000000 scatter_append-0.2/scatter_append.egg-info/dependency_links.txt
+-rw-rw-r--   0 taco      (1000) taco      (1000)       15 2024-04-15 05:32:00.000000 scatter_append-0.2/scatter_append.egg-info/top_level.txt
+-rw-rw-r--   0 taco      (1000) taco      (1000)       38 2024-04-15 05:32:00.622969 scatter_append-0.2/setup.cfg
+-rw-rw-r--   0 taco      (1000) taco      (1000)      514 2024-04-15 05:31:11.000000 scatter_append-0.2/setup.py
+drwxrwxr-x   0 taco      (1000) taco      (1000)        0 2024-04-15 05:32:00.622969 scatter_append-0.2/test/
+-rw-rw-r--   0 taco      (1000) taco      (1000)     1098 2024-04-15 05:28:48.000000 scatter_append-0.2/test/test.py
```

### Comparing `scatter_append-0.1/scatter_append/scatter_append.py` & `scatter_append-0.2/scatter_append/scatter_append.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
+from typing import MutableSequence, Any, Tuple
 
-from typing import Sequence, MutableSequence, Any, Tuple
 
 class ScatterAppend:
     @classmethod
-    def make_n(cls, n : int):
+    def make_n(cls, n: int):
         return cls(*tuple([] for _ in range(n)))
 
     def __init__(self, *refs: MutableSequence[Any]) -> None:
         self.refs = refs
 
-    def __iadd__(self, others: Sequence[Any]):
+    def __iadd__(self, others: tuple[Any, ...]):
         for ref, o in zip(self.refs, others):
             ref.append(o)
         return self
 
-    def __getitem__(self, i : int):
+    def __getitem__(self, i: int):
         return self.refs[i]
-    
+
     def __repr__(self):
         return str([x for x in self.refs])
-    
-    def get(self, index : int) -> Tuple[Any]:
-        return tuple(x[index] for x in self.refs)
+
+    def get(self, index: int) -> tuple[Any, ...]:
+        return tuple(x[index] for x in self.refs)
+
+    def size(self, i=None):
+        return tuple(len(x) for x in self.refs) if i is None else len(self.refs[i])
```

### Comparing `scatter_append-0.1/setup.py` & `scatter_append-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='scatter-append',
-    version='0.1',
+    version='0.2',
     description='A utility for scatter appending to mutable sequences.',
     author='Rhys Newbury, Bryce Ferenczi',
     author_email='rhys.newbury@monash.edu, bryce.ferenczi@monash.edu',
     packages=find_packages(),
     python_requires='>=3.6',
     classifiers=[
         'Programming Language :: Python :: 3',
```

