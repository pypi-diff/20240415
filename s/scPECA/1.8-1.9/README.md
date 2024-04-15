# Comparing `tmp/scPECA-1.8.tar.gz` & `tmp/scPECA-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scPECA-1.8.tar", last modified: Wed Jan 31 05:19:02 2024, max compression
+gzip compressed data, was "dist/scPECA-1.9.tar", last modified: Wed Jan 31 05:30:28 2024, max compression
```

## Comparing `scPECA-1.8.tar` & `scPECA-1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 amss      (1009) student   (1007)        0 2024-01-31 05:19:02.000000 scPECA-1.8/
--rw-r--r--   0 amss      (1009) student   (1007)     1091 2024-01-30 19:06:21.000000 scPECA-1.8/LICENSE
--rw-r--r--   0 amss      (1009) student   (1007)     3413 2024-01-31 05:19:02.000000 scPECA-1.8/PKG-INFO
--rw-r--r--   0 amss      (1009) student   (1007)     3227 2024-01-30 19:06:21.000000 scPECA-1.8/README.md
-drwxr-xr-x   0 amss      (1009) student   (1007)        0 2024-01-31 05:19:02.000000 scPECA-1.8/scPECA/
--rw-r--r--   0 amss      (1009) student   (1007)     7159 2024-01-31 04:30:15.000000 scPECA-1.8/scPECA/PECA_network.py
--rw-r--r--   0 amss      (1009) student   (1007)        1 2024-01-30 19:06:21.000000 scPECA-1.8/scPECA/__init__.py
--rw-r--r--   0 amss      (1009) student   (1007)     1744 2024-01-30 19:06:21.000000 scPECA-1.8/scPECA/homer_motifinding.py
--rw-r--r--   0 amss      (1009) student   (1007)     1903 2024-01-30 19:06:21.000000 scPECA-1.8/scPECA/mf_collect.py
--rw-r--r--   0 amss      (1009) student   (1007)     2408 2024-01-30 19:06:21.000000 scPECA-1.8/scPECA/mfbs.py
--rw-r--r--   0 amss      (1009) student   (1007)     4707 2024-01-30 19:06:21.000000 scPECA-1.8/scPECA/preprocessing.py
--rw-r--r--   0 amss      (1009) student   (1007)      285 2024-01-31 05:17:55.000000 scPECA-1.8/scPECA/prior_install.py
--rw-r--r--   0 amss      (1009) student   (1007)     6178 2024-01-30 19:06:21.000000 scPECA-1.8/scPECA/scPECA.py
-drwxr-xr-x   0 amss      (1009) student   (1007)        0 2024-01-31 05:19:02.000000 scPECA-1.8/scPECA.egg-info/
--rw-r--r--   0 amss      (1009) student   (1007)     3413 2024-01-31 05:19:02.000000 scPECA-1.8/scPECA.egg-info/PKG-INFO
--rw-r--r--   0 amss      (1009) student   (1007)      317 2024-01-31 05:19:02.000000 scPECA-1.8/scPECA.egg-info/SOURCES.txt
--rw-r--r--   0 amss      (1009) student   (1007)        1 2024-01-31 05:19:02.000000 scPECA-1.8/scPECA.egg-info/dependency_links.txt
--rw-r--r--   0 amss      (1009) student   (1007)        7 2024-01-31 05:19:02.000000 scPECA-1.8/scPECA.egg-info/top_level.txt
--rw-r--r--   0 amss      (1009) student   (1007)       38 2024-01-31 05:19:02.000000 scPECA-1.8/setup.cfg
--rw-r--r--   0 amss      (1009) student   (1007)     2889 2024-01-31 05:18:50.000000 scPECA-1.8/setup.py
+drwxr-xr-x   0 amss      (1009) student   (1007)        0 2024-01-31 05:30:28.000000 scPECA-1.9/
+-rw-r--r--   0 amss      (1009) student   (1007)     1091 2024-01-30 19:06:21.000000 scPECA-1.9/LICENSE
+-rw-r--r--   0 amss      (1009) student   (1007)     3413 2024-01-31 05:30:28.000000 scPECA-1.9/PKG-INFO
+-rw-r--r--   0 amss      (1009) student   (1007)     3227 2024-01-30 19:06:21.000000 scPECA-1.9/README.md
+drwxr-xr-x   0 amss      (1009) student   (1007)        0 2024-01-31 05:30:28.000000 scPECA-1.9/scPECA/
+-rw-r--r--   0 amss      (1009) student   (1007)     7159 2024-01-31 04:30:15.000000 scPECA-1.9/scPECA/PECA_network.py
+-rw-r--r--   0 amss      (1009) student   (1007)        1 2024-01-30 19:06:21.000000 scPECA-1.9/scPECA/__init__.py
+-rw-r--r--   0 amss      (1009) student   (1007)     1744 2024-01-30 19:06:21.000000 scPECA-1.9/scPECA/homer_motifinding.py
+-rw-r--r--   0 amss      (1009) student   (1007)     1903 2024-01-30 19:06:21.000000 scPECA-1.9/scPECA/mf_collect.py
+-rw-r--r--   0 amss      (1009) student   (1007)     2408 2024-01-30 19:06:21.000000 scPECA-1.9/scPECA/mfbs.py
+-rw-r--r--   0 amss      (1009) student   (1007)     4707 2024-01-30 19:06:21.000000 scPECA-1.9/scPECA/preprocessing.py
+-rw-r--r--   0 amss      (1009) student   (1007)     1649 2024-01-31 05:28:59.000000 scPECA-1.9/scPECA/prior_install.py
+-rw-r--r--   0 amss      (1009) student   (1007)     6213 2024-01-31 05:25:05.000000 scPECA-1.9/scPECA/scPECA.py
+drwxr-xr-x   0 amss      (1009) student   (1007)        0 2024-01-31 05:30:28.000000 scPECA-1.9/scPECA.egg-info/
+-rw-r--r--   0 amss      (1009) student   (1007)     3413 2024-01-31 05:30:28.000000 scPECA-1.9/scPECA.egg-info/PKG-INFO
+-rw-r--r--   0 amss      (1009) student   (1007)      317 2024-01-31 05:30:28.000000 scPECA-1.9/scPECA.egg-info/SOURCES.txt
+-rw-r--r--   0 amss      (1009) student   (1007)        1 2024-01-31 05:30:28.000000 scPECA-1.9/scPECA.egg-info/dependency_links.txt
+-rw-r--r--   0 amss      (1009) student   (1007)        7 2024-01-31 05:30:28.000000 scPECA-1.9/scPECA.egg-info/top_level.txt
+-rw-r--r--   0 amss      (1009) student   (1007)       38 2024-01-31 05:30:28.000000 scPECA-1.9/setup.cfg
+-rw-r--r--   0 amss      (1009) student   (1007)     2889 2024-01-31 05:26:01.000000 scPECA-1.9/setup.py
```

### Comparing `scPECA-1.8/LICENSE` & `scPECA-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/PKG-INFO` & `scPECA-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scPECA
-Version: 1.8
+Version: 1.9
 Summary: PECA2 gene regulatory network construction for single-cell data
 Home-page: https://github.com/zhangjiahao1234/scPECA
 Author: Jiahao Zhang
 Author-email: zhangjiahao@amss.ac.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scPECA Version: 1.8 Summary: PECA2 gene regulatory
+Metadata-Version: 2.1 Name: scPECA Version: 1.9 Summary: PECA2 gene regulatory
 network construction for single-cell data Home-page: https://github.com/
 zhangjiahao1234/scPECA Author: Jiahao Zhang Author-email:
 zhangjiahao@amss.ac.cn License: UNKNOWN Platform: UNKNOWN Description-Content-
 Type: text/markdown License-File: LICENSE # scPECA ## Introduction This is a
 python version of PECA2 gene regulatory network construction software designed
 for single-cell data. It has a faster running speed and a lower memory
 footprint. ## Installation ```commandline pip install scPECA ``` Or install via
```

### Comparing `scPECA-1.8/README.md` & `scPECA-1.9/README.md`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/scPECA/PECA_network.py` & `scPECA-1.9/scPECA/PECA_network.py`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/scPECA/homer_motifinding.py` & `scPECA-1.9/scPECA/homer_motifinding.py`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/scPECA/mf_collect.py` & `scPECA-1.9/scPECA/mf_collect.py`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/scPECA/mfbs.py` & `scPECA-1.9/scPECA/mfbs.py`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/scPECA/preprocessing.py` & `scPECA-1.9/scPECA/preprocessing.py`

 * *Files identical despite different names*

### Comparing `scPECA-1.8/scPECA/scPECA.py` & `scPECA-1.9/scPECA/scPECA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import pandas as pd
-from PECA_network import GRN
-from preprocessing import CPM, FPKM, RNA_process_mode_1, RNA_process_mode_2, RNA_process_mode_3, ATAC_process_mode_1, ATAC_process_mode_2, ATAC_process_mode_3
-from homer_motifinding import Split, Homer, Homer_prior, MotifFind
-from mf_collect import mf_collect
-from mfbs import mfbs, mfbs_c
+from scPECA.PECA_network import GRN
+from scPECA.preprocessing import CPM, FPKM, RNA_process_mode_1, RNA_process_mode_2, RNA_process_mode_3, ATAC_process_mode_1, ATAC_process_mode_2, ATAC_process_mode_3
+from scPECA.homer_motifinding import Split, Homer, Homer_prior, MotifFind
+from scPECA.mf_collect import mf_collect
+from scPECA.mfbs import mfbs, mfbs_c
 import pybedtools
 import subprocess
 
 
 class scPECA:
     def __init__(self, path, sample_name, genome):
         self.path = path
```

### Comparing `scPECA-1.8/scPECA.egg-info/PKG-INFO` & `scPECA-1.9/scPECA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scPECA
-Version: 1.8
+Version: 1.9
 Summary: PECA2 gene regulatory network construction for single-cell data
 Home-page: https://github.com/zhangjiahao1234/scPECA
 Author: Jiahao Zhang
 Author-email: zhangjiahao@amss.ac.cn
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: scPECA Version: 1.8 Summary: PECA2 gene regulatory
+Metadata-Version: 2.1 Name: scPECA Version: 1.9 Summary: PECA2 gene regulatory
 network construction for single-cell data Home-page: https://github.com/
 zhangjiahao1234/scPECA Author: Jiahao Zhang Author-email:
 zhangjiahao@amss.ac.cn License: UNKNOWN Platform: UNKNOWN Description-Content-
 Type: text/markdown License-File: LICENSE # scPECA ## Introduction This is a
 python version of PECA2 gene regulatory network construction software designed
 for single-cell data. It has a faster running speed and a lower memory
 footprint. ## Installation ```commandline pip install scPECA ``` Or install via
```

### Comparing `scPECA-1.8/setup.py` & `scPECA-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='scPECA',
-    version='1.8',
+    version='1.9',
     author='Jiahao Zhang',
     author_email='zhangjiahao@amss.ac.cn',
     description='PECA2 gene regulatory network construction for single-cell data',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/zhangjiahao1234/scPECA',
     packages=find_packages(),
```

