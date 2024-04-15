# Comparing `tmp/corkit-1.0.3.tar.gz` & `tmp/corkit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corkit-1.0.3.tar", last modified: Sun Apr 14 18:52:16 2024, max compression
+gzip compressed data, was "corkit-1.0.4.tar", last modified: Sun Apr 14 19:31:24 2024, max compression
```

## Comparing `corkit-1.0.3.tar` & `corkit-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-14 18:52:16.355846 corkit-1.0.3/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 18:51:34.000000 corkit-1.0.3/LICENSE
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      300 2024-04-14 18:52:16.355846 corkit-1.0.3/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2265 2024-04-14 18:51:33.000000 corkit-1.0.3/README.md
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-14 18:52:16.355846 corkit-1.0.3/corkit/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-14 18:50:22.000000 corkit-1.0.3/corkit/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     6800 2024-04-14 18:50:10.000000 corkit-1.0.3/corkit/dataset.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-14 06:05:38.000000 corkit-1.0.3/corkit/lasco.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-14 06:05:40.000000 corkit-1.0.3/corkit/reconstruction.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-14 06:05:40.000000 corkit-1.0.3/corkit/secchi.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-14 18:50:01.000000 corkit-1.0.3/corkit/utils.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-14 18:52:16.355846 corkit-1.0.3/corkit.egg-info/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      300 2024-04-14 18:52:16.000000 corkit-1.0.3/corkit.egg-info/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      286 2024-04-14 18:52:16.000000 corkit-1.0.3/corkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-14 18:52:16.000000 corkit-1.0.3/corkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-14 18:52:16.000000 corkit-1.0.3/corkit.egg-info/requires.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-14 18:52:16.000000 corkit-1.0.3/corkit.egg-info/top_level.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-14 18:52:16.355846 corkit-1.0.3/setup.cfg
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1174 2024-04-14 18:51:31.000000 corkit-1.0.3/setup.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-14 19:31:24.499970 corkit-1.0.4/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.4/LICENSE
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      300 2024-04-14 19:31:24.499970 corkit-1.0.4/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2195 2024-04-14 19:27:35.000000 corkit-1.0.4/README.md
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-14 19:31:24.499970 corkit-1.0.4/corkit/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-14 18:50:22.000000 corkit-1.0.4/corkit/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-14 19:19:04.000000 corkit-1.0.4/corkit/dataset.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-14 06:05:38.000000 corkit-1.0.4/corkit/lasco.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-14 06:05:40.000000 corkit-1.0.4/corkit/reconstruction.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-14 06:05:40.000000 corkit-1.0.4/corkit/secchi.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-14 19:31:11.000000 corkit-1.0.4/corkit/utils.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-14 19:31:24.499970 corkit-1.0.4/corkit.egg-info/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      300 2024-04-14 19:31:24.000000 corkit-1.0.4/corkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      286 2024-04-14 19:31:24.000000 corkit-1.0.4/corkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-14 19:31:24.000000 corkit-1.0.4/corkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-14 19:31:24.000000 corkit-1.0.4/corkit.egg-info/requires.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-14 19:31:24.000000 corkit-1.0.4/corkit.egg-info/top_level.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-14 19:31:24.499970 corkit-1.0.4/setup.cfg
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1374 2024-04-14 19:31:17.000000 corkit-1.0.4/setup.py
```

### Comparing `corkit-1.0.3/LICENSE` & `corkit-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `corkit-1.0.3/README.md` & `corkit-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 
 ![status](https://img.shields.io/badge/status-beta-red.svg)
-![Version](https://img.shields.io/badge/version-1.0.3-blue.svg)
-![pypi](https://img.shields.io/pypi/pyversions/corkit)
+![Version](https://img.shields.io/pypi/v/corkit)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 <h1 style="text-align:center;">CorKit: Coronagraph Science Kit</h1>
 
 <div style="text-align:center;">
     <img src="https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png">
 </div>
```

### Comparing `corkit-1.0.3/corkit/dataset.py` & `corkit-1.0.4/corkit/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,8 +147,11 @@
         new = np.asarray(sav_df['c_utc'])
         data['c_utc_time'] = new['time']
         data['c_utc_mjd'] = new['mjd']
         df = pd.DataFrame(data, index = index, columns = data.keys())
         dfs.append(df)
     
     for filepath, df in zip(filepaths, dfs):
-        df.to_csv(filepath)
+        df.to_csv(filepath)
+
+if __name__ == '__main__':
+    asyncio.run(update())
```

### Comparing `corkit-1.0.3/corkit/lasco.py` & `corkit-1.0.4/corkit/lasco.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.3/corkit/reconstruction.py` & `corkit-1.0.4/corkit/reconstruction.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.3/corkit/utils.py` & `corkit-1.0.4/corkit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib import tri
 from PIL import Image
 import pandas as pd
 import numpy as np 
 import glob
 import os
 
-version = '1.0.3'
+version = '1.0.4'
 
 radeg = 180/np.pi
 
 DEFAULT_SAVE_DIR = os.path.join(os.path.dirname(__file__),'data')
 
 #done
 def datetime_interval(init: datetime, last: datetime, step_size: timedelta, output_format: str = '%Y%m%d'):
```

### Comparing `corkit-1.0.3/setup.py` & `corkit-1.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 from setuptools import setup, find_packages
+from setuptools.command.install import install
+import subprocess
+import sys
+import os
+
+class InstallDataset(install):
+    def run(self):
+        install.run(self)
+        subprocess.check_call([sys.executable, 'corkit/dataset.py'])
 
-version = '1.0.3'
+version = '1.0.4'
 
 def find_calibration_files():
     module_root = os.path.dirname(__file__)
     calibration_data_dir = os.path.join(module_root, 'corkit', 'data')
     calibration_files = []
     for root, _, files in os.walk(calibration_data_dir):
         for file in files:
@@ -28,17 +37,14 @@
             'scipy',
             'scikit-image',
             'beautifulsoup4',
             'matplotlib',
             'pillow',
             'pandas',
         ],
+        cmdclass={
+            'install': InstallDataset
+        }
     )
 
-    from corkit.dataset import update
-    import asyncio
-    import os
-
-    asyncio.run(update())
-
```

