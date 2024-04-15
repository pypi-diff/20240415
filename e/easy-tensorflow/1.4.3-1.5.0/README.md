# Comparing `tmp/easy-tensorflow-1.4.3.tar.gz` & `tmp/easy-tensorflow-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/easy-tensorflow-1.4.3.tar", last modified: Wed Apr 26 16:02:07 2023, max compression
+gzip compressed data, was "easy-tensorflow-1.5.0.tar", last modified: Mon Apr 15 18:38:42 2024, max compression
```

## Comparing `easy-tensorflow-1.4.3.tar` & `easy-tensorflow-1.5.0.tar`

### file list

```diff
@@ -1,36 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easy_tensorflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1760 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/data/mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/categorical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/numerical_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/feature_encoders/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/feature_preprocessor_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/preprocessing/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/easyflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/tests/test_feature_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/easyflow/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 16:02:07.000000 easy-tensorflow-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-26 16:00:27.000000 easy-tensorflow-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/easy_tensorflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-15 18:38:42.000000 easy-tensorflow-1.5.0/easy_tensorflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-15 18:38:42.000000 easy-tensorflow-1.5.0/easy_tensorflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:38:42.000000 easy-tensorflow-1.5.0/easy_tensorflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 18:38:42.000000 easy-tensorflow-1.5.0/easy_tensorflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 18:38:42.000000 easy-tensorflow-1.5.0/easy_tensorflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:38:42.746410 easy-tensorflow-1.5.0/easyflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/easyflow/data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1760 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/data/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/easyflow/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/preprocessing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8445 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/preprocessing/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/preprocessing/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8768 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/preprocessing/feature_preprocessor_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/preprocessing/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/easyflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7942 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/easyflow/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:38:42.750410 easy-tensorflow-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-15 18:37:45.000000 easy-tensorflow-1.5.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `easy-tensorflow-1.4.3/CHANGELOG.md` & `easy-tensorflow-1.5.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## VERSION 1.5.0
+* Bump Python to 3.10
+* Update code to be compatible with Keras 3
+
 ## VERSION 1.4.3
 * Minor update to the classes that contained serialization errors.
 * Minor fix to one of the notebook examples
 
 ## VERSION 1.4.2
 * Added temp fix when using StringLookup layer as first layer in Keras Sequential model
   (reference: https://github.com/keras-team/keras/issues/16101)
```

### Comparing `easy-tensorflow-1.4.3/PKG-INFO` & `easy-tensorflow-1.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,167 +1,162 @@
 Metadata-Version: 2.1
 Name: easy-tensorflow
-Version: 1.4.3
+Version: 1.5.0
 Summary: Feature Pipelines for Keras preprocessing layers.
 Home-page: https://github.com/fernandonieuwveldt/easyflow
 Author: Fernando Nieuwveldt
 Author-email: fdnieuwveldt@gmail.com
-License: UNKNOWN
-Description: # EasyFlow: Keras Feature Preprocessing Pipelines
-        
-        ![Keras logo](https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png)
-        
-        # Table of Contents
-        1. [About EasyFlow](#about-EasyFlow)
-        2. [Motivation](#motivation)
-        3. [Installation](#installation)
-        4. [Example](#example)
-        5. [Tutorials](#tutorials)
-        
-        ---
-        
-        ## About EasyFlow
-        
-        The `EasyFlow` package implements an interface similar to SKLearn's Pipeline API that contains easy feature preprocessing pipelines to build a full training and inference pipeline natively in Keras. All pipelines are implemented as Keras layers. 
-        
-        ---
-        
-        ## Motivation
-        
-        There is a need to have a similar interface for Keras that mimics the SKLearn Pipeline API such as `Pipeline`, `FeatureUnion` and `ColumnTransformer`, but natively in Keras as Keras layers. The usual design pattern especially for tabular data is to first do preprocessing with SKLearn and then feed the data to a Keras model. With `EasyFlow` you don't need to leave the Tensorflow/Keras ecosystem to build custom pipelines and your preprocessing pipeline is part of your model architecture.
-        
-        Main interfaces are:
-        
-        * `FeaturePreprocessor`: This layer applies feature preprocessing steps and returns a separate layer for each step supplied. This gives more flexibility to the user and if a more advance network architecture is needed. For example something like a Wide and Deep network.
-        * `FeatureUnion`: This layer is similar to `FeaturePreprocessor` with an extra step that concatenates all layers into a single layer.
-        
-        ---
-        
-        ## Installation:
-        
-        ```bash
-        pip install easy-tensorflow
-        ```
-        
-        ---
-        
-        ## Example
-        
-        Lets look at a quick example:
-        
-        ```python
-        import pandas as pd
-        import tensorflow as tf
-        from tensorflow.keras.layers import Normalization, StringLookup, IntegerLookup
-        
-        # local imports
-        from easyflow.data import TensorflowDataMapper
-        from easyflow.preprocessing import FeatureUnion
-        from easyflow.preprocessing import (
-            FeatureInputLayer,
-            StringToIntegerLookup,
-        )
-        
-        ```
-        
-        ### Read in data and map as tf.data.Dataset
-        Use the TensorflowDataMapper class to map pandas data frame to a tf.data.Dataset type.
-        
-        ```python
-        file_url = "http://storage.googleapis.com/download.tensorflow.org/data/heart.csv"
-        dataframe = pd.read_csv(file_url)
-        labels = dataframe.pop("target")
-        
-        batch_size = 32
-        dataset_mapper = TensorflowDataMapper() 
-        dataset = dataset_mapper.map(dataframe, labels)
-        train_data_set, val_data_set = dataset_mapper.split_data_set(dataset)
-        train_data_set = train_data_set.batch(batch_size)
-        val_data_set = val_data_set.batch(batch_size)
-        ```
-        
-        ### Set constants
-        ```python
-        NUMERICAL_FEATURES = ['age', 'trestbps', 'chol', 'thalach', 'oldpeak', 'slope']
-        CATEGORICAL_FEATURES = ['sex', 'cp', 'fbs', 'restecg', 'exang', 'ca']
-        # thal is represented as a string
-        STRING_CATEGORICAL_FEATURES = ['thal']
-        
-        dtype_mapper = {
-            "age": tf.float32,
-            "sex": tf.float32,
-            "cp": tf.float32,
-            "trestbps": tf.float32,
-            "chol": tf.float32,
-            "fbs": tf.float32,
-            "restecg": tf.float32,
-            "thalach": tf.float32,
-            "exang": tf.float32,
-            "oldpeak": tf.float32,
-            "slope": tf.float32,
-            "ca": tf.float32,
-            "thal": tf.string,
-        }
-        ```
-        
-        ### Setup Preprocessing layer using FeatureUnion
-        
-        This is the main part where `EasyFlow` fits in. We can now easily setup a feature preprocessing pipeline as a Keras layer with only a few lines of code.
-        
-        ```python
-        feature_preprocessor_list = [
-            ('numeric_encoder', Normalization(), NUMERICAL_FEATURES),
-            ('categorical_encoder', IntegerLookup(output_mode='multi_hot'), CATEGORICAL_FEATURES),
-            ('string_encoder', StringToIntegerLookup(), STRING_CATEGORICAL_FEATURES)
-        ]
-        
-        preprocessor = FeatureUnion(feature_preprocessor_list)
-        preprocessor.adapt(train_data_set)
-        
-        feature_layer_inputs = FeatureInputLayer(dtype_mapper)
-        preprocessing_layer = preprocessor(feature_layer_inputs)
-        ```
-        
-        ### Set up network
-        
-        ```python
-        # setup simple network
-        x = tf.keras.layers.Dense(128, activation="relu")(preprocessing_layer)
-        x = tf.keras.layers.Dropout(0.5)(x)
-        outputs = tf.keras.layers.Dense(1, activation='sigmoid')(x)
-        model = tf.keras.Model(inputs=feature_layer_inputs, outputs=outputs)
-        model.compile(
-            optimizer=tf.keras.optimizers.Adam(),
-            loss=tf.keras.losses.BinaryCrossentropy(),
-            metrics=[tf.keras.metrics.BinaryAccuracy(name='accuracy'), tf.keras.metrics.AUC(name='auc')])
-        ```
-        
-        ### Fit model
-        
-        ```python
-        history=model.fit(train_data_set, validation_data=val_data_set, epochs=10)
-        ```
-        
-        ---
-        
-        ## Tutorials
-        
-        ### Migrate an Sklearn training Pipeline to Tensorflow Keras: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/migrating_from_sklearn_to_keras/migrate_sklearn_pipeline.ipynb)
-        * In this notebook we look at ways to migrate an Sklearn training pipeline to Tensorflow Keras. There might be a few reasons to move from Sklearn to Tensorflow.
-        
-        
-        ### Single Input Multiple Output Preprocessor: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/single_input_multiple_output/single_input_multiple_output_preprocessor.ipynb)
-        * In this example we will show case how to apply different transformations and preprocessing steps on the same feature. What we have here is an example of a Single input Multiple output feature transformation scenario.
-        
-        ### Preprocessing module quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/preprocessing_example/preprocessing_example.ipynb)
-        * The `easyflow.preprocessing` module contains functionality similar to what Sklearn does with its `Pipeline`, `FeatureUnion` and `ColumnTransformer` does. This is a quick introduction.
-        
-        
-        ### Tensorflow Feature columns quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/feature_column_demo/feature_column_example.ipynb)
-        *  Model building Pipeline using `EasyFlow` feature_encoders module. This module is a fusion between Keras layers and Tensorflow feature columns.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# EasyFlow: Keras Feature Preprocessing Pipelines
+
+![Keras logo](https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png)
+
+# Table of Contents
+1. [About EasyFlow](#about-EasyFlow)
+2. [Motivation](#motivation)
+3. [Installation](#installation)
+4. [Example](#example)
+5. [Tutorials](#tutorials)
+
+---
+
+## About EasyFlow
+
+The `EasyFlow` package implements an interface similar to SKLearn's Pipeline API that contains easy feature preprocessing pipelines to build a full training and inference pipeline natively in Keras. All pipelines are implemented as Keras layers. 
+
+---
+
+## Motivation
+
+There is a need to have a similar interface for Keras that mimics the SKLearn Pipeline API such as `Pipeline`, `FeatureUnion` and `ColumnTransformer`, but natively in Keras as Keras layers. The usual design pattern especially for tabular data is to first do preprocessing with SKLearn and then feed the data to a Keras model. With `EasyFlow` you don't need to leave the Tensorflow/Keras ecosystem to build custom pipelines and your preprocessing pipeline is part of your model architecture.
+
+Main interfaces are:
+
+* `FeaturePreprocessor`: This layer applies feature preprocessing steps and returns a separate layer for each step supplied. This gives more flexibility to the user and if a more advance network architecture is needed. For example something like a Wide and Deep network.
+* `FeatureUnion`: This layer is similar to `FeaturePreprocessor` with an extra step that concatenates all layers into a single layer.
+
+---
+
+## Installation:
+
+```bash
+pip install easy-tensorflow
+```
+
+---
+
+## Example
+
+Lets look at a quick example:
+
+```python
+import pandas as pd
+import tensorflow as tf
+from tensorflow.keras.layers import Normalization, StringLookup, IntegerLookup
+
+# local imports
+from easyflow.data import TensorflowDataMapper
+from easyflow.preprocessing import FeatureUnion
+from easyflow.preprocessing import (
+    FeatureInputLayer,
+    StringToIntegerLookup,
+)
+
+```
+
+### Read in data and map as tf.data.Dataset
+Use the TensorflowDataMapper class to map pandas data frame to a tf.data.Dataset type.
+
+```python
+file_url = "http://storage.googleapis.com/download.tensorflow.org/data/heart.csv"
+dataframe = pd.read_csv(file_url)
+labels = dataframe.pop("target")
+
+batch_size = 32
+dataset_mapper = TensorflowDataMapper() 
+dataset = dataset_mapper.map(dataframe, labels)
+train_data_set, val_data_set = dataset_mapper.split_data_set(dataset)
+train_data_set = train_data_set.batch(batch_size)
+val_data_set = val_data_set.batch(batch_size)
+```
+
+### Set constants
+```python
+NUMERICAL_FEATURES = ['age', 'trestbps', 'chol', 'thalach', 'oldpeak', 'slope']
+CATEGORICAL_FEATURES = ['sex', 'cp', 'fbs', 'restecg', 'exang', 'ca']
+# thal is represented as a string
+STRING_CATEGORICAL_FEATURES = ['thal']
+
+dtype_mapper = {
+    "age": tf.float32,
+    "sex": tf.float32,
+    "cp": tf.float32,
+    "trestbps": tf.float32,
+    "chol": tf.float32,
+    "fbs": tf.float32,
+    "restecg": tf.float32,
+    "thalach": tf.float32,
+    "exang": tf.float32,
+    "oldpeak": tf.float32,
+    "slope": tf.float32,
+    "ca": tf.float32,
+    "thal": tf.string,
+}
+```
+
+### Setup Preprocessing layer using FeatureUnion
+
+This is the main part where `EasyFlow` fits in. We can now easily setup a feature preprocessing pipeline as a Keras layer with only a few lines of code.
+
+```python
+feature_preprocessor_list = [
+    ('numeric_encoder', Normalization(), NUMERICAL_FEATURES),
+    ('categorical_encoder', IntegerLookup(output_mode='multi_hot'), CATEGORICAL_FEATURES),
+    ('string_encoder', StringToIntegerLookup(), STRING_CATEGORICAL_FEATURES)
+]
+
+preprocessor = FeatureUnion(feature_preprocessor_list)
+preprocessor.adapt(train_data_set)
+
+feature_layer_inputs = FeatureInputLayer(dtype_mapper)
+preprocessing_layer = preprocessor(feature_layer_inputs)
+```
+
+### Set up network
+
+```python
+# setup simple network
+x = tf.keras.layers.Dense(128, activation="relu")(preprocessing_layer)
+x = tf.keras.layers.Dropout(0.5)(x)
+outputs = tf.keras.layers.Dense(1, activation='sigmoid')(x)
+model = tf.keras.Model(inputs=feature_layer_inputs, outputs=outputs)
+model.compile(
+    optimizer=tf.keras.optimizers.Adam(),
+    loss=tf.keras.losses.BinaryCrossentropy(),
+    metrics=[tf.keras.metrics.BinaryAccuracy(name='accuracy'), tf.keras.metrics.AUC(name='auc')])
+```
+
+### Fit model
+
+```python
+history=model.fit(train_data_set, validation_data=val_data_set, epochs=10)
+```
+
+---
+
+## Tutorials
+
+### Migrate an Sklearn training Pipeline to Tensorflow Keras: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/migrating_from_sklearn_to_keras/migrate_sklearn_pipeline.ipynb)
+* In this notebook we look at ways to migrate an Sklearn training pipeline to Tensorflow Keras. There might be a few reasons to move from Sklearn to Tensorflow.
+
+
+### Single Input Multiple Output Preprocessor: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/single_input_multiple_output/single_input_multiple_output_preprocessor.ipynb)
+* In this example we will show case how to apply different transformations and preprocessing steps on the same feature. What we have here is an example of a Single input Multiple output feature transformation scenario.
+
+### Preprocessing module quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/preprocessing_example/preprocessing_example.ipynb)
+* The `easyflow.preprocessing` module contains functionality similar to what Sklearn does with its `Pipeline`, `FeatureUnion` and `ColumnTransformer` does. This is a quick introduction.
```

### Comparing `easy-tensorflow-1.4.3/README.md` & `easy-tensorflow-1.5.0/easy_tensorflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: easy-tensorflow
+Version: 1.5.0
+Summary: Feature Pipelines for Keras preprocessing layers.
+Home-page: https://github.com/fernandonieuwveldt/easyflow
+Author: Fernando Nieuwveldt
+Author-email: fdnieuwveldt@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # EasyFlow: Keras Feature Preprocessing Pipelines
 
 ![Keras logo](https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png)
 
 # Table of Contents
 1. [About EasyFlow](#about-EasyFlow)
 2. [Motivation](#motivation)
@@ -142,11 +156,7 @@
 
 
 ### Single Input Multiple Output Preprocessor: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/single_input_multiple_output/single_input_multiple_output_preprocessor.ipynb)
 * In this example we will show case how to apply different transformations and preprocessing steps on the same feature. What we have here is an example of a Single input Multiple output feature transformation scenario.
 
 ### Preprocessing module quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/preprocessing_example/preprocessing_example.ipynb)
 * The `easyflow.preprocessing` module contains functionality similar to what Sklearn does with its `Pipeline`, `FeatureUnion` and `ColumnTransformer` does. This is a quick introduction.
-
-
-### Tensorflow Feature columns quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/feature_column_demo/feature_column_example.ipynb)
-*  Model building Pipeline using `EasyFlow` feature_encoders module. This module is a fusion between Keras layers and Tensorflow feature columns.
```

### Comparing `easy-tensorflow-1.4.3/easy_tensorflow.egg-info/PKG-INFO` & `easy-tensorflow-1.5.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,167 +1,148 @@
-Metadata-Version: 2.1
-Name: easy-tensorflow
-Version: 1.4.3
-Summary: Feature Pipelines for Keras preprocessing layers.
-Home-page: https://github.com/fernandonieuwveldt/easyflow
-Author: Fernando Nieuwveldt
-Author-email: fdnieuwveldt@gmail.com
-License: UNKNOWN
-Description: # EasyFlow: Keras Feature Preprocessing Pipelines
-        
-        ![Keras logo](https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png)
-        
-        # Table of Contents
-        1. [About EasyFlow](#about-EasyFlow)
-        2. [Motivation](#motivation)
-        3. [Installation](#installation)
-        4. [Example](#example)
-        5. [Tutorials](#tutorials)
-        
-        ---
-        
-        ## About EasyFlow
-        
-        The `EasyFlow` package implements an interface similar to SKLearn's Pipeline API that contains easy feature preprocessing pipelines to build a full training and inference pipeline natively in Keras. All pipelines are implemented as Keras layers. 
-        
-        ---
-        
-        ## Motivation
-        
-        There is a need to have a similar interface for Keras that mimics the SKLearn Pipeline API such as `Pipeline`, `FeatureUnion` and `ColumnTransformer`, but natively in Keras as Keras layers. The usual design pattern especially for tabular data is to first do preprocessing with SKLearn and then feed the data to a Keras model. With `EasyFlow` you don't need to leave the Tensorflow/Keras ecosystem to build custom pipelines and your preprocessing pipeline is part of your model architecture.
-        
-        Main interfaces are:
-        
-        * `FeaturePreprocessor`: This layer applies feature preprocessing steps and returns a separate layer for each step supplied. This gives more flexibility to the user and if a more advance network architecture is needed. For example something like a Wide and Deep network.
-        * `FeatureUnion`: This layer is similar to `FeaturePreprocessor` with an extra step that concatenates all layers into a single layer.
-        
-        ---
-        
-        ## Installation:
-        
-        ```bash
-        pip install easy-tensorflow
-        ```
-        
-        ---
-        
-        ## Example
-        
-        Lets look at a quick example:
-        
-        ```python
-        import pandas as pd
-        import tensorflow as tf
-        from tensorflow.keras.layers import Normalization, StringLookup, IntegerLookup
-        
-        # local imports
-        from easyflow.data import TensorflowDataMapper
-        from easyflow.preprocessing import FeatureUnion
-        from easyflow.preprocessing import (
-            FeatureInputLayer,
-            StringToIntegerLookup,
-        )
-        
-        ```
-        
-        ### Read in data and map as tf.data.Dataset
-        Use the TensorflowDataMapper class to map pandas data frame to a tf.data.Dataset type.
-        
-        ```python
-        file_url = "http://storage.googleapis.com/download.tensorflow.org/data/heart.csv"
-        dataframe = pd.read_csv(file_url)
-        labels = dataframe.pop("target")
-        
-        batch_size = 32
-        dataset_mapper = TensorflowDataMapper() 
-        dataset = dataset_mapper.map(dataframe, labels)
-        train_data_set, val_data_set = dataset_mapper.split_data_set(dataset)
-        train_data_set = train_data_set.batch(batch_size)
-        val_data_set = val_data_set.batch(batch_size)
-        ```
-        
-        ### Set constants
-        ```python
-        NUMERICAL_FEATURES = ['age', 'trestbps', 'chol', 'thalach', 'oldpeak', 'slope']
-        CATEGORICAL_FEATURES = ['sex', 'cp', 'fbs', 'restecg', 'exang', 'ca']
-        # thal is represented as a string
-        STRING_CATEGORICAL_FEATURES = ['thal']
-        
-        dtype_mapper = {
-            "age": tf.float32,
-            "sex": tf.float32,
-            "cp": tf.float32,
-            "trestbps": tf.float32,
-            "chol": tf.float32,
-            "fbs": tf.float32,
-            "restecg": tf.float32,
-            "thalach": tf.float32,
-            "exang": tf.float32,
-            "oldpeak": tf.float32,
-            "slope": tf.float32,
-            "ca": tf.float32,
-            "thal": tf.string,
-        }
-        ```
-        
-        ### Setup Preprocessing layer using FeatureUnion
-        
-        This is the main part where `EasyFlow` fits in. We can now easily setup a feature preprocessing pipeline as a Keras layer with only a few lines of code.
-        
-        ```python
-        feature_preprocessor_list = [
-            ('numeric_encoder', Normalization(), NUMERICAL_FEATURES),
-            ('categorical_encoder', IntegerLookup(output_mode='multi_hot'), CATEGORICAL_FEATURES),
-            ('string_encoder', StringToIntegerLookup(), STRING_CATEGORICAL_FEATURES)
-        ]
-        
-        preprocessor = FeatureUnion(feature_preprocessor_list)
-        preprocessor.adapt(train_data_set)
-        
-        feature_layer_inputs = FeatureInputLayer(dtype_mapper)
-        preprocessing_layer = preprocessor(feature_layer_inputs)
-        ```
-        
-        ### Set up network
-        
-        ```python
-        # setup simple network
-        x = tf.keras.layers.Dense(128, activation="relu")(preprocessing_layer)
-        x = tf.keras.layers.Dropout(0.5)(x)
-        outputs = tf.keras.layers.Dense(1, activation='sigmoid')(x)
-        model = tf.keras.Model(inputs=feature_layer_inputs, outputs=outputs)
-        model.compile(
-            optimizer=tf.keras.optimizers.Adam(),
-            loss=tf.keras.losses.BinaryCrossentropy(),
-            metrics=[tf.keras.metrics.BinaryAccuracy(name='accuracy'), tf.keras.metrics.AUC(name='auc')])
-        ```
-        
-        ### Fit model
-        
-        ```python
-        history=model.fit(train_data_set, validation_data=val_data_set, epochs=10)
-        ```
-        
-        ---
-        
-        ## Tutorials
-        
-        ### Migrate an Sklearn training Pipeline to Tensorflow Keras: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/migrating_from_sklearn_to_keras/migrate_sklearn_pipeline.ipynb)
-        * In this notebook we look at ways to migrate an Sklearn training pipeline to Tensorflow Keras. There might be a few reasons to move from Sklearn to Tensorflow.
-        
-        
-        ### Single Input Multiple Output Preprocessor: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/single_input_multiple_output/single_input_multiple_output_preprocessor.ipynb)
-        * In this example we will show case how to apply different transformations and preprocessing steps on the same feature. What we have here is an example of a Single input Multiple output feature transformation scenario.
-        
-        ### Preprocessing module quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/preprocessing_example/preprocessing_example.ipynb)
-        * The `easyflow.preprocessing` module contains functionality similar to what Sklearn does with its `Pipeline`, `FeatureUnion` and `ColumnTransformer` does. This is a quick introduction.
-        
-        
-        ### Tensorflow Feature columns quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/feature_column_demo/feature_column_example.ipynb)
-        *  Model building Pipeline using `EasyFlow` feature_encoders module. This module is a fusion between Keras layers and Tensorflow feature columns.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
+# EasyFlow: Keras Feature Preprocessing Pipelines
+
+![Keras logo](https://s3.amazonaws.com/keras.io/img/keras-logo-2018-large-1200.png)
+
+# Table of Contents
+1. [About EasyFlow](#about-EasyFlow)
+2. [Motivation](#motivation)
+3. [Installation](#installation)
+4. [Example](#example)
+5. [Tutorials](#tutorials)
+
+---
+
+## About EasyFlow
+
+The `EasyFlow` package implements an interface similar to SKLearn's Pipeline API that contains easy feature preprocessing pipelines to build a full training and inference pipeline natively in Keras. All pipelines are implemented as Keras layers. 
+
+---
+
+## Motivation
+
+There is a need to have a similar interface for Keras that mimics the SKLearn Pipeline API such as `Pipeline`, `FeatureUnion` and `ColumnTransformer`, but natively in Keras as Keras layers. The usual design pattern especially for tabular data is to first do preprocessing with SKLearn and then feed the data to a Keras model. With `EasyFlow` you don't need to leave the Tensorflow/Keras ecosystem to build custom pipelines and your preprocessing pipeline is part of your model architecture.
+
+Main interfaces are:
+
+* `FeaturePreprocessor`: This layer applies feature preprocessing steps and returns a separate layer for each step supplied. This gives more flexibility to the user and if a more advance network architecture is needed. For example something like a Wide and Deep network.
+* `FeatureUnion`: This layer is similar to `FeaturePreprocessor` with an extra step that concatenates all layers into a single layer.
+
+---
+
+## Installation:
+
+```bash
+pip install easy-tensorflow
+```
+
+---
+
+## Example
+
+Lets look at a quick example:
+
+```python
+import pandas as pd
+import tensorflow as tf
+from tensorflow.keras.layers import Normalization, StringLookup, IntegerLookup
+
+# local imports
+from easyflow.data import TensorflowDataMapper
+from easyflow.preprocessing import FeatureUnion
+from easyflow.preprocessing import (
+    FeatureInputLayer,
+    StringToIntegerLookup,
+)
+
+```
+
+### Read in data and map as tf.data.Dataset
+Use the TensorflowDataMapper class to map pandas data frame to a tf.data.Dataset type.
+
+```python
+file_url = "http://storage.googleapis.com/download.tensorflow.org/data/heart.csv"
+dataframe = pd.read_csv(file_url)
+labels = dataframe.pop("target")
+
+batch_size = 32
+dataset_mapper = TensorflowDataMapper() 
+dataset = dataset_mapper.map(dataframe, labels)
+train_data_set, val_data_set = dataset_mapper.split_data_set(dataset)
+train_data_set = train_data_set.batch(batch_size)
+val_data_set = val_data_set.batch(batch_size)
+```
+
+### Set constants
+```python
+NUMERICAL_FEATURES = ['age', 'trestbps', 'chol', 'thalach', 'oldpeak', 'slope']
+CATEGORICAL_FEATURES = ['sex', 'cp', 'fbs', 'restecg', 'exang', 'ca']
+# thal is represented as a string
+STRING_CATEGORICAL_FEATURES = ['thal']
+
+dtype_mapper = {
+    "age": tf.float32,
+    "sex": tf.float32,
+    "cp": tf.float32,
+    "trestbps": tf.float32,
+    "chol": tf.float32,
+    "fbs": tf.float32,
+    "restecg": tf.float32,
+    "thalach": tf.float32,
+    "exang": tf.float32,
+    "oldpeak": tf.float32,
+    "slope": tf.float32,
+    "ca": tf.float32,
+    "thal": tf.string,
+}
+```
+
+### Setup Preprocessing layer using FeatureUnion
+
+This is the main part where `EasyFlow` fits in. We can now easily setup a feature preprocessing pipeline as a Keras layer with only a few lines of code.
+
+```python
+feature_preprocessor_list = [
+    ('numeric_encoder', Normalization(), NUMERICAL_FEATURES),
+    ('categorical_encoder', IntegerLookup(output_mode='multi_hot'), CATEGORICAL_FEATURES),
+    ('string_encoder', StringToIntegerLookup(), STRING_CATEGORICAL_FEATURES)
+]
+
+preprocessor = FeatureUnion(feature_preprocessor_list)
+preprocessor.adapt(train_data_set)
+
+feature_layer_inputs = FeatureInputLayer(dtype_mapper)
+preprocessing_layer = preprocessor(feature_layer_inputs)
+```
+
+### Set up network
+
+```python
+# setup simple network
+x = tf.keras.layers.Dense(128, activation="relu")(preprocessing_layer)
+x = tf.keras.layers.Dropout(0.5)(x)
+outputs = tf.keras.layers.Dense(1, activation='sigmoid')(x)
+model = tf.keras.Model(inputs=feature_layer_inputs, outputs=outputs)
+model.compile(
+    optimizer=tf.keras.optimizers.Adam(),
+    loss=tf.keras.losses.BinaryCrossentropy(),
+    metrics=[tf.keras.metrics.BinaryAccuracy(name='accuracy'), tf.keras.metrics.AUC(name='auc')])
+```
+
+### Fit model
+
+```python
+history=model.fit(train_data_set, validation_data=val_data_set, epochs=10)
+```
+
+---
+
+## Tutorials
+
+### Migrate an Sklearn training Pipeline to Tensorflow Keras: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/migrating_from_sklearn_to_keras/migrate_sklearn_pipeline.ipynb)
+* In this notebook we look at ways to migrate an Sklearn training pipeline to Tensorflow Keras. There might be a few reasons to move from Sklearn to Tensorflow.
+
+
+### Single Input Multiple Output Preprocessor: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/single_input_multiple_output/single_input_multiple_output_preprocessor.ipynb)
+* In this example we will show case how to apply different transformations and preprocessing steps on the same feature. What we have here is an example of a Single input Multiple output feature transformation scenario.
+
+### Preprocessing module quick intro: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fernandonieuwveldt/easyflow/blob/develop/examples/preprocessing_example/preprocessing_example.ipynb)
+* The `easyflow.preprocessing` module contains functionality similar to what Sklearn does with its `Pipeline`, `FeatureUnion` and `ColumnTransformer` does. This is a quick introduction.
```

### Comparing `easy-tensorflow-1.4.3/easyflow/data/mapper.py` & `easy-tensorflow-1.5.0/easyflow/data/mapper.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.3/easyflow/preprocessing/__init__.py` & `easy-tensorflow-1.5.0/easyflow/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.3/easyflow/preprocessing/base.py` & `easy-tensorflow-1.5.0/easyflow/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.3/easyflow/preprocessing/custom.py` & `easy-tensorflow-1.5.0/easyflow/preprocessing/custom.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Custom preprocessing layers"""
 
-from tensorflow.python.keras.engine.base_preprocessing_layer import PreprocessingLayer
 import tensorflow as tf
 from tensorflow.keras import layers
 
 
 class FeatureInputLayer:
     """Create model inputs for each Feature in the dataset of features that will be used for training. There are two
     options to create the input layer. By default we will be taking in a dict mapper with feature name and dtype as input to
@@ -65,17 +64,20 @@
 
         return {
             feature: tf.keras.Input(shape=(1,), name=feature, dtype=tspec.dtype)
             for feature, tspec in spec.items()
         }
 
 
-class NumericPreprocessingLayer(PreprocessingLayer):
+class NumericPreprocessingLayer(tf.keras.layers.Layer):
     """Helper class to apply no preprocessing and use feature as is"""
 
+    def adapt(self, data):
+        pass
+
     def call(self, inputs):
         return tf.keras.layers.Reshape((1,))(inputs)
 
     def get_config(self):
         """Override get_config to ensure saving of models works"""
         return super().get_config().copy()
 
@@ -151,24 +153,24 @@
 
     def __init__(self, layers_to_adapt=[], **kwargs):
         super(PreprocessorChain, self).__init__(layers=[], **kwargs)
         if not isinstance(layers_to_adapt, (list, tuple)):
             layers_to_adapt = [layers_to_adapt]
         self.layers_to_adapt = layers_to_adapt
 
-    def adapt(self, data, *args, **kwargs):
+    def adapt(self, data):
         """Adapt layers to adapt sequentially and add layers with the tf.keras.models.Sequential add 
         method.
 
         Args:
             data (tf.data.Dataset): Mapped tf.data.Dataset containing only the single feature
         """
         for counter, layer in enumerate(self.layers_to_adapt):
             if hasattr(layer, 'adapt'):
-                layer.adapt(data, *args, **kwargs)
+                layer.adapt(data)
 
             super().add(layer)
 
             if len(self.layers_to_adapt) > counter:
                 data = (
                     data.map(layer)
                     if isinstance(data, tf.data.Dataset)
@@ -194,24 +196,24 @@
     def __init__(self, steps=[], **kwargs):
         super(MultiOutputTransformer, self).__init__(**kwargs)
         if not isinstance(steps, (list, tuple)):
             steps = [steps]
         self.steps = steps
         self.processed_layers = []
 
-    def adapt(self, data, *args, **kwargs):
+    def adapt(self, data):
         """Apply different or independent preprocessing steps on the same data. The results will be concatenated
         into a single layer.
 
         Args:
             data (tf.data.Dataset): Mapped tf.data.Dataset containing only the single feature
         """
         for layer in self.steps:
             if hasattr(layer, 'adapt'):
-                layer.adapt(data, *args, **kwargs)
+                layer.adapt(data)
             self.processed_layers.append(layer)
 
     def call(self, inputs):
         """Apply sequential model containing adapted layers.
 
         Args:
             inputs (tf.data.Dataset): Feature to be adapted as a Mapped Dataset
@@ -240,11 +242,10 @@
     """Implements a common pipeline when categorical features are of type string.
     Steps involve to first apply StringLookup followed by IntegerLookup.
 
     Args:
         kwargs: All arguments are related to IntegerLookup
     """
     return PreprocessorChain([
-             tf.keras.layers.InputLayer(input_shape=(1,), dtype=tf.string), 
              layers.StringLookup(),
              layers.IntegerLookup(output_mode='multi_hot', **kwargs)]   
     )
```

### Comparing `easy-tensorflow-1.4.3/easyflow/preprocessing/factory.py` & `easy-tensorflow-1.5.0/easyflow/preprocessing/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         """
         if isinstance(dataset, tf.data.Dataset):
             feature_preprocessor_list = (
                 FeaturePreprocessorFromTensorflowDataset.from_infered_pipeline(dataset)
             )
             return cls(feature_preprocessor_list)
 
-    def adapt(self, dataset, *args, **kwargs):
+    def adapt(self, dataset):
         """Adapt preprocessing layers.
 
         Args:
             dataset ([pandas.DataFrame, tf.data.Dataset]): Training data.
         """
         if isinstance(dataset, tf.data.Dataset):
             self.preprocessor_flow = FeaturePreprocessorFromTensorflowDataset(
@@ -52,15 +52,15 @@
             self.preprocessor_flow = FeaturePreprocessorFromPandasDataFrame(
                 self.feature_preprocessor_list
             )
 
         if not self.preprocessor_flow:
             raise Exception("Datatype not supported: dataset should be of type pandas DataFrame or Tensorflow tf.data.Dataset")
 
-        self.preprocessor_flow.adapt(dataset, *args, **kwargs)
+        self.preprocessor_flow.adapt(dataset)
 
     def call(self, inputs):
         """Apply adapted layers on new data
 
         Args:
             inputs (dict): Dictionary of Tensors.
```

### Comparing `easy-tensorflow-1.4.3/easyflow/preprocessing/feature_preprocessor_layer.py` & `easy-tensorflow-1.5.0/easyflow/preprocessing/feature_preprocessor_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 
     def __init__(self, feature_preprocessor_list=[], *args, **kwargs):
         super(FeaturePreprocessorFromTensorflowDataset, self).__init__(*args, *kwargs)
         self.feature_preprocessor_list = feature_preprocessor_list
         self.feature_preprocessor_list = self.map_preprocessor(self.feature_preprocessor_list)
         self.adapted_preprocessors = dict()
 
-    def adapt(self, dataset, *args, **kwargs):
+    def adapt(self, dataset):
         """Loop through the feature preprocessor list and dapt features with the corresponding preprocessing
         layer. The adapted preprocessing layers can be accessed from the adapted_preprocessors attribute.
 
         Args:
             dataset (tf.data.Dataset): Training data.
         """
         for _, preprocessor, features in self.feature_preprocessor_list:
             # get initial preprocessing layer config
             config = preprocessor.get_config()
             for k, feature in enumerate(features):
                 # get a fresh preprocessing instance
                 cloned_preprocessor = preprocessor if k==0 else preprocessor.from_config(config)
                 feature_ds = extract_feature_column_tensorflow(dataset, feature)
                 # check if layer has adapt method
-                cloned_preprocessor.adapt(feature_ds, *args, **kwargs)
+                cloned_preprocessor.adapt(feature_ds)
                 self.adapted_preprocessors[feature] = cloned_preprocessor
 
     def call(self, inputs):
         """Apply adapted layers on new data.
 
         Args:
             inputs (dict): Dictionary of Tensors.
@@ -119,29 +119,29 @@
     """
 
     def __init__(self, feature_preprocessor_list=[], *args, **kwargs):
         super(FeaturePreprocessorFromPandasDataFrame, self).__init__(*args, *kwargs)
         self.feature_preprocessor_list = self.map_preprocessor(feature_preprocessor_list)
         self.adapted_preprocessors = dict()
 
-    def adapt(self, dataset, *args, **kwargs):
+    def adapt(self, dataset):
         """Adapt layers from tf.data.Dataset source type.
 
         Args:
             dataset (tf.data.Dataset): Training data.
         """
         for _, preprocessor, features in self.feature_preprocessor_list:
             # get initial preprocessing layer config
             config = preprocessor.get_config()
             for k, feature in enumerate(features):
                 # get a fresh preprocessing instance
                 cloned_preprocessor = preprocessor if k==0 else preprocessor.from_config(config)
                 feature_ds = extract_feature_column_pandas(dataset, feature)
                 # check if layer has adapt method
-                cloned_preprocessor.adapt(feature_ds, *args, **kwargs)
+                cloned_preprocessor.adapt(feature_ds)
                 self.adapted_preprocessors[feature] = cloned_preprocessor
 
     def call(self, inputs):
         """Apply adapted layers on new data
 
         Args:
             inputs (dict): Dictionary of Tensors.
```

### Comparing `easy-tensorflow-1.4.3/easyflow/preprocessing/pipeline.py` & `easy-tensorflow-1.5.0/easyflow/preprocessing/pipeline.py`

 * *Files identical despite different names*

### Comparing `easy-tensorflow-1.4.3/easyflow/tests/test_preprocessing.py` & `easy-tensorflow-1.5.0/easyflow/tests/test_preprocessing.py`

 * *Files 20% similar despite different names*

```diff
@@ -61,26 +61,28 @@
                 layers.IntegerLookup(output_mode="multi_hot"),
                 self.categorical_features,
             ),
             # For feature thal we first need to run StringLookup followed by a IntegerLookup layer
             (
                 "string_encoder",
                 PreprocessorChain(
-                    [tf.keras.layers.InputLayer(input_shape=(1,), dtype=tf.string), layers.StringLookup(), layers.IntegerLookup(output_mode="multi_hot")]
+                    [
+                     layers.StringLookup(),
+                     layers.IntegerLookup(output_mode="multi_hot")]
                 ),
                 self.string_categorical_features,
             ),
         ]
 
     def test_feature_preprocessor(self):
         """Test FeaturePreprocessor class
         """
         preprocessor = FeaturePreprocessor(self.feature_preprocessor_list)
         preprocessor.adapt(self.dataframe)
-        preprocessing_layer = preprocessor(self.all_feature_inputs)
+        preprocessing_layer = preprocessor.call(self.all_feature_inputs)
         assert list(preprocessing_layer.keys()) == ['numeric_encoder', 'categorical_encoder', 'string_encoder']
         assert preprocessing_layer.numeric_encoder.shape[-1] == 6
 
     def test_preprocessing_pipeline(self):
         """Test Feature union and model fit
         """
         all_feature_inputs, history = train_model_util(
@@ -100,15 +102,18 @@
                 layers.IntegerLookup(output_mode="multi_hot"),
                 self.categorical_features,
             ),
             # For feature thal we first need to run StringLookup followed by a IntegerLookup layer
             (
                 "string_encoder",
                 PreprocessorChain(
-                    [tf.keras.layers.InputLayer(input_shape=(1,), dtype=tf.string), layers.StringLookup(), layers.IntegerLookup(output_mode="multi_hot")]
+                    [
+                     #tf.keras.layers.InputLayer(input_shape=(1,), dtype=tf.string), 
+                     layers.StringLookup(),
+                     layers.IntegerLookup(output_mode="multi_hot")]
                 ),
                 self.string_categorical_features,
             ),
         ]
 
         all_feature_inputs, history = train_model_util(
             self.dataset, self.all_feature_inputs, feature_encoder_list_none
@@ -120,15 +125,16 @@
     def test_preprocessing_layer_with_no_args(self):
         """Test preprocessing layers with no arguments supplied
         """
         steps_list = [
             (
                 "string_encoder",
                 PreprocessorChain(
-                    [tf.keras.layers.InputLayer(input_shape=(1,), dtype=tf.string), layers.StringLookup(), layers.IntegerLookup(output_mode="multi_hot")]
+                    [
+                        layers.StringLookup(), layers.IntegerLookup(output_mode="multi_hot")]
                 ),
                 self.string_categorical_features,
             )
         ]
         preprocessor = FeatureUnion(steps_list)
         preprocessor.adapt(self.dataset)
         preprocessing_layer = preprocessor(self.all_feature_inputs)
@@ -138,45 +144,26 @@
         """Test preprocessing layers with arguments supplied
         """
         steps_list = [
             (
                 "string_encoder",
                 PreprocessorChain(
                     [
-                        tf.keras.layers.InputLayer(input_shape=(1,), dtype=tf.string),
                         layers.StringLookup(max_tokens=4),
                         layers.IntegerLookup(output_mode="multi_hot"),
                     ]
                 ),
                 self.string_categorical_features,
             )
         ]
         preprocessor = FeatureUnion(steps_list)
         preprocessor.adapt(self.dataset)
         preprocessing_layer = preprocessor(self.all_feature_inputs)
         assert preprocessing_layer.shape[-1] == 5
 
-    def test_adapt_with_args(self):
-        """Test pipeline with args passed to .adapt
-        """
-        steps_list = [
-                ("numeric_encoder", layers.Normalization(), self.numerical_features)
-        ]
-        # Apply on tf.data dataset
-        preprocessor = FeatureUnion(steps_list)
-        preprocessor.adapt(self.dataset, steps=1)
-        preprocessing_layer = preprocessor(self.all_feature_inputs)
-        assert preprocessing_layer.shape[-1] == 6
-        del preprocessor
-        # Apply on dataframe
-        preprocessor = FeatureUnion(steps_list)
-        preprocessor.adapt(self.dataframe, steps=1)
-        preprocessing_layer = preprocessor(self.all_feature_inputs)
-        assert preprocessing_layer.shape[-1] == 6
-
     def test_infered_pipeline(self):
         """test infered pipeline"""
         preprocessor = FeatureUnion.from_infered_pipeline(self.dataset)
         preprocessor.adapt(self.dataset)
         preprocessing_layer = preprocessor(self.all_feature_inputs)
         # setup simple network
         x = tf.keras.layers.Dense(128, activation="relu")(preprocessing_layer)
```

### Comparing `easy-tensorflow-1.4.3/setup.py` & `easy-tensorflow-1.5.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import io
 import os
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text(encoding='utf-8')
 REQUIREMENTS = (pathlib.Path(__file__).parent / "requirements.txt").read_text().splitlines()[1:]
-REQUIRES_PYTHON = '>=3.7.0'
+REQUIRES_PYTHON = '>=3.10'
 
 
 setup(
     name="easy-tensorflow",
-    version="1.4.3",
+    version="1.5.0",
     author="Fernando Nieuwveldt",
     author_email="fdnieuwveldt@gmail.com",
     description="Feature Pipelines for Keras preprocessing layers.",
     long_description_content_type='text/markdown',
     long_description=README,
     url="https://github.com/fernandonieuwveldt/easyflow",
     python_requires=REQUIRES_PYTHON,
```

