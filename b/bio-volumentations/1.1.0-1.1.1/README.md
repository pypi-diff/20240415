# Comparing `tmp/bio_volumentations-1.1.0.tar.gz` & `tmp/bio_volumentations-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bio_volumentations-1.1.0.tar", last modified: Mon Apr 15 09:39:58 2024, max compression
+gzip compressed data, was "bio_volumentations-1.1.1.tar", last modified: Mon Apr 15 11:24:46 2024, max compression
```

## Comparing `bio_volumentations-1.1.0.tar` & `bio_volumentations-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/
--rw-rw-rw-   0        0        0     1120 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/LICENSE
--rw-rw-rw-   0        0        0    11364 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9047 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.300001 bio_volumentations-1.1.0/bio_volumentations/
--rw-rw-rw-   0        0        0     4025 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.316562 bio_volumentations-1.1.0/bio_volumentations/augmentations/
--rw-rw-rw-   0        0        0     3953 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/__init__.py
--rw-rw-rw-   0        0        0    25874 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/functional.py
--rw-rw-rw-   0        0        0     6343 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/spatial_funcional.py
--rw-rw-rw-   0        0        0    63200 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/transforms.py
--rw-rw-rw-   0        0        0     7379 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/augmentations/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/bio_volumentations/conversion/
--rw-rw-rw-   0        0        0     3910 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/conversion/__init__.py
--rw-rw-rw-   0        0        0     4070 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/conversion/functional.py
--rw-rw-rw-   0        0        0     7095 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/conversion/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/bio_volumentations/core/
--rw-rw-rw-   0        0        0     3869 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/core/__init__.py
--rw-rw-rw-   0        0        0     6040 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/core/composition.py
--rw-rw-rw-   0        0        0     6382 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/core/transforms_interface.py
--rw-rw-rw-   0        0        0     5558 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/random_utils.py
--rw-rw-rw-   0        0        0     2557 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/bio_volumentations/typing.py
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/bio_volumentations.egg-info/
--rw-rw-rw-   0        0        0    11364 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      851 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-15 09:39:58.000000 bio_volumentations-1.1.0/bio_volumentations.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2686 2024-04-15 09:39:45.000000 bio_volumentations-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 09:39:58.333228 bio_volumentations-1.1.0/tests/
--rw-rw-rw-   0        0        0      204 2024-04-15 07:21:36.000000 bio_volumentations-1.1.0/tests/test_random_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.529189 bio_volumentations-1.1.1/
+-rw-rw-rw-   0        0        0     1120 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0    10148 2024-04-15 11:24:46.529189 bio_volumentations-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9108 2024-04-15 11:16:30.000000 bio_volumentations-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.495736 bio_volumentations-1.1.1/bio_volumentations/
+-rw-rw-rw-   0        0        0     4025 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.512508 bio_volumentations-1.1.1/bio_volumentations/augmentations/
+-rw-rw-rw-   0        0        0     3953 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/augmentations/__init__.py
+-rw-rw-rw-   0        0        0    25874 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/augmentations/functional.py
+-rw-rw-rw-   0        0        0     6343 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/augmentations/spatial_funcional.py
+-rw-rw-rw-   0        0        0    63200 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/augmentations/transforms.py
+-rw-rw-rw-   0        0        0     7379 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/augmentations/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.512508 bio_volumentations-1.1.1/bio_volumentations/conversion/
+-rw-rw-rw-   0        0        0     3910 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/conversion/__init__.py
+-rw-rw-rw-   0        0        0     4070 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/conversion/functional.py
+-rw-rw-rw-   0        0        0     7095 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/conversion/transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.512508 bio_volumentations-1.1.1/bio_volumentations/core/
+-rw-rw-rw-   0        0        0     3869 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/core/__init__.py
+-rw-rw-rw-   0        0        0     6040 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/core/composition.py
+-rw-rw-rw-   0        0        0     6382 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/core/transforms_interface.py
+-rw-rw-rw-   0        0        0     5558 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/random_utils.py
+-rw-rw-rw-   0        0        0     2557 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/bio_volumentations/typing.py
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.529189 bio_volumentations-1.1.1/bio_volumentations.egg-info/
+-rw-rw-rw-   0        0        0    10148 2024-04-15 11:24:46.000000 bio_volumentations-1.1.1/bio_volumentations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      851 2024-04-15 11:24:46.000000 bio_volumentations-1.1.1/bio_volumentations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 11:24:46.000000 bio_volumentations-1.1.1/bio_volumentations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-15 11:24:46.000000 bio_volumentations-1.1.1/bio_volumentations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-15 11:24:46.000000 bio_volumentations-1.1.1/bio_volumentations.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2795 2024-04-15 11:16:30.000000 bio_volumentations-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 11:24:46.529189 bio_volumentations-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 11:24:46.512508 bio_volumentations-1.1.1/tests/
+-rw-rw-rw-   0        0        0      204 2024-04-15 07:21:36.000000 bio_volumentations-1.1.1/tests/test_random_utils.py
```

### Comparing `bio_volumentations-1.1.0/LICENSE` & `bio_volumentations-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/PKG-INFO` & `bio_volumentations-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,18 @@
 Metadata-Version: 2.1
 Name: bio-volumentations
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images
 Author: Samuel Šuľan
 Author-email: Lucia Hradecká <lucia.d.hradecka@gmail.com>, Filip Lux <lux.filip@gmail.com>
 License: MIT License
-        
-        Copyright (c) 2024 Samuel Šuľan, Lucia Hradecká, Filip Lux
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
-Project-URL: Documentation, https://biovolumentations.readthedocs.io/v1-1-0/
+Project-URL: Documentation, https://biovolumentations.readthedocs.io/v1-1-1/
 Project-URL: Repository, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
-Keywords: image,augmentation,volumetric,biomedical,bioimage,preprocessing,transformation,3D
+Keywords: image,augmentation,3D,volumetric,biomedical,bioimage,preprocessing,transformation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -54,15 +33,15 @@
 It can be used with any major Python deep learning library, including PyTorch, PyTorch Lightning, TensorFlow, and Keras.
 
 This library builds upon wide-spread libraries such as Albumentations (see the Contributions section below) 
 in terms of design and user interface. Therefore, it can easily be adopted by developers.
 
 # Installation
 
-Install the package from PyPi using:
+Install the package from pip using:
 ```python
 pip install bio-volumentations
 ```
 ## Requirements
 
 NumPy       https://numpy.org/ <br> 
 SciPy       https://scipy.org/ <br>
@@ -100,14 +79,16 @@
 - [C, Z, Y, X, T] (a single-channel as well as multi-channel volumetric image sequence)
 
 **It is strongly recommended to use `Compose` to create and use transformation pipelines.** 
 The `Compose` class automatically checks and adjusts image format, datatype, stacks
 individual transforms to a pipeline, and outputs the image as a contiguous array. 
 Optionally, it can also convert the transformed image to a desired format.
 
+More at the [documentation pages](https://www.google.com).
+
 Below, there are several examples of how to use this library.
 
 ### Example: Transforming a Single Image
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
```

### Comparing `bio_volumentations-1.1.0/README.md` & `bio_volumentations-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 It can be used with any major Python deep learning library, including PyTorch, PyTorch Lightning, TensorFlow, and Keras.
 
 This library builds upon wide-spread libraries such as Albumentations (see the Contributions section below) 
 in terms of design and user interface. Therefore, it can easily be adopted by developers.
 
 # Installation
 
-Install the package from PyPi using:
+Install the package from pip using:
 ```python
 pip install bio-volumentations
 ```
 ## Requirements
 
 NumPy       https://numpy.org/ <br> 
 SciPy       https://scipy.org/ <br>
@@ -56,14 +56,16 @@
 - [C, Z, Y, X, T] (a single-channel as well as multi-channel volumetric image sequence)
 
 **It is strongly recommended to use `Compose` to create and use transformation pipelines.** 
 The `Compose` class automatically checks and adjusts image format, datatype, stacks
 individual transforms to a pipeline, and outputs the image as a contiguous array. 
 Optionally, it can also convert the transformed image to a desired format.
 
+More at the [documentation pages](https://www.google.com).
+
 Below, there are several examples of how to use this library.
 
 ### Example: Transforming a Single Image
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
```

### Comparing `bio_volumentations-1.1.0/bio_volumentations/__init__.py` & `bio_volumentations-1.1.1/bio_volumentations/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/augmentations/__init__.py` & `bio_volumentations-1.1.1/bio_volumentations/augmentations/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/augmentations/functional.py` & `bio_volumentations-1.1.1/bio_volumentations/augmentations/functional.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/augmentations/spatial_funcional.py` & `bio_volumentations-1.1.1/bio_volumentations/augmentations/spatial_funcional.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/augmentations/transforms.py` & `bio_volumentations-1.1.1/bio_volumentations/augmentations/transforms.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/augmentations/utils.py` & `bio_volumentations-1.1.1/bio_volumentations/augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/conversion/__init__.py` & `bio_volumentations-1.1.1/bio_volumentations/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/conversion/functional.py` & `bio_volumentations-1.1.1/bio_volumentations/conversion/functional.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/conversion/transforms.py` & `bio_volumentations-1.1.1/bio_volumentations/conversion/transforms.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/core/__init__.py` & `bio_volumentations-1.1.1/bio_volumentations/core/__init__.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/core/composition.py` & `bio_volumentations-1.1.1/bio_volumentations/core/composition.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/core/transforms_interface.py` & `bio_volumentations-1.1.1/bio_volumentations/core/transforms_interface.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/random_utils.py` & `bio_volumentations-1.1.1/bio_volumentations/random_utils.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations/typing.py` & `bio_volumentations-1.1.1/bio_volumentations/typing.py`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/bio_volumentations.egg-info/PKG-INFO` & `bio_volumentations-1.1.1/bio_volumentations.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,18 @@
 Metadata-Version: 2.1
 Name: bio-volumentations
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images
 Author: Samuel Šuľan
 Author-email: Lucia Hradecká <lucia.d.hradecka@gmail.com>, Filip Lux <lux.filip@gmail.com>
 License: MIT License
-        
-        Copyright (c) 2024 Samuel Šuľan, Lucia Hradecká, Filip Lux
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
 Project-URL: Homepage, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
-Project-URL: Documentation, https://biovolumentations.readthedocs.io/v1-1-0/
+Project-URL: Documentation, https://biovolumentations.readthedocs.io/v1-1-1/
 Project-URL: Repository, https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads
-Keywords: image,augmentation,volumetric,biomedical,bioimage,preprocessing,transformation,3D
+Keywords: image,augmentation,3D,volumetric,biomedical,bioimage,preprocessing,transformation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.1
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -54,15 +33,15 @@
 It can be used with any major Python deep learning library, including PyTorch, PyTorch Lightning, TensorFlow, and Keras.
 
 This library builds upon wide-spread libraries such as Albumentations (see the Contributions section below) 
 in terms of design and user interface. Therefore, it can easily be adopted by developers.
 
 # Installation
 
-Install the package from PyPi using:
+Install the package from pip using:
 ```python
 pip install bio-volumentations
 ```
 ## Requirements
 
 NumPy       https://numpy.org/ <br> 
 SciPy       https://scipy.org/ <br>
@@ -100,14 +79,16 @@
 - [C, Z, Y, X, T] (a single-channel as well as multi-channel volumetric image sequence)
 
 **It is strongly recommended to use `Compose` to create and use transformation pipelines.** 
 The `Compose` class automatically checks and adjusts image format, datatype, stacks
 individual transforms to a pipeline, and outputs the image as a contiguous array. 
 Optionally, it can also convert the transformed image to a desired format.
 
+More at the [documentation pages](https://www.google.com).
+
 Below, there are several examples of how to use this library.
 
 ### Example: Transforming a Single Image
 
 ```python
 import numpy as np
 from bio_volumentations import Compose, RandomGamma, RandomRotate90, GaussianBlur
```

### Comparing `bio_volumentations-1.1.0/bio_volumentations.egg-info/SOURCES.txt` & `bio_volumentations-1.1.1/bio_volumentations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bio_volumentations-1.1.0/pyproject.toml` & `bio_volumentations-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 
 [project]
 # Put the name of your project on PyPI.
 name = "bio-volumentations"
 
 # Put the version of your project. This field is required, although it is often marked as dynamic:
- version = "1.1.0"
+version = "1.1.1"
 #dynamic = ["version"]
+# https://stackoverflow.com/questions/21064581/how-to-overwrite-pypi-package-when-doing-upload-from-command-line
 
 # If your project has dependencies, list them like this:
 dependencies = [
   "numpy",
   "scipy",
   "scikit-image",
   "matplotlib",
@@ -24,47 +25,47 @@
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#dependencies-and-requirements
 
 # Declare the minimum version of Python that you support:
 requires-python = ">=3.1"
 
 # Authors (identified by a name and/or an email address)
 authors = [
-  {name = "Samuel Šuľan"},
   {name = "Lucia Hradecká", email = "lucia.d.hradecka@gmail.com"},
   {name = "Filip Lux", email = "lux.filip@gmail.com"},
+  {name = "Samuel Šuľan"},
 ]
 # Optionally, can also include the maintainers field
 
 # A one-line description of your project, to show as the “headline” of your project page on PyPI
 # and other places such as lists of search results:
 description = "Library for 3D-5D augmentations of volumetric multi-dimensional biomedical images"
 
 # A longer description - can use readme.md
 readme = "README.md"
 
-# Lincense
-license = {file = "LICENSE"}
-#  license = {text = "MIT License"} # another possibility
+# Lincense - two possibilities
+#license = {file = "LICENSE"}
+license = {text = "MIT License"}
 
 # Keywords to help PyPI’s search box to suggest your project when people search for these keywords
-keywords = ["image", "augmentation", "volumetric", "biomedical", "bioimage",
-    "preprocessing", "transformation", "3D"]
+keywords = ["image", "augmentation", "3D", "volumetric", "biomedical", "bioimage",
+    "preprocessing", "transformation"]
 
 # Classifiers: this information is used for searching and browsing projects on PyPI
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#classifiers
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 # A list of URLs associated with your project, displayed on the left sidebar of your PyPI project page.
 [project.urls]
 Homepage = "https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads"
-Documentation = "https://biovolumentations.readthedocs.io/v1-1-0/"
+Documentation = "https://biovolumentations.readthedocs.io/v1-1-1/"
 Repository = "https://gitlab.fi.muni.cz/cbia/bio-volumentations/-/tree/v1-1-0?ref_type=heads"
 
 # MISSING FROM SETUP.PY
 # entry_points={
 #        'console_scripts': [
 #            'bioVolumentation=bio_volumentations:__init__'
 #        ]
```

