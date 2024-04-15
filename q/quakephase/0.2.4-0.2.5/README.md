# Comparing `tmp/quakephase-0.2.4.tar.gz` & `tmp/quakephase-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quakephase-0.2.4.tar", last modified: Fri Feb 16 05:56:57 2024, max compression
+gzip compressed data, was "quakephase-0.2.5.tar", last modified: Sun Apr 14 19:57:20 2024, max compression
```

## Comparing `quakephase-0.2.4.tar` & `quakephase-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-02-16 05:56:57.094858 quakephase-0.2.4/
--rw-rw-r--   0 peidong   (1000) peidong   (1000)    35149 2023-09-10 08:01:40.000000 quakephase-0.2.4/LICENSE
--rw-rw-r--   0 peidong   (1000) peidong   (1000)       48 2023-09-16 10:25:00.000000 quakephase-0.2.4/MANIFEST.in
--rw-r--r--   0 peidong   (1000) peidong   (1000)      435 2024-02-16 05:56:57.094858 quakephase-0.2.4/PKG-INFO
--rw-rw-r--   0 peidong   (1000) peidong   (1000)      221 2023-09-13 11:39:45.000000 quakephase-0.2.4/README.md
-drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-02-16 05:56:57.090858 quakephase-0.2.4/example_data/
--rw-rw-r--   0 peidong   (1000) peidong   (1000)   136192 2023-10-13 14:23:43.000000 quakephase-0.2.4/example_data/example_2C_LAK24.MSEED
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     1169 2023-12-12 13:09:43.000000 quakephase-0.2.4/parameters.yaml
-drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-02-16 05:56:57.094858 quakephase-0.2.4/quakephase/
--rw-rw-r--   0 peidong   (1000) peidong   (1000)      217 2024-02-01 16:13:30.000000 quakephase-0.2.4/quakephase/__init__.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     4435 2023-10-25 18:50:18.000000 quakephase-0.2.4/quakephase/load_MLmodel.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)    11298 2023-12-10 13:18:07.000000 quakephase-0.2.4/quakephase/pfinput.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     9819 2024-02-15 21:15:09.000000 quakephase-0.2.4/quakephase/quakephase.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     7945 2024-02-01 16:40:57.000000 quakephase-0.2.4/quakephase/streamprocess.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     6296 2024-02-15 21:27:10.000000 quakephase-0.2.4/quakephase/utilplot.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     9496 2024-02-01 16:42:10.000000 quakephase-0.2.4/quakephase/xpick.py
--rw-rw-r--   0 peidong   (1000) peidong   (1000)     8486 2023-12-10 13:18:07.000000 quakephase-0.2.4/quakephase/xprob.py
-drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-02-16 05:56:57.094858 quakephase-0.2.4/quakephase.egg-info/
--rw-r--r--   0 peidong   (1000) peidong   (1000)      435 2024-02-16 05:56:57.000000 quakephase-0.2.4/quakephase.egg-info/PKG-INFO
--rw-rw-r--   0 peidong   (1000) peidong   (1000)      447 2024-02-16 05:56:57.000000 quakephase-0.2.4/quakephase.egg-info/SOURCES.txt
--rw-rw-r--   0 peidong   (1000) peidong   (1000)        1 2024-02-16 05:56:57.000000 quakephase-0.2.4/quakephase.egg-info/dependency_links.txt
--rw-rw-r--   0 peidong   (1000) peidong   (1000)       30 2024-02-16 05:56:57.000000 quakephase-0.2.4/quakephase.egg-info/requires.txt
--rw-rw-r--   0 peidong   (1000) peidong   (1000)       11 2024-02-16 05:56:57.000000 quakephase-0.2.4/quakephase.egg-info/top_level.txt
--rw-rw-r--   0 peidong   (1000) peidong   (1000)       38 2024-02-16 05:56:57.094858 quakephase-0.2.4/setup.cfg
--rw-rw-r--   0 peidong   (1000) peidong   (1000)      584 2024-02-15 21:40:48.000000 quakephase-0.2.4/setup.py
+drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-04-14 19:57:20.070126 quakephase-0.2.5/
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)    35149 2023-09-10 08:01:40.000000 quakephase-0.2.5/LICENSE
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)       48 2023-09-16 10:25:00.000000 quakephase-0.2.5/MANIFEST.in
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     2619 2024-04-14 19:57:20.070126 quakephase-0.2.5/PKG-INFO
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     1881 2024-04-14 19:43:02.000000 quakephase-0.2.5/README.md
+drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-04-14 19:57:20.070126 quakephase-0.2.5/example_data/
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)   136192 2023-10-13 14:23:43.000000 quakephase-0.2.5/example_data/example_2C_LAK24.MSEED
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     1209 2024-03-20 20:43:33.000000 quakephase-0.2.5/parameters.yaml
+drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-04-14 19:57:20.070126 quakephase-0.2.5/quakephase/
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)      217 2024-02-01 16:13:30.000000 quakephase-0.2.5/quakephase/__init__.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     4435 2023-10-25 18:50:18.000000 quakephase-0.2.5/quakephase/load_MLmodel.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)    11298 2023-12-10 13:18:07.000000 quakephase-0.2.5/quakephase/pfinput.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)    10231 2024-04-06 03:42:39.000000 quakephase-0.2.5/quakephase/quakephase.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     7945 2024-02-01 16:40:57.000000 quakephase-0.2.5/quakephase/streamprocess.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     6296 2024-02-15 21:27:10.000000 quakephase-0.2.5/quakephase/utilplot.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     9496 2024-02-01 16:42:10.000000 quakephase-0.2.5/quakephase/xpick.py
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)     8486 2023-12-10 13:18:07.000000 quakephase-0.2.5/quakephase/xprob.py
+drwxrwxr-x   0 peidong   (1000) peidong   (1000)        0 2024-04-14 19:57:20.070126 quakephase-0.2.5/quakephase.egg-info/
+-rw-r--r--   0 peidong   (1000) peidong   (1000)     2619 2024-04-14 19:57:20.000000 quakephase-0.2.5/quakephase.egg-info/PKG-INFO
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)      447 2024-04-14 19:57:20.000000 quakephase-0.2.5/quakephase.egg-info/SOURCES.txt
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)        1 2024-04-14 19:57:20.000000 quakephase-0.2.5/quakephase.egg-info/dependency_links.txt
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)       30 2024-04-14 19:57:20.000000 quakephase-0.2.5/quakephase.egg-info/requires.txt
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)       11 2024-04-14 19:57:20.000000 quakephase-0.2.5/quakephase.egg-info/top_level.txt
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)       38 2024-04-14 19:57:20.070126 quakephase-0.2.5/setup.cfg
+-rw-rw-r--   0 peidong   (1000) peidong   (1000)      802 2024-04-14 19:48:24.000000 quakephase-0.2.5/setup.py
```

### Comparing `quakephase-0.2.4/LICENSE` & `quakephase-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/example_data/example_2C_LAK24.MSEED` & `quakephase-0.2.5/example_data/example_2C_LAK24.MSEED`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/parameters.yaml` & `quakephase-0.2.5/parameters.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 MLmodel:
     - SeisBench,PhaseNet,original
     # - SeisBench,PhaseNet,stead
     - SeisBench,EQT,original
     # - SeisBench,EQT,stead
     
-overlap_ratio: 0.95
+overlap_ratio: 0.9
     
 rescaling: 
     - None
     - 2 
     - 3
     - 4
     - 5
     # - 0.5
-    # - 4.5
+    # - 0.2
+    # - 0.1
+    # - 0.05
+    # - 8.5
     
 frequency: 
     - None  # no filtering
     - [1, 40]
     - [2, 40]  # bandpass filtering
     - [5, None]  # highpass filtering
 
@@ -29,14 +32,14 @@
     P_threshold: 0.1  # None or number
     S_threshold: 0.1  # None or number
 
 output: all  # pick or prob
 
 prob_sampling_rate: None  # None or float/int
 
-data:  # specify the input seismic data information 
-    component_input: Z12  # the input data component(s), only required if the input data format is numpy.ndarray
-    # auto_expend: 
-    #     method: symmetric  # method to auto expend the input data if input duration is too short, can be constant or symmetric ... (check numpy.pad)
-    #     window_ratio: 2.0  # the ratio of the expended window size to the required input duration, 1.0 means the same size
+# data:  # specify the input seismic data information 
+#     component_input: Z12  # the input data component(s), only required if the input data format is numpy.ndarray
+#     auto_expend: 
+#         method: symmetric  # method to auto expend the input data if input duration is too short, can be constant or symmetric ... (check numpy.pad)
+#         window_ratio: 2.0  # the ratio of the expended window size to the required input duration, 1.0 means the same size
```

### Comparing `quakephase-0.2.4/quakephase/load_MLmodel.py` & `quakephase-0.2.5/quakephase/load_MLmodel.py`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/quakephase/pfinput.py` & `quakephase-0.2.5/quakephase/pfinput.py`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/quakephase/quakephase.py` & `quakephase-0.2.5/quakephase/quakephase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 from .load_MLmodel import load_MLmodel
 from .xprob import prob_ensemble
-from .streamprocess import stfilter, check_compile_stream, array2stream, expend_trace
+from .streamprocess import stfilter, check_compile_stream, array2stream, expend_trace, sbresample
 from .pfinput import load_check_input
 from .xpick import get_picks
 import obspy
 import seisbench.util as sbu
 import pandas as pd
 import numpy as np
 from obspy import UTCDateTime
@@ -182,26 +182,32 @@
             del stream_ft
     
     Nfreq = len(paras['frequency'])  # total number of frequency ranges
     assert(len(probs_all)==len(phasemodels)*Nfreq)
 
     if len(probs_all) == 1:
         prob = probs_all[0]
+        if paras['prob_sampling_rate'] is not None:
+            # resample prob to the set frequency sampling_rate
+            sbresample(stream=prob, sampling_rate=paras['prob_sampling_rate'])
     else:
         # remove potential empty prob_streams
         for iprob in probs_all:
             for itrace in iprob:
                 if (itrace.count()==0): iprob.remove(itrace)
         probs_all = [iprob for iprob in probs_all if iprob.count()>0]
 
         if len(probs_all) > 1:            
             # aggregate results from different models/predictions
             prob = prob_ensemble(probs_all=probs_all, method=paras['ensemble'], sampling_rate=paras['prob_sampling_rate'])
         else:
             prob = probs_all[0]
+            if paras['prob_sampling_rate'] is not None:
+                # resample prob to the set frequency sampling_rate
+                sbresample(stream=prob, sampling_rate=paras['prob_sampling_rate'])
 
     ioutput = {}
     if (paras['output'].lower() == 'prob') or (paras['output'].lower() == 'all'):
         ioutput['prob'] = prob
 
     if (paras['output'].lower() == 'pick') or (paras['output'].lower() == 'all'):
         # get picks
```

### Comparing `quakephase-0.2.4/quakephase/streamprocess.py` & `quakephase-0.2.5/quakephase/streamprocess.py`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/quakephase/utilplot.py` & `quakephase-0.2.5/quakephase/utilplot.py`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/quakephase/xpick.py` & `quakephase-0.2.5/quakephase/xpick.py`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/quakephase/xprob.py` & `quakephase-0.2.5/quakephase/xprob.py`

 * *Files identical despite different names*

### Comparing `quakephase-0.2.4/setup.py` & `quakephase-0.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup, find_packages
+from pathlib import Path
+
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='quakephase',
-    version='0.2.4',
+    version='0.2.5',
     packages=find_packages(),
     author='Peidong Shi',
     author_email="speedshi@hotmail.com",
     description="A Python package for automatic seismic phase characterization",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     url="https://github.com/speedshi/quakephase",
     license="GPLv3",
     keywords="Seismology, Machine Learning, Phase Picking, Seismic Monitoring, Earthquake Monitoring",
     install_requires=[
         'seisbench',
         'pyyaml',
         'scikit-learn',
         # Add any other dependencies here
     ],
-)
+)
```

