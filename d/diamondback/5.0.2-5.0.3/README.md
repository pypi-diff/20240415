# Comparing `tmp/diamondback-5.0.2.tar.gz` & `tmp/diamondback-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diamondback-5.0.2.tar", last modified: Mon Mar 18 18:13:09 2024, max compression
+gzip compressed data, was "diamondback-5.0.3.tar", last modified: Mon Apr 15 19:51:41 2024, max compression
```

## Comparing `diamondback-5.0.2.tar` & `diamondback-5.0.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:09.000718 diamondback-5.0.2/
--rw-rw-rw-   0        0        0      132 2024-03-18 16:07:59.000000 diamondback-5.0.2/.gitignore
--rw-rw-rw-   0        0        0    18406 2024-03-18 18:13:09.000718 diamondback-5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    13177 2024-03-18 18:11:32.000000 diamondback-5.0.2/changelog.rst
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.967400 diamondback-5.0.2/diamondback/
--rw-rw-rw-   0        0        0     1441 2024-03-18 18:10:30.000000 diamondback-5.0.2/diamondback/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.984710 diamondback-5.0.2/diamondback/commons/
--rw-rw-rw-   0        0        0     5712 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/commons/Log.py
--rw-rw-rw-   0        0        0     4467 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/commons/RestClient.py
--rw-rw-rw-   0        0        0     5162 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/commons/Serial.py
--rw-rw-rw-   0        0        0      483 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/commons/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.992718 diamondback-5.0.2/diamondback/filters/
--rw-rw-rw-   0        0        0     4652 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/ComplexBandPassFilter.py
--rw-rw-rw-   0        0        0     2928 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/ComplexExponentialFilter.py
--rw-rw-rw-   0        0        0     5106 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/ComplexFrequencyFilter.py
--rw-rw-rw-   0        0        0     5179 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/DerivativeFilter.py
--rw-rw-rw-   0        0        0    11369 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/FirFilter.py
--rw-rw-rw-   0        0        0     4792 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/GoertzelFilter.py
--rw-rw-rw-   0        0        0    14418 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/IirFilter.py
--rw-rw-rw-   0        0        0     4431 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/IntegralFilter.py
--rw-rw-rw-   0        0        0     3255 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/PidFilter.py
--rw-rw-rw-   0        0        0     5152 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/PolynomialRateFilter.py
--rw-rw-rw-   0        0        0     6731 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/PolyphaseRateFilter.py
--rw-rw-rw-   0        0        0     3352 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/RankFilter.py
--rw-rw-rw-   0        0        0     3729 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/WindowFilter.py
--rw-rw-rw-   0        0        0     1264 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/filters/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.994717 diamondback-5.0.2/diamondback/models/
--rw-rw-rw-   0        0        0     6035 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/models/DiversityModel.py
--rw-rw-rw-   0        0        0     5774 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/models/GaussianMixtureModel.py
--rw-rw-rw-   0        0        0     4591 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/models/GaussianModel.py
--rw-rw-rw-   0        0        0      567 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.996718 diamondback-5.0.2/diamondback/transforms/
--rw-rw-rw-   0        0        0     3903 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/transforms/ComplexTransform.py
--rw-rw-rw-   0        0        0     4116 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/transforms/FourierTransform.py
--rw-rw-rw-   0        0        0     3981 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/transforms/PsdTransform.py
--rw-rw-rw-   0        0        0    18538 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/transforms/WaveletTransform.py
--rw-rw-rw-   0        0        0     5214 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/transforms/ZTransform.py
--rw-rw-rw-   0        0        0      689 2024-03-18 16:07:59.000000 diamondback-5.0.2/diamondback/transforms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.998718 diamondback-5.0.2/diamondback.egg-info/
--rw-rw-rw-   0        0        0    18406 2024-03-18 18:13:08.000000 diamondback-5.0.2/diamondback.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1473 2024-03-18 18:13:08.000000 diamondback-5.0.2/diamondback.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 18:13:08.000000 diamondback-5.0.2/diamondback.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      484 2024-03-18 18:13:08.000000 diamondback-5.0.2/diamondback.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-18 18:13:08.000000 diamondback-5.0.2/diamondback.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1556 2024-03-18 16:07:59.000000 diamondback-5.0.2/license
--rw-rw-rw-   0        0        0     9636 2024-03-18 16:37:29.000000 diamondback-5.0.2/noxfile.py
--rw-rw-rw-   0        0        0     2770 2024-03-18 18:10:19.000000 diamondback-5.0.2/pyproject.toml
--rw-rw-rw-   0        0        0    14585 2024-03-18 16:07:59.000000 diamondback-5.0.2/readme.rst
--rw-rw-rw-   0        0        0       42 2024-03-18 18:13:09.000718 diamondback-5.0.2/setup.cfg
--rw-rw-rw-   0        0        0      382 2024-03-18 16:07:59.000000 diamondback-5.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.944975 diamondback-5.0.2/tests/
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.947989 diamondback-5.0.2/tests/unit/
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.997719 diamondback-5.0.2/tests/unit/commons/
--rw-rw-rw-   0        0        0     3195 2024-03-18 16:07:59.000000 diamondback-5.0.2/tests/unit/commons/test_commons.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.997719 diamondback-5.0.2/tests/unit/filters/
--rw-rw-rw-   0        0        0    20378 2024-03-18 16:07:59.000000 diamondback-5.0.2/tests/unit/filters/test_filters.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.998718 diamondback-5.0.2/tests/unit/models/
--rw-rw-rw-   0        0        0     3750 2024-03-18 16:07:59.000000 diamondback-5.0.2/tests/unit/models/test_models.py
-drwxrwxrwx   0        0        0        0 2024-03-18 18:13:08.998718 diamondback-5.0.2/tests/unit/transforms/
--rw-rw-rw-   0        0        0     8283 2024-03-18 16:07:59.000000 diamondback-5.0.2/tests/unit/transforms/test_transforms.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.143789 diamondback-5.0.3/
+-rw-rw-rw-   0        0        0      132 2024-03-18 16:07:59.000000 diamondback-5.0.3/.gitignore
+-rw-rw-rw-   0        0        0    18355 2024-04-15 19:51:41.142673 diamondback-5.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13177 2024-03-18 18:17:58.000000 diamondback-5.0.3/changelog.rst
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.068570 diamondback-5.0.3/diamondback/
+-rw-rw-rw-   0        0        0     1441 2024-04-15 19:44:38.000000 diamondback-5.0.3/diamondback/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.119672 diamondback-5.0.3/diamondback/commons/
+-rw-rw-rw-   0        0        0     5712 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/commons/Log.py
+-rw-rw-rw-   0        0        0     4467 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/commons/RestClient.py
+-rw-rw-rw-   0        0        0     5162 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/commons/Serial.py
+-rw-rw-rw-   0        0        0      483 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/commons/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.129673 diamondback-5.0.3/diamondback/filters/
+-rw-rw-rw-   0        0        0     4652 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/ComplexBandPassFilter.py
+-rw-rw-rw-   0        0        0     2928 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/ComplexExponentialFilter.py
+-rw-rw-rw-   0        0        0     5106 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/ComplexFrequencyFilter.py
+-rw-rw-rw-   0        0        0     5179 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/DerivativeFilter.py
+-rw-rw-rw-   0        0        0    11369 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/FirFilter.py
+-rw-rw-rw-   0        0        0     4792 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/GoertzelFilter.py
+-rw-rw-rw-   0        0        0    14418 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/IirFilter.py
+-rw-rw-rw-   0        0        0     4431 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/IntegralFilter.py
+-rw-rw-rw-   0        0        0     3255 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/PidFilter.py
+-rw-rw-rw-   0        0        0     5152 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/PolynomialRateFilter.py
+-rw-rw-rw-   0        0        0     6731 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/PolyphaseRateFilter.py
+-rw-rw-rw-   0        0        0     3352 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/RankFilter.py
+-rw-rw-rw-   0        0        0     3729 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/WindowFilter.py
+-rw-rw-rw-   0        0        0     1264 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/filters/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.131672 diamondback-5.0.3/diamondback/models/
+-rw-rw-rw-   0        0        0     6035 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/models/DiversityModel.py
+-rw-rw-rw-   0        0        0     5774 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/models/GaussianMixtureModel.py
+-rw-rw-rw-   0        0        0     4591 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/models/GaussianModel.py
+-rw-rw-rw-   0        0        0      567 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.136673 diamondback-5.0.3/diamondback/transforms/
+-rw-rw-rw-   0        0        0     3903 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/transforms/ComplexTransform.py
+-rw-rw-rw-   0        0        0     4116 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/transforms/FourierTransform.py
+-rw-rw-rw-   0        0        0     3981 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/transforms/PsdTransform.py
+-rw-rw-rw-   0        0        0    18538 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/transforms/WaveletTransform.py
+-rw-rw-rw-   0        0        0     5214 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/transforms/ZTransform.py
+-rw-rw-rw-   0        0        0      689 2024-03-18 16:07:59.000000 diamondback-5.0.3/diamondback/transforms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.141679 diamondback-5.0.3/diamondback.egg-info/
+-rw-rw-rw-   0        0        0    18355 2024-04-15 19:51:41.000000 diamondback-5.0.3/diamondback.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1473 2024-04-15 19:51:41.000000 diamondback-5.0.3/diamondback.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 19:51:41.000000 diamondback-5.0.3/diamondback.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      484 2024-04-15 19:51:41.000000 diamondback-5.0.3/diamondback.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 19:51:41.000000 diamondback-5.0.3/diamondback.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1556 2024-03-18 16:07:59.000000 diamondback-5.0.3/license
+-rw-rw-rw-   0        0        0     9636 2024-03-18 16:37:29.000000 diamondback-5.0.3/noxfile.py
+-rw-rw-rw-   0        0        0     2712 2024-04-15 19:50:55.000000 diamondback-5.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0    14585 2024-03-18 16:07:59.000000 diamondback-5.0.3/readme.rst
+-rw-rw-rw-   0        0        0       42 2024-04-15 19:51:41.143789 diamondback-5.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      382 2024-03-18 16:07:59.000000 diamondback-5.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.048615 diamondback-5.0.3/tests/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.049624 diamondback-5.0.3/tests/unit/
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.139776 diamondback-5.0.3/tests/unit/commons/
+-rw-rw-rw-   0        0        0     3195 2024-03-18 16:07:59.000000 diamondback-5.0.3/tests/unit/commons/test_commons.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.139776 diamondback-5.0.3/tests/unit/filters/
+-rw-rw-rw-   0        0        0    20378 2024-03-18 16:07:59.000000 diamondback-5.0.3/tests/unit/filters/test_filters.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.140672 diamondback-5.0.3/tests/unit/models/
+-rw-rw-rw-   0        0        0     3750 2024-03-18 16:07:59.000000 diamondback-5.0.3/tests/unit/models/test_models.py
+drwxrwxrwx   0        0        0        0 2024-04-15 19:51:41.140672 diamondback-5.0.3/tests/unit/transforms/
+-rw-rw-rw-   0        0        0     8283 2024-03-18 16:07:59.000000 diamondback-5.0.3/tests/unit/transforms/test_transforms.py
```

### Comparing `diamondback-5.0.2/PKG-INFO` & `diamondback-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamondback
-Version: 5.0.2
+Version: 5.0.3
 Summary: diamondback DSP package.
 Author-email: Larry Turner <larry.turner@se.com>
 License: © 2018 - 2024 Schneider Electric Industries SAS. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met :
         
@@ -31,45 +31,44 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/larryturner/diamondback
 Keywords: BSON,DSP,FFT,FIR,GZIP,IIR,JSON,PSD,REST,derivative,diversity,filter,frequency,gaussian,goertzel,integral,log,model,polynomial,polyphase,rate,request,serial,transform,wavelet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.14,>=3.9
 Description-Content-Type: text/x-rst
 License-File: license
 Requires-Dist: jsonpickle<4.0.0,>=3.0.2
-Requires-Dist: loguru<1.0.0,>=0.7.2
+Requires-Dist: loguru<1.0.0,>=0.6.0
 Requires-Dist: numpy<2.0.0,>=1.26.4
-Requires-Dist: pandas<3.0.0,>=2.2.0
+Requires-Dist: pandas<3.0.0,>=2.2.2
 Requires-Dist: requests<3.0.0,>=2.31.0
 Requires-Dist: scikit-learn<2.0.0,>=1.4.0
-Requires-Dist: scipy<2.0.0,>=1.12.0
+Requires-Dist: scipy<2.0.0,>=1.13.0
 Provides-Extra: doc
 Requires-Dist: ipython<9.0.0,>=8.21.0; extra == "doc"
 Requires-Dist: ipywidgets<9.0.0,>=8.1.2; extra == "doc"
 Requires-Dist: jupyter<2.0.0,>=1.0.0; extra == "doc"
-Requires-Dist: matplotlib<4.0.0,>=3.8.2; extra == "doc"
+Requires-Dist: matplotlib<4.0.0,>=3.8.4; extra == "doc"
 Requires-Dist: mypy<2.0.0,>=1.8.0; extra == "doc"
-Requires-Dist: nox<2025.04.22,>=2023.04.22; extra == "doc"
-Requires-Dist: pillow<11.0.0,>=10.2.0; extra == "doc"
-Requires-Dist: pydeps<2.0.0,>=1.12.18; extra == "doc"
+Requires-Dist: nox<2026.04.14,>=2024.04.14; extra == "doc"
+Requires-Dist: pillow<11.0.0,>=10.3.0; extra == "doc"
+Requires-Dist: pydeps<2.0.0,>=1.12.20; extra == "doc"
 Requires-Dist: requests<3.0.0,>=2.31.0; extra == "doc"
 Requires-Dist: sphinx<8.0.0,>=7.2.6; extra == "doc"
 Requires-Dist: sphinx-rtd-theme<3.0.0,>=2.0.0; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pytest<9.0.0,>=8.0.0; extra == "test"
+Requires-Dist: pytest<9.0.0,>=8.1.1; extra == "test"
 Requires-Dist: requests<3.0.0,>=2.31.0; extra == "test"
 
 diamondback
 ===========
 
 .. image:: https://img.shields.io/pypi/pyversions/diamondback.svg?color=steelblue
     :target: https://www.python.org/
```

### Comparing `diamondback-5.0.2/changelog.rst` & `diamondback-5.0.3/changelog.rst`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/__init__.py` & `diamondback-5.0.3/diamondback/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 
 __all__ = [ 'Log', 'RestClient', 'Serial', 'FirFilter',
             'IirFilter', 'ComplexBandPassFilter', 'ComplexExponentialFilter', 'ComplexFrequencyFilter',
             'DerivativeFilter', 'GoertzelFilter', 'IntegralFilter', 'PidFilter',
             'PolynomialRateFilter', 'PolyphaseRateFilter', 'RankFilter', 'WindowFilter',
             'DiversityModel', 'GaussianModel', 'GaussianMixtureModel', 'ComplexTransform',
             'FourierTransform', 'PsdTransform', 'WaveletTransform', 'ZTransform' ]
-__version__ = '5.0.2'
+__version__ = '5.0.3'
```

### Comparing `diamondback-5.0.2/diamondback/commons/Log.py` & `diamondback-5.0.3/diamondback/commons/Log.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/commons/RestClient.py` & `diamondback-5.0.3/diamondback/commons/RestClient.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/commons/Serial.py` & `diamondback-5.0.3/diamondback/commons/Serial.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/ComplexBandPassFilter.py` & `diamondback-5.0.3/diamondback/filters/ComplexBandPassFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/ComplexExponentialFilter.py` & `diamondback-5.0.3/diamondback/filters/ComplexExponentialFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/ComplexFrequencyFilter.py` & `diamondback-5.0.3/diamondback/filters/ComplexFrequencyFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/DerivativeFilter.py` & `diamondback-5.0.3/diamondback/filters/DerivativeFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/FirFilter.py` & `diamondback-5.0.3/diamondback/filters/FirFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/GoertzelFilter.py` & `diamondback-5.0.3/diamondback/filters/GoertzelFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/IirFilter.py` & `diamondback-5.0.3/diamondback/filters/IirFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/IntegralFilter.py` & `diamondback-5.0.3/diamondback/filters/IntegralFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/PidFilter.py` & `diamondback-5.0.3/diamondback/filters/PidFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/PolynomialRateFilter.py` & `diamondback-5.0.3/diamondback/filters/PolynomialRateFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/PolyphaseRateFilter.py` & `diamondback-5.0.3/diamondback/filters/PolyphaseRateFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/RankFilter.py` & `diamondback-5.0.3/diamondback/filters/RankFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/WindowFilter.py` & `diamondback-5.0.3/diamondback/filters/WindowFilter.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/filters/__init__.py` & `diamondback-5.0.3/diamondback/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/models/DiversityModel.py` & `diamondback-5.0.3/diamondback/models/DiversityModel.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/models/GaussianMixtureModel.py` & `diamondback-5.0.3/diamondback/models/GaussianMixtureModel.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/models/GaussianModel.py` & `diamondback-5.0.3/diamondback/models/GaussianModel.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/models/__init__.py` & `diamondback-5.0.3/diamondback/models/__init__.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/transforms/ComplexTransform.py` & `diamondback-5.0.3/diamondback/transforms/ComplexTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/transforms/FourierTransform.py` & `diamondback-5.0.3/diamondback/transforms/FourierTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/transforms/PsdTransform.py` & `diamondback-5.0.3/diamondback/transforms/PsdTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/transforms/WaveletTransform.py` & `diamondback-5.0.3/diamondback/transforms/WaveletTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/transforms/ZTransform.py` & `diamondback-5.0.3/diamondback/transforms/ZTransform.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback/transforms/__init__.py` & `diamondback-5.0.3/diamondback/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/diamondback.egg-info/PKG-INFO` & `diamondback-5.0.3/diamondback.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diamondback
-Version: 5.0.2
+Version: 5.0.3
 Summary: diamondback DSP package.
 Author-email: Larry Turner <larry.turner@se.com>
 License: © 2018 - 2024 Schneider Electric Industries SAS. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met :
         
@@ -31,45 +31,44 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: homepage, https://github.com/larryturner/diamondback
 Keywords: BSON,DSP,FFT,FIR,GZIP,IIR,JSON,PSD,REST,derivative,diversity,filter,frequency,gaussian,goertzel,integral,log,model,polynomial,polyphase,rate,request,serial,transform,wavelet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: <3.13,>=3.8
+Requires-Python: <3.14,>=3.9
 Description-Content-Type: text/x-rst
 License-File: license
 Requires-Dist: jsonpickle<4.0.0,>=3.0.2
-Requires-Dist: loguru<1.0.0,>=0.7.2
+Requires-Dist: loguru<1.0.0,>=0.6.0
 Requires-Dist: numpy<2.0.0,>=1.26.4
-Requires-Dist: pandas<3.0.0,>=2.2.0
+Requires-Dist: pandas<3.0.0,>=2.2.2
 Requires-Dist: requests<3.0.0,>=2.31.0
 Requires-Dist: scikit-learn<2.0.0,>=1.4.0
-Requires-Dist: scipy<2.0.0,>=1.12.0
+Requires-Dist: scipy<2.0.0,>=1.13.0
 Provides-Extra: doc
 Requires-Dist: ipython<9.0.0,>=8.21.0; extra == "doc"
 Requires-Dist: ipywidgets<9.0.0,>=8.1.2; extra == "doc"
 Requires-Dist: jupyter<2.0.0,>=1.0.0; extra == "doc"
-Requires-Dist: matplotlib<4.0.0,>=3.8.2; extra == "doc"
+Requires-Dist: matplotlib<4.0.0,>=3.8.4; extra == "doc"
 Requires-Dist: mypy<2.0.0,>=1.8.0; extra == "doc"
-Requires-Dist: nox<2025.04.22,>=2023.04.22; extra == "doc"
-Requires-Dist: pillow<11.0.0,>=10.2.0; extra == "doc"
-Requires-Dist: pydeps<2.0.0,>=1.12.18; extra == "doc"
+Requires-Dist: nox<2026.04.14,>=2024.04.14; extra == "doc"
+Requires-Dist: pillow<11.0.0,>=10.3.0; extra == "doc"
+Requires-Dist: pydeps<2.0.0,>=1.12.20; extra == "doc"
 Requires-Dist: requests<3.0.0,>=2.31.0; extra == "doc"
 Requires-Dist: sphinx<8.0.0,>=7.2.6; extra == "doc"
 Requires-Dist: sphinx-rtd-theme<3.0.0,>=2.0.0; extra == "doc"
 Provides-Extra: test
-Requires-Dist: pytest<9.0.0,>=8.0.0; extra == "test"
+Requires-Dist: pytest<9.0.0,>=8.1.1; extra == "test"
 Requires-Dist: requests<3.0.0,>=2.31.0; extra == "test"
 
 diamondback
 ===========
 
 .. image:: https://img.shields.io/pypi/pyversions/diamondback.svg?color=steelblue
     :target: https://www.python.org/
```

### Comparing `diamondback-5.0.2/diamondback.egg-info/SOURCES.txt` & `diamondback-5.0.3/diamondback.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/license` & `diamondback-5.0.3/license`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/noxfile.py` & `diamondback-5.0.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/pyproject.toml` & `diamondback-5.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 [ project ]
 authors = [ { name = 'Larry Turner', email = 'larry.turner@se.com' } ]
 classifiers = [ 'Development Status :: 5 - Production/Stable',
                 'Operating System :: OS Independent',
                 'Programming Language :: Python :: 3',
-                'Programming Language :: Python :: 3.8',
                 'Programming Language :: Python :: 3.9',
                 'Programming Language :: Python :: 3.10',
                 'Programming Language :: Python :: 3.11',
                 'Programming Language :: Python :: 3.12',
                 'Programming Language :: Python :: 3.13',
                 'License :: OSI Approved :: BSD License' ]
 dependencies = [ 'jsonpickle >= 3.0.2, < 4.0.0',
-                 'loguru >= 0.7.2, < 1.0.0',
+                 'loguru >= 0.6.0, < 1.0.0',
                  'numpy >= 1.26.4, < 2.0.0',
-                 'pandas >= 2.2.0, < 3.0.0',
+                 'pandas >= 2.2.2, < 3.0.0',
                  'requests >= 2.31.0, < 3.0.0',
                  'scikit-learn >= 1.4.0, < 2.0.0',
-                 'scipy >= 1.12.0, < 2.0.0' ]
+                 'scipy >= 1.13.0, < 2.0.0' ]
 description = 'diamondback DSP package.'
 keywords = [ 'BSON',
              'DSP',
              'FFT',
              'FIR',
              'GZIP',
              'IIR',
@@ -42,40 +41,40 @@
              'request',
              'serial',
              'transform',
              'wavelet' ]
 license = { file = 'license' }
 name = 'diamondback'
 readme = 'readme.rst'
-requires-python = '>= 3.8, < 3.13'
-version = '5.0.2'
+requires-python = '>= 3.9, < 3.14'
+version = '5.0.3'
 
 [ project.optional-dependencies ]
 doc = [ 'ipython >= 8.21.0, < 9.0.0',
         'ipywidgets >= 8.1.2, < 9.0.0',
         'jupyter >= 1.0.0, < 2.0.0',
-        'matplotlib >= 3.8.2, < 4.0.0',
+        'matplotlib >= 3.8.4, < 4.0.0',
         'mypy >= 1.8.0, < 2.0.0',
-        'nox >= 2023.04.22, < 2025.04.22',
-        'pillow >= 10.2.0, < 11.0.0',
-        'pydeps >= 1.12.18, < 2.0.0',
+        'nox >= 2024.04.14, < 2026.04.14',
+        'pillow >= 10.3.0, < 11.0.0',
+        'pydeps >= 1.12.20, < 2.0.0',
         'requests >= 2.31.0, < 3.0.0',
         'sphinx >= 7.2.6, < 8.0.0',
         'sphinx-rtd-theme >= 2.0.0, < 3.0.0' ]
-test = [ 'pytest >= 8.0.0, < 9.0.0',
+test = [ 'pytest >= 8.1.1, < 9.0.0',
          'requests >= 2.31.0, < 3.0.0' ]
 
 [ project.urls ]
 homepage = 'https://github.com/larryturner/diamondback'
 
 [ build-system ]
 build-backend = 'setuptools.build_meta'
-requires = [ 'build >= 1.0.3, < 2.0.0',
+requires = [ 'build >= 1.2.1, < 2.0.0',
              'requests >= 2.31.0, < 3.0.0',
-             'setuptools >= 69.0.3, < 70.0.0',
-             'wheel >= 0.42.0, < 1.0.0' ]
+             'setuptools >= 69.5.1, < 70.0.0',
+             'wheel >= 0.43.0, < 1.0.0' ]
 
 [ tool.setuptools.packages.find ]
 include = [ 'diamondback*' ]
 
 [ tool.mypy ]
 ignore_missing_imports = true
```

### Comparing `diamondback-5.0.2/readme.rst` & `diamondback-5.0.3/readme.rst`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/tests/unit/commons/test_commons.py` & `diamondback-5.0.3/tests/unit/commons/test_commons.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/tests/unit/filters/test_filters.py` & `diamondback-5.0.3/tests/unit/filters/test_filters.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/tests/unit/models/test_models.py` & `diamondback-5.0.3/tests/unit/models/test_models.py`

 * *Files identical despite different names*

### Comparing `diamondback-5.0.2/tests/unit/transforms/test_transforms.py` & `diamondback-5.0.3/tests/unit/transforms/test_transforms.py`

 * *Files identical despite different names*

