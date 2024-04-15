# Comparing `tmp/corkit-1.0.6.tar.gz` & `tmp/corkit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corkit-1.0.6.tar", last modified: Mon Apr 15 00:53:16 2024, max compression
+gzip compressed data, was "corkit-1.0.7.tar", last modified: Mon Apr 15 01:01:44 2024, max compression
```

## Comparing `corkit-1.0.6.tar` & `corkit-1.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:53:16.611848 corkit-1.0.6/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.6/LICENSE
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     3239 2024-04-15 00:53:16.611848 corkit-1.0.6/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2909 2024-04-15 00:49:40.000000 corkit-1.0.6/README.rst
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:53:16.611848 corkit-1.0.6/corkit/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.6/corkit/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:50:19.000000 corkit-1.0.6/corkit/dataset.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 00:50:18.000000 corkit-1.0.6/corkit/lasco.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:50:17.000000 corkit-1.0.6/corkit/reconstruction.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:50:16.000000 corkit-1.0.6/corkit/secchi.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 00:52:57.000000 corkit-1.0.6/corkit/utils.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:53:16.611848 corkit-1.0.6/corkit.egg-info/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     3239 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      287 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/requires.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/top_level.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 00:53:16.611848 corkit-1.0.6/setup.cfg
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1563 2024-04-15 00:49:54.000000 corkit-1.0.6/setup.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:01:44.107457 corkit-1.0.7/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.7/LICENSE
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     3202 2024-04-15 01:01:44.107457 corkit-1.0.7/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2909 2024-04-15 00:49:40.000000 corkit-1.0.7/README.rst
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:01:44.107457 corkit-1.0.7/corkit/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.7/corkit/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:50:19.000000 corkit-1.0.7/corkit/dataset.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 01:00:44.000000 corkit-1.0.7/corkit/lasco.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:50:17.000000 corkit-1.0.7/corkit/reconstruction.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:50:16.000000 corkit-1.0.7/corkit/secchi.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 01:00:48.000000 corkit-1.0.7/corkit/utils.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:01:44.107457 corkit-1.0.7/corkit.egg-info/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     3202 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      287 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/requires.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/top_level.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 01:01:44.107457 corkit-1.0.7/setup.cfg
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1486 2024-04-15 01:00:36.000000 corkit-1.0.7/setup.py
```

### Comparing `corkit-1.0.6/LICENSE` & `corkit-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `corkit-1.0.6/PKG-INFO` & `corkit-1.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: corkit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Open source coronagraph data downloader and calibrator
 Home-page: https://github.com/Jorgedavyd/corkit
 Author: Jorge David Enciso Martínez
 Author-email: jorged.encyso@gmail.com
 License: MIT
 Platform: UNKNOWN
-Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
 |PyPi| |Status| |License|
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/corkit
```

### Comparing `corkit-1.0.6/README.rst` & `corkit-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `corkit-1.0.6/corkit/dataset.py` & `corkit-1.0.7/corkit/dataset.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.6/corkit/lasco.py` & `corkit-1.0.7/corkit/lasco.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import aiofiles
 import aiohttp
 import asyncio
 import os
 import glob
 
-version = '1.0.6'
+version = '1.0.7'
 
 #done
 def level_1(
         fits_file: Union[str, BytesIO],
         target_path: str,
         **kwargs
 ) -> None:
```

### Comparing `corkit-1.0.6/corkit/reconstruction.py` & `corkit-1.0.7/corkit/reconstruction.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.6/corkit/utils.py` & `corkit-1.0.7/corkit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib import tri
 from PIL import Image
 import pandas as pd
 import numpy as np 
 import glob
 import os
 
-version = '1.0.6'
+version = '1.0.7'
 
 radeg = 180/np.pi
 
 DEFAULT_SAVE_DIR = os.path.join(os.path.dirname(__file__),'data')
 
 #done
 def datetime_interval(init: datetime, last: datetime, step_size: timedelta, output_format: str = '%Y%m%d'):
```

### Comparing `corkit-1.0.6/corkit.egg-info/PKG-INFO` & `corkit-1.0.7/corkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: corkit
-Version: 1.0.6
+Version: 1.0.7
 Summary: Open source coronagraph data downloader and calibrator
 Home-page: https://github.com/Jorgedavyd/corkit
 Author: Jorge David Enciso Martínez
 Author-email: jorged.encyso@gmail.com
 License: MIT
 Platform: UNKNOWN
-Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
 |PyPi| |Status| |License|
 
 .. |PyPi| image:: https://img.shields.io/pypi/v/corkit
```

### Comparing `corkit-1.0.6/setup.py` & `corkit-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,36 +5,35 @@
 import os
 
 class InstallDataset(install):
     def run(self):
         install.run(self)
         subprocess.check_call([sys.executable, 'corkit/dataset.py'])
 
-version = '1.0.6'
+version = '1.0.7'
 
 def find_calibration_files():
     module_root = os.path.dirname(__file__)
     calibration_data_dir = os.path.join(module_root, 'corkit', 'data')
     calibration_files = []
     for root, _, files in os.walk(calibration_data_dir):
         for file in files:
             calibration_files.append(os.path.relpath(os.path.join(root, file), module_root))
     return calibration_files
 
-with open('README.rst', 'r', encoding = 'utf-8') as file:
+with open('README.rst') as file:
     long_description = file.read()
 
 if __name__ == '__main__':
     setup(
         name='corkit',
         version=version,
         packages=find_packages(),
         author='Jorge David Enciso Martínez',
         long_description=long_description,
-        long_description_content_type="text/x-rst",
         author_email='jorged.encyso@gmail.com',
         description='Open source coronagraph data downloader and calibrator',
         url='https://github.com/Jorgedavyd/corkit',
         license='MIT',
         install_requires=[
             'astropy',
             'numpy',
```

