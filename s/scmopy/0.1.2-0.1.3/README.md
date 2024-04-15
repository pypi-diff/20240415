# Comparing `tmp/scmopy-0.1.2.tar.gz` & `tmp/scmopy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmopy-0.1.2.tar", last modified: Sun Apr 14 19:36:04 2024, max compression
+gzip compressed data, was "scmopy-0.1.3.tar", last modified: Mon Apr 15 20:36:49 2024, max compression
```

## Comparing `scmopy-0.1.2.tar` & `scmopy-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:36:04.414207 scmopy-0.1.2/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.1.2/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.1.2/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)    21227 2024-04-14 19:36:04.414207 scmopy-0.1.2/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)    20911 2024-04-14 19:26:23.000000 scmopy-0.1.2/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:36:04.414207 scmopy-0.1.2/examples/
--rw-r--r--   0 soli      (1000) soli      (1000)        0 2024-04-14 19:31:15.000000 scmopy-0.1.2/examples/placeholder.ipynb
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:36:04.414207 scmopy-0.1.2/scmopy/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.1.2/scmopy/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-14 19:35:13.000000 scmopy-0.1.2/scmopy/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.1.2/scmopy/base.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:36:04.414207 scmopy-0.1.2/scmopy/components/
--rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.1.2/scmopy/components/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.1.2/scmopy/components/syniv.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.1.2/scmopy/gaussian_scm.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5227 2024-04-14 17:43:16.000000 scmopy-0.1.2/scmopy/model_selection.py
--rw-r--r--   0 soli      (1000) soli      (1000)    14355 2024-04-14 17:43:56.000000 scmopy-0.1.2/scmopy/nongaussian_scm.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:36:04.414207 scmopy-0.1.2/scmopy.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)    21227 2024-04-14 19:36:04.000000 scmopy-0.1.2/scmopy.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      395 2024-04-14 19:36:04.000000 scmopy-0.1.2/scmopy.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 19:36:04.000000 scmopy-0.1.2/scmopy.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 19:36:04.000000 scmopy-0.1.2/scmopy.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-14 19:36:04.000000 scmopy-0.1.2/scmopy.egg-info/top_level.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 19:36:04.414207 scmopy-0.1.2/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-14 19:35:19.000000 scmopy-0.1.2/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.1.3/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.1.3/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)    21327 2024-04-15 20:36:49.119946 scmopy-0.1.3/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)    21011 2024-04-15 20:13:13.000000 scmopy-0.1.3/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/examples/
+-rw-r--r--   0 soli      (1000) soli      (1000)   133028 2024-04-15 20:26:10.000000 scmopy-0.1.3/examples/ESA-2SCM_Example.ipynb
+-rw-r--r--   0 soli      (1000) soli      (1000)        0 2024-04-14 19:31:15.000000 scmopy-0.1.3/examples/gngscm_placeholder.ipynb
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/scmopy/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.1.3/scmopy/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-15 20:36:07.000000 scmopy-0.1.3/scmopy/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.1.3/scmopy/base.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/scmopy/components/
+-rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.1.3/scmopy/components/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.1.3/scmopy/components/syniv.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.1.3/scmopy/gaussian_scm.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5087 2024-04-15 20:14:24.000000 scmopy-0.1.3/scmopy/model_selection.py
+-rw-r--r--   0 soli      (1000) soli      (1000)    14208 2024-04-15 20:16:14.000000 scmopy-0.1.3/scmopy/nongaussian_scm.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/scmopy.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)    21327 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      490 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-15 20:36:49.000000 scmopy-0.1.3/scmopy.egg-info/top_level.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-15 20:36:49.119946 scmopy-0.1.3/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-15 20:36:08.000000 scmopy-0.1.3/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-15 20:36:49.119946 scmopy-0.1.3/test/
+-rw-r--r--   0 soli      (1000) soli      (1000)     2112 2024-04-15 20:26:41.000000 scmopy-0.1.3/test/test_ESA-2SCM_model.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2630 2024-04-15 20:27:06.000000 scmopy-0.1.3/test/test_ESA-2SCM_syniv.py
```

### Comparing `scmopy-0.1.2/LICENSE` & `scmopy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.2/PKG-INFO` & `scmopy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.1.2
+Version: 0.1.3
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,29 +13,29 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/scmopy.svg)](https://pypi.org/project/scmopy/)
 
 
 scmopy is a composite package for causal discovery/analysis using several **novel** types of Structural Causal Models Optimization algorithms.
 <br>
 
-scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, distributional assumptions in typical SCM/SEM such as satisfying the normality conditions are *not* required.
+scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, users can deviate from the necessity of satisfying any specific distributional assumptions as regards to the dataset, and as regards to the whole process of causal estimation to hypothesis-testing.
 <br>
 
 The package is mainly structured in three parts:
 
 1. **ESA-2SCM (Elastic Segment Allocation-based Two-Stage Least Squares SCM)**
 - ESA-2SCM is a new method for detecting causality based on the Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
-- For details and documentation, please refer to my Original Article: <br>
+- For details and documentation, please refer to my original article: <br>
 - [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
 <br><br>
 
 2. **Gradient Non-Gaussian SCM**
 - Gradient Non-Gaussian SCM incorporates the information of higher order moment structures assuming non-gaussianity to determine the true causal direction.
 - Gradient Non-Gaussian SCM is a customized implementation of S.Shimizu and Y.Kano's conceptualization of nnSEM. Specifically, the quadratic objective function based on the difference between the sample moments and theoretical moments is optimized via gradient method (defaulting to BFGS) instead of performing GLS.
-- For details regarding the original nnSEM, please refer to:
+- For details regarding the concepts of the original nnSEM, please refer to:
 - S.Shimizu and Y.Kano (2008). **Use of non-normality in structural equation modeling: Application to direction of causation**, *Journal of Statistical Planning and Inference,* *138*, *11*, 3483-3491.
 <br><br>
 
 3. **Auto-SCM Selector for Optimization**
 - The SCM Selector automatically determines the optimal model via pre-inspecting the dataset. 
 - Internally, it utilizes voting methods in combination with multiple hypothesis testing techniques on the data's original distribution for the precision of model determination: ESA-2SCM is selected as the basemodel if the pre-inspection result suggests gaussianity, otherwise the Gradient Non-Gaussian SCM is selected.
 
@@ -92,15 +92,14 @@
 # To confirm the estimated True Causal Coefficient
 print(scm.causal_coef)
 
 # To confirm the test statistic (T2) and p-value for hypothesis testing on the Causal Direction
 print(scm.test_statistic)
 print(scm.p_value)
 
-
 # To confirm the fit score
 print(scm.score)
 ```
 
 ```python
 # For result summary:
 scm.summary()
@@ -274,15 +273,15 @@
 
 and with $\tau$ estimation rewritten as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/12.png?raw=true" width="400"/>
 </p>
 
-Assuming unit variance $(I)$ and single parameter/moment ($\tau$, $\sigma(\tau)$) for simplification:
+Assuming unit variance $(I)$ and single parameter/moment ( $\tau$, $\sigma(\tau)$ ) for simplification:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/13.png?raw=true" width="400"/>
 </p>
 
 so that
 
@@ -351,27 +350,27 @@
 Now, expanding up to third and fourth order moment structures, S.Shimizu and Y.Kano (2008) prove that under the satisfaction of the following three conditions:<br>
 (1) Either the exogenous variable $x_2$ or the noise $e_1$ is non-gaussian (when assuming that the model $(1)$ holds True) <br>
 (2) $corr(x_1, x_2) \neq 0$ <br>
 (3) $-1 < corr(x_1, x_2) < 1$ <br>
 models $(1)$ and $(2)$ can be differentiated. 
 
 That is to say, <br>
-with $ r = corr(x_1,x_2) $, and $i$-th order moment structure defined as:
+with $r = corr(x_1,x_2)$, and $i$-th order moment structure defined as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/25.png?raw=true" width="190"/>
 </p>
 
 and,
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/26.png?raw=true" width="300"/>
 </p>
 
-to get the isolated quantity from the fourth order moment ($E(z^4)$), especially the parts that are independent from the lower order moments, leaving a quantity that captures the "pure" fourth-order behavior of the distribution,
+to get the isolated quantity from the fourth order moment ( $E(z^4)$ ), especially the parts that are independent from the lower order moments, leaving a quantity that captures the "pure" fourth-order behavior of the distribution,
 
 if (1) $0< |r| < 1$ and (2) either $E(x_2^3), E(e_1^3), cum_4(x_2)$, or $cum_4(e_1)$ is non-zero, the following holds:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/27.png?raw=true" width="350"/>
 </p>
 
@@ -407,15 +406,15 @@
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/33.png?raw=true" width="400"/>
 </p>
 
 Similar derivation process can be applied for the fourth-order moment.
 
-Thus, the two models $(1)$ and $(2)$ are distinguishable from each other using either third- and/or fourth-order moments, with each order moment structure (e.g., for model $(1)$) defined respectively as:
+Thus, the two models $(1)$ and $(2)$ are distinguishable from each other using either third- and/or fourth-order moments, with each order moment structure ( e.g., for model $(1)$ ) defined respectively as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/34.png?raw=true" width="500"/>
 </p>
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/35.png?raw=true" width="500"/>
@@ -539,12 +538,12 @@
 ## License
 scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 
 ## References
 
 ### scmopy Package
 
-Should you use the scmopy package to perform causal discovery, please kindly cite my original article and the original article by S.Shimizu and Y.Kano:
+Should you use the scmopy package to perform causal discovery, please cite my original article and the original article by S.Shimizu and Y.Kano:
 
 * Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 * S.Shimizu and Y.Kano (2008). **Use of non-normality in structural equation modeling: Application to direction of causation**, *Journal of Statistical Planning and Inference,* *138*, *11*, 3483-3491.
```

### Comparing `scmopy-0.1.2/README.md` & `scmopy-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/scmopy.svg)](https://pypi.org/project/scmopy/)
 
 
 scmopy is a composite package for causal discovery/analysis using several **novel** types of Structural Causal Models Optimization algorithms.
 <br>
 
-scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, distributional assumptions in typical SCM/SEM such as satisfying the normality conditions are *not* required.
+scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, users can deviate from the necessity of satisfying any specific distributional assumptions as regards to the dataset, and as regards to the whole process of causal estimation to hypothesis-testing.
 <br>
 
 The package is mainly structured in three parts:
 
 1. **ESA-2SCM (Elastic Segment Allocation-based Two-Stage Least Squares SCM)**
 - ESA-2SCM is a new method for detecting causality based on the Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
-- For details and documentation, please refer to my Original Article: <br>
+- For details and documentation, please refer to my original article: <br>
 - [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
 <br><br>
 
 2. **Gradient Non-Gaussian SCM**
 - Gradient Non-Gaussian SCM incorporates the information of higher order moment structures assuming non-gaussianity to determine the true causal direction.
 - Gradient Non-Gaussian SCM is a customized implementation of S.Shimizu and Y.Kano's conceptualization of nnSEM. Specifically, the quadratic objective function based on the difference between the sample moments and theoretical moments is optimized via gradient method (defaulting to BFGS) instead of performing GLS.
-- For details regarding the original nnSEM, please refer to:
+- For details regarding the concepts of the original nnSEM, please refer to:
 - S.Shimizu and Y.Kano (2008). **Use of non-normality in structural equation modeling: Application to direction of causation**, *Journal of Statistical Planning and Inference,* *138*, *11*, 3483-3491.
 <br><br>
 
 3. **Auto-SCM Selector for Optimization**
 - The SCM Selector automatically determines the optimal model via pre-inspecting the dataset. 
 - Internally, it utilizes voting methods in combination with multiple hypothesis testing techniques on the data's original distribution for the precision of model determination: ESA-2SCM is selected as the basemodel if the pre-inspection result suggests gaussianity, otherwise the Gradient Non-Gaussian SCM is selected.
 
@@ -82,15 +82,14 @@
 # To confirm the estimated True Causal Coefficient
 print(scm.causal_coef)
 
 # To confirm the test statistic (T2) and p-value for hypothesis testing on the Causal Direction
 print(scm.test_statistic)
 print(scm.p_value)
 
-
 # To confirm the fit score
 print(scm.score)
 ```
 
 ```python
 # For result summary:
 scm.summary()
@@ -264,15 +263,15 @@
 
 and with $\tau$ estimation rewritten as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/12.png?raw=true" width="400"/>
 </p>
 
-Assuming unit variance $(I)$ and single parameter/moment ($\tau$, $\sigma(\tau)$) for simplification:
+Assuming unit variance $(I)$ and single parameter/moment ( $\tau$, $\sigma(\tau)$ ) for simplification:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/13.png?raw=true" width="400"/>
 </p>
 
 so that
 
@@ -341,27 +340,27 @@
 Now, expanding up to third and fourth order moment structures, S.Shimizu and Y.Kano (2008) prove that under the satisfaction of the following three conditions:<br>
 (1) Either the exogenous variable $x_2$ or the noise $e_1$ is non-gaussian (when assuming that the model $(1)$ holds True) <br>
 (2) $corr(x_1, x_2) \neq 0$ <br>
 (3) $-1 < corr(x_1, x_2) < 1$ <br>
 models $(1)$ and $(2)$ can be differentiated. 
 
 That is to say, <br>
-with $ r = corr(x_1,x_2) $, and $i$-th order moment structure defined as:
+with $r = corr(x_1,x_2)$, and $i$-th order moment structure defined as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/25.png?raw=true" width="190"/>
 </p>
 
 and,
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/26.png?raw=true" width="300"/>
 </p>
 
-to get the isolated quantity from the fourth order moment ($E(z^4)$), especially the parts that are independent from the lower order moments, leaving a quantity that captures the "pure" fourth-order behavior of the distribution,
+to get the isolated quantity from the fourth order moment ( $E(z^4)$ ), especially the parts that are independent from the lower order moments, leaving a quantity that captures the "pure" fourth-order behavior of the distribution,
 
 if (1) $0< |r| < 1$ and (2) either $E(x_2^3), E(e_1^3), cum_4(x_2)$, or $cum_4(e_1)$ is non-zero, the following holds:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/27.png?raw=true" width="350"/>
 </p>
 
@@ -397,15 +396,15 @@
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/33.png?raw=true" width="400"/>
 </p>
 
 Similar derivation process can be applied for the fourth-order moment.
 
-Thus, the two models $(1)$ and $(2)$ are distinguishable from each other using either third- and/or fourth-order moments, with each order moment structure (e.g., for model $(1)$) defined respectively as:
+Thus, the two models $(1)$ and $(2)$ are distinguishable from each other using either third- and/or fourth-order moments, with each order moment structure ( e.g., for model $(1)$ ) defined respectively as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/34.png?raw=true" width="500"/>
 </p>
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/35.png?raw=true" width="500"/>
@@ -529,12 +528,12 @@
 ## License
 scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 
 ## References
 
 ### scmopy Package
 
-Should you use the scmopy package to perform causal discovery, please kindly cite my original article and the original article by S.Shimizu and Y.Kano:
+Should you use the scmopy package to perform causal discovery, please cite my original article and the original article by S.Shimizu and Y.Kano:
 
 * Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 * S.Shimizu and Y.Kano (2008). **Use of non-normality in structural equation modeling: Application to direction of causation**, *Journal of Statistical Planning and Inference,* *138*, *11*, 3483-3491.
```

### Comparing `scmopy-0.1.2/scmopy/LICENSE` & `scmopy-0.1.3/scmopy/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.2/scmopy/__init__.py` & `scmopy-0.1.3/scmopy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 Should you use the scmopy package, please cite the following articles.
 - Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>.
 - S.Shimizu and Y.Kano (2008). Use of non-normality in structural equation modeling: Application to direction of causation, Journal of Statistical Planning and Inference, 138, 11, 3483-3491.
 
 """
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
```

### Comparing `scmopy-0.1.2/scmopy/base.py` & `scmopy-0.1.3/scmopy/base.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.2/scmopy/components/__init__.py` & `scmopy-0.1.3/scmopy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.2/scmopy/components/syniv.py` & `scmopy-0.1.3/scmopy/components/syniv.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.2/scmopy/gaussian_scm.py` & `scmopy-0.1.3/scmopy/gaussian_scm.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.1.2/scmopy/model_selection.py` & `scmopy-0.1.3/scmopy/model_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,16 +118,14 @@
         else:
             self._test_result = 'non-gaussian' if all(np.sum(v) >= int(vote_thres[voting_strategy]) for v in vote_list) else 'gaussian'
         
         self._is_fitted = True
         
         self._selected_scm = Esa2Scm(self._x1, self._x2, self._prior_knowledge) if self._test_result == 'gaussian' else GradientNonGaussianScm(self._x1, self._x2, self._prior_knowledge)
         
-        # print(f"{self._selected_scm.__class__.__name__}(x1={self._x1}, x2={self._x2}, prior_knowledge={self._prior_knowledge})")
-        
         return self
     
 
     @property
     def selected_scm(self):
         if not self._is_fitted:
             raise RuntimeError("You must fit the ScmSelector first")
```

### Comparing `scmopy-0.1.2/scmopy/nongaussian_scm.py` & `scmopy-0.1.3/scmopy/nongaussian_scm.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,15 +302,14 @@
 
     
     def _summary(self):
         
         summary_idx = ['Causal Direction', "Causal Coefficient",  'Test Statistic', 'P-value', "Reject H0", "Goodness of Fit"]
         
         if self._prior_knowledge is not None:
-            #self._result = pd.DataFrame({summary_idx[0] + ' (FIXED)': [self._prior_knowledge], summary_idx[-1]: [self._b]}, index=['Estimation'])
             self._result = pd.DataFrame({self._prior_knowledge + " (Predetermined)": [self._prior_knowledge, self._b, self._score]}, index=[summary_idx[0], summary_idx[1], summary_idx[-1]])
             
         else:
             summary_columns = ['x2->x1', 'x1->x2']
             summary_values = [self._confidence + ' ' + str(self._causal_dir == 'x2->x1'), self._b12, self._T2, self._p_value, self._reject_H0]
             summary_values_rev = [self._confidence + ' ' + str(self._causal_dir == 'x1->x2'), self._b21, self._T2_rev, self._p_value_rev, 
                                     self._reject_H0_rev]
```

### Comparing `scmopy-0.1.2/scmopy.egg-info/PKG-INFO` & `scmopy-0.1.3/scmopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.1.2
+Version: 0.1.3
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,29 +13,29 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 [![PyPI - Version](https://img.shields.io/pypi/v/scmopy.svg)](https://pypi.org/project/scmopy/)
 
 
 scmopy is a composite package for causal discovery/analysis using several **novel** types of Structural Causal Models Optimization algorithms.
 <br>
 
-scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, distributional assumptions in typical SCM/SEM such as satisfying the normality conditions are *not* required.
+scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, users can deviate from the necessity of satisfying any specific distributional assumptions as regards to the dataset, and as regards to the whole process of causal estimation to hypothesis-testing.
 <br>
 
 The package is mainly structured in three parts:
 
 1. **ESA-2SCM (Elastic Segment Allocation-based Two-Stage Least Squares SCM)**
 - ESA-2SCM is a new method for detecting causality based on the Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
-- For details and documentation, please refer to my Original Article: <br>
+- For details and documentation, please refer to my original article: <br>
 - [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
 <br><br>
 
 2. **Gradient Non-Gaussian SCM**
 - Gradient Non-Gaussian SCM incorporates the information of higher order moment structures assuming non-gaussianity to determine the true causal direction.
 - Gradient Non-Gaussian SCM is a customized implementation of S.Shimizu and Y.Kano's conceptualization of nnSEM. Specifically, the quadratic objective function based on the difference between the sample moments and theoretical moments is optimized via gradient method (defaulting to BFGS) instead of performing GLS.
-- For details regarding the original nnSEM, please refer to:
+- For details regarding the concepts of the original nnSEM, please refer to:
 - S.Shimizu and Y.Kano (2008). **Use of non-normality in structural equation modeling: Application to direction of causation**, *Journal of Statistical Planning and Inference,* *138*, *11*, 3483-3491.
 <br><br>
 
 3. **Auto-SCM Selector for Optimization**
 - The SCM Selector automatically determines the optimal model via pre-inspecting the dataset. 
 - Internally, it utilizes voting methods in combination with multiple hypothesis testing techniques on the data's original distribution for the precision of model determination: ESA-2SCM is selected as the basemodel if the pre-inspection result suggests gaussianity, otherwise the Gradient Non-Gaussian SCM is selected.
 
@@ -92,15 +92,14 @@
 # To confirm the estimated True Causal Coefficient
 print(scm.causal_coef)
 
 # To confirm the test statistic (T2) and p-value for hypothesis testing on the Causal Direction
 print(scm.test_statistic)
 print(scm.p_value)
 
-
 # To confirm the fit score
 print(scm.score)
 ```
 
 ```python
 # For result summary:
 scm.summary()
@@ -274,15 +273,15 @@
 
 and with $\tau$ estimation rewritten as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/12.png?raw=true" width="400"/>
 </p>
 
-Assuming unit variance $(I)$ and single parameter/moment ($\tau$, $\sigma(\tau)$) for simplification:
+Assuming unit variance $(I)$ and single parameter/moment ( $\tau$, $\sigma(\tau)$ ) for simplification:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/13.png?raw=true" width="400"/>
 </p>
 
 so that
 
@@ -351,27 +350,27 @@
 Now, expanding up to third and fourth order moment structures, S.Shimizu and Y.Kano (2008) prove that under the satisfaction of the following three conditions:<br>
 (1) Either the exogenous variable $x_2$ or the noise $e_1$ is non-gaussian (when assuming that the model $(1)$ holds True) <br>
 (2) $corr(x_1, x_2) \neq 0$ <br>
 (3) $-1 < corr(x_1, x_2) < 1$ <br>
 models $(1)$ and $(2)$ can be differentiated. 
 
 That is to say, <br>
-with $ r = corr(x_1,x_2) $, and $i$-th order moment structure defined as:
+with $r = corr(x_1,x_2)$, and $i$-th order moment structure defined as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/25.png?raw=true" width="190"/>
 </p>
 
 and,
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/26.png?raw=true" width="300"/>
 </p>
 
-to get the isolated quantity from the fourth order moment ($E(z^4)$), especially the parts that are independent from the lower order moments, leaving a quantity that captures the "pure" fourth-order behavior of the distribution,
+to get the isolated quantity from the fourth order moment ( $E(z^4)$ ), especially the parts that are independent from the lower order moments, leaving a quantity that captures the "pure" fourth-order behavior of the distribution,
 
 if (1) $0< |r| < 1$ and (2) either $E(x_2^3), E(e_1^3), cum_4(x_2)$, or $cum_4(e_1)$ is non-zero, the following holds:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/27.png?raw=true" width="350"/>
 </p>
 
@@ -407,15 +406,15 @@
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/33.png?raw=true" width="400"/>
 </p>
 
 Similar derivation process can be applied for the fourth-order moment.
 
-Thus, the two models $(1)$ and $(2)$ are distinguishable from each other using either third- and/or fourth-order moments, with each order moment structure (e.g., for model $(1)$) defined respectively as:
+Thus, the two models $(1)$ and $(2)$ are distinguishable from each other using either third- and/or fourth-order moments, with each order moment structure ( e.g., for model $(1)$ ) defined respectively as:
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/34.png?raw=true" width="500"/>
 </p>
 
 <p align="center">
   <img src="https://github.com/DSsoli/scmopy/blob/main/img/35.png?raw=true" width="500"/>
@@ -539,12 +538,12 @@
 ## License
 scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 
 ## References
 
 ### scmopy Package
 
-Should you use the scmopy package to perform causal discovery, please kindly cite my original article and the original article by S.Shimizu and Y.Kano:
+Should you use the scmopy package to perform causal discovery, please cite my original article and the original article by S.Shimizu and Y.Kano:
 
 * Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 * S.Shimizu and Y.Kano (2008). **Use of non-normality in structural equation modeling: Application to direction of causation**, *Journal of Statistical Planning and Inference,* *138*, *11*, 3483-3491.
```

### Comparing `scmopy-0.1.2/setup.py` & `scmopy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     README = fh.read()
 
 setup(
     author="Sanghoon Lee (DSsoli)",
     author_email="solisoli3197@gmail.com",
     name="scmopy",
-    version="0.1.2",
+    version="0.1.3",
     description="scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "pandas", "scipy"],
     url="https://github.com/DSsoli/scmopy.git",
     packages=find_packages(include=['scmopy', 'scmopy.*']),
     package_data={"scmopy": ['LICENSE', 'examples/*']},
```

