# Comparing `tmp/fta-0.0.3.tar.gz` & `tmp/fta-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fta-0.0.3.tar", last modified: Mon Apr 15 09:51:29 2024, max compression
+gzip compressed data, was "fta-0.0.4.tar", last modified: Mon Apr 15 09:53:11 2024, max compression
```

## Comparing `fta-0.0.3.tar` & `fta-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:51:29.736036 fta-0.0.3/
--rw-r--r--   0 voidful    (501) staff       (20)     4156 2024-04-09 07:40:16.000000 fta-0.0.3/.gitignore
--rw-r--r--   0 voidful    (501) staff       (20)    11357 2024-04-09 07:40:16.000000 fta-0.0.3/LICENSE
--rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:51:29.735885 fta-0.0.3/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)    28702 2024-04-09 10:34:05.000000 fta-0.0.3/README.md
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:51:29.734226 fta-0.0.3/fta/
--rw-r--r--   0 voidful    (501) staff       (20)       29 2024-04-09 07:40:16.000000 fta-0.0.3/fta/__init__.py
--rw-r--r--   0 voidful    (501) staff       (20)     9906 2024-04-15 09:51:17.000000 fta-0.0.3/fta/main.py
--rw-r--r--   0 voidful    (501) staff       (20)    37165 2024-04-09 07:40:16.000000 fta-0.0.3/fta/pantulipy.py
-drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:51:29.735632 fta-0.0.3/fta.egg-info/
--rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:51:29.000000 fta-0.0.3/fta.egg-info/PKG-INFO
--rw-r--r--   0 voidful    (501) staff       (20)      259 2024-04-15 09:51:29.000000 fta-0.0.3/fta.egg-info/SOURCES.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-15 09:51:29.000000 fta-0.0.3/fta.egg-info/dependency_links.txt
--rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-09 07:53:14.000000 fta-0.0.3/fta.egg-info/not-zip-safe
--rw-r--r--   0 voidful    (501) staff       (20)      109 2024-04-15 09:51:29.000000 fta-0.0.3/fta.egg-info/requires.txt
--rw-r--r--   0 voidful    (501) staff       (20)        4 2024-04-15 09:51:29.000000 fta-0.0.3/fta.egg-info/top_level.txt
--rw-r--r--   0 voidful    (501) staff       (20)      108 2024-04-09 07:41:47.000000 fta-0.0.3/requirements.txt
--rw-r--r--   0 voidful    (501) staff       (20)       38 2024-04-15 09:51:29.736192 fta-0.0.3/setup.cfg
--rw-r--r--   0 voidful    (501) staff       (20)      744 2024-04-15 09:51:27.000000 fta-0.0.3/setup.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:53:11.282564 fta-0.0.4/
+-rw-r--r--   0 voidful    (501) staff       (20)     4156 2024-04-09 07:40:16.000000 fta-0.0.4/.gitignore
+-rw-r--r--   0 voidful    (501) staff       (20)    11357 2024-04-09 07:40:16.000000 fta-0.0.4/LICENSE
+-rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:53:11.282291 fta-0.0.4/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)    28702 2024-04-09 10:34:05.000000 fta-0.0.4/README.md
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:53:11.280543 fta-0.0.4/fta/
+-rw-r--r--   0 voidful    (501) staff       (20)       29 2024-04-09 07:40:16.000000 fta-0.0.4/fta/__init__.py
+-rw-r--r--   0 voidful    (501) staff       (20)     9878 2024-04-15 09:53:01.000000 fta-0.0.4/fta/main.py
+-rw-r--r--   0 voidful    (501) staff       (20)    37165 2024-04-09 07:40:16.000000 fta-0.0.4/fta/pantulipy.py
+drwxr-xr-x   0 voidful    (501) staff       (20)        0 2024-04-15 09:53:11.281956 fta-0.0.4/fta.egg-info/
+-rw-r--r--   0 voidful    (501) staff       (20)    29091 2024-04-15 09:53:11.000000 fta-0.0.4/fta.egg-info/PKG-INFO
+-rw-r--r--   0 voidful    (501) staff       (20)      259 2024-04-15 09:53:11.000000 fta-0.0.4/fta.egg-info/SOURCES.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-15 09:53:11.000000 fta-0.0.4/fta.egg-info/dependency_links.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        1 2024-04-09 07:53:14.000000 fta-0.0.4/fta.egg-info/not-zip-safe
+-rw-r--r--   0 voidful    (501) staff       (20)      109 2024-04-15 09:53:11.000000 fta-0.0.4/fta.egg-info/requires.txt
+-rw-r--r--   0 voidful    (501) staff       (20)        4 2024-04-15 09:53:11.000000 fta-0.0.4/fta.egg-info/top_level.txt
+-rw-r--r--   0 voidful    (501) staff       (20)      108 2024-04-09 07:41:47.000000 fta-0.0.4/requirements.txt
+-rw-r--r--   0 voidful    (501) staff       (20)       38 2024-04-15 09:53:11.282674 fta-0.0.4/setup.cfg
+-rw-r--r--   0 voidful    (501) staff       (20)      744 2024-04-15 09:53:09.000000 fta-0.0.4/setup.py
```

### Comparing `fta-0.0.3/.gitignore` & `fta-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fta-0.0.3/LICENSE` & `fta-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fta-0.0.3/PKG-INFO` & `fta-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fta
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/voidful/FTA
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: finance
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fta-0.0.3/README.md` & `fta-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fta-0.0.3/fta/main.py` & `fta-0.0.4/fta/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         Using Tulip indicators and Pandas_TA Indicators.
     """
 
     unique_pandas_ta_indicators = {
         'accbands': ta.accbands, 'amat': ta.amat, 'aobv': ta.aobv,
         'cg': ta.cg, 'coppock': ta.coppock, 'decreasing': ta.decreasing,
         'donchian': ta.donchian, 'efi': ta.efi, 'eom': ta.eom, 'fwma': ta.fwma,
-        'ichimoku': ta.ichimoku, 'increasing': ta.increasing, 'kc': ta.kc,
+        'increasing': ta.increasing, 'kc': ta.kc,
         'kst': ta.kst, 'kurtosis': ta.kurtosis, 'linear_decay': ta.decay,
         'log_return': ta.log_return, 'mad': ta.mad, 'median': ta.median,
         'midpoint': ta.midpoint, 'midprice': ta.midprice,
         'percent_return': ta.percent_return, 'pvol': ta.pvol, 'pvt': ta.pvt,
         'pwma': ta.pwma, 'quantile': ta.quantile, 'rma': ta.rma, 'rvi': ta.rvi,
         'sinwma': ta.sinwma, 'skew': ta.skew, 'slope': ta.slope, 'swma': ta.swma,
         't3': ta.t3, 'tsi': ta.tsi, 'uo': ta.uo, 'variance': ta.variance,
@@ -74,23 +74,23 @@
         'coppock': ta.coppock, 'decreasing': ta.decreasing, 'dema': ta.dema,
         'donchian': ta.donchian, 'dpo': ta.dpo, 'efi': ta.efi, 'ema': ta.ema,
         'eom': ta.eom, 'fisher': ta.fisher, 'fwma': ta.fwma, 'hma': ta.hma,
         'increasing': ta.increasing, 'kama': ta.kama,
         'kc': ta.kc, 'kst': ta.kst, 'kurtosis': ta.kurtosis,
         'log_return': ta.log_return, 'mad': ta.mad, 'massi': ta.massi, 'median': ta.median,
         'midpoint': ta.midpoint, 'midprice': ta.midprice,
-        'mom': ta.mom, 'natr': ta.natr,  'obv': ta.obv, 'ppo': ta.ppo,
+        'mom': ta.mom, 'natr': ta.natr, 'obv': ta.obv, 'ppo': ta.ppo,
         'pvol': ta.pvol, 'pvt': ta.pvt, 'pwma': ta.pwma, 'qstick': ta.qstick,
         'quantile': ta.quantile, 'rma': ta.rma, 'roc': ta.roc, 'rsi': ta.rsi,
         'rvi': ta.rvi, 'sinwma': ta.sinwma, 'skew': ta.skew, 'slope': ta.slope,
-        'sma': ta.sma, 'stdev': ta.stdev,  'swma': ta.swma,
+        'sma': ta.sma, 'stdev': ta.stdev, 'swma': ta.swma,
         't3': ta.t3, 'tema': ta.tema, 'trima': ta.trima, 'trix': ta.trix,
         'true_range': ta.true_range, 'tsi': ta.tsi, 'uo': ta.uo,
         'variance': ta.variance, 'vortex': ta.vortex,
-         'vwma': ta.vwma, 'willr': ta.willr, 'wma': ta.wma,
+        'vwma': ta.vwma, 'willr': ta.willr, 'wma': ta.wma,
         'zlma': ta.zlma, 'zscore': ta.zscore
     }
     unique_pantulipy_indicators = {
         'adxr': adxr, 'aroonosc': aroonosc, 'avgprice': avgprice,
         'cvi': cvi, 'decay': decay, 'di': di, 'dm': dm, 'dx': dx,
         'edecay': edecay, 'emv': emv, 'fosc': fosc, 'kvo': kvo,
         'lag': lag, 'linreg': linreg, 'linregintercept': linregintercept,
```

### Comparing `fta-0.0.3/fta/pantulipy.py` & `fta-0.0.4/fta/pantulipy.py`

 * *Files identical despite different names*

### Comparing `fta-0.0.3/fta.egg-info/PKG-INFO` & `fta-0.0.4/fta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fta
-Version: 0.0.3
+Version: 0.0.4
 Home-page: https://github.com/voidful/FTA
 Author: Voidful
 Author-email: voidful.stack@gmail.com
 License: Apache
 Keywords: finance
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fta-0.0.3/setup.py` & `fta-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='fta',
-    version='0.0.3',
+    version='0.0.4',
     description='',
     url='https://github.com/voidful/FTA',
     author='Voidful',
     author_email='voidful.stack@gmail.com',
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     setup_requires=['setuptools-git'],
```

