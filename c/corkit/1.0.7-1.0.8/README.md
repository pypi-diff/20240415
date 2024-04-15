# Comparing `tmp/corkit-1.0.7.tar.gz` & `tmp/corkit-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corkit-1.0.7.tar", last modified: Mon Apr 15 01:01:44 2024, max compression
+gzip compressed data, was "corkit-1.0.8.tar", last modified: Mon Apr 15 01:21:49 2024, max compression
```

## Comparing `corkit-1.0.7.tar` & `corkit-1.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:01:44.107457 corkit-1.0.7/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.7/LICENSE
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     3202 2024-04-15 01:01:44.107457 corkit-1.0.7/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     2909 2024-04-15 00:49:40.000000 corkit-1.0.7/README.rst
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:01:44.107457 corkit-1.0.7/corkit/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.7/corkit/__init__.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:50:19.000000 corkit-1.0.7/corkit/dataset.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 01:00:44.000000 corkit-1.0.7/corkit/lasco.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:50:17.000000 corkit-1.0.7/corkit/reconstruction.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:50:16.000000 corkit-1.0.7/corkit/secchi.py
--rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 01:00:48.000000 corkit-1.0.7/corkit/utils.py
-drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:01:44.107457 corkit-1.0.7/corkit.egg-info/
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     3202 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/PKG-INFO
--rw-rw-r--   0 jenci     (1000) jenci     (1000)      287 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/requires.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 01:01:44.000000 corkit-1.0.7/corkit.egg-info/top_level.txt
--rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 01:01:44.107457 corkit-1.0.7/setup.cfg
--rw-rw-r--   0 jenci     (1000) jenci     (1000)     1486 2024-04-15 01:00:36.000000 corkit-1.0.7/setup.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:21:49.569021 corkit-1.0.8/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1078 2024-04-14 19:27:35.000000 corkit-1.0.8/LICENSE
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2876 2024-04-15 01:21:49.569021 corkit-1.0.8/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2583 2024-04-15 01:18:04.000000 corkit-1.0.8/README.md
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:21:49.569021 corkit-1.0.8/corkit/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      146 2024-04-15 00:50:20.000000 corkit-1.0.8/corkit/__init__.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     6854 2024-04-15 00:50:19.000000 corkit-1.0.8/corkit/dataset.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    18207 2024-04-15 01:00:44.000000 corkit-1.0.8/corkit/lasco.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     8006 2024-04-15 00:50:17.000000 corkit-1.0.8/corkit/reconstruction.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       98 2024-04-15 00:50:16.000000 corkit-1.0.8/corkit/secchi.py
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)    42201 2024-04-15 01:17:23.000000 corkit-1.0.8/corkit/utils.py
+drwxrwxr-x   0 jenci     (1000) jenci     (1000)        0 2024-04-15 01:21:49.569021 corkit-1.0.8/corkit.egg-info/
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     2876 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)      286 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        1 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       82 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/requires.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)        7 2024-04-15 01:21:49.000000 corkit-1.0.8/corkit.egg-info/top_level.txt
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)       38 2024-04-15 01:21:49.569021 corkit-1.0.8/setup.cfg
+-rw-rw-r--   0 jenci     (1000) jenci     (1000)     1485 2024-04-15 01:17:57.000000 corkit-1.0.8/setup.py
```

### Comparing `corkit-1.0.7/LICENSE` & `corkit-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `corkit-1.0.7/PKG-INFO` & `corkit-1.0.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,35 @@
 Metadata-Version: 2.1
 Name: corkit
-Version: 1.0.7
+Version: 1.0.8
 Summary: Open source coronagraph data downloader and calibrator
 Home-page: https://github.com/Jorgedavyd/corkit
 Author: Jorge David Enciso Martínez
 Author-email: jorged.encyso@gmail.com
 License: MIT
 Platform: UNKNOWN
 License-File: LICENSE
 
-.. -*- mode: rst -*-
+[![pypi](https://img.shields.io/pypi/v/corkit)](https://pypi.org/project/corkit)
+![status](https://img.shields.io/badge/status-beta-red.svg)
+[![license](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-|PyPi| |Status| |License|
+# CorKit: Coronagraph Science Kit
 
-.. |PyPi| image:: https://img.shields.io/pypi/v/corkit
-   :target: https://pypi.org/project/corkit
-
-.. |Status| image:: https://img.shields.io/badge/status-beta-red.svg
-    
-.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
-
-===============================
-CorKit: Coronagraph Science Kit
-===============================
-
-.. figure:: https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png
-  :target: https://pypi.org/project/corkit
-  :align: center
+[![logo](https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png)](https://pypi.org/project/corkit)
 
 **CorKit** is an open-source Python library designed to streamline the 
 retrieval and preprocessing of solar coronagraph data. Its primary aim 
 is to democratize access to coronagraph data, enabling a broader community 
 of solar scientists to engage in research without the need for proprietary 
-software like IDL. It's derived from `Solarsoft <https://www.lmsal.com/solarsoft/>`__:
+software like IDL. It's derived from [Solarsoft](https://www.lmsal.com/solarsoft/):
 
-.. figure:: https://github.com/Jorgedavyd/corkit/blob/main/docs/examples/c2.png
-    :align: center
+![example](https://github.com/Jorgedavyd/corkit/blob/main/docs/examples/c2.png)
 
-Key Features:
--------------------------------
+## Key Features:
 
 1. **Open Source Accessibility**: **CorKit** removes barriers to entry by providing 
 free access to solar coronagraph data. Its open-source nature ensures that researchers, 
 educators, and enthusiasts can easily retrieve and analyze data without worrying about 
 proprietary software licenses.
 
 2. **User-Friendly Interface**: With simple and intuitive methods, **CorKit** makes it 
@@ -57,26 +43,17 @@
 leading to new insights and discoveries.
 
 4. **Community Collaboration**: **CorKit** fosters collaboration and knowledge sharing 
 within the solar science community. By providing a common platform for data access and 
 preprocessing, the library encourages interdisciplinary collaborations and accelerates 
 scientific progress.
 
-Coronagraph data supported
--------------------------------
-
-.. figure::https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif
-    :align: center
-    :width: 240px
-
-
-.. image::https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA
-    :align: center
-    :width: 240px
-
-Contact
--------------------------------
-- `Linkedin <https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/>`__
-- `Email <jorged.encyso@gmail.com>`__
-- `GitHub <https://github.com/Jorgedavyd>`__
-
+## Coronagraph data supported
+<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif" width="200" height="200" />
+<img src="https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA" width="200" height="200" />
+
+## Contact  
+
+- [Linkedin](https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/)
+- [Email](jorged.encyso@gmail.com)
+- [GitHub](https://github.com/Jorgedavyd)
```

### Comparing `corkit-1.0.7/README.rst` & `corkit-1.0.8/corkit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,35 @@
-.. -*- mode: rst -*-
+Metadata-Version: 2.1
+Name: corkit
+Version: 1.0.8
+Summary: Open source coronagraph data downloader and calibrator
+Home-page: https://github.com/Jorgedavyd/corkit
+Author: Jorge David Enciso Martínez
+Author-email: jorged.encyso@gmail.com
+License: MIT
+Platform: UNKNOWN
+License-File: LICENSE
+
+[![pypi](https://img.shields.io/pypi/v/corkit)](https://pypi.org/project/corkit)
+![status](https://img.shields.io/badge/status-beta-red.svg)
+[![license](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
-|PyPi| |Status| |License|
+# CorKit: Coronagraph Science Kit
 
-.. |PyPi| image:: https://img.shields.io/pypi/v/corkit
-   :target: https://pypi.org/project/corkit
-
-.. |Status| image:: https://img.shields.io/badge/status-beta-red.svg
-    
-.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
-
-===============================
-CorKit: Coronagraph Science Kit
-===============================
-
-.. figure:: https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png
-  :target: https://pypi.org/project/corkit
-  :align: center
+[![logo](https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png)](https://pypi.org/project/corkit)
 
 **CorKit** is an open-source Python library designed to streamline the 
 retrieval and preprocessing of solar coronagraph data. Its primary aim 
 is to democratize access to coronagraph data, enabling a broader community 
 of solar scientists to engage in research without the need for proprietary 
-software like IDL. It's derived from `Solarsoft <https://www.lmsal.com/solarsoft/>`__:
+software like IDL. It's derived from [Solarsoft](https://www.lmsal.com/solarsoft/):
 
-.. figure:: https://github.com/Jorgedavyd/corkit/blob/main/docs/examples/c2.png
-    :align: center
+![example](https://github.com/Jorgedavyd/corkit/blob/main/docs/examples/c2.png)
 
-Key Features:
--------------------------------
+## Key Features:
 
 1. **Open Source Accessibility**: **CorKit** removes barriers to entry by providing 
 free access to solar coronagraph data. Its open-source nature ensures that researchers, 
 educators, and enthusiasts can easily retrieve and analyze data without worrying about 
 proprietary software licenses.
 
 2. **User-Friendly Interface**: With simple and intuitive methods, **CorKit** makes it 
@@ -46,24 +43,17 @@
 leading to new insights and discoveries.
 
 4. **Community Collaboration**: **CorKit** fosters collaboration and knowledge sharing 
 within the solar science community. By providing a common platform for data access and 
 preprocessing, the library encourages interdisciplinary collaborations and accelerates 
 scientific progress.
 
-Coronagraph data supported
--------------------------------
+## Coronagraph data supported
+<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif" width="200" height="200" />
+<img src="https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA" width="200" height="200" />
+
+## Contact  
+
+- [Linkedin](https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/)
+- [Email](jorged.encyso@gmail.com)
+- [GitHub](https://github.com/Jorgedavyd)
 
-.. figure::https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif
-    :align: center
-    :width: 240px
-
-
-.. image::https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA
-    :align: center
-    :width: 240px
-
-Contact
--------------------------------
-- `Linkedin <https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/>`__
-- `Email <jorged.encyso@gmail.com>`__
-- `GitHub <https://github.com/Jorgedavyd>`__
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `corkit-1.0.7/corkit/dataset.py` & `corkit-1.0.8/corkit/dataset.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.7/corkit/lasco.py` & `corkit-1.0.8/corkit/lasco.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.7/corkit/reconstruction.py` & `corkit-1.0.8/corkit/reconstruction.py`

 * *Files identical despite different names*

### Comparing `corkit-1.0.7/corkit/utils.py` & `corkit-1.0.8/corkit/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from matplotlib import tri
 from PIL import Image
 import pandas as pd
 import numpy as np 
 import glob
 import os
 
-version = '1.0.7'
+version = '1.0.8'
 
 radeg = 180/np.pi
 
 DEFAULT_SAVE_DIR = os.path.join(os.path.dirname(__file__),'data')
 
 #done
 def datetime_interval(init: datetime, last: datetime, step_size: timedelta, output_format: str = '%Y%m%d'):
```

### Comparing `corkit-1.0.7/corkit.egg-info/PKG-INFO` & `corkit-1.0.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,24 @@
-Metadata-Version: 2.1
-Name: corkit
-Version: 1.0.7
-Summary: Open source coronagraph data downloader and calibrator
-Home-page: https://github.com/Jorgedavyd/corkit
-Author: Jorge David Enciso Martínez
-Author-email: jorged.encyso@gmail.com
-License: MIT
-Platform: UNKNOWN
-License-File: LICENSE
-
-.. -*- mode: rst -*-
-
-|PyPi| |Status| |License|
-
-.. |PyPi| image:: https://img.shields.io/pypi/v/corkit
-   :target: https://pypi.org/project/corkit
-
-.. |Status| image:: https://img.shields.io/badge/status-beta-red.svg
-    
-.. |License| image:: https://img.shields.io/badge/License-MIT-yellow.svg
-   :target: https://opensource.org/licenses/MIT
-
-===============================
-CorKit: Coronagraph Science Kit
-===============================
-
-.. figure:: https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png
-  :target: https://pypi.org/project/corkit
-  :align: center
+[![pypi](https://img.shields.io/pypi/v/corkit)](https://pypi.org/project/corkit)
+![status](https://img.shields.io/badge/status-beta-red.svg)
+[![license](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+# CorKit: Coronagraph Science Kit
+
+[![logo](https://github.com/Jorgedavyd/corkit/blob/main/docs/source/logo.png)](https://pypi.org/project/corkit)
 
 **CorKit** is an open-source Python library designed to streamline the 
 retrieval and preprocessing of solar coronagraph data. Its primary aim 
 is to democratize access to coronagraph data, enabling a broader community 
 of solar scientists to engage in research without the need for proprietary 
-software like IDL. It's derived from `Solarsoft <https://www.lmsal.com/solarsoft/>`__:
+software like IDL. It's derived from [Solarsoft](https://www.lmsal.com/solarsoft/):
 
-.. figure:: https://github.com/Jorgedavyd/corkit/blob/main/docs/examples/c2.png
-    :align: center
+![example](https://github.com/Jorgedavyd/corkit/blob/main/docs/examples/c2.png)
 
-Key Features:
--------------------------------
+## Key Features:
 
 1. **Open Source Accessibility**: **CorKit** removes barriers to entry by providing 
 free access to solar coronagraph data. Its open-source nature ensures that researchers, 
 educators, and enthusiasts can easily retrieve and analyze data without worrying about 
 proprietary software licenses.
 
 2. **User-Friendly Interface**: With simple and intuitive methods, **CorKit** makes it 
@@ -57,26 +32,16 @@
 leading to new insights and discoveries.
 
 4. **Community Collaboration**: **CorKit** fosters collaboration and knowledge sharing 
 within the solar science community. By providing a common platform for data access and 
 preprocessing, the library encourages interdisciplinary collaborations and accelerates 
 scientific progress.
 
-Coronagraph data supported
--------------------------------
-
-.. figure::https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif
-    :align: center
-    :width: 240px
-
-
-.. image::https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA
-    :align: center
-    :width: 240px
-
-Contact
--------------------------------
-- `Linkedin <https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/>`__
-- `Email <jorged.encyso@gmail.com>`__
-- `GitHub <https://github.com/Jorgedavyd>`__
-
-
+## Coronagraph data supported
+<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Stereo_logo.gif/1200px-Stereo_logo.gif" width="200" height="200" />
+<img src="https://lh6.googleusercontent.com/proxy/1sXRF-9df_jeWpUWlyDqUn4ddQ34PIis-2zBpOf46TeKkQPJdNVbLL_ciXXUaS-AZR0Z4tBFqaYSdIZJwuKnhNtIy2pFekckiA" width="200" height="200" />
+
+## Contact  
+
+- [Linkedin](https://www.linkedin.com/in/jorge-david-enciso-mart%C3%ADnez-149977265/)
+- [Email](jorged.encyso@gmail.com)
+- [GitHub](https://github.com/Jorgedavyd)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `corkit-1.0.7/setup.py` & `corkit-1.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 import os
 
 class InstallDataset(install):
     def run(self):
         install.run(self)
         subprocess.check_call([sys.executable, 'corkit/dataset.py'])
 
-version = '1.0.7'
+version = '1.0.8'
 
 def find_calibration_files():
     module_root = os.path.dirname(__file__)
     calibration_data_dir = os.path.join(module_root, 'corkit', 'data')
     calibration_files = []
     for root, _, files in os.walk(calibration_data_dir):
         for file in files:
             calibration_files.append(os.path.relpath(os.path.join(root, file), module_root))
     return calibration_files
 
-with open('README.rst') as file:
+with open('README.md') as file:
     long_description = file.read()
 
 if __name__ == '__main__':
     setup(
         name='corkit',
         version=version,
         packages=find_packages(),
```

