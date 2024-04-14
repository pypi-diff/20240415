# Comparing `tmp/nzshm_common-0.6.1.tar.gz` & `tmp/nzshm_common-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nzshm_common-0.6.1.tar", max compression
+gzip compressed data, was "nzshm_common-0.7.0.tar", max compression
```

## Comparing `nzshm_common-0.6.1.tar` & `nzshm_common-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    34523 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/LICENSE
--rw-r--r--   0        0        0     1109 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/README.md
--rw-r--r--   0        0        0      111 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/__init__.py
--rw-r--r--   0        0        0     1457 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/geometry/geometry.py
--rw-r--r--   0        0        0       47 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/__init__.py
--rw-r--r--   0        0        0      477 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/io.py
--rw-r--r--   0        0        0     2831 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/nz_0_1_nb_1_v0.py
--rw-r--r--   0        0        0     3524 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/nz_0_1_nb_1_v1.py
--rw-r--r--   0        0        0    47971 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/nz_0_2_nb_1_1.py
--rw-r--r--   0        0        0     1511 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/region_grid.py
--rw-r--r--   0        0        0    38248 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/wlg_0_01_nb_1_1.py
--rw-r--r--   0        0        0     3260 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/grids/wlg_0_05_nb_1_1.py
--rw-r--r--   0        0        0       41 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/location/__init__.py
--rw-r--r--   0        0        0     1411 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/location/code_location.py
--rw-r--r--   0        0        0     1631 2024-01-09 21:31:45.461123 nzshm_common-0.6.1/nzshm_common/location/location.py
--rw-r--r--   0        0        0  3218277 2024-01-09 21:31:45.469123 nzshm_common-0.6.1/nzshm_common/location/locations.json
--rw-r--r--   0        0        0      252 2024-01-09 21:31:45.469123 nzshm_common-0.6.1/nzshm_common/location/nz_ids.json
--rw-r--r--   0        0        0       75 2024-01-09 21:31:45.469123 nzshm_common-0.6.1/nzshm_common/util/__init__.py
--rw-r--r--   0        0        0     1440 2024-01-09 21:31:45.469123 nzshm_common-0.6.1/nzshm_common/util/compression.py
--rw-r--r--   0        0        0     2046 2024-01-09 21:31:45.469123 nzshm_common-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     1907 2024-01-09 21:31:45.473123 nzshm_common-0.6.1/tests/test_backarc.py
--rw-r--r--   0        0        0     3565 2024-01-09 21:31:45.473123 nzshm_common-0.6.1/tests/test_coded_location.py
--rw-r--r--   0        0        0     2317 2024-01-09 21:31:45.473123 nzshm_common-0.6.1/tests/test_compression.py
--rw-r--r--   0        0        0     3760 2024-01-09 21:31:45.473123 nzshm_common-0.6.1/tests/test_geometry.py
--rw-r--r--   0        0        0     1662 2024-01-09 21:31:45.473123 nzshm_common-0.6.1/tests/test_location.py
--rw-r--r--   0        0        0     1018 2024-01-09 21:31:45.473123 nzshm_common-0.6.1/tests/test_region_grid.py
--rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 nzshm_common-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-14 22:31:26.946921 nzshm_common-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1109 2024-04-14 22:31:26.946921 nzshm_common-0.7.0/README.md
+-rw-r--r--   0        0        0      111 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/__init__.py
+-rw-r--r--   0        0        0     1457 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/geometry/geometry.py
+-rw-r--r--   0        0        0       47 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/__init__.py
+-rw-r--r--   0        0        0      477 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/io.py
+-rw-r--r--   0        0        0     2831 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/nz_0_1_nb_1_v0.py
+-rw-r--r--   0        0        0     3524 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/nz_0_1_nb_1_v1.py
+-rw-r--r--   0        0        0    47971 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/nz_0_2_nb_1_1.py
+-rw-r--r--   0        0        0     1551 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/region_grid.py
+-rw-r--r--   0        0        0    38248 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/wlg_0_01_nb_1_1.py
+-rw-r--r--   0        0        0     3260 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/grids/wlg_0_05_nb_1_1.py
+-rw-r--r--   0        0        0       41 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/location/__init__.py
+-rw-r--r--   0        0        0     1825 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/location/code_location.py
+-rw-r--r--   0        0        0     5184 2024-04-14 22:31:26.950921 nzshm_common-0.7.0/nzshm_common/location/location.py
+-rw-r--r--   0        0        0  3218277 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/nzshm_common/location/locations.json
+-rw-r--r--   0        0        0      252 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/nzshm_common/location/nz_ids.json
+-rw-r--r--   0        0        0       75 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/nzshm_common/util/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/nzshm_common/util/compression.py
+-rw-r--r--   0        0        0     2475 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/fixtures/location_file.csv
+-rw-r--r--   0        0        0     1907 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_backarc.py
+-rw-r--r--   0        0        0     4190 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_coded_location.py
+-rw-r--r--   0        0        0     2317 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_compression.py
+-rw-r--r--   0        0        0     3760 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_geometry.py
+-rw-r--r--   0        0        0      941 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_get_locations.py
+-rw-r--r--   0        0        0     1662 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_location.py
+-rw-r--r--   0        0        0     1018 2024-04-14 22:31:26.958921 nzshm_common-0.7.0/tests/test_region_grid.py
+-rw-r--r--   0        0        0     2158 1970-01-01 00:00:00.000000 nzshm_common-0.7.0/PKG-INFO
```

### Comparing `nzshm_common-0.6.1/LICENSE` & `nzshm_common-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/README.md` & `nzshm_common-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/geometry/geometry.py` & `nzshm_common-0.7.0/nzshm_common/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/grids/nz_0_1_nb_1_v0.py` & `nzshm_common-0.7.0/nzshm_common/grids/nz_0_1_nb_1_v0.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/grids/nz_0_1_nb_1_v1.py` & `nzshm_common-0.7.0/nzshm_common/grids/nz_0_1_nb_1_v1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/grids/nz_0_2_nb_1_1.py` & `nzshm_common-0.7.0/nzshm_common/grids/nz_0_2_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/grids/region_grid.py` & `nzshm_common-0.7.0/nzshm_common/grids/region_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import namedtuple
 from enum import Enum
+from typing import Tuple
 
 from nzshm_common.grids.nz_0_1_nb_1_v0 import NZ01nb1v0
 from nzshm_common.grids.nz_0_1_nb_1_v1 import NZ01nb1v1
 from nzshm_common.grids.nz_0_2_nb_1_1 import NZ_0_2_nb_1_1
 from nzshm_common.grids.wlg_0_01_nb_1_1 import WLG_0_01_nb_1_1
 from nzshm_common.grids.wlg_0_05_nb_1_1 import WLG_0_05_nb_1_1
 
@@ -36,9 +37,9 @@
         self.neighbours = neighbours
         self.grid = grid
 
     def load(self):
         return self.grid.load()
 
 
-def load_grid(gri_name: str) -> list:
+def load_grid(gri_name: str) -> Tuple[float, float]:
     return RegionGrid[gri_name].load()
```

### Comparing `nzshm_common-0.6.1/nzshm_common/grids/wlg_0_01_nb_1_1.py` & `nzshm_common-0.7.0/nzshm_common/grids/wlg_0_01_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/grids/wlg_0_05_nb_1_1.py` & `nzshm_common-0.7.0/nzshm_common/grids/wlg_0_05_nb_1_1.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/location/code_location.py` & `nzshm_common-0.7.0/nzshm_common/location/code_location.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,31 +9,42 @@
     ref https://stackoverflow.com/a/28750072 for  the techniques used here to calculate decimal places.
     """
 
     lat: float = field(hash=True)
     lon: float = field(hash=True)
     resolution: float = field(hash=True)
 
-    def __init__(self, lat, lon, resolution):
-        assert 0 < resolution < 180
+    def __init__(self, lat: float, lon: float, resolution: float) -> None:
+        """
+        Create a CodedLocation instance.
+
+        Arguments:
+            lat: latitude
+            lon: longitude
+            resolution: the resolution used to resolve the location
+        """
+        assert 0 < resolution < 180, "Resolution must be between 0 and 180 degrees."
 
         self.grid_res = decimal.Decimal(str(resolution).rstrip("0"))
-        self.display_places = max(abs(self.grid_res.as_tuple().exponent), 1)
+        self.display_places = max(abs(self.grid_res.as_tuple().exponent), 1)  # type: ignore
 
         div_res = 1 / float(self.grid_res)
-        places = abs(decimal.Decimal(div_res).as_tuple().exponent)
+        places = abs(decimal.Decimal(div_res).as_tuple().exponent)  # type: ignore
 
         self.lon = round(lon * div_res, places) / div_res
         self.lat = round(lat * div_res, places) / div_res
         self.resolution = resolution
 
         self._code = f"{self.lat:.{self.display_places}f}~{self.lon:.{self.display_places}f}"
 
     @property
     def code(self) -> str:
+        """
+        The string code for the location expressed as latitude~longitude.
+        """
         return self._code
 
     def resample(self, resolution: float) -> "CodedLocation":
         """Downsample/Resample."""
         return self.downsample(resolution)
 
     def downsample(self, resolution: float) -> "CodedLocation":
```

### Comparing `nzshm_common-0.6.1/nzshm_common/location/locations.json` & `nzshm_common-0.7.0/nzshm_common/location/locations.json`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/nzshm_common/util/compression.py` & `nzshm_common-0.7.0/nzshm_common/util/compression.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/pyproject.toml` & `nzshm_common-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nzshm-common"
-version = "0.6.1"
+version = "0.7.0"
 homepage = "https://github.com/GNS-Science/nzshm-common-py"
 description = "A small pure python library for shared NZ NSHM data like locations."
 authors = ["GNS Science <chrisbc@artisan.co.nz>"]
 readme = "README.md"
 license = "GNU Affero V3"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -37,26 +37,44 @@
     "flake8",
     "flake8-docstrings",
     "pytest-cov"
     ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml", "bump2version"]
 
+doc = [
+    "mkdocs",
+    "mkdocs-include-markdown-plugin",
+    "mkdocs-material",
+    "mkdocstrings",
+    "mkdocs-material-extension",
+    "mkdocs-autorefs"
+    ]
+
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 isort = "^5.10.1"
 flake8  = { version = "^3.9.2"}
 flake8-docstrings = { version = "^1.6.0", optional = true }
-mypy = {version = "^0.900"}
 pytest-cov  = { version = "^2.12.0"}
 tox = "^4.2.8"
 virtualenv  = { version = "^20.2.2", optional = true}
 pip  = { version = "^20.3.1", optional = true}
 bump2version = "^1.0.1"
+mypy = "^1.9.0"
+mkdocs = "^1.5.3"
+mkdocs-autorefs = "^1.0.1"
+mkdocs-include-markdown-plugin = "^6.0.4"
+mkdocs-material = "^9.5.14"
+mkdocs-material-extensions = "^1.3.1"
+mkdocs-pymdownx-material-extras = "^2.5.6"
+mkdocstrings = "^0.24.1"
+mkdocstrings-python = "^1.9.0"
+mkdocs-click = "^0.8.1"
 
 
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
 target-version = ['py310', 'py39']
```

### Comparing `nzshm_common-0.6.1/tests/test_backarc.py` & `nzshm_common-0.7.0/tests/test_backarc.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/tests/test_coded_location.py` & `nzshm_common-0.7.0/tests/test_coded_location.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from contextlib import contextmanager
 import pytest
 import unittest
 
 from nzshm_common.location import CodedLocation
 from nzshm_common.grids.region_grid import load_grid
 import random
 
 GRID_02 = load_grid('NZ_0_2_NB_1_1')
-LOCS = [CodedLocation(loc[0], loc[1], 0.001) for loc in GRID_02[20:50]]
+LOCS = [CodedLocation(loc[0], loc[1], 0.001) for loc in GRID_02[20:50]]  # type: ignore
 
 
 def test_coded_location_is_hashable():
     c = CodedLocation(-45.2, 175.2, 0.1)
     s = set()
     s.add(c)
     assert c in s
@@ -106,7 +107,29 @@
         (-45.27, 171.03, '-45.25~171.05'),
         (-41.333, 174.78, '-41.35~174.80'),  # WLG
     ],
 )
 def test_downsample_oh_point_oh_five(lat, lon, expected):
     c = CodedLocation(lat, lon, 0.05)
     assert c.downsample(0.05).code == expected
+
+
+@contextmanager
+def does_not_raise():
+    yield
+
+
+@pytest.mark.parametrize(
+    "resolution, expectation",
+    [
+        (-0.1, pytest.raises(AssertionError)),
+        (0.0, pytest.raises(AssertionError)),
+        (0.05, does_not_raise()),
+        (0.1, does_not_raise()),
+        (150, does_not_raise()),
+        (180, pytest.raises(AssertionError)),
+    ],
+)
+def test_resolution_bounds(resolution, expectation):
+    """Ensure invalid resolutions throw an assertion error before calculating."""
+    with expectation:
+        CodedLocation(-41.333, 174.78, resolution)
```

### Comparing `nzshm_common-0.6.1/tests/test_compression.py` & `nzshm_common-0.7.0/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/tests/test_geometry.py` & `nzshm_common-0.7.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/tests/test_location.py` & `nzshm_common-0.7.0/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/tests/test_region_grid.py` & `nzshm_common-0.7.0/tests/test_region_grid.py`

 * *Files identical despite different names*

### Comparing `nzshm_common-0.6.1/PKG-INFO` & `nzshm_common-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nzshm-common
-Version: 0.6.1
+Version: 0.7.0
 Summary: A small pure python library for shared NZ NSHM data like locations.
 Home-page: https://github.com/GNS-Science/nzshm-common-py
 License: GNU Affero V3
 Author: GNS Science
 Author-email: chrisbc@artisan.co.nz
 Requires-Python: >=3.8,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
+Provides-Extra: doc
 Provides-Extra: geometry
 Provides-Extra: test
 Requires-Dist: shapely (>=2.0.2,<3.0.0) ; extra == "geometry"
 Description-Content-Type: text/markdown
 
 # nzshm-common
```

