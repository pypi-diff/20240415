# Comparing `tmp/requests_oauth2client-1.5.1.tar.gz` & `tmp/requests_oauth2client-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_oauth2client-1.5.1.tar", max compression
+gzip compressed data, was "requests_oauth2client-1.5.2.tar", max compression
```

## Comparing `requests_oauth2client-1.5.1.tar` & `requests_oauth2client-1.5.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      126 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/AUTHORS.md
--rw-r--r--   0        0        0      586 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/LICENSE
--rw-r--r--   0        0        0    42324 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/README.md
--rw-r--r--   0        0        0     3404 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     4915 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/requests_oauth2client/__init__.py
--rw-r--r--   0        0        0    20663 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/requests_oauth2client/api_client.py
--rw-r--r--   0        0        0    15250 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/requests_oauth2client/auth.py
--rw-r--r--   0        0        0    30628 2024-03-12 10:11:04.421001 requests_oauth2client-1.5.1/requests_oauth2client/authorization_request.py
--rw-r--r--   0        0        0     5230 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/backchannel_authentication.py
--rw-r--r--   0        0        0    65234 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/client.py
--rw-r--r--   0        0        0    15640 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/client_authentication.py
--rw-r--r--   0        0        0     4348 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/device_authorization.py
--rw-r--r--   0        0        0     2775 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/discovery.py
--rw-r--r--   0        0        0     8319 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/exceptions.py
--rw-r--r--   0        0        0      228 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/flask/__init__.py
--rw-r--r--   0        0        0     2552 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/flask/auth.py
--rw-r--r--   0        0        0     3491 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/pooling.py
--rw-r--r--   0        0        0        0 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/py.typed
--rw-r--r--   0        0        0    17344 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/tokens.py
--rw-r--r--   0        0        0     3588 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/utils.py
--rw-r--r--   0        0        0      293 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/vendor_specific/__init__.py
--rw-r--r--   0        0        0     5104 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/vendor_specific/auth0.py
--rw-r--r--   0        0        0     2379 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/requests_oauth2client/vendor_specific/ping.py
--rw-r--r--   0        0        0      550 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/.coveragerc
--rw-r--r--   0        0        0        0 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/__init__.py
--rw-r--r--   0        0        0    20551 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/conftest.py
--rw-r--r--   0        0        0     7304 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/test_authorization_code.py
--rw-r--r--   0        0        0     2068 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/test_client_credentials.py
--rw-r--r--   0        0        0     4888 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/test_device_authorization.py
--rw-r--r--   0        0        0     3358 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/test_oidc.py
--rw-r--r--   0        0        0     2006 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/test_refresh_token.py
--rw-r--r--   0        0        0     5675 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/test_token_exchange.py
--rw-r--r--   0        0        0        0 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/__init__.py
--rw-r--r--   0        0        0    16685 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/conftest.py
--rw-r--r--   0        0        0    11645 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_api_client.py
--rw-r--r--   0        0        0     8702 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_auth.py
--rw-r--r--   0        0        0    10541 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_authorization_request.py
--rw-r--r--   0        0        0    10149 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_backchannel_authentication.py
--rw-r--r--   0        0        0    57347 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_client.py
--rw-r--r--   0        0        0     6095 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_client_authentication.py
--rw-r--r--   0        0        0     7773 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_device_authorization.py
--rw-r--r--   0        0        0     1909 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_discovery.py
--rw-r--r--   0        0        0     3392 2024-03-12 10:11:04.425001 requests_oauth2client-1.5.1/tests/unit_tests/test_flask.py
--rw-r--r--   0        0        0    21063 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/test_oidc.py
--rw-r--r--   0        0        0     1460 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/test_pkce.py
--rw-r--r--   0        0        0    11502 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/test_tokens.py
--rw-r--r--   0        0        0     1248 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/test_utils.py
--rw-r--r--   0        0        0        0 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/vendor_specific/__init__.py
--rw-r--r--   0        0        0     1828 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/vendor_specific/test_auth0.py
--rw-r--r--   0        0        0     1752 2024-03-12 10:11:04.429001 requests_oauth2client-1.5.1/tests/unit_tests/vendor_specific/test_ping.py
--rw-r--r--   0        0        0    43327 1970-01-01 00:00:00.000000 requests_oauth2client-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2024-04-15 12:48:08.410838 requests_oauth2client-1.5.2/AUTHORS.md
+-rw-r--r--   0        0        0      586 2024-04-15 12:48:08.410838 requests_oauth2client-1.5.2/LICENSE
+-rw-r--r--   0        0        0    42324 2024-04-15 12:48:08.410838 requests_oauth2client-1.5.2/README.md
+-rw-r--r--   0        0        0     3405 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4915 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/__init__.py
+-rw-r--r--   0        0        0    20663 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/api_client.py
+-rw-r--r--   0        0        0    15250 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/auth.py
+-rw-r--r--   0        0        0    30628 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/authorization_request.py
+-rw-r--r--   0        0        0     5230 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/backchannel_authentication.py
+-rw-r--r--   0        0        0    65234 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/client.py
+-rw-r--r--   0        0        0    15640 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/client_authentication.py
+-rw-r--r--   0        0        0     4348 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/device_authorization.py
+-rw-r--r--   0        0        0     2775 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/discovery.py
+-rw-r--r--   0        0        0     8319 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/exceptions.py
+-rw-r--r--   0        0        0      228 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/flask/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/flask/auth.py
+-rw-r--r--   0        0        0     3491 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/pooling.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/py.typed
+-rw-r--r--   0        0        0    17344 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/tokens.py
+-rw-r--r--   0        0        0     3588 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/utils.py
+-rw-r--r--   0        0        0      293 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/__init__.py
+-rw-r--r--   0        0        0     5104 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/auth0.py
+-rw-r--r--   0        0        0     2379 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/ping.py
+-rw-r--r--   0        0        0      550 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/.coveragerc
+-rw-r--r--   0        0        0        0 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/__init__.py
+-rw-r--r--   0        0        0    20551 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/conftest.py
+-rw-r--r--   0        0        0     7304 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_authorization_code.py
+-rw-r--r--   0        0        0     2068 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_client_credentials.py
+-rw-r--r--   0        0        0     4888 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_device_authorization.py
+-rw-r--r--   0        0        0     3358 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_oidc.py
+-rw-r--r--   0        0        0     2006 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_refresh_token.py
+-rw-r--r--   0        0        0     5675 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/test_token_exchange.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/__init__.py
+-rw-r--r--   0        0        0    16685 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/conftest.py
+-rw-r--r--   0        0        0    11645 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_api_client.py
+-rw-r--r--   0        0        0     8702 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_auth.py
+-rw-r--r--   0        0        0    10541 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_authorization_request.py
+-rw-r--r--   0        0        0    10149 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_backchannel_authentication.py
+-rw-r--r--   0        0        0    57347 2024-04-15 12:48:08.414838 requests_oauth2client-1.5.2/tests/unit_tests/test_client.py
+-rw-r--r--   0        0        0     6095 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_client_authentication.py
+-rw-r--r--   0        0        0     7773 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_device_authorization.py
+-rw-r--r--   0        0        0     1909 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_discovery.py
+-rw-r--r--   0        0        0     3392 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_flask.py
+-rw-r--r--   0        0        0    21063 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_oidc.py
+-rw-r--r--   0        0        0     1460 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_pkce.py
+-rw-r--r--   0        0        0    11502 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_tokens.py
+-rw-r--r--   0        0        0     1248 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/__init__.py
+-rw-r--r--   0        0        0     1828 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_auth0.py
+-rw-r--r--   0        0        0     1752 2024-04-15 12:48:08.418838 requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_ping.py
+-rw-r--r--   0        0        0    43327 1970-01-01 00:00:00.000000 requests_oauth2client-1.5.2/PKG-INFO
```

### Comparing `requests_oauth2client-1.5.1/LICENSE` & `requests_oauth2client-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/README.md` & `requests_oauth2client-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/pyproject.toml` & `requests_oauth2client-1.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "requests_oauth2client"
-version = "1.5.1"
+version = "1.5.2"
 homepage = "https://github.com/guillp/requests_oauth2client"
 description = "An OAuth2.x client based on `requests`."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'Development Status :: 4 - Beta',
@@ -13,15 +13,15 @@
     'Topic :: Security',
     'License :: OSI Approved :: Apache Software License',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
-    'Programming Language :: Python :: 3.12'
+    'Programming Language :: Python :: 3.12',
 ]
 packages = [
     { include = "requests_oauth2client" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/__init__.py` & `requests_oauth2client-1.5.2/requests_oauth2client/__init__.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/api_client.py` & `requests_oauth2client-1.5.2/requests_oauth2client/api_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/auth.py` & `requests_oauth2client-1.5.2/requests_oauth2client/auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/authorization_request.py` & `requests_oauth2client-1.5.2/requests_oauth2client/authorization_request.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/backchannel_authentication.py` & `requests_oauth2client-1.5.2/requests_oauth2client/backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/client.py` & `requests_oauth2client-1.5.2/requests_oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/client_authentication.py` & `requests_oauth2client-1.5.2/requests_oauth2client/client_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/device_authorization.py` & `requests_oauth2client-1.5.2/requests_oauth2client/device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/discovery.py` & `requests_oauth2client-1.5.2/requests_oauth2client/discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/exceptions.py` & `requests_oauth2client-1.5.2/requests_oauth2client/exceptions.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/flask/auth.py` & `requests_oauth2client-1.5.2/requests_oauth2client/flask/auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/pooling.py` & `requests_oauth2client-1.5.2/requests_oauth2client/pooling.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/tokens.py` & `requests_oauth2client-1.5.2/requests_oauth2client/tokens.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/utils.py` & `requests_oauth2client-1.5.2/requests_oauth2client/utils.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/vendor_specific/auth0.py` & `requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/auth0.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/requests_oauth2client/vendor_specific/ping.py` & `requests_oauth2client-1.5.2/requests_oauth2client/vendor_specific/ping.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/.coveragerc` & `requests_oauth2client-1.5.2/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/conftest.py` & `requests_oauth2client-1.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/test_authorization_code.py` & `requests_oauth2client-1.5.2/tests/test_authorization_code.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/test_client_credentials.py` & `requests_oauth2client-1.5.2/tests/test_client_credentials.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/test_device_authorization.py` & `requests_oauth2client-1.5.2/tests/test_device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/test_oidc.py` & `requests_oauth2client-1.5.2/tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/test_refresh_token.py` & `requests_oauth2client-1.5.2/tests/test_refresh_token.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/test_token_exchange.py` & `requests_oauth2client-1.5.2/tests/test_token_exchange.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/conftest.py` & `requests_oauth2client-1.5.2/tests/unit_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_api_client.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_auth.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_authorization_request.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_authorization_request.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_backchannel_authentication.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_backchannel_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_client.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_client.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_client_authentication.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_client_authentication.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_device_authorization.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_device_authorization.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_discovery.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_flask.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_oidc.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_oidc.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_pkce.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_pkce.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_tokens.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/test_utils.py` & `requests_oauth2client-1.5.2/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/vendor_specific/test_auth0.py` & `requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_auth0.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/tests/unit_tests/vendor_specific/test_ping.py` & `requests_oauth2client-1.5.2/tests/unit_tests/vendor_specific/test_ping.py`

 * *Files identical despite different names*

### Comparing `requests_oauth2client-1.5.1/PKG-INFO` & `requests_oauth2client-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests_oauth2client
-Version: 1.5.1
+Version: 1.5.2
 Summary: An OAuth2.x client based on `requests`.
 Home-page: https://github.com/guillp/requests_oauth2client
 License: Apache-2.0
 Author: Guillaume Pujol
 Author-email: guill.p.linux@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
```

