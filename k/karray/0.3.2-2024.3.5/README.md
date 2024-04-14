# Comparing `tmp/karray-0.3.2.tar.gz` & `tmp/karray-2024.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karray-0.3.2.tar", last modified: Thu Aug 10 12:56:15 2023, max compression
+gzip compressed data, was "karray-2024.3.5.tar", last modified: Sun Apr 14 23:47:10 2024, max compression
```

## Comparing `karray-0.3.2.tar` & `karray-2024.3.5.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-08-10 12:56:15.524410 karray-0.3.2/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     1069 2023-05-23 09:09:19.000000 karray-0.3.2/LICENSE
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      898 2023-08-10 12:56:15.524410 karray-0.3.2/PKG-INFO
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      108 2023-05-23 09:09:19.000000 karray-0.3.2/README.md
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-08-10 12:56:15.520410 karray-0.3.2/karray/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      241 2023-08-10 12:51:59.000000 karray-0.3.2/karray/__init__.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)    78462 2023-08-10 12:51:32.000000 karray-0.3.2/karray/arrays.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)    32016 2023-08-10 12:51:32.000000 karray-0.3.2/karray/long.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      411 2023-07-21 21:48:54.000000 karray-0.3.2/karray/setting.py
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     5625 2023-08-10 12:51:32.000000 karray-0.3.2/karray/utils.py
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-08-10 12:56:15.524410 karray-0.3.2/karray.egg-info/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      898 2023-08-10 12:56:15.000000 karray-0.3.2/karray.egg-info/PKG-INFO
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)      273 2023-08-10 12:56:15.000000 karray-0.3.2/karray.egg-info/SOURCES.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)        1 2023-08-10 12:56:15.000000 karray-0.3.2/karray.egg-info/dependency_links.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)        6 2023-08-10 12:56:15.000000 karray-0.3.2/karray.egg-info/requires.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)        7 2023-08-10 12:56:15.000000 karray-0.3.2/karray.egg-info/top_level.txt
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)       38 2023-08-10 12:56:15.524410 karray-0.3.2/setup.cfg
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)     1472 2023-08-10 12:52:07.000000 karray-0.3.2/setup.py
-drwxr-xr-x   0 cgaete   (738813943) domänen-benutzer (738800513)        0 2023-08-10 12:56:15.524410 karray-0.3.2/test/
--rw-r--r--   0 cgaete   (738813943) domänen-benutzer (738800513)    10901 2023-07-21 21:48:54.000000 karray-0.3.2/test/test.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-14 23:47:10.394467 karray-2024.3.5/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1069 2024-04-14 17:13:13.000000 karray-2024.3.5/LICENSE
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)    21272 2024-04-14 23:47:10.394467 karray-2024.3.5/PKG-INFO
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)    20334 2024-04-14 17:55:46.000000 karray-2024.3.5/README.md
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-14 23:47:10.394467 karray-2024.3.5/karray.egg-info/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)    21272 2024-04-14 23:47:10.000000 karray-2024.3.5/karray.egg-info/PKG-INFO
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)      490 2024-04-14 23:47:10.000000 karray-2024.3.5/karray.egg-info/SOURCES.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)        1 2024-04-14 23:47:10.000000 karray-2024.3.5/karray.egg-info/dependency_links.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)        6 2024-04-14 23:47:10.000000 karray-2024.3.5/karray.egg-info/requires.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)        4 2024-04-14 23:47:10.000000 karray-2024.3.5/karray.egg-info/top_level.txt
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)       38 2024-04-14 23:47:10.394467 karray-2024.3.5/setup.cfg
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1624 2024-04-14 23:38:13.000000 karray-2024.3.5/setup.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-14 23:47:10.390467 karray-2024.3.5/src/
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-14 23:47:10.394467 karray-2024.3.5/src/karray/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)      605 2024-04-14 23:35:58.000000 karray-2024.3.5/src/karray/__init__.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1155 2024-04-14 17:13:13.000000 karray-2024.3.5/src/karray/constants.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)   191359 2024-04-14 21:38:52.000000 karray-2024.3.5/src/karray/source_code.py
+drwxr-xr-x   0 cgaete    (1000) cgaete    (1000)        0 2024-04-14 23:47:10.394467 karray-2024.3.5/tests/
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1472 2024-04-14 17:13:13.000000 karray-2024.3.5/tests/test_array_choice.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3464 2024-04-14 21:50:09.000000 karray-2024.3.5/tests/test_array_filehandling.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     2029 2024-04-14 17:13:13.000000 karray-2024.3.5/tests/test_array_initialization.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3320 2024-04-14 17:13:13.000000 karray-2024.3.5/tests/test_array_insert.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     2077 2024-04-14 17:13:13.000000 karray-2024.3.5/tests/test_array_mismatch.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     3331 2024-04-14 17:13:13.000000 karray-2024.3.5/tests/test_array_operations.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1036 2024-04-14 21:35:21.000000 karray-2024.3.5/tests/test_dense.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     6869 2024-04-14 17:13:13.000000 karray-2024.3.5/tests/test_long.py
+-rw-r--r--   0 cgaete    (1000) cgaete    (1000)     1037 2024-04-14 21:50:48.000000 karray-2024.3.5/tests/test_sparse.py
```

### Comparing `karray-0.3.2/LICENSE` & `karray-2024.3.5/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Carlos Gaete
+Copyright (c) 2024 Carlos Gaete
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `karray-0.3.2/setup.py` & `karray-2024.3.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 root_dir = os.path.dirname(__file__)
 if root_dir:
     os.chdir(root_dir)
 
 with open(os.path.join(root_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-for dirpath, dirnames, filenames in os.walk("karray"):
+for dirpath, dirnames, filenames in os.walk(os.path.join('src', 'karray')):
     # Ignore dirnames that start with '.'
     if "__init__.py" in filenames:
         pkg = dirpath.replace(os.path.sep, ".")
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, ".")
         packages.append(pkg)
 
 setup(
     name="karray",
-    version="0.3.2",
+    version="2024.3.5",
+    python_requires=">=3.8",
     packages=packages,
     author="Carlos Gaete-Morales",
     author_email="cdgaete@gmail.com",
     install_requires=[
         "numpy"
     ],
     include_package_data=True,
@@ -34,13 +35,15 @@
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Topic :: Scientific/Engineering",
     ],
 )
```

