# Comparing `tmp/pynoesmartmeter-0.3.2.tar.gz` & `tmp/pynoesmartmeter-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynoesmartmeter-0.3.2.tar", max compression
+gzip compressed data, was "pynoesmartmeter-0.3.3.tar", max compression
```

## Comparing `pynoesmartmeter-0.3.2.tar` & `pynoesmartmeter-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.3.2/LICENSE
--rw-r--r--   0        0        0     1716 2024-04-15 15:15:57.546593 pynoesmartmeter-0.3.2/README.md
--rw-r--r--   0        0        0      507 2024-04-15 16:51:03.641536 pynoesmartmeter-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.3.2/src/pynoesmartmeter/__init__.py
--rw-r--r--   0        0        0    10156 2024-04-15 16:50:55.913650 pynoesmartmeter-0.3.2/src/pynoesmartmeter/client.py
--rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.3.2/src/pynoesmartmeter/errors.py
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 pynoesmartmeter-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.3.3/LICENSE
+-rw-r--r--   0        0        0     1716 2024-04-15 15:15:57.546593 pynoesmartmeter-0.3.3/README.md
+-rw-r--r--   0        0        0      507 2024-04-15 16:54:02.120871 pynoesmartmeter-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.3.3/src/pynoesmartmeter/__init__.py
+-rw-r--r--   0        0        0    10168 2024-04-15 16:53:30.287988 pynoesmartmeter-0.3.3/src/pynoesmartmeter/client.py
+-rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.3.3/src/pynoesmartmeter/errors.py
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 pynoesmartmeter-0.3.3/PKG-INFO
```

### Comparing `pynoesmartmeter-0.3.2/LICENSE` & `pynoesmartmeter-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.3.2/README.md` & `pynoesmartmeter-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.3.2/src/pynoesmartmeter/client.py` & `pynoesmartmeter-0.3.3/src/pynoesmartmeter/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
         self._username = username
         self._password = password
 
     async def authenticate(self, username = None, password = None):
         """Load session file or authenticate user."""
         if username is not None:
             self._username = username
-            self._clear_stored_session()
+            await self._clear_stored_session()
         if password is not None:
             self._password = password
-            self._clear_stored_session()
+            await self._clear_stored_session()
 
         if await self._load_check_session():
            return True
 
         print("Starting new session and authenticate")
         session = httpx.AsyncClient(timeout=30.0)
         auth_data = {"user": self._username, "pwd": self._password}
```

### Comparing `pynoesmartmeter-0.3.2/src/pynoesmartmeter/errors.py` & `pynoesmartmeter-0.3.3/src/pynoesmartmeter/errors.py`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.3.2/PKG-INFO` & `pynoesmartmeter-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynoesmartmeter
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python library to access the Netz Nö (EVN) Smart Meter private API
 License: MIT
 Author: David Illichmann
 Author-email: david.illichmann@ebcont.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.3.2 Summary: Python
+Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.3.3 Summary: Python
 library to access the Netz NÃ¶ (EVN) Smart Meter private API License: MIT
 Author: David Illichmann Author-email: david.illichmann@ebcont.com Requires-
 Python: >=3.12,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-
 Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/
```

