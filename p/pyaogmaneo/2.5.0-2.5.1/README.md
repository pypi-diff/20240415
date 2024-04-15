# Comparing `tmp/pyaogmaneo-2.5.0.tar.gz` & `tmp/pyaogmaneo-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaogmaneo-2.5.0.tar", last modified: Sat Apr 13 22:43:13 2024, max compression
+gzip compressed data, was "pyaogmaneo-2.5.1.tar", last modified: Mon Apr 15 00:01:39 2024, max compression
```

## Comparing `pyaogmaneo-2.5.0.tar` & `pyaogmaneo-2.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:43:13.078680 pyaogmaneo-2.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:43:13.074680 pyaogmaneo-2.5.0/CMake/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/CMake/FindAOgmaNeo.cmake
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-13 22:43:13.078680 pyaogmaneo-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:43:13.078680 pyaogmaneo-2.5.0/pyaogmaneo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-13 22:43:13.000000 pyaogmaneo-2.5.0/pyaogmaneo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 22:43:13.000000 pyaogmaneo-2.5.0/pyaogmaneo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:43:13.000000 pyaogmaneo-2.5.0/pyaogmaneo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:43:12.000000 pyaogmaneo-2.5.0/pyaogmaneo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 22:43:13.000000 pyaogmaneo-2.5.0/pyaogmaneo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:43:13.078680 pyaogmaneo-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:43:13.074680 pyaogmaneo-2.5.0/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:43:13.078680 pyaogmaneo-2.5.0/source/pyaogmaneo/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_helpers.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_helpers.h
--rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7343 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_hierarchy.h
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_image_encoder.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_image_encoder.h
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-04-13 22:43:05.000000 pyaogmaneo-2.5.0/source/pyaogmaneo/py_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/CMake/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/CMake/FindAOgmaNeo.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17842 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:01:38.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 00:01:39.000000 pyaogmaneo-2.5.1/pyaogmaneo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.062031 pyaogmaneo-2.5.1/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:01:39.066031 pyaogmaneo-2.5.1/source/pyaogmaneo/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12890 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7313 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-15 00:01:31.000000 pyaogmaneo-2.5.1/source/pyaogmaneo/py_module.cpp
```

### Comparing `pyaogmaneo-2.5.0/CMake/FindAOgmaNeo.cmake` & `pyaogmaneo-2.5.1/CMake/FindAOgmaNeo.cmake`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.0/CMakeLists.txt` & `pyaogmaneo-2.5.1/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     find_package(AOgmaNeo)
 else()
     message(STATUS "Not using system installation of AOgmaNeo, will download from repository")
 
     FetchContent_Declare(
         AOgmaNeo
         GIT_REPOSITORY https://github.com/ogmacorp/AOgmaNeo.git
-        GIT_TAG 549d56b8e32dd00dcca84b49099f6a1c36ec8af3
+        GIT_TAG efd239a88ff5e75acb4b4b0d4509526bdde50cae
     )
 
     FetchContent_MakeAvailable(AOgmaNeo)
 endif()
 
 FetchContent_Declare(
     pybind11
```

### Comparing `pyaogmaneo-2.5.0/LICENSE.md` & `pyaogmaneo-2.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.0/PKG-INFO` & `pyaogmaneo-2.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.5.0/README.md` & `pyaogmaneo-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.0/pyaogmaneo.egg-info/PKG-INFO` & `pyaogmaneo-2.5.1/pyaogmaneo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaogmaneo
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python bindings for the AOgmaNeo library
 Home-page: https://ogmacorp.com/
 Author: Ogma Intelligent Systems Corp
 Author-email: info@ogmacorp.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `pyaogmaneo-2.5.0/setup.py` & `pyaogmaneo-2.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             os.makedirs(self.build_temp)
 
         subprocess.check_call([ 'cmake', ext.sourcedir ] + cmake_args, cwd=self.build_temp, env=env)
         subprocess.check_call([ 'cmake', '--build', '.' ] + build_args, cwd=self.build_temp)
 
 setup(
     name="pyaogmaneo",
-    version="2.5.0",
+    version="2.5.1",
     description="Python bindings for the AOgmaNeo library",
     long_description='https://github.com/ogmacorp/PyAOgmaNeo',
     author='Ogma Intelligent Systems Corp',
     author_email='info@ogmacorp.com',
     url='https://ogmacorp.com/',
     license='Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License',
     classifiers=[
```

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_helpers.cpp` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_helpers.h` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_helpers.h`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_hierarchy.cpp` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     // copy params
     params.layers.resize(h.get_num_layers());
 
     for (int l = 0; l < h.get_num_layers(); l++)
         params.layers[l] = h.params.layers[l];
 
-    params.representation_anticipation = h.params.representation_anticipation;
+    params.anticipation = h.params.anticipation;
 
     c_input_cis_backing.resize(h.get_num_io());
     c_input_cis.resize(h.get_num_io());
 
     for (int i = 0; i < c_input_cis_backing.size(); i++)
         c_input_cis_backing[i].resize(h.get_io_size(i).x * h.get_io_size(i).y);
 }
@@ -386,15 +386,15 @@
     for (int i = 0; i < params.ios.size(); i++)
         h.params.ios[i] = params.ios[i];
 
     // copy params
     for (int l = 0; l < params.layers.size(); l++)
         h.params.layers[l] = params.layers[l];
 
-    h.params.representation_anticipation = params.representation_anticipation;
+    h.params.anticipation = params.anticipation;
 }
 
 void Hierarchy::merge(
     const std::vector<Hierarchy*> &hierarchies,
     Merge_Mode mode
 ) {
     aon::Array<aon::Hierarchy*> c_hierarchies(hierarchies.size());
```

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_hierarchy.h` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_hierarchy.h`

 * *Files 1% similar despite different names*

```diff
@@ -87,19 +87,19 @@
     void check_in_range() const;
 };
 
 struct Params {
     std::vector<aon::Hierarchy::Layer_Params> layers;
     std::vector<aon::Hierarchy::IO_Params> ios;
 
-    bool representation_anticipation;
+    bool anticipation;
 
     Params()
     :
-    representation_anticipation(true)
+    anticipation(true)
     {}
 };
 
 class Hierarchy {
 private:
     aon::Hierarchy h;
```

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_image_encoder.cpp` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.cpp`

 * *Files identical despite different names*

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_image_encoder.h` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_image_encoder.h`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 #include "py_helpers.h"
 #include <aogmaneo/image_encoder.h>
 
 namespace py = pybind11;
 
 namespace pyaon {
-const int image_encoder_magic = 7557115;
+const int image_encoder_magic = 4153116;
 
 struct Image_Visible_Layer_Desc {
     std::tuple<int, int, int> size;
 
     int radius;
 
     Image_Visible_Layer_Desc(
```

### Comparing `pyaogmaneo-2.5.0/source/pyaogmaneo/py_module.cpp` & `pyaogmaneo-2.5.1/source/pyaogmaneo/py_module.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
         .def_readwrite("actor", &aon::Hierarchy::IO_Params::actor)
         .def_readwrite("importance", &aon::Hierarchy::IO_Params::importance);
 
     py::class_<pyaon::Params>(m, "Params")
         .def(py::init<>())
         .def_readwrite("layers", &pyaon::Params::layers)
         .def_readwrite("ios", &pyaon::Params::ios)
-        .def_readwrite("representation_anticipation", &pyaon::Params::representation_anticipation);
+        .def_readwrite("anticipation", &pyaon::Params::anticipation);
 
     py::class_<pyaon::Hierarchy>(m, "Hierarchy")
         .def(py::init<
                 const std::vector<pyaon::IO_Desc>&,
                 const std::vector<pyaon::Layer_Desc>&,
                 const std::string&,
                 const py::array_t<unsigned char>&
@@ -210,15 +210,16 @@
 
     // bind params
     py::class_<aon::Image_Encoder::Params>(m, "ImageEncoderParams")
         .def(py::init<>())
         .def_readwrite("falloff", &aon::Image_Encoder::Params::falloff)
         .def_readwrite("lr", &aon::Image_Encoder::Params::lr)
         .def_readwrite("scale", &aon::Image_Encoder::Params::scale)
-        .def_readwrite("rr", &aon::Image_Encoder::Params::rr);
+        .def_readwrite("rr", &aon::Image_Encoder::Params::rr)
+        .def_readwrite("radius", &aon::Image_Encoder::Params::radius);
 
     py::class_<pyaon::Image_Encoder>(m, "ImageEncoder")
         .def(py::init<
                 const std::tuple<int, int, int>&,
                 const std::vector<pyaon::Image_Visible_Layer_Desc>&,
                 const std::string&,
                 const py::array_t<unsigned char>&
```

