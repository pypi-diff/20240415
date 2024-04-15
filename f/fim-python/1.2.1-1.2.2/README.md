# Comparing `tmp/fim-python-1.2.1.tar.gz` & `tmp/fim_python-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fim-python-1.2.1.tar", last modified: Sun Mar 24 23:13:27 2024, max compression
+gzip compressed data, was "fim_python-1.2.2.tar", last modified: Mon Apr 15 09:46:21 2024, max compression
```

## Comparing `fim-python-1.2.1.tar` & `fim_python-1.2.2.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.018693 fim-python-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-24 23:13:19.000000 fim-python-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-03-24 23:13:27.018693 fim-python-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-03-24 23:13:19.000000 fim-python-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.014693 fim-python-1.2.1/fim_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-03-24 23:13:27.000000 fim-python-1.2.1/fim_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-24 23:13:27.000000 fim-python-1.2.1/fim_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 23:13:27.000000 fim-python-1.2.1/fim_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-24 23:13:27.000000 fim-python-1.2.1/fim_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-24 23:13:27.000000 fim-python-1.2.1/fim_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.010693 fim-python-1.2.1/fimpy/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/cupy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/fim_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    20956 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/fim_cupy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.010693 fim-python-1.2.1/fimpy/fim_cutils/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/fim_cutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1092467 2024-03-24 23:13:25.000000 fim-python-1.2.1/fimpy/fim_cutils/fim_cutils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/fim_np.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.014693 fim-python-1.2.1/fimpy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/utils/comp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.014693 fim-python-1.2.1/fimpy/utils/cython/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/utils/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1391833 2024-03-24 23:13:26.000000 fim-python-1.2.1/fimpy/utils/cython/comp.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-24 23:13:19.000000 fim-python-1.2.1/fimpy/utils/tsitsiklis.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-24 23:13:19.000000 fim-python-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 23:13:27.018693 fim-python-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-03-24 23:13:19.000000 fim-python-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 23:13:27.014693 fim-python-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-03-24 23:13:19.000000 fim-python-1.2.1/tests/test_custom_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-24 23:13:19.000000 fim-python-1.2.1/tests/test_cython_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-03-24 23:13:19.000000 fim-python-1.2.1/tests/test_fim_solvers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.040136 fim_python-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-15 09:46:14.000000 fim_python-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 09:46:14.000000 fim_python-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-15 09:46:21.040136 fim_python-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-15 09:46:14.000000 fim_python-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.040136 fim_python-1.2.2/fim_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-04-15 09:46:21.000000 fim_python-1.2.2/fim_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-15 09:46:21.000000 fim_python-1.2.2/fim_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:46:21.000000 fim_python-1.2.2/fim_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 09:46:21.000000 fim_python-1.2.2/fim_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 09:46:21.000000 fim_python-1.2.2/fim_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.036136 fim_python-1.2.2/fimpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/cupy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21361 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/fim_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20956 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/fim_cupy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.036136 fim_python-1.2.2/fimpy/fim_cutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/fim_cutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1093286 2024-04-15 09:46:19.000000 fim_python-1.2.2/fimpy/fim_cutils/fim_cutils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/fim_cutils/fim_cutils.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/fim_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.036136 fim_python-1.2.2/fimpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/utils/comp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.040136 fim_python-1.2.2/fimpy/utils/cython/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/utils/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1392652 2024-04-15 09:46:20.000000 fim_python-1.2.2/fimpy/utils/cython/comp.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/utils/cython/comp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-15 09:46:14.000000 fim_python-1.2.2/fimpy/utils/tsitsiklis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 09:46:14.000000 fim_python-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 09:46:21.040136 fim_python-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-15 09:46:14.000000 fim_python-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:46:21.040136 fim_python-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-04-15 09:46:14.000000 fim_python-1.2.2/tests/test_custom_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-15 09:46:14.000000 fim_python-1.2.2/tests/test_cython_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-15 09:46:14.000000 fim_python-1.2.2/tests/test_fim_solvers.py
```

### Comparing `fim-python-1.2.1/LICENSE` & `fim_python-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/PKG-INFO` & `fim_python-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fim-python
-Version: 1.2.1
+Version: 1.2.2
 Summary: This repository implements the Fast Iterative Method on tetrahedral domains and triangulated surfaces purely in python both for CPU (numpy) and GPU (cupy).
 Home-page: https://github.com/thomgrand/fim-python
 Author: Thomas Grandits
 Author-email: tomdev@gmx.net
 License: AGPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `fim-python-1.2.1/README.md` & `fim_python-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fim_python.egg-info/PKG-INFO` & `fim_python-1.2.2/fim_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fim-python
-Version: 1.2.1
+Version: 1.2.2
 Summary: This repository implements the Fast Iterative Method on tetrahedral domains and triangulated surfaces purely in python both for CPU (numpy) and GPU (cupy).
 Home-page: https://github.com/thomgrand/fim-python
 Author: Thomas Grandits
 Author-email: tomdev@gmx.net
 License: AGPL
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
```

### Comparing `fim-python-1.2.1/fim_python.egg-info/SOURCES.txt` & `fim_python-1.2.2/fim_python.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 fim_python.egg-info/PKG-INFO
 fim_python.egg-info/SOURCES.txt
 fim_python.egg-info/dependency_links.txt
 fim_python.egg-info/requires.txt
@@ -11,15 +12,17 @@
 fimpy/cupy_kernels.py
 fimpy/fim_base.py
 fimpy/fim_cupy.py
 fimpy/fim_np.py
 fimpy/solver.py
 fimpy/fim_cutils/__init__.py
 fimpy/fim_cutils/fim_cutils.cpp
+fimpy/fim_cutils/fim_cutils.pyx
 fimpy/utils/__init__.py
 fimpy/utils/comp.py
 fimpy/utils/tsitsiklis.py
 fimpy/utils/cython/__init__.py
 fimpy/utils/cython/comp.cpp
+fimpy/utils/cython/comp.pyx
 tests/test_custom_kernels.py
 tests/test_cython_methods.py
 tests/test_fim_solvers.py
```

### Comparing `fim-python-1.2.1/fimpy/cupy_kernels.py` & `fim_python-1.2.2/fimpy/cupy_kernels.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fimpy/fim_base.py` & `fim_python-1.2.2/fimpy/fim_base.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fimpy/fim_cupy.py` & `fim_python-1.2.2/fimpy/fim_cupy.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fimpy/fim_cutils/fim_cutils.cpp` & `fim_python-1.2.2/fimpy/fim_cutils/fim_cutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "extra_compile_args": [
             "-O3",
             "-fopenmp"
@@ -40,18 +40,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -135,14 +135,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -196,14 +198,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -257,60 +261,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -393,14 +420,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `fim-python-1.2.1/fimpy/fim_np.py` & `fim_python-1.2.2/fimpy/fim_np.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fimpy/solver.py` & `fim_python-1.2.2/fimpy/solver.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fimpy/utils/comp.py` & `fim_python-1.2.2/fimpy/utils/comp.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/fimpy/utils/cython/comp.cpp` & `fim_python-1.2.2/fimpy/utils/cython/comp.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.9 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O3",
@@ -41,18 +41,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_9" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030009F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -136,14 +136,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -197,14 +199,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -258,60 +262,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -394,14 +421,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
```

### Comparing `fim-python-1.2.1/fimpy/utils/tsitsiklis.py` & `fim_python-1.2.2/fimpy/utils/tsitsiklis.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/setup.py` & `fim_python-1.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 lib_requires_gpu = ["cupy>=9.0"]
 test_requires_cpu = ["scipy", "pytest", "pytest-cov", "matplotlib", "pandas", "ipython"]    
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as readme:
      long_description = readme.read()
 
 setup(name="fim-python",
-    version="1.2.1",    
+    version="1.2.2",    
     description="This repository implements the Fast Iterative Method on tetrahedral domains and triangulated surfaces purely in python both for CPU (numpy) and GPU (cupy).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/thomgrand/fim-python",
     packages=["fimpy", "fimpy.utils", "fimpy.fim_cutils", "fimpy.utils.cython"],
     install_requires=lib_requires_cpu,
     classifiers=[
```

### Comparing `fim-python-1.2.1/tests/test_custom_kernels.py` & `fim_python-1.2.2/tests/test_custom_kernels.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/tests/test_cython_methods.py` & `fim_python-1.2.2/tests/test_cython_methods.py`

 * *Files identical despite different names*

### Comparing `fim-python-1.2.1/tests/test_fim_solvers.py` & `fim_python-1.2.2/tests/test_fim_solvers.py`

 * *Files identical despite different names*

