# Comparing `tmp/holcstore-0.1.6.tar.gz` & `tmp/holcstore-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "holcstore-0.1.6.tar", last modified: Thu Apr  4 07:06:00 2024, max compression
+gzip compressed data, was "holcstore-0.1.7.tar", last modified: Mon Apr 15 08:53:31 2024, max compression
```

## Comparing `holcstore-0.1.6.tar` & `holcstore-0.1.7.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.050542 holcstore-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-04 07:05:56.000000 holcstore-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-04 07:05:56.000000 holcstore-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-04 07:06:00.050542 holcstore-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-04 07:05:56.000000 holcstore-0.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.046542 holcstore-0.1.6/holcstore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-04 07:05:56.000000 holcstore-0.1.6/holcstore/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.050542 holcstore-0.1.6/holcstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-04 07:06:00.000000 holcstore-0.1.6/holcstore.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.046542 holcstore-0.1.6/hostore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.046542 holcstore-0.1.6/hostore/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7226 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 07:06:00.050542 holcstore-0.1.6/hostore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9019 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-04 07:05:56.000000 holcstore-0.1.6/hostore/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-04 07:05:56.000000 holcstore-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-04 07:06:00.050542 holcstore-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 07:05:56.000000 holcstore-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-15 08:53:27.000000 holcstore-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 08:53:27.000000 holcstore-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 08:53:31.017711 holcstore-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-15 08:53:27.000000 holcstore-0.1.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.013712 holcstore-0.1.7/holcstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 08:53:27.000000 holcstore-0.1.7/holcstore/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/holcstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 08:53:31.000000 holcstore-0.1.7/holcstore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/hostore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/hostore/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:31.017711 holcstore-0.1.7/hostore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9105 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-15 08:53:27.000000 holcstore-0.1.7/hostore/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 08:53:27.000000 holcstore-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 08:53:31.017711 holcstore-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-15 08:53:27.000000 holcstore-0.1.7/setup.py
```

### Comparing `holcstore-0.1.6/LICENSE` & `holcstore-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.6/PKG-INFO` & `holcstore-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.6/README.rst` & `holcstore-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.6/holcstore/settings.py` & `holcstore-0.1.7/holcstore/settings.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.6/holcstore/urls.py` & `holcstore-0.1.7/holcstore/urls.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.6/holcstore.egg-info/PKG-INFO` & `holcstore-0.1.7/holcstore.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holcstore
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Django App to use a simple load curve store
 Home-page: 
 Author: Jean-Pierre Lartigue
 Author-email: 
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `holcstore-0.1.6/holcstore.egg-info/SOURCES.txt` & `holcstore-0.1.7/holcstore.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,9 @@
 hostore/tests.py
 hostore/views.py
 hostore/migrations/0001_initial.py
 hostore/migrations/0002_rename_store_testd_prm_91e86e_idx_hostore_tes_prm_897468_idx.py
 hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py
 hostore/migrations/__init__.py
 hostore/utils/__init__.py
-hostore/utils/timeseries.py
+hostore/utils/timeseries.py
+hostore/utils/utils.py
```

### Comparing `holcstore-0.1.6/hostore/migrations/0001_initial.py` & `holcstore-0.1.7/hostore/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.6/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py` & `holcstore-0.1.7/hostore/migrations/0003_alter_testdatastore_unique_together_and_more.py`

 * *Files identical despite different names*

### Comparing `holcstore-0.1.6/hostore/models.py` & `holcstore-0.1.7/hostore/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import io
 import logging
 from collections import defaultdict
 from typing import List, Dict
-
+import datetime as dt
 import pandas as pd
 from django.db import models
 from django.db.models import Max
 from pyarrow import BufferReader
 
 from .manager import StoreQuerySet
-from .utils.timeseries import ts_combine_first
+from .utils.timeseries import ts_combine_first, find_constant_sequences, check_ts_completeness
+from .utils.utils import chunks
 
 logger = logging.getLogger(__name__)
 
 
 class Store(models.Model):
     client_id = models.IntegerField()
     prm = models.CharField(max_length=30)
@@ -29,14 +30,59 @@
         indexes = [models.Index(fields=['prm', 'client_id']), ]
 
     @classmethod
     def count(cls, client_id: int):
         return cls.objects.filter(client_id=client_id).count()
 
     @classmethod
+    def find_holes(cls, client_id: int, sd: dt.datetime, ed: dt.datetime, freq='30min', prms: List[str] = None, chunk_size=50,
+                   freq_margin=pd.Timedelta(minutes=0)) -> Dict[str, List]:
+        """
+        Find holes (missing data periods) for multiple prms within a specified datetime range.
+
+        This method retrieves data from a database for each parameter associated with a client_id,
+        checks each dataset for missing data within the specified datetime range, and identifies the start
+        and end of each missing data period.
+
+        :param client_id: ID of the client for whom the data is being checked.
+        :param sd: Start datetime of the range to check for holes.
+        :param ed: End datetime of the range to check for holes.
+        :param freq: Frequency at which the data is expected, defaulting to '30min'.
+        :param prms: Optional list of prms to check; if None, all parameters for the client are checked.
+        :param chunk_size: The size of chunks to break the parameter list into for batch processing.
+                           This helps in managing memory and processing large datasets efficiently, defaulting to 50.
+        :param freq_margin: Freq margin for null sequences
+        :return: A dictionary with prm as keys and a list of tuples (start, end) indicating
+                 the missing data periods for each parameter. Start and end are included
+        """
+        # If no prm are specified, retrieve all prm for the given client from the database
+        if prms is None:
+            prms = list(cls.objects.filter(client_id=client_id).values_list('prm', flat=True))
+
+        # Iterate over prms in chunks to manage memory usage and efficiency
+        for prm_chunk in chunks(prms, chunk_size):
+            data_by_prm = cls.get_many_lc(prm_chunk, client_id, combined_versions=True)
+
+            # Check each parameter's data for completeness
+            for prm in prm_chunk:
+                nulls_seqs = []
+                data = data_by_prm[prm]
+                if len(data) == 0:
+                    # If there's no data for a prm, the entire range is considered as a hole
+                    nulls_seqs = [(sd, ed)]
+                else:
+                    # Data is wrapped in a list, and there's only one dataset per prm (combined_versions=True)
+                    assert len(data) == 1
+                    nulls_seqs = check_ts_completeness(data[0]['data'], sd, ed, freq=freq, freq_margin=freq_margin)
+
+                # Yield the output for this prm
+                # This allows processing part by part without waiting for the entire operation to complete
+                yield prm, nulls_seqs
+
+    @classmethod
     def get_lc(cls, prm: str, client_id: int, combined_versions=True, version: int = None) -> List[Dict]:
         """
         Get the prm load curve
         Args:
             prm: str
             client_id: int, client's id
             combined_versions: bool, if multiple versions exists we combine them (default True)
```

### Comparing `holcstore-0.1.6/hostore/tests.py` & `holcstore-0.1.7/hostore/tests.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import io
 import random
-
+import datetime as dt
 import numpy as np
 import pandas as pd
+import pytz
 from django.test import TestCase
 
 from .models import TestDataStore
 
 
 class HoCacheTestCase(TestCase):
     databases = ('default',)
@@ -206,7 +207,55 @@
     def test_set_index_with_different_names(self):
         ds = pd.Series([1, 2, 3])
         ds.index.name = 'test'
         TestDataStore.set_lc('key', ds, self.test_client_id)
         # Get the serie from cache
         ds_from_cache = TestDataStore.get_lc('key', self.test_client_id)[0]['data']
         pd.testing.assert_series_equal(ds, ds_from_cache, check_names=False)
+
+    def test_find_holes(self):
+        sd = dt.datetime(2024, 1, 1).astimezone(tz=pytz.UTC)
+        ed = dt.datetime(2024, 1, 11).astimezone(tz=pytz.UTC)
+        idx = pd.date_range(sd, ed, freq='D')
+        ds_no_hole = pd.Series(10, idx)
+        ds_no_hole.index.name = 'no_hole'
+
+        ds_one_hole = ds_no_hole.copy()
+        ds_one_hole.loc['2024-01-02':'2024-01-03'] = None
+        ds_one_hole.index.name = 'one_hole'
+
+        ds_two_holes = ds_no_hole.copy()
+        ds_two_holes.loc['2024-01-02':'2024-01-03'] = None
+        ds_two_holes.loc['2024-01-05':'2024-01-08'] = None
+        ds_two_holes.index.name = 'two_holes'
+
+        TestDataStore.set_lc('no_hole', ds_no_hole, self.test_client_id)
+        TestDataStore.set_lc('one_hole', ds_one_hole, self.test_client_id)
+        TestDataStore.set_lc('two_holes', ds_two_holes, self.test_client_id)
+
+        # Get holes of one_hole
+        holes = list(TestDataStore.find_holes(self.test_client_id, sd, ed, freq='D', prms=['one_hole']))
+        self.assertEquals(len(holes), 1)
+        self.assertEquals(holes[0][0], 'one_hole')
+        self.assertEquals(holes[0][1][0],
+                          (dt.datetime(2024, 1, 2).astimezone(tz=pytz.UTC),
+                           dt.datetime(2024, 1, 3).astimezone(tz=pytz.UTC)))
+
+        # Get holes of two_holes
+        holes = list(TestDataStore.find_holes(self.test_client_id, sd, ed, freq='D', prms=['two_holes']))
+        self.assertEquals(len(holes), 1)
+        self.assertEquals(holes[0][0], 'two_holes')
+        self.assertEquals(holes[0][1][0],
+                          (dt.datetime(2024, 1, 2).astimezone(tz=pytz.UTC),
+                           dt.datetime(2024, 1, 3).astimezone(tz=pytz.UTC)))
+        self.assertEquals(holes[0][1][1],
+                          (dt.datetime(2024, 1, 5).astimezone(tz=pytz.UTC),
+                           dt.datetime(2024, 1, 8).astimezone(tz=pytz.UTC)))
+
+        # Get holes of no_hole
+        holes = list(TestDataStore.find_holes(self.test_client_id, sd, ed, freq='D', prms=['no_hole']))
+        self.assertEquals(holes[0][0], 'no_hole')
+        self.assertEquals(holes[0][1], [])
+
+        # Get all holes
+        holes = list(TestDataStore.find_holes(self.test_client_id, sd, ed, freq='D', prms=['no_hole', 'one_hole', 'two_holes', 'non_existing']))
+        self.assertEquals(len(holes), 4)
```

### Comparing `holcstore-0.1.6/hostore/utils/timeseries.py` & `holcstore-0.1.7/hostore/utils/timeseries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime as dt
 import logging
 import pandas as pd
-from typing import Union
+from typing import Union, List, Tuple
 
 logger = logging.getLogger(__name__)
 
 
 def check_ts_completeness(ds: pd.Series, start: dt.datetime, end: dt.datetime, tag=None, freq=None, freq_margin=None,
-                          msgs=None):
+                          msgs=None) -> List[Tuple[Union[dt.datetime, dt.date], Union[dt.datetime, dt.date]]]:
     """
     Check if timeserie ds contains full data between start and end at freq.
 
     Optionnally store descriptions of holes in msgs.
 
     :param ds: timeserie to check
     :type ds: pd.DataFrame or pd.Series
```

### Comparing `holcstore-0.1.6/setup.cfg` & `holcstore-0.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = holcstore
-version = 0.1.6
+version = 0.1.7
 description = A Django App to use a simple load curve store
 long_description = file: README.rst
 url = 
 author = Jean-Pierre Lartigue
 author_email = 
 license = BSD-3-Clause
 classifiers =
```

