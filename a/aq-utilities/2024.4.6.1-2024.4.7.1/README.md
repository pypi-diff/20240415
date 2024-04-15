# Comparing `tmp/aq_utilities-2024.4.6.1.tar.gz` & `tmp/aq_utilities-2024.4.7.1.tar.gz`

## Comparing `aq_utilities-2024.4.6.1.tar` & `aq_utilities-2024.4.7.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/requirements.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/config/__init__.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/config/data.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/__init__.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/psql.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/remote.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/test_psql.py
--rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/test_remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/daily_stations/__init__.py
--rw-r--r--   0        0        0     4780 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/daily_stations/psql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/failures/__init__.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/failures/psql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/hourly_data/__init__.py
--rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/hourly_data/psql.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/processing/__init__.py
--rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/processing/filter_stations.py
--rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/processing/reindex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/stations_info/__init__.py
--rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/data/stations_info/psql.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/engine/__init__.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/engine/psql.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/aq_utilities/engine/test_psql.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/LICENSE.md
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/README.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/pyproject.toml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aq_utilities-2024.4.6.1/PKG-INFO
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/requirements.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/config/__init__.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/config/data.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/__init__.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/psql.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/remote.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/test_psql.py
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/test_remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/daily_stations/__init__.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/daily_stations/psql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/failures/__init__.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/failures/psql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/hourly_data/__init__.py
+-rw-r--r--   0        0        0     9706 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/hourly_data/psql.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/processing/__init__.py
+-rw-r--r--   0        0        0     4756 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/processing/filter_stations.py
+-rw-r--r--   0        0        0    10950 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/processing/reindex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/stations_info/__init__.py
+-rw-r--r--   0        0        0     5329 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/data/stations_info/psql.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/engine/__init__.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/engine/psql.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/aq_utilities/engine/test_psql.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/LICENSE.md
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/README.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/pyproject.toml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 aq_utilities-2024.4.7.1/PKG-INFO
```

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/__init__.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/__init__.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/remote.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/remote.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/test_psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/test_psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/test_remote.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/test_remote.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/daily_stations/psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/daily_stations/psql.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,25 +18,27 @@
                                chunksize: int = CHUNCKSIZE,
                                verbose: bool = False) -> int:
     """Load daily stations data to postgres database."""
     # get timestamp from the directory name
     timestamp_component = Path(daily_stations_fp).parent.stem
     if verbose:
         print(f"[{datetime.now()}] loading {daily_stations_fp} to postgres")
-    if verbose: print(f"[{datetime.now()}] file timestamp is {timestamp}")
+        print(f"[{datetime.now()}] file timestamp is {timestamp_component}")
     if timestamp_component == "today":
         timestamp = datetime.utcnow()
         timestamp = timestamp.replace(hour=0, minute=0, second=0,
                                       microsecond=0)
     elif timestamp_component == "yesterday":
         timestamp = datetime.utcnow() - timedelta(days=1)
         timestamp = timestamp.replace(hour=0, minute=0, second=0,
                                       microsecond=0)
     else:
         timestamp = datetime.strptime(timestamp_component, "%Y%m%d")
+    if verbose:
+        print(f"[{datetime.now()}] file timestamp is {timestamp_component}")
     try:
         names = download_file(fp=daily_stations_fp, timestamp=timestamp)
         if verbose: print(f"[{datetime.now()}] downloaded {daily_stations_fp}")
         local_fp, blob_name = names
         df = df = pd.read_csv(local_fp, sep="|", encoding="latin-1",
                               header=None)
         if verbose: print(f"[{datetime.now()}] read {local_fp}")
```

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/failures/psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/failures/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/hourly_data/psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/hourly_data/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/processing/filter_stations.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/processing/filter_stations.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/processing/reindex.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/processing/reindex.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/data/stations_info/psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/data/stations_info/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/engine/psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/engine/psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/aq_utilities/engine/test_psql.py` & `aq_utilities-2024.4.7.1/aq_utilities/engine/test_psql.py`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/.gitignore` & `aq_utilities-2024.4.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/LICENSE.md` & `aq_utilities-2024.4.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aq_utilities-2024.4.6.1/pyproject.toml` & `aq_utilities-2024.4.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="aq-utilities"
-version="2024.04.06.1"
+version="2024.04.07.1"
 authors=[
     {name="Chris Jellen", email="cdjellen@gmail.com"},
 ]
 description="Data utilities for air quality data."
 readme="README.md"
 requires-python=">=3.9"
 keywords=[
```

### Comparing `aq_utilities-2024.4.6.1/PKG-INFO` & `aq_utilities-2024.4.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aq-utilities
-Version: 2024.4.6.1
+Version: 2024.4.7.1
 Summary: Data utilities for air quality data.
 Project-URL: homepage, https://github.com/cdjellen/aq
 Project-URL: documentation, https://github.com/cdjellen/aq
 Author-email: Chris Jellen <cdjellen@gmail.com>
 License-File: LICENSE.md
 Keywords: earth-systems,geometric-deep-learning,graph-neural-networks
 Classifier: License :: OSI Approved :: MIT License
```

