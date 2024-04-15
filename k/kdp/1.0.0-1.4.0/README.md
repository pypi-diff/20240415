# Comparing `tmp/kdp-1.0.0.tar.gz` & `tmp/kdp-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kdp-1.0.0.tar", max compression
+gzip compressed data, was "kdp-1.4.0.tar", max compression
```

## Comparing `kdp-1.0.0.tar` & `kdp-1.4.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1073 2024-03-08 19:22:44.009498 kdp-1.0.0/LICENSE
--rw-r--r--   0        0        0     3392 2024-03-14 13:58:44.450251 kdp-1.0.0/README.md
--rw-r--r--   0        0        0      524 2024-03-14 14:11:46.135384 kdp-1.0.0/kdp/__init__.py
--rw-r--r--   0        0        0   146582 2024-03-13 12:31:09.025181 kdp-1.0.0/kdp/debug.ipynb
--rw-r--r--   0        0        0     3822 2024-03-13 12:28:37.022431 kdp-1.0.0/kdp/layers_factory.py
--rw-r--r--   0        0        0     3491 2024-03-14 14:09:29.699377 kdp-1.0.0/kdp/pipeline.py
--rw-r--r--   0        0        0    16317 2024-03-13 12:31:25.398335 kdp-1.0.0/kdp/processor.py
--rw-r--r--   0        0        0    16345 2024-03-11 16:35:28.162501 kdp-1.0.0/kdp/stats.py
--rw-r--r--   0        0        0     4015 2024-03-14 15:01:55.135876 kdp-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4073 1970-01-01 00:00:00.000000 kdp-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-15 11:27:26.891808 kdp-1.4.0/LICENSE
+-rw-r--r--   0        0        0     3851 2024-04-15 11:27:26.891808 kdp-1.4.0/README.md
+-rw-r--r--   0        0        0   102413 2024-04-15 11:27:26.899808 kdp-1.4.0/docs/kdp_logo.png
+-rw-r--r--   0        0        0      668 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/__init__.py
+-rw-r--r--   0        0        0     2632 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/custom_layers.py
+-rw-r--r--   0        0        0     5046 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/features.py
+-rw-r--r--   0        0        0     8096 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/layers_factory.py
+-rw-r--r--   0        0        0     3322 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/pipeline.py
+-rw-r--r--   0        0        0    26344 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/processor.py
+-rw-r--r--   0        0        0    11967 2024-04-15 11:27:26.899808 kdp-1.4.0/kdp/stats.py
+-rw-r--r--   0        0        0     4034 2024-04-15 11:28:49.564487 kdp-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4532 1970-01-01 00:00:00.000000 kdp-1.4.0/PKG-INFO
```

### Comparing `kdp-1.0.0/LICENSE` & `kdp-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kdp-1.0.0/README.md` & `kdp-1.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,88 +1,119 @@
-# 🚀 Welcome to Keras Data Processor: Unleash Preprocessing Power with TensorFlow Keras!
+Metadata-Version: 2.1
+Name: kdp
+Version: 1.4.0
+Summary: Data Preprocessing model based on Keras preprocessing layers
+Home-page: https://github.com/piotrlaczkowski/keras-data-processor
+Author: piotrlaczkowski
+Author-email: piotr.laczkowski@gmail.com
+Requires-Python: >=3.11,<3.12
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: loguru (>=0.6.0)
+Requires-Dist: numpy (>=1.23)
+Requires-Dist: tensorflow (>=2.11)
+Project-URL: Documentation, http://piotrlaczkowski.github.io/keras-data-processor/
+Project-URL: Repository, https://github.com/piotrlaczkowski/keras-data-processor
+Description-Content-Type: text/markdown
+
+# 🌟 Welcome to Keras Data Processor (KDP) - Preprocessing Power with TensorFlow Keras 🌟
 
 <p align="center">
   <img src="docs/kdp_logo.png" width="350"/>
 </p>
 
-**Embark on a Data Preprocessing Adventure!**
+** Welcome to the Future of Data Preprocessing!**
 
-Venture into the thrilling realm of machine learning and data science with ease! 🌌 We're thrilled to introduce an advanced data preprocessing model that harnesses the power of TensorFlow Keras and its innovative preprocessing layers.
+Diving into the world of machine learning and data science, we often find ourselves tangled in the preprocessing jungle.
+Worry no more! Introducing a state-of-the-art data preprocessing model based on TensorFlow Keras and the innovative use of Keras preprocessing layers.
 
-Bid farewell to the drudgery of data prep and embrace a world where data pipelines are not only streamlined but also efficient and scalable. Whether you're a battle-tested data warrior or a budding data enthusiast, our toolkit is engineered to amplify your ML endeavors, propelling your workflows to unprecedented speeds and robustness!
+Say goodbye to tedious data preparation tasks and hello to streamlined, efficient, and scalable data pipelines. Whether you're a seasoned data scientist or just starting out, this tool is designed to supercharge your ML workflows, making them more robust and faster than ever!
 
-## 🌟 Stellar Features:
+## 🔑 Key Features:
 
-- **Automated Feature Engineering**: Watch in awe as our tool deftly navigates through your dataset, intuitively applying the perfect preprocessing maneuvers for each feature type.
+- Automated Feature Engineering: Automatically detects and applies the optimal preprocessing steps for each feature type in your dataset.
 
-- **Tailor-Made Preprocessing Pipelines**: Craft your preprocessing odyssey with unparalleled ease, selecting from a vast universe of options for numeric, categorical, and the intricate dance of feature crosses.
+- Customizable Preprocessing Pipelines: Tailor your preprocessing steps with ease, choosing from a wide range of options for numeric, categorical, and even complex feature crosses.
 
-- **Galactic Scalability and Efficiency**: Built for the performance-hungry, our model effortlessly devours large datasets, all thanks to TensorFlow's might.
+- Scalability and Efficiency: Designed for performance, handling large datasets with ease thanks to TensorFlow's powerful backend.
 
-- **Seamless Integration**: Merge seamlessly into the TensorFlow Keras cosmos, transitioning from raw data to a fully-trained model at warp speed.
+- Easy Integration: Seamlessly fits into your TensorFlow Keras models (as first layers of the mode), making it a breeze to go from raw data to trained model faster than ever.
 
-## 🚀 Getting Started:
+## 🚀 Getting started:
 
-Embarking with us requires the installation of poetry for dependency management. Here's how you can set sail:
+We use poetry for handling dependencies so you will need to install it first.
+Then you can install the dependencies by running:
 
-### Install Dependencies:
+To install dependencies:
 
 ```bash
 poetry install
 ```
 
-### Enter the Poetry Shell:
+or to enter a dedicated env directly:
 
 ```bash
 poetry shell
 ```
 
-### Configure Your Preprocessor:
+Then you can simply configure your preprocessor:
+
+## 🛠️ Building Preprocessor:
 
 ```python
-from kdp import PreprocessingModel, FeatureType
+from kdp import PreprocessingModel
+from kdp import FeatureType
 
-# DEFINING THE STARS OF YOUR DATA GALAXY
-features_spec = {
-    "num_1": FeatureType.FLOAT,
-    "num_2": "float",
-    "cat_1": FeatureType.STRING_CATEGORICAL,
-    "cat_2": FeatureType.INTEGER_CATEGORICAL,
+# DEFINING FEATURES PROCESSORS
+features_specs = {
+    # ======= NUMERICAL Features =========================
+    "feat1": FeatureType.FLOAT_NORMALIZED,
+    "feat2": FeatureType.FLOAT_RESCALED,
+    # ======= CATEGORICAL Features ========================
+    "feat3": FeatureType.STRING_CATEGORICAL,
+    "feat4": FeatureType.INTEGER_CATEGORICAL,
+    # ======= TEXT Features ========================
+    "feat5": FeatureType.TEXT,
 }
 
-# BRINGING YOUR PREPROCESSOR TO LIFE
+# INSTANTIATE THE PREPROCESSING MODEL with your data
 ppr = PreprocessingModel(
     path_data="data/my_data.csv",
     features_specs=features_spec,
 )
-# Forging the preprocessing pipelines
+# construct the preprocessing pipelines
 ppr.build_preprocessor()
 ```
 
-### The Marvelous Output:
+This wil output:
 
 ```JS
 {
-    'model': <Functional name=preprocessor, built=True>,
-    'inputs': {
-        'num_1': <KerasTensor shape=(None, 1), dtype=float32, name=num_1>,
-        'num_2': <KerasTensor shape=(None, 1), dtype=float32, name=num_2>,
-        'cat_1': <KerasTensor shape=(None, 1), dtype=string, name=cat_1>
-        'cat_2': <KerasTensor shape=(None, 1), dtype=int32, name=cat_2>,
+'model': <Functional name=preprocessor, built=True>,
+'inputs': {
+    'feat1': <KerasTensor shape=(None, 1), dtype=float32, sparse=None, name=feat1>,
+    'feat2': <KerasTensor shape=(None, 1), dtype=float32, sparse=None, name=feat2>,
+    'feat3': <KerasTensor shape=(None, 1), dtype=string, sparse=None, name=feat3>,
+    'feat4': <KerasTensor shape=(None, 1), dtype=int32, sparse=None, name=feat4>,
+    'feat5': <KerasTensor shape=(None, 1), dtype=string, sparse=None, name=feat5>
     },
-    'signature': {...},
-    'output_dims': 9
+'signature': {
+    'feat1': TensorSpec(shape=(None, 1), dtype=tf.float32, name='feat1'),
+    'feat2': TensorSpec(shape=(None, 1), dtype=tf.float32, name='feat2'),
+    'feat3': TensorSpec(shape=(None, 1), dtype=tf.string, name='feat3'),
+    'feat4': TensorSpec(shape=(None, 1), dtype=tf.int32, name='feat4'),
+    'feat5': TensorSpec(shape=(None, 1), dtype=tf.string, name='feat5')
+    },
+'output_dims': 45
 }
 ```
 
-### Seamlessly Integrate into Your Keras Model:
+This will result in the following preprocessing steps:
 
-```python
-class FunctionalModelWithPreprocessing(tf.keras.Model):
-    # Your adventure with a fully integrated preprocessing model begins here...
-```
+<p align="center">
+  <img src="docs/imgs/Model_Architecture.png" width="800"/>
+</p>
 
-## 🌠 Dive Deeper:
+## 🔍 Dive Deeper:
 
-Journey through our comprehensive documentation to exploit the full might of this preprocessing toolkit. Delve into the art of feature crosses, bucketization strategies, and uncovering the mysteries of embedding sizes to craft the perfect preprocessing pipeline for your celestial quest.
+Explore the detailed documentation to leverage the full potential of this preprocessing tool. Learn about customizing feature crosses, bucketization strategies, embedding sizes, and much more to truly tailor your preprocessing pipeline to your project's needs.
 
-Embark on this exhilarating adventure with us and redefine the boundaries of machine learning. Let's turn your data preprocessing dreams into reality! 🚀
```

### Comparing `kdp-1.0.0/kdp/pipeline.py` & `kdp-1.4.0/kdp/pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,106 +2,96 @@
 
 import tensorflow as tf
 from loguru import logger
 
 
 class ProcessingStep:
     def __init__(self, layer_creator: Callable[..., tf.keras.layers.Layer], **layer_kwargs) -> None:
-        """Initialize a processing step."""
+        """Initialize a processing step.
+
+        Args:
+            layer_creator (Callable[..., tf.keras.layers.Layer]): A callable that creates a layer.
+            **layer_kwargs: Additional keyword arguments for the layer creator.
+        """
         self.layer = layer_creator(**layer_kwargs)
 
     def process(self, input_data) -> tf.keras.layers.Layer:
         """Apply the processing step to the input data.
 
         Args:
-            input_data: The input data to be processed.
+            input_data: The input data to process.
         """
         return self.layer(input_data)
 
     def connect(self, input_layer) -> tf.keras.layers.Layer:
-        """Connect this step's layer to an input layer and return the output layer."""
+        """Connect this step's layer to an input layer and return the output layer.
+
+        Args:
+            input_layer: The input layer to connect to.
+        """
         return self.layer(input_layer)
 
     @property
-    def name(self) -> object:
+    def name(self) -> str:
         """Return the name of the layer."""
-        return self.layer
+        return self.layer.name
 
 
 class Pipeline:
     def __init__(self, steps: list[ProcessingStep] = None, name: str = "") -> None:
         """Initialize a pipeline with a list of processing steps.
 
         Args:
-            steps: A list of processing steps.
-            name: The name of the pipeline.
+            steps (list[ProcessingStep]): A list of processing steps.
+            name (str): The name of the pipeline.
         """
         logger.info(f"🔂 Initializing New Pipeline for: {name}")
         self.steps = steps or []
 
     def add_step(self, step: ProcessingStep) -> None:
         """Add a processing step to the pipeline.
 
         Args:
-            step: A processing step.
+            step (ProcessingStep): The processing step to add.
         """
         logger.info(f"Adding new preprocessing layer: {step.name} to the pipeline ➕")
         self.steps.append(step)
 
-    def apply(self, input_data) -> tf.data.Dataset:
-        """Apply the pipeline to the input data.
-
-        Args:
-            input_data: The input data to be processed.
-
-        """
-        for step in self.steps:
-            input_data = step.process(input_data=input_data)
-        return input_data
-
     def chain(self, input_layer) -> tf.keras.layers.Layer:
         """Chain the pipeline steps by connecting each step in sequence, starting from the input layer.
 
         Args:
-            input_layer: The input layer to start the chain.
+            input_layer: The input layer to start the chain from.
         """
         output_layer = input_layer
         for step in self.steps:
             output_layer = step.connect(output_layer)
         return output_layer
 
 
 class FeaturePreprocessor:
     def __init__(self, name: str) -> None:
         """Initialize a feature preprocessor.
 
         Args:
-            name: The name of the feature preprocessor.
+            name (str): The name of the feature preprocessor.
         """
         self.name = name
         self.pipeline = Pipeline(name=name)
 
     def add_processing_step(self, layer_creator: Callable[..., tf.keras.layers.Layer], **layer_kwargs) -> None:
         """Add a processing step to the feature preprocessor.
 
         Args:
-            layer_creator: A callable that creates a Keras layer.
-            layer_kwargs: Keyword arguments to be passed to the layer creator.
+            layer_creator (Callable[..., tf.keras.layers.Layer]): A callable that creates a layer.
+            **layer_kwargs: Additional keyword arguments for the layer creator.
         """
         step = ProcessingStep(layer_creator=layer_creator, **layer_kwargs)
         self.pipeline.add_step(step=step)
 
-    def preprocess(self, input_data) -> tf.data.Dataset:
-        """Apply the feature preprocessor to the input data.
-
-        Args:
-            input_data: The input data to be processed.
-        """
-        return self.pipeline.apply(input_data)
-
     def chain(self, input_layer) -> tf.keras.layers.Layer:
         """Chain the preprocessor's pipeline steps starting from the input layer.
 
         Args:
-            input_layer: The input layer to start the chain.
+            input_layer: The input layer to start the chain from.
         """
         return self.pipeline.chain(input_layer)
```

### Comparing `kdp-1.0.0/kdp/stats.py` & `kdp-1.4.0/kdp/stats.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,16 @@
 import json
-from enum import Enum
 from pathlib import Path
 from typing import Any
 
 import numpy as np
 import tensorflow as tf
 from loguru import logger
 
-
-class FeatureType(Enum):
-    """Enum for the different types of features supported by the statistics calculator."""
-
-    FLOAT = "float"
-    INTEGER_CATEGORICAL = "integer_categorical"
-    STRING_CATEGORICAL = "string_categorical"
+from kdp.features import CategoricalFeature, FeatureType, NumericalFeature
 
 
 class WelfordAccumulator:
     """Accumulator for computing the mean and variance of a sequence of numbers
     using the Welford algorithm (streaming data).
     """
 
@@ -108,83 +101,48 @@
         return tf.unique(all_values)[0].numpy().tolist()
 
 
 class DatasetStatistics:
     def __init__(
         self,
         path_data: str,
-        numeric_cols: list[str] = None,
-        categorical_cols: list[str] = None,
         features_specs: dict[str, FeatureType | str] = None,
+        numeric_features: list[NumericalFeature] = None,
+        categorical_features: list[CategoricalFeature] = None,
         features_stats_path: Path = None,
         overwrite_stats: bool = False,
         batch_size: int = 50_000,
     ) -> None:
         """Initializes the statistics accumulators for numeric and categorical features.
 
         Args:
             path_data: Path to the folder containing the CSV files.
             batch_size: The batch size to use when reading data from the dataset.
-            numeric_cols: List of numeric feature names (defaults to None).
-            categorical_cols: List of categorical feature names (defaults to None).
             features_stats_path: Path to the features statistics JSON file (defaults to None).
             overwrite_stats: Whether or not to overwrite existing statistics file (defaults to False).
             features_specs:
                 A dictionary mapping feature names to feature specifications (defaults to None).
                 Easier alternative to proviginh numerical and categorical lists.
+            numeric_features: A list of numerical features to calculate statistics for (defaults to None).
+            categorical_features: A list of categorical features to calculate statistics for (defaults to None).
         """
         self.path_data = path_data
-        self.numeric_cols = numeric_cols or []
-        self.categorical_cols = categorical_cols or []
+        self.numeric_features = numeric_features or []
+        self.categorical_features = categorical_features or []
         self.features_specs = features_specs or {}
         self.features_stats_path = features_stats_path or "features_stats.json"
         self.overwrite_stats = overwrite_stats
         self.batch_size = batch_size
 
         # placeholders
         self.features_dtypes = {}
 
-        # checkinng if we have feature specs or numerical and categorical columns
-        if not (numeric_cols or categorical_cols):
-            if not features_specs:
-                raise ValueError("You must provide either numeric_cols and/or categorical_cols or features_specs 🚨")
-            # extracting info from feature scope
-            self._parse_features_specs()
-
-        if not features_specs and not (numeric_cols or categorical_cols):
-            raise ValueError("You must provide either numeric_cols and/or categorical_cols OR features_specs 🚨")
-
         # Initializing placeholders for statistics
-        self.numeric_stats = {col: WelfordAccumulator() for col in self.numeric_cols}
-        self.categorical_stats = {col: CategoricalAccumulator() for col in self.categorical_cols}
-
-    def _parse_features_specs(self) -> None:
-        """Parses the features specifications and updates the numeric and categorical columns accordingly."""
-        logger.info("Parsing features specifications ...")
-        for feature, spec in self.features_specs.items():
-            # Ensure spec is always the string representation, whether it's an enum member or a string
-            spec_value = spec if isinstance(spec, str) else spec.value
-            logger.debug(f"Processing {feature =} with {spec_value =}")
-            if spec_value == FeatureType.FLOAT.value:
-                self.numeric_cols.append(feature)
-                self.features_dtypes[feature] = tf.float32
-                logger.debug(f"Adding {feature =} as a numeric feature")
-
-            elif spec_value == FeatureType.INTEGER_CATEGORICAL.value:
-                self.categorical_cols.append(feature)
-                self.features_dtypes[feature] = tf.int32
-                logger.debug(f"Adding {feature =} as a integer categorical feature")
-
-            elif spec_value == FeatureType.STRING_CATEGORICAL.value:
-                self.categorical_cols.append(feature)
-                self.features_dtypes[feature] = tf.string
-                logger.debug(f"Adding {feature =} as a string categorical feature")
-            else:
-                _availble_specs = [spec.value for spec in FeatureType]
-                raise ValueError(f"Invalid {feature = }, {spec_value =}, You must use {_availble_specs =}")
+        self.numeric_stats = {col: WelfordAccumulator() for col in self.numeric_features}
+        self.categorical_stats = {col: CategoricalAccumulator() for col in self.categorical_features}
 
     def _get_csv_file_pattern(self, path) -> str:
         """Get the csv file pattern that will handle directories and file paths.
 
         Args:
             path (str): Path to the csv file (can be a directory or a file)
 
@@ -213,115 +171,70 @@
             shuffle=False,
             ignore_errors=True,
             batch_size=self.batch_size,
         )
         logger.info(f"DataSet Ready to be used (batched by: {self.batch_size}) ✅")
         return self.ds
 
-    def _infer_feature_dtypes(self, dataset: tf.data.Dataset) -> None:
-        """Infer data types for features based on a sample from the dataset.
-
-        Args:
-            dataset: The dataset to sample from for data type inference.
-
-        Returns:
-            A dictionary mapping feature names to inferred TensorFlow data types.
-        """
-        logger.info("Inferring data types for features based on a sample from the dataset 🔬")
-        self.feature_dtypes = {}
-        for batch in dataset.take(1):  # Sample the first batch
-            for feature in self.categorical_cols:
-                # Check the data type of the first element in the batch for this feature
-                value = batch[feature].numpy()[0]
-                # checking if I can cast to int32
-                try:
-                    value = tf.cast(value, tf.int32)
-                    # value = keras.ops.cast(value, "int32")
-                    logger.debug(f"Value {value} of {feature} can be cast to int32")
-                    inferred_dtype = tf.int32
-                except Exception:
-                    _type = type(value)
-                    logger.debug(f"Value {value} of {feature} is of type {_type} and cannot be cast to int32")
-                    inferred_dtype = tf.string
-                logger.debug(f"Inferred dtype for {feature} (value: {value}): {inferred_dtype}")
-                self.features_dtypes[feature] = inferred_dtype
-
-            for feature in self.numeric_cols:
-                self.features_dtypes[feature] = tf.float32
-
-        return self.features_dtypes
-
-    def _get_dtype_for_feature(self, feature_name: str) -> tf.dtypes.DType:
-        """Returns the TensorFlow data type for a given feature, with special handling for categorical features.
-
-        Args:
-            feature_name: The name of the feature for which to get the data type.
-
-        Returns:
-            The TensorFlow data type for the given feature.
-        """
-        # Use inferred dtype if available, otherwise default to float32 for numeric and string for categorical
-        return self.features_dtypes.get(feature_name, tf.float32 if feature_name in self.numeric_cols else tf.string)
-
     def _process_batch(self, batch: tf.Tensor) -> None:
         """Update statistics accumulators for each batch.
 
         Args:
             batch: A batch of data from the dataset.
         """
-        for feature in self.numeric_cols:
+        for feature in self.numeric_features:
             self.numeric_stats[feature].update(batch[feature])
 
-        for feature in self.categorical_cols:
+        for feature in self.categorical_features:
             self.categorical_stats[feature].update(batch[feature])
 
     def _compute_final_statistics(self) -> dict[str, dict]:
         """Compute final statistics for numeric and categorical features."""
         logger.info("Computing final statistics for numeric and categorical features 📊")
         final_stats = {"numeric_stats": {}, "categorical_stats": {}}
-        for feature in self.numeric_cols:
+        for feature in self.numeric_features:
+            logger.debug(f"numeric {feature =}")
             final_stats["numeric_stats"][feature] = {
                 "mean": self.numeric_stats[feature].mean.numpy(),
                 "count": self.numeric_stats[feature].count.numpy(),
                 "var": self.numeric_stats[feature].variance.numpy(),
-                "dtype": self._get_dtype_for_feature(feature_name=feature),
+                "dtype": self.features_specs[feature].dtype,
             }
 
-        for feature in self.categorical_cols:
+        for feature in self.categorical_features:
+            logger.debug(f"categorical {feature =}")
             # Convert TensorFlow string tensor to Python list for unique values
-            _dtype = self.features_dtypes.get(feature, tf.string)
+            _dtype = self.features_specs[feature].dtype
+            logger.debug(f"{_dtype =}")
+            # converting unique values
             if _dtype == tf.int32:
                 unique_values = [int(_byte) for _byte in self.categorical_stats[feature].get_unique_values()]
                 unique_values.sort()
             else:
                 _unique_values = self.categorical_stats[feature].get_unique_values()
                 unique_values = [(_byte).decode("utf-8") for _byte in _unique_values]
+            # forming stats
             final_stats["categorical_stats"][feature] = {
                 "size": len(unique_values),
                 "vocab": unique_values,
-                "dtype": self._get_dtype_for_feature(feature_name=feature),
+                "dtype": _dtype,
             }
 
         return final_stats
 
     def calculate_dataset_statistics(self, dataset: tf.data.Dataset) -> dict[str, dict]:
         """Calculates and returns statistics for the dataset.
 
         Args:
             dataset: The dataset for which to calculate statistics.
         """
         logger.info("Calculating statistics for the dataset 📊")
         for batch in dataset:
             self._process_batch(batch)
 
-        # Infer data types for features
-        if not self.features_specs:
-            logger.debug("Infering features dtypes")
-            self.features_dtypes = self._infer_feature_dtypes(dataset) if dataset is not None else {}
-
         # calculating data statistics
         self.features_stats = self._compute_final_statistics()
 
         return self.features_stats
 
     @staticmethod
     def _custom_serializer(obj) -> Any:
```

### Comparing `kdp-1.0.0/pyproject.toml` & `kdp-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "kdp"
-version = "1.0.0"
+version = "1.4.0"
 documentation = "http://piotrlaczkowski.github.io/keras-data-processor/"
 repository = "https://github.com/piotrlaczkowski/keras-data-processor"
 description = "Data Preprocessing model based on Keras preprocessing layers"
 authors = ["piotrlaczkowski <piotr.laczkowski@gmail.com>"]
 readme = "README.md"
-include = []
+include = ["docs/kdp_logo.png"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.12"
```

