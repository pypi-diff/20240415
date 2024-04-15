# Comparing `tmp/statmorph-0.5.6.tar.gz` & `tmp/statmorph-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statmorph-0.5.6.tar", last modified: Sat Apr 13 00:24:10 2024, max compression
+gzip compressed data, was "statmorph-0.5.7.tar", last modified: Mon Apr 15 19:59:41 2024, max compression
```

## Comparing `statmorph-0.5.6.tar` & `statmorph-0.5.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/
--rw-r--r--   0 vrg       (1000) users      (985)     1528 2024-02-12 03:04:55.000000 statmorph-0.5.6/LICENSE
--rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.6/MANIFEST.in
--rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-04-13 00:24:10.621439 statmorph-0.5.6/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.6/README.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.618105 statmorph-0.5.6/docs/
--rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/Makefile
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/docs/_static/
--rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/_static/banner.svg
--rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/_static/favicon.ico
--rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/_static/logo.png
--rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/api.rst
--rw-r--r--   0 vrg       (1000) users      (985)     2613 2024-04-12 23:54:40.000000 statmorph-0.5.6/docs/conf.py
--rw-r--r--   0 vrg       (1000) users      (985)     5009 2023-08-03 22:44:15.000000 statmorph-0.5.6/docs/description.rst
--rw-r--r--   0 vrg       (1000) users      (985)       88 2023-08-01 00:03:20.000000 statmorph-0.5.6/docs/examples.rst
--rw-r--r--   0 vrg       (1000) users      (985)     1424 2023-08-01 00:01:24.000000 statmorph-0.5.6/docs/index.rst
--rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/installation.rst
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/docs/notebooks/
--rw-r--r--   0 vrg       (1000) users      (985)    16723 2024-04-12 23:59:38.000000 statmorph-0.5.6/docs/notebooks/doublesersic.ipynb
--rw-r--r--   0 vrg       (1000) users      (985)    13570 2024-04-12 23:58:51.000000 statmorph-0.5.6/docs/notebooks/tutorial.ipynb
--rw-r--r--   0 vrg       (1000) users      (985)     1943 2024-04-13 00:02:01.000000 statmorph-0.5.6/docs/overview.rst
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.6/docs/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.6/requirements.txt
--rw-r--r--   0 vrg       (1000) users      (985)       38 2024-04-13 00:24:10.621439 statmorph-0.5.6/setup.cfg
--rw-r--r--   0 vrg       (1000) users      (985)     1363 2024-04-12 23:53:31.000000 statmorph-0.5.6/setup.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/
--rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/__init__.py
--rw-r--r--   0 vrg       (1000) users      (985)   121807 2024-04-13 00:18:58.000000 statmorph-0.5.6/statmorph/statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/tests/
--rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/tests/__init__.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/tests/data/
--rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/tests/data/slice.fits
--rw-r--r--   0 vrg       (1000) users      (985)    15145 2024-04-12 23:24:50.000000 statmorph-0.5.6/statmorph/tests/test_statmorph.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/utils/
--rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/utils/__init__.py
--rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.6/statmorph/utils/image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph/utils/tests/
--rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.6/statmorph/utils/tests/test_image_diagnostics.py
-drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-13 00:24:10.621439 statmorph-0.5.6/statmorph.egg-info/
--rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/PKG-INFO
--rw-r--r--   0 vrg       (1000) users      (985)      763 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/SOURCES.txt
--rw-r--r--   0 vrg       (1000) users      (985)        1 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/dependency_links.txt
--rw-r--r--   0 vrg       (1000) users      (985)      103 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/requires.txt
--rw-r--r--   0 vrg       (1000) users      (985)       10 2024-04-13 00:24:10.000000 statmorph-0.5.6/statmorph.egg-info/top_level.txt
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/
+-rw-r--r--   0 vrg       (1000) users      (985)     1528 2024-02-12 03:04:55.000000 statmorph-0.5.7/LICENSE
+-rw-r--r--   0 vrg       (1000) users      (985)      176 2022-10-15 05:52:48.000000 statmorph-0.5.7/MANIFEST.in
+-rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-04-15 19:59:41.992186 statmorph-0.5.7/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)     1585 2022-10-15 05:52:47.000000 statmorph-0.5.7/README.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.988853 statmorph-0.5.7/docs/
+-rw-r--r--   0 vrg       (1000) users      (985)      609 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/Makefile
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.988853 statmorph-0.5.7/docs/_static/
+-rw-r--r--   0 vrg       (1000) users      (985)    15518 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/_static/banner.svg
+-rw-r--r--   0 vrg       (1000) users      (985)     2238 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/_static/favicon.ico
+-rw-r--r--   0 vrg       (1000) users      (985)    31694 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/_static/logo.png
+-rw-r--r--   0 vrg       (1000) users      (985)      132 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/api.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     2613 2024-04-15 19:51:55.000000 statmorph-0.5.7/docs/conf.py
+-rw-r--r--   0 vrg       (1000) users      (985)     5009 2023-08-03 22:44:15.000000 statmorph-0.5.7/docs/description.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       88 2023-08-01 00:03:20.000000 statmorph-0.5.7/docs/examples.rst
+-rw-r--r--   0 vrg       (1000) users      (985)     1424 2023-08-01 00:01:24.000000 statmorph-0.5.7/docs/index.rst
+-rw-r--r--   0 vrg       (1000) users      (985)      780 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/installation.rst
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/docs/notebooks/
+-rw-r--r--   0 vrg       (1000) users      (985)    16723 2024-04-12 23:59:38.000000 statmorph-0.5.7/docs/notebooks/doublesersic.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)    13570 2024-04-12 23:58:51.000000 statmorph-0.5.7/docs/notebooks/tutorial.ipynb
+-rw-r--r--   0 vrg       (1000) users      (985)     1943 2024-04-13 00:02:01.000000 statmorph-0.5.7/docs/overview.rst
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.7/docs/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       73 2022-10-15 05:52:48.000000 statmorph-0.5.7/requirements.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       38 2024-04-15 19:59:41.992186 statmorph-0.5.7/setup.cfg
+-rw-r--r--   0 vrg       (1000) users      (985)     1363 2024-04-15 19:51:38.000000 statmorph-0.5.7/setup.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/statmorph/
+-rw-r--r--   0 vrg       (1000) users      (985)       25 2022-10-15 05:52:47.000000 statmorph-0.5.7/statmorph/__init__.py
+-rw-r--r--   0 vrg       (1000) users      (985)   121809 2024-04-15 19:51:11.000000 statmorph-0.5.7/statmorph/statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/statmorph/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)       30 2022-10-15 05:52:47.000000 statmorph-0.5.7/statmorph/tests/__init__.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/statmorph/tests/data/
+-rw-r--r--   0 vrg       (1000) users      (985)   276480 2022-10-15 05:52:47.000000 statmorph-0.5.7/statmorph/tests/data/slice.fits
+-rw-r--r--   0 vrg       (1000) users      (985)    15146 2024-04-15 19:50:54.000000 statmorph-0.5.7/statmorph/tests/test_statmorph.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/statmorph/utils/
+-rw-r--r--   0 vrg       (1000) users      (985)       33 2022-10-15 05:52:47.000000 statmorph-0.5.7/statmorph/utils/__init__.py
+-rwxr-xr-x   0 vrg       (1000) users      (985)    14333 2023-01-06 20:37:18.000000 statmorph-0.5.7/statmorph/utils/image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/statmorph/utils/tests/
+-rw-r--r--   0 vrg       (1000) users      (985)     1170 2022-10-15 05:52:47.000000 statmorph-0.5.7/statmorph/utils/tests/test_image_diagnostics.py
+drwxr-xr-x   0 vrg       (1000) users      (985)        0 2024-04-15 19:59:41.992186 statmorph-0.5.7/statmorph.egg-info/
+-rw-r--r--   0 vrg       (1000) users      (985)     2465 2024-04-15 19:59:41.000000 statmorph-0.5.7/statmorph.egg-info/PKG-INFO
+-rw-r--r--   0 vrg       (1000) users      (985)      763 2024-04-15 19:59:41.000000 statmorph-0.5.7/statmorph.egg-info/SOURCES.txt
+-rw-r--r--   0 vrg       (1000) users      (985)        1 2024-04-15 19:59:41.000000 statmorph-0.5.7/statmorph.egg-info/dependency_links.txt
+-rw-r--r--   0 vrg       (1000) users      (985)      103 2024-04-15 19:59:41.000000 statmorph-0.5.7/statmorph.egg-info/requires.txt
+-rw-r--r--   0 vrg       (1000) users      (985)       10 2024-04-15 19:59:41.000000 statmorph-0.5.7/statmorph.egg-info/top_level.txt
```

### Comparing `statmorph-0.5.6/LICENSE` & `statmorph-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/PKG-INFO` & `statmorph-0.5.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.6
+Version: 0.5.7
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.6/README.rst` & `statmorph-0.5.7/README.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/Makefile` & `statmorph-0.5.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/_static/banner.svg` & `statmorph-0.5.7/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/_static/favicon.ico` & `statmorph-0.5.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/_static/logo.png` & `statmorph-0.5.7/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/conf.py` & `statmorph-0.5.7/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'statmorph'
 copyright = '2017-2024, Vicente Rodriguez-Gomez'
 author = 'Vicente Rodriguez-Gomez'
 
 # The full version, including alpha/beta/rc tags
-release = '0.5.6'
+release = '0.5.7'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `statmorph-0.5.6/docs/description.rst` & `statmorph-0.5.7/docs/description.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/index.rst` & `statmorph-0.5.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/installation.rst` & `statmorph-0.5.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/notebooks/doublesersic.ipynb` & `statmorph-0.5.7/docs/notebooks/doublesersic.ipynb`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/notebooks/tutorial.ipynb` & `statmorph-0.5.7/docs/notebooks/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/docs/overview.rst` & `statmorph-0.5.7/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/setup.py` & `statmorph-0.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='statmorph',
-    version='0.5.6',
+    version='0.5.7',
     description='Non-parametric morphological diagnostics of galaxy images',
     long_description=long_description,
     url='https://github.com/vrodgom/statmorph',
     author='Vicente Rodriguez-Gomez',
     author_email='vrodgom.astro@gmail.com',
     license='BSD',
     classifiers=[
```

### Comparing `statmorph-0.5.6/statmorph/statmorph.py` & `statmorph-0.5.7/statmorph/statmorph.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'DoubleSersic2D',
     'ConvolvedDoubleSersic2D',
     'SourceMorphology',
     'source_morphology',
     '__version__',
 ]
 
-__version__ = '0.5.6'
+__version__ = '0.5.7'
 
 # A list of the quantities calculated by SourceMorphology,
 # excluding the double Sersic parameters:
 _quantity_names = [
     'xc_centroid',
     'yc_centroid',
     'ellipticity_centroid',
@@ -65,15 +65,15 @@
     'sn_per_pixel',
     'concentration',
     'asymmetry',
     'smoothness',
     'multimode',
     'intensity',
     'deviation',
-    'rms_asymmetry',
+    'rms_asymmetry2',
     'outer_asymmetry',
     'shape_asymmetry',
     'sersic_amplitude',
     'sersic_rhalf',
     'sersic_n',
     'sersic_xc',
     'sersic_yc',
@@ -1851,15 +1851,15 @@
         image = self._cutout_stamp_maskzeroed
         asym = self._asymmetry_function(self._asymmetry_center,
                                         image, 'cas')
 
         return asym
 
     @lazyproperty
-    def rms_asymmetry(self):
+    def rms_asymmetry2(self):
         """
         Calculate the RMS asymmetry as in eq. 27 of Sazonova et al. (2024).
         Note that this actually corresponds to the *square* of A_rms.
         """
         image = self._cutout_stamp_maskzeroed
         asym = self._asymmetry_function(self._asymmetry_center,
                                         image, 'rms')
```

### Comparing `statmorph-0.5.6/statmorph/tests/data/slice.fits` & `statmorph-0.5.7/statmorph/tests/data/slice.fits`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/statmorph/tests/test_statmorph.py` & `statmorph-0.5.7/statmorph/tests/test_statmorph.py`

 * *Files 1% similar despite different names*

```diff
@@ -313,15 +313,15 @@
             'sn_per_pixel': 6.80319166183472,
             'concentration': 2.19100140632153,
             'asymmetry': 0.00377345808887,
             'smoothness': 0.00430880839402,
             'multimode': 0.23423423423423,
             'intensity': 0.51203949030140,
             'deviation': 0.01522525597953,
-            'rms_asymmetry': 0.0053900924481633,
+            'rms_asymmetry2': 0.0053900924481633,
             'outer_asymmetry': -0.01821399684443,
             'shape_asymmetry': 0.16308278287864,
             'sersic_amplitude': 1296.95288208155739,
             'sersic_rhalf': 22.45788866502031,
             'sersic_n': 0.61206828194077,
             'sersic_xc': 81.56197595338546,
             'sersic_yc': 80.40465135599014,
```

### Comparing `statmorph-0.5.6/statmorph/utils/image_diagnostics.py` & `statmorph-0.5.7/statmorph/utils/image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/statmorph/utils/tests/test_image_diagnostics.py` & `statmorph-0.5.7/statmorph/utils/tests/test_image_diagnostics.py`

 * *Files identical despite different names*

### Comparing `statmorph-0.5.6/statmorph.egg-info/PKG-INFO` & `statmorph-0.5.7/statmorph.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statmorph
-Version: 0.5.6
+Version: 0.5.7
 Summary: Non-parametric morphological diagnostics of galaxy images
 Home-page: https://github.com/vrodgom/statmorph
 Author: Vicente Rodriguez-Gomez
 Author-email: vrodgom.astro@gmail.com
 License: BSD
 Keywords: astronomy galaxies galaxy-morphology non-parametric
 Classifier: Development Status :: 4 - Beta
```

### Comparing `statmorph-0.5.6/statmorph.egg-info/SOURCES.txt` & `statmorph-0.5.7/statmorph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

