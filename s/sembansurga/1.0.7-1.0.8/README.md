# Comparing `tmp/sembansurga-1.0.7.tar.gz` & `tmp/sembansurga-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.0.7.tar", last modified: Mon Apr 15 06:22:43 2024, max compression
+gzip compressed data, was "sembansurga-1.0.8.tar", last modified: Mon Apr 15 06:26:14 2024, max compression
```

## Comparing `sembansurga-1.0.7.tar` & `sembansurga-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:22:42.989287 sembansurga-1.0.7/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:22:42.989287 sembansurga-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:22:42.989287 sembansurga-1.0.7/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:22:32.000000 sembansurga-1.0.7/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-15 06:22:13.000000 sembansurga-1.0.7/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:22:42.989287 sembansurga-1.0.7/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:22:42.989287 sembansurga-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:22:29.000000 sembansurga-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:26:14.759248 sembansurga-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:26:14.759248 sembansurga-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:26:14.759248 sembansurga-1.0.8/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:22:32.000000 sembansurga-1.0.8/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3523 2024-04-15 06:25:52.000000 sembansurga-1.0.8/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:26:14.759248 sembansurga-1.0.8/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:26:14.000000 sembansurga-1.0.8/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:26:14.759248 sembansurga-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:26:01.000000 sembansurga-1.0.8/setup.py
```

### Comparing `sembansurga-1.0.7/sembansurga/sembansurga.py` & `sembansurga-1.0.8/sembansurga/sembansurga.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,27 +86,32 @@
     Think step by step, use careful reasoning. Your name is Semban Surga
     Question: {question}
     Answer:
     ""
     response = gemma_lm.generate(prompt.format(question=question), max_length=500)
     start_idx = response.find("Answer:") + len("Answer:")
     return response[start_idx:].strip()
+"""
 
-def np(message):
-    from usellm import Message, Options, UseLLM
+def np(question):
+    response = generate_response(question)
+    print(response)
+    """
+
+    print(code)
 
+def np(message):
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
 
-    # Print the assistant's response
-    print(response.content)
-
+    # Return the assistant's response
+    return response.content
```

### Comparing `sembansurga-1.0.7/setup.py` & `sembansurga-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.0.7',
+    version='1.0.8',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

