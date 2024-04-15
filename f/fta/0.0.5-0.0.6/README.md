# Comparing `tmp/fta-0.0.5.tar.gz` & `tmp/fta-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fta-0.0.5.tar", last modified: Mon Apr 15 09:56:07 2024, max compression
+gzip compressed data, was "fta-0.0.6.tar", last modified: Mon Apr 15 09:56:59 2024, max compression
```

## Comparing `fta-0.0.5.tar` & `fta-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:56:07.966574 fta-0.0.5/
--rw-r--r--   0 voidful    (501) staff       (20)     4156 2024-04-09 07:40:16.000000 fta-0.0.5/.gitignore
--rw-r--r--   0 voidful    (501) staff       (20)    11357 2024-04-09 07:40:16.000000 fta-0.0.5/LICENSE
--rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:56:07.966343 fta-0.0.5/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)    28702 2024-04-09 10:34:05.000000 fta-0.0.5/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:56:07.963668 fta-0.0.5/fta/
--rw-r--r--   0 voidful    (501) staff       (20)       29 2024-04-09 07:40:16.000000 fta-0.0.5/fta/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)     9865 2024-04-15 09:55:59.000000 fta-0.0.5/fta/main.py
--rw-r--r--   0 voidful    (501) staff       (20)    37165 2024-04-09 07:40:16.000000 fta-0.0.5/fta/pantulipy.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:56:07.965854 fta-0.0.5/fta.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:56:07.000000 fta-0.0.5/fta.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      259 2024-04-15 09:56:07.000000 fta-0.0.5/fta.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-15 09:56:07.000000 fta-0.0.5/fta.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-09 07:53:14.000000 fta-0.0.5/fta.egg-info/not-zip-safe
--rw-r--r--   0 voidful    (501) staff       (20)      109 2024-04-15 09:56:07.000000 fta-0.0.5/fta.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        4 2024-04-15 09:56:07.000000 fta-0.0.5/fta.egg-info/top_level.txt
--rw-r--r--   0 voidful    (501) staff       (20)      108 2024-04-09 07:41:47.000000 fta-0.0.5/requirements.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2024-04-15 09:56:07.966634 fta-0.0.5/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)      744 2024-04-15 09:56:06.000000 fta-0.0.5/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:56:59.680587 fta-0.0.6/
+-rw-r--r--   0 voidful    (501) staff       (20)     4156 2024-04-09 07:40:16.000000 fta-0.0.6/.gitignore
+-rw-r--r--   0 voidful    (501) staff       (20)    11357 2024-04-09 07:40:16.000000 fta-0.0.6/LICENSE
+-rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:56:59.680390 fta-0.0.6/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)    28702 2024-04-09 10:34:05.000000 fta-0.0.6/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:56:59.678418 fta-0.0.6/fta/
+-rw-r--r--   0 voidful    (501) staff       (20)       29 2024-04-09 07:40:16.000000 fta-0.0.6/fta/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)     9848 2024-04-15 09:56:52.000000 fta-0.0.6/fta/main.py
+-rw-r--r--   0 voidful    (501) staff       (20)    37165 2024-04-09 07:40:16.000000 fta-0.0.6/fta/pantulipy.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:56:59.680143 fta-0.0.6/fta.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:56:59.000000 fta-0.0.6/fta.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      259 2024-04-15 09:56:59.000000 fta-0.0.6/fta.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-15 09:56:59.000000 fta-0.0.6/fta.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-09 07:53:14.000000 fta-0.0.6/fta.egg-info/not-zip-safe
+-rw-r--r--   0 voidful    (501) staff       (20)      109 2024-04-15 09:56:59.000000 fta-0.0.6/fta.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        4 2024-04-15 09:56:59.000000 fta-0.0.6/fta.egg-info/top_level.txt
+-rw-r--r--   0 voidful    (501) staff       (20)      108 2024-04-09 07:41:47.000000 fta-0.0.6/requirements.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2024-04-15 09:56:59.680639 fta-0.0.6/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)      744 2024-04-15 09:56:58.000000 fta-0.0.6/setup.py
```

### Comparing `fta-0.0.5/.gitignore` & `fta-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fta-0.0.5/LICENSE` & `fta-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fta-0.0.5/PKG-INFO` & `fta-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fta
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/voidful/FTA
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: finance
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fta-0.0.5/README.md` & `fta-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `fta-0.0.5/fta/main.py` & `fta-0.0.6/fta/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         'kst': ta.kst, 'kurtosis': ta.kurtosis, 'linear_decay': ta.decay,
         'log_return': ta.log_return, 'mad': ta.mad, 'median': ta.median,
         'midpoint': ta.midpoint, 'midprice': ta.midprice,
         'percent_return': ta.percent_return, 'pvol': ta.pvol, 'pvt': ta.pvt,
         'pwma': ta.pwma, 'quantile': ta.quantile, 'rma': ta.rma, 'rvi': ta.rvi,
         'sinwma': ta.sinwma, 'skew': ta.skew, 'slope': ta.slope, 'swma': ta.swma,
         't3': ta.t3, 'tsi': ta.tsi, 'uo': ta.uo, 'variance': ta.variance,
-        'vortex': ta.vortex, 'vwap': ta.vwap, 'zscore': ta.zscore
+        'vortex': ta.vortex, 'zscore': ta.zscore
     }
     pandas_ta_indicators = {
         'accbands': ta.accbands, 'ad': ta.ad, 'adosc': ta.adosc, 'adx': ta.adx,
         'amat': ta.amat, 'ao': ta.ao, 'aobv': ta.aobv, 'apo': ta.apo,
         'aroon': ta.aroon, 'atr': ta.atr, 'bbands': ta.bbands, 'bop': ta.bop,
         'cci': ta.cci, 'cg': ta.cg, 'cmo': ta.cmo,
         'coppock': ta.coppock, 'decreasing': ta.decreasing, 'dema': ta.dema,
```

### Comparing `fta-0.0.5/fta/pantulipy.py` & `fta-0.0.6/fta/pantulipy.py`

 * *Files identical despite different names*

### Comparing `fta-0.0.5/fta.egg-info/PKG-INFO` & `fta-0.0.6/fta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fta
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/voidful/FTA
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: finance
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fta-0.0.5/setup.py` & `fta-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='fta',
-    version='0.0.5',
+    version='0.0.6',
     description='',
     url='https://github.com/voidful/FTA',
     author='Voidful',
     author_email='voidful.stack@gmail.com',
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     setup_requires=['setuptools-git'],
```

