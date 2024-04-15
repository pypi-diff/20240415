# Comparing `tmp/hsr-0.1.7.tar.gz` & `tmp/hsr-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsr-0.1.7.tar", last modified: Wed Apr 10 12:15:10 2024, max compression
+gzip compressed data, was "hsr-0.1.8.tar", last modified: Mon Apr 15 09:19:55 2024, max compression
```

## Comparing `hsr-0.1.7.tar` & `hsr-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 12:15:10.083486 hsr-0.1.7/
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 12:15:10.065306 hsr-0.1.7/HSR/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 hsr-0.1.7/HSR/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 hsr-0.1.7/HSR/fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 hsr-0.1.7/HSR/hsr_cli.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 hsr-0.1.7/HSR/pca_transform.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 hsr-0.1.7/HSR/pre_processing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 hsr-0.1.7/HSR/similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 hsr-0.1.7/HSR/utils.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-10 12:11:15.000000 hsr-0.1.7/HSR/version.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 12:15:10.082021 hsr-0.1.7/HSR.egg-info/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-10 12:15:06.000000 hsr-0.1.7/HSR.egg-info/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)      779 2024-04-10 12:15:07.000000 hsr-0.1.7/HSR.egg-info/SOURCES.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-10 12:15:06.000000 hsr-0.1.7/HSR.egg-info/dependency_links.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-10 12:15:06.000000 hsr-0.1.7/HSR.egg-info/entry_points.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-10 12:15:06.000000 hsr-0.1.7/HSR.egg-info/requires.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)        4 2024-04-10 12:15:07.000000 hsr-0.1.7/HSR.egg-info/top_level.txt
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 hsr-0.1.7/LICENSE
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 hsr-0.1.7/MANIFEST.in
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-10 12:15:10.082839 hsr-0.1.7/PKG-INFO
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 hsr-0.1.7/README.md
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-10 12:15:10.083573 hsr-0.1.7/setup.cfg
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1018 2024-04-10 12:14:01.000000 hsr-0.1.7/setup.py
-drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-10 12:15:10.081441 hsr-0.1.7/tests/
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 hsr-0.1.7/tests/__init__.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 hsr-0.1.7/tests/test_fingerprint.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 hsr-0.1.7/tests/test_pca.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 hsr-0.1.7/tests/test_preprocessing.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 hsr-0.1.7/tests/test_similarity.py
--rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 hsr-0.1.7/tests/test_utils.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:55.140887 hsr-0.1.8/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)    34523 2024-02-21 11:44:17.000000 hsr-0.1.8/LICENSE
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       33 2024-04-09 12:22:09.000000 hsr-0.1.8/MANIFEST.in
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-15 09:19:55.138908 hsr-0.1.8/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1712 2024-02-28 12:10:43.000000 hsr-0.1.8/README.md
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:54.697943 hsr-0.1.8/hsr/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      180 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     7806 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4761 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/hsr_cli.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9745 2024-03-07 09:58:34.000000 hsr-0.1.8/hsr/pca_transform.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     4342 2024-03-07 09:57:05.000000 hsr-0.1.8/hsr/pre_processing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     9553 2024-03-20 12:00:09.000000 hsr-0.1.8/hsr/similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3830 2024-02-21 11:44:17.000000 hsr-0.1.8/hsr/utils.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      229 2024-04-15 09:19:26.000000 hsr-0.1.8/hsr/version.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:55.136671 hsr-0.1.8/hsr.egg-info/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1931 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/PKG-INFO
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)      476 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/SOURCES.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        1 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/dependency_links.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       41 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/entry_points.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       18 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/requires.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)        4 2024-04-15 09:19:54.000000 hsr-0.1.8/hsr.egg-info/top_level.txt
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       38 2024-04-15 09:19:55.141155 hsr-0.1.8/setup.cfg
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1018 2024-04-10 12:14:01.000000 hsr-0.1.8/setup.py
+drwxr-xr-x   0 marcellocostamagna   (501) staff       (20)        0 2024-04-15 09:19:55.132587 hsr-0.1.8/tests/
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)       17 2024-03-07 14:03:24.000000 hsr-0.1.8/tests/__init__.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     3230 2024-03-07 14:03:14.000000 hsr-0.1.8/tests/test_fingerprint.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1320 2024-03-07 14:03:15.000000 hsr-0.1.8/tests/test_pca.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     5315 2024-03-07 14:03:16.000000 hsr-0.1.8/tests/test_preprocessing.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     2241 2024-03-07 14:03:18.000000 hsr-0.1.8/tests/test_similarity.py
+-rw-r--r--   0 marcellocostamagna   (501) staff       (20)     1562 2024-03-07 14:03:20.000000 hsr-0.1.8/tests/test_utils.py
```

### Comparing `hsr-0.1.7/HSR/fingerprint.py` & `hsr-0.1.8/hsr/fingerprint.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/HSR/hsr_cli.py` & `hsr-0.1.8/hsr/hsr_cli.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/HSR/pca_transform.py` & `hsr-0.1.8/hsr/pca_transform.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/HSR/pre_processing.py` & `hsr-0.1.8/hsr/pre_processing.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/HSR/similarity.py` & `hsr-0.1.8/hsr/similarity.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/HSR/utils.py` & `hsr-0.1.8/hsr/utils.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/HSR.egg-info/PKG-INFO` & `hsr-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsr
-Version: 0.1.7
+Version: 0.1.8
 Author: Marcello Costamagna
 License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
```

### Comparing `hsr-0.1.7/LICENSE` & `hsr-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/PKG-INFO` & `hsr-0.1.8/hsr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hsr
-Version: 0.1.7
+Version: 0.1.8
 Author: Marcello Costamagna
 License: AGPL-3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: rdkit
```

### Comparing `hsr-0.1.7/README.md` & `hsr-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/setup.py` & `hsr-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/tests/test_fingerprint.py` & `hsr-0.1.8/tests/test_fingerprint.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/tests/test_pca.py` & `hsr-0.1.8/tests/test_pca.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/tests/test_preprocessing.py` & `hsr-0.1.8/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/tests/test_similarity.py` & `hsr-0.1.8/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `hsr-0.1.7/tests/test_utils.py` & `hsr-0.1.8/tests/test_utils.py`

 * *Files identical despite different names*

