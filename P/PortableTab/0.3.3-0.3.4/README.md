# Comparing `tmp/portabletab-0.3.3.tar.gz` & `tmp/portabletab-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portabletab-0.3.3.tar", max compression
+gzip compressed data, was "portabletab-0.3.4.tar", max compression
```

## Comparing `portabletab-0.3.3.tar` & `portabletab-0.3.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.3.3/LICENSE
--rw-r--r--   0        0        0      203 2023-07-02 08:12:40.637313 portabletab-0.3.3/PortableTab/__init__.py
--rw-r--r--   0        0        0     4861 2023-04-11 03:07:38.494545 portabletab-0.3.3/PortableTab/__main__.py
--rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.3.3/PortableTab/base_table.py
--rw-r--r--   0        0        0     4697 2023-07-02 08:10:59.976983 portabletab-0.3.3/PortableTab/capnp_manager.py
--rw-r--r--   0        0        0    18443 2023-07-02 08:09:44.284891 portabletab-0.3.3/PortableTab/capnp_table.py
--rw-r--r--   0        0        0      155 2023-04-11 03:07:38.498545 portabletab-0.3.3/PortableTab/exceptions.py
--rw-r--r--   0        0        0     1837 2023-04-11 03:07:29.170336 portabletab-0.3.3/README.md
--rw-r--r--   0        0        0      634 2023-07-02 08:12:36.821296 portabletab-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2586 1970-01-01 00:00:00.000000 portabletab-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-03-23 04:47:41.138638 portabletab-0.3.4/LICENSE
+-rw-r--r--   0        0        0      203 2024-04-15 01:24:23.588886 portabletab-0.3.4/PortableTab/__init__.py
+-rw-r--r--   0        0        0     4861 2023-04-11 03:07:38.494545 portabletab-0.3.4/PortableTab/__main__.py
+-rw-r--r--   0        0        0     1917 2023-04-04 07:41:11.567861 portabletab-0.3.4/PortableTab/base_table.py
+-rw-r--r--   0        0        0     4697 2024-03-28 02:55:40.041699 portabletab-0.3.4/PortableTab/capnp_manager.py
+-rw-r--r--   0        0        0    18443 2024-03-28 02:55:46.657808 portabletab-0.3.4/PortableTab/capnp_table.py
+-rw-r--r--   0        0        0      155 2023-04-11 03:07:38.498545 portabletab-0.3.4/PortableTab/exceptions.py
+-rw-r--r--   0        0        0     2432 2024-04-03 05:01:01.335427 portabletab-0.3.4/README.md
+-rw-r--r--   0        0        0      730 2024-04-15 01:36:03.399047 portabletab-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     3175 1970-01-01 00:00:00.000000 portabletab-0.3.4/PKG-INFO
```

### Comparing `portabletab-0.3.3/LICENSE` & `portabletab-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.3/PortableTab/__main__.py` & `portabletab-0.3.4/PortableTab/__main__.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.3/PortableTab/base_table.py` & `portabletab-0.3.4/PortableTab/base_table.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.3/PortableTab/capnp_manager.py` & `portabletab-0.3.4/PortableTab/capnp_manager.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.3/PortableTab/capnp_table.py` & `portabletab-0.3.4/PortableTab/capnp_table.py`

 * *Files identical despite different names*

### Comparing `portabletab-0.3.3/PKG-INFO` & `portabletab-0.3.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
-Name: portabletab
-Version: 0.3.3
+Name: PortableTab
+Version: 0.3.4
 Summary: Python package for serializing tables in portable format with Capnp.
 License: MIT
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
-Requires-Dist: marisa-trie (>=0.7.8,<0.8.0)
-Requires-Dist: pycapnp (>=1.3.0,<2.0.0)
+Requires-Dist: marisa-trie (>=1.1.0)
+Requires-Dist: pycapnp (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # PortableTab
 
+![Python 3.7](https://github.com/t-sagara/PortableTab/actions/workflows/python-3.7.yml/badge.svg)
+![Python 3.8](https://github.com/t-sagara/PortableTab/actions/workflows/python-3.8.yml/badge.svg)
+![Python 3.9](https://github.com/t-sagara/PortableTab/actions/workflows/python-3.9.yml/badge.svg)
+![Python 3.10](https://github.com/t-sagara/PortableTab/actions/workflows/python-3.10.yml/badge.svg)
+![Python 3.11](https://github.com/t-sagara/PortableTab/actions/workflows/python-3.11.yml/badge.svg)
+![Python 3.12](https://github.com/t-sagara/PortableTab/actions/workflows/python-3.12.yml/badge.svg)
+
 *PortableTab* is a Python library that allows for serialization of 
 typed tables into a set of files, as well as deserialization of
 specific rows extracted from the files.
 
 ## Features
 
 The serialized files are independent of OS and CPU architecture, so it can
```

