# Comparing `tmp/pynumstim-0.2.2b0.tar.gz` & `tmp/pynumstim-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumstim-0.2.2b0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynumstim-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynumstim-0.2.2b0.tar` & `pynumstim-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.2b0/.gitignore
--rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.2b0/LICENSE
--rw-r--r--   0        0        0      624 2024-04-13 13:19:42.020203 pynumstim-0.2.2b0/README.md
--rw-r--r--   0        0        0      363 2024-04-15 14:03:24.122330 pynumstim-0.2.2b0/pynumstim/__init__.py
--rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.2b0/pynumstim/_data_sets.py
--rw-r--r--   0        0        0     6440 2024-04-15 11:49:38.946539 pynumstim-0.2.2b0/pynumstim/_mplist.py
--rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.2b0/pynumstim/_number.py
--rw-r--r--   0        0        0     9404 2024-04-15 14:02:41.097568 pynumstim-0.2.2b0/pynumstim/_problem.py
--rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.2b0/pynumstim/datasets/Ahren_Jackson_79.toml
--rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.2b0/pynumstim/datasets/Lindemann_Tira_10.toml
--rw-r--r--   0        0        0     4513 2024-04-15 13:57:57.608656 pynumstim-0.2.2b0/pynumstim/image.py
--rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.2b0/pyproject.toml
--rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.2b0/trial_list.txt
--rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 pynumstim-0.2.2b0/PKG-INFO
+-rw-r--r--   0        0        0     2751 2024-04-15 13:38:43.853890 pynumstim-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1083 2024-04-13 12:50:27.198971 pynumstim-0.2.3/LICENSE
+-rw-r--r--   0        0        0      624 2024-04-13 13:19:42.020203 pynumstim-0.2.3/README.md
+-rw-r--r--   0        0        0      362 2024-04-15 14:08:26.227585 pynumstim-0.2.3/pynumstim/__init__.py
+-rw-r--r--   0        0        0     2373 2024-04-15 08:50:32.395928 pynumstim-0.2.3/pynumstim/_data_sets.py
+-rw-r--r--   0        0        0     6440 2024-04-15 11:49:38.946539 pynumstim-0.2.3/pynumstim/_mplist.py
+-rw-r--r--   0        0        0     3313 2024-04-15 09:53:32.721596 pynumstim-0.2.3/pynumstim/_number.py
+-rw-r--r--   0        0        0     9404 2024-04-15 14:02:41.097568 pynumstim-0.2.3/pynumstim/_problem.py
+-rw-r--r--   0        0        0      346 2024-04-13 12:50:43.351235 pynumstim-0.2.3/pynumstim/datasets/Ahren_Jackson_79.toml
+-rw-r--r--   0        0        0      726 2024-04-14 14:30:03.628333 pynumstim-0.2.3/pynumstim/datasets/Lindemann_Tira_10.toml
+-rw-r--r--   0        0        0     4513 2024-04-15 13:57:57.608656 pynumstim-0.2.3/pynumstim/image.py
+-rw-r--r--   0        0        0      724 2024-04-15 12:38:06.182596 pynumstim-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0   237189 2024-04-13 13:06:53.547394 pynumstim-0.2.3/trial_list.txt
+-rw-r--r--   0        0        0     1326 1970-01-01 00:00:00.000000 pynumstim-0.2.3/PKG-INFO
```

### Comparing `pynumstim-0.2.2b0/.gitignore` & `pynumstim-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/LICENSE` & `pynumstim-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/README.md` & `pynumstim-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_data_sets.py` & `pynumstim-0.2.3/pynumstim/_data_sets.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_mplist.py` & `pynumstim-0.2.3/pynumstim/_mplist.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_number.py` & `pynumstim-0.2.3/pynumstim/_number.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/_problem.py` & `pynumstim-0.2.3/pynumstim/_problem.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/datasets/Lindemann_Tira_10.toml` & `pynumstim-0.2.3/pynumstim/datasets/Lindemann_Tira_10.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pynumstim/image.py` & `pynumstim-0.2.3/pynumstim/image.py`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/pyproject.toml` & `pynumstim-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/trial_list.txt` & `pynumstim-0.2.3/trial_list.txt`

 * *Files identical despite different names*

### Comparing `pynumstim-0.2.2b0/PKG-INFO` & `pynumstim-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynumstim
-Version: 0.2.2b0
+Version: 0.2.3
 Summary: Python library to create symbolic number and arithmetic stimuli for psychological experiments
 Keywords: experiment control,open science,experimental psychology
 Author-email: Oliver Lindemann <lindemann@essb.eur.nl>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

