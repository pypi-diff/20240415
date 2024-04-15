# Comparing `tmp/sembansurga-1.0.6.tar.gz` & `tmp/sembansurga-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sembansurga-1.0.6.tar", last modified: Mon Apr 15 06:17:48 2024, max compression
+gzip compressed data, was "sembansurga-1.0.7.tar", last modified: Mon Apr 15 06:22:43 2024, max compression
```

## Comparing `sembansurga-1.0.6.tar` & `sembansurga-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:17:48.429335 sembansurga-1.0.6/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:17:48.429335 sembansurga-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:17:48.419335 sembansurga-1.0.6/sembansurga/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:16:33.000000 sembansurga-1.0.6/sembansurga/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3518 2024-04-15 06:16:54.000000 sembansurga-1.0.6/sembansurga/sembansurga.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:17:48.429335 sembansurga-1.0.6/sembansurga.egg-info/
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:17:48.000000 sembansurga-1.0.6/sembansurga.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:17:48.429335 sembansurga-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:17:39.000000 sembansurga-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:22:42.989287 sembansurga-1.0.7/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:22:42.989287 sembansurga-1.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        6 2023-12-24 05:56:18.000000 sembansurga-1.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:22:42.989287 sembansurga-1.0.7/sembansurga/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-15 06:22:32.000000 sembansurga-1.0.7/sembansurga/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-15 06:22:13.000000 sembansurga-1.0.7/sembansurga/sembansurga.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 06:22:42.989287 sembansurga-1.0.7/sembansurga.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      243 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-15 06:22:42.000000 sembansurga-1.0.7/sembansurga.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 06:22:42.989287 sembansurga-1.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-15 06:22:29.000000 sembansurga-1.0.7/setup.py
```

### Comparing `sembansurga-1.0.6/sembansurga/sembansurga.py` & `sembansurga-1.0.7/sembansurga/sembansurga.py`

 * *Files 7% similar despite different names*

```diff
@@ -87,30 +87,26 @@
     Question: {question}
     Answer:
     ""
     response = gemma_lm.generate(prompt.format(question=question), max_length=500)
     start_idx = response.find("Answer:") + len("Answer:")
     return response[start_idx:].strip()
 
-def np(question):
-    response = generate_response(question)
-    print(response)
-    """
-
-    print(code)
-
 def np(message):
+    from usellm import Message, Options, UseLLM
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
+
```

### Comparing `sembansurga-1.0.6/setup.py` & `sembansurga-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sembansurga',
-    version='1.0.6',
+    version='1.0.7',
     author='sidharth',
     author_email='sidharthss2690@gmail.com',
     description='Simply superb',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

