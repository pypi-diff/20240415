# Comparing `tmp/corkit-1.0.5.tar.gz` & `tmp/corkit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corkit-1.0.5.tar", last modified: Mon Apr 15 00:37:20 2024, max compression
+gzip compressed data, was "corkit-1.0.6.tar", last modified: Mon Apr 15 00:53:16 2024, max compression
```

## Comparing `corkit-1.0.5.tar` & `corkit-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:37:20.422671 corkit-1.0.5/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.5/LICENSE
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      300 2024-04-15 00:37:20.422671 corkit-1.0.5/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2695 2024-04-15 00:33:55.000000 corkit-1.0.5/README.rst
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:37:20.422671 corkit-1.0.5/corkit/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:01:58.000000 corkit-1.0.5/corkit/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:01:56.000000 corkit-1.0.5/corkit/dataset.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 00:01:46.000000 corkit-1.0.5/corkit/lasco.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:01:50.000000 corkit-1.0.5/corkit/reconstruction.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:01:49.000000 corkit-1.0.5/corkit/secchi.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 00:01:52.000000 corkit-1.0.5/corkit/utils.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:37:20.422671 corkit-1.0.5/corkit.egg-info/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      300 2024-04-15 00:37:20.000000 corkit-1.0.5/corkit.egg-info/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      287 2024-04-15 00:37:20.000000 corkit-1.0.5/corkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 00:37:20.000000 corkit-1.0.5/corkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 00:37:20.000000 corkit-1.0.5/corkit.egg-info/requires.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 00:37:20.000000 corkit-1.0.5/corkit.egg-info/top_level.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 00:37:20.422671 corkit-1.0.5/setup.cfg
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1374 2024-04-15 00:35:15.000000 corkit-1.0.5/setup.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:53:16.611848 corkit-1.0.6/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.6/LICENSE
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     3239 2024-04-15 00:53:16.611848 corkit-1.0.6/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2909 2024-04-15 00:49:40.000000 corkit-1.0.6/README.rst
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:53:16.611848 corkit-1.0.6/corkit/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.6/corkit/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:50:19.000000 corkit-1.0.6/corkit/dataset.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 00:50:18.000000 corkit-1.0.6/corkit/lasco.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:50:17.000000 corkit-1.0.6/corkit/reconstruction.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:50:16.000000 corkit-1.0.6/corkit/secchi.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 00:52:57.000000 corkit-1.0.6/corkit/utils.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 00:53:16.611848 corkit-1.0.6/corkit.egg-info/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     3239 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      287 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/requires.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 00:53:16.000000 corkit-1.0.6/corkit.egg-info/top_level.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 00:53:16.611848 corkit-1.0.6/setup.cfg
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1563 2024-04-15 00:49:54.000000 corkit-1.0.6/setup.py
```

### Comparing `corkit-1.0.5/LICENSE` & `corkit-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `corkit-1.0.5/README.rst` & `corkit-1.0.6/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -56,8 +56,14 @@
 .. figure::https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif
     :align: center
     :width: 240px
 
 
 .. image::https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA
     :align: center
-    :width: 240px
+    :width: 240px
+
+Contact
+-------------------------------
+- `Linkedin <https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/>`__
+- `Email <jorged.encyso@gmail.com>`__
+- `GitHub <https://github.com/Jorgedavyd>`__
```

### Comparing `corkit-1.0.5/corkit/dataset.py` & `corkit-1.0.6/corkit/dataset.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.5/corkit/lasco.py` & `corkit-1.0.6/corkit/lasco.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import numpy as np
 import aiofiles
 import aiohttp
 import asyncio
 import os
 import glob
 
-version = '1.0.4'
+version = '1.0.6'
 
 #done
 def level_1(
         fits_file: Union[str, BytesIO],
         target_path: str,
         **kwargs
 ) -> None:
```

### Comparing `corkit-1.0.5/corkit/reconstruction.py` & `corkit-1.0.6/corkit/reconstruction.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.5/corkit/utils.py` & `corkit-1.0.6/corkit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib import tri
 from PIL import Image
 import pandas as pd
 import numpy as np 
 import glob
 import os
 
-version = '1.0.4'
+version = '1.0.6'
 
 radeg = 180/np.pi
 
 DEFAULT_SAVE_DIR = os.path.join(os.path.dirname(__file__),'data')
 
 #done
 def datetime_interval(init: datetime, last: datetime, step_size: timedelta, output_format: str = '%Y%m%d'):
```

### Comparing `corkit-1.0.5/setup.py` & `corkit-1.0.6/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,31 +5,36 @@
 import os
 
 class InstallDataset(install):
     def run(self):
         install.run(self)
         subprocess.check_call([sys.executable, 'corkit/dataset.py'])
 
-version = '1.0.5'
+version = '1.0.6'
 
 def find_calibration_files():
     module_root = os.path.dirname(__file__)
     calibration_data_dir = os.path.join(module_root, 'corkit', 'data')
     calibration_files = []
     for root, _, files in os.walk(calibration_data_dir):
         for file in files:
             calibration_files.append(os.path.relpath(os.path.join(root, file), module_root))
     return calibration_files
 
+with open('README.rst', 'r', encoding = 'utf-8') as file:
+    long_description = file.read()
+
 if __name__ == '__main__':
     setup(
         name='corkit',
         version=version,
         packages=find_packages(),
         author='Jorge David Enciso Martínez',
+        long_description=long_description,
+        long_description_content_type="text/x-rst",
         author_email='jorged.encyso@gmail.com',
         description='Open source coronagraph data downloader and calibrator',
         url='https://github.com/Jorgedavyd/corkit',
         license='MIT',
         install_requires=[
             'astropy',
             'numpy',
```

