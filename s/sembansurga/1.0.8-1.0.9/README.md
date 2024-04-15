# Comparing `tmp/sembansurga-1.0.8.tar.gz` & `tmp/sembansurga-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.0.8.tar", last modified: Mon Apr 15 06:26:14 2024, max compression
+gzip compressed data, was "sembansurga-1.0.9.tar", last modified: Mon Apr 15 06:29:29 2024, max compression
```

## Comparing `sembansurga-1.0.8.tar` & `sembansurga-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:26:14.759248 sembansurga-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:26:14.759248 sembansurga-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:26:14.759248 sembansurga-1.0.8/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:22:32.000000 sembansurga-1.0.8/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3523 2024-04-15 06:25:52.000000 sembansurga-1.0.8/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:26:14.759248 sembansurga-1.0.8/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:26:14.759248 sembansurga-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:26:01.000000 sembansurga-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:29:29.299222 sembansurga-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:29:29.299222 sembansurga-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:29:29.299222 sembansurga-1.0.9/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:29:20.000000 sembansurga-1.0.9/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2024-04-15 06:29:02.000000 sembansurga-1.0.9/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:29:29.299222 sembansurga-1.0.9/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:29:29.000000 sembansurga-1.0.9/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:29:29.000000 sembansurga-1.0.9/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:29:29.000000 sembansurga-1.0.9/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:29:29.000000 sembansurga-1.0.9/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:29:29.000000 sembansurga-1.0.9/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:29:29.299222 sembansurga-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:29:14.000000 sembansurga-1.0.9/setup.py
```

### Comparing `sembansurga-1.0.8/sembansurga/sembansurga.py` & `sembansurga-1.0.9/sembansurga/sembansurga.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,42 +76,39 @@
 gemma_lm = keras_nlp.models.GemmaCausalLM.from_preset("gemma_instruct_2b_en")
 
 import keras
 import keras_nlp
 import numpy as np
 
 def generate_response(question):
-    prompt = ""
-    You are an AI assistant designed to answer simple questions.
-    Please restrict your answer to the exact question asked.
-    Think step by step, use careful reasoning. Your name is Semban Surga
-    Question: {question}
-    Answer:
-    ""
+    prompt = '''
+You are an AI assistant designed to answer simple questions.
+Please restrict your answer to the exact question asked.
+Think step by step, use careful reasoning. Your name is Semban Surga
+Question: {question}
+Answer:
+'''
     response = gemma_lm.generate(prompt.format(question=question), max_length=500)
     start_idx = response.find("Answer:") + len("Answer:")
     return response[start_idx:].strip()
 """
 
-def np(question):
-    response = generate_response(question)
-    print(response)
-    """
-
     print(code)
 
+
 def np(message):
+
     # Initialize the service
     service = UseLLM(service_url="https://usellm.org/api/llm")
 
     # Prepare the conversation
     messages = [
         Message(role="system", content="You are a helpful assistant."),
         Message(role="user", content=message),
     ]
     options = Options(messages=messages)
 
     # Interact with the service
     response = service.chat(options)
 
-    # Return the assistant's response
-    return response.content
+    # Print the assistant's response
+    print(response.content)
```

### Comparing `sembansurga-1.0.8/setup.py` & `sembansurga-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.0.8',
+    version='1.0.9',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

