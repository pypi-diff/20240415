# Comparing `tmp/maitai-sdk-python-0.422.tar.gz` & `tmp/maitai-sdk-python-0.423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maitai-sdk-python-0.422.tar", last modified: Sat Apr 13 20:55:36 2024, max compression
+gzip compressed data, was "maitai-sdk-python-0.423.tar", last modified: Mon Apr 15 21:15:08 2024, max compression
```

## Comparing `maitai-sdk-python-0.422.tar` & `maitai-sdk-python-0.423.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 20:55:36.837799 maitai-sdk-python-0.422/
--rw-rw-rw-   0        0        0      380 2024-04-13 20:55:36.835799 maitai-sdk-python-0.422/PKG-INFO
--rw-rw-rw-   0        0        0     5183 2024-04-09 05:15:20.000000 maitai-sdk-python-0.422/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 20:55:36.820799 maitai-sdk-python-0.422/maitai/
--rw-rw-rw-   0        0        0      327 2024-04-13 18:48:05.000000 maitai-sdk-python-0.422/maitai/__init__.py
--rw-rw-rw-   0        0        0      413 2024-04-13 18:48:23.000000 maitai-sdk-python-0.422/maitai/_config.py
--rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.422/maitai/_eval_request.py
--rw-rw-rw-   0        0        0     9656 2024-04-13 20:55:17.000000 maitai-sdk-python-0.422/maitai/_evaluator.py
--rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.422/maitai/_loadable.py
--rw-rw-rw-   0        0        0      206 2024-04-13 18:48:42.000000 maitai-sdk-python-0.422/maitai/_maitai_object.py
-drwxrwxrwx   0        0        0        0 2024-04-13 20:55:36.834799 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      349 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-13 20:55:36.000000 maitai-sdk-python-0.422/maitai_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 20:55:36.837799 maitai-sdk-python-0.422/setup.cfg
--rw-rw-rw-   0        0        0      573 2024-04-13 20:02:42.000000 maitai-sdk-python-0.422/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:15:08.862220 maitai-sdk-python-0.423/
+-rw-rw-rw-   0        0        0      380 2024-04-15 21:15:08.861220 maitai-sdk-python-0.423/PKG-INFO
+-rw-rw-rw-   0        0        0     5332 2024-04-15 21:14:54.000000 maitai-sdk-python-0.423/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 21:15:08.832266 maitai-sdk-python-0.423/maitai/
+-rw-rw-rw-   0        0        0      327 2024-04-13 18:48:05.000000 maitai-sdk-python-0.423/maitai/__init__.py
+-rw-rw-rw-   0        0        0      413 2024-04-13 18:48:23.000000 maitai-sdk-python-0.423/maitai/_config.py
+-rw-rw-rw-   0        0        0      594 2024-04-09 05:13:35.000000 maitai-sdk-python-0.423/maitai/_eval_request.py
+-rw-rw-rw-   0        0        0     9658 2024-04-15 21:11:56.000000 maitai-sdk-python-0.423/maitai/_evaluator.py
+-rw-rw-rw-   0        0        0     1171 2022-12-02 23:23:26.000000 maitai-sdk-python-0.423/maitai/_loadable.py
+-rw-rw-rw-   0        0        0      206 2024-04-13 18:48:42.000000 maitai-sdk-python-0.423/maitai/_maitai_object.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:15:08.859219 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 21:15:08.000000 maitai-sdk-python-0.423/maitai_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 21:15:08.862220 maitai-sdk-python-0.423/setup.cfg
+-rw-rw-rw-   0        0        0      573 2024-04-15 21:11:56.000000 maitai-sdk-python-0.423/setup.py
```

### Comparing `maitai-sdk-python-0.422/README.md` & `maitai-sdk-python-0.423/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -113,7 +113,21 @@
 ```
 
 This will send the evaluation request to the MaiTai service asynchronously. Ensure that your `application_id` and `api_key` are correctly set as shown in the Configuration section above.
 
 ## Conclusion
 
 You're now ready to start using the MaiTai Python SDK to evaluate AI outputs in your application. Remember to follow best practices for managing your `api_key` and `application_id` securely within your application. If you encounter any issues or have further questions, refer to the [MaiTai Documentation](https://docs.maitai.ai) or reach out to the support team.
+
+
+## Contributions
+
+To build, run
+```bash
+python setup.py sdist bdist_wheel
+```
+
+
+To upload to pypi, run
+```bash
+twine upload dist/*
+```
```

### Comparing `maitai-sdk-python-0.422/maitai/_eval_request.py` & `maitai-sdk-python-0.423/maitai/_eval_request.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.422/maitai/_evaluator.py` & `maitai-sdk-python-0.423/maitai/_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from maitai._eval_request import EvalRequestEncoder
 from maitai._config import config
 from maitai import MaiTaiObject, EvalRequest
 
 
 class Evaluator(MaiTaiObject):
 
-    MAITAI_HOST = 'https://api.dev.yewpay.com'
+    MAITAI_HOST = 'https://maitai.ai.yewpay.com'
 
     def __init__(self):
         super().__init__()
 
     @classmethod
     def evaluate(cls, application_id, session_id, reference_id, action_type, content):
         eval_request: EvalRequest = cls.create_eval_request(application_id, session_id, reference_id, action_type, content)
```

### Comparing `maitai-sdk-python-0.422/maitai/_loadable.py` & `maitai-sdk-python-0.423/maitai/_loadable.py`

 * *Files identical despite different names*

### Comparing `maitai-sdk-python-0.422/setup.py` & `maitai-sdk-python-0.423/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setup.py
 
 from setuptools import setup, find_packages
 
 setup(
     name='maitai-sdk-python',
-    version='0.422',
+    version='0.423',
     packages=find_packages(),
     install_requires=[
         'requests',
         'aiohttp'
     ],
     # Optional metadata
     author='Christian DalSanto',
```

