# Comparing `tmp/freeze-uuid-0.3.0.tar.gz` & `tmp/freeze_uuid-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freeze-uuid-0.3.0.tar", last modified: Sun Jan 21 05:23:50 2024, max compression
+gzip compressed data, was "freeze_uuid-0.3.1.tar", last modified: Mon Apr 15 15:59:05 2024, max compression
```

## Comparing `freeze-uuid-0.3.0.tar` & `freeze_uuid-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 05:23:50.009343 freeze-uuid-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-21 05:23:50.009343 freeze-uuid-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 05:23:50.005344 freeze-uuid-0.3.0/freeze_uuid/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/freeze_uuid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/freeze_uuid/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 05:23:50.009343 freeze-uuid-0.3.0/freeze_uuid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-21 05:23:50.000000 freeze-uuid-0.3.0/freeze_uuid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-21 05:23:50.000000 freeze-uuid-0.3.0/freeze_uuid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 05:23:50.000000 freeze-uuid-0.3.0/freeze_uuid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-21 05:23:50.000000 freeze-uuid-0.3.0/freeze_uuid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 05:23:50.009343 freeze-uuid-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 05:23:50.009343 freeze-uuid-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-21 05:23:40.000000 freeze-uuid-0.3.0/tests/testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/freeze_uuid/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/freeze_uuid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/freeze_uuid/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/freeze_uuid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 15:59:05.000000 freeze_uuid-0.3.1/freeze_uuid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:05.577396 freeze_uuid-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-15 15:59:01.000000 freeze_uuid-0.3.1/tests/testdata.py
```

### Comparing `freeze-uuid-0.3.0/LICENSE` & `freeze_uuid-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freeze-uuid-0.3.0/PKG-INFO` & `freeze_uuid-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freeze-uuid
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python package for mocking uuid.
 Author: Alexander Balashov
 Author-email: alaex777@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -45,7 +45,18 @@
 def test_uuid_list():
     assert str(uuid.uuid1()) == '12af6b44-8181-11ee-b890-628ab7cd4d99'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
 
 ```
+
+### Since library mocks uuid.UUID class, it can be used with all libraries, that support UUID class, i.e. uuid7
+
+```python
+from uuid_extensions import uuid7
+
+@freeze_uuid(TEST_UUID)
+def test_uuid_7():
+    assert str(uuid7()) == TEST_UUID
+
+```
```

### Comparing `freeze-uuid-0.3.0/README.md` & `freeze_uuid-0.3.1/freeze_uuid.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: freeze-uuid
+Version: 0.3.1
+Summary: Python package for mocking uuid.
+Author: Alexander Balashov
+Author-email: alaex777@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # freeze-uuid
 
 ## Python package for mocking uuid
 
 ### Usage Example
 
 ```python
@@ -31,8 +44,19 @@
 @freeze_uuid(['12af6b44-8181-11ee-b890-628ab7cd4d99', '12af6b44-8181-11ee-b890-628ab7cd4d98'])
 def test_uuid_list():
     assert str(uuid.uuid1()) == '12af6b44-8181-11ee-b890-628ab7cd4d99'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
 
-```
+```
+
+### Since library mocks uuid.UUID class, it can be used with all libraries, that support UUID class, i.e. uuid7
+
+```python
+from uuid_extensions import uuid7
+
+@freeze_uuid(TEST_UUID)
+def test_uuid_7():
+    assert str(uuid7()) == TEST_UUID
+
+```
```

### Comparing `freeze-uuid-0.3.0/freeze_uuid.egg-info/PKG-INFO` & `freeze_uuid-0.3.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: freeze-uuid
-Version: 0.3.0
-Summary: Python package for mocking uuid.
-Author: Alexander Balashov
-Author-email: alaex777@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # freeze-uuid
 
 ## Python package for mocking uuid
 
 ### Usage Example
 
 ```python
@@ -45,7 +32,18 @@
 def test_uuid_list():
     assert str(uuid.uuid1()) == '12af6b44-8181-11ee-b890-628ab7cd4d99'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
     assert str(uuid.uuid4()) == '12af6b44-8181-11ee-b890-628ab7cd4d98'
 
 ```
+
+### Since library mocks uuid.UUID class, it can be used with all libraries, that support UUID class, i.e. uuid7
+
+```python
+from uuid_extensions import uuid7
+
+@freeze_uuid(TEST_UUID)
+def test_uuid_7():
+    assert str(uuid7()) == TEST_UUID
+
+```
```

### Comparing `freeze-uuid-0.3.0/setup.py` & `freeze_uuid-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='freeze-uuid',
-    version='0.3.0',
+    version='0.3.1',
     author='Alexander Balashov',
     author_email='alaex777@gmail.com',
     description='Python package for mocking uuid.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     classifiers=[
```

### Comparing `freeze-uuid-0.3.0/tests/test_api.py` & `freeze_uuid-0.3.1/tests/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import uuid
+from uuid_extensions import uuid7
 
 import pytest
 
 from freeze_uuid import freeze_uuid
 
 from tests.testdata import (
     TEST_UUID, TEST_UUID_2, TEST_UUID_3, TEST_UUID_4,
@@ -91,7 +92,16 @@
     assert str(uuid.uuid4()) == '00000000-0000-0000-0000-000000000000'
 
 
 @freeze_uuid(TEST_UUID)
 def test_uuid_3():
     assert str(uuid.uuid3(uuid.NAMESPACE_DNS, 'google.com')) == TEST_UUID
     assert str(uuid.uuid5(uuid.NAMESPACE_DNS, 'google.com')) == TEST_UUID
+
+
+@freeze_uuid(TEST_UUID)
+def test_uuid_7():
+    assert str(uuid7()) == TEST_UUID
+
+
+def test_uuid_7_not_equal():
+    assert str(uuid7()) != TEST_UUID
```

