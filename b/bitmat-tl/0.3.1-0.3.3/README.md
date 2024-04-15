# Comparing `tmp/bitmat-tl-0.3.1.tar.gz` & `tmp/bitmat_tl-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat-tl-0.3.1.tar", last modified: Thu Apr 11 18:48:01 2024, max compression
+gzip compressed data, was "bitmat_tl-0.3.3.tar", last modified: Mon Apr 15 10:48:26 2024, max compression
```

## Comparing `bitmat-tl-0.3.1.tar` & `bitmat_tl-0.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.303643 bitmat-tl-0.3.1/
--rw-rw-r--   0 marco     (1000) marco     (1000)    11357 2024-04-01 22:08:01.000000 bitmat-tl-0.3.1/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     4347 2024-04-11 18:48:01.303643 bitmat-tl-0.3.1/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     3715 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.299643 bitmat-tl-0.3.1/bitmat/
--rw-rw-r--   0 marco     (1000) marco     (1000)      489 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     3594 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/bitlinear.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.299643 bitmat-tl-0.3.1/bitmat/triton_kernels/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/triton_kernels/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5641 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/triton_kernels/bitmat_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     5241 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7037 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/triton_kernels/utils.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.299643 bitmat-tl-0.3.1/bitmat/utils/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/utils/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2664 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/bitmat.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2978 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/convert_hf_model.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     7547 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/custom_autotune.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.299643 bitmat-tl-0.3.1/bitmat/utils/model_hijacks/
--rw-rw-r--   0 marco     (1000) marco     (1000)        0 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/model_hijacks/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    61141 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/model_hijacks/gemma_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73359 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/model_hijacks/llama_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64378 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/model_hijacks/mistral_1_58b.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.303643 bitmat-tl-0.3.1/bitmat/utils/modeling/
--rw-rw-r--   0 marco     (1000) marco     (1000)       76 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/bitmat/utils/modeling/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1740 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/bitmat/utils/modeling/automodel.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.303643 bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/
--rw-rw-r--   0 marco     (1000) marco     (1000)      139 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    61145 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73363 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64382 2024-04-04 14:43:19.000000 bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      497 2024-04-11 18:47:44.000000 bitmat-tl-0.3.1/bitmat/utils/pack_model_before_save.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     2106 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/utils/packing.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      384 2024-04-05 08:31:48.000000 bitmat-tl-0.3.1/bitmat/utils/rmsnorm.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-11 18:48:01.303643 bitmat-tl-0.3.1/bitmat_tl.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     4347 2024-04-11 18:48:01.000000 bitmat-tl-0.3.1/bitmat_tl.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     1012 2024-04-11 18:48:01.000000 bitmat-tl-0.3.1/bitmat_tl.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-11 18:48:01.000000 bitmat-tl-0.3.1/bitmat_tl.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       50 2024-04-11 18:48:01.000000 bitmat-tl-0.3.1/bitmat_tl.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        7 2024-04-11 18:48:01.000000 bitmat-tl-0.3.1/bitmat_tl.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-11 18:48:01.303643 bitmat-tl-0.3.1/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      796 2024-04-11 18:47:53.000000 bitmat-tl-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.053539 bitmat_tl-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-15 10:48:26.053539 bitmat_tl-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.045539 bitmat_tl-0.3.3/bitmat/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/bitlinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.049539 bitmat_tl-0.3.3/bitmat/triton_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/triton_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/triton_kernels/bitmat_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/triton_kernels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.049539 bitmat_tl-0.3.3/bitmat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/bitmat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/convert_hf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/custom_autotune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.049539 bitmat_tl-0.3.3/bitmat/utils/model_hijacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/model_hijacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61141 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/model_hijacks/gemma_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73359 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/model_hijacks/llama_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64378 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/model_hijacks/mistral_1_58b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.049539 bitmat_tl-0.3.3/bitmat/utils/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/modeling/automodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.053539 bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61145 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73363 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64382 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/pack_model_before_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 10:48:16.000000 bitmat_tl-0.3.3/bitmat/utils/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:48:26.053539 bitmat_tl-0.3.3/bitmat_tl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-15 10:48:26.000000 bitmat_tl-0.3.3/bitmat_tl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-15 10:48:26.000000 bitmat_tl-0.3.3/bitmat_tl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:48:26.000000 bitmat_tl-0.3.3/bitmat_tl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 10:48:26.000000 bitmat_tl-0.3.3/bitmat_tl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 10:48:26.000000 bitmat_tl-0.3.3/bitmat_tl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:48:26.053539 bitmat_tl-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-15 10:48:25.000000 bitmat_tl-0.3.3/setup.py
```

### Comparing `bitmat-tl-0.3.1/LICENSE` & `bitmat_tl-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/PKG-INFO` & `bitmat_tl-0.3.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.3.1
+Version: 0.3.3
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,22 @@
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
+## Currently supported models
+
+| Model  | Supported |
+| ------------- | ------------- |
+| Mistral  |  ✅ |
+| LLama  |  ✅ |
+| Gemma  |  ✅ |
+
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
@@ -73,14 +81,26 @@
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
 ```
 
+## 📊 Results
+
+It can be observed that the performance of the custom matmul to 
+handle the multiplication of ternary matrices is better for higher precision. 
+This may be due to the optimized process within the GPU.
+
+
+**(left) 16-bit precision, (right) 32-bit precision**
+
+<img src="img/fp16.png" width="300" alt="Local Image"> <img src="img/fp32.png" width="300" alt="Local Image">
+
+
 ## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
 ## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
 
 ## Citation
```

### Comparing `bitmat-tl-0.3.1/README.md` & `bitmat_tl-0.3.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
+## Currently supported models
+
+| Model  | Supported |
+| ------------- | ------------- |
+| Mistral  |  ✅ |
+| LLama  |  ✅ |
+| Gemma  |  ✅ |
+
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
@@ -53,14 +61,26 @@
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
 ```
 
+## 📊 Results
+
+It can be observed that the performance of the custom matmul to 
+handle the multiplication of ternary matrices is better for higher precision. 
+This may be due to the optimized process within the GPU.
+
+
+**(left) 16-bit precision, (right) 32-bit precision**
+
+<img src="img/fp16.png" width="300" alt="Local Image"> <img src="img/fp32.png" width="300" alt="Local Image">
+
+
 ## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
 ## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
 
 ## Citation
```

### Comparing `bitmat-tl-0.3.1/bitmat/bitlinear.py` & `bitmat_tl-0.3.3/bitmat/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat_tl-0.3.3/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat_tl-0.3.3/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/triton_kernels/utils.py` & `bitmat_tl-0.3.3/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/bitmat.py` & `bitmat_tl-0.3.3/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/convert_hf_model.py` & `bitmat_tl-0.3.3/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/custom_autotune.py` & `bitmat_tl-0.3.3/bitmat/utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/model_hijacks/gemma_1_58b.py` & `bitmat_tl-0.3.3/bitmat/utils/model_hijacks/gemma_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/model_hijacks/llama_1_58b.py` & `bitmat_tl-0.3.3/bitmat/utils/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/model_hijacks/mistral_1_58b.py` & `bitmat_tl-0.3.3/bitmat/utils/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/modeling/automodel.py` & `bitmat_tl-0.3.3/bitmat/utils/modeling/automodel.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py` & `bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/llama_1_58b.py` & `bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/llama_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py` & `bitmat_tl-0.3.3/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat/utils/packing.py` & `bitmat_tl-0.3.3/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/bitmat_tl.egg-info/PKG-INFO` & `bitmat_tl-0.3.3/bitmat_tl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.3.1
+Version: 0.3.3
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,22 @@
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: numpy
 Requires-Dist: tqdm
 
 # BitMat: Improving Ternary Matrix Multiplication with Triton
 
+## Currently supported models
+
+| Model  | Supported |
+| ------------- | ------------- |
+| Mistral  |  ✅ |
+| LLama  |  ✅ |
+| Gemma  |  ✅ |
+
 
 ## 0️⃣1️⃣ Introduction
 BitMat is a Python package designed to optimize matrix multiplication operations by utilizing custom kernels written in Triton. Our package leverages the principles outlined in the "1bit-LLM Era" paper, specifically utilizing packed int8 data to enhance computational efficiency and performance in deep learning and numerical computing tasks.
 
 ## 🎛 Features
 Custom Triton Kernels: Utilize highly optimized kernels for matrix multiplication, tailored for performance and efficiency.
 
@@ -73,14 +81,26 @@
 import torch
 from bitmat import BitLinear
 
 layer = BitLinear(in_features=1024, out_features=512, bias=True, eps=1e-5)
 # You can use the layer as a normal torch.nn.Linear layer
 ```
 
+## 📊 Results
+
+It can be observed that the performance of the custom matmul to 
+handle the multiplication of ternary matrices is better for higher precision. 
+This may be due to the optimized process within the GPU.
+
+
+**(left) 16-bit precision, (right) 32-bit precision**
+
+<img src="img/fp16.png" width="300" alt="Local Image"> <img src="img/fp32.png" width="300" alt="Local Image">
+
+
 ## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
 ## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
 
 ## Citation
```

### Comparing `bitmat-tl-0.3.1/bitmat_tl.egg-info/SOURCES.txt` & `bitmat_tl-0.3.3/bitmat_tl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitmat-tl-0.3.1/setup.py` & `bitmat_tl-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.3.1',
+    version='0.3.3',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

