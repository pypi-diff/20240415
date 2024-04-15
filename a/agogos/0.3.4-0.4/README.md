# Comparing `tmp/agogos-0.3.4.tar.gz` & `tmp/agogos-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agogos-0.3.4.tar", last modified: Tue Apr  2 09:32:56 2024, max compression
+gzip compressed data, was "agogos-0.4.tar", last modified: Mon Apr 15 13:16:39 2024, max compression
```

## Comparing `agogos-0.3.4.tar` & `agogos-0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:32:56.743682 agogos-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 09:32:53.000000 agogos-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-02 09:32:56.743682 agogos-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 09:32:53.000000 agogos-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:32:56.739682 agogos-0.3.4/agogos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 09:32:53.000000 agogos-0.3.4/agogos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-04-02 09:32:53.000000 agogos-0.3.4/agogos/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-04-02 09:32:53.000000 agogos-0.3.4/agogos/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     6644 2024-04-02 09:32:53.000000 agogos-0.3.4/agogos/transforming.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:32:56.743682 agogos-0.3.4/agogos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-02 09:32:56.000000 agogos-0.3.4/agogos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-02 09:32:56.000000 agogos-0.3.4/agogos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 09:32:56.000000 agogos-0.3.4/agogos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 09:32:56.000000 agogos-0.3.4/agogos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 09:32:56.000000 agogos-0.3.4/agogos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-02 09:32:53.000000 agogos-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 09:32:56.743682 agogos-0.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 09:32:56.743682 agogos-0.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-02 09:32:53.000000 agogos-0.3.4/tests/test__core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17074 2024-04-02 09:32:53.000000 agogos-0.3.4/tests/test_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     8629 2024-04-02 09:32:53.000000 agogos-0.3.4/tests/test_transforming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:16:39.313861 agogos-0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 13:16:35.000000 agogos-0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-15 13:16:39.313861 agogos-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-15 13:16:35.000000 agogos-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:16:39.309861 agogos-0.4/agogos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:16:35.000000 agogos-0.4/agogos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-15 13:16:35.000000 agogos-0.4/agogos/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15450 2024-04-15 13:16:35.000000 agogos-0.4/agogos/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7165 2024-04-15 13:16:35.000000 agogos-0.4/agogos/transforming.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:16:39.313861 agogos-0.4/agogos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-15 13:16:39.000000 agogos-0.4/agogos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-15 13:16:39.000000 agogos-0.4/agogos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:16:39.000000 agogos-0.4/agogos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 13:16:39.000000 agogos-0.4/agogos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:16:39.000000 agogos-0.4/agogos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-15 13:16:35.000000 agogos-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:16:39.313861 agogos-0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:16:39.313861 agogos-0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-15 13:16:35.000000 agogos-0.4/tests/test__core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-15 13:16:35.000000 agogos-0.4/tests/test_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-15 13:16:35.000000 agogos-0.4/tests/test_transforming.py
```

### Comparing `agogos-0.3.4/LICENSE` & `agogos-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `agogos-0.3.4/PKG-INFO` & `agogos-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agogos
-Version: 0.3.4
+Version: 0.4
 Summary: Package that creates the underlying construction of a machine learning pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 </p>
 
 ## Pytest coverage report
 
 To generate pytest coverage report run
 
 ```shell
-pytest --cov=agogos --cov-report=html:coverage_re
+python -m pytest --cov=agogos --cov-report=html:coverage_re
 ```
 
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
```

### Comparing `agogos-0.3.4/README.md` & `agogos-0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 </p>
 
 ## Pytest coverage report
 
 To generate pytest coverage report run
 
 ```shell
-pytest --cov=agogos --cov-report=html:coverage_re
+python -m pytest --cov=agogos --cov-report=html:coverage_re
 ```
 
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
```

### Comparing `agogos-0.3.4/agogos/_core.py` & `agogos-0.4/agogos/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """This module contains the core classes for all classes in the agogos package."""
-from pathlib import Path
-from dataclasses import field, dataclass
-from joblib import hash
 from abc import abstractmethod
+from dataclasses import field, dataclass
+from pathlib import Path
 from typing import Any
 
+from joblib import hash
+
 
 @dataclass
 class _Base:
     """The _Base class is the base class for all classes in the agogos package.
 
     Methods:
     .. code-block:: python
@@ -125,14 +126,15 @@
 
 @dataclass
 class _ParallelSystem(_Base):
     """The _System class is the base class for all systems.
 
     Parameters:
     - steps (list[_Base]): The steps in the system.
+    - weights (list[float]): Weights of steps in the system, if not specified they are equal.
 
     Methods:
     .. code-block:: python
         @abstractmethod
         def concat(self, original_data: Any), data_to_concat: Any, weight: float = 1.0) -> Any:
             # Specifies how to concat data after parallel computations
 
@@ -146,34 +148,54 @@
             # Get the children of the block
 
         def save_to_html(self, file_path: Path) -> None:
             # Save html format to file_path
     """
 
     steps: list[_Base] = field(default_factory=list)
+    weights: list[float] = field(default_factory=list)
 
     def __post_init__(self) -> None:
         """Post init function of _System class"""
+
+        # Sort the steps by name, to ensure consistent ordering of parallel computations
+        self.steps = sorted(self.steps, key=lambda x: x.__class__.__name__)
+
         super().__post_init__()
 
         # Set parent and children
         for step in self.steps:
             step._set_parent(self)
 
+        # Set weights if they exist
+        if len(self.weights) == len(self.get_steps()):
+            [w / sum(self.weights) for w in self.weights]
+        else:
+            num_steps = len(self.get_steps())
+            self.weights = [1 / num_steps for x in self.steps]
+
         self._set_children(self.steps)
 
     def get_steps(self) -> list[_Base]:
         """Return list of steps of _ParallelSystem
 
         :return: List of steps
         """
         if self.steps is None:
             return []
         return self.steps
 
+    def get_weights(self) -> list[float]:
+        """Return list of weights of _ParallelSystem
+
+        :return: List of weights"""
+        if len(self.get_steps()) != len(self.weights):
+            raise TypeError("Mismatch between weights and steps")
+        return self.weights
+
     def _set_hash(self, prev_hash: str) -> None:
         """Set the hash of the system.
 
         :param prev_hash: The hash of the previous block.
         """
         self._hash = prev_hash
```

### Comparing `agogos-0.3.4/agogos/training.py` & `agogos-0.4/agogos/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-from abc import abstractmethod
 import copy
-from joblib import hash
-from typing import Any
+import warnings
+
+from abc import abstractmethod
+
 from dataclasses import dataclass
+from typing import Any
+
+from joblib import hash
+
 from agogos._core import _Block, _SequentialSystem, _ParallelSystem, _Base
 from agogos.transforming import TransformingSystem
 
 
 class TrainType(_Base):
     """Abstract train type describing a class that implements two functions train and predict"""
 
@@ -128,14 +133,26 @@
     def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
         """Train the system.
 
         :param x: The input to the system.
         :param y: The output of the system.
         :return: The input and output of the system."""
 
+        set_of_steps = set()
+        for step in self.steps:
+            step_name = step.__class__.__name__
+            set_of_steps.add(step_name)
+
+        if set_of_steps != set(train_args.keys()):
+            # Raise a warning and print all the keys that do not match
+            warnings.warn(
+                f"The following steps do not exist but were given in the kwargs: {set(train_args.keys()) - set_of_steps}",
+                UserWarning,
+            )
+
         # Loop through each step and call the train method
         for step in self.steps:
             step_name = step.__class__.__name__
 
             step_args = train_args.get(step_name, {})
             if isinstance(step, (TrainType)):
                 x, y = step.train(x, y, **step_args)
@@ -147,14 +164,26 @@
     def predict(self, x: Any, **pred_args: Any) -> Any:
         """Predict the output of the system.
 
         :param x: The input to the system.
         :return: The output of the system.
         """
 
+        set_of_steps = set()
+        for step in self.steps:
+            step_name = step.__class__.__name__
+            set_of_steps.add(step_name)
+
+        if set_of_steps != set(pred_args.keys()):
+            # Raise a warning and print all the keys that do not match
+            warnings.warn(
+                f"The following steps do not exist but were given in the kwargs: {set(pred_args.keys()) - set_of_steps}",
+                UserWarning,
+            )
+
         # Loop through each step and call the predict method
         for step in self.steps:
             step_name = step.__class__.__name__
 
             step_args = pred_args.get(step_name, {})
 
             if isinstance(step, (TrainType)):
@@ -166,14 +195,15 @@
 
 
 class ParallelTrainingSystem(TrainType, _ParallelSystem):
     """A system that trains the input data in parallel.
 
     Parameters:
     - steps (list[Trainer | TrainingSystem | ParallelTrainingSystem]): The steps in the system.
+    - weights (list[float]): The weights of steps in the system, if not specified they are all equal.
 
     Methods:
     .. code-block:: python
         @abstractmethod
         def concat(self, data1: Any, data2: Any) -> Any: # Concatenate the transformed data.
 
         def train(self, x: Any, y: Any) -> tuple[Any, Any]: # Train the system.
@@ -216,52 +246,50 @@
 
         :param x: The input to the system.
         :param y: The expected output of the system.
         :return: The input and output of the system.
         """
 
         # Loop through each step and call the train method
-        num_steps = len(self.steps)
         out_x, out_y = None, None
         for i, step in enumerate(self.steps):
             step_name = step.__class__.__name__
 
             step_args = train_args.get(step_name, {})
 
             if isinstance(step, (TrainType)):
                 step_x, step_y = step.train(
                     copy.deepcopy(x), copy.deepcopy(y), **step_args
                 )
                 out_x, out_y = (
-                    self.concat(out_x, step_x, 1 / num_steps),
-                    self.concat_labels(out_y, step_y, 1 / num_steps),
+                    self.concat(out_x, step_x, self.get_weights()[i]),
+                    self.concat_labels(out_y, step_y, self.get_weights()[i]),
                 )
             else:
                 raise TypeError(f"{step} is not an instance of TrainType")
 
         return out_x, out_y
 
     def predict(self, x: Any, **pred_args: Any) -> Any:
         """Predict the output of the system.
 
         :param x: The input to the system.
         :return: The output of the system.
         """
 
         # Loop through each trainer and call the predict method
-        num_steps = len(self.steps)
         out_x = None
         for i, step in enumerate(self.steps):
             step_name = step.__class__.__name__
 
             step_args = pred_args.get(step_name, {})
 
             if isinstance(step, (TrainType)):
                 step_x = step.predict(copy.deepcopy(x), **step_args)
-                out_x = self.concat(out_x, step_x, 1 / num_steps)
+                out_x = self.concat(out_x, step_x, self.get_weights()[i])
             else:
                 raise TypeError(f"{step} is not an instance of TrainType")
 
         return out_x
 
     def concat_labels(
         self, original_data: Any, data_to_concat: Any, weight: float = 1.0
```

### Comparing `agogos-0.3.4/agogos/transforming.py` & `agogos-0.4/agogos/transforming.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
+import copy
 from abc import abstractmethod
 from typing import Any
-import copy
+
+import warnings
+
 
 from agogos._core import _Block, _SequentialSystem, _ParallelSystem, _Base
 
 
 class TransformType(_Base):
     """Abstract transform type describing a class that implements the transform function"""
 
@@ -104,14 +107,24 @@
     def transform(self, data: Any, **transform_args: Any) -> Any:
         """Transform the input data.
 
         :param data: The input data.
         :return: The transformed data.
         """
 
+        set_of_steps = set()
+        for step in self.steps:
+            step_name = step.__class__.__name__
+            set_of_steps.add(step_name)
+        if set_of_steps != set(transform_args.keys()):
+            # Raise a warning and print all the keys that do not match
+            warnings.warn(
+                f"The following steps do not exist but were given in the kwargs: {set(transform_args.keys()) - set_of_steps}"
+            )
+
         # Loop through each step and call the transform method
         for step in self.steps:
             step_name = step.__class__.__name__
 
             step_args = transform_args.get(step_name, {})
             if isinstance(step, (TransformType)):
                 data = step.transform(data, **step_args)
@@ -122,14 +135,15 @@
 
 
 class ParallelTransformingSystem(TransformType, _ParallelSystem):
     """A system that transforms the input data in parallel.
 
     Parameters:
     - steps (list[Transformer | TransformingSystem | ParallelTransformingSystem]): The steps in the system.
+    - weights (list[float]): Weights of steps in system, if not specified they are all equal.
 
     Methods:
     .. code-block:: python
         @abstractmethod
         def concat(self, original_data: Any), data_to_concat: Any, weight: float = 1.0) -> Any:
             # Specifies how to concat data after parallel computations
 
@@ -175,24 +189,23 @@
     def transform(self, data: Any, **transform_args: Any) -> Any:
         """Transform the input data.
 
         :param data: The input data.
         :return: The transformed data.
         """
         # Loop through each step and call the transform method
-        num_steps = len(self.get_steps())
         out_data = None
         if len(self.get_steps()) == 0:
             return data
 
         for i, step in enumerate(self.get_steps()):
             step_name = step.__class__.__name__
 
             step_args = transform_args.get(step_name, {})
 
             if isinstance(step, (TransformType)):
                 step_data = step.transform(copy.deepcopy(data), **step_args)
-                out_data = self.concat(out_data, step_data, 1 / num_steps)
+                out_data = self.concat(out_data, step_data, self.get_weights()[i])
             else:
                 raise TypeError(f"{step} is not an instance of TransformType")
 
         return out_data
```

### Comparing `agogos-0.3.4/agogos.egg-info/PKG-INFO` & `agogos-0.4/agogos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agogos
-Version: 0.3.4
+Version: 0.4
 Summary: Package that creates the underlying construction of a machine learning pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -29,15 +29,15 @@
 </p>
 
 ## Pytest coverage report
 
 To generate pytest coverage report run
 
 ```shell
-pytest --cov=agogos --cov-report=html:coverage_re
+python -m pytest --cov=agogos --cov-report=html:coverage_re
 ```
 
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
```

### Comparing `agogos-0.3.4/tests/test__core.py` & `agogos-0.4/tests/test__core.py`

 * *Files identical despite different names*

### Comparing `agogos-0.3.4/tests/test_training.py` & `agogos-0.4/tests/test_training.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+import warnings
 from agogos.training import Trainer, TrainingSystem, ParallelTrainingSystem, Pipeline
 from agogos.transforming import Transformer, TransformingSystem
 import numpy as np
 
 
 class TestTrainer:
     def test_trainer_abstract_train(self):
@@ -122,14 +123,64 @@
         with pytest.raises(TypeError):
             training_system.train([1, 2, 3], [1, 2, 3])
 
     def test_training_system_empty_hash(self):
         training_system = TrainingSystem()
         assert training_system.get_hash() == ""
 
+    def test_training_system_wrong_kwargs(self):
+        class Block1(Trainer):
+            def train(self, x, y, **kwargs):
+                return x, y
+
+            def predict(self, x, **pred_args):
+                return x
+
+        class Block2(Trainer):
+            def train(self, x, y, **kwargs):
+                return x, y
+
+            def predict(self, x, **pred_args):
+                return x
+
+        block1 = Block1()
+        block2 = Block2()
+        system = TrainingSystem(steps=[block1, block2])
+        kwargs = {"Block1": {}, "block2": {}}
+        with pytest.warns(
+            UserWarning,
+            match="The following steps do not exist but were given in the kwargs:",
+        ):
+            system.train([1, 2, 3], [1, 2, 3], **kwargs)
+            system.predict([1, 2, 3], **kwargs)
+
+    def test_training_system_right_kwargs(self):
+        class Block1(Trainer):
+            def train(self, x, y, **kwargs):
+                return x, y
+
+            def predict(self, x, **pred_args):
+                return x
+
+        class Block2(Trainer):
+            def train(self, x, y, **kwargs):
+                return x, y
+
+            def predict(self, x, **pred_args):
+                return x
+
+        block1 = Block1()
+        block2 = Block2()
+        system = TrainingSystem(steps=[block1, block2])
+        kwargs = {"Block1": {}, "Block2": {}}
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            system.train([1, 2, 3], [1, 2, 3], **kwargs)
+            system.predict([1, 2, 3], **kwargs)
+        assert not caught_warnings
+
 
 class TestParallelTrainingSystem:
     def test_PTrainSys_init(self):
         system = ParallelTrainingSystem()
 
         assert system is not None
 
@@ -335,14 +386,35 @@
 
         with pytest.raises(TypeError):
             system.train([1, 2, 3], [1, 2, 3])
 
         with pytest.raises(TypeError):
             system.predict([1, 2, 3])
 
+    def test_train_parallel_hashes(self):
+        class SubTrainer1(Trainer):
+            def train(self, x, y):
+                return x, y
+
+        class SubTrainer2(Trainer):
+            def train(self, x, y):
+                return x * 2, y
+
+        block1 = SubTrainer1()
+        block2 = SubTrainer2()
+
+        system1 = ParallelTrainingSystem(steps=[block1, block2])
+        system1_copy = ParallelTrainingSystem(steps=[block1, block2])
+        system2 = ParallelTrainingSystem(steps=[block2, block1])
+        system2_copy = ParallelTrainingSystem(steps=[block2, block1])
+
+        assert system1.get_hash() == system2.get_hash()
+        assert system1.get_hash() == system1_copy.get_hash()
+        assert system2.get_hash() == system2_copy.get_hash()
+
 
 class TestPipeline:
     def test_pipeline_init(self):
         pipeline = Pipeline()
         assert pipeline is not None
 
     def test_pipeline_init_with_systems(self):
```

### Comparing `agogos-0.3.4/tests/test_transforming.py` & `agogos-0.4/tests/test_transforming.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+import warnings
+import numpy as np
 import pytest
+
 from agogos.training import Trainer
 from agogos.transforming import (
     Transformer,
     TransformingSystem,
     ParallelTransformingSystem,
 )
-import numpy as np
 
 
 class TestTransformer:
     def test_transformer_abstract(self):
         transformer = Transformer()
 
         with pytest.raises(NotImplementedError):
@@ -159,14 +161,51 @@
             np.array([6, 12, 18]),
         )
 
     def test_transforming_system_empty_hash(self):
         transforming_system = TransformingSystem()
         assert transforming_system.get_hash() == ""
 
+    def test_transforming_system_wrong_kwargs(self):
+        class Block1(Transformer):
+            def transform(self, x, **kwargs):
+                return x
+
+        class Block2(Transformer):
+            def transform(self, x, **kwargs):
+                return x
+
+        block1 = Block1()
+        block2 = Block2()
+        system = TransformingSystem(steps=[block1, block2])
+        kwargs = {"Block1": {}, "block2": {}}
+        with pytest.warns(
+            UserWarning,
+            match="The following steps do not exist but were given in the kwargs:",
+        ):
+            system.transform([1, 2, 3], **kwargs)
+
+    def test_transforming_system_right_kwargs(self):
+        class Block1(Transformer):
+            def transform(self, x, **kwargs):
+                return x
+
+        class Block2(Transformer):
+            def transform(self, x, **kwargs):
+                return x
+
+        block1 = Block1()
+        block2 = Block2()
+        system = TransformingSystem(steps=[block1, block2])
+        kwargs = {"Block1": {}, "Block2": {}}
+        with warnings.catch_warnings(record=True) as caught_warnings:
+            system.transform([1, 2, 3], **kwargs)
+
+        assert not caught_warnings
+
 
 class TestParallelTransformingSystem:
     def test_parallel_transforming_system(self):
         # Create an instance of the system
         system = ParallelTransformingSystem()
 
         # Assert the system is an instance of ParallelTransformingSystem
@@ -255,7 +294,28 @@
 
         t1 = transformer()
         t2 = Trainer()
         system.steps = [t1, t2]
 
         with pytest.raises(TypeError):
             system.transform([1, 2, 3])
+
+    def test_transform_parallel_hashes(self):
+        class SubTransformer1(Transformer):
+            def transform(self, x):
+                return x
+
+        class SubTransformer2(Transformer):
+            def transform(self, x):
+                return x * 2
+
+        block1 = SubTransformer1()
+        block2 = SubTransformer2()
+
+        system1 = ParallelTransformingSystem(steps=[block1, block2])
+        system1_copy = ParallelTransformingSystem(steps=[block1, block2])
+        system2 = ParallelTransformingSystem(steps=[block2, block1])
+        system2_copy = ParallelTransformingSystem(steps=[block2, block1])
+
+        assert system1.get_hash() == system2.get_hash()
+        assert system1.get_hash() == system1_copy.get_hash()
+        assert system2.get_hash() == system2_copy.get_hash()
```

