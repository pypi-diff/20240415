# Comparing `tmp/utubes-0.0.1.tar.gz` & `tmp/utubes-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utubes-0.0.1.tar", last modified: Mon Apr 15 15:58:26 2024, max compression
+gzip compressed data, was "utubes-0.0.2.tar", last modified: Mon Apr 15 16:06:31 2024, max compression
```

## Comparing `utubes-0.0.1.tar` & `utubes-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:58:26.372020 utubes-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 15:58:22.000000 utubes-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 15:58:26.372020 utubes-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 15:58:22.000000 utubes-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:58:26.372020 utubes-0.0.1/Utube/
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-15 15:58:22.000000 utubes-0.0.1/Utube/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:58:26.372020 utubes-0.0.1/Utube/functions/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 15:58:22.000000 utubes-0.0.1/Utube/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 15:58:22.000000 utubes-0.0.1/Utube/functions/function01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:58:26.372020 utubes-0.0.1/Utube/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 15:58:22.000000 utubes-0.0.1/Utube/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:58:22.000000 utubes-0.0.1/Utube/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 15:58:22.000000 utubes-0.0.1/Utube/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:58:26.372020 utubes-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-15 15:58:22.000000 utubes-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:58:26.372020 utubes-0.0.1/utubes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-15 15:58:26.000000 utubes-0.0.1/utubes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 15:58:26.000000 utubes-0.0.1/utubes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:58:26.000000 utubes-0.0.1/utubes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:58:26.000000 utubes-0.0.1/utubes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 15:58:26.000000 utubes-0.0.1/utubes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.260479 utubes-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 16:06:26.000000 utubes-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 16:06:31.260479 utubes-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-15 16:06:26.000000 utubes-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.256479 utubes-0.0.2/Utube/
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.256479 utubes-0.0.2/Utube/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/functions/function01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.256479 utubes-0.0.2/Utube/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 16:06:26.000000 utubes-0.0.2/Utube/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:06:31.260479 utubes-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-15 16:06:26.000000 utubes-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:06:31.260479 utubes-0.0.2/utubes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 16:06:31.000000 utubes-0.0.2/utubes.egg-info/top_level.txt
```

### Comparing `utubes-0.0.1/LICENSE` & `utubes-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utubes-0.0.1/PKG-INFO` & `utubes-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.1
+Version: 0.0.2
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,monisha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -15,9 +15,9 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
- 📦 <a href="https://pypi.org/project/utube-dl" style="text-decoration:none;">Utube-dl</a>
+ 📦 <a href="https://pypi.org/project/utubes" style="text-decoration:none;">YOUTUBE EXTENSIONS</a>
 </p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.1 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.2 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,monisha
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
-                                 ð¦ _U_t_u_b_e_-_d_l
+                            ð¦ _Y_O_U_T_U_B_E_ _E_X_T_E_N_S_I_O_N_S
```

### Comparing `utubes-0.0.1/Utube/__init__.py` & `utubes-0.0.2/Utube/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-code = "0.0.1"
+code = "0.0.2"
 
 name = "utubes"
 
 with open("README.md", "r") as o:
     long_description = o.read()
 
 DATA01 = ['Natural Language :: English',
```

### Comparing `utubes-0.0.1/Utube/functions/function01.py` & `utubes-0.0.2/Utube/functions/function01.py`

 * *Files identical despite different names*

### Comparing `utubes-0.0.1/utubes.egg-info/PKG-INFO` & `utubes-0.0.2/utubes.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utubes
-Version: 0.0.1
+Version: 0.0.2
 Summary: ㅤ
 Home-page: https://github.com/Monisha
 License: MIT
 Keywords: python,youtube,monisha
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -15,9 +15,9 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
- 📦 <a href="https://pypi.org/project/utube-dl" style="text-decoration:none;">Utube-dl</a>
+ 📦 <a href="https://pypi.org/project/utubes" style="text-decoration:none;">YOUTUBE EXTENSIONS</a>
 </p>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: utubes Version: 0.0.1 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: utubes Version: 0.0.2 Summary: ã¤ Home-page:
 https://github.com/Monisha License: MIT Keywords: python,youtube,monisha
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Classifier: License :: OSI Approved
 :: GNU Lesser General Public License v3 (LGPLv3) Requires-Python: ~=3.10
 Description-Content-Type: text/markdown License-File: LICENSE
-                                 ð¦ _U_t_u_b_e_-_d_l
+                            ð¦ _Y_O_U_T_U_B_E_ _E_X_T_E_N_S_I_O_N_S
```

