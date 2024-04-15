# Comparing `tmp/gliner-finetune-0.0.1.tar.gz` & `tmp/gliner-finetune-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-finetune-0.0.1.tar", last modified: Sat Apr 13 08:52:32 2024, max compression
+gzip compressed data, was "gliner-finetune-0.0.2.tar", last modified: Mon Apr 15 06:19:41 2024, max compression
```

## Comparing `gliner-finetune-0.0.1.tar` & `gliner-finetune-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-13 08:52:32.746343 gliner-finetune-0.0.1/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3944 2024-04-13 08:52:32.746214 gliner-finetune-0.0.1/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     2958 2024-04-13 08:48:35.000000 gliner-finetune-0.0.1/README.md
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-13 08:52:32.745419 gliner-finetune-0.0.1/gliner_finetune/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       68 2024-04-13 08:33:15.000000 gliner-finetune-0.0.1/gliner_finetune/__init__.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1690 2024-04-13 08:33:15.000000 gliner-finetune-0.0.1/gliner_finetune/convert.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     4382 2024-04-13 08:39:02.000000 gliner-finetune-0.0.1/gliner_finetune/synthetic.py
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     5544 2024-04-13 08:33:15.000000 gliner-finetune-0.0.1/gliner_finetune/train.py
-drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-13 08:52:32.746048 gliner-finetune-0.0.1/gliner_finetune.egg-info/
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     3944 2024-04-13 08:52:32.000000 gliner-finetune-0.0.1/gliner_finetune.egg-info/PKG-INFO
--rw-r--r--   0 wjbmattingly   (501) staff       (20)      321 2024-04-13 08:52:32.000000 gliner-finetune-0.0.1/gliner_finetune.egg-info/SOURCES.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-13 08:52:32.000000 gliner-finetune-0.0.1/gliner_finetune.egg-info/dependency_links.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       64 2024-04-13 08:52:32.000000 gliner-finetune-0.0.1/gliner_finetune.egg-info/requires.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       16 2024-04-13 08:52:32.000000 gliner-finetune-0.0.1/gliner_finetune.egg-info/top_level.txt
--rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-13 08:52:32.746393 gliner-finetune-0.0.1/setup.cfg
--rw-r--r--   0 wjbmattingly   (501) staff       (20)     1388 2024-04-13 08:51:50.000000 gliner-finetune-0.0.1/setup.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-15 06:19:41.914198 gliner-finetune-0.0.2/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4020 2024-04-15 06:19:41.914085 gliner-finetune-0.0.2/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     3034 2024-04-13 08:53:13.000000 gliner-finetune-0.0.2/README.md
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-15 06:19:41.913104 gliner-finetune-0.0.2/gliner_finetune/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       68 2024-04-13 08:33:15.000000 gliner-finetune-0.0.2/gliner_finetune/__init__.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1690 2024-04-13 08:33:15.000000 gliner-finetune-0.0.2/gliner_finetune/convert.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4382 2024-04-13 08:39:02.000000 gliner-finetune-0.0.2/gliner_finetune/synthetic.py
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     5544 2024-04-13 08:33:15.000000 gliner-finetune-0.0.2/gliner_finetune/train.py
+drwxr-xr-x   0 wjbmattingly   (501) staff       (20)        0 2024-04-15 06:19:41.913923 gliner-finetune-0.0.2/gliner_finetune.egg-info/
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     4020 2024-04-15 06:19:41.000000 gliner-finetune-0.0.2/gliner_finetune.egg-info/PKG-INFO
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)      321 2024-04-15 06:19:41.000000 gliner-finetune-0.0.2/gliner_finetune.egg-info/SOURCES.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)        1 2024-04-15 06:19:41.000000 gliner-finetune-0.0.2/gliner_finetune.egg-info/dependency_links.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       69 2024-04-15 06:19:41.000000 gliner-finetune-0.0.2/gliner_finetune.egg-info/requires.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       16 2024-04-15 06:19:41.000000 gliner-finetune-0.0.2/gliner_finetune.egg-info/top_level.txt
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)       38 2024-04-15 06:19:41.914230 gliner-finetune-0.0.2/setup.cfg
+-rw-r--r--   0 wjbmattingly   (501) staff       (20)     1393 2024-04-15 06:19:40.000000 gliner-finetune-0.0.2/setup.py
```

### Comparing `gliner-finetune-0.0.1/PKG-INFO` & `gliner-finetune-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-finetune
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to create synthetic data with OpenAI and train a GLiNER model on that data.
 Home-page: https://github.com/wjbmattingly/gliner-finetune
 Author: William J.B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <=3.10
+Requires-Python: >=3.7, <=3.11
 Description-Content-Type: text/markdown
 
 # GLiNER-Finetune
 
 `gliner-finetune` is a Python library designed to generate synthetic data using OpenAI's GPT models, process this data, and then use it to train a GLiNER model. GLiNER is a framework for learning and inference in Named Entity Recognition (NER) tasks.
 
 ## Features
@@ -38,14 +38,16 @@
 pip install gliner-finetune
 ```
 
 ## Quick Start
 
 The following example demonstrates how to generate synthetic data, process it, and train a GLiNER model using the `gliner-finetune` library.
 
+Make sure you have a .env file with your OPENAI_API_KEY set as a variable.
+
 ### Step 1: Generate Synthetic Data
 
 ```python
 from gliner_finetune.synthetic import generate_data, create_prompt
 import json
 
 # Define your example data
```

### Comparing `gliner-finetune-0.0.1/README.md` & `gliner-finetune-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 pip install gliner-finetune
 ```
 
 ## Quick Start
 
 The following example demonstrates how to generate synthetic data, process it, and train a GLiNER model using the `gliner-finetune` library.
 
+Make sure you have a .env file with your OPENAI_API_KEY set as a variable.
+
 ### Step 1: Generate Synthetic Data
 
 ```python
 from gliner_finetune.synthetic import generate_data, create_prompt
 import json
 
 # Define your example data
```

### Comparing `gliner-finetune-0.0.1/gliner_finetune/convert.py` & `gliner-finetune-0.0.2/gliner_finetune/convert.py`

 * *Files identical despite different names*

### Comparing `gliner-finetune-0.0.1/gliner_finetune/synthetic.py` & `gliner-finetune-0.0.2/gliner_finetune/synthetic.py`

 * *Files identical despite different names*

### Comparing `gliner-finetune-0.0.1/gliner_finetune/train.py` & `gliner-finetune-0.0.2/gliner_finetune/train.py`

 * *Files identical despite different names*

### Comparing `gliner-finetune-0.0.1/gliner_finetune.egg-info/PKG-INFO` & `gliner-finetune-0.0.2/gliner_finetune.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner-finetune
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library to create synthetic data with OpenAI and train a GLiNER model on that data.
 Home-page: https://github.com/wjbmattingly/gliner-finetune
 Author: William J.B. Mattingly
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7, <=3.10
+Requires-Python: >=3.7, <=3.11
 Description-Content-Type: text/markdown
 
 # GLiNER-Finetune
 
 `gliner-finetune` is a Python library designed to generate synthetic data using OpenAI's GPT models, process this data, and then use it to train a GLiNER model. GLiNER is a framework for learning and inference in Named Entity Recognition (NER) tasks.
 
 ## Features
@@ -38,14 +38,16 @@
 pip install gliner-finetune
 ```
 
 ## Quick Start
 
 The following example demonstrates how to generate synthetic data, process it, and train a GLiNER model using the `gliner-finetune` library.
 
+Make sure you have a .env file with your OPENAI_API_KEY set as a variable.
+
 ### Step 1: Generate Synthetic Data
 
 ```python
 from gliner_finetune.synthetic import generate_data, create_prompt
 import json
 
 # Define your example data
```

### Comparing `gliner-finetune-0.0.1/setup.py` & `gliner-finetune-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gliner-finetune',
-    version='0.0.1',
+    version='0.0.2',
     author='William J.B. Mattingly',
     description='A library to create synthetic data with OpenAI and train a GLiNER model on that data.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/wjbmattingly/gliner-finetune',
     packages=find_packages(),
     install_requires=[
         'gliner',
         'openai',
         'spacy',
-        'sklearn',
+        'scikit-learn',
         'torch',
         'transformers',
         'tqdm',
         'json',
         'dotenv'
     ],
-    python_requires='>=3.7, <=3.10',
+    python_requires='>=3.7, <=3.11',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',  # Assuming MIT License, replace if different
         'Natural Language :: English',
         'Operating System :: OS Independent',
```

