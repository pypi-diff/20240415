# Comparing `tmp/funccache-2.0.1.tar.gz` & `tmp/funccache-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funccache-2.0.1.tar", last modified: Mon Apr 15 01:13:58 2024, max compression
+gzip compressed data, was "funccache-2.0a1.tar", last modified: Mon Apr  1 02:09:47 2024, max compression
```

## Comparing `funccache-2.0.1.tar` & `funccache-2.0a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:13:58.268072 funccache-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-15 01:13:54.000000 funccache-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-15 01:13:58.268072 funccache-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-15 01:13:54.000000 funccache-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:13:58.268072 funccache-2.0.1/funccache/
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-15 01:13:54.000000 funccache-2.0.1/funccache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17563 2024-04-15 01:13:54.000000 funccache-2.0.1/funccache/i funccache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:13:58.268072 funccache-2.0.1/funccache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-15 01:13:58.000000 funccache-2.0.1/funccache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 01:13:58.000000 funccache-2.0.1/funccache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:13:58.000000 funccache-2.0.1/funccache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 01:13:58.000000 funccache-2.0.1/funccache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:13:58.268072 funccache-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-15 01:13:54.000000 funccache-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:09:47.288896 funccache-2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-01 02:09:43.000000 funccache-2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-01 02:09:47.288896 funccache-2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-01 02:09:43.000000 funccache-2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:09:47.288896 funccache-2.0a1/funccache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 02:09:43.000000 funccache-2.0a1/funccache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-01 02:09:43.000000 funccache-2.0a1/funccache/i funccache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:09:47.288896 funccache-2.0a1/funccache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 02:09:47.288896 funccache-2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-01 02:09:43.000000 funccache-2.0a1/setup.py
```

### Comparing `funccache-2.0.1/LICENSE` & `funccache-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `funccache-2.0.1/PKG-INFO` & `funccache-2.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 2.0.1
-Summary: True to its name, `funccache` implements the cache function. Cache the return value of a callable object or all methods defined in a class.
+Version: 2.0a1
+Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/funccache.svg?style=flat-square")](https://github.com/gqylpy/funccache/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/funccache)](https://pypi.org/project/funccache)
 [![License](https://img.shields.io/pypi/l/funccache)](https://github.com/gqylpy/funccache/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/funccache)](https://pepy.tech/project/funccache)
 
 # funccache
-English | [中文](https://github.com/gqylpy/funccache/blob/master/README_CN.md)
+English | [中文](README_CN.md)
 
 `funccache`, as its name suggests, is a framework developed by the GQYLPY team that implements function caching. It can cache the return values of specific functions or all methods defined within a class.
 
 > _What if you have a function in your program that gets called multiple times and always returns the same value? To improve code efficiency, you might call the function once, store the return value in a variable, and then use that variable instead of repeatedly calling the function. Sound familiar? That's great! But now, we're here to introduce a more elegant solution: using the `funccache` module to directly cache function return values._
 
 `funccache` can be used in two ways: as a metaclass to cache the return values of all methods defined in its metaclass instances, or as a decorator to cache the return values of decorated functions.
```

### Comparing `funccache-2.0.1/README.md` & `funccache-2.0a1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/funccache.svg?style=flat-square")](https://github.com/gqylpy/funccache/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/funccache)](https://pypi.org/project/funccache)
 [![License](https://img.shields.io/pypi/l/funccache)](https://github.com/gqylpy/funccache/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/funccache)](https://pepy.tech/project/funccache)
 
 # funccache
-English | [中文](https://github.com/gqylpy/funccache/blob/master/README_CN.md)
+English | [中文](README_CN.md)
 
 `funccache`, as its name suggests, is a framework developed by the GQYLPY team that implements function caching. It can cache the return values of specific functions or all methods defined within a class.
 
 > _What if you have a function in your program that gets called multiple times and always returns the same value? To improve code efficiency, you might call the function once, store the return value in a variable, and then use that variable instead of repeatedly calling the function. Sound familiar? That's great! But now, we're here to introduce a more elegant solution: using the `funccache` module to directly cache function return values._
 
 `funccache` can be used in two ways: as a metaclass to cache the return values of all methods defined in its metaclass instances, or as a decorator to cache the return values of decorated functions.
```

### Comparing `funccache-2.0.1/funccache/__init__.py` & `funccache-2.0a1/funccache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> class Alpha(metaclass=funccache):
     >>>     ...
 
     >>> @funccache
     >>> def alpha():
     >>>     ...
 
-    @version: 2.0.1
+    @version: 2.0alpha1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/funccache
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `funccache-2.0.1/funccache/i funccache.py` & `funccache-2.0a1/funccache/i funccache.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,31 +10,30 @@
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import re
-import sys
 import time
 import asyncio
 import threading
 import functools
 
 from types import MethodType, FunctionType
 
 from typing import (
     TypeVar, Type, Optional, Union, Dict, List, Tuple, Set, Iterable, Callable,
     FrozenSet, Any
 )
 
-if sys.version_info >= (3, 10):
+try:
     from typing import TypeAlias
-else:
-    TypeAlias = TypeVar("TypeAlias")
+except ImportError:
+    TypeAlias = ...
 
 MethodTypeOrName: TypeAlias = TypeVar('MethodTypeOrName', MethodType, str)
 Closure:          TypeAlias = TypeVar('Closure', bound=Callable)
 
 MethodCachePool: TypeAlias = Dict[
     Union[Tuple[str, Tuple[Tuple[Any, ...], FrozenSet[Tuple[str, Any]]]], str],
     Dict[str, Any]
```

### Comparing `funccache-2.0.1/funccache.egg-info/PKG-INFO` & `funccache-2.0a1/funccache.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 2.0.1
-Summary: True to its name, `funccache` implements the cache function. Cache the return value of a callable object or all methods defined in a class.
+Version: 2.0a1
+Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/funccache.svg?style=flat-square")](https://github.com/gqylpy/funccache/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/funccache)](https://pypi.org/project/funccache)
 [![License](https://img.shields.io/pypi/l/funccache)](https://github.com/gqylpy/funccache/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/funccache)](https://pepy.tech/project/funccache)
 
 # funccache
-English | [中文](https://github.com/gqylpy/funccache/blob/master/README_CN.md)
+English | [中文](README_CN.md)
 
 `funccache`, as its name suggests, is a framework developed by the GQYLPY team that implements function caching. It can cache the return values of specific functions or all methods defined within a class.
 
 > _What if you have a function in your program that gets called multiple times and always returns the same value? To improve code efficiency, you might call the function once, store the return value in a variable, and then use that variable instead of repeatedly calling the function. Sound familiar? That's great! But now, we're here to introduce a more elegant solution: using the `funccache` module to directly cache function return values._
 
 `funccache` can be used in two ways: as a metaclass to cache the return values of all methods defined in its metaclass instances, or as a decorator to cache the return values of decorated functions.
```

### Comparing `funccache-2.0.1/setup.py` & `funccache-2.0a1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,15 @@
     name=i.__name__,
     version=version,
     author=author,
     author_email=email,
     license='Apache 2.0',
     url='http://gqylpy.com',
     project_urls={'Source': source},
-    description='''
-        True to its name, `funccache` implements the cache function. Cache the
-        return value of a callable object or all methods defined in a class.
-    '''.strip().replace('\n       ', ''),
+    description='如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。',
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=[i.__name__],
     python_requires='>=3.8',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

