# Comparing `tmp/hestia-earth-earth-engine-0.4.6.tar.gz` & `tmp/hestia-earth-earth-engine-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hestia-earth-earth-engine-0.4.6.tar", last modified: Thu Dec 14 12:06:22 2023, max compression
+gzip compressed data, was "hestia-earth-earth-engine-0.4.7.tar", last modified: Mon Apr 15 09:49:03 2024, max compression
```

## Comparing `hestia-earth-earth-engine-0.4.6.tar` & `hestia-earth-earth-engine-0.4.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.780851 hestia-earth-earth-engine-0.4.6/
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2004 2023-12-14 12:06:22.779851 hestia-earth-earth-engine-0.4.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.775851 hestia-earth-earth-engine-0.4.6/hestia_earth/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.776851 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/
--rw-rw-rw-   0 root         (0) root         (0)     2583 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2450 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/boundary.py
--rw-rw-rw-   0 root         (0) root         (0)     2376 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/gadm.py
--rw-rw-rw-   0 root         (0) root         (0)     1352 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.777851 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7934 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/gee.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.777851 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/storage/
--rw-rw-rw-   0 root         (0) root         (0)     1017 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/storage/_azure_client.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/storage/_local_client.py
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/storage/_s3_client.py
--rw-rw-rw-   0 root         (0) root         (0)     4760 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/vector.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.778851 hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2004 2023-12-14 12:06:22.000000 hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1046 2023-12-14 12:06:22.000000 hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-14 12:06:22.000000 hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-12-14 12:06:22.000000 hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-12-14 12:06:22.000000 hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-14 12:06:22.780851 hestia-earth-earth-engine-0.4.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.774851 hestia-earth-earth-engine-0.4.6/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-14 12:06:22.779851 hestia-earth-earth-engine-0.4.6/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2197 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/tests/integration/test_boundary.py
--rw-rw-rw-   0 root         (0) root         (0)     2456 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/tests/integration/test_coordinates.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/tests/integration/test_earth_engine.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-12-14 12:06:02.000000 hestia-earth-earth-engine-0.4.6/tests/integration/test_gadm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.229280 hestia-earth-earth-engine-0.4.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-15 09:49:03.229280 hestia-earth-earth-engine-0.4.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.224280 hestia-earth-earth-engine-0.4.7/hestia_earth/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.225280 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2450 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/gadm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.226280 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8444 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/gee.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.227280 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       96 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/storage/_azure_client.py
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/storage/_local_client.py
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/storage/_s3_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     4760 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/vector.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.228280 hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-04-15 09:49:03.000000 hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1046 2024-04-15 09:49:03.000000 hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 09:49:03.000000 hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-15 09:49:03.000000 hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-15 09:49:03.000000 hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 09:49:03.229280 hestia-earth-earth-engine-0.4.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.223280 hestia-earth-earth-engine-0.4.7/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 09:49:03.229280 hestia-earth-earth-engine-0.4.7/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/tests/integration/test_boundary.py
+-rw-rw-rw-   0 root         (0) root         (0)     2456 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/tests/integration/test_coordinates.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/tests/integration/test_earth_engine.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2024-04-15 09:48:46.000000 hestia-earth-earth-engine-0.4.7/tests/integration/test_gadm.py
```

### Comparing `hestia-earth-earth-engine-0.4.6/LICENSE` & `hestia-earth-earth-engine-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/PKG-INFO` & `hestia-earth-earth-engine-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-earth-engine
-Version: 0.4.6
+Version: 0.4.7
 Summary: Hestia's earth engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-earth-engine
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-earth-engine-0.4.6/README.md` & `hestia-earth-earth-engine-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/__init__.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/boundary.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/boundary.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/coordinates.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/coordinates.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/gadm.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/gadm.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/log.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/log.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/__init__.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/gee.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/gee.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,47 +88,61 @@
     return ee.Algorithms.If(
         image.size().eq(0),
         ee.Image().unmask(MISSING_DATA_VALUE),
         image.reduce(reducer_func())
     )
 
 
-def _filter_image_by_years(
-    image: ee.ImageCollection, start_date: str, end_date: str, reducer_annual: str, reducer_period: str
-):
-    start_year = _date_year(start_date)
-    end_year = _date_year(end_date)
+def _filter_image_by_dates(image: ee.Image, dates: list, reducer_annual: str, reducer_period: str = 'mean'):
+    # reducer applied for each tuple of dates
     reducer_annual_func = getattr(ee.Reducer, reducer_annual)
     collections = [
-        _filter_or_empty(image.filterDate(f"{year}-01-01", f"{year}-12-31"), reducer_annual_func)
-        for year in range(start_year, end_year + 1)
+        _filter_or_empty(image.filterDate(start_date, end_date), reducer_annual_func) for start_date, end_date in dates
     ]
+
+    # reducer applied for each collections
     reducer_period_func = getattr(ee.Reducer, reducer_period)
     return ee.ImageCollection(collections).reduce(reducer_period_func())
 
 
+def _filter_image_by_years(
+    image: ee.ImageCollection, start_date: str, end_date: str, reducer_annual: str, reducer_period: str
+):
+    start_year = _date_year(start_date)
+    end_year = _date_year(end_date)
+    dates = [(f"{year}-01-01", f"{year}-12-31") for year in range(start_year, end_year + 1)]
+    return _filter_image_by_dates(image, dates, reducer_annual, reducer_period)
+
+
 def _filter_image_by_year(image: ee.Image, year: str, reducer_annual: str):
-    return _filter_image_by_years(image, f"{year}-01-01", f"{year}-12-31", reducer_annual, 'mean')
+    return _filter_image_by_dates(image, [(f"{year}-01-01", f"{year}-12-31")], reducer_annual)
 
 
 def _image_from_collection(data: dict):
     collection = get_required_param(data, 'collection')
     band_name = get_param(data, 'band_name')
     image = ee.ImageCollection(collection).select(band_name) if band_name else ee.Image(collection)
 
+    reducer_annual = get_param(data, 'reducer_annual', 'sum')
+
+    reducer_period = get_param(data, 'reducer_period')
     year = get_param(data, 'year')
     start_date = get_param(data, 'start_date')
     end_date = get_param(data, 'end_date')
-    reducer_annual = get_param(data, 'reducer_annual', 'sum')
-    reducer_period = get_param(data, 'reducer_period', 'mean')
 
-    return _filter_image_by_year(image, year, reducer_annual) if year else (
-        _filter_image_by_years(image, start_date, end_date, reducer_annual, reducer_period) if start_date and end_date
-        else image
-    )
+    return _filter_image_by_years(image, start_date, end_date, reducer_annual, reducer_period) if all([
+        start_date,
+        end_date,
+        reducer_period
+    ]) else _filter_image_by_year(image, year, reducer_annual) if all([
+        year
+    ]) else _filter_image_by_dates(image, [(start_date, end_date)], reducer_annual) if all([
+        start_date,
+        end_date
+    ]) else image
 
 
 def bands_from_collections(collections: list, unmask: bool = False):
     """
     Get the list of bands to query from the collections.
     Note: when querying for coordinates, if one of the bands has no data, the result will be empty.
     """
```

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/storage/__init__.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth/earth_engine/utils/vector.py` & `hestia-earth-earth-engine-0.4.7/hestia_earth/earth_engine/utils/vector.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/PKG-INFO` & `hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hestia-earth-earth-engine
-Version: 0.4.6
+Version: 0.4.7
 Summary: Hestia's earth engine.
 Home-page: https://gitlab.com/hestia-earth/hestia-earth-engine
 Author: Hestia Team
 Author-email: guillaume@hestia.earth
 License: GPL
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hestia-earth-earth-engine-0.4.6/hestia_earth_earth_engine.egg-info/SOURCES.txt` & `hestia-earth-earth-engine-0.4.7/hestia_earth_earth_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/setup.py` & `hestia-earth-earth-engine-0.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/tests/integration/test_boundary.py` & `hestia-earth-earth-engine-0.4.7/tests/integration/test_gadm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import os
 import json
 from tests.utils import fixtures_path
-from hestia_earth.earth_engine.boundary import run, get_size_km2
+from hestia_earth.earth_engine.gadm import run, get_size_km2
 
-fixtures_folder = os.path.join(fixtures_path, 'boundary')
+fixtures_folder = os.path.join(fixtures_path, 'gadm')
 
 
 def test_run_raster():
     with open(os.path.join(fixtures_folder, 'raster.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
-    assert [r if r is None else round(r, 2) for r in results] == [44.02, 0.77, 0.92, 285.72, 284.05]
+    assert [r if r is None else round(r, 2) for r in results] == [78, 0.13, 0.23, 294.18, 293.5]
 
 
 def test_run_raster_missing_data():
     with open(os.path.join(fixtures_folder, 'raster-missing-data.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
-    assert [r if r is None else round(r, 2) for r in results] == [15, 1.59, 31, 5, None, 0.29]
+    assert [r if r is None else round(r, 2) for r in results] == [4, 0.32, 84, 5.1, 0.43, 0.3]
 
 
 def test_run_raster_multiple():
     with open(os.path.join(fixtures_folder, 'raster-multiple.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
-    assert [r if r is None else round(r) for r in results] == [44, 1, 1, 43, 1, 1]
+    assert [r if r is None else round(r) for r in results] == [53, 3, 3, 42, 9, 1]
 
 
 def test_run_vector():
-    expected = '5180'
+    expected = '10435'
 
     os.environ['HEE_USE_GEOPANDAS'] = 'true'
     with open(os.path.join(fixtures_folder, 'vector.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
     assert results[0] == expected
@@ -45,15 +45,15 @@
         data = json.load(f)
 
     results = run(data)
     assert results[0] == expected
 
 
 def test_run_vector_multiple():
-    expected = ['5180', 'PA0445', '5180', 'PA0402']
+    expected = ['4647', 'PA0409', '5592', 'PA0445']
 
     os.environ['HEE_USE_GEOPANDAS'] = 'true'
     with open(os.path.join(fixtures_folder, 'vector-multiple.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     values = run(data)
     assert values == expected
@@ -63,11 +63,8 @@
         data = json.load(f)
 
     values = run(data)
     assert values == expected
 
 
 def test_get_size_km2():
-    with open(os.path.join(fixtures_folder, 'boundary.json'), encoding='utf-8') as f:
-        data = json.load(f)
-
-    assert round(get_size_km2(data)) == 5284
+    assert round(get_size_km2('GADM-AUS.8.14_1')) == 78
```

### Comparing `hestia-earth-earth-engine-0.4.6/tests/integration/test_coordinates.py` & `hestia-earth-earth-engine-0.4.7/tests/integration/test_coordinates.py`

 * *Files identical despite different names*

### Comparing `hestia-earth-earth-engine-0.4.6/tests/integration/test_gadm.py` & `hestia-earth-earth-engine-0.4.7/tests/integration/test_boundary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 import os
 import json
 from tests.utils import fixtures_path
-from hestia_earth.earth_engine.gadm import run, get_size_km2
+from hestia_earth.earth_engine.boundary import run, get_size_km2
 
-fixtures_folder = os.path.join(fixtures_path, 'gadm')
+fixtures_folder = os.path.join(fixtures_path, 'boundary')
 
 
 def test_run_raster():
     with open(os.path.join(fixtures_folder, 'raster.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
-    assert [r if r is None else round(r, 2) for r in results] == [78, 0.13, 0.23, 294.18, 293.5]
+    assert [r if r is None else round(r, 2) for r in results] == [
+        44.02, 0.77, 0.08, 0.06, 0.04, 0.06, 0.08, 0.09, 0.04, 0.03, 0.05, 0.11, 0.07, 0.06, 0.92, 285.72, 284.05
+    ]
 
 
 def test_run_raster_missing_data():
     with open(os.path.join(fixtures_folder, 'raster-missing-data.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
-    assert [r if r is None else round(r, 2) for r in results] == [4, 0.32, 84, 5.1, 0.43, 0.3]
+    assert [r if r is None else round(r, 2) for r in results] == [15, 1.59, 31, 5, None, 0.29]
 
 
 def test_run_raster_multiple():
     with open(os.path.join(fixtures_folder, 'raster-multiple.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
-    assert [r if r is None else round(r) for r in results] == [53, 3, 3, 42, 9, 1]
+    assert [r if r is None else round(r) for r in results] == [44, 1, 1, 43, 1, 1]
 
 
 def test_run_vector():
-    expected = '10435'
+    expected = '5180'
 
     os.environ['HEE_USE_GEOPANDAS'] = 'true'
     with open(os.path.join(fixtures_folder, 'vector.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     results = run(data)
     assert results[0] == expected
@@ -45,15 +47,15 @@
         data = json.load(f)
 
     results = run(data)
     assert results[0] == expected
 
 
 def test_run_vector_multiple():
-    expected = ['4647', 'PA0409', '5592', 'PA0445']
+    expected = ['5180', 'PA0445', '5180', 'PA0402']
 
     os.environ['HEE_USE_GEOPANDAS'] = 'true'
     with open(os.path.join(fixtures_folder, 'vector-multiple.json'), encoding='utf-8') as f:
         data = json.load(f)
 
     values = run(data)
     assert values == expected
@@ -63,8 +65,11 @@
         data = json.load(f)
 
     values = run(data)
     assert values == expected
 
 
 def test_get_size_km2():
-    assert round(get_size_km2('GADM-AUS.8.14_1')) == 78
+    with open(os.path.join(fixtures_folder, 'boundary.json'), encoding='utf-8') as f:
+        data = json.load(f)
+
+    assert round(get_size_km2(data)) == 5284
```

