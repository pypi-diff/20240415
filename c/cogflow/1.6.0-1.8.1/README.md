# Comparing `tmp/cogflow-1.6.0.tar.gz` & `tmp/cogflow-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogflow-1.6.0.tar", last modified: Tue Mar 26 22:16:51 2024, max compression
+gzip compressed data, was "cogflow-1.8.1.tar", last modified: Mon Apr 15 14:01:35 2024, max compression
```

## Comparing `cogflow-1.6.0.tar` & `cogflow-1.8.1.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/
--rw-r--r--   0 bola      (1000) bola      (1000)      681 2024-03-26 22:16:51.068174 cogflow-1.6.0/PKG-INFO
--rw-rw-r--   0 bola      (1000) bola      (1000)     3878 2024-03-18 14:03:47.000000 cogflow-1.6.0/README.md
-drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/cogflow/
--rw-rw-r--   0 bola      (1000) bola      (1000)        0 2024-03-18 14:03:47.000000 cogflow-1.6.0/cogflow/__init__.py
--rw-rw-r--   0 bola      (1000) bola      (1000)    18896 2024-03-26 21:19:58.000000 cogflow-1.6.0/cogflow/cog_framework.py
--rw-rw-r--   0 bola      (1000) bola      (1000)      197 2024-03-18 14:03:47.000000 cogflow-1.6.0/cogflow/constant_vars.py
-drwxrwxr-x   0 bola      (1000) bola      (1000)        0 2024-03-26 22:16:51.068174 cogflow-1.6.0/cogflow.egg-info/
--rw-r--r--   0 bola      (1000) bola      (1000)      681 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/PKG-INFO
--rw-rw-r--   0 bola      (1000) bola      (1000)      242 2024-03-26 22:16:51.000000 cogflow-1.6.0/cogflow.egg-info/SOURCES.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)        1 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/dependency_links.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)      144 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/requires.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)        8 2024-03-26 22:16:50.000000 cogflow-1.6.0/cogflow.egg-info/top_level.txt
--rw-rw-r--   0 bola      (1000) bola      (1000)       38 2024-03-26 22:16:51.068174 cogflow-1.6.0/setup.cfg
--rw-rw-r--   0 bola      (1000) bola      (1000)      808 2024-03-26 21:20:18.000000 cogflow-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:01:35.090990 cogflow-1.8.1/
+-rw-rw-rw-   0        0        0      401 2024-04-15 14:01:35.075410 cogflow-1.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4024 2024-04-15 10:04:49.000000 cogflow-1.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 14:01:35.043374 cogflow-1.8.1/cogflow/
+-rw-rw-rw-   0        0        0      757 2024-04-15 10:41:15.000000 cogflow-1.8.1/cogflow/__init__.py
+-rw-rw-rw-   0        0        0     4029 2024-04-15 10:27:20.000000 cogflow-1.8.1/cogflow/dataset_plugin.py
+-rw-rw-rw-   0        0        0     8959 2024-04-15 10:26:32.000000 cogflow-1.8.1/cogflow/kubeflowplugin.py
+-rw-rw-rw-   0        0        0    11107 2024-04-15 10:33:52.000000 cogflow-1.8.1/cogflow/mlflowplugin.py
+-rw-rw-rw-   0        0        0      714 2024-04-15 10:04:49.000000 cogflow-1.8.1/cogflow/plugin_config.py
+-rw-rw-rw-   0        0        0      620 2024-04-15 10:04:49.000000 cogflow-1.8.1/cogflow/plugin_status.py
+-rw-rw-rw-   0        0        0      174 2024-04-15 10:04:49.000000 cogflow-1.8.1/cogflow/pluginerrors.py
+-rw-rw-rw-   0        0        0     5492 2024-04-15 10:36:36.000000 cogflow-1.8.1/cogflow/pluginmanager.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:01:35.069507 cogflow-1.8.1/cogflow.egg-info/
+-rw-rw-rw-   0        0        0      401 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-15 14:01:34.000000 cogflow-1.8.1/cogflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:01:35.090990 cogflow-1.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-04-15 14:01:29.000000 cogflow-1.8.1/setup.py
```

### Comparing `cogflow-1.6.0/README.md` & `cogflow-1.8.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,127 @@
-### **Step 1: Create a project directory**
-
-The first step to creating a Python package is to create a new project directory. This will contain all the files and
-directories necessary for the package.
-
-To create a new project directory, open a terminal or command prompt and run the following command:
-
-```
-mkdir mypackage
-cd mypackage
-```
-
-Replace "mypackage" with the name of your package.
-
-### **Step 2: Create a package directory**
-
-The next step is to create a new directory inside the project directory to hold the package code. It should have the
-same name as your package.
-
-To create a new package directory, run the following command:
-
-```
-mkdir mypackage
-```
-
-Replace "mypackage" with the name of your package.
-
-### **Step 3: Create a module file**
-
-Inside the package directory, create a new Python file to hold the package code. The file should have the same name as
-your package with a .py extension.
-
-For example, if your package is named "mypackage", create a file named "mypackage.py".
-
-In case of wrapping multiple modules with different names then create an “__**init__.py”** hosting all the modules which
-needs to be utilized
-
-### **Step 4: Write the package code**
-
-Write your package code in the module file you just created. It can include any Python code you want to have in the
-package, such as functions, classes, and variables.
-
-### **Step 5: Create a setup.py file**
-
-To publish your Python package to PyPI, you need to create a setup.py file. It contains metadata about your package like
-its name, version, author, and dependencies.
-
-Create a new file named "setup.py" in the project directory and add the following code:
-
-```
-from setuptools import setup, find_packages
-setup(
-name='mypackage',
-version='0.1.0',
-author='Your Name',
-author_email='your.email@example.com',
-description='A short description of your package',
-packages=find_packages(),
-classifiers=[
-'Programming Language :: Python :: 3',
-'License :: OSI Approved :: MIT License',
-'Operating System :: OS Independent',
-],
-python_requires='>=3.6',
-)
-```
-
-### **Step 6: Build the package**
-
-To build the package, run the following command in the project directory:
-
-```
-python setup.py sdist
-
-python setup.py sdist bdist_wheel
-```
-
-This will create a source distribution of your package in a new directory named "dist".
-
-### **Step 7: Upload the package to PyPI**
-
-To upload your package to PyPI, you first need to create an account on
-the[PyPI](https://pypi.org/account/register/)/ [TestPyPI · The Python Package Index](https://test.pypi.org/) website
-
-Once done, run the following command in the project directory:
-
-```
-twine upload dist/*
-```
-
-This will upload your package to PyPI.
-
-# **Step 8: PyPi .pypirc location on windows**
-
-Your .pypirc file on windows should be in your`$HOME`directory.
-
-On windows this is typically your user folder under`C:\Users\`. For example my current home folder for the user`hiro`
-is`C:\Users\hiro\`
-
-This means that my`.pypirc`file should live at`C:\Users\hiro\.pypirc`.
-
-If .pypirc file is not existing for the user then create it with the help of below template. on pypi/testpypi, generate
-your respective API token and use it as your password below.
-
-# **Typical PyPi .pypirc file contents**
-
-Typically the PyPi file will include information for the pypi and testpypi server. If you have a token for each of these
-your file will look something like this
-
-Here the settings for pypi and testpypi
-
-```python
-[distutils]
-index-servers =
-    pypi
-    testpypi
- 
-[pypi]
-repository = https://upload.pypi.org/legacy/
-username = __token__
-password = <PyPI token>
- 
-[testpypi]
-repository = https://test.pypi.org/legacy/
-username = __token__
-password = <PyPI token>
-```
-
-### **Step 9: Install the package**
-
-To install your package from PyPI, run the following command:
-
-```
-pip install mypackage
-```
-
-Replace "mypackage" with the name of your package.
+### **Step 1: Create a project directory**
+
+The first step to creating a Python package is to create a new project directory. This will contain all the files and directories necessary for the package.
+
+To create a new project directory, open a terminal or command prompt and run the following command:
+
+```
+mkdir mypackage
+cd mypackage
+```
+
+Replace "mypackage" with the name of your package.
+
+### **Step 2: Create a package directory**
+
+The next step is to create a new directory inside the project directory to hold the package code. It should have the same name as your package.
+
+To create a new package directory, run the following command:
+
+```
+mkdir mypackage
+```
+
+Replace "mypackage" with the name of your package.
+
+### **Step 3: Create a module file**
+
+Inside the package directory, create a new Python file to hold the package code. The file should have the same name as your package with a .py extension.
+
+For example, if your package is named "mypackage", create a file named "mypackage.py".
+
+In case of wrapping multiple modules with different names then create an “__**init__.py”** hosting all the modules which needs to be utilized
+
+### **Step 4: Write the package code**
+
+Write your package code in the module file you just created. It can include any Python code you want to have in the package, such as functions, classes, and variables.
+
+### **Step 5: Create a setup.py file**
+
+To publish your Python package to PyPI, you need to create a setup.py file. It contains metadata about your package like its name, version, author, and dependencies.
+
+Create a new file named "setup.py" in the project directory and add the following code:
+
+```
+from setuptools import setup, find_packages
+setup(
+name='mypackage',
+version='0.1.0',
+author='Your Name',
+author_email='your.email@example.com',
+description='A short description of your package',
+packages=find_packages(),
+classifiers=[
+'Programming Language :: Python :: 3',
+'License :: OSI Approved :: MIT License',
+'Operating System :: OS Independent',
+],
+python_requires='>=3.6',
+)
+```
+
+### **Step 6: Build the package**
+
+To build the package, run the following command in the project directory:
+
+```
+python setup.py sdist
+
+python setup.py sdist bdist_wheel
+```
+
+This will create a source distribution of your package in a new directory named "dist".
+
+### **Step 7: Upload the package to PyPI**
+
+To upload your package to PyPI, you first need to create an account on the [PyPI](https://pypi.org/account/register/) / [TestPyPI · The Python Package Index](https://test.pypi.org/) website
+
+Once done, run the following command in the project directory:
+
+```
+twine upload dist/*
+```
+
+This will upload your package to PyPI.
+
+# **Step 8: PyPi .pypirc location on windows**
+
+Your .pypirc file on windows should be in your `$HOME` directory.
+
+On windows this is typically your user folder under `C:\Users\`. For example my current home folder for the user `hiro` is `C:\Users\hiro\`
+
+This means that my `.pypirc` file should live at `C:\Users\hiro\.pypirc`.
+
+If .pypirc file is not existing for the user then create it with the help of below template. on pypi/testpypi, generate your respective API token and use it as your password below.
+
+# **Typical PyPi .pypirc file contents**
+
+Typically the PyPi file will include information for the pypi and testpypi server. If you have a token for each of these your file will look something like this
+
+Here the settings for pypi and testpypi
+
+```python
+[distutils]
+index-servers =
+    pypi
+    testpypi
+ 
+[pypi]
+repository = https://upload.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+ 
+[testpypi]
+repository = https://test.pypi.org/legacy/
+username = __token__
+password = <PyPI token>
+```
+
+### **Step 9: Install the package**
+
+To install your package from PyPI, run the following command:
+
+```
+pip install mypackage
+```
+
+Replace "mypackage" with the name of your package.
```

### Comparing `cogflow-1.6.0/cogflow/cog_framework.py` & `cogflow-1.8.1/cogflow/mlflowplugin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,130 +1,46 @@
 """
-CogFramework: A class for defining reusable components and pipelines for Kubeflow Pipelines.
-
-CogContainer: A subclass of Container that extends it with additional functionality for
-adding environment variables related to model access.
-
-CogFramework:
-- Initializes methods to add model access environment variables to Container classes.
-- Defines a static method `pipeline` to create pipeline decorators for defining Kubeflow Pipelines.
-- Provides methods for creating components from Python functions, managing the Kubeflow Pipeline client,
-and loading components from URLs.
-- Provides methods for defining InputPath and OutputPath components.
+This module provides functionality related to Mlflow.
 """
 
-import time
 import os
-from cogflow import constant_vars
-import pandas as pd
-import numpy as np
-import mlflow as ml
-import kfp
-import kserve
 from typing import Union
-from kubernetes.client.models import V1EnvVar
-from kfp import dsl
+
+import mlflow as ml
+import numpy as np
+import pandas as pd
+import requests
 from mlflow.models.signature import ModelSignature
-from scipy.sparse import csr_matrix, csc_matrix
-from kfp.components import InputPath, OutputPath
-from tenacity import retry, stop_after_attempt, wait_exponential
-from kserve import KServeClient
-from kubernetes import client
-from kserve import utils
 from mlflow.tracking import MlflowClient
-from datetime import datetime
-from kubernetes.client.exceptions import ApiException
-from kubernetes.client import V1ObjectMeta
-from kubernetes import client as k8s_client, config as k8s_config
-from kserve import (
-    constants,
-    KServeClient,
-    V1beta1InferenceService,
-    V1beta1InferenceServiceSpec,
-    V1beta1PredictorSpec,
-    V1beta1TFServingSpec,
-    V1beta1ModelFormat,
-    V1beta1ModelSpec,
-    V1beta1SKLearnSpec,
-)
-
-
-class CogContainer(kfp.dsl._container_op.Container):
-    """
-    Subclass of Container to add model access environment variables.
-    """
-
-    def __init__(self):
-        """
-        Initializes the CogContainer class.
-        """
-        super().__init__()
-
-    def AddModelAccess(self):
-        """
-        Adds model access environment variables to the container.
+from scipy.sparse import csr_matrix, csc_matrix
 
-        Returns:
-            CogContainer: Container instance with added environment variables.
-        """
-        return (
-            self.add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.TRACKING_URI,
-                    value=os.getenv(constant_vars.TRACKING_URI),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.S3_ENDPOINT_URL,
-                    value=os.getenv(constant_vars.S3_ENDPOINT_URL),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.ACCESS_KEY_ID,
-                    value=os.getenv(constant_vars.ACCESS_KEY_ID),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.SECRET_ACCESS_KEY,
-                    value=os.getenv(constant_vars.SECRET_ACCESS_KEY),
-                )
-            )
-        )
+from cogflow import plugin_config
 
 
 class CogModel(ml.pyfunc.PythonModel):
     """
-    A custom MLflow PythonModel implementation for demonstration purposes.
+    A custom Mlflow PythonModel implementation for demonstration purposes.
     """
 
-    def __init__(self):
-        """
-        Constructor for the CustomModel class.
-        """
-        pass
-
-    def fit(self):
+    @staticmethod
+    def fit():
         """
         Train the model.
 
         This method is called to train the model.
         """
         print("Fitting model...")
 
-    def predict(self, context, model_input: [str]):  # type: ignore
+    def predict(self, model_input: [str]):  # type: ignore
         """
         Generate predictions.
 
         This method generates predictions based on the input data.
 
         Parameters:
-            context (Any): Additional context or information passed to the prediction function.
             model_input (List[str]): List of input strings for prediction.
 
         Returns:
             None: This method prints the predictions instead of returning them.
         """
         print(self.get_prediction(model_input))
 
@@ -140,32 +56,61 @@
         Returns:
             str: The concatenated uppercase version of the input strings.
         """
 
         return " ".join([w.upper() for w in model_input])
 
 
-class CogFramework:
+class MlflowPlugin:
     """
-    Class for defining reusable components and pipelines for Kubeflow Pipelines.
+    Class for defining reusable components.
     """
 
     def __init__(self):
         """
-        Initializes the CogFramework class.
+        Initializes the MlFlowPlugin class.
         """
-        kfp.dsl._container_op.Container.AddModelAccess = self.AddModelAccess
-        kfp.dsl._container_op.ContainerOp.AddModelAccess = self.AddModelAccess
         self.mlflow = ml
         self.sklearn = ml.sklearn
-        self.tensorflow = ml.tensorflow
-        self.pytorch = ml.pytorch
+        self.cogclient = MlflowClient()
         self.pyfunc = ml.pyfunc
         self.models = ml.models
-        self.cogclient = MlflowClient()
+
+    def is_alive(self):
+        """
+        Check if Mlflow UI is accessible.
+
+        Returns:
+            tuple: A tuple containing a boolean indicating if Mlflow UI is accessible
+             and the status code of the response.
+        """
+        response = requests.get(os.getenv(plugin_config.TRACKING_URI))
+        try:
+            if response.status_code == 200:
+                return response.status_code, response.text
+            print(
+                f"Mlflow UI is not accessible. Status code: {response.status_code}, "
+                f"Message: {response.text}"
+            )
+        except Exception as e:
+            print(
+                f"An error occurred while accessing Mlflow UI: {str(e)}, "
+                f"Status code: {response.status_code}, Message: {response.text}"
+            )
+        return response.status_code, response.text
+
+    @staticmethod
+    def version():
+        """
+        Retrieve the version of the Mlflow.
+
+        Returns:
+            str: Version of the Mlflow.
+        """
+        return ml.__version__
 
     def delete_registered_model(self, model_name):
         """
         Deletes a registered model with the given name.
 
         Args:
             model_name (str): The name of the registered model to delete.
@@ -183,88 +128,77 @@
             list: A list of registered model objects matching the search criteria.
         """
         registered_models = self.cogclient.search_registered_models()
         return registered_models
 
     def load_model(self, model_name: str, model_version: int):
         """
-        Loads a model from MLflow.
+        Loads a model from Mlflow.
 
         Args:
-            model_name (str): The name of the registered MLflow model.
-            model_version (int): The version of the registered MLflow model.
+            model_name (str): The name of the registered Mlflow model.
+            model_version (int): The version of the registered Mlflow model.
 
         Returns:
             loaded_model: The loaded model.
         """
         model_uri = f"models:/{model_name}/{model_version}"
         loaded_model = ml.sklearn.load_model(model_uri)
         return loaded_model
 
     def register_model(self, model, model_uri):
         """
-        Registers the given model with MLflow.
+        Registers the given model with Mlflow.
 
         Args:
             model: The model object to register.
-            model_uri (str): The MLflow model URI.
+            model_uri (str): The Mlflow model URI.
         """
         return ml.register_model(model, model_uri)
 
     def autolog(self):
         """
-        Enable automatic logging of parameters, metrics, and models with MLflow.
+        Enable automatic logging of parameters, metrics, and models with Mlflow.
 
         Returns:
             None
         """
         return self.mlflow.autolog()
 
-    # def cogclient(self):
-    #     """
-    #     Get the MLflow Tracking client.
-
-    #     Returns:
-    #         MlflowClient: MLflow Tracking client instance.
-    #     """
-    #     return MlflowClient()
-
     def create_registered_model(self, name):
         """
         Create a registered model.
 
         Args:
             name (str): Name of the registered model.
 
         Returns:
             str: ID of the created registered model.
         """
-        # client = self.cogclient()
         return self.cogclient.create_registered_model(name)
 
     def create_model_version(self, name, source):
         """
         Create a model version for a registered model.
 
         Args:
             name (str): Name of the registered model.
             source (str): Source path or URI of the model.
 
         Returns:
             str: ID of the created model version.
         """
-        # client = self.cogclient()
         return self.cogclient.create_model_version(name, source)
 
     def set_tracking_uri(self, tracking_uri):
         """
-        Set the MLflow tracking URI.
+        Set the Mlflow tracking URI.
 
         Args:
-            tracking_uri (str): The URI of the MLflow tracking server.
+            tracking_uri (str): The URI of the Mlflow tracking server.
 
         Returns:
             None
         """
         return self.mlflow.set_tracking_uri(tracking_uri)
 
     def set_experiment(self, experiment_name):
@@ -277,70 +211,66 @@
         Returns:
             None
         """
         return self.mlflow.set_experiment(experiment_name)
 
     def get_artifact_uri(self, run_id=None):
         """
-        Get the artifact URI of the current or specified MLflow run.
+        Get the artifact URI of the current or specified Mlflow run.
 
         Args:
-            run_id (str, optional): ID of the MLflow run. If not provided, the current run's artifact URI is returned.
+            run_id (str, optional): ID of the Mlflow run. If not provided,
+            the current run's artifact URI is returned.
 
         Returns:
-            str: Artifact URI of the specified MLflow run.
+            str: Artifact URI of the specified Mlflow run.
         """
         return self.mlflow.get_artifact_uri(run_id)
 
-    def start_run(self, experiment_name=None, run_name=None):
+    def start_run(self, run_name=None):
         """
-        Start an MLflow run.
+        Start a Mlflow run.
 
         Args:
-            experiment_name (str): Name of the MLflow experiment to log the run to.
-            run_name (str): Name of the MLflow run.
+            run_name (str): Name of the Mlflow run.
 
         Returns:
-            MLflow Run object
+            Mlflow Run object
         """
         return self.mlflow.start_run(run_name=run_name)
 
     def end_run(self):
         """
-        Start an MLflow run.
-
-        Args:
-            experiment_name (str): Name of the MLflow experiment to log the run to.
-            run_name (str): Name of the MLflow run.
+        End a Mlflow run.
 
         Returns:
-            MLflow Run object
+            Mlflow Run object
         """
         return self.mlflow.end_run()
 
     def log_param(self, *args):
         """
-        Log parameters to the MLflow run.
+        Log parameters to the Mlflow run.
 
         Args:
-            run: MLflow Run object returned by start_mlflow_run method.
-            params (dict): Dictionary containing parameters to log.
+            run: Mlflow Run object returned by start_mlflow_run method.
+            param: Containing parameters to log.
 
         Returns:
             None
         """
         return self.mlflow.log_param(*args)
 
     def log_metric(self, *args):
         """
-        Log metrics to the MLflow run.
+        Log metrics to the Mlflow run.
 
         Args:
-            run: MLflow Run object returned by start_mlflow_run method.
-            metrics (dict): Dictionary containing metrics to log.
+            run: Mlflow Run object returned by start_mlflow_run method.
+            metric: Containing metrics to log.
 
         Returns:
             None
         """
         return self.mlflow.log_metric(*args)
 
     def log_model(
@@ -365,14 +295,51 @@
         ] = None,
         await_registration_for=300,
         pip_requirements=None,
         extra_pip_requirements=None,
         pyfunc_predict_fn="predict",
         metadata=None,
     ):
+        """
+        Log a scikit-learn model to Mlflow.
+
+        Args:
+            sk_model: The scikit-learn model to be logged.
+            artifact_path (str): The run-relative artifact path to which the model artifacts will
+            be saved.
+            conda_env (str, optional): The path to a Conda environment YAML file. Defaults to None.
+            code_paths (list, optional): A list of local filesystem paths to Python files that
+            contain code to be
+            included as part of the model's logged artifacts. Defaults to None.
+            serialization_format (str, optional): The format used to serialize the model. Defaults
+            to "cloudpickle".
+            registered_model_name (str, optional): The name under which to register the model with
+            Mlflow. Defaults to None.
+            signature (ModelSignature, optional): The signature defining model input and output
+            data types and shapes. Defaults to None.
+            input_example (Union[pd.DataFrame, np.ndarray, dict, list, csr_matrix, csc_matrix, str,
+            bytes, tuple], optional): An example input to the model. Defaults to None.
+            await_registration_for (int, optional): The duration, in seconds, to wait for the
+            model version to finish being created and is in the READY status. Defaults to 300.
+            pip_requirements (str, optional): A file in pip requirements format specifying
+            additional pip dependencies for the model environment. Defaults to None.
+            extra_pip_requirements (str, optional): A string containing additional pip dependencies
+            that should be added to the environment. Defaults to None.
+            pyfunc_predict_fn (str, optional): The name of the function to invoke for prediction,
+            when the model is a PyFunc model. Defaults to "predict".
+            metadata (dict, optional): A dictionary of metadata to log with the model.
+            Defaults to None.
+
+        Returns:
+            Model: The logged scikit-learn model.
+
+        Raises:
+            Exception: If an error occurs during the logging process.
+
+        """
         return self.mlflow.sklearn.log_model(
             sk_model=sk_model,
             artifact_path=artifact_path,
             conda_env=conda_env,
             code_paths=code_paths,
             serialization_format=serialization_format,
             registered_model_name=registered_model_name,
@@ -380,228 +347,7 @@
             input_example=input_example,
             await_registration_for=await_registration_for,
             pip_requirements=pip_requirements,
             extra_pip_requirements=extra_pip_requirements,
             pyfunc_predict_fn=pyfunc_predict_fn,
             metadata=metadata,
         )
-
-    def pipeline(name=None, description=None):
-        """
-        Decorator function to define Kubeflow Pipelines.
-
-        Args:
-            name (str, optional): Name of the pipeline. Defaults to None.
-            description (str, optional): Description of the pipeline. Defaults to None.
-
-        Returns:
-            Callable: Decorator for defining Kubeflow Pipelines.
-        """
-        return dsl.pipeline(name=name, description=description)
-
-    def create_component_from_func(
-        func, output_component_file=None, base_image=None, packages_to_install=None
-    ):
-        """
-        Create a component from a Python function.
-
-        Args:
-            func (Callable): Python function to convert into a component.
-            output_component_file (str, optional): Path to save the component YAML file. Defaults to None.
-            base_image (str, optional): Base Docker image for the component. Defaults to None.
-            packages_to_install (List[str], optional): List of additional Python packages to install in the component.
-            Defaults to None.
-
-        Returns:
-            kfp.components.ComponentSpec: Component specification.
-        """
-        training_var = kfp.components.create_component_from_func(
-            func=func,
-            output_component_file=output_component_file,
-            base_image=base_image,
-            packages_to_install=packages_to_install,
-        )
-        kfp.dsl._container_op.ContainerOp.AddModelAccess = CogFramework.AddModelAccess
-        return training_var
-
-    def client():
-        """
-        Get the Kubeflow Pipeline client.
-
-        Returns:
-            kfp.Client: Kubeflow Pipeline client instance.
-        """
-        return kfp.Client()
-
-    def load_component_from_url(url):
-        """
-        Load a component from a URL.
-
-        Args:
-            url (str): URL to load the component from.
-
-        Returns:
-            kfp.components.ComponentSpec: Loaded component specification.
-        """
-        return kfp.components.load_component_from_url(url)
-
-    def InputPath(label: str):
-        """
-        Create an InputPath component.
-
-        Args:
-            label (str): Label for the input path.
-
-        Returns:
-            InputPath: InputPath component instance.
-        """
-        return kfp.components.InputPath(label)
-
-    def OutputPath(label: str):
-        """
-        Create an OutputPath component.
-
-        Args:
-            label (str): Label for the output path.
-
-        Returns:
-            OutputPath: OutputPath component instance.
-        """
-        return kfp.components.OutputPath(label)
-
-    def AddModelAccess(self):
-        """
-        Add model access environment variables to the container.
-
-        Returns:
-            CogContainer: Container instance with added environment variables.
-        """
-        return (
-            self.add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.TRACKING_URI,
-                    value=os.getenv(constant_vars.TRACKING_URI),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.S3_ENDPOINT_URL,
-                    value=os.getenv(constant_vars.S3_ENDPOINT_URL),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.ACCESS_KEY_ID,
-                    value=os.getenv(constant_vars.ACCESS_KEY_ID),
-                )
-            )
-            .add_env_variable(
-                V1EnvVar(
-                    name=constant_vars.SECRET_ACCESS_KEY,
-                    value=os.getenv(constant_vars.SECRET_ACCESS_KEY),
-                )
-            )
-        )
-
-    def Serve_Model_v2(model_uri: str, name: str):
-        """
-        Create a kserve instance.
-
-        Args:
-            model_uri (str): URI of the model.
-            name (str, optional): Name of the kserve instance. If not provided, a default name will be generated.
-
-        Returns:
-            None
-        """
-
-        namespace = utils.get_default_target_namespace()
-        if name is None:
-            now = datetime.now()
-            v = now.strftime("%d%M")
-            name = "predictor_model{}".format(v)
-        ISVC_NAME = name
-        predictor = V1beta1PredictorSpec(
-            service_account_name="kserve-controller-s3",
-            min_replicas=1,
-            model=V1beta1ModelSpec(
-                model_format=V1beta1ModelFormat(
-                    name=constant_vars.ML_TOOL,
-                ),
-                storage_uri=model_uri,
-                protocol_version="v2",
-            ),
-        )
-
-        isvc = V1beta1InferenceService(
-            api_version=constants.KSERVE_V1BETA1,
-            kind=constants.KSERVE_KIND,
-            metadata=client.V1ObjectMeta(
-                name=ISVC_NAME,
-                namespace=namespace,
-                annotations={"sidecar.istio.io/inject": "false"},
-            ),
-            spec=V1beta1InferenceServiceSpec(predictor=predictor),
-        )
-        KServe = KServeClient()
-        try:
-            KServe.create(isvc)
-        except ApiException as e:
-            if e.status == 409:
-                # Handle the conflict error
-                print("Inference service already exists.")
-            else:
-                #    Handle other ApiException errors
-                print("An error occurred:", e)
-
-    def Serve_Model_v1(model_uri: str, name: str):
-        """
-        Create a kserve instance version1.
-
-        Args:
-            model_uri (str): URI of the model.
-            name (str, optional): Name of the kserve instance. If not provided, a default name will be generated.
-
-        Returns:
-            None
-        """
-
-        ISVC_NAME = name
-        namespace = utils.get_default_target_namespace()
-        isvc = V1beta1InferenceService(
-            api_version=constants.KSERVE_V1BETA1,
-            kind=constants.KSERVE_KIND,
-            metadata=V1ObjectMeta(
-                name=ISVC_NAME,
-                namespace=namespace,
-                annotations={"sidecar.istio.io/inject": "false"},
-            ),
-            spec=V1beta1InferenceServiceSpec(
-                predictor=V1beta1PredictorSpec(
-                    service_account_name="kserve-controller-s3",
-                    sklearn=V1beta1SKLearnSpec(storage_uri=model_uri),
-                )
-            ),
-        )
-
-        client = KServeClient()
-        client.create(isvc)
-        time.sleep(constant_vars.Timer_IN_SEC)
-
-    def GetModelUrl(modelName: str):
-        """
-        Retrieve the URL of a deployed model.
-
-        Args:
-            modelName (str): Name of the deployed model.
-
-        Returns:
-            str: URL of the deployed model.
-        """
-        client = KServeClient()
-        namespace = utils.get_default_target_namespace()
-
-        time.sleep(constant_vars.Timer_IN_SEC)
-        isvc_resp = client.get(modelName)
-        isvc_url = isvc_resp["status"]["address"]["url"]
-        print(isvc_url)
-        return isvc_url
```

