# Comparing `tmp/dqc-toolkit-0.1.0b1.tar.gz` & `tmp/dqc_toolkit-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dqc-toolkit-0.1.0b1.tar", last modified: Sat Apr 13 04:47:16 2024, max compression
+gzip compressed data, was "dqc_toolkit-0.1.0b2.tar", last modified: Mon Apr 15 11:57:39 2024, max compression
```

## Comparing `dqc-toolkit-0.1.0b1.tar` & `dqc_toolkit-0.1.0b2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.425813 dqc-toolkit-0.1.0b1/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc-toolkit-0.1.0b1/LICENSE
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2973 2024-04-13 04:47:16.425176 dqc-toolkit-0.1.0b1/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc-toolkit-0.1.0b1/README.md
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.401839 dqc-toolkit-0.1.0b1/dqc/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc-toolkit-0.1.0b1/dqc/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1936 2024-04-12 10:00:13.000000 dqc-toolkit-0.1.0b1/dqc/base.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)    11684 2024-04-12 11:34:46.000000 dqc-toolkit-0.1.0b1/dqc/crossval.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.411610 dqc-toolkit-0.1.0b1/dqc/utils/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      277 2024-04-12 10:00:13.000000 dqc-toolkit-0.1.0b1/dqc/utils/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4893 2024-04-08 10:03:03.000000 dqc-toolkit-0.1.0b1/dqc/utils/_dataprocessing.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7543 2024-04-09 05:35:00.000000 dqc-toolkit-0.1.0b1/dqc/utils/_generic.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3258 2024-04-09 05:35:00.000000 dqc-toolkit-0.1.0b1/dqc/utils/_sklearn_artifacts.py
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.421625 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     2973 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      414 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      306 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/requires.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-13 04:47:16.000000 dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/top_level.txt
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1624 2024-04-13 04:45:15.000000 dqc-toolkit-0.1.0b1/pyproject.toml
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-13 04:47:16.425985 dqc-toolkit-0.1.0b1/setup.cfg
-drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-13 04:47:16.419116 dqc-toolkit-0.1.0b1/tests/
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc-toolkit-0.1.0b1/tests/__init__.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-08 17:00:40.000000 dqc-toolkit-0.1.0b1/tests/conftest.py
--rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3084 2024-04-09 05:33:59.000000 dqc-toolkit-0.1.0b1/tests/test_crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.131095 dqc_toolkit-0.1.0b2/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1070 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b2/LICENSE
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 11:57:39.130379 dqc_toolkit-0.1.0b2/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        4 2024-03-11 14:48:40.000000 dqc_toolkit-0.1.0b2/README.md
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.110712 dqc_toolkit-0.1.0b2/dqc/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       67 2024-04-12 10:00:13.000000 dqc_toolkit-0.1.0b2/dqc/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      585 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/base.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)    14405 2024-04-15 11:55:41.000000 dqc_toolkit-0.1.0b2/dqc/crossval.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.119762 dqc_toolkit-0.1.0b2/dqc/utils/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      329 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     7539 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/_curation.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4894 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/_dataprocessing.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     4680 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/_sanitychecks.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      959 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/dqc/utils/logging.py
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.127744 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     3017 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      431 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        1 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      335 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/requires.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       25 2024-04-15 11:57:39.000000 dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     1659 2024-04-15 11:56:48.000000 dqc_toolkit-0.1.0b2/pyproject.toml
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)       38 2024-04-15 11:57:39.131298 dqc_toolkit-0.1.0b2/setup.cfg
+drwxr-xr-x   0 sumanthprabhu   (501) staff       (20)        0 2024-04-15 11:57:39.126546 dqc_toolkit-0.1.0b2/tests/
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)        0 2024-03-11 16:13:36.000000 dqc_toolkit-0.1.0b2/tests/__init__.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)      252 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/tests/conftest.py
+-rw-r--r--   0 sumanthprabhu   (501) staff       (20)     6078 2024-04-15 11:31:19.000000 dqc_toolkit-0.1.0b2/tests/test_crossval.py
```

### Comparing `dqc-toolkit-0.1.0b1/LICENSE` & `dqc_toolkit-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dqc-toolkit-0.1.0b1/PKG-INFO` & `dqc_toolkit-0.1.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: transformers>=4.39
+Requires-Dist: sentence_transformers>=2.6.1
 Requires-Dist: datasets>=2.18
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: ruff>=0.3.4
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.17; extra == "docs"
 Requires-Dist: mkdocstrings[python]==1.9.2; extra == "docs"
```

### Comparing `dqc-toolkit-0.1.0b1/dqc/crossval.py` & `dqc_toolkit-0.1.0b2/dqc/crossval.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,86 @@
+from typing import List, Tuple, Union
+
+import numpy as np
+import pandas as pd
+from sentence_transformers import SentenceTransformer
+from sklearn.base import ClassifierMixin
+from sklearn.feature_extraction.text import CountVectorizer, TfidfVectorizer
+from sklearn.preprocessing import MinMaxScaler
+from tqdm import tqdm
+
 from dqc.base import BaseCurate
 from dqc.utils import (
     Logger,
-    _get_pipeline,
-    _is_valid,
-    _DataProcessor,
+    SentenceTransformerVectorizer,
     _data_splitter,
+    _DataProcessor,
     _exception_handler,
+    _fetch_curation_artifacts,
+    _get_pipeline,
+    _is_valid,
 )
 
-from sklearn.preprocessing import MinMaxScaler
-from tqdm import tqdm
-import numpy as np
-import pandas as pd
-from typing import Union, List, Tuple
-
 logger = Logger("C2")
 
 tqdm.pandas()
 
 
 class CrossValCurate(BaseCurate):
     """
-
     Args:
+        curate_feature_extractor (Union[str, TfidfVectorizer, CountVectorizer, SentenceTransformer], optional): Feature extraction method to be used during curation. Defaults to 'TfidfVectorizer' (`sklearn.feature_extraction.text.TfidfVectorizer`).
+        curate_model (str, optional): Machine learning model that is trained with `curate_feature_extractor` features during curation. Defaults to 'logistic_regression' (sklearn.linear_model.LogisticRegression).
+        calibration_method (Union[str, None], optional): Approach to be used for calibration of `curate_model` predictions. Defaults to None.
+        correctness_threshold (float, optional): Minimum prediction probability using `curate_model` to consider the corresponding sample as 'correctly labelled'. Defaults to 0.5.
         n_splits (int, optional): Number of splits to use when running cross-validation based curation.
         verbose (bool, optional): Sets the verbosity level during execution. `True` indicates logging level INFO and `False` indicates logging level 'ERROR'.
 
+    Examples:
+    Assuming `data` is a pandas dataframe containing samples with noisy labels, here is how you would use `CrossValCurate` -
+    ```python
+
+    from dqc import CrossValCurate
+
+    cvc = CrossValCurate()
+    data_curated = cvc.fit_transform(data[['text', 'label']])
+    ```
+
+    `data_curated` is a pandas dataframe similar to `data` with the following columns -
+    ```python
+    >>> data_curated.columns
+    ['text', 'label', 'label_correctness_score', 'is_label_correct', 'predicted_label', 'prediction_probability']
+    ```
+
+    `'label_correctness_score'` represents a normalized score quantifying the correctness of `'label'`. \n
+    `'is_label_correct'` is a boolean flag indicating whether the given `'label'` is correct (`True`) or incorrect (`False`). \n
+    `'predicted_label'` and `'prediction_probability'` represent the curation model's prediction and the corresponding probability score.
     """
 
-    def __init__(self, n_splits: int = 5, verbose: bool = False, **options):
+    def __init__(
+        self,
+        curate_feature_extractor: Union[
+            str, TfidfVectorizer, CountVectorizer, SentenceTransformerVectorizer
+        ] = "TfidfVectorizer",
+        curate_model: Union[str, ClassifierMixin] = "logistic_regression",
+        calibration_method: Union[str, None] = "calibrate_using_baseline",
+        correctness_threshold: float = 0.5,
+        n_splits: int = 5,
+        verbose: bool = False,
+        **options,
+    ):
         super().__init__(**options)
+
+        self.curate_feature_extractor, self.curate_model, self.calibration_method = (
+            _fetch_curation_artifacts(
+                curate_feature_extractor, curate_model, calibration_method
+            )
+        )
+
+        self.correctness_threshold = correctness_threshold
         self.n_splits = n_splits
         self.verbose = verbose
         self._set_verbosity(verbose)
 
         self.curate_pipeline = None
         self.scaler = None
         self.y_col_name_int = None
@@ -218,14 +265,17 @@
                 2) Prediction probabilities \n
                 3) An indicator variable `is_label_correct` capturing label correctness
         """
         _is_valid(data_with_noisy_labels, X_col_name, y_col_name)
         n_splits = self.n_splits
         options["num_samples"] = len(data_with_noisy_labels)
 
+        # TBD
+        # 'max_features': min(options["num_samples"] // 10, options.get("max_features", 1000))
+
         logger.info("Pre-processing the data..")
         dp = _DataProcessor(
             random_state=self.random_state,
         )
 
         data_with_noisy_labels, row_id_col, y_col_name_int = dp._preprocess(
             data_with_noisy_labels, y_col_name=y_col_name
@@ -235,15 +285,15 @@
         self.y_col_name_int = y_col_name_int
 
         data_columns = [X_col_name, y_col_name_int]
         logger.info(
             f"Building the curation pipeline with {n_splits}-fold cross validation.."
         )
         self.curate_pipeline = _get_pipeline(
-            self.curate_representation, self.curate_model, **options
+            self.curate_feature_extractor, self.curate_model, **options
         )
 
         split_indices = _data_splitter(
             data_with_noisy_labels,
             X_col_name=X_col_name,
             y_col_name_int=y_col_name_int,
             n_splits=self.n_splits,
```

### Comparing `dqc-toolkit-0.1.0b1/dqc/utils/_dataprocessing.py` & `dqc_toolkit-0.1.0b2/dqc/utils/_dataprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import pandas as pd
-import string
 import random
-from typing import Tuple, List, Union
+import string
+from typing import List, Tuple, Union
+
+import pandas as pd
 from pandas._typing import RandomState
 
 
 class _DataProcessor:
     """Encapsulates data preparation steps pre-curation
     and processing results post-curation."""
```

### Comparing `dqc-toolkit-0.1.0b1/dqc_toolkit.egg-info/PKG-INFO` & `dqc_toolkit-0.1.0b2/dqc_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dqc-toolkit
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Data Quality Check for Machine Learning
 Author-email: Sumanth S Prabhu <sumanthprabhu.104@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 sumanthprabhu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -40,14 +40,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: transformers>=4.39
+Requires-Dist: sentence_transformers>=2.6.1
 Requires-Dist: datasets>=2.18
 Requires-Dist: scikit-learn>=1.3.2
 Requires-Dist: ruff>=0.3.4
 Provides-Extra: docs
 Requires-Dist: mkdocs==1.5.3; extra == "docs"
 Requires-Dist: mkdocs-material==9.5.17; extra == "docs"
 Requires-Dist: mkdocstrings[python]==1.9.2; extra == "docs"
```

### Comparing `dqc-toolkit-0.1.0b1/pyproject.toml` & `dqc_toolkit-0.1.0b2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["setuptools >= 68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dqc-toolkit"
-version = "0.1.0-beta1"
+version = "0.1.0-beta2"
 authors = [
   { name="Sumanth S Prabhu", email="sumanthprabhu.104@gmail.com" },
 ]
 description = "Data Quality Check for Machine Learning"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9"
 dependencies = [
     "transformers>=4.39",
+    "sentence_transformers>=2.6.1",
     "datasets>=2.18",
     "scikit-learn>=1.3.2",
-    "ruff>=0.3.4",
+    "ruff>=0.3.4"
 ]
 keywords = [
   "nlp", 
   "data curation", 
   "machine learning"
 ]
 classifiers = [
```

