# Comparing `tmp/series_intro_recognizer-0.1.0b0.tar.gz` & `tmp/series_intro_recognizer-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "series_intro_recognizer-0.1.0b0.tar", last modified: Mon Apr 15 21:16:23 2024, max compression
+gzip compressed data, was "series_intro_recognizer-1.0.0.tar", last modified: Mon Apr 15 21:00:09 2024, max compression
```

## Comparing `series_intro_recognizer-0.1.0b0.tar` & `series_intro_recognizer-1.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.974873 series_intro_recognizer-0.1.0b0/
--rw-rw-rw-   0        0        0     1074 2024-04-15 20:59:09.000000 series_intro_recognizer-0.1.0b0/LICENSE
--rw-rw-rw-   0        0        0     3720 2024-04-15 21:16:23.970873 series_intro_recognizer-0.1.0b0/PKG-INFO
--rw-rw-rw-   0        0        0     3188 2024-04-15 20:51:48.000000 series_intro_recognizer-0.1.0b0/README.md
--rw-rw-rw-   0        0        0      614 2024-04-15 21:16:00.000000 series_intro_recognizer-0.1.0b0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.965870 series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/
--rw-rw-rw-   0        0        0     3720 2024-04-15 21:16:23.000000 series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      923 2024-04-15 21:16:23.000000 series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 21:16:23.000000 series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-15 21:16:23.000000 series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.913837 series_intro_recognizer-0.1.0b0/series_opening_recognizer/
--rw-rw-rw-   0        0        0      269 2024-04-13 10:41:54.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/__init__.py
--rw-rw-rw-   0        0        0     2657 2024-04-14 15:44:08.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/config.py
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.917837 series_intro_recognizer-0.1.0b0/series_opening_recognizer/helpers/
--rw-rw-rw-   0        0        0     1885 2024-04-12 18:45:43.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/helpers/cached_iterator.py
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.925839 series_intro_recognizer-0.1.0b0/series_opening_recognizer/processors/
--rw-rw-rw-   0        0        0     1578 2024-04-14 21:12:07.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/processors/audio_files.py
--rw-rw-rw-   0        0        0     5694 2024-04-14 22:18:24.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/processors/audio_samples.py
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.931840 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/
--rw-rw-rw-   0        0        0      496 2024-04-14 14:05:51.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/best_offset_finder.py
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.947353 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/
--rw-rw-rw-   0        0        0     1754 2024-04-14 15:54:14.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/async_correlator.py
--rw-rw-rw-   0        0        0     2161 2024-04-15 08:31:21.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/correlator.py
--rw-rw-rw-   0        0        0     2375 2024-04-14 15:54:46.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/fragments_normalizer.py
--rw-rw-rw-   0        0        0     2022 2024-04-14 15:51:47.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/sync_correlator.py
--rw-rw-rw-   0        0        0     1561 2024-04-14 22:06:38.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/offsets_calculator.py
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.955874 series_intro_recognizer-0.1.0b0/series_opening_recognizer/tp/
--rw-rw-rw-   0        0        0      104 2024-04-12 00:01:01.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/tp/interval.py
--rw-rw-rw-   0        0        0      284 2024-04-11 22:53:32.000000 series_intro_recognizer-0.1.0b0/series_opening_recognizer/tp/tp.py
--rw-rw-rw-   0        0        0       42 2024-04-15 21:16:23.974873 series_intro_recognizer-0.1.0b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-15 21:16:23.960872 series_intro_recognizer-0.1.0b0/tests/
--rw-rw-rw-   0        0        0      728 2024-04-14 22:23:15.000000 series_intro_recognizer-0.1.0b0/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.399002 series_intro_recognizer-1.0.0/
+-rw-rw-rw-   0        0        0     1074 2024-04-15 20:59:09.000000 series_intro_recognizer-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     3718 2024-04-15 21:00:09.395002 series_intro_recognizer-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3188 2024-04-15 20:51:48.000000 series_intro_recognizer-1.0.0/README.md
+-rw-rw-rw-   0        0        0      609 2024-04-15 21:00:00.000000 series_intro_recognizer-1.0.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.392004 series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/
+-rw-rw-rw-   0        0        0     3718 2024-04-15 21:00:09.000000 series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      923 2024-04-15 21:00:09.000000 series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 21:00:09.000000 series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-15 21:00:09.000000 series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.272456 series_intro_recognizer-1.0.0/series_opening_recognizer/
+-rw-rw-rw-   0        0        0      269 2024-04-13 10:41:54.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/__init__.py
+-rw-rw-rw-   0        0        0     2657 2024-04-14 15:44:08.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/config.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.275455 series_intro_recognizer-1.0.0/series_opening_recognizer/helpers/
+-rw-rw-rw-   0        0        0     1885 2024-04-12 18:45:43.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/helpers/cached_iterator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.294454 series_intro_recognizer-1.0.0/series_opening_recognizer/processors/
+-rw-rw-rw-   0        0        0     1578 2024-04-14 21:12:07.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/processors/audio_files.py
+-rw-rw-rw-   0        0        0     5694 2024-04-14 22:18:24.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/processors/audio_samples.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.301456 series_intro_recognizer-1.0.0/series_opening_recognizer/services/
+-rw-rw-rw-   0        0        0      496 2024-04-14 14:05:51.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/services/best_offset_finder.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.339971 series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/
+-rw-rw-rw-   0        0        0     1754 2024-04-14 15:54:14.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/async_correlator.py
+-rw-rw-rw-   0        0        0     2161 2024-04-15 08:31:21.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/correlator.py
+-rw-rw-rw-   0        0        0     2375 2024-04-14 15:54:46.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/fragments_normalizer.py
+-rw-rw-rw-   0        0        0     2022 2024-04-14 15:51:47.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/sync_correlator.py
+-rw-rw-rw-   0        0        0     1561 2024-04-14 22:06:38.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/services/offsets_calculator.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.370484 series_intro_recognizer-1.0.0/series_opening_recognizer/tp/
+-rw-rw-rw-   0        0        0      104 2024-04-12 00:01:01.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/tp/interval.py
+-rw-rw-rw-   0        0        0      284 2024-04-11 22:53:32.000000 series_intro_recognizer-1.0.0/series_opening_recognizer/tp/tp.py
+-rw-rw-rw-   0        0        0       42 2024-04-15 21:00:09.399002 series_intro_recognizer-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 21:00:09.383484 series_intro_recognizer-1.0.0/tests/
+-rw-rw-rw-   0        0        0      728 2024-04-14 22:23:15.000000 series_intro_recognizer-1.0.0/tests/test_main.py
```

### Comparing `series_intro_recognizer-0.1.0b0/LICENSE` & `series_intro_recognizer-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/PKG-INFO` & `series_intro_recognizer-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: series_intro_recognizer
-Version: 0.1.0b0
+Version: 1.0.0
 Summary: Find the intro of episodes of a series
 Author: HRAshton
 Project-URL: Homepage, https://github.com/HRAshton/SeriesIntroRecognizer
 Project-URL: Issues, https://github.com/HRAshton/SeriesIntroRecognizer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `series_intro_recognizer-0.1.0b0/README.md` & `series_intro_recognizer-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/pyproject.toml` & `series_intro_recognizer-1.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "series_intro_recognizer"
-version = "0.1.0-beta"
+version = "1.0.0"
 authors = [
     { name = "HRAshton" },
 ]
 description = "Find the intro of episodes of a series"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/PKG-INFO` & `series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: series_intro_recognizer
-Version: 0.1.0b0
+Version: 1.0.0
 Summary: Find the intro of episodes of a series
 Author: HRAshton
 Project-URL: Homepage, https://github.com/HRAshton/SeriesIntroRecognizer
 Project-URL: Issues, https://github.com/HRAshton/SeriesIntroRecognizer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `series_intro_recognizer-0.1.0b0/series_intro_recognizer.egg-info/SOURCES.txt` & `series_intro_recognizer-1.0.0/series_intro_recognizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/config.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/config.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/helpers/cached_iterator.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/helpers/cached_iterator.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/processors/audio_files.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/processors/audio_files.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/processors/audio_samples.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/processors/audio_samples.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/async_correlator.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/async_correlator.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/correlator.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/correlator.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/fragments_normalizer.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/fragments_normalizer.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/correlator/sync_correlator.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/services/correlator/sync_correlator.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/series_opening_recognizer/services/offsets_calculator.py` & `series_intro_recognizer-1.0.0/series_opening_recognizer/services/offsets_calculator.py`

 * *Files identical despite different names*

### Comparing `series_intro_recognizer-0.1.0b0/tests/test_main.py` & `series_intro_recognizer-1.0.0/tests/test_main.py`

 * *Files identical despite different names*

