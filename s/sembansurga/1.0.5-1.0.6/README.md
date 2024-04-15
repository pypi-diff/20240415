# Comparing `tmp/sembansurga-1.0.5.tar.gz` & `tmp/sembansurga-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.0.5.tar", last modified: Sat Apr 13 20:35:43 2024, max compression
+gzip compressed data, was "sembansurga-1.0.6.tar", last modified: Mon Apr 15 06:17:48 2024, max compression
```

## Comparing `sembansurga-1.0.5.tar` & `sembansurga-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:35:43.544648 sembansurga-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-13 20:35:43.544648 sembansurga-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:35:43.534648 sembansurga-1.0.5/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      137 2024-04-13 20:34:57.000000 sembansurga-1.0.5/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2993 2024-04-13 20:34:38.000000 sembansurga-1.0.5/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 20:35:43.544648 sembansurga-1.0.5/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-13 20:35:43.000000 sembansurga-1.0.5/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 20:35:43.544648 sembansurga-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      730 2024-04-13 20:35:11.000000 sembansurga-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:17:48.429335 sembansurga-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:17:48.429335 sembansurga-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:17:48.419335 sembansurga-1.0.6/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:16:33.000000 sembansurga-1.0.6/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3518 2024-04-15 06:16:54.000000 sembansurga-1.0.6/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:17:48.429335 sembansurga-1.0.6/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:17:48.429335 sembansurga-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:17:39.000000 sembansurga-1.0.6/setup.py
```

### Comparing `sembansurga-1.0.5/sembansurga/sembansurga.py` & `sembansurga-1.0.6/sembansurga/sembansurga.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from google.colab import drive
 import libtorrent as lt
 import time
 import sys
 import warnings
+from usellm import Message, Options, UseLLM
+
 
 def authenticate_google():
     drive.mount('/content/drive')
     print("Google Drive has been connected!")
 
 def download_from_magnet(link, save_path=None):
     if not save_path:
@@ -85,13 +87,30 @@
     Question: {question}
     Answer:
     ""
     response = gemma_lm.generate(prompt.format(question=question), max_length=500)
     start_idx = response.find("Answer:") + len("Answer:")
     return response[start_idx:].strip()
 
-def ask(question):
+def np(question):
     response = generate_response(question)
     print(response)
     """
 
     print(code)
+
+def np(message):
+    # Initialize the service
+    service = UseLLM(service_url="https://usellm.org/api/llm")
+
+    # Prepare the conversation
+    messages = [
+        Message(role="system", content="You are a helpful assistant."),
+        Message(role="user", content=message),
+    ]
+    options = Options(messages=messages)
+
+    # Interact with the service
+    response = service.chat(options)
+
+    # Return the assistant's response
+    return response.content
```

### Comparing `sembansurga-1.0.5/setup.py` & `sembansurga-1.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.0.5',
+    version='1.0.6',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
         'libtorrent',
+        'usellm',
+
+    
 
     ],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
```

