# Comparing `tmp/moval-0.2.8.tar.gz` & `tmp/moval-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-lduc2xvv/moval-0.2.8.tar", last modified: Sat Apr  6 18:29:00 2024, max compression
+gzip compressed data, was "/Users/zejuli/Local/Imperial/MOVAL/dist/.tmp-kn7ei667/moval-0.2.9.tar", last modified: Tue Apr  9 00:31:42 2024, max compression
```

## Comparing `moval-0.2.8.tar` & `moval-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.778117 moval-0.2.8/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-06 18:29:00.778039 moval-0.2.8/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.2.8/README.md
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.774701 moval-0.2.8/moval/
--rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-06 18:28:11.000000 moval-0.2.8/moval/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.775617 moval-0.2.8/moval/integrations/
--rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.2.8/moval/integrations/__init__.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.775937 moval-0.2.8/moval/integrations/sklearn/
--rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.2.8/moval/integrations/sklearn/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    41022 2024-03-21 04:23:11.000000 moval-0.2.8/moval/integrations/sklearn/moval.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.776890 moval-0.2.8/moval/models/
--rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.2.8/moval/models/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.2.8/moval/models/confidences.py
--rw-r--r--   0 zejuli     (501) staff       (20)    45579 2024-03-21 04:07:43.000000 moval-0.2.8/moval/models/model.py
--rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.2.8/moval/models/solver_temperature.py
--rw-r--r--   0 zejuli     (501) staff       (20)    10516 2024-01-15 18:30:37.000000 moval-0.2.8/moval/models/utils.py
--rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.2.8/moval/registry.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.777598 moval-0.2.8/moval/solvers/
--rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.2.8/moval/solvers/__init__.py
--rw-r--r--   0 zejuli     (501) staff       (20)    12169 2024-04-06 18:27:52.000000 moval-0.2.8/moval/solvers/criterions.py
--rw-r--r--   0 zejuli     (501) staff       (20)    19442 2024-04-06 18:27:14.000000 moval-0.2.8/moval/solvers/solver.py
--rw-r--r--   0 zejuli     (501) staff       (20)     2807 2024-03-21 04:25:50.000000 moval-0.2.8/moval/solvers/utils.py
-drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-06 18:29:00.777795 moval-0.2.8/moval.egg-info/
--rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-06 18:29:00.000000 moval-0.2.8/moval.egg-info/PKG-INFO
--rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-06 18:29:00.000000 moval-0.2.8/moval.egg-info/SOURCES.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-06 18:29:00.000000 moval-0.2.8/moval.egg-info/dependency_links.txt
--rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-06 18:29:00.000000 moval-0.2.8/moval.egg-info/requires.txt
--rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-06 18:29:00.000000 moval-0.2.8/moval.egg-info/top_level.txt
--rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.2.8/pyproject.toml
--rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-06 18:29:00.778461 moval-0.2.8/setup.cfg
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.052916 moval-0.2.9/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-09 00:31:42.052843 moval-0.2.9/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)     2259 2024-01-19 15:02:41.000000 moval-0.2.9/README.md
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.049669 moval-0.2.9/moval/
+-rw-r--r--   0 zejuli     (501) staff       (20)      706 2024-04-09 00:31:10.000000 moval-0.2.9/moval/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.050562 moval-0.2.9/moval/integrations/
+-rw-r--r--   0 zejuli     (501) staff       (20)       68 2023-07-28 01:11:44.000000 moval-0.2.9/moval/integrations/__init__.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.050848 moval-0.2.9/moval/integrations/sklearn/
+-rw-r--r--   0 zejuli     (501) staff       (20)      462 2023-10-26 14:28:12.000000 moval-0.2.9/moval/integrations/sklearn/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    41022 2024-04-08 20:19:47.000000 moval-0.2.9/moval/integrations/sklearn/moval.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.051709 moval-0.2.9/moval/models/
+-rw-r--r--   0 zejuli     (501) staff       (20)      447 2023-11-09 00:55:21.000000 moval-0.2.9/moval/models/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     6840 2023-11-26 14:30:38.000000 moval-0.2.9/moval/models/confidences.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    45831 2024-04-08 23:54:06.000000 moval-0.2.9/moval/models/model.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     1631 2024-01-08 19:28:25.000000 moval-0.2.9/moval/models/solver_temperature.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10804 2024-04-08 22:32:31.000000 moval-0.2.9/moval/models/utils.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    15406 2023-11-08 14:02:19.000000 moval-0.2.9/moval/registry.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.052431 moval-0.2.9/moval/solvers/
+-rw-r--r--   0 zejuli     (501) staff       (20)      429 2023-11-09 00:58:57.000000 moval-0.2.9/moval/solvers/__init__.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    10268 2024-04-09 00:26:42.000000 moval-0.2.9/moval/solvers/criterions.py
+-rw-r--r--   0 zejuli     (501) staff       (20)    19424 2024-04-08 23:38:44.000000 moval-0.2.9/moval/solvers/solver.py
+-rw-r--r--   0 zejuli     (501) staff       (20)     3054 2024-04-08 23:54:48.000000 moval-0.2.9/moval/solvers/utils.py
+drwxr-xr-x   0 zejuli     (501) staff       (20)        0 2024-04-09 00:31:42.052615 moval-0.2.9/moval.egg-info/
+-rw-r--r--   0 zejuli     (501) staff       (20)     3097 2024-04-09 00:31:42.000000 moval-0.2.9/moval.egg-info/PKG-INFO
+-rw-r--r--   0 zejuli     (501) staff       (20)      553 2024-04-09 00:31:42.000000 moval-0.2.9/moval.egg-info/SOURCES.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        1 2024-04-09 00:31:42.000000 moval-0.2.9/moval.egg-info/dependency_links.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)       61 2024-04-09 00:31:42.000000 moval-0.2.9/moval.egg-info/requires.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)        6 2024-04-09 00:31:42.000000 moval-0.2.9/moval.egg-info/top_level.txt
+-rw-r--r--   0 zejuli     (501) staff       (20)    15479 2023-12-08 04:03:18.000000 moval-0.2.9/pyproject.toml
+-rw-r--r--   0 zejuli     (501) staff       (20)      896 2024-04-09 00:31:42.053249 moval-0.2.9/setup.cfg
```

### Comparing `moval-0.2.8/PKG-INFO` & `moval-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.2.8
+Version: 0.2.9
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.2.8 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.2.9 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.2.8/README.md` & `moval-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/moval/__init__.py` & `moval-0.2.9/moval/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 try:
     from moval.integrations.sklearn.moval import MOVAL
 except ImportError as e:
     # silently fail for now
     pass
 
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 __all__ = ["MOVAL"]
 
 def __getattr__(key):
     """Lazy import of moval submodules and -packages.
 
     Once :py:mod:`moval` is imported, it is possible to lazy import
```

### Comparing `moval-0.2.8/moval/integrations/sklearn/moval.py` & `moval-0.2.9/moval/integrations/sklearn/moval.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/moval/models/confidences.py` & `moval-0.2.9/moval/models/confidences.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/moval/models/model.py` & `moval-0.2.9/moval/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,44 +371,48 @@
             for kcls in range(len(estim_dsc)):
                 m_estim_dsc.append(estim_dsc_list[:, kcls][estim_dsc_list[:,kcls] >= 0].mean())
             
             return np.array(m_estim_dsc)
         else:
             raise ValueError(f"Unknown mode '{self.mode}'")
     
-    def estimate_auc(self, probability: Union[List[Iterable], np.ndarray], gt_guide: np.ndarray = None) -> Tuple[float, np.ndarray]:
+    def estimate_auc(self, 
+                     probability: Union[List[Iterable], np.ndarray], 
+                     gt_guide: np.ndarray = None, 
+                     sel_cls: int = None) -> Tuple[float, np.ndarray]:
         """Esimate the AUC using network output.
 
         Args:
             probability: The calibrated probability of shape ``(n, d)`` or a list of n ``(d, H, W, (D))``.
             gt_guide: The cooresponding annotation guide of shape ``(n, d)`` for segmentation. This is only rquired for segmentation task during optimizaing.
                 We will utilize this to determine if there is label in the case. If not, we do not calculate the dsc and utilize for optimizing.
                 This is because we do not want to optimize parameter with blank segmentation map. 
                 This should be bool, if ``False``, it means that there isn't any manuel label of class d in this sample.
+            sel_cls: The selected class for calculation. If it is None, return all classes.
         
         Returns:
-            estim_AUC: Estimated class-wise AUC of shape ``(d, )``.
+            estim_AUC: Estimated class-wise AUC of shape ``(d, )``, or ``(1, )`` if sel_cls is givien.
 
         """
 
         if self.estim_algorithm == "atc-model" or self.estim_algorithm == "ts-atc-model":
             raise ValueError(f"estimation algorithm '{self.estim_algorithm}' does not support the estimation of AUC (because FP is always 0)")
 
         # Estimate the sensitivity.
         if self.mode == "classification":
             # probability is of shape ``(n, d)``
-            estim_AUC, _, _ = SoftAUC(probability)
+            estim_AUC, _, _ = SoftAUC(probability, sel_cls = sel_cls)
             return estim_AUC
         elif self.mode == "segmentation":
             # probability is a list of n ``(d, H, W, (D))``.
             estim_AUC_list = []
             for n_case in range(len(probability)):
                 score_filled = probability[n_case] # ``(d, H, W, (D))``
                 #
-                estim_AUC, _, _ = SoftAUC(score_filled[np.newaxis, ...])
+                estim_AUC, _, _ = SoftAUC(score_filled[np.newaxis, ...], sel_cls = sel_cls)
                 #
                 if isinstance(gt_guide, np.ndarray):
                     gt_case = gt_guide[n_case]
                     # We remove the class DSC if there isn't any in gt
                     for kcls in range(len(estim_AUC)):
                         if gt_case[kcls] is False:
                             estim_AUC[kcls] = -1
```

### Comparing `moval-0.2.8/moval/models/solver_temperature.py` & `moval-0.2.9/moval/models/solver_temperature.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/moval/models/utils.py` & `moval-0.2.9/moval/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,29 +210,30 @@
 
     axes = [0] + list(range(2, len(shp_x)))
     tp, fp, fn = get_tp_fp_fn(x, y, axes, square)
     precision = (tp + smooth) / (tp + fp + smooth)
 
     return precision
 
-def SoftAUC(x: np.ndarray) -> np.ndarray:
+def SoftAUC(x: np.ndarray, sel_cls: int = None) -> np.ndarray:
     """Calculate the estimated AUC given the probability.
     
     Note:
         When dealing with multi-class AUC, we calculate the One-vs-Rest strategy for simplicity.
         More information could refer to https://scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html.
         Similar strategy is adopted in https://nannyml.readthedocs.io/en/stable/how_it_works/performance_estimation.html.
     
     Args:
         x: The predicted probability of shape ``(n, d, (H), (W), (D))``.
+        sel_cls: Selected class to calculate AUC.
 
     Returns:
-        AUCs: Estimated class-wise AUC of shape ``(d, )``.
-        TPRall: A list of d true positive rates for different classes.
-        FPRall: A list of d false positive rates for different classes.
+        AUCs: Estimated class-wise AUC of shape ``(d, )``, or ``(1, )`` if sel_cls is givien.
+        TPRall: A list of d true positive rates for different classes, or a list of 1 if sel_cls is givien.
+        FPRall: A list of d false positive rates for different classes, or a list of 1 if sel_cls is givien.
 
     """
     
     # thresholds = [0.00001, 0.0001, 0.001, 0.01, 0.05, 
     #               0.1, 0.2, 0.3, 0.4, 0.5, 
     #               0.6, 0.7, 0.8, 0.9, 0.95, 
     #               0.99, 0.999, 0.9999, 0.99999]
@@ -242,15 +243,21 @@
     square = False
     axes = [0] + list(range(2, len(shp_x)))
     #
     AUCs = []
     TPRall = []
     FPRall = []
     smooth = 1e-6
-    for test_cls in range(x.shape[1]):
+    #
+    if sel_cls is None:
+        allcls = range(x.shape[1])
+    else:
+        allcls = range(sel_cls, sel_cls+1)
+
+    for test_cls in allcls:
         # low thres -> high FPR -> high sensitivity (TPR)
         # obtain TPRs and FPRs
 
         # customize thresholds
         # generate thresholds that fit the probability, just in case tpr == 0
         prob_max = np.min((np.max(x[:, test_cls]) - 0.05, 1.))
         prob_min = np.max((np.min(x[:, test_cls]) + 0.05, 0.))
```

### Comparing `moval-0.2.8/moval/registry.py` & `moval-0.2.9/moval/registry.py`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/moval/solvers/solver.py` & `moval-0.2.9/moval/solvers/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,20 +74,19 @@
                 probability = self.model.calculate_probability(self.inp, midstage = True, appr=True, full=True)
                 estim_perf = self.model.estimate_precision(probability, gt_guide = self.gt_guide)
             elif self.metric == "f1score":
                 probability = self.model.calculate_probability(self.inp, midstage = True, appr=True)
                 estim_perf = self.model.estimate_f1score(self.inp, probability, gt_guide = self.gt_guide)
             elif self.metric == "auc":
                 probability = self.model.calculate_probability(self.inp, midstage = True, appr=True, full=True)
-                estim_perf = self.model.estimate_auc(probability, gt_guide = self.gt_guide)
+                estim_perf = self.model.estimate_auc(probability, gt_guide = self.gt_guide, sel_cls = self.kcls)
             else:
                 ValueError(f"Unsupported metric '{self.metric}'")
 
-            err_cls = self.criterions(self.inp, self.gt, estim_perf)
-            err = err_cls[self.kcls]
+            err = self.criterions(self.inp, self.gt, estim_perf, self.kcls)
 
         return err
 
     def eval_func_ext(self, x: float) -> float:
         """The evaluation function for scipy optimization of extended parameters.
         
         Args:
@@ -113,20 +112,19 @@
                 probability = self.model.calculate_probability(self.inp, appr=True, full=True)
                 estim_perf = self.model.estimate_precision(probability, gt_guide = self.gt_guide)
             elif self.metric == "f1score":
                 probability = self.model.calculate_probability(self.inp, appr=True)
                 estim_perf = self.model.estimate_f1score(self.inp, probability, gt_guide = self.gt_guide)
             elif self.metric == "auc":
                 probability = self.model.calculate_probability(self.inp, appr=True, full=True)
-                estim_perf = self.model.estimate_auc(probability, gt_guide = self.gt_guide)
+                estim_perf = self.model.estimate_auc(probability, gt_guide = self.gt_guide, sel_cls = self.kcls)
             else:
                 ValueError(f"Unsupported metric '{self.metric}'")
 
-            err_cls = self.criterions(self.inp, self.gt, estim_perf)
-            err = err_cls[self.kcls]
+            err = self.criterions(self.inp, self.gt, estim_perf, self.kcls)
 
         return err
 
     def kcls_order_list(self, inp: np.ndarray, exclusive_background: bool = False) -> List[Iterable]:
         """Generate a list of kcls, such that the predicted samples are in ascending order.
 
         Args:
@@ -260,15 +258,15 @@
 
                 if len(gt_pos_cls) > 0 and len(pred_pos_cls) > 0:
 
                     optimization_result = scipy.optimize.minimize(
                                     fun = self.eval_func,
                                     x0 = x0,
                                     method = optimization_method,
-                                    bounds = [(1e-06,None)],
+                                    bounds = [(1e-03,None)],
                                     tol = 1e-07)
                     
                     optimized_param = optimization_result.x[0]
 
                     if optimization_result.fun > search_threshold:
                         # change the initial state, if we are not satisfied with the optimization results.
                         print(f"Not satisfied with initial optimization results of param for class {kcls}, trying more initial states...")
@@ -276,29 +274,29 @@
                         results.append((optimization_result.fun, optimization_result.x[0]))
                         cnt_guess = 0
                         for initial_guess in initial_conditions:
                             optimization_result = scipy.optimize.minimize(
                                     fun = self.eval_func,
                                     x0 = initial_guess,
                                     method = optimization_method,
-                                    bounds = [(1e-06,None)],
+                                    bounds = [(1e-03,None)],
                                     tol = 1e-07)
                             results.append((optimization_result.fun, optimization_result.x[0]))
                             cnt_guess += 1
                             print(f"Tried {cnt_guess}/{len(initial_conditions)} times.")
                         
                         optimized_param = min(results, key=lambda x: x[0])[1]
 
                     self.model.param[kcls] = optimized_param
         else:
             optimization_result = scipy.optimize.minimize(
                             fun = self.eval_func,
                             x0 = x0,
                             method = optimization_method,
-                            bounds = [(1e-06,None)],
+                            bounds = [(1e-03,None)],
                             tol = 1e-07)
         
             optimized_param = optimization_result.x
 
             if optimization_result.fun > search_threshold:
                 # change the initial state, if we are not satisfied with the optimization results.
                 print(f"Not satisfied with initial optimization results of param, trying more initial states...")
@@ -306,15 +304,15 @@
                 results.append((optimization_result.fun, optimization_result.x))
                 cnt_guess = 0
                 for initial_guess in initial_conditions:
                     optimization_result = scipy.optimize.minimize(
                             fun = self.eval_func,
                             x0 = initial_guess,
                             method = optimization_method,
-                            bounds = [(1e-06,None)],
+                            bounds = [(1e-03,None)],
                             tol = 1e-07)
                     results.append((optimization_result.fun, optimization_result.x))
                     cnt_guess += 1
                     print(f"Tried {cnt_guess}/{len(initial_conditions)} times.")
                 
                 optimized_param = min(results, key=lambda x: x[0])[1]
```

### Comparing `moval-0.2.8/moval/solvers/utils.py` & `moval-0.2.9/moval/solvers/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -31,41 +31,48 @@
     else:
         dice = 2 * tp / (2 * tp + fp + fn)
         precision = tp / (tp + fp)
         sensitivity = tp / (tp + fn)
     return dice, sensitivity, precision
 
 # AUC calculation here.
-def ComputAUC(ACTUAL: np.ndarray, PROBABILITY: np.ndarray) -> float:
+def ComputAUC(ACTUAL: np.ndarray, PROBABILITY: np.ndarray, sel_cls: int = None) -> float:
     """Calculate the AUC.
 
     Note:
         When dealing with multi-class AUC, we calculate the One-vs-Rest strategy for simplicity.
         More information could refer to https://scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html.
         It is not used in the framework of MOVAL, but could be useful to validate moval's performance.
 
     Args:
-        PROBABILITY: The predicted probability of shape ``(d, H, W, (D))`` or predicted classification results of shape ``(n, d)``.
         ACTUAL: The ground truth segmentation map of shape ``(H, W, (D))`` or predicted classification results of shape ``(n, )``.
+        PROBABILITY: The predicted probability of shape ``(d, H, W, (D))`` or predicted classification results of shape ``(n, d)``.
+        sel_cls: The selected class for calculation. If it is None, return all classes.
     
     Returns:
-        AUCs: The calculate class-wise AUC of shape ``(d, )``.
+        AUCs: The calculate class-wise AUC of shape ``(d, )``, or ``(1, )`` if sel_cls is givien.
     
     """
 
     ACTUAL = ACTUAL.flatten() # ``(n, )``
     if len(PROBABILITY.shape) > 2:
         # from ``(d, H, W, (D))`` to ``(n, d)``
         d, *rest_of_dimensions = PROBABILITY.shape
         flatten_dim = np.prod(rest_of_dimensions)
         PROBABILITY = PROBABILITY.reshape((d, flatten_dim))
         PROBABILITY = PROBABILITY.T
 
     y_onehot_test = one_hot_embedding(ACTUAL, PROBABILITY.shape[1])
     fpr, tpr, roc_auc = dict(), dict(), dict()
-    for i in range(PROBABILITY.shape[1]):
+
+    if sel_cls is None:
+        allcls = range(PROBABILITY.shape[1])
+    else:
+        allcls = range(sel_cls, sel_cls+1)
+
+    for i in allcls:
         
         fpr[i], tpr[i], _ = roc_curve(y_onehot_test[:, i], PROBABILITY[:, i])
         roc_auc[i] = auc(fpr[i], tpr[i])
 
     return np.array(list(roc_auc.values()))
```

### Comparing `moval-0.2.8/moval.egg-info/PKG-INFO` & `moval-0.2.9/moval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moval
-Version: 0.2.8
+Version: 0.2.9
 Summary: Model evaluation without manual labels
 Home-page: https://github.com/ZerojumpLine/MOVAL
 Author: Zeju Li
 Author-email: lizeju8@gmail.com
 Project-URL: Bug Tracker, https://github.com/ZerojumpLine/MOVAL/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moval Version: 0.2.8 Summary: Model evaluation
+Metadata-Version: 2.1 Name: moval Version: 0.2.9 Summary: Model evaluation
 without manual labels Home-page: https://github.com/ZerojumpLine/MOVAL Author:
 Zeju Li Author-email: lizeju8@gmail.com Project-URL: Bug Tracker, https://
 github.com/ZerojumpLine/MOVAL/issues Classifier: Development Status :: 3 -
 Alpha Classifier: Environment :: GPU :: NVIDIA CUDA Classifier: Intended
 Audience :: Science/Research Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: License :: Free
```

### Comparing `moval-0.2.8/moval.egg-info/SOURCES.txt` & `moval-0.2.9/moval.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/pyproject.toml` & `moval-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `moval-0.2.8/setup.cfg` & `moval-0.2.9/setup.cfg`

 * *Files identical despite different names*

