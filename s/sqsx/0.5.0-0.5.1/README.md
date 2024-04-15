# Comparing `tmp/sqsx-0.5.tar.gz` & `tmp/sqsx-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqsx-0.5.tar", last modified: Fri Apr 12 21:28:25 2024, max compression
+gzip compressed data, was "sqsx-0.5.1.tar", last modified: Mon Apr 15 10:19:06 2024, max compression
```

## Comparing `sqsx-0.5.tar` & `sqsx-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.903609 sqsx-0.5/
--rw-r--r--   0 allisson   (501) staff       (20)     1073 2024-02-23 10:48:45.000000 sqsx-0.5/LICENSE
--rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-04-12 21:28:25.903378 sqsx-0.5/PKG-INFO
--rw-r--r--   0 allisson   (501) staff       (20)     6844 2024-02-23 10:48:45.000000 sqsx-0.5/README.md
--rw-r--r--   0 allisson   (501) staff       (20)      598 2024-04-12 21:27:51.000000 sqsx-0.5/pyproject.toml
--rw-r--r--   0 allisson   (501) staff       (20)       38 2024-04-12 21:28:25.903653 sqsx-0.5/setup.cfg
--rw-r--r--   0 allisson   (501) staff       (20)     1091 2024-04-12 21:27:51.000000 sqsx-0.5/setup.py
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.901067 sqsx-0.5/sqsx/
--rw-r--r--   0 allisson   (501) staff       (20)       47 2024-02-23 10:48:45.000000 sqsx-0.5/sqsx/__init__.py
--rw-r--r--   0 allisson   (501) staff       (20)      443 2024-02-23 10:48:45.000000 sqsx-0.5/sqsx/exceptions.py
--rw-r--r--   0 allisson   (501) staff       (20)      406 2024-02-23 10:48:45.000000 sqsx-0.5/sqsx/helper.py
--rw-r--r--   0 allisson   (501) staff       (20)     7481 2024-04-12 21:27:51.000000 sqsx-0.5/sqsx/queue.py
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.903078 sqsx-0.5/sqsx.egg-info/
--rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/PKG-INFO
--rw-r--r--   0 allisson   (501) staff       (20)      322 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/SOURCES.txt
--rw-r--r--   0 allisson   (501) staff       (20)        1 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/dependency_links.txt
--rw-r--r--   0 allisson   (501) staff       (20)       31 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/requires.txt
--rw-r--r--   0 allisson   (501) staff       (20)       11 2024-04-12 21:28:25.000000 sqsx-0.5/sqsx.egg-info/top_level.txt
-drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-12 21:28:25.902331 sqsx-0.5/tests/
--rw-r--r--   0 allisson   (501) staff       (20)        0 2024-02-23 10:48:45.000000 sqsx-0.5/tests/__init__.py
--rw-r--r--   0 allisson   (501) staff       (20)     1941 2024-02-23 10:48:45.000000 sqsx-0.5/tests/conftest.py
--rw-r--r--   0 allisson   (501) staff       (20)      954 2024-02-23 10:48:45.000000 sqsx-0.5/tests/test_helper.py
--rw-r--r--   0 allisson   (501) staff       (20)     9485 2024-04-12 21:27:51.000000 sqsx-0.5/tests/test_queue.py
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-15 10:19:06.133512 sqsx-0.5.1/
+-rw-r--r--   0 allisson   (501) staff       (20)     1073 2024-02-23 10:48:45.000000 sqsx-0.5.1/LICENSE
+-rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-04-15 10:19:06.133257 sqsx-0.5.1/PKG-INFO
+-rw-r--r--   0 allisson   (501) staff       (20)     6844 2024-02-23 10:48:45.000000 sqsx-0.5.1/README.md
+-rw-r--r--   0 allisson   (501) staff       (20)      598 2024-04-15 10:17:53.000000 sqsx-0.5.1/pyproject.toml
+-rw-r--r--   0 allisson   (501) staff       (20)       38 2024-04-15 10:19:06.133559 sqsx-0.5.1/setup.cfg
+-rw-r--r--   0 allisson   (501) staff       (20)     1091 2024-04-15 10:17:53.000000 sqsx-0.5.1/setup.py
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-15 10:19:06.131355 sqsx-0.5.1/sqsx/
+-rw-r--r--   0 allisson   (501) staff       (20)       47 2024-02-23 10:48:45.000000 sqsx-0.5.1/sqsx/__init__.py
+-rw-r--r--   0 allisson   (501) staff       (20)      443 2024-02-23 10:48:45.000000 sqsx-0.5.1/sqsx/exceptions.py
+-rw-r--r--   0 allisson   (501) staff       (20)      406 2024-02-23 10:48:45.000000 sqsx-0.5.1/sqsx/helper.py
+-rw-r--r--   0 allisson   (501) staff       (20)     7555 2024-04-15 10:14:12.000000 sqsx-0.5.1/sqsx/queue.py
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-15 10:19:06.132985 sqsx-0.5.1/sqsx.egg-info/
+-rw-r--r--   0 allisson   (501) staff       (20)     7578 2024-04-15 10:19:06.000000 sqsx-0.5.1/sqsx.egg-info/PKG-INFO
+-rw-r--r--   0 allisson   (501) staff       (20)      322 2024-04-15 10:19:06.000000 sqsx-0.5.1/sqsx.egg-info/SOURCES.txt
+-rw-r--r--   0 allisson   (501) staff       (20)        1 2024-04-15 10:19:06.000000 sqsx-0.5.1/sqsx.egg-info/dependency_links.txt
+-rw-r--r--   0 allisson   (501) staff       (20)       31 2024-04-15 10:19:06.000000 sqsx-0.5.1/sqsx.egg-info/requires.txt
+-rw-r--r--   0 allisson   (501) staff       (20)       11 2024-04-15 10:19:06.000000 sqsx-0.5.1/sqsx.egg-info/top_level.txt
+drwxr-xr-x   0 allisson   (501) staff       (20)        0 2024-04-15 10:19:06.132542 sqsx-0.5.1/tests/
+-rw-r--r--   0 allisson   (501) staff       (20)        0 2024-02-23 10:48:45.000000 sqsx-0.5.1/tests/__init__.py
+-rw-r--r--   0 allisson   (501) staff       (20)     1941 2024-02-23 10:48:45.000000 sqsx-0.5.1/tests/conftest.py
+-rw-r--r--   0 allisson   (501) staff       (20)      954 2024-02-23 10:48:45.000000 sqsx-0.5.1/tests/test_helper.py
+-rw-r--r--   0 allisson   (501) staff       (20)     9485 2024-04-12 21:27:51.000000 sqsx-0.5.1/tests/test_queue.py
```

### Comparing `sqsx-0.5/LICENSE` & `sqsx-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqsx-0.5/PKG-INFO` & `sqsx-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqsx
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple task processor for Amazon SQS
 Home-page: https://github.com/allisson/pysqsx
 Author: Allisson Azevedo
 Author-email: allisson@gmail.com
 Keywords: aws,sqs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sqsx-0.5/README.md` & `sqsx-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sqsx-0.5/pyproject.toml` & `sqsx-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqsx"
-version = "0.5.0"
+version = "0.5.1"
 description = "A simple task processor for Amazon SQS"
 authors = ["Allisson Azevedo"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.33.13"
```

### Comparing `sqsx-0.5/setup.py` & `sqsx-0.5.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="sqsx",
-    version="0.5.0",
+    version="0.5.1",
     description="A simple task processor for Amazon SQS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/allisson/pysqsx",
     author="Allisson Azevedo",
     author_email="allisson@gmail.com",
     classifiers=[
```

### Comparing `sqsx-0.5/sqsx/queue.py` & `sqsx-0.5.1/sqsx/queue.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
                 MessageAttributeNames=["All"],
                 WaitTimeSeconds=polling_wait_seconds,
             )
 
             sqs_messages = response.get("Messages", [])
             if not sqs_messages:
                 logger.debug(
-                    f"Waiting some seconds because no message was received, seconds={wait_seconds}, queue_url={self.url}"
+                    f"Waiting some seconds because no message was received, wait_seconds={wait_seconds}, "
+                    f"polling_wait_seconds={polling_wait_seconds}, queue_url={self.url}"
                 )
                 time.sleep(wait_seconds)
                 continue
 
             with ThreadPoolExecutor(max_workers=max_threads) as executor:
                 futures = []
                 for sqs_message in sqs_messages:
```

### Comparing `sqsx-0.5/sqsx.egg-info/PKG-INFO` & `sqsx-0.5.1/sqsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqsx
-Version: 0.5.0
+Version: 0.5.1
 Summary: A simple task processor for Amazon SQS
 Home-page: https://github.com/allisson/pysqsx
 Author: Allisson Azevedo
 Author-email: allisson@gmail.com
 Keywords: aws,sqs
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `sqsx-0.5/tests/conftest.py` & `sqsx-0.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sqsx-0.5/tests/test_helper.py` & `sqsx-0.5.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `sqsx-0.5/tests/test_queue.py` & `sqsx-0.5.1/tests/test_queue.py`

 * *Files identical despite different names*

