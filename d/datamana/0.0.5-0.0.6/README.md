# Comparing `tmp/datamana-0.0.5.tar.gz` & `tmp/datamana-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.0.5.tar", last modified: Sun Apr 14 11:07:29 2024, max compression
+gzip compressed data, was "datamana-0.0.6.tar", last modified: Mon Apr 15 12:57:32 2024, max compression
```

## Comparing `datamana-0.0.5.tar` & `datamana-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.208389 datamana-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-14 11:07:19.000000 datamana-0.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 11:07:19.000000 datamana-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 11:07:29.204389 datamana-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:19.000000 datamana-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.204389 datamana-0.0.5/csrc/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-14 11:07:19.000000 datamana-0.0.5/csrc/mqueue.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-14 11:07:19.000000 datamana-0.0.5/csrc/python.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-14 11:07:19.000000 datamana-0.0.5/csrc/semaphore.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.204389 datamana-0.0.5/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:19.000000 datamana-0.0.5/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:19.000000 datamana-0.0.5/datamana/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-14 11:07:19.000000 datamana-0.0.5/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:07:29.204389 datamana-0.0.5/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 11:07:29.000000 datamana-0.0.5/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 11:07:19.000000 datamana-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:07:29.208389 datamana-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-14 11:07:19.000000 datamana-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.838795 datamana-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-15 12:57:19.000000 datamana-0.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 12:57:19.000000 datamana-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-15 12:57:32.838795 datamana-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:19.000000 datamana-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.834795 datamana-0.0.6/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-15 12:57:19.000000 datamana-0.0.6/csrc/mqueue.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 12:57:19.000000 datamana-0.0.6/csrc/python.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-15 12:57:19.000000 datamana-0.0.6/csrc/semaphore.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.834795 datamana-0.0.6/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:19.000000 datamana-0.0.6/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:19.000000 datamana-0.0.6/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-15 12:57:19.000000 datamana-0.0.6/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:57:32.834795 datamana-0.0.6/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 12:57:32.000000 datamana-0.0.6/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-15 12:57:19.000000 datamana-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:57:32.838795 datamana-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-15 12:57:19.000000 datamana-0.0.6/setup.py
```

### Comparing `datamana-0.0.5/CMakeLists.txt` & `datamana-0.0.6/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,10 +13,11 @@
   COMMAND "${Python_EXECUTABLE}" -m nanobind --cmake_dir
   OUTPUT_STRIP_TRAILING_WHITESPACE OUTPUT_VARIABLE NB_DIR)
 list(APPEND CMAKE_PREFIX_PATH "${NB_DIR}")
 find_package(nanobind CONFIG REQUIRED)
 
 nanobind_add_module(
   core STABLE_ABI
-  csrc/semaphore.hpp csrc/mqueue.hpp
+  csrc/semaphore.hpp csrc/mqueue.hpp csrc/fcntl.hpp
   csrc/python.cpp
 )
+target_link_libraries(core PRIVATE rt)
```

### Comparing `datamana-0.0.5/LICENSE` & `datamana-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.0.5/PKG-INFO` & `datamana-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.5/csrc/mqueue.hpp` & `datamana-0.0.6/csrc/mqueue.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,14 @@
 #include <nanobind/nanobind.h>
 #include <nanobind/stl/string.h>
 
 namespace nb = nanobind;
 
 struct MQueue {
     mqd_t mqd;
-    const int o_rdonly = O_RDONLY;
-    const int o_wronly = O_WRONLY;
-    const int o_rdwr = O_RDWR;
-    const int o_creat = O_CREAT;
-    const int o_excl = O_EXCL;
-    const int o_nonblock = O_NONBLOCK;
 
     MQueue() : mqd((mqd_t)-1) {}
 
     int py_mq_open(const char *name, int oflag, unsigned int mode, struct mq_attr *attr) {
         mqd = mq_open(name, oflag, (mode_t)mode, attr);
         if (mqd == (mqd_t)-1) {
             return -1;
```

### Comparing `datamana-0.0.5/datamana/torch.py` & `datamana-0.0.6/datamana/torch.py`

 * *Files identical despite different names*

### Comparing `datamana-0.0.5/datamana.egg-info/PKG-INFO` & `datamana-0.0.6/datamana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamana
-Version: 0.0.5
+Version: 0.0.6
 Summary: Dataset Manager
 Author-email: Jiau Zhang <jiauzhang@163.com>
 Project-URL: Homepage, https://github.com/jiauzhang/datamana
 Keywords: Deep Learning,Dataset Manager,Artificial Intelligence
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `datamana-0.0.5/pyproject.toml` & `datamana-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "cmake >= 3.15",
     "nanobind >= 1.9.2",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datamana"
-version = "0.0.5"
+version = "0.0.6"
 description = "Dataset Manager"
 readme = "README.md"
 authors = [
     {name = "Jiau Zhang", email = "jiauzhang@163.com"},
 ]
 classifiers = [
     'Intended Audience :: Developers',
```

### Comparing `datamana-0.0.5/setup.py` & `datamana-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,11 +116,11 @@
         subprocess.run(
             ["cmake", "--build", ".", *build_args], cwd=build_temp, check=True
         )
 
 setup(
     ext_modules=[CMakeExtension("datamana.core", sourcedir=".", sources=[
         'CMakeLists.txt',
-        'csrc/semaphore.hpp', 'csrc/mqueue.hpp', 'csrc/python.cpp',
+        'csrc/semaphore.hpp', 'csrc/mqueue.hpp', 'csrc/python.cpp', ' csrc/fcntl.hpp',
     ])],
     cmdclass={"build_ext": CMakeBuild},
 )
```

