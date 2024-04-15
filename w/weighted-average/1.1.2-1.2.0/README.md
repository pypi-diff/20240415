# Comparing `tmp/weighted-average-1.1.2.tar.gz` & `tmp/weighted_average-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted-average-1.1.2.tar", last modified: Wed Feb  7 20:44:00 2024, max compression
+gzip compressed data, was "weighted_average-1.2.0.tar", last modified: Mon Apr 15 17:12:42 2024, max compression
```

## Comparing `weighted-average-1.1.2.tar` & `weighted_average-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:44:00.467699 weighted-average-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-02-07 20:42:38.000000 weighted-average-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-07 20:44:00.467699 weighted-average-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-07 20:42:38.000000 weighted-average-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-07 20:42:38.000000 weighted-average-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-07 20:44:00.467699 weighted-average-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-07 20:42:38.000000 weighted-average-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:44:00.459699 weighted-average-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:44:00.463699 weighted-average-1.1.2/src/weave/
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    18814 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/smoother.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-02-07 20:42:38.000000 weighted-average-1.1.2/src/weave/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:44:00.463699 weighted-average-1.1.2/src/weighted_average.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-07 20:44:00.000000 weighted-average-1.1.2/src/weighted_average.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-07 20:44:00.000000 weighted-average-1.1.2/src/weighted_average.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 20:44:00.000000 weighted-average-1.1.2/src/weighted_average.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-07 20:42:42.000000 weighted-average-1.1.2/src/weighted_average.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-07 20:44:00.000000 weighted-average-1.1.2/src/weighted_average.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-07 20:44:00.000000 weighted-average-1.1.2/src/weighted_average.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-07 20:44:00.463699 weighted-average-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-02-07 20:42:38.000000 weighted-average-1.1.2/tests/test_dimension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-02-07 20:42:38.000000 weighted-average-1.1.2/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4182 2024-02-07 20:42:38.000000 weighted-average-1.1.2/tests/test_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    12150 2024-02-07 20:42:38.000000 weighted-average-1.1.2/tests/test_smoother.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-07 20:42:38.000000 weighted-average-1.1.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:12:42.234368 weighted_average-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-15 17:11:37.000000 weighted_average-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-15 17:12:42.234368 weighted_average-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-15 17:11:37.000000 weighted_average-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 17:11:37.000000 weighted_average-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-15 17:12:42.234368 weighted_average-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-15 17:11:37.000000 weighted_average-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:12:42.230368 weighted_average-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:12:42.230368 weighted_average-1.2.0/src/weave/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23672 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8209 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28073 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/smoother.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-15 17:11:37.000000 weighted_average-1.2.0/src/weave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:12:42.234368 weighted_average-1.2.0/src/weighted_average.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-15 17:12:42.000000 weighted_average-1.2.0/src/weighted_average.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-15 17:12:42.000000 weighted_average-1.2.0/src/weighted_average.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:12:42.000000 weighted_average-1.2.0/src/weighted_average.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:11:42.000000 weighted_average-1.2.0/src/weighted_average.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-15 17:12:42.000000 weighted_average-1.2.0/src/weighted_average.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 17:12:42.000000 weighted_average-1.2.0/src/weighted_average.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:12:42.234368 weighted_average-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13261 2024-04-15 17:11:37.000000 weighted_average-1.2.0/tests/test_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4677 2024-04-15 17:11:37.000000 weighted_average-1.2.0/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-15 17:11:37.000000 weighted_average-1.2.0/tests/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15909 2024-04-15 17:11:37.000000 weighted_average-1.2.0/tests/test_smoother.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-15 17:11:37.000000 weighted_average-1.2.0/tests/test_utils.py
```

### Comparing `weighted-average-1.1.2/LICENSE` & `weighted_average-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weighted-average-1.1.2/PKG-INFO` & `weighted_average-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted-average
-Version: 1.1.2
+Version: 1.2.0
 Summary: Smooth data across multiple dimensions using weighted averages
 Home-page: https://github.com/ihmeuw-msca/weighted-average
 Author: IHME Math Sciences
 Author-email: ihme.math.sciences@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `weighted-average-1.1.2/README.md` & `weighted_average-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `weighted-average-1.1.2/setup.cfg` & `weighted_average-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weighted-average
-version = 1.1.2
+version = 1.2.0
 description = Smooth data across multiple dimensions using weighted averages
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = IHME Math Sciences
 author_email = ihme.math.sciences@gmail.com
 license = BSD 2-Clause License
 url = https://github.com/ihmeuw-msca/weighted-average
```

### Comparing `weighted-average-1.1.2/src/weave/__about__.py` & `weighted_average-1.2.0/src/weave/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     'License :: OSI Approved :: BSD License',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Natural Language :: English',
     'Programming Language :: Python :: 3',
 ]
 
-__version__ = '1.1.2'
+__version__ = '1.2.0'
 __year__ = '2024'
 __author__ = 'IHME Math Sciences'
 __email__ = 'ihme.math.sciences@gmail.com'
 
 __license__ = 'BSD 2-Clause'
 __copyright__ = f"Copyright {__year__} {__author__}"
```

### Comparing `weighted-average-1.1.2/src/weave/dimension.py` & `weighted_average-1.2.0/src/weave/dimension.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 from numba.typed import Dict as TypedDict  # type: ignore
 from numba.types import DictType, UniTuple  # type: ignore
 from numba.types import float32, unicode_type  # type: ignore
 import numpy as np
 from pandas import DataFrame  # type: ignore
 
 from weave.distance import euclidean, tree
-from weave.kernels import exponential, depth, tricubic
+from weave.kernels import exponential, tricubic, depth, inverse
 from weave.utils import as_list, is_float, is_number
 
 number = Union[int, float]
 DistanceDict = Dict[Tuple[number, number], number]
 WeightDict = Dict[Tuple[float, float], float]
 
 
-@jitclass([('name', unicode_type),
-           ('kernel', unicode_type),
-           ('weight_dict', DictType(UniTuple(float32, 2), float32))])
+@jitclass(
+    [
+        ("name", unicode_type),
+        ("kernel", unicode_type),
+        ("weight_dict", DictType(UniTuple(float32, 2), float32)),
+    ]
+)
 class TypedDimension:
     """Smoothing dimension specifications."""
-    def __init__(self, name: str, kernel: str, weight_dict: WeightDict) \
-            -> None:
+
+    def __init__(self, name: str, kernel: str, weight_dict: WeightDict) -> None:
         """Create smoothing dimension.
 
         Parameters
         ----------
         name : unicode_type
             Dimension name.
         kernel : unicode_type
@@ -60,15 +64,15 @@
         Dimension coordinates.
 
         Column(s) in data frame containing the coordinates of points in
         the given dimension. For example, `'age_mid'`, `['lat', 'lon']`,
         or `['super_region', 'region', 'country']`. Can be same as
         `name` attribute if dimension is 1D.
 
-    kernel : {'exponential', 'tricubic', 'depth', 'identity'}
+    kernel : {'exponential', 'tricubic', 'depth', 'inverse', 'identity'}
         Kernel function name.
 
         Name of kernel function to compute smoothing weights.
 
         See Also
         --------
         weave.kernels
@@ -81,15 +85,15 @@
         See Also
         --------
         weave.distance
 
     radius : positive number, optional
         Kernel radius.
 
-        Kernel radius if `kernel` is 'exponential' or 'depth'.
+        Kernel radius if `kernel` is 'exponential', 'depth', or 'inverse'.
 
     exponent : positive number, optional
         Kernel exponent.
 
         Kernel exponent if `kernel` is 'tricubic'.
 
     version : {'codem', 'stgpr'}, optional
@@ -103,41 +107,45 @@
         User-defined dictionary of distances between points if
         `distance` attribute is 'dictionary'. Dictionary keys are
         tuples of point ID pairs, and dictionary values are the
         corresponding distances.
 
     """
 
-    def __init__(self, name: str,
-                 coordinates: Optional[Union[str, List[str]]] = None,
-                 kernel: Optional[str] = 'identity',
-                 distance: Optional[str] = None,
-                 radius: Optional[number] = None,
-                 exponent: Optional[number] = None,
-                 version: Optional[str] = None,
-                 distance_dict: Optional[DistanceDict] = None) -> None:
+    def __init__(
+        self,
+        name: str,
+        coordinates: Optional[Union[str, List[str]]] = None,
+        kernel: Optional[str] = "identity",
+        distance: Optional[str] = None,
+        radius: Optional[number] = None,
+        exponent: Optional[number] = None,
+        version: Optional[str] = None,
+        distance_dict: Optional[DistanceDict] = None,
+    ) -> None:
         """Create smoothing dimension.
 
         Parameters
         ----------
         name : str
             Dimension name.
         coordinates : str or list of str, optional
             Dimension coordinates, if different from `name`.
-        kernel : {'exponential', 'tricubic', 'depth', 'identity'}, optional
+        kernel : {'exponential', 'tricubic', 'depth', 'inverse', 'identity'}, optional
             Kernel function name. Default is 'identity'.
         distance : {'euclidean', 'tree', 'dictionary'}, optional
             Distance function name. If None, default distance function
             is assigned based on `kernel`.
 
         Other Parameters
         ----------------
         radius : positive number, optional
-            Kernel radius if `kernel` is 'exponential' or 'depth'. For
-            depth kernel, `radius` must be a float in (0.5, 1).
+            Kernel radius if `kernel` is 'exponential', 'depth', or
+            'inverse'. For depth kernel, `radius` must be a float in
+            (0.5, 1).
         exponent : positive number, optional
             Kernel exponent if `kernel` is 'tricubic'.
         version : {'codem', 'stgpr'}, optional
             Kernel version if `kernel` is 'depth'. Default is 'codem'.
         distance_dict : dict of {(number, number): number}, optional
             Dictionary of distances between points if `distance` is
             'dictionary'. Dictionary values must be nonnegative.
@@ -167,14 +175,18 @@
                - ``radius``
                - float in :math:`(0.5, 1)`
                - ``tree``
              * -
                - ``version``
                - \\{'codem', 'stgpr'\\}, optional (default is 'codem')
                -
+             * - ``inverse``
+               - ``radius``
+               - Positive number
+               - ``euclidean``
              * - ``identity``
                -
                -
                - ``euclidean``
 
         The identity kernel does not have any kernel parameters because
         the weight values are equal to the distance values.
@@ -283,20 +295,20 @@
         AttributeError
             If `name` has already been set.
         TypeError
             If `name` is not a str.
 
         """
         # Once set, `name` cannot be changed
-        if hasattr(self, 'name'):
-            raise AttributeError('`name` cannot be changed')
+        if hasattr(self, "name"):
+            raise AttributeError("`name` cannot be changed")
 
         # Check type
         if not isinstance(name, str):
-            raise TypeError('`name` is not a str')
+            raise TypeError("`name` is not a str")
 
         self._name = name
 
     @property
     def coordinates(self) -> List[str]:
         """Get dimension coordinates.
 
@@ -305,16 +317,15 @@
         list of str
             Dimension coordinates.
 
         """
         return self._coordinates
 
     @coordinates.setter
-    def coordinates(self, coordinates: Optional[Union[str, List[str]]]) \
-            -> None:
+    def coordinates(self, coordinates: Optional[Union[str, List[str]]]) -> None:
         """Set dimension coordinates.
 
         Parameters
         ----------
         coordinates : str or list of str, optional
             Dimension coordinates. If None, set equal to `name`.
 
@@ -325,31 +336,31 @@
         TypeError
             If `coordinates` not a str or list of str or None.
         ValueError
             If `coordinates` is an empty list or contains duplicates.
 
         """
         # Once set, `coordinates` cannot be changed
-        if hasattr(self, 'coordinates'):
-            raise AttributeError('`coordinates` cannot be changed')
+        if hasattr(self, "coordinates"):
+            raise AttributeError("`coordinates` cannot be changed")
 
         # Set default
         if coordinates is None:
             coordinates = self._name
 
         # Check types
         coordinates = as_list(coordinates)
         if not all(isinstance(coord, str) for coord in coordinates):
-            raise TypeError('`coordinates` contains invalid types')
+            raise TypeError("`coordinates` contains invalid types")
 
         # Check values
         if len(coordinates) == 0:
-            raise ValueError('`coordinates` is an empty list')
+            raise ValueError("`coordinates` is an empty list")
         if len(coordinates) > len(set(coordinates)):
-            raise ValueError('`coordinates` contains duplicates')
+            raise ValueError("`coordinates` contains duplicates")
 
         self._coordinates = coordinates
 
     @property
     def kernel(self) -> str:
         """Get kernel function name.
 
@@ -363,38 +374,38 @@
 
     @kernel.setter
     def kernel(self, kernel: str) -> None:
         """Set kernel function name.
 
         Parameters
         ----------
-        kernel : {'depth', 'exponential', 'identity', 'tricubic'}
+        kernel : {'exponential', 'tricubic', 'depth', 'inverse', 'identity'}
             Kernel function name.
 
         Raises
         ------
         AttributeError
             If `kernel` has already been set.
         TypeError
             If `kernel` not a str.
         ValueError
             If `kernel` is not a valid kernel function.
 
         """
         # Once set, `kernel` cannot be changed
-        if hasattr(self, 'kernel'):
-            raise AttributeError('`kernel` cannot be changed')
+        if hasattr(self, "kernel"):
+            raise AttributeError("`kernel` cannot be changed")
 
         # Check type
         if not isinstance(kernel, str):
-            raise TypeError('`kernel` is not a str')
+            raise TypeError("`kernel` is not a str")
 
         # Check value
-        if kernel not in ('exponential', 'tricubic', 'depth', 'identity'):
-            raise ValueError('`kernel` is not a valid kernel function')
+        if kernel not in ("exponential", "tricubic", "depth", "inverse", "identity"):
+            raise ValueError("`kernel` is not a valid kernel function")
 
         self._kernel = kernel
 
     @property
     def distance(self) -> str:
         """Get distance function name.
 
@@ -422,82 +433,82 @@
         TypeError
             If `distance` is not a str or None.
         ValueError
             If `distance` is not a valid distance function.
 
         """
         # Once set, `distance` cannot be changed
-        if hasattr(self, 'distance'):
-            raise AttributeError('`distance` cannot be changed')
+        if hasattr(self, "distance"):
+            raise AttributeError("`distance` cannot be changed")
 
         # Set default
         if distance is None:
-            if self._kernel == 'depth':
-                distance = 'tree'
+            if self._kernel == "depth":
+                distance = "tree"
             else:
-                distance = 'euclidean'
+                distance = "euclidean"
 
         # Check type
         if not isinstance(distance, str):
-            raise TypeError('`distance` is not a str')
+            raise TypeError("`distance` is not a str")
 
         # Check value
-        if distance not in ('euclidean', 'tree', 'dictionary'):
-            msg = '`distance` is not a valid distance function'
+        if distance not in ("euclidean", "tree", "dictionary"):
+            msg = "`distance` is not a valid distance function"
             raise ValueError(msg)
 
         self._distance = distance
 
     @property
     def radius(self) -> number:
-        """Get kernel radius if `kernel` is 'exponential' or 'depth'.
+        """Get kernel radius if `kernel` is 'exponential', 'depth', or 'inverse'.
 
         Returns
         -------
         positive number
             Kernel radius.
 
         """
         return self._radius
 
     @radius.setter
     def radius(self, radius: Optional[number]) -> None:
-        """Set kernel radius if `kernel` is 'exponential' or 'depth'.
+        """Set kernel radius if `kernel` is 'exponential', 'depth', or 'inverse'.
 
         Parameters
         ----------
         radius : positive number or None
             Kernel radius.
 
         Raises
         ------
         AttributeError
-            If `kernel` is 'exponential' or 'depth' but `radius` is None.
+            If `kernel` is 'exponential', 'depth', or 'inverse' but `radius` is None.
         TypeError
-            If `kernel` is 'exponential' but `radius` is not a number.
+            If `kernel` is 'exponential' or 'inverse' but `radius` is not a number.
             If `kernel` is 'depth' but `radius` is not a float.
         ValueError
-            If `kernel` is 'exponential' but `radius` is not positive.
+            If `kernel` is 'exponential' or 'inverse' but `radius` is not positive.
             If `kernel` is 'depth' but `radius` is not in (0.5, 1).
 
         """
-        if self._kernel in ('exponential', 'depth'):
+        if self._kernel in ("exponential", "depth", "inverse"):
             if radius is None:
                 msg = f"`radius` is required for '{self._kernel}' kernel"
                 raise AttributeError(msg)
-            if self._kernel == 'exponential':
+            if self._kernel in ("exponential", "inverse"):
                 if not is_number(radius):
-                    raise TypeError('`radius` is not an int or float')
+                    raise TypeError("`radius` is not an int or float")
                 if radius <= 0:
-                    raise ValueError('`radius` is not positive')
-            elif self._kernel == 'depth':
+                    raise ValueError("`radius` is not positive")
+            elif self._kernel == "depth":
                 if not is_float(radius):
-                    raise TypeError('`radius` is not a float')
+                    raise TypeError("`radius` is not a float")
                 if radius <= 0.5 or radius >= 1:
-                    raise ValueError('`radius` is not in (0.5, 1)')
+                    raise ValueError("`radius` is not in (0.5, 1)")
             self._radius = radius
 
     @property
     def exponent(self) -> number:
         """Get kernel exponent if `kernel` is 'tricubic'.
 
         Returns
@@ -523,22 +534,22 @@
             If `kernel` is 'tricubic' but `exponent` is None.
         TypeError
             If `kernel` is 'tricubic' but `exponent` is not a number.
         ValueError
             If `kernel` is 'tricubic' but `exponent` is not positive.
 
         """
-        if self._kernel == 'tricubic':
+        if self._kernel == "tricubic":
             if exponent is None:
                 msg = "`exponent` is required for 'tricubic' kernel"
                 raise AttributeError(msg)
             if not is_number(exponent):
-                raise TypeError('`exponent` is not an int or float')
+                raise TypeError("`exponent` is not an int or float")
             if exponent <= 0:
-                raise ValueError('`exponent` is not positive')
+                raise ValueError("`exponent` is not positive")
             self._exponent = exponent
 
     @property
     def version(self) -> str:
         """Get kernel version if `kernel` is 'depth'.
 
         Returns
@@ -563,21 +574,21 @@
         TypeError
             If `kernel` is 'depth' but `version` is not a str or None.
         ValueError
             If `kernel` is 'depth' but `version` not in
             {'codem', 'stgpr'}.
 
         """
-        if self._kernel == 'depth':
+        if self._kernel == "depth":
             if version is None:
-                self._version = 'codem'
+                self._version = "codem"
             else:
                 if not isinstance(version, str):
-                    raise TypeError('`version` is not a str')
-                if version not in ('codem', 'stgpr'):
+                    raise TypeError("`version` is not a str")
+                if version not in ("codem", "stgpr"):
                     raise ValueError("`version` not in {'codem', 'stgpr'}")
                 self._version = version
 
     @property
     def distance_dict(self) -> DistanceDict:
         """Get dictionary of distances between points.
 
@@ -603,22 +614,22 @@
         AttributeError
             If `distance_dict` has already been set.
         ValueError
             If `distance` is 'dictionary' but `distance_dict` is None.
 
         """
         # Once set, `distance_dict` cannot be changed
-        if hasattr(self, 'distance_dict'):
-            raise AttributeError('`distance_dict` cannot be changed')
+        if hasattr(self, "distance_dict"):
+            raise AttributeError("`distance_dict` cannot be changed")
 
         # Check values
-        if self._distance == 'dictionary':
+        if self._distance == "dictionary":
             if distance_dict is None:
                 msg = "`distance` is 'dictionary', "
-                msg += 'but `distance_dict` is None'
+                msg += "but `distance_dict` is None"
                 raise ValueError(msg)
             check_dict(distance_dict)
             self._distance_dict = distance_dict
 
     def get_typed_dimension(self, data: DataFrame) -> TypedDimension:
         """Get smoothing dimension cast as jitclass object.
 
@@ -651,27 +662,28 @@
 
         """
         # Get point names and coordinates
         points = data[[self._name] + self._coordinates]
         points = np.array(points.drop_duplicates(), dtype=np.float32)
 
         # Initialize weight dictionary
-        weight_dict = TypedDict.empty(
-            key_type=UniTuple(float32, 2),
-            value_type=float32
-        )
+        weight_dict = TypedDict.empty(key_type=UniTuple(float32, 2), value_type=float32)
 
         # Compute weights
         for idx_x, x in enumerate(points[:, 0]):
-            distances = {y: self.get_distance(points[idx_x], points[idx_y])
-                         for idx_y, y in enumerate(points[:, 0])}
+            distances = {
+                y: self.get_distance(points[idx_x], points[idx_y])
+                for idx_y, y in enumerate(points[:, 0])
+            }
             radius = max(distances.values()) + 1  # tricubic kernel
             levels = len(points[idx_x, 1:])  # depth kernel
-            weights = {(x, y): self.get_weight(distances[y], radius, levels)
-                       for y in points[:, 0]}
+            weights = {
+                (x, y): self.get_weight(distances[y], radius, levels)
+                for y in points[:, 0]
+            }
             weight_dict.update(weights)
 
         return weight_dict
 
     def get_distance(self, x: np.ndarray, y: np.ndarray) -> np.float32:
         """Get distance between `x` and `y`.
 
@@ -684,22 +696,21 @@
 
         Returns
         -------
         nonnegative float32
             Distance between `x` and `y`.
 
         """
-        if self._distance == 'euclidean':
+        if self._distance == "euclidean":
             return euclidean(x[1:], y[1:])
-        if self._distance == 'tree':
+        if self._distance == "tree":
             return tree(x[1:], y[1:])
         return np.float32(self._distance_dict[(x[0], y[0])])
 
-    def get_weight(self, distance: number, radius: number, levels: int) \
-            -> np.float32:
+    def get_weight(self, distance: number, radius: number, levels: int) -> np.float32:
         """Get dimension smoothing weight.
 
         Parameters
         ----------
         distance : nonnegative int or float
             Distance between points.
         radius : positive int or float
@@ -709,20 +720,22 @@
 
         Returns
         -------
         nonnegative float32
             Dimension smoothing weight.
 
         """
-        if self._kernel == 'exponential':
+        if self._kernel == "exponential":
             return exponential(distance, self._radius)
-        if self._kernel == 'tricubic':
+        if self._kernel == "tricubic":
             return tricubic(distance, radius, self._exponent)
-        if self._kernel == 'depth':
+        if self._kernel == "depth":
             return depth(distance, levels, self._radius, self._version)
+        if self._kernel == "inverse":
+            return inverse(distance, self._radius)
         return np.float32(distance)  # identity
 
 
 def check_dict(distance_dict: Dict[Tuple[number, number], number]) -> None:
     """Check distance dictionary keys and values.
 
     Parameters
@@ -742,22 +755,22 @@
     -----
     Does not check that the values in `distance_dict` satisfy
     properties 2-4 in `weave.distance`.
 
     """
     # Check types
     if not isinstance(distance_dict, dict):
-        raise TypeError('`distance_dict` is not a dict')
+        raise TypeError("`distance_dict` is not a dict")
     if not all(isinstance(key, tuple) for key in distance_dict):
-        raise TypeError('`distance_dict` keys not all tuple')
+        raise TypeError("`distance_dict` keys not all tuple")
     if not all(is_number(point) for key in distance_dict for point in key):
-        raise TypeError('`distance_dict` key entries not all int or float')
+        raise TypeError("`distance_dict` key entries not all int or float")
     if not all(is_number(value) for value in distance_dict.values()):
-        raise TypeError('`distance_dict` values not all int or float')
+        raise TypeError("`distance_dict` values not all int or float")
 
     # Check values
     if len(distance_dict) == 0:
-        raise ValueError('`distance_dict` is an empty dict')
+        raise ValueError("`distance_dict` is an empty dict")
     if any(len(key) != 2 for key in distance_dict):
-        raise ValueError('`distance_dict` keys are not all length 2')
+        raise ValueError("`distance_dict` keys are not all length 2")
     if any(value < 0.0 for value in distance_dict.values()):
-        raise ValueError('`distance_dict` contains negative values')
+        raise ValueError("`distance_dict` contains negative values")
```

### Comparing `weighted-average-1.1.2/src/weave/distance.py` & `weighted_average-1.2.0/src/weave/distance.py`

 * *Files identical despite different names*

### Comparing `weighted-average-1.1.2/src/weave/kernels.py` & `weighted_average-1.2.0/src/weave/kernels.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
        <https://en.wikipedia.org/wiki/Kernel_smoother>`_
 .. [2] `Cause of Death Ensemble model
        <https://pophealthmetrics.biomedcentral.com/articles/10.1186/1478-7954-10-1>`_
 .. [3] `Kernel (statistics)
        <https://en.wikipedia.org/wiki/Kernel_(statistics)#Kernel_functions_in_common_use>`_
 
 """
+# TODO: add note about inverse-distance kernel to kernel module documentation
 from typing import Union
 
 import numpy as np
 
 number = Union[int, float]
 
 
@@ -85,15 +86,15 @@
     1.0
     >>> exponential(1, 0.5)
     0.13533528
     >>> exponential(2, 0.5)
     0.01831564
 
     """
-    return np.float32(1/np.exp(distance/radius))
+    return np.float32(1 / np.exp(distance / radius))
 
 
 def tricubic(distance: number, radius: number, exponent: number) -> np.float32:
     """Get tricubic smoothing weight.
 
     Parameters
     ----------
@@ -139,19 +140,18 @@
     1.0
     >>> tricubic(1, 2, 3)
     0.6699219
     >>> tricubic(2, 2, 3)
     0.0
 
     """
-    return np.float32(np.maximum(0, (1 - (distance/radius)**exponent)**3))
+    return np.float32(np.maximum(0, (1 - (distance / radius) ** exponent) ** 3))
 
 
-def depth(distance: number, levels: int, radius: float, version: str) \
-        -> np.float32:
+def depth(distance: number, levels: int, radius: float, version: str) -> np.float32:
     """Get depth smoothing weight.
 
     Parameters
     ----------
     distance : nonnegative int or float
         Distance between points.
     levels : positive int
@@ -227,12 +227,48 @@
     >>> depth(2, 3, 0.9, 'stgpr')
     0.81
     >>> depth(3, 3, 0.9, 'stgpr')
     0.0
 
     """
     same_tree = distance <= levels - 1
-    if version == 'stgpr':
-        return np.float32(same_tree*radius**np.ceil(distance))
+    if version == "stgpr":
+        return np.float32(same_tree * radius ** np.ceil(distance))
     not_root = levels > 1 and distance <= levels - 2
-    weight = same_tree*radius**not_root*(1 - radius)**np.ceil(distance)
+    weight = same_tree * radius**not_root * (1 - radius) ** np.ceil(distance)
     return np.float32(weight)
+
+
+def inverse(distance: number, radius: float) -> np.float32:
+    """Get inverse-distance smoothing weight.
+
+    Parameters
+    ----------
+    distance : nonnegative int or float
+        Distance between points.
+    radius : positive int or float
+        Kernel radius.
+
+    Returns
+    -------
+    nonnegative numpy.float32
+        Inverse-distance smoothing weight.
+
+    Notes
+    -----
+    The inverse-distance kernel function for a single dimension is
+    defined as
+
+    .. math:: k(d; r) = \\frac{d}{r},
+
+    which is combined over all dimensions :math:`m \in \mathcal{M}` to
+    create intermediate weights
+
+    .. math:: \\tilde{w}_{i,j} = \\frac{1}
+              {\\sum_{m \\in \\mathcal{M}} k(d_{i,j}^m; r^m) + \\sigma_i^2}.
+
+    When using inverse-distance weights, all dimension kernels must be
+    set to 'inverse', and the `stdev` argument is required for
+    :mod:`weave.smoother.Smoother()`.
+
+    """
+    return np.float32(distance / radius)
```

### Comparing `weighted-average-1.1.2/src/weave/smoother.py` & `weighted_average-1.2.0/src/weave/smoother.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # pylint: disable=C0103, E0611, E1133, R0912, R0913, R0914
 """Smooth data across multiple dimensions using weighted averages."""
 from itertools import product
 from typing import List, Optional, Union
 import warnings
 
-from numba import njit, prange  # type: ignore
+from numba import njit  # type: ignore
 from numba.typed import List as TypedList  # type: ignore
 import numpy as np
 from pandas import DataFrame  # type: ignore
 from pandas.api.types import is_bool_dtype, is_numeric_dtype  # type: ignore
 
 from weave.dimension import Dimension, TypedDimension
-from weave.utils import as_list, flatten
+from weave.utils import as_list, flatten, is_number
+
+number = Union[int, float]
 
 
 class Smoother:
     """Smoother function.
 
     Attributes
     ----------
     dimensions : list of Dimension
         Smoothing dimensions.
+    inverse_weights: bool
+        Whether or not to use inverse-distance weights.
 
     See Also
     --------
     weave.dimension.Dimension
 
     """
 
@@ -61,14 +65,15 @@
                 radius=0.9
             )
         >>> dimensions = [age, year, location]
         >>> smoother = Smoother(dimensions)
 
         """
         self.dimensions = as_list(dimensions)
+        self.inverse_weights = all(dim.kernel == "inverse" for dim in self._dimensions)
 
     @property
     def dimensions(self) -> List[Dimension]:
         """Get smoothing dimensions.
 
         Returns
         -------
@@ -94,38 +99,85 @@
         TypeError
             If `dimensions` is not a list of Dimension.
         ValueError
             If `dimensions` is an empty list, contains an empty list, or
             contains duplicate names or columns.
 
         """
-        # Once set, `name` cannot be changed
-        if hasattr(self, 'dimensions'):
-            raise AttributeError('`dimensions` cannot be changed')
+        # Once set, `dimensions` cannot be changed
+        if hasattr(self, "dimensions"):
+            raise AttributeError("`dimensions` cannot be changed")
 
         # Check types
         if not all(isinstance(dim, Dimension) for dim in dimensions):
-            raise TypeError('`dimensions` contains invalid types')
+            raise TypeError("`dimensions` contains invalid types")
 
         # Check values
         if len(dimensions) == 0:
-            raise ValueError('`dimensions` is an empty list')
+            raise ValueError("`dimensions` is an empty list")
         name_list = [dim.name for dim in dimensions]
         if len(name_list) > len(set(name_list)):
-            raise ValueError('Duplicate names found in `dimensions`')
+            raise ValueError("Duplicate names found in `dimensions`")
         coord_list = flatten([dim.coordinates for dim in dimensions])
         if len(coord_list) > len(set(coord_list)):
-            raise ValueError('Duplicate coordinates found in `dimensions`')
+            raise ValueError("Duplicate coordinates found in `dimensions`")
 
         self._dimensions = dimensions
 
-    def __call__(self, data: DataFrame, observed: str,
-                 stdev: Optional[str] = None, smoothed: Optional[str] = None,
-                 fit: Optional[str] = None, predict: Optional[str] = None) \
-            -> DataFrame:
+    @property
+    def inverse_weights(self) -> bool:
+        """Get inverse-distance weights flag.
+
+        Returns
+        -------
+        bool
+            Whether or not to use inverse-distance weights.
+
+        """
+        return self._inverse_weights
+
+    @inverse_weights.setter
+    def inverse_weights(self, inverse_weights: bool) -> None:
+        """Set inverse-distance weights flag.
+
+        Parameters
+        ----------
+        inverse_weights : bool
+            Whether or not to use inverse-distance weights.
+
+        Raises
+        ------
+        AttributeError
+            If `inverse_weights` has already been set.
+        ValueError
+            If dimensions have both inverse and non-inverse kernels.
+
+        """
+        # Once set, `inverse_weights` cannot be changed
+        if hasattr(self, "inverse_weights"):
+            raise AttributeError("`inverse_weights` cannot be changed")
+
+        # Check values
+        if inverse_weights:
+            self._inverse_weights = True
+        else:
+            if any(dim.kernel == "inverse" for dim in self._dimensions):
+                raise ValueError("Cannot mix inverse and non-inverse kernels")
+            self._inverse_weights = False
+
+    def __call__(
+        self,
+        data: DataFrame,
+        observed: str,
+        stdev: Optional[str] = None,
+        smoothed: Optional[str] = None,
+        fit: Optional[str] = None,
+        predict: Optional[str] = None,
+        down_weight: Optional[number] = 1,
+    ) -> DataFrame:
         """Smooth data across dimensions with weighted averages.
 
         For each point in `predict`, smooth values in `observed` using
         a weighted average of points in `fit`, where weights are
         calculated based on proximity across `dimensions`. Return a
         data frame of points in `predict` with column `smoothed`
         containing smoothed values.
@@ -133,24 +185,29 @@
         Parameters
         ----------
         data : pandas.DataFrame
             Input data structure.
         observed : str
             Column name of values to smooth.
         stdev: str, optional
-            Column name of standard deviations.
+            Column name of standard deviations. Required for
+            inverse-distance kernels.
         smoothed : str, optional
             Column name of smoothed values. If None, append '_smooth'
             to  `observed`.
         fit : str, optional
             Column name indicating points to include in weighted
             averages. If None, all points in `data` are used.
         predict : str, optional
             Column name indicating where to predict smoothed values.
             If None, predictions are made for all points in `data`.
+        down_weight : int or float in [0, 1], optional
+            Down-weight neighbors for in-sample points. Default is 1,
+            which corresponds to no down-weighting. If 0, in-sample
+            points are not smoothed.
 
         Returns
         -------
         pandas.DataFrame
             Points in `predict` with smoothed values `smoothed`.
 
         Examples
@@ -197,41 +254,103 @@
         >>> smoother(data, 'count', predict='test')
            age_id  ...  count  test  count_smooth
         0       2  ...    2.0  True      2.084069
         1       3  ...    3.0  True      2.919984
 
         """
         # Check input
-        self.check_args(data, observed, stdev, smoothed, fit, predict)
-        self.check_data(data, observed, stdev, smoothed, fit, predict)
+        self.check_input(data, observed, stdev, smoothed, fit, predict, down_weight)
         smoothed = f"{observed}_smooth" if smoothed is None else smoothed
+        down_weight = np.float32(down_weight)
 
         # Extract data
         idx_fit = self.get_indices(data, fit)
         idx_pred = self.get_indices(data, predict)
         col_obs = self.get_values(data, observed, idx_fit)
         col_sd = self.get_values(data, stdev, idx_fit)
         points = self.get_points(data)
         dim_list = self.get_typed_dimensions(data)
 
         # Calculate smoothed values
-        col_smooth = smooth(dim_list, points, col_obs, col_sd, idx_fit,
-                            idx_pred)
+        if self.inverse_weights:
+            col_smooth = smooth_inverse(
+                dim_list, points, col_obs, col_sd, idx_fit, idx_pred, down_weight
+            )
+        else:
+            col_smooth = smooth(
+                dim_list, points, col_obs, col_sd, idx_fit, idx_pred, down_weight
+            )
 
         # Construct smoothed data frame
         data_smooth = data.iloc[idx_pred].reset_index(drop=True)
         data_smooth[smoothed] = col_smooth
 
         return data_smooth
 
+    def check_input(
+        self,
+        data: DataFrame,
+        observed: str,
+        stdev: Optional[str],
+        smoothed: Optional[str],
+        fit: Optional[str],
+        predict: Optional[str],
+        down_weight: float,
+    ) -> None:
+        """Check `smoother` arguments and data.
+
+        Parameters
+        ----------
+        data : pandas.DataFrame
+            Input data structure.
+        observed : str
+            Column name of values to smooth.
+        stdev : str, optional
+            Column name of standard deviations.
+        smoothed : str, optional
+            Column name of smoothed values.
+        fit : str, optional
+            Column name indicating points to include in weighted
+            averages.
+        predict : str, optional
+            Column name indicating where to predict smoothed values.
+        down_weight : float in [0, 1]
+            Down-weight neighbors for in-sample points.
+
+        """
+        # Check argument types and values
+        self.check_arg_types(data, observed, stdev, smoothed, fit, predict, down_weight)
+        self.check_arg_values(observed, stdev, smoothed, down_weight)
+
+        # Check data and dictionary keys
+        names = [dim.name for dim in self._dimensions]
+        coords = flatten([dim.coordinates for dim in self._dimensions])
+        self.check_data_columns(
+            names, coords, data, observed, stdev, smoothed, fit, predict
+        )
+        for dim in self._dimensions:
+            if dim.distance == "dictionary":
+                self.check_dist_dict(dim, data)
+
+        # Check data types and values
+        self.check_data_types(names, coords, data, observed, stdev, fit, predict)
+        self.check_data_values(names, coords, data, observed, stdev)
+        self.check_dim_values(data)
+
     @staticmethod
-    def check_args(data: DataFrame, observed: str, stdev: Optional[str],
-                   smoothed: Optional[str], fit: Optional[str],
-                   predict: Optional[str]) -> None:
-        """Check `smoother` argument types and values.
+    def check_arg_types(
+        data: DataFrame,
+        observed: str,
+        stdev: Optional[str],
+        smoothed: Optional[str],
+        fit: Optional[str],
+        predict: Optional[str],
+        down_weight: float,
+    ) -> None:
+        """Check `smoother` argument types.
 
         Parameters
         ----------
         data : pandas.DataFrame
             Input data structure.
         observed : str
             Column name of values to smooth.
@@ -240,49 +359,93 @@
         smoothed : str, optional
             Column name of smoothed values.
         fit : str, optional
             Column name indicating points to include in weighted
             averages.
         predict : str, optional
             Column name indicating where to predict smoothed values.
+        down_weight : float in [0, 1], optional
+            Down-weight neighbors for in-sample points.
 
         Raises
         ------
         TypeError
             If `smoother` arguments contain invalid types.
-        ValueError
-            If `observed`, `stdev`, or `smoothed` overlap.
 
         """
-        # Check types
         if not isinstance(data, DataFrame):
-            raise TypeError('`data` is not a DataFrame')
+            raise TypeError("`data` is not a DataFrame")
         if not isinstance(observed, str):
-            raise TypeError('`observed` is not a str')
+            raise TypeError("`observed` is not a str")
         if stdev is not None and not isinstance(stdev, str):
-            raise TypeError('`stdev` is not a str')
+            raise TypeError("`stdev` is not a str")
         if smoothed is not None and not isinstance(smoothed, str):
-            raise TypeError('`smoothed` is not a str')
+            raise TypeError("`smoothed` is not a str")
         if fit is not None and not isinstance(fit, str):
-            raise TypeError('`fit` is not a str')
+            raise TypeError("`fit` is not a str")
         if predict is not None and not isinstance(predict, str):
-            raise TypeError('`predict` is not a str')
+            raise TypeError("`predict` is not a str")
+        if not is_number(down_weight):
+            raise TypeError("`down_weight` is not an int or float")
+
+    def check_arg_values(
+        self,
+        observed: str,
+        stdev: Optional[str],
+        smoothed: Optional[str],
+        down_weight: float,
+    ) -> None:
+        """Check `smoother` argument values.
 
-        # Check values
+        Parameters
+        ----------
+        observed : str
+            Column name of values to smooth.
+        stdev : str, optional
+            Column name of standard deviations.
+        smoothed : str, optional
+            Column name of smoothed values.
+        down_weight : float in [0, 1], optional
+            Down-weight neighbors for in-sample points.
+
+        Raises
+        ------
+        ValueError
+            If `observed`, `stdev`, or `smoothed` overlap.
+            If `stdev` not passed when `self.inverse_weights` is True.
+            If `down_weight` is not in [0, 1].
+
+        """
         col_set = set([observed, stdev, smoothed])
         if not (stdev is None and smoothed is None) and len(col_set) < 3:
-            raise ValueError('Duplicates in `observed`, `stdev`, `smoothed`')
+            raise ValueError("Duplicates in `observed`, `stdev`, `smoothed`")
+        if self.inverse_weights and stdev is None:
+            raise ValueError("`stdev` required for inverse-distance weighting")
+        if not 0 <= down_weight <= 1:
+            raise ValueError("`down_weight` must be in [0, 1]")
 
-    def check_data(self, data: DataFrame, observed: str, stdev: Optional[str],
-                   smoothed: Optional[str], fit: Optional[str],
-                   predict: Optional[str]) -> None:
-        """Check input data.
+    @staticmethod
+    def check_data_columns(
+        names: List[str],
+        coords: List[str],
+        data: DataFrame,
+        observed: str,
+        stdev: Optional[str],
+        smoothed: Optional[str],
+        fit: Optional[str],
+        predict: Optional[str],
+    ) -> None:
+        """Check data frame column names.
 
         Parameters
         ----------
+        names : list of str
+            Smoothing dimension names.
+        coords : list of str
+            Smoothing dimension coordinates.
         data : pandas.DataFrame
             Input data structure.
         observed : str
             Column name of values to smooth.
         stdev : str, optional
             Column name of standard deviations.
         smoothed : str, optional
@@ -294,95 +457,177 @@
             Column name indicating where to predict smoothed values.
 
         Raises
         ------
         KeyError
             If columns `dimension.name`, `dimensions.coordinates`,
             `observed`, `stdev`, `fit`, or `predict` not in `data`.
-            If `dimension.distance` is 'dictionary', but not all keys
-            `dimension.name` in `dimension.distance_dict`.
-        TypeError
-            If columns `dimension.name`, `dimensions.coordinates`,
-            `observed`, `stdev`, `fit`, or `predict` in `data` contain
-            invalid types.
-        ValueError
-            If columns `dimension.name` and `dimension.coordinates` not
-            one-to-one in `data`.
-            If `data` contains NaNs or Infs.
 
         Warns
         -----
         If columns in `smoothed` in `data`.
 
         """
-        # Get column names
-        names = [dim.name for dim in self._dimensions]
-        coords = flatten([dim.coordinates for dim in self._dimensions])
-
-        # Check data frame columns
         if not all(name in data for name in names):
-            raise KeyError('Not all `dimension.name` in data')
+            raise KeyError("Not all `dimension.name` in data")
         if not all(coord in data for coord in coords):
-            raise KeyError('Not all `dimension.coordinates` in data')
+            raise KeyError("Not all `dimension.coordinates` in data")
         if observed not in data:
             raise KeyError(f"`observed` column {observed} not in data")
         if stdev is not None and stdev not in data:
             raise KeyError(f"`stdev` column {stdev} not in data")
         if smoothed in data:
-            msg = f"`smoothed` column {smoothed} will be overwritten"
-            warnings.warn(msg)
+            warnings.warn(f"`smoothed` column {smoothed} will be overwritten")
         if fit is not None and fit not in data:
             raise KeyError(f"`fit` column {fit} not in data")
         if predict is not None and predict not in data:
             raise KeyError(f"`predict` column {predict} not in data")
 
-        # Check dictionary keys
-        for dim in self._dimensions:
-            if dim.distance == 'dictionary':
-                dim_names = data[dim.name].unique()
-                for key in product(dim_names, repeat=2):
-                    if key not in dim.distance_dict:
-                        msg = 'Not all `dimension.name` in '
-                        msg += '`dimension.distance_dict`'
-                        raise KeyError(msg)
+    @staticmethod
+    def check_dist_dict(dimension: Dimension, data: DataFrame) -> None:
+        """Check distance dictionary keys.
 
-        # Check types
+        Parameters
+        ----------
+        dimension : Dimension
+            Smoothing dimension.
+        data : pandas.DataFrame
+            Input data structure.
+
+        Raises
+        ------
+        KeyError
+            If `dimension.distance` is 'dictionary', but not all keys
+            `dimension.name` in `dimension.distance_dict`.
+
+        """
+        dim_names = data[dimension.name].unique()
+        for key in product(dim_names, repeat=2):
+            if key not in dimension.distance_dict:
+                raise KeyError("Not all `dimension.name` in `dimension.distance_dict`")
+
+    @staticmethod
+    def check_data_types(
+        names: List[str],
+        coords: List[str],
+        data: DataFrame,
+        observed: str,
+        stdev: Optional[str],
+        fit: Optional[str],
+        predict: Optional[str],
+    ) -> None:
+        """Check input data types.
+
+        Parameters
+        ----------
+        names : list of str
+            Smoothing dimension names.
+        coords : list of str
+            Smoothing dimension coordinates.
+        data : pandas.DataFrame
+            Input data structure.
+        observed : str
+            Column name of values to smooth.
+        stdev : str, optional
+            Column name of standard deviations.
+        fit : str, optional
+            Column name indicating points to include in weighted
+            averages.
+        predict : str, optional
+            Column name indicating where to predict smoothed values.
+
+        Raises
+        ------
+        TypeError
+            If columns `dimension.name`, `dimensions.coordinates`,
+            `observed`, `stdev`, `fit`, or `predict` in `data` contain
+            invalid types.
+
+        """
         if not all(is_numeric_dtype(data[name]) for name in names):
-            raise TypeError('Not all `dimension.name` data int or float')
+            raise TypeError("Not all `dimension.name` data int or float")
         if not all(is_numeric_dtype(data[coord]) for coord in coords):
-            msg = 'Not all `dimension.coordinates` data int or float'
-            raise TypeError(msg)
+            raise TypeError("Not all `dimension.coordinates` data int or float")
         if not is_numeric_dtype(data[observed]):
             raise TypeError(f"`observed` data {observed} not int or float")
         if stdev is not None:
             if not is_numeric_dtype(data[stdev]):
                 raise TypeError(f"`stdev` data {stdev} is not int or float")
         if fit is not None:
             if not is_bool_dtype(data[fit]):
                 raise TypeError(f"`fit` data {fit} is not bool")
         if predict is not None:
             if not is_bool_dtype(data[predict]):
                 raise TypeError(f"`predict` data {predict} is not bool")
 
-        # Check `name` and `coordinates` one-to-one
+    @staticmethod
+    def check_data_values(
+        names: List[str],
+        coords: List[str],
+        data: DataFrame,
+        observed: str,
+        stdev: Optional[str],
+    ) -> None:
+        """Check input data.
+
+        Parameters
+        ----------
+        names : list of str
+            Smoothing dimension names.
+        coords : list of str
+            Smoothing dimension coordinates.
+        data : pandas.DataFrame
+            Input data structure.
+        observed : str
+            Column name of values to smooth.
+        stdev : str, optional
+            Column name of standard deviations.
+
+        Raises
+        ------
+        ValueError
+            If `data` contains NaNs or Infs.
+            If `stdev` contains zeros or negative values.
+
+        """
+        if data.isna().any(axis=None):
+            raise ValueError("`data` contains NaNs")
+        cols_in = [observed] if stdev is None else [observed, stdev]
+        if np.isinf(data[names + coords + cols_in]).any(axis=None):
+            raise ValueError("`data` contains Infs")
+        if stdev is not None:
+            if np.any(data[stdev] <= 0):
+                raise ValueError("`stdev` values must be positive")
+
+    def check_dim_values(
+        self,
+        data: DataFrame,
+    ) -> None:
+        """Check dimension names and coordinates one-to-one in data.
+
+        Parameters
+        ----------
+        data : pandas.DataFrame
+            Input data structure.
+
+        Raises
+        ------
+        ValueError
+            If columns `dimension.name` and `dimension.coordinates` not
+            one-to-one in `data`.
+
+        """
         for dim in self._dimensions:
             if [dim.name] != dim.coordinates:
                 points = data[[dim.name] + dim.coordinates].drop_duplicates()
                 points = points.loc[:, ~points.columns.duplicated()]
                 if any(points.groupby(dim.name).size() != 1):
-                    raise ValueError('`name` maps to multiple `coordinates`')
+                    raise ValueError("`name` maps to multiple `coordinates`")
                 if any(points.groupby(dim.coordinates).size() != 1):
-                    raise ValueError('`coordinates` maps to multiple `name`')
-
-        # Check values
-        if data.isna().any(axis=None):
-            raise ValueError('`data` contains NaNs')
-        cols_in = [observed] if stdev is None else [observed, stdev]
-        if np.isinf(data[names + coords + cols_in]).any(axis=None):
-            raise ValueError('`data` contains Infs')
+                    raise ValueError("`coordinates` maps to multiple `name`")
 
     @staticmethod
     def get_indices(data: DataFrame, indicator: str = None) -> np.ndarray:
         """Get indices of `fit` or `predict` data.
 
         Parameters
         ----------
@@ -398,16 +643,17 @@
 
         """
         if indicator is None:
             return np.arange(len(data)).astype(np.int32)
         return np.where(data[indicator])[0].astype(np.int32)
 
     @staticmethod
-    def get_values(data: DataFrame, values: Optional[str],
-                   idx_fit: np.ndarray) -> np.ndarray:
+    def get_values(
+        data: DataFrame, values: Optional[str], idx_fit: np.ndarray
+    ) -> np.ndarray:
         """Get input values.
 
         Parameters
         ----------
         data : pandas.DataFrame
             Input data structure.
         values : str, optional
@@ -418,15 +664,15 @@
         Returns
         -------
         numpy.ndarray of float32
             Input values.
 
         """
         if values is None:
-            return np.nan*np.ones(len(idx_fit)).astype(np.float32)
+            return np.nan * np.ones(len(idx_fit)).astype(np.float32)
         return np.array(data[values].values[idx_fit], dtype=np.float32)
 
     def get_points(self, data: DataFrame) -> np.ndarray:
         """Get point IDs.
 
         Parameters
         ----------
@@ -438,37 +684,43 @@
         2D numpy.ndarray of float32
             Point IDs.
 
         """
         points = [dim.name for dim in self._dimensions]
         return np.ascontiguousarray(data[points].values, dtype=np.float32)
 
-    def get_typed_dimensions(self, data: DataFrame) \
-            -> TypedList[TypedDimension]:
+    def get_typed_dimensions(self, data: DataFrame) -> TypedList[TypedDimension]:
         """Get smoothing dimensions cast as jitclass objects.
 
         Parameters
         ----------
         data : pandas.DataFrame
             Input data structure.
 
         Returns
         -------
         numba.typed.List of TypedDimension
             Smoothing dimensions cast as jitclass objects.
 
         """
-        return TypedList([dimension.get_typed_dimension(data)
-                          for dimension in self._dimensions])
+        return TypedList(
+            [dimension.get_typed_dimension(data) for dimension in self._dimensions]
+        )
 
 
-@njit(parallel=True)
-def smooth(dim_list: List[TypedDimension], points: np.ndarray,
-           col_obs: np.ndarray, col_sd: np.ndarray, idx_fit: np.ndarray,
-           idx_pred: np.ndarray) -> np.ndarray:
+@njit
+def smooth(
+    dim_list: List[TypedDimension],
+    points: np.ndarray,
+    col_obs: np.ndarray,
+    col_sd: np.ndarray,
+    idx_fit: np.ndarray,
+    idx_pred: np.ndarray,
+    down_weight: float,
+) -> np.ndarray:
     """Smooth data across dimensions with weighted averages.
 
     Parameters
     ----------
     dim_list : list of TypedDimension
         Smoothing dimensions.
     points : 2D numpy.ndarray of float
@@ -477,46 +729,111 @@
         Values to smooth.
     col_sd: 1D numpy.ndarray of float
         Standard deviations.
     idx_fit : 1D numpy.ndarray of int
         Indices of points to include in weighted averages.
     idx_pred: 1D numpy.ndarray of int
         Indices of points to predict smoothed values.
+    down_weight: float in [0, 1]
+        Down-weight neighbors for in-sample points.
 
     Returns
     -------
     1D numpy.ndarray of float32
         Smoothed values.
 
     """
     # Initialize weight matrix
     n_fit = len(idx_fit)
     n_pred = len(idx_pred)
     weights = np.ones((n_pred, n_fit), dtype=np.float32)
 
-    # Calculate weights one dimension at a time
-    for idx_dim, dim in enumerate(dim_list):
-        dim_weights = np.zeros((n_pred, n_fit), dtype=np.float32)
-        for ii in prange(n_pred):
+    # Calculate weights one prediction at a time
+    for ii in range(n_pred):
+        for idx_dim, dim in enumerate(dim_list):
             pred = points[idx_pred[ii], idx_dim]
+            dim_weights = np.zeros(n_fit, dtype=np.float32)
             for jj in range(n_fit):
                 fit = points[idx_fit[jj], idx_dim]
-                dim_weights[ii, jj] = dim.weight_dict[(pred, fit)]
+                dim_weights[jj] = dim.weight_dict[(pred, fit)]
 
             # Normalize by depth subgroup
-            if dim.kernel == 'depth':
-                for weight in list(set(dim_weights[ii, :])):
-                    cond = dim_weights[ii, :] == weight
-                    scale = np.where(cond, weights[ii, :], 0).sum()
+            if dim.kernel == "depth":
+                for weight in list(set(dim_weights)):
+                    cond = dim_weights == weight
+                    scale = np.where(cond, weights[ii], 0).sum()
                     if scale != 0:
-                        weights[ii, :] = np.where(cond, weights[ii, :]/scale,
-                                                  weights[ii, :])
+                        weights[ii] = np.where(cond, weights[ii] / scale, weights[ii])
+
+            # Update weight matrix
+            weights[ii] *= dim_weights
 
-        # Update weight matrix
-        weights *= dim_weights
+        # Down-weight neighbors for in-sample points
+        if idx_pred[ii] in idx_fit and down_weight < 1:
+            neighbors = idx_pred[ii] != idx_fit
+            weights[ii] = np.where(neighbors, weights[ii] * down_weight, weights[ii])
 
     # Scale by standard deviation
     if not np.isnan(col_sd).any():
-        weights = weights/(col_sd**2)
+        weights = weights / (col_sd**2)
 
     # Compute smoothed values
-    return weights.dot(col_obs)/weights.sum(axis=1)
+    return weights.dot(col_obs) / weights.sum(axis=1)
+
+
+@njit
+def smooth_inverse(
+    dim_list: List[TypedDimension],
+    points: np.ndarray,
+    col_obs: np.ndarray,
+    col_sd: np.ndarray,
+    idx_fit: np.ndarray,
+    idx_pred: np.ndarray,
+    down_weight: float,
+) -> np.ndarray:
+    """Smooth data across dimensions with inverse-distance weighted averages.
+
+    Parameters
+    ----------
+    dim_list : list of TypedDimension
+        Smoothing dimensions.
+    points : 2D numpy.ndarray of float
+        Point IDs.
+    col_obs : 1D numpy.ndarray of float
+        Values to smooth.
+    col_sd: 1D numpy.ndarray of float
+        Standard deviations.
+    idx_fit : 1D numpy.ndarray of int
+        Indices of points to include in weighted averages.
+    idx_pred: 1D numpy.ndarray of int
+        Indices of points to predict smoothed values.
+    down_weight: float in [0, 1]
+        Down-weight neighbors for in-sample points.
+
+    Returns
+    -------
+    1D numpy.ndarray of float32
+        Smoothed values.
+
+    """
+    # Initialize distance matrix
+    n_fit = len(idx_fit)
+    n_pred = len(idx_pred)
+    weights = np.zeros((n_pred, n_fit), dtype=np.float32)
+
+    # Calculate distance weights one prediction at a time
+    for ii in range(n_pred):
+        distance = col_sd**2
+        for idx_dim, dim in enumerate(dim_list):
+            pred = points[idx_pred[ii], idx_dim]
+            dim_distance = np.zeros(n_fit, dtype=np.float32)
+            for jj in range(n_fit):
+                fit = points[idx_fit[jj], idx_dim]
+                dim_distance[jj] = dim.weight_dict[(pred, fit)]
+            distance += dim_distance
+        weights[ii] = 1 / distance
+        if idx_pred[ii] in idx_fit and down_weight < 1:
+            neighbors = idx_pred[ii] != idx_fit
+            weights[ii] = np.where(neighbors, weights[ii] * down_weight, weights[ii])
+
+    # Compute smoothed values with inverse-distance weights
+    return weights.dot(col_obs) / weights.sum(axis=1)
```

### Comparing `weighted-average-1.1.2/src/weave/utils.py` & `weighted_average-1.2.0/src/weave/utils.py`

 * *Files identical despite different names*

### Comparing `weighted-average-1.1.2/src/weighted_average.egg-info/PKG-INFO` & `weighted_average-1.2.0/src/weighted_average.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weighted-average
-Version: 1.1.2
+Version: 1.2.0
 Summary: Smooth data across multiple dimensions using weighted averages
 Home-page: https://github.com/ihmeuw-msca/weighted-average
 Author: IHME Math Sciences
 Author-email: ihme.math.sciences@gmail.com
 License: BSD 2-Clause License
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `weighted-average-1.1.2/src/weighted_average.egg-info/SOURCES.txt` & `weighted_average-1.2.0/src/weighted_average.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `weighted-average-1.1.2/tests/test_dimension.py` & `weighted_average-1.2.0/tests/test_dimension.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,354 +1,392 @@
 """Tests for Dimension class."""
+
 import pytest
 
 from weave.dimension import Dimension
 
 # Lists of wrong types to test exceptions
-not_int = [1.0, 'dummy', True, None, [], (), {}]
-not_float = [1, 'dummy', True, None, [], (), {}]
-not_numeric = ['dummy', True, None, [], (), {}]
+not_int = [1.0, "dummy", True, None, [], (), {}]
+not_float = [1, "dummy", True, None, [], (), {}]
+not_numeric = ["dummy", True, None, [], (), {}]
 not_str = [1, 1.0, True, None, [], (), {}]
-not_bool = [1, 1.0, 'dummy', None, [], (), {}]
-not_tuple = [1, 1.0, 'dummy', True, None, [], {}]
+not_bool = [1, 1.0, "dummy", None, [], (), {}]
+not_tuple = [1, 1.0, "dummy", True, None, [], {}]
 not_coordinates = not_str + [[value] for value in not_str]
-not_dict = [1, 1.0, 'dummy', True, None, [], ()]
+not_dict = [1, 1.0, "dummy", True, None, [], ()]
 
 # Example kernel parameters and distance dictionary
-kernel_pars = {'radius': 0.6, 'exponent': 3}
+kernel_pars = {"radius": 0.6, "exponent": 3}
 distance_dict = {(1.0, 1.0): 1.0}
 
 
 # Test constructor types
-@pytest.mark.parametrize('name', not_str)
+@pytest.mark.parametrize("name", not_str)
 def test_name_type(name):
     """Raise TypeError if `name` not a str."""
     with pytest.raises(TypeError):
         Dimension(name)
 
 
-@pytest.mark.parametrize('coordinates', not_coordinates)
+@pytest.mark.parametrize("coordinates", not_coordinates)
 def test_coordinates_type(coordinates):
     """Raise TypeError if `coordinates` is not a str or list of str."""
     if coordinates is not None and coordinates != []:
         with pytest.raises(TypeError):
-            Dimension('dummy', coordinates)
+            Dimension("dummy", coordinates)
 
 
-@pytest.mark.parametrize('kernel', not_str)
+@pytest.mark.parametrize("kernel", not_str)
 def test_kernel_type(kernel):
     """Raise TypeError if `kernel` is not a str."""
     with pytest.raises(TypeError):
-        Dimension('dummy', kernel=kernel)
+        Dimension("dummy", kernel=kernel)
 
 
-@pytest.mark.parametrize('radius', not_numeric)
+@pytest.mark.parametrize("radius", not_numeric)
 def test_exponential_radius_type(radius):
     """Raise TypeError if `radius` is not an int or float."""
     if radius is not None:
         with pytest.raises(TypeError):
-            Dimension('dummy', kernel='exponential', radius=radius)
+            Dimension("dummy", kernel="exponential", radius=radius)
 
 
-@pytest.mark.parametrize('exponent', not_numeric)
+@pytest.mark.parametrize("exponent", not_numeric)
 def test_tricubic_exponent_type(exponent):
     """Raise TypeError if `exponent` is not an int or float."""
     if exponent is not None:
         with pytest.raises(TypeError):
-            Dimension('dummy', kernel='tricubic', exponent=exponent)
+            Dimension("dummy", kernel="tricubic", exponent=exponent)
 
 
-@pytest.mark.parametrize('radius', not_float)
+@pytest.mark.parametrize("radius", not_float)
 def test_depth_radius_type(radius):
     """Raise TypeError if `radius` is not a float."""
     if radius is not None:
         with pytest.raises(TypeError):
-            Dimension('dummy', kernel='depth', radius=radius)
+            Dimension("dummy", kernel="depth", radius=radius)
 
 
-@pytest.mark.parametrize('version', not_str)
+@pytest.mark.parametrize("version", not_str)
 def test_depth_version_type(version):
-    """Raise TypeError if `version` not a str."""
+    """Raise TypeError if `version` is not a str."""
     if version is not None:
         with pytest.raises(TypeError):
-            Dimension('dummy', kernel='depth', radius=0.6, version=version)
+            Dimension("dummy", kernel="depth", radius=0.6, version=version)
+
+
+@pytest.mark.parametrize("radius", not_numeric)
+def test_inverse_radius_type(radius):
+    """Raise TypeError if `radius` is not an int or float."""
+    if radius is not None:
+        with pytest.raises(TypeError):
+            Dimension("dummy", kernel="inverse", radius=radius)
 
 
-@pytest.mark.parametrize('distance', not_str)
+@pytest.mark.parametrize("distance", not_str)
 def test_distance_type(distance):
     """Raise TypeError if `distance` is not a str."""
     if distance is not None:
         with pytest.raises(TypeError):
-            Dimension('dummy', distance=distance)
+            Dimension("dummy", distance=distance)
 
 
-@pytest.mark.parametrize('bad_dict', not_dict)
+@pytest.mark.parametrize("bad_dict", not_dict)
 def test_distance_dict_type(bad_dict):
     """Raise TypeError if `distance_dict` not a dict."""
     if bad_dict is not None:
         with pytest.raises(TypeError):
-            Dimension('dummy', distance='dictionary', distance_dict=bad_dict)
+            Dimension("dummy", distance="dictionary", distance_dict=bad_dict)
 
 
-@pytest.mark.parametrize('key', not_tuple)
-@pytest.mark.parametrize('value', [1, 1.0])
+@pytest.mark.parametrize("key", not_tuple)
+@pytest.mark.parametrize("value", [1, 1.0])
 def test_distance_dict_key_type(key, value):
     """Raise TypeError if `distance_dict` keys are not tuples."""
     with pytest.raises(TypeError):
         bad_dict = {key: value}
-        Dimension('dummy', distance='dictionary', distance_dict=bad_dict)
+        Dimension("dummy", distance="dictionary", distance_dict=bad_dict)
 
 
-@pytest.mark.parametrize('key1', not_numeric)
-@pytest.mark.parametrize('key2', not_numeric)
-@pytest.mark.parametrize('value', [1, 1.0])
+@pytest.mark.parametrize("key1", not_numeric)
+@pytest.mark.parametrize("key2", not_numeric)
+@pytest.mark.parametrize("value", [1, 1.0])
 def test_distance_dict_key_element_type(key1, key2, value):
     """Raise TypeError if `distance_dict` keys contain invalid values."""
     with pytest.raises(TypeError):
         bad_dict = {(key1, key2): value}
-        Dimension('dummy', distance='dictionary', distance_dict=bad_dict)
+        Dimension("dummy", distance="dictionary", distance_dict=bad_dict)
 
 
-@pytest.mark.parametrize('key1', [1, 1.0])
-@pytest.mark.parametrize('key2', [1, 1.0])
-@pytest.mark.parametrize('value', not_numeric)
+@pytest.mark.parametrize("key1", [1, 1.0])
+@pytest.mark.parametrize("key2", [1, 1.0])
+@pytest.mark.parametrize("value", not_numeric)
 def test_distance_dict_value_type(key1, key2, value):
     """Raise TypeError if `distance_dict` values not all int or float."""
     with pytest.raises(TypeError):
         bad_dict = {(key1, key2): value}
-        Dimension('dummy', distance='dictionary', distance_dict=bad_dict)
+        Dimension("dummy", distance="dictionary", distance_dict=bad_dict)
 
 
 # Test constructor values
 def test_coordinates_empty():
     """Raise ValueError if `coordinates` is an empty list."""
     with pytest.raises(ValueError):
-        Dimension('dummy', [])
+        Dimension("dummy", [])
 
 
 def test_coordinates_duplicates():
     """Raise ValueError if duplicates found in `coordinates`."""
     with pytest.raises(ValueError):
-        Dimension('dummy', ['dummy', 'dummy'])
+        Dimension("dummy", ["dummy", "dummy"])
 
 
 def test_coordinates_default():
     """`coordinates` set to [`name`] if not supplied."""
-    dim = Dimension('dummy')
+    dim = Dimension("dummy")
     assert dim.coordinates == [dim.name]
 
 
 def test_kernel_value():
     """Raise ValueError if `kernel` is not valid."""
     with pytest.raises(ValueError):
-        Dimension('dummy', kernel='dummy')
+        Dimension("dummy", kernel="dummy")
 
 
 def test_kernel_default():
     """`kernel` set to 'identity' if not supplied."""
-    dim = Dimension('dummy')
-    assert dim.kernel == 'identity'
+    dim = Dimension("dummy")
+    assert dim.kernel == "identity"
 
 
 def test_exponential_radius_exist():
-    """Raise KeyError if `radius` is not passed."""
+    """Raise AttributeError if `radius` is not passed."""
     with pytest.raises(AttributeError):
-        Dimension('dummy', kernel='exponential')
+        Dimension("dummy", kernel="exponential")
 
 
-@pytest.mark.parametrize('radius', [-1, -1.0, 0, 0.0])
+@pytest.mark.parametrize("radius", [-1, -1.0, 0, 0.0])
 def test_exponential_radius_value(radius):
     """Raise ValueError if `radius` is not valid."""
     with pytest.raises(ValueError):
-        Dimension('dummy', kernel='exponential', radius=radius)
+        Dimension("dummy", kernel="exponential", radius=radius)
 
 
 def test_tricubic_exponent_exist():
-    """Raise KeyError if `exponent` is not passed."""
+    """Raise AttributeError if `exponent` is not passed."""
     with pytest.raises(AttributeError):
-        Dimension('dummy', kernel='tricubic')
+        Dimension("dummy", kernel="tricubic")
 
 
-@pytest.mark.parametrize('exponent', [-1, -1.0, 0, 0.0])
+@pytest.mark.parametrize("exponent", [-1, -1.0, 0, 0.0])
 def test_tricubic_exponent_value(exponent):
     """Raise ValueError if `exponenent` is not valid."""
     with pytest.raises(ValueError):
-        Dimension('dummy', kernel='tricubic', exponent=exponent)
+        Dimension("dummy", kernel="tricubic", exponent=exponent)
 
 
 def test_depth_radius_exist():
-    """Raise KeyError if `radius` is not passed."""
+    """Raise AttributeError if `radius` is not passed."""
     with pytest.raises(AttributeError):
-        Dimension('dummy', kernel='depth')
+        Dimension("dummy", kernel="depth")
 
 
-@pytest.mark.parametrize('radius', [-1.0, 0.0, 0.25, 0.5, 1.0, 2.0])
+@pytest.mark.parametrize("radius", [-1.0, 0.0, 0.25, 0.5, 1.0, 2.0])
 def test_depth_radius_value(radius):
     """Raise ValueError if `radius` is not valid."""
     with pytest.raises(ValueError):
-        Dimension('dummy', kernel='depth', radius=radius)
+        Dimension("dummy", kernel="depth", radius=radius)
 
 
 def test_depth_version_value():
     """Raise ValueError if `version` is not valid."""
     with pytest.raises(ValueError):
-        Dimension('dummy', kernel='depth', radius=0.6, version='dummy')
+        Dimension("dummy", kernel="depth", radius=0.6, version="dummy")
 
 
 def test_depth_version_default():
     """`version` set to 'codem' if not passed."""
-    dim = Dimension('dummy', kernel='depth', radius=0.6)
-    assert dim.version == 'codem'
+    dim = Dimension("dummy", kernel="depth", radius=0.6)
+    assert dim.version == "codem"
+
+
+def test_inverse_radius_exists():
+    """Raise AttributeError if `radius` is not passed."""
+    with pytest.raises(AttributeError):
+        Dimension("dummy", kernel="inverse")
+
+
+@pytest.mark.parametrize("radius", [-1, -1.0, 0, 0.0])
+def test_inverse_radius_value(radius):
+    """Raise ValueError if `radius` not valid."""
+    with pytest.raises(ValueError):
+        Dimension("dummy", kernel="inverse", radius=radius)
 
 
 def test_distance_value():
     """Raise ValueError if `distance` is not valid."""
     with pytest.raises(ValueError):
-        Dimension('dummy', distance='dummy')
+        Dimension("dummy", distance="dummy")
 
 
-@pytest.mark.parametrize('kernel', ['exponential', 'tricubic', 'identity'])
+@pytest.mark.parametrize("kernel", ["exponential", "tricubic", "identity"])
 def test_euclidean_default(kernel):
     """`distance` set to 'euclidean' if not supplied."""
-    dim = Dimension('dummy', kernel=kernel, **kernel_pars)
-    assert dim.distance == 'euclidean'
+    dim = Dimension("dummy", kernel=kernel, **kernel_pars)
+    assert dim.distance == "euclidean"
 
 
 def test_tree_default():
     """`distance` is set to 'tree' if not supplied."""
-    dim = Dimension('dummy', kernel='depth', radius=0.6)
-    assert dim.distance == 'tree'
+    dim = Dimension("dummy", kernel="depth", radius=0.6)
+    assert dim.distance == "tree"
 
 
 def test_dictionary_distance_dict():
     """Raise ValueError if `distance_dict` if not passed."""
     with pytest.raises(ValueError):
-        Dimension('dummy', distance='dictionary')
+        Dimension("dummy", distance="dictionary")
 
 
 def test_dictionary_empty():
     """Raise ValueError if `distance_dict` is an empty dict."""
     with pytest.raises(ValueError):
-        Dimension('dummy', kernel='dictionary', distance_dict={})
+        Dimension("dummy", kernel="dictionary", distance_dict={})
 
 
-@pytest.mark.parametrize('key', [(), (1, ), (1., ), (1, 2, 3), (1., 2., 3.)])
-@pytest.mark.parametrize('value', [1, 1.0])
+@pytest.mark.parametrize("key", [(), (1,), (1.0,), (1, 2, 3), (1.0, 2.0, 3.0)])
+@pytest.mark.parametrize("value", [1, 1.0])
 def test_distance_dict_key_length(key, value):
     """Raise ValueError if `distance_dict` keys not all length 2."""
     with pytest.raises(ValueError):
         bad_dict = {key: value}
-        Dimension('dummy', distance='dictionary', distance_dict=bad_dict)
+        Dimension("dummy", distance="dictionary", distance_dict=bad_dict)
 
 
-@pytest.mark.parametrize('key1', [1, 1.0])
-@pytest.mark.parametrize('key2', [1, 1.0])
-@pytest.mark.parametrize('value', [-1, -1.0])
+@pytest.mark.parametrize("key1", [1, 1.0])
+@pytest.mark.parametrize("key2", [1, 1.0])
+@pytest.mark.parametrize("value", [-1, -1.0])
 def test_distance_dict_value_nonnegative(key1, key2, value):
     """Raise ValueError if `distance_dict` values not all nonnegative."""
     with pytest.raises(ValueError):
         bad_dict = {(key1, key2): value}
-        Dimension('dummy', distance='dictionary', distance_dict=bad_dict)
+        Dimension("dummy", distance="dictionary", distance_dict=bad_dict)
 
 
 # Test setter behavior
 def test_name_immutable():
     """Raise AttributeError if attempt to reset `name`."""
     with pytest.raises(AttributeError):
-        dim = Dimension('dummy')
-        dim.name = 'spam'
+        dim = Dimension("dummy")
+        dim.name = "spam"
 
 
 def test_coordinates_immutable():
     """Raise AttributeError if attempt to reset `coordinates`."""
     with pytest.raises(AttributeError):
-        dim = Dimension('dummy')
-        dim.coordinates = 'spam'
+        dim = Dimension("dummy")
+        dim.coordinates = "spam"
 
 
 def test_kernel_immutable():
     """Raise AttributeError if attempt to reset `kernel`."""
     with pytest.raises(AttributeError):
-        dim = Dimension('dummy')
-        dim.kernel = 'exponential'
+        dim = Dimension("dummy")
+        dim.kernel = "exponential"
 
 
 def test_distance_immutable():
     """Raise AttributeError if attempt to reset `distance`."""
     with pytest.raises(AttributeError):
-        dim = Dimension('dummy')
-        dim.distance = 'tree'
+        dim = Dimension("dummy")
+        dim.distance = "tree"
 
 
 def test_distance_dict_immutable():
     """Raise AttributeError if attempt to reset `distance_dict`."""
     with pytest.raises(AttributeError):
-        dim = Dimension('dummy', distance='dictionary',
-                        distance_dict=distance_dict)
+        dim = Dimension("dummy", distance="dictionary", distance_dict=distance_dict)
         dim.distance_dict = {(2.0, 2.0): 2.0}
 
 
-@pytest.mark.parametrize('radius', not_numeric)
+@pytest.mark.parametrize("radius", not_numeric)
 def test_exponential_reset_radius_type(radius):
     """Raise TypeError if `radius` is not an int or float."""
-    dim = Dimension('dummy', kernel='exponential', radius=0.6)
+    dim = Dimension("dummy", kernel="exponential", radius=0.6)
     if radius is not None:
         with pytest.raises(TypeError):
             dim.radius = radius
 
 
-@pytest.mark.parametrize('exponent', not_numeric)
+@pytest.mark.parametrize("exponent", not_numeric)
 def test_tricubic_reset_exponent_type(exponent):
     """Raise TypeError if `exponent` is not an int or float."""
-    dim = Dimension('dummy', kernel='tricubic', exponent=3)
+    dim = Dimension("dummy", kernel="tricubic", exponent=3)
     if exponent is not None:
         with pytest.raises(TypeError):
             dim.exponent = exponent
 
 
-@pytest.mark.parametrize('radius', not_float)
+@pytest.mark.parametrize("radius", not_float)
 def test_depth_reset_radius_type(radius):
     """Raise TypeError if `radius` is not a float."""
-    dim = Dimension('dummy', kernel='depth', radius=0.6)
+    dim = Dimension("dummy", kernel="depth", radius=0.6)
     if radius is not None:
         with pytest.raises(TypeError):
             dim.radius = radius
 
 
-@pytest.mark.parametrize('version', not_str)
+@pytest.mark.parametrize("version", not_str)
 def test_depth_reset_version_type(version):
     """Raise TypeError if `version` not a str."""
-    dim = Dimension('dummy', kernel='depth', radius=0.6)
+    dim = Dimension("dummy", kernel="depth", radius=0.6)
     if version is not None:
         with pytest.raises(TypeError):
             dim.version = version
 
 
-@pytest.mark.parametrize('radius', [-1, -1.0, 0, 0.0])
+@pytest.mark.parametrize("radius", not_numeric)
+def test_inverse_reset_radius_type(radius):
+    """Raise TypeError if `radius` is not an int or float."""
+    dim = Dimension("dummy", kernel="inverse", radius=0.6)
+    if radius is not None:
+        with pytest.raises(TypeError):
+            dim.radius = radius
+
+
+@pytest.mark.parametrize("radius", [-1, -1.0, 0, 0.0])
 def test_exponential_reset_radius_value(radius):
     """Raise ValueError if `radius` is not valid."""
-    dim = Dimension('dummy', kernel='exponential', radius=0.6)
+    dim = Dimension("dummy", kernel="exponential", radius=0.6)
     with pytest.raises(ValueError):
         dim.radius = radius
 
 
-@pytest.mark.parametrize('exponent', [-1, -1.0, 0, 0.0])
+@pytest.mark.parametrize("exponent", [-1, -1.0, 0, 0.0])
 def test_tricubic_reset_exponent_value(exponent):
     """Raise ValueError if `exponenent` is not valid."""
-    dim = Dimension('dummy', kernel='tricubic', exponent=3)
+    dim = Dimension("dummy", kernel="tricubic", exponent=3)
     with pytest.raises(ValueError):
         dim.exponent = exponent
 
 
-@pytest.mark.parametrize('radius', [-1.0, 0.0, 0.25, 0.5, 1.0, 2.0])
+@pytest.mark.parametrize("radius", [-1.0, 0.0, 0.25, 0.5, 1.0, 2.0])
 def test_depth_reset_radius_value(radius):
     """Raise ValueError if `radius` is not valid."""
-    dim = Dimension('dummy', kernel='depth', radius=0.6)
+    dim = Dimension("dummy", kernel="depth", radius=0.6)
     with pytest.raises(ValueError):
         dim.radius = radius
 
 
 def test_depth_reset_version_value():
     """Raise ValueError if `version` is not valid."""
-    dim = Dimension('dummy', kernel='depth', radius=0.6)
+    dim = Dimension("dummy", kernel="depth", radius=0.6)
+    with pytest.raises(ValueError):
+        dim.version = "dummy"
+
+
+@pytest.mark.parametrize("radius", [-1, -1.0, 0, 0.0])
+def test_inverse_reset_radius_value(radius):
+    """Raise ValueError if `radius` is not valid."""
+    dim = Dimension("dummy", kernel="inverse", radius=0.6)
     with pytest.raises(ValueError):
-        dim.version = 'dummy'
+        dim.radius = radius
```

### Comparing `weighted-average-1.1.2/tests/test_distance.py` & `weighted_average-1.2.0/tests/test_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,34 +17,40 @@
 from weave.distance import euclidean, tree
 
 
 # Hypothesis types
 @composite
 def my_floats(draw):
     """Return float32 rounded to 5 decimals."""
-    my_float = draw(floats(min_value=-1e-5, max_value=1e5, allow_nan=False,
-                           allow_infinity=False, allow_subnormal=False))
+    my_float = draw(
+        floats(
+            min_value=-1e-5,
+            max_value=1e5,
+            allow_nan=False,
+            allow_infinity=False,
+            allow_subnormal=False,
+        )
+    )
     return np.float32(np.around(my_float, decimals=5))
 
 
 @composite
 def my_arrays(draw, n=2):
     """Return n vectors of float32 with matching lengths."""
     m = draw(integers(min_value=1, max_value=5))
-    array_list = [draw(arrays(np.float32, m, elements=my_floats()))
-                  for ii in range(n)]
+    array_list = [draw(arrays(np.float32, m, elements=my_floats())) for ii in range(n)]
     return array_list
 
 
 # Property 1: Output is a real-valued, finite, nonnegative float
 def property_1(distance):
     """Output satisfies property 1."""
     assert np.isreal(distance)
     assert np.isfinite(distance)
-    assert distance >= 0.
+    assert distance >= 0.0
     assert isinstance(distance, np.float32)
 
 
 @settings(deadline=None)
 @given(my_arrays())
 def test_euclidean_type(xy):
     """Euclidean output satisfies property 1."""
@@ -62,18 +68,18 @@
     distance = tree(x, y)
     property_1(distance)
 
 
 # Property 2: Output == 0 iff x == y
 def property_2(x, y, distance):
     """Output satisfies property 2."""
-    if np.isclose(distance, 0.):
+    if np.isclose(distance, 0.0):
         assert np.allclose(x, y, rtol=1e-6)
-    if np.allclose(x, y, rtol=1e0-6):
-        assert np.isclose(distance, 0.)
+    if np.allclose(x, y, rtol=1e0 - 6):
+        assert np.isclose(distance, 0.0)
 
 
 @given(my_arrays())
 def test_euclidean_zero(xy):
     """Euclidean output satisfies property 2."""
     x, y = xy
     distance = euclidean(x, y)
@@ -142,29 +148,29 @@
 
 
 # Test specific output values
 def test_same_country():
     """Test tree output with same country."""
     x = np.array([1, 2, 4])
     y = np.array([1, 2, 4])
-    assert np.isclose(tree(x, y), 0.)
+    assert np.isclose(tree(x, y), 0.0)
 
 
 def test_same_region():
     """Test tree output with same region."""
     x = np.array([1, 2, 4])
     y = np.array([1, 2, 5])
-    assert np.isclose(tree(x, y), 1.)
+    assert np.isclose(tree(x, y), 1.0)
 
 
 def test_same_super_region():
     """Test tree output with same super region."""
     x = np.array([1, 2, 4])
     y = np.array([1, 3, 6])
-    assert np.isclose(tree(x, y), 2.)
+    assert np.isclose(tree(x, y), 2.0)
 
 
 def test_different_super_region():
     """Test tree output with different super regions."""
     x = np.array([1, 2, 4])
     y = np.array([7, 8, 9])
-    assert np.isclose(tree(x, y), 3.)
+    assert np.isclose(tree(x, y), 3.0)
```

### Comparing `weighted-average-1.1.2/tests/test_kernels.py` & `weighted_average-1.2.0/tests/test_kernels.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,54 @@
 
 In general, kernel functions should satisfy the following properties:
 1. k(x, y) is real-valued, finite, and nonnegative
 2. k(x, y) <= k(x', y') if d(x, y) > d(x', y')
    k(x, y) >= k(x', y') if d(x, y) < d(x', y')
 
 """
+
 from hypothesis import given, settings
 from hypothesis.strategies import floats, integers
 import numpy as np
 
-from weave.kernels import exponential, depth, tricubic
+from weave.kernels import exponential, depth, tricubic, inverse
 
 # Hypothesis types
-my_dist = floats(min_value=0.0, max_value=1e3, allow_nan=False,
-                 allow_infinity=False, allow_subnormal=False)
+my_dist = floats(
+    min_value=0.0,
+    max_value=1e3,
+    allow_nan=False,
+    allow_infinity=False,
+    allow_subnormal=False,
+)
 my_level = integers(min_value=1, max_value=10)
-my_radius1 = floats(min_value=1e2, max_value=1e3, allow_nan=False,
-                    allow_infinity=False, allow_subnormal=False)
-my_radius2 = floats(min_value=0.5, max_value=1.0, allow_nan=False,
-                    allow_infinity=False, allow_subnormal=False,
-                    exclude_min=True, exclude_max=True)
-my_exponent = floats(min_value=1e-1, max_value=1e1, allow_nan=False,
-                     allow_infinity=False, allow_subnormal=False)
-my_version = ['codem', 'stgpr']
+my_radius1 = floats(
+    min_value=1e2,
+    max_value=1e3,
+    allow_nan=False,
+    allow_infinity=False,
+    allow_subnormal=False,
+)
+my_radius2 = floats(
+    min_value=0.5,
+    max_value=1.0,
+    allow_nan=False,
+    allow_infinity=False,
+    allow_subnormal=False,
+    exclude_min=True,
+    exclude_max=True,
+)
+my_exponent = floats(
+    min_value=1e-1,
+    max_value=1e1,
+    allow_nan=False,
+    allow_infinity=False,
+    allow_subnormal=False,
+)
+my_version = ["codem", "stgpr"]
 
 
 # Property 1: Output is a real-valued, finite, nonnegative float
 def property_1(weight):
     """Output satisfies property 1."""
     assert np.isreal(weight)
     assert np.isfinite(weight)
@@ -56,14 +78,22 @@
 @given(my_dist, my_radius1, my_exponent)
 def test_tricubic_type(distance, radius, exponent):
     """Tricubic output satisfies property 1."""
     weight = tricubic(distance, radius, exponent)
     property_1(weight)
 
 
+@settings(deadline=None)
+@given(my_dist, my_radius1)
+def test_inverse_type(distance, radius):
+    """Inverse output satisfies property 1."""
+    inverse_term = inverse(distance, radius)
+    property_1(inverse_term)
+
+
 # Property 2: Output decreases as distance increases
 def property_2(distance_a, distance_b, weight_a, weight_b):
     """Output satisfies property 2."""
     if distance_a > distance_b:
         assert weight_a <= weight_b
     if distance_a < distance_b:
         assert weight_a >= weight_b
@@ -90,30 +120,38 @@
 def test_tricubic_direction(distance_a, distance_b, radius, exponent):
     """Tricubic output satisfies property 2."""
     weight_a = tricubic(distance_a, radius, exponent)
     weight_b = tricubic(distance_b, radius, exponent)
     property_2(distance_a, distance_b, weight_a, weight_b)
 
 
+@given(my_dist, my_dist, my_radius1)
+def test_inverse_direction(distance_a, distance_b, radius):
+    """Inverse output satisfies property 2."""
+    weight_a = 1 / (inverse(distance_a, radius) + 0.1)
+    weight_b = 1 / (inverse(distance_b, radius) + 0.1)
+    property_2(distance_a, distance_b, weight_a, weight_b)
+
+
 # Test specific output values
 def test_same_country():
     """Test depth kernel with same country."""
-    assert np.isclose(depth(0, 3, 0.9, 'codem'), 0.9)
-    assert np.isclose(depth(0, 3, 0.9, 'stgpr'), 1)
+    assert np.isclose(depth(0, 3, 0.9, "codem"), 0.9)
+    assert np.isclose(depth(0, 3, 0.9, "stgpr"), 1)
 
 
 def test_same_region():
     """Test depth kernel with same region."""
-    assert np.isclose(depth(1, 3, 0.9, 'codem'), 0.09)
-    assert np.isclose(depth(1, 3, 0.9, 'stgpr'), 0.9)
+    assert np.isclose(depth(1, 3, 0.9, "codem"), 0.09)
+    assert np.isclose(depth(1, 3, 0.9, "stgpr"), 0.9)
 
 
 def test_same_super_region():
     """Test depth kernel with same super region."""
-    assert np.isclose(depth(2, 3, 0.9, 'codem'), 0.01)
-    assert np.isclose(depth(2, 3, 0.9, 'stgpr'), 0.81)
+    assert np.isclose(depth(2, 3, 0.9, "codem"), 0.01)
+    assert np.isclose(depth(2, 3, 0.9, "stgpr"), 0.81)
 
 
 def test_different_super_region():
     """Test depth kernel with different super regions."""
-    assert np.isclose(depth(3, 3, 0.9, 'codem'), 0)
-    assert np.isclose(depth(3, 3, 0.9, 'stgpr'), 0)
+    assert np.isclose(depth(3, 3, 0.9, "codem"), 0)
+    assert np.isclose(depth(3, 3, 0.9, "stgpr"), 0)
```

### Comparing `weighted-average-1.1.2/tests/test_smoother.py` & `weighted_average-1.2.0/tests/test_smoother.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,63 +1,89 @@
 """Tests inputs for smoother function."""
+
 import pytest
 
 import numpy as np
 from pandas import DataFrame
 
 from weave.dimension import Dimension
-from weave.smoother import Smoother, smooth
+from weave.smoother import Smoother, smooth, smooth_inverse
 
 # Lists of wrong types to test exceptions
-value_list = [1, 1.0, 'dummy', True, None, [], (), {}]
+value_list = [1, 1.0, "dummy", True, None, [], (), {}]
 not_str = [1, 1.0, True, None, [], (), {}]
 not_bool = [1, 1.0, None, [], (), {}]
 not_dimensions = value_list + [[value] for value in value_list]
 not_columns = not_str + [[value] for value in not_str]
+not_number = ["dummy", True, None, [], (), {}]
 
 # Example smoother
 age = Dimension(
-    name='age_id',
-    kernel='exponential',
-    radius=1
+    name="age_id",
+    kernel="exponential",
+    radius=1,
 )
 year = Dimension(
-    name='year_id',
-    kernel='tricubic',
-    exponent=0.5
+    name="year_id",
+    kernel="tricubic",
+    exponent=0.5,
 )
 location = Dimension(
-    name='location_id',
-    coordinates=['super_region', 'region', 'country'],
-    kernel='depth',
-    radius=0.9
+    name="location_id",
+    coordinates=["super_region", "region", "country"],
+    kernel="depth",
+    radius=0.9,
 )
 smoother = Smoother([age, year, location])
 
+# Example inverse smoother
+age_inverse = Dimension(
+    name="age_id",
+    kernel="inverse",
+    radius=0.5,
+)
+year_inverse = Dimension(
+    name="year_id",
+    kernel="inverse",
+    radius=0.5,
+)
+location_inverse = Dimension(
+    name="location_id",
+    coordinates=["super_region", "region", "country"],
+    kernel="inverse",
+    radius=0.5,
+)
+smoother_inverse = Smoother([age_inverse, year_inverse, location_inverse])
+
+
 # Example data
-data = DataFrame({
-    'age_id': [1, 2, 3, 4, 4],
-    'age_mean': [0.5, 1.5, 2.5, 3.5, 3.5],
-    'year_id': [1980, 1990, 2000, 2010, 2020],
-    'location_id': [5, 5, 6, 7, 9],
-    'super_region': [1, 1, 1, 1, 2],
-    'region': [3, 3, 3, 4, 8],
-    'country': [5, 5, 6, 7, 9],
-    'fit': [True, False, False, True, True],
-    'predict': [False, True, True, False, False],
-    'count': [1.0, 2.0, 3.0, 4.0, 5.0],
-    'fraction': [0.1, 0.2, 0.3, 0.4, 0.5],
-    'residual': [0.2, 0.4, 0.6, 0.8, 1.0],
-    'residual_sd': [0.01, 0.02, 0.03, 0.04, 0.05],
-    'name': ['a', 'b', 'c', 'd', 'e']
-})
+data = DataFrame(
+    {
+        "age_id": [1, 2, 3, 4, 4],
+        "age_mean": [0.5, 1.5, 2.5, 3.5, 3.5],
+        "year_id": [1980, 1990, 2000, 2010, 2020],
+        "location_id": [5, 5, 6, 7, 9],
+        "super_region": [1, 1, 1, 1, 2],
+        "region": [3, 3, 3, 4, 8],
+        "country": [5, 5, 6, 7, 9],
+        "fit": [True, False, False, True, True],
+        "predict": [False, True, True, False, False],
+        "count": [1.0, 2.0, 3.0, 4.0, 5.0],
+        "fraction": [0.1, 0.2, 0.3, 0.4, 0.5],
+        "residual": [0.2, 0.4, 0.6, 0.8, 1.0],
+        "residual_sd": [0.01, 0.02, 0.03, 0.04, 0.05],
+        "sd_zero": [0.0, 0.02, 0.03, 0.04, 0.05],
+        "sd_negative": [-0.01, 0.02, 0.03, 0.04, 0.05],
+        "name": ["a", "b", "c", "d", "e"],
+    }
+)
 
 
 # Test constructor types
-@pytest.mark.parametrize('dimensions', not_dimensions)
+@pytest.mark.parametrize("dimensions", not_dimensions)
 def test_dimensions_type(dimensions):
     """Raise TypeError if invalid type for `dimensions`."""
     if dimensions != []:
         with pytest.raises(TypeError):
             Smoother(dimensions)
 
 
@@ -67,255 +93,299 @@
     with pytest.raises(ValueError):
         Smoother([])
 
 
 def test_duplicate_dimension_names():
     """Raise ValueError if duplicate names in `dimensions`."""
     with pytest.raises(ValueError):
-        dim1 = Dimension('dummy', 'columns1')
-        dim2 = Dimension('dummy', 'columns2')
+        dim1 = Dimension("dummy", "columns1")
+        dim2 = Dimension("dummy", "columns2")
         Smoother([dim1, dim2])
 
 
-@pytest.mark.parametrize('coords1', ['dummy1', ['dummy1', 'dummy2']])
-@pytest.mark.parametrize('coords2', ['dummy1', ['dummy1', 'dummy2']])
+@pytest.mark.parametrize("coords1", ["dummy1", ["dummy1", "dummy2"]])
+@pytest.mark.parametrize("coords2", ["dummy1", ["dummy1", "dummy2"]])
 def test_duplicate_dimension_coords(coords1, coords2):
     """Raise ValueError if duplicate coordinates in `dimensions`."""
     with pytest.raises(ValueError):
-        dim1 = Dimension('dummy1', coords1)
-        dim2 = Dimension('dummy2', coords2)
+        dim1 = Dimension("dummy1", coords1)
+        dim2 = Dimension("dummy2", coords2)
         Smoother([dim1, dim2])
 
 
 def test_dimension_immutable():
     """Raise AttributeError if attempt to reset `dimensions`."""
     with pytest.raises(AttributeError):
-        dim = Dimension('dummy')
+        dim = Dimension("dummy")
         smoother.dimensions = dim
 
 
+def test_inverse_weights_value():
+    """`inverse_weights` set to correct values."""
+    assert smoother.inverse_weights is False
+    assert smoother_inverse.inverse_weights is True
+
+
+def test_inverse_weights_error():
+    """Raise ValueError if dimensions have inverse and non-inverse kernels."""
+    with pytest.raises(ValueError):
+        Smoother([age, year_inverse])
+
+
+def test_inverse_weights_immutable():
+    """Raise AttributeError if attempt to reset `inverse_weights`."""
+    with pytest.raises(AttributeError):
+        smoother.inverse_weights = False
+
+
 # Test input types
-@pytest.mark.parametrize('bad_data', value_list)
+@pytest.mark.parametrize("bad_data", value_list)
 def test_data_type(bad_data):
     """Raise TypeError if `data` is not a DataFrame."""
     with pytest.raises(TypeError):
-        smoother(bad_data, 'residual')
+        smoother(bad_data, "residual")
 
 
-@pytest.mark.parametrize('observed', not_str)
+@pytest.mark.parametrize("observed", not_str)
 def test_observed_type(observed):
     """Raise TypeError if `observed` is not a str."""
     with pytest.raises(TypeError):
         smoother(data, observed)
 
 
-@pytest.mark.parametrize('stdev', not_str)
+@pytest.mark.parametrize("stdev", not_str)
 def test_stdev_type(stdev):
     """Raise TypeError if `stdev` is not a str."""
     if stdev is not None:
         with pytest.raises(TypeError):
-            smoother(data, 'residual', stdev)
+            smoother(data, "residual", stdev)
 
 
-@pytest.mark.parametrize('smoothed', not_str)
+@pytest.mark.parametrize("smoothed", not_str)
 def test_smoothed_type(smoothed):
     """Raise TypeError if `smoothed` is not a str."""
     if smoothed is not None:
         with pytest.raises(TypeError):
-            smoother(data, 'residual', smoothed=smoothed)
+            smoother(data, "residual", smoothed=smoothed)
 
 
-@pytest.mark.parametrize('fit', not_str)
+@pytest.mark.parametrize("fit", not_str)
 def test_fit_type(fit):
     """Raise TypeError if `fit` is not a str."""
     if fit is not None:
         with pytest.raises(TypeError):
-            smoother(data, 'residual', fit=fit)
+            smoother(data, "residual", fit=fit)
 
 
-@pytest.mark.parametrize('predict', not_str)
+@pytest.mark.parametrize("predict", not_str)
 def test_predict_type(predict):
     """Raise TypeError if `predict` is not a str."""
     if predict is not None:
         with pytest.raises(TypeError):
-            smoother(data, 'residual', predict=predict)
+            smoother(data, "residual", predict=predict)
+
+
+@pytest.mark.parametrize("down_weight", not_number)
+def test_down_weight_type(down_weight):
+    """Raise TypeError if `down_weight` is not an int or float."""
+    with pytest.raises(TypeError):
+        smoother(data, "residual", down_weight=down_weight)
 
 
 # Test input values
 def test_observed_stdev_overlap():
     """Raise ValueError if `observed` == `stdev`."""
     with pytest.raises(ValueError):
-        smoother(data, 'residual', 'residual')
+        smoother(data, "residual", "residual")
 
 
 def test_observed_smoothed_overlap():
     """Raise ValueError if `observed` == `smoothed`."""
     with pytest.raises(ValueError):
-        smoother(data, 'residual', smoothed='residual')
+        smoother(data, "residual", smoothed="residual")
 
 
 def test_stdev_smoothed_overlap():
     """Raise ValueError if `stdev` == `smoothed`."""
     with pytest.raises(ValueError):
-        smoother(data, 'residual', stdev='residual_sd', smoothed='residual_sd')
+        smoother(data, "residual", stdev="residual_sd", smoothed="residual_sd")
+
+
+def test_stdev_passed_with_inverse_weights():
+    """Raise ValueError if `stdev` not passed when `inverse_weights` is True."""
+    with pytest.raises(ValueError):
+        smoother_inverse(data, "residual")
 
 
 def test_smoothed_warning():
     """Trigger UserWarning if `smoothed` already in `data`."""
     with pytest.warns(UserWarning):
-        smoother(data, 'count', smoothed='residual')
+        smoother(data, "count", smoothed="residual")
+
+
+@pytest.mark.parametrize("down_weight", [-1, 2])
+def test_down_weight_value(down_weight):
+    """Raise ValueError if `down_weight` not in [0, 1]."""
+    with pytest.raises(ValueError):
+        smoother(data, "residual", stdev="residual_sd", down_weight=down_weight)
 
 
 # Test data keys
 def test_names_in_data():
     """Raise KeyError if `dimension.name` not in `data`."""
     with pytest.raises(KeyError):
-        dummy = Dimension('dummy', 'age_id')
+        dummy = Dimension("dummy", "age_id")
         smoother2 = Smoother([dummy, year, location])
-        smoother2(data, 'residual')
+        smoother2(data, "residual")
 
 
-@pytest.mark.parametrize('coords', ['dummy', ['age_id', 'dummy']])
+@pytest.mark.parametrize("coords", ["dummy", ["age_id", "dummy"]])
 def test_coordinates_in_data(coords):
     """Raise KeyError if `dimension.coordinates` not in `data`."""
     with pytest.raises(KeyError):
-        dummy = Dimension('age_id', coords)
+        dummy = Dimension("age_id", coords)
         smoother2 = Smoother([dummy, year, location])
-        smoother2(data, 'residual')
+        smoother2(data, "residual")
 
 
 def test_observed_in_data():
     """Raise KeyError if `observed` not in `data`."""
     with pytest.raises(KeyError):
-        smoother(data, 'dummy')
+        smoother(data, "dummy")
 
 
 def test_stdev_in_data():
     """Raise KeyError if `stdev` not in `data`."""
     with pytest.raises(KeyError):
-        smoother(data, 'residual', 'dummy')
+        smoother(data, "residual", "dummy")
 
 
 def test_fit_in_data():
     """Raise KeyError if `fit` not in `data`."""
     with pytest.raises(KeyError):
-        smoother(data, 'residual', fit='dummy')
+        smoother(data, "residual", fit="dummy")
 
 
 def test_predict_in_data():
     """Raise KeyError if `predict` not in `data`."""
     with pytest.raises(KeyError):
-        smoother(data, 'residual', predict='dummy')
+        smoother(data, "residual", predict="dummy")
 
 
 def test_names_in_distance_dict():
     """Raise KeyError if not all `names` in `distance_dict`."""
     with pytest.raises(KeyError):
-        dummy = Dimension('age_id', distance='dictionary',
-                          distance_dict={(1, 1): 0})
+        dummy = Dimension("age_id", distance="dictionary", distance_dict={(1, 1): 0})
         smoother2 = Smoother([dummy, year, location])
-        smoother2(data, 'residual')
+        smoother2(data, "residual")
 
 
 # Test data types
 def test_data_name_type():
     """Raise TypeError if `dimension.name` not int or float."""
     with pytest.raises(TypeError):
-        dummy = Dimension('name', 'age_id')
+        dummy = Dimension("name", "age_id")
         smoother2 = Smoother([dummy, year, location])
-        smoother2(data, 'residual')
+        smoother2(data, "residual")
 
 
-@pytest.mark.parametrize('coords', ['name', ['age_id', 'name']])
+@pytest.mark.parametrize("coords", ["name", ["age_id", "name"]])
 def test_data_coordinates_type(coords):
     """Raise TypeError if `dimension.coordinates` not int or float."""
     with pytest.raises(TypeError):
-        dummy = Dimension('age_id', coords)
+        dummy = Dimension("age_id", coords)
         smoother2 = Smoother([dummy, year, location])
-        smoother2(data, 'residual')
+        smoother2(data, "residual")
 
 
 def test_data_observed_type():
     """Raise TypeError if `observed` not int or float."""
     with pytest.raises(TypeError):
-        smoother(data, 'name')
+        smoother(data, "name")
 
 
 def test_data_stdev_type():
     """Raise TypeError if `stdev` not int or float."""
     with pytest.raises(TypeError):
-        smoother(data, 'residual', 'name')
+        smoother(data, "residual", "name")
 
 
-@pytest.mark.parametrize('fit', ['age_id', 'count', 'name'])
+@pytest.mark.parametrize("fit", ["age_id", "count", "name"])
 def test_data_fit_type(fit):
     """Raise TypeError if `fit` column is not bool."""
     with pytest.raises(TypeError):
-        smoother(data, 'residual', fit=fit)
+        smoother(data, "residual", fit=fit)
 
 
-@pytest.mark.parametrize('predict', ['age_id', 'count', 'name'])
+@pytest.mark.parametrize("predict", ["age_id", "count", "name"])
 def test_data_predict_type(predict):
     """Raise TypeError if `predict` column is not bool."""
     with pytest.raises(TypeError):
-        smoother(data, 'residual', predict=predict)
+        smoother(data, "residual", predict=predict)
 
 
 # Test data values
 def test_data_name2coord():
     """Raise ValueError if `name` maps to multiple `coordinates`."""
     with pytest.raises(ValueError):
         data2 = data.copy()
-        data2.loc[2, 'location_id'] = 5
-        smoother(data2, 'residual')
+        data2.loc[2, "location_id"] = 5
+        smoother(data2, "residual")
 
 
 def test_data_coord2name():
     """Raise ValueError if `coordinates` maps to multiple `name`."""
     with pytest.raises(ValueError):
         data2 = data.copy()
-        data2.loc[2, 'level_3'] = 5
-        smoother(data2, 'residual')
+        data2.loc[2, "level_3"] = 5
+        smoother(data2, "residual")
 
 
 def test_data_nans():
     """Raise ValueError if NaNs in `data`."""
     with pytest.raises(ValueError):
         data2 = data.copy()
-        data2['dummy'] = 5*[np.nan]
-        smoother(data2, 'residual')
+        data2["dummy"] = 5 * [np.nan]
+        smoother(data2, "residual")
 
 
-@pytest.mark.parametrize('value', [-np.inf, np.inf])
+@pytest.mark.parametrize("value", [-np.inf, np.inf])
 def test_data_infs(value):
     """Raise ValueError if Infs in `data`."""
     with pytest.raises(ValueError):
         data2 = data.copy()
-        data2['residual'] = 5*[value]
-        smoother(data2, 'residual')
+        data2["residual"] = 5 * [value]
+        smoother(data2, "residual")
+
+
+@pytest.mark.parametrize("stdev", ["sd_zero", "sd_negative"])
+def test_stdev_values(stdev):
+    """Raise ValueError if `stdev` column contains zeros or negative values."""
+    with pytest.raises(ValueError):
+        smoother(data, "residual", stdev)
 
 
 # Test smoother output
 def test_idx_fit_len():
     """`get_indices` returns array of correct length."""
-    idx_fit = smoother.get_indices(data, 'fit')
-    assert len(idx_fit) == data['fit'].sum()
+    idx_fit = smoother.get_indices(data, "fit")
+    assert len(idx_fit) == data["fit"].sum()
 
 
 def test_idx_predict_len():
     """`get_indices` returns array of correct length."""
-    idx_pred = smoother.get_indices(data, 'predict')
-    assert len(idx_pred) == data['predict'].sum()
+    idx_pred = smoother.get_indices(data, "predict")
+    assert len(idx_pred) == data["predict"].sum()
 
 
-@pytest.mark.parametrize('fit', ['fit', 'predict'])
+@pytest.mark.parametrize("fit", ["fit", "predict"])
 def test_obs_shape(fit):
     """`get_observed` returns array of correct shape."""
     idx_fit = smoother.get_indices(data, fit)
-    cols_obs = smoother.get_values(data, 'residual', idx_fit)
+    cols_obs = smoother.get_values(data, "residual", idx_fit)
     assert cols_obs.shape == (len(idx_fit),)
 
 
 def test_points_shape():
     """`get_points` returns array of correct shape."""
     points = smoother.get_points(data)
     assert points.shape == (len(data), len(smoother.dimensions))
@@ -326,55 +396,93 @@
     dim_list = smoother.get_typed_dimensions(data)
     assert len(dim_list) == len(smoother.dimensions)
     for dimension in dim_list:
         n_ids = len(data[dimension.name].unique())
         assert len(dimension.weight_dict) == n_ids**2
 
 
-@pytest.mark.parametrize('predict', [None, 'fit', 'predict'])
+@pytest.mark.parametrize("predict", [None, "fit", "predict"])
 def test_smooth_shape(predict):
     """`smooth` returns array of correct shape."""
     idx_fit = smoother.get_indices(data, None)
     idx_pred = smoother.get_indices(data, predict)
-    col_obs = smoother.get_values(data, 'residual', idx_fit)
+    col_obs = smoother.get_values(data, "residual", idx_fit)
     col_sd = smoother.get_values(data, None, idx_fit)
     points = smoother.get_points(data)
     dim_list = smoother.get_typed_dimensions(data)
-    cols_smooth = smooth(dim_list, points, col_obs, col_sd, idx_fit, idx_pred)
+    cols_smooth = smooth(dim_list, points, col_obs, col_sd, idx_fit, idx_pred, 1.0)
     if predict is None:
         assert cols_smooth.shape == (len(data),)
     else:
         assert cols_smooth.shape == (data[predict].sum(),)
 
 
-@pytest.mark.parametrize('predict', [None, 'fit', 'predict'])
+@pytest.mark.parametrize("predict", [None, "fit", "predict"])
+def test_smooth_inverse_shape(predict):
+    """`smooth_inverse` returns array of correct shape."""
+    idx_fit = smoother.get_indices(data, None)
+    idx_pred = smoother.get_indices(data, predict)
+    col_obs = smoother.get_values(data, "residual", idx_fit)
+    col_sd = smoother.get_values(data, None, idx_fit)
+    points = smoother.get_points(data)
+    dim_list = smoother.get_typed_dimensions(data)
+    cols_smooth = smooth_inverse(
+        dim_list, points, col_obs, col_sd, idx_fit, idx_pred, 1.0
+    )
+    if predict is None:
+        assert cols_smooth.shape == (len(data),)
+    else:
+        assert cols_smooth.shape == (data[predict].sum(),)
+
+
+@pytest.mark.parametrize("predict", [None, "fit", "predict"])
 def test_smoother_shape(predict):
     """Return data frame with correct shape."""
-    result = smoother(data, 'residual', predict=predict)
+    result = smoother(data, "residual", predict=predict)
     if predict is None:
         assert len(result) == len(data)
     else:
         assert len(result) == data[predict].sum()
     assert len(result.columns) == len(data.columns) + 1
 
 
-@pytest.mark.parametrize('smoothed', [None, 'dummy'])
+@pytest.mark.parametrize("smoothed", [None, "dummy"])
 def test_smoother_columns(smoothed):
     """Return data frame with correct column names."""
-    result = smoother(data, 'residual', smoothed=smoothed)
+    result = smoother(data, "residual", smoothed=smoothed)
     if smoothed is None:
-        assert 'residual_smooth' in result.columns
+        assert "residual_smooth" in result.columns
+    else:
+        assert smoothed in result.columns
+
+
+@pytest.mark.parametrize("smoothed", [None, "dummy"])
+def test_smoother_inverse_columns(smoothed):
+    """Return data frame with correct column names."""
+    result = smoother_inverse(data, "residual", "residual_sd", smoothed=smoothed)
+    if smoothed is None:
+        assert "residual_smooth" in result.columns
     else:
         assert smoothed in result.columns
 
 
 def test_result():
     """Check output values."""
-    result = smoother(data, 'residual')
-    vals = np.array([0.25019485, 0.41681382, 0.5839969, 0.79772836, 1.])
-    assert np.allclose(vals, result['residual_smooth'].values)
-    result = smoother(data, 'residual', 'residual_sd')
-    vals = np.array([0.20730056, 0.38848886, 0.5644261, 0.79567325, 1.])
-    assert np.allclose(vals, result['residual_smooth'].values)
-    result = smoother(data, 'residual', fit='fit')
-    vals = np.array([0.20659341, 0.20659341, 0.26, 0.7934066, 1.])
-    assert np.allclose(vals, result['residual_smooth'].values)
+    result = smoother(data, "residual")
+    vals = np.array([0.25019485, 0.41681382, 0.5839969, 0.79772836, 1.0])
+    assert np.allclose(vals, result["residual_smooth"].values)
+    result = smoother(data, "residual", "residual_sd")
+    vals = np.array([0.20730056, 0.38848886, 0.5644261, 0.79567325, 1.0])
+    assert np.allclose(vals, result["residual_smooth"].values)
+    result = smoother(data, "residual", fit="fit")
+    vals = np.array([0.20659341, 0.20659341, 0.26, 0.7934066, 1.0])
+    assert np.allclose(vals, result["residual_smooth"].values)
+
+
+def test_inverse_result():
+    """Check output values."""
+    result = smoother_inverse(data, "residual", "residual_sd")
+    vals = np.array([0.20000343, 0.40000615, 0.59999865, 0.7999712, 0.99992466])
+    assert np.allclose(vals, result["residual_smooth"].values)
+    result = smoother_inverse(data, "residual", "residual_sd", fit="fit")
+    vals = np.array([0.20000166, 0.4879758, 0.6842466, 0.7999973, 0.9999626])
+    assert np.allclose(vals, result["residual_smooth"].values)
```

### Comparing `weighted-average-1.1.2/tests/test_utils.py` & `weighted_average-1.2.0/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,90 @@
 """Tests for general utility functions."""
+
 from hypothesis import given
 from hypothesis.strategies import integers, floats
 import numpy as np
 import pytest
 
 from weave.utils import as_list, flatten, is_number, is_int, is_float
 
 # Example types
-value_list = [1, 1.0, 'dummy', True, None, (), {}]
-not_int = [1.0, np.nan, np.inf, 'dummy', True, None, [], (), {}]
-not_float = [1, np.nan, np.inf, 'dummy', True, None, (), {}]
-not_number = [np.nan, np.inf, 'dummy', True, None, [], (), {}]
+value_list = [1, 1.0, "dummy", True, None, (), {}]
+not_int = [1.0, np.nan, np.inf, "dummy", True, None, [], (), {}]
+not_float = [1, np.nan, np.inf, "dummy", True, None, (), {}]
+not_number = [np.nan, np.inf, "dummy", True, None, [], (), {}]
 
 # Hypothesis types
 my_integers = integers(min_value=-1e5, max_value=1e5)
-my_floats = floats(min_value=-1e-5, max_value=1e5, allow_nan=False,
-                   allow_infinity=False)
+my_floats = floats(
+    min_value=-1e-5, max_value=1e5, allow_nan=False, allow_infinity=False
+)
 
 
 # Test `as_list()`
-@pytest.mark.parametrize('values', value_list)
+@pytest.mark.parametrize("values", value_list)
 def test_list_single_type(values):
     """Cast `values` as list if not already."""
     assert isinstance(as_list(values), list)
 
 
-@pytest.mark.parametrize('values', value_list)
+@pytest.mark.parametrize("values", value_list)
 def test_list_single_value(values):
     """Returns list of `values`."""
     result = as_list(values)
     assert result[0] == values
 
 
-@pytest.mark.parametrize('values', [[value] for value in value_list])
+@pytest.mark.parametrize("values", [[value] for value in value_list])
 def test_list_multi(values):
     """Return `values` if already a list."""
     assert as_list(values) == values
 
 
 # Test `flatten()`
-@pytest.mark.parametrize('values', value_list)
+@pytest.mark.parametrize("values", value_list)
 def test_flatten_type(values):
     """Raise TypeError if `values` is not a list."""
     with pytest.raises(TypeError):
         flatten(values)
 
 
 def test_flatten_not_flat():
     """Return a flattened list."""
-    values = [['age', 'year'], [['sup_reg', 'reg', 'loc']]]
-    assert flatten(values) == ['age', 'year', 'sup_reg', 'reg', 'loc']
+    values = [["age", "year"], [["sup_reg", "reg", "loc"]]]
+    assert flatten(values) == ["age", "year", "sup_reg", "reg", "loc"]
 
 
 def test_flatten_flat():
     """Return `values` if already flattened."""
-    values = ['age', 'year', 'location']
+    values = ["age", "year", "location"]
     assert flatten(values) == values
 
 
 # Test `is_int()`
 @given(my_integers)
 def test_int_true(value):
     """Return True if `value` is an int."""
     assert is_int(value)
 
 
-@pytest.mark.parametrize('value', not_int)
+@pytest.mark.parametrize("value", not_int)
 def test_int_false(value):
     """Return False if `value` is not an int."""
     assert not is_int(value)
 
 
 # Test `is_float()`
 @given(my_floats)
 def test_float_true(value):
     """Return True if `value` is a float."""
     assert is_float(value)
 
 
-@pytest.mark.parametrize('value', not_float)
+@pytest.mark.parametrize("value", not_float)
 def test_float_false(value):
     """Return False if `value` is not a float."""
     assert not is_float(value)
 
 
 # Test `is_number()`
 @given(my_integers)
@@ -93,11 +95,11 @@
 
 @given(my_floats)
 def test_number_float_true(value):
     """Return True if `value` is a float."""
     assert is_number(value)
 
 
-@pytest.mark.parametrize('value', not_number)
+@pytest.mark.parametrize("value", not_number)
 def test_number_false(value):
     """Return False if `value` is not an int or float."""
     assert not is_number(value)
```

