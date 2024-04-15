# Comparing `tmp/deepctools-1.0.2.tar.gz` & `tmp/deepctools-1.0.3.tar.gz`

## Comparing `deepctools-1.0.2.tar` & `deepctools-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 deepctools-1.0.2/.pypirc
--rw-r--r--   0        0        0    22042 2020-02-02 00:00:00.000000 deepctools-1.0.2/src/deepctools/DeePCtools.py
--rw-r--r--   0        0        0    14413 2020-02-02 00:00:00.000000 deepctools-1.0.2/src/deepctools/Modeltools.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 deepctools-1.0.2/src/deepctools/__init__.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 deepctools-1.0.2/src/deepctools/util.py
--rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 deepctools-1.0.2/tests/tutorial.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 deepctools-1.0.2/.gitignore
--rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 deepctools-1.0.2/LICENSE
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 deepctools-1.0.2/README.md
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 deepctools-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    20432 2020-02-02 00:00:00.000000 deepctools-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 deepctools-1.0.3/.pypirc
+-rw-r--r--   0        0        0    22042 2020-02-02 00:00:00.000000 deepctools-1.0.3/src/deepctools/DeePCtools.py
+-rw-r--r--   0        0        0    14413 2020-02-02 00:00:00.000000 deepctools-1.0.3/src/deepctools/Modeltools.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 deepctools-1.0.3/src/deepctools/__init__.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 deepctools-1.0.3/src/deepctools/util.py
+-rw-r--r--   0        0        0     8393 2020-02-02 00:00:00.000000 deepctools-1.0.3/tests/tutorial.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 deepctools-1.0.3/.gitignore
+-rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 deepctools-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7098 2020-02-02 00:00:00.000000 deepctools-1.0.3/README.md
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 deepctools-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    20463 2020-02-02 00:00:00.000000 deepctools-1.0.3/PKG-INFO
```

### Comparing `deepctools-1.0.2/src/deepctools/DeePCtools.py` & `deepctools-1.0.3/src/deepctools/DeePCtools.py`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.2/src/deepctools/Modeltools.py` & `deepctools-1.0.3/src/deepctools/Modeltools.py`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.2/src/deepctools/__init__.py` & `deepctools-1.0.3/src/deepctools/__init__.py`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.2/src/deepctools/util.py` & `deepctools-1.0.3/src/deepctools/util.py`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.2/tests/tutorial.py` & `deepctools-1.0.3/tests/tutorial.py`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.2/LICENSE` & `deepctools-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepctools-1.0.2/README.md` & `deepctools-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,20 @@
 
 - Numpy
 - Matplotlib
 - CasADi &emsp; &emsp;     <-- 3 <= __version__ <= 4
 
 ### 2. Usage
 
-Download the [*deepctools*](https://github.com/QiYuan-Zhang/DeePCtools/tree/8dbc2458966214bf9885f4d622e20c3b840641e2/deepctools) file and save it to your project directory.
+- Download the [*deepctools*](https://github.com/QiYuan-Zhang/DeePCtools/tree/8dbc2458966214bf9885f4d622e20c3b840641e2/deepctools) file and save it to your project directory.
+
+- Or install using pip
 
 ```
-    import deepctools
+    pip install deepctools
 ```
 Then you can use the deepctools in your python project.
 
 ## II. deepctools toolbox organization
 ```
 . 
 └── deeptools
```

### Comparing `deepctools-1.0.2/pyproject.toml` & `deepctools-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deepctools"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Xuewen Zhang", email="xuewen.zhang741@outlook.com"}
 ]
 maintainers = [
   { name="Xuewen Zhang", email="xuewen.zhang741@outlook.com"}
 ]
 dependencies = [
```

### Comparing `deepctools-1.0.2/PKG-INFO` & `deepctools-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deepctools
-Version: 1.0.2
+Version: 1.0.3
 Summary: A wrapped package for Data-enabled predictive control (DeePC) implementation. Including DeePC and Robust DeePC design with multiple objective functions.
 Project-URL: Homepage, https://github.com/QiYuan-Zhang/DeePCtools
 Project-URL: Issues, https://github.com/QiYuan-Zhang/DeePCtools/issues
 Project-URL: Introduction, https://qiyuan-zhang.github.io/my-toolbox/2024/04/15/Developed-deepctools.html
 Author-email: Xuewen Zhang <xuewen.zhang741@outlook.com>
 Maintainer-email: Xuewen Zhang <xuewen.zhang741@outlook.com>
 License:                                 Apache License
@@ -235,18 +235,20 @@
 
 - Numpy
 - Matplotlib
 - CasADi &emsp; &emsp;     <-- 3 <= __version__ <= 4
 
 ### 2. Usage
 
-Download the [*deepctools*](https://github.com/QiYuan-Zhang/DeePCtools/tree/8dbc2458966214bf9885f4d622e20c3b840641e2/deepctools) file and save it to your project directory.
+- Download the [*deepctools*](https://github.com/QiYuan-Zhang/DeePCtools/tree/8dbc2458966214bf9885f4d622e20c3b840641e2/deepctools) file and save it to your project directory.
+
+- Or install using pip
 
 ```
-    import deepctools
+    pip install deepctools
 ```
 Then you can use the deepctools in your python project.
 
 ## II. deepctools toolbox organization
 ```
 . 
 └── deeptools
```

