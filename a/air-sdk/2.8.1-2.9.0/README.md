# Comparing `tmp/air_sdk-2.8.1.tar.gz` & `tmp/air_sdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air_sdk-2.8.1.tar", max compression
+gzip compressed data, was "air_sdk-2.9.0.tar", max compression
```

## Comparing `air_sdk-2.8.1.tar` & `air_sdk-2.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    14657 2024-01-04 17:07:54.682951 air_sdk-2.8.1/LICENSE
--rw-r--r--   0        0        0     9167 2024-02-06 14:08:45.467197 air_sdk-2.8.1/README.md
--rw-r--r--   0        0        0      215 2024-01-04 17:07:54.683907 air_sdk-2.8.1/air_sdk/__init__.py
--rw-r--r--   0        0        0     3178 2024-01-04 17:07:54.684427 air_sdk-2.8.1/air_sdk/account.py
--rw-r--r--   0        0        0    11491 2024-01-11 13:51:14.733381 air_sdk-2.8.1/air_sdk/air_api.py
--rw-r--r--   0        0        0     7867 2024-01-04 17:07:54.687840 air_sdk-2.8.1/air_sdk/air_model.py
--rw-r--r--   0        0        0     1997 2024-01-04 17:07:54.688343 air_sdk-2.8.1/air_sdk/capacity.py
--rw-r--r--   0        0        0     2409 2024-01-04 17:07:54.690098 air_sdk-2.8.1/air_sdk/demo.py
--rw-r--r--   0        0        0     1808 2024-01-04 17:07:54.691872 air_sdk-2.8.1/air_sdk/exceptions.py
--rw-r--r--   0        0        0     4717 2024-01-04 17:07:54.693161 air_sdk-2.8.1/air_sdk/fleet.py
--rw-r--r--   0        0        0     5930 2024-02-06 14:08:50.528896 air_sdk-2.8.1/air_sdk/image.py
--rw-r--r--   0        0        0     2541 2024-01-04 17:07:54.698827 air_sdk-2.8.1/air_sdk/interface.py
--rw-r--r--   0        0        0     2581 2024-01-04 17:07:54.699418 air_sdk-2.8.1/air_sdk/job.py
--rw-r--r--   0        0        0     3742 2024-01-04 17:07:54.700025 air_sdk-2.8.1/air_sdk/link.py
--rw-r--r--   0        0        0      639 2024-01-04 17:07:54.701088 air_sdk-2.8.1/air_sdk/logger.py
--rw-r--r--   0        0        0     2096 2024-01-04 17:07:54.701784 air_sdk-2.8.1/air_sdk/login.py
--rw-r--r--   0        0        0     2377 2024-01-04 17:07:54.702950 air_sdk-2.8.1/air_sdk/marketplace.py
--rw-r--r--   0        0        0     4080 2024-01-04 17:07:54.704168 air_sdk-2.8.1/air_sdk/node.py
--rw-r--r--   0        0        0     9244 2024-01-08 17:28:49.133098 air_sdk-2.8.1/air_sdk/organization.py
--rw-r--r--   0        0        0     4635 2024-01-04 17:07:54.706872 air_sdk-2.8.1/air_sdk/permission.py
--rw-r--r--   0        0        0     2748 2024-01-04 17:07:54.708495 air_sdk-2.8.1/air_sdk/resource_budget.py
--rw-r--r--   0        0        0     6090 2024-01-04 17:07:54.710651 air_sdk-2.8.1/air_sdk/service.py
--rw-r--r--   0        0        0    12127 2024-01-08 17:29:02.972670 air_sdk-2.8.1/air_sdk/simulation.py
--rw-r--r--   0        0        0     3346 2024-01-04 17:07:54.713595 air_sdk-2.8.1/air_sdk/simulation_interface.py
--rw-r--r--   0        0        0     6805 2024-01-04 17:07:54.714331 air_sdk-2.8.1/air_sdk/simulation_node.py
--rw-r--r--   0        0        0     2804 2024-01-04 17:07:54.715019 air_sdk-2.8.1/air_sdk/ssh_key.py
--rw-r--r--   0        0        0     3410 2024-01-04 17:07:54.715729 air_sdk-2.8.1/air_sdk/token.py
--rw-r--r--   0        0        0     6433 2024-01-11 13:53:31.871755 air_sdk-2.8.1/air_sdk/topology.py
--rw-r--r--   0        0        0     2236 2024-01-04 17:07:54.716983 air_sdk-2.8.1/air_sdk/user_preference.py
--rw-r--r--   0        0        0     3466 2024-01-04 17:07:54.717474 air_sdk-2.8.1/air_sdk/util.py
--rw-r--r--   0        0        0     7209 2024-01-04 17:07:54.718038 air_sdk-2.8.1/air_sdk/worker.py
--rw-r--r--   0        0        0     1088 2024-02-06 14:09:51.645988 air_sdk-2.8.1/pyproject.toml
--rw-r--r--   0        0        0    10340 1970-01-01 00:00:00.000000 air_sdk-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0    14657 2024-01-04 17:07:54.682951 air_sdk-2.9.0/LICENSE
+-rw-r--r--   0        0        0     9167 2024-02-06 14:08:45.467197 air_sdk-2.9.0/README.md
+-rw-r--r--   0        0        0      215 2024-01-04 17:07:54.683907 air_sdk-2.9.0/air_sdk/__init__.py
+-rw-r--r--   0        0        0     3178 2024-01-04 17:07:54.684427 air_sdk-2.9.0/air_sdk/account.py
+-rw-r--r--   0        0        0    12029 2024-03-07 17:28:47.953672 air_sdk-2.9.0/air_sdk/air_api.py
+-rw-r--r--   0        0        0     7867 2024-01-04 17:07:54.687840 air_sdk-2.9.0/air_sdk/air_model.py
+-rw-r--r--   0        0        0     1997 2024-01-04 17:07:54.688343 air_sdk-2.9.0/air_sdk/capacity.py
+-rw-r--r--   0        0        0     2409 2024-01-04 17:07:54.690098 air_sdk-2.9.0/air_sdk/demo.py
+-rw-r--r--   0        0        0     1808 2024-01-04 17:07:54.691872 air_sdk-2.9.0/air_sdk/exceptions.py
+-rw-r--r--   0        0        0     4717 2024-01-04 17:07:54.693161 air_sdk-2.9.0/air_sdk/fleet.py
+-rw-r--r--   0        0        0     6990 2024-03-07 17:28:47.953839 air_sdk-2.9.0/air_sdk/image.py
+-rw-r--r--   0        0        0     2541 2024-01-04 17:07:54.698827 air_sdk-2.9.0/air_sdk/interface.py
+-rw-r--r--   0        0        0     2581 2024-01-04 17:07:54.699418 air_sdk-2.9.0/air_sdk/job.py
+-rw-r--r--   0        0        0     3742 2024-01-04 17:07:54.700025 air_sdk-2.9.0/air_sdk/link.py
+-rw-r--r--   0        0        0      639 2024-01-04 17:07:54.701088 air_sdk-2.9.0/air_sdk/logger.py
+-rw-r--r--   0        0        0     2096 2024-01-04 17:07:54.701784 air_sdk-2.9.0/air_sdk/login.py
+-rw-r--r--   0        0        0     2377 2024-01-04 17:07:54.702950 air_sdk-2.9.0/air_sdk/marketplace.py
+-rw-r--r--   0        0        0     4080 2024-01-04 17:07:54.704168 air_sdk-2.9.0/air_sdk/node.py
+-rw-r--r--   0        0        0     9244 2024-01-08 17:28:49.133098 air_sdk-2.9.0/air_sdk/organization.py
+-rw-r--r--   0        0        0     4635 2024-01-04 17:07:54.706872 air_sdk-2.9.0/air_sdk/permission.py
+-rw-r--r--   0        0        0     2748 2024-01-04 17:07:54.708495 air_sdk-2.9.0/air_sdk/resource_budget.py
+-rw-r--r--   0        0        0     6090 2024-01-04 17:07:54.710651 air_sdk-2.9.0/air_sdk/service.py
+-rw-r--r--   0        0        0    12127 2024-01-08 17:29:02.972670 air_sdk-2.9.0/air_sdk/simulation.py
+-rw-r--r--   0        0        0     3346 2024-01-04 17:07:54.713595 air_sdk-2.9.0/air_sdk/simulation_interface.py
+-rw-r--r--   0        0        0     6805 2024-01-04 17:07:54.714331 air_sdk-2.9.0/air_sdk/simulation_node.py
+-rw-r--r--   0        0        0     2804 2024-01-04 17:07:54.715019 air_sdk-2.9.0/air_sdk/ssh_key.py
+-rw-r--r--   0        0        0     3410 2024-01-04 17:07:54.715729 air_sdk-2.9.0/air_sdk/token.py
+-rw-r--r--   0        0        0     6433 2024-01-11 13:53:31.871755 air_sdk-2.9.0/air_sdk/topology.py
+-rw-r--r--   0        0        0     2236 2024-01-04 17:07:54.716983 air_sdk-2.9.0/air_sdk/user_preference.py
+-rw-r--r--   0        0        0     3466 2024-01-04 17:07:54.717474 air_sdk-2.9.0/air_sdk/util.py
+-rw-r--r--   0        0        0     7209 2024-01-04 17:07:54.718038 air_sdk-2.9.0/air_sdk/worker.py
+-rw-r--r--   0        0        0     1088 2024-03-07 17:28:47.954995 air_sdk-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10340 1970-01-01 00:00:00.000000 air_sdk-2.9.0/PKG-INFO
```

### Comparing `air_sdk-2.8.1/LICENSE` & `air_sdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/README.md` & `air_sdk-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/account.py` & `air_sdk-2.9.0/air_sdk/account.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/air_api.py` & `air_sdk-2.9.0/air_sdk/air_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,20 +46,28 @@
     'staging.air.cumulusnetworks.com',
 ]
 
 
 class AirSession(requests.Session):
     """Wrapper around requests.Session"""
 
+    default_connect_timeout = 16
+    default_read_timeout = 61
+
     def rebuild_auth(self, prepared_request, response):
         """Allow credential sharing between nvidia.com and cumulusnetworks.com only"""
         if urlparse(prepared_request.url).hostname in ALLOWED_HOSTS:
             return
         super().rebuild_auth(prepared_request, response)
 
+    def request(self, method, url, **kwargs):
+        """Override request method to pass the timeout"""
+        kwargs.setdefault('timeout', (self.default_connect_timeout, self.default_read_timeout))
+        return super().request(method, url, **kwargs)
+
 
 class AirApi:
     """
     Main interface for an API client instance
     """
 
     def __init__(self, api_url='https://air.nvidia.com/api/', api_version='v1', **kwargs):
@@ -284,19 +292,23 @@
             kwargs['params'] = _serialize_dict(kwargs['params'])
         logger.debug(f'request args: {args}')
         logger.debug(f'request kwargs: {kwargs}')
         res = self.client.request(method, url, allow_redirects=False, *args, **kwargs)
         if res.status_code == 301 and urlparse(res.headers.get('Location')).hostname in ALLOWED_HOSTS:
             res = self.client.request(method, res.headers['Location'], *args, **kwargs)
         if getattr(res, 'status_code') == 403:
+            missing_creds_err_msg = '{"detail":"Authentication credentials were not provided."}'
             if attempt_reauth and self._kwargs.get('username') and self._kwargs.get('password'):
                 logger.debug('Request failed with 403, attempting reauth')
                 self.authorize(**self._kwargs)
                 return self._request(method, url, *args, **{'attempt_reauth': False, **kwargs})
-            raise AirForbiddenError
+            if res.text != missing_creds_err_msg:
+                raise AirForbiddenError(res.text)
+            else:
+                raise AirForbiddenError
         try:
             res.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise AirUnexpectedResponse(err.response.text, err.response.status_code)
         return res
 
     def get(self, url, *args, **kwargs):
```

### Comparing `air_sdk-2.8.1/air_sdk/air_model.py` & `air_sdk-2.9.0/air_sdk/air_model.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/capacity.py` & `air_sdk-2.9.0/air_sdk/capacity.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/demo.py` & `air_sdk-2.9.0/air_sdk/demo.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/exceptions.py` & `air_sdk-2.9.0/air_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/fleet.py` & `air_sdk-2.9.0/air_sdk/fleet.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/image.py` & `air_sdk-2.9.0/air_sdk/image.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 """
 
 from . import util
 from .air_model import AirModel
 from .logger import air_sdk_logger as logger
 
 
-
 class Image(AirModel):
     """
     Manage an Image
 
     ### delete
     Delete the image. Once successful, the object should no longer be used and will raise
     [`AirDeletedObject`](/docs/exceptions) when referenced.
@@ -73,14 +72,49 @@
         [`AirUnexpectedResposne`](/docs/exceptions) - Upload failed
         """
         url = f'{self._api.url}{self.id}/upload/'
         with open(filename, 'rb') as image_file:
             res = self._api.client.put(url, data=image_file)
         util.raise_if_invalid_response(res, status_code=204, data_type=None)
 
+    @util.required_kwargs(['contact'])
+    def publish(self, contact: str):
+        """
+        Publish the image for public use
+
+        Arguments:
+            contact (str): The email address for the contact person associated with this image.
+
+        Raises:
+        [`AirUnexpectedResposne`](/docs/exceptions) - Publish failed
+        Example:
+        ```
+        >>> image.publish(contact='contact@nvidia.com')
+        ```
+        """
+        url = f'{self._api.url}{self.id}/publish/'
+        res = self._api.client.put(url, json={'contact': contact})
+        util.raise_if_invalid_response(res, status_code=204, data_type=None)
+
+    def unpublish(self):
+        """
+        Unpublish the image from public use
+
+        Raises:
+        [`AirUnexpectedResposne`](/docs/exceptions) - Unpublish failed
+
+        Example:
+        ```
+        >>> image.unpublish()
+        ```
+        """
+        url = f'{self._api.url}{self.id}/publish/'
+        res = self._api.client.delete(url)
+        util.raise_if_invalid_response(res, status_code=204, data_type=None)
+
     def __repr__(self):
         if self._deleted or not self.name:
             return super().__repr__()
         return f'<Image {self.name} {self.id}>'
 
 
 class ImageApi:
```

### Comparing `air_sdk-2.8.1/air_sdk/interface.py` & `air_sdk-2.9.0/air_sdk/interface.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/job.py` & `air_sdk-2.9.0/air_sdk/job.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/link.py` & `air_sdk-2.9.0/air_sdk/link.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/logger.py` & `air_sdk-2.9.0/air_sdk/logger.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/login.py` & `air_sdk-2.9.0/air_sdk/login.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/marketplace.py` & `air_sdk-2.9.0/air_sdk/marketplace.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/node.py` & `air_sdk-2.9.0/air_sdk/node.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/organization.py` & `air_sdk-2.9.0/air_sdk/organization.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/permission.py` & `air_sdk-2.9.0/air_sdk/permission.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/resource_budget.py` & `air_sdk-2.9.0/air_sdk/resource_budget.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/service.py` & `air_sdk-2.9.0/air_sdk/service.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/simulation.py` & `air_sdk-2.9.0/air_sdk/simulation.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/simulation_interface.py` & `air_sdk-2.9.0/air_sdk/simulation_interface.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/simulation_node.py` & `air_sdk-2.9.0/air_sdk/simulation_node.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/ssh_key.py` & `air_sdk-2.9.0/air_sdk/ssh_key.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/token.py` & `air_sdk-2.9.0/air_sdk/token.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/topology.py` & `air_sdk-2.9.0/air_sdk/topology.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/user_preference.py` & `air_sdk-2.9.0/air_sdk/user_preference.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/util.py` & `air_sdk-2.9.0/air_sdk/util.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/air_sdk/worker.py` & `air_sdk-2.9.0/air_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `air_sdk-2.8.1/pyproject.toml` & `air_sdk-2.9.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "air-sdk"
-version = "2.8.1"
+version = "2.9.0"
 description = "Python SDK for interacting with NVIDIA Air"
 license = "MIT"
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 homepage = "https://github.com/NVIDIA/air_sdk"
 authors = ["NVIDIA Air <air-support@nvidia.com>"]
 readme = "README.md"
 
@@ -12,17 +12,17 @@
 python = "^3.7.2"
 python-dateutil = "2.8.2"
 requests = "2.31.0"
 
 # Optional extras for development
 coverage = { version = "7.2.7", optional = true}
 pre-commit = {version = "2.21", optional = true}
-pytest = { version = "7.4.0", optional = true}
+pytest = { version = "7.4.4", optional = true}
 requests-mock = { version = "1.11.0", optional = true}
-ruff = { version = "0.1.7", optional = true}
+ruff = { version = "0.2.1", optional = true}
 
 [tool.poetry.extras]
 dev = [
     "coverage",
     "pre-commit",
     "pytest",
     "requests_mock",
```

### Comparing `air_sdk-2.8.1/PKG-INFO` & `air_sdk-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: air-sdk
-Version: 2.8.1
+Version: 2.9.0
 Summary: Python SDK for interacting with NVIDIA Air
 Home-page: https://github.com/NVIDIA/air_sdk
 License: MIT
 Author: NVIDIA Air
 Author-email: air-support@nvidia.com
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: dev
 Requires-Dist: coverage (==7.2.7) ; extra == "dev"
 Requires-Dist: pre-commit (==2.21) ; extra == "dev"
-Requires-Dist: pytest (==7.4.0) ; extra == "dev"
+Requires-Dist: pytest (==7.4.4) ; extra == "dev"
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: requests-mock (==1.11.0) ; extra == "dev"
-Requires-Dist: ruff (==0.1.7) ; extra == "dev"
+Requires-Dist: ruff (==0.2.1) ; extra == "dev"
 Project-URL: Bug Tracker, https://github.com/NVIDIA/air_sdk/issues
 Project-URL: Homepage, https://github.com/NVIDIA/air_sdk/issues
 Description-Content-Type: text/markdown
 
 # air_sdk
 
 This project provides a Python SDK for interacting with the NVIDIA Air API (https://air.nvidia.com/api/).
```

