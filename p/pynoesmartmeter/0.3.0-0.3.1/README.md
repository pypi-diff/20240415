# Comparing `tmp/pynoesmartmeter-0.3.0.tar.gz` & `tmp/pynoesmartmeter-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynoesmartmeter-0.3.0.tar", max compression
+gzip compressed data, was "pynoesmartmeter-0.3.1.tar", max compression
```

## Comparing `pynoesmartmeter-0.3.0.tar` & `pynoesmartmeter-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.3.0/LICENSE
--rw-r--r--   0        0        0     1716 2024-04-15 15:15:57.546593 pynoesmartmeter-0.3.0/README.md
--rw-r--r--   0        0        0      507 2024-04-15 15:16:42.628054 pynoesmartmeter-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.3.0/src/pynoesmartmeter/__init__.py
--rw-r--r--   0        0        0     9886 2024-04-15 15:11:39.403601 pynoesmartmeter-0.3.0/src/pynoesmartmeter/client.py
--rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.3.0/src/pynoesmartmeter/errors.py
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 pynoesmartmeter-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1716 2024-04-15 15:15:57.546593 pynoesmartmeter-0.3.1/README.md
+-rw-r--r--   0        0        0      507 2024-04-15 16:45:36.931017 pynoesmartmeter-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.3.1/src/pynoesmartmeter/__init__.py
+-rw-r--r--   0        0        0    10028 2024-04-15 16:45:25.822278 pynoesmartmeter-0.3.1/src/pynoesmartmeter/client.py
+-rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.3.1/src/pynoesmartmeter/errors.py
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 pynoesmartmeter-0.3.1/PKG-INFO
```

### Comparing `pynoesmartmeter-0.3.0/LICENSE` & `pynoesmartmeter-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.3.0/README.md` & `pynoesmartmeter-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.3.0/src/pynoesmartmeter/client.py` & `pynoesmartmeter-0.3.1/src/pynoesmartmeter/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,20 +35,23 @@
         self._account_id = None
         self._session = None
         self._username = username
         self._password = password
 
     async def authenticate(self, username = None, password = None):
         """Load session file or authenticate user."""
+        credentials_changed = False
         if username is not None:
             self._username = username
+            credentials_changed = True
         if password is not None:
             self._password = password
+            credentials_changed = True
 
-        if await self._load_check_session():
+        if not credentials_changed and await self._load_check_session():
            return True
 
         print("Starting new session and authenticate")
         session = httpx.AsyncClient(timeout=30.0)
         auth_data = {"user": self._username, "pwd": self._password}
         response = await session.post(self.AUTH_URL, data=auth_data)
```

### Comparing `pynoesmartmeter-0.3.0/src/pynoesmartmeter/errors.py` & `pynoesmartmeter-0.3.1/src/pynoesmartmeter/errors.py`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.3.0/PKG-INFO` & `pynoesmartmeter-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynoesmartmeter
-Version: 0.3.0
+Version: 0.3.1
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
-Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.3.0 Summary: Python
+Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.3.1 Summary: Python
 library to access the Netz NÃ¶ (EVN) Smart Meter private API License: MIT
 Author: David Illichmann Author-email: david.illichmann@ebcont.com Requires-
 Python: >=3.12,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-
 Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/
```

