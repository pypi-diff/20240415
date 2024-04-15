# Comparing `tmp/heart_library-0.3.0.tar.gz` & `tmp/heart_library-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heart_library-0.3.0.tar", max compression
+gzip compressed data, was "heart_library-0.3.1.tar", max compression
```

## Comparing `heart_library-0.3.0.tar` & `heart_library-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1088 2024-04-01 15:44:12.741325 heart_library-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     2954 2024-04-01 15:44:12.741397 heart_library-0.3.0/README.md
--rw-r--r--   0        0        0     2532 2024-04-01 17:51:12.151314 heart_library-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-01 15:44:12.843608 heart_library-0.3.0/src/heart_library/__init__.py
--rw-r--r--   0        0        0        0 2024-04-01 15:44:12.843669 heart_library-0.3.0/src/heart_library/attacks/__init__.py
--rw-r--r--   0        0        0     3406 2024-04-01 15:44:12.843758 heart_library-0.3.0/src/heart_library/attacks/attack.py
--rw-r--r--   0        0        0      310 2024-04-01 15:44:12.843843 heart_library-0.3.0/src/heart_library/attacks/evasion/__init__.py
--rw-r--r--   0        0        0    12926 2024-04-01 15:44:12.843980 heart_library-0.3.0/src/heart_library/attacks/evasion/auto_attack.py
--rw-r--r--   0        0        0     9863 2024-04-01 15:44:12.844061 heart_library-0.3.0/src/heart_library/attacks/evasion/laser_attack.py
--rw-r--r--   0        0        0     3034 2024-04-01 15:44:12.844144 heart_library-0.3.0/src/heart_library/attacks/evasion/query_efficient_bb_attack.py
--rw-r--r--   0        0        0     2578 2024-04-01 15:44:12.844214 heart_library-0.3.0/src/heart_library/attacks/typing.py
--rw-r--r--   0        0        0     3928 2024-04-01 15:44:12.844275 heart_library-0.3.0/src/heart_library/config.py
--rw-r--r--   0        0        0        0 2024-04-01 15:44:12.844333 heart_library-0.3.0/src/heart_library/estimators/__init__.py
--rw-r--r--   0        0        0      234 2024-04-01 15:44:12.844468 heart_library-0.3.0/src/heart_library/estimators/classification/__init__.py
--rw-r--r--   0        0        0     3007 2024-04-01 15:44:12.844540 heart_library-0.3.0/src/heart_library/estimators/classification/pytorch.py
--rw-r--r--   0        0        0     2531 2024-04-01 15:44:12.844608 heart_library-0.3.0/src/heart_library/estimators/classification/query_efficient_bb.py
--rw-r--r--   0        0        0      170 2024-04-01 15:44:12.844688 heart_library-0.3.0/src/heart_library/estimators/object_detection/__init__.py
--rw-r--r--   0        0        0     4520 2024-04-01 15:44:12.844787 heart_library-0.3.0/src/heart_library/estimators/object_detection/pytorch_yolo.py
--rw-r--r--   0        0        0      227 2024-04-01 15:44:12.844895 heart_library-0.3.0/src/heart_library/metrics/__init__.py
--rw-r--r--   0        0        0     9167 2024-04-01 15:44:12.844967 heart_library-0.3.0/src/heart_library/metrics/metrics.py
--rw-r--r--   0        0        0     4438 2024-04-01 15:44:12.845041 heart_library-0.3.0/src/heart_library/utils.py
--rw-r--r--   0        0        0     5107 1970-01-01 00:00:00.000000 heart_library-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-04-15 17:29:21.874476 heart_library-0.3.1/LICENSE.txt
+-rw-r--r--   0        0        0     2954 2024-04-15 17:29:21.874559 heart_library-0.3.1/README.md
+-rw-r--r--   0        0        0     2700 2024-04-15 17:29:22.017691 heart_library-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-04-15 17:29:22.017929 heart_library-0.3.1/src/heart_library/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 17:29:22.018000 heart_library-0.3.1/src/heart_library/attacks/__init__.py
+-rw-r--r--   0        0        0     3406 2024-04-15 17:29:22.018100 heart_library-0.3.1/src/heart_library/attacks/attack.py
+-rw-r--r--   0        0        0      310 2024-04-15 17:29:22.018215 heart_library-0.3.1/src/heart_library/attacks/evasion/__init__.py
+-rw-r--r--   0        0        0    12926 2024-04-15 17:29:22.018346 heart_library-0.3.1/src/heart_library/attacks/evasion/auto_attack.py
+-rw-r--r--   0        0        0     9863 2024-04-15 17:29:22.018518 heart_library-0.3.1/src/heart_library/attacks/evasion/laser_attack.py
+-rw-r--r--   0        0        0     3034 2024-04-15 17:29:22.018593 heart_library-0.3.1/src/heart_library/attacks/evasion/query_efficient_bb_attack.py
+-rw-r--r--   0        0        0     2578 2024-04-15 17:29:22.018677 heart_library-0.3.1/src/heart_library/attacks/typing.py
+-rw-r--r--   0        0        0     3928 2024-04-15 17:29:22.018756 heart_library-0.3.1/src/heart_library/config.py
+-rw-r--r--   0        0        0        0 2024-04-15 17:29:22.018835 heart_library-0.3.1/src/heart_library/estimators/__init__.py
+-rw-r--r--   0        0        0      234 2024-04-15 17:29:22.018968 heart_library-0.3.1/src/heart_library/estimators/classification/__init__.py
+-rw-r--r--   0        0        0     3007 2024-04-15 17:29:22.019056 heart_library-0.3.1/src/heart_library/estimators/classification/pytorch.py
+-rw-r--r--   0        0        0     2531 2024-04-15 17:29:22.019142 heart_library-0.3.1/src/heart_library/estimators/classification/query_efficient_bb.py
+-rw-r--r--   0        0        0      170 2024-04-15 17:29:22.019252 heart_library-0.3.1/src/heart_library/estimators/object_detection/__init__.py
+-rw-r--r--   0        0        0     4723 2024-04-15 17:29:22.019346 heart_library-0.3.1/src/heart_library/estimators/object_detection/pytorch_yolo.py
+-rw-r--r--   0        0        0      227 2024-04-15 17:29:22.019451 heart_library-0.3.1/src/heart_library/metrics/__init__.py
+-rw-r--r--   0        0        0     9167 2024-04-15 17:29:22.019621 heart_library-0.3.1/src/heart_library/metrics/metrics.py
+-rw-r--r--   0        0        0     4438 2024-04-15 17:29:22.019727 heart_library-0.3.1/src/heart_library/utils.py
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 heart_library-0.3.1/PKG-INFO
```

### Comparing `heart_library-0.3.0/LICENSE.txt` & `heart_library-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/README.md` & `heart_library-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/pyproject.toml` & `heart_library-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "heart-library"
-version = "0.3.0"
+version = "0.3.1"
 description = "Hardened Extension of the Adversarial Robustness Toolbox (HEART) supports assessment of adversarial AI vulnerabilities in Test & Evaluation workflows."
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/IBM/heart-library"
 packages = [{include = "heart_library", from = "src" }]
 keywords = [
     "machine learning",
@@ -15,30 +15,32 @@
 authors = ["Mark Baker, Jordan Fischer, Kieran Fraser, Jackson Lee, Adam Lockwood"]
 
 
 [tool.poetry.dependencies]
 # HEART Required Dependences
 python = ">=3.9, <3.11"
 adversarial-robustness-toolbox = ">=1.17.1"
-maite = ">=0.4.0,<0.5.0"
+maite = ">=0.4.0, <0.5.0"
 numpy = ">=1.18.5, <2"
 scikit-learn = ">=0.22.2"
 six = "*"
 setuptools = "*"
 tqdm = "*"
 
 # HEART Optional Dependencies
-datasets = { version = "*", optional = true }
-gradio = { version = ">=4.13.0,<4.24.0", optional = true }
+datasets = { version = ">=2.18.0", optional = true }
+gradio = { version = ">=4.13.0, <4.24.0", optional = true }
 jupyter = { version = "*", optional = true}
 matplotlib = { version = "*", optional = true }
 multiprocess = { version = "*", optional = true }
 numba = { version = "*", optional = true }
 pandas = { version = "*", optional = true }
 Pillow = { version = "*", optional = true }
+sphinx = { version = ">=4.2.0", optional = true }
+furo = { version = "*", optional = true }
 torch = { version = "*", optional = true }
 torchvision = { version = "*", optional = true }
 yolov5 = { version = "*", optional = true }
 
 
 [tool.poetry.extras]
 # All Optional Dependencies
@@ -92,14 +94,20 @@
 gradio = [
     "datasets",
     "gradio",
     "matplotlib",
     "pandas",
 ]
 
+# Optional Sphinx Dependencies
+docs = [
+    "sphinx",
+    "furo"
+]
+
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 isort = "*"
@@ -115,8 +123,7 @@
 [tool.black]
 line-length=120
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
```

### Comparing `heart_library-0.3.0/src/heart_library/__init__.py` & `heart_library-0.3.1/src/heart_library/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The HEART extension.
 """
 import logging.config
 
 # Project Imports
 
 # Semantic Version
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 
 # pylint: disable=C0103
 
 LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {
```

### Comparing `heart_library-0.3.0/src/heart_library/attacks/attack.py` & `heart_library-0.3.1/src/heart_library/attacks/attack.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/attacks/evasion/auto_attack.py` & `heart_library-0.3.1/src/heart_library/attacks/evasion/auto_attack.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/attacks/evasion/laser_attack.py` & `heart_library-0.3.1/src/heart_library/attacks/evasion/laser_attack.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/attacks/evasion/query_efficient_bb_attack.py` & `heart_library-0.3.1/src/heart_library/attacks/evasion/query_efficient_bb_attack.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/attacks/typing.py` & `heart_library-0.3.1/src/heart_library/attacks/typing.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/config.py` & `heart_library-0.3.1/src/heart_library/config.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/estimators/classification/pytorch.py` & `heart_library-0.3.1/src/heart_library/estimators/classification/pytorch.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/estimators/classification/query_efficient_bb.py` & `heart_library-0.3.1/src/heart_library/estimators/classification/query_efficient_bb.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/estimators/object_detection/pytorch_yolo.py` & `heart_library-0.3.1/src/heart_library/estimators/object_detection/pytorch_yolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -93,17 +93,21 @@
 class JaticPyTorchYolo(PyTorchYolo):  # pylint: disable=R0901
     """
     JATIC compatible extension of ART core PyTorchYolo
     """
 
     metadata: HeartObjectDetectionMetadata
 
-    def __init__(self, labels: Sequence[str], **kwargs: Any):
+    def __init__(self, labels: Sequence[str], model_path: str = "yolov5s.pt", **kwargs: Any):
+        model = None
+        try:
+            model = yolov5.load(model_path)
+        except Exception as load_exception:
+            raise Exception("Yolov5 model was not successful loaded.") from load_exception
 
-        model = yolov5.load("yolov5s.pt")
         model = Yolo(model, kwargs["device_type"])
         super().__init__(model=model, **kwargs)
 
         if labels is None:
             raise InvalidArgument("No labels were provided.")
         self._labels: Sequence[str] = labels
         self.metadata = HeartObjectDetectionMetadata(model_name="YOLOv5", provider="yolov5")
```

### Comparing `heart_library-0.3.0/src/heart_library/metrics/metrics.py` & `heart_library-0.3.1/src/heart_library/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/src/heart_library/utils.py` & `heart_library-0.3.1/src/heart_library/utils.py`

 * *Files identical despite different names*

### Comparing `heart_library-0.3.0/PKG-INFO` & `heart_library-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: heart-library
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hardened Extension of the Adversarial Robustness Toolbox (HEART) supports assessment of adversarial AI vulnerabilities in Test & Evaluation workflows.
 Home-page: https://github.com/IBM/heart-library
 License: MIT
 Keywords: machine learning,adversarial ai,evasion
 Author: Mark Baker, Jordan Fischer, Kieran Fraser, Jackson Lee, Adam Lockwood
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: all
+Provides-Extra: docs
 Provides-Extra: gradio
 Provides-Extra: image-classification
 Provides-Extra: non-framework
 Provides-Extra: notebooks
 Provides-Extra: object-detection
 Provides-Extra: pytorch
 Provides-Extra: yolov5
 Requires-Dist: Pillow ; extra == "all" or extra == "non-framework"
 Requires-Dist: adversarial-robustness-toolbox (>=1.17.1)
-Requires-Dist: datasets ; extra == "all" or extra == "non-framework" or extra == "gradio"
+Requires-Dist: datasets (>=2.18.0) ; extra == "all" or extra == "non-framework" or extra == "gradio"
+Requires-Dist: furo ; extra == "docs"
 Requires-Dist: gradio (>=4.13.0,<4.24.0) ; extra == "gradio"
 Requires-Dist: jupyter ; extra == "all" or extra == "non-framework" or extra == "notebooks"
 Requires-Dist: maite (>=0.4.0,<0.5.0)
 Requires-Dist: matplotlib ; extra == "all" or extra == "non-framework" or extra == "notebooks" or extra == "gradio"
 Requires-Dist: multiprocess ; extra == "all" or extra == "non-framework"
 Requires-Dist: numba ; extra == "all" or extra == "non-framework"
 Requires-Dist: numpy (>=1.18.5,<2)
 Requires-Dist: pandas ; extra == "all" or extra == "non-framework" or extra == "notebooks" or extra == "gradio"
 Requires-Dist: scikit-learn (>=0.22.2)
 Requires-Dist: setuptools
 Requires-Dist: six
+Requires-Dist: sphinx (>=4.2.0) ; extra == "docs"
 Requires-Dist: torch ; extra == "all" or extra == "pytorch" or extra == "image-classification"
 Requires-Dist: torchvision ; extra == "all" or extra == "pytorch" or extra == "image-classification"
 Requires-Dist: tqdm
 Requires-Dist: yolov5 ; extra == "all" or extra == "yolov5" or extra == "object-detection"
 Project-URL: Repository, https://github.com/IBM/heart-library
 Description-Content-Type: text/markdown
```

