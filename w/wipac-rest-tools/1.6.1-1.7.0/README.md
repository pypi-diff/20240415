# Comparing `tmp/wipac-rest-tools-1.6.1.tar.gz` & `tmp/wipac-rest-tools-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.6.1.tar", last modified: Wed Mar  6 19:53:04 2024, max compression
+gzip compressed data, was "wipac-rest-tools-1.7.0.tar", last modified: Mon Apr 15 15:28:10 2024, max compression
```

## Comparing `wipac-rest-tools-1.6.1.tar` & `wipac-rest-tools-1.7.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6028 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4958 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 19:53:04.215511 wipac-rest-tools-1.6.1/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2024-03-06 19:53:02.000000 wipac-rest-tools-1.6.1/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      605 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15182 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1960 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     7380 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     3048 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2523 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      798 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8514 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    12766 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    18560 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2251 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5388 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4832 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2273 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-03-06 19:53:01.000000 wipac-rest-tools-1.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-06 19:53:04.219511 wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6028 2024-03-06 19:53:04.000000 wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      815 2024-03-06 19:53:04.000000 wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-06 19:53:04.000000 wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      546 2024-03-06 19:53:04.000000 wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-06 19:53:04.000000 wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:28:10.677048 wipac-rest-tools-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-04-15 15:28:10.677048 wipac-rest-tools-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4958 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:28:10.669047 wipac-rest-tools-1.7.0/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:28:10.673048 wipac-rest-tools-1.7.0/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15182 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1960 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     7380 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     3048 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)     2593 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:28:10.673048 wipac-rest-tools-1.7.0/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      843 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    17104 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    18560 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:28:10.673048 wipac-rest-tools-1.7.0/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5388 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-04-15 15:28:10.677048 wipac-rest-tools-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2024-04-15 15:28:08.000000 wipac-rest-tools-1.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:28:10.677048 wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-04-15 15:28:10.000000 wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-15 15:28:10.000000 wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 15:28:10.000000 wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2024-04-15 15:28:10.000000 wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-15 15:28:10.000000 wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.6.1/LICENSE` & `wipac-rest-tools-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/PKG-INFO` & `wipac-rest-tools-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.6.1
+Version: 1.7.0
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: openapi
 Provides-Extra: telemetry
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: mypy
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
```

### Comparing `wipac-rest-tools-1.6.1/README.md` & `wipac-rest-tools-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/__init__.py` & `wipac-rest-tools-1.7.0/rest_tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.6.1"
+__version__ = "1.7.0"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.6.1/rest_tools/client/__init__.py` & `wipac-rest-tools-1.7.0/rest_tools/client/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Sub-package __init__."""
 
+from . import utils
 from .client import (
     MAX_RETRIES,
     CalcRetryFromBackoffMax,
     CalcRetryFromWaittimeMax,
     RestClient,
 )
 from .client_credentials import ClientCredentialsAuth
@@ -18,8 +19,9 @@
     "DeviceGrantAuth",
     "SavedDeviceGrantAuth",
     "AsyncSession",
     "Session",
     "CalcRetryFromBackoffMax",
     "CalcRetryFromWaittimeMax",
     "MAX_RETRIES",
+    "utils",
 ]
```

### Comparing `wipac-rest-tools-1.6.1/rest_tools/client/client.py` & `wipac-rest-tools-1.7.0/rest_tools/client/client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.7.0/rest_tools/client/client_credentials.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/client/device_client.py` & `wipac-rest-tools-1.7.0/rest_tools/client/device_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.7.0/rest_tools/client/openid_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/client/session.py` & `wipac-rest-tools-1.7.0/rest_tools/client/session.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/server/__init__.py` & `wipac-rest-tools-1.7.0/rest_tools/server/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Sub-package __init__."""
 
-
 from .arghandler import ArgumentHandler, ArgumentSource
 from .decorators import (
     authenticated,
     catch_error,
     keycloak_role_auth,
     role_authorization,
     scope_role_auth,
     token_attribute_role_mapping_auth,
+    validate_request,
 )
 from .handler import (
     KeycloakUsernameMixin,
     OpenIDCookieHandlerMixin,
     OpenIDLoginHandler,
     RestHandler,
     RestHandlerSetup,
@@ -30,8 +30,9 @@
     "catch_error",
     "role_authorization",
     "scope_role_auth",
     "keycloak_role_auth",
     "token_attribute_role_mapping_auth",
     "ArgumentHandler",
     "ArgumentSource",
+    "validate_request",
 ]
```

### Comparing `wipac-rest-tools-1.6.1/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.7.0/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/server/decorators.py` & `wipac-rest-tools-1.7.0/rest_tools/server/decorators.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """decorators.py."""
 
-
 # fmt:off
 
 import logging
+import os
 import re
 from functools import wraps
 from inspect import isawaitable
 
 import requests.exceptions
 import tornado.web
 
 from .. import telemetry as wtt
 
 LOGGER = logging.getLogger(__name__)
 
 
+########################################################################################################################
+
+
 def authenticated(method):
     """Decorate methods with this to require that the Authorization header is
     filled with a valid token. Does *not* check the authorization of the token,
     just that it exists.
 
     On failure, raises a 403 error.
 
@@ -35,14 +38,17 @@
         if isawaitable(ret):
             return await ret
         else:
             return ret
     return wrapper
 
 
+########################################################################################################################
+
+
 def catch_error(method):
     """Decorator to catch and handle errors on handlers.
 
     All failures caught here
     """
     @wraps(method)
     async def wrapper(self, *args, **kwargs):
@@ -77,14 +83,17 @@
                 pass  # ignore statsd errors
             message = 'Error in '+self.__class__.__name__
             self.send_error(500, reason=message)
         return None
     return wrapper
 
 
+########################################################################################################################
+
+
 def role_authorization(**_auth):
     """Handle RBAC authorization.
 
     Like :py:func:`authenticated`, this requires the Authorization header
     to be filled with a valid token.  Note that calling both decorators
     is not necessary, as this decorator will perform authentication
     checking as well.
@@ -116,14 +125,17 @@
                 return await ret
             else:
                 return ret
         return wrapper
     return make_wrapper
 
 
+########################################################################################################################
+
+
 def scope_role_auth(**_auth):
     """Handle RBAC authorization using oauth2 scopes.
 
     Like :py:func:`authenticated`, this requires the Authorization header
     to be filled with a valid token.  Note that calling both decorators
     is not necessary, as this decorator will perform authentication
     checking as well.
@@ -165,14 +177,17 @@
                 return await ret
             else:
                 return ret
         return wrapper
     return make_wrapper
 
 
+########################################################################################################################
+
+
 def keycloak_role_auth(**_auth):
     """Handle RBAC authorization using keycloak realm roles.
     Like :py:func:`authenticated`, this requires the Authorization header
     to be filled with a valid token.  Note that calling both decorators
     is not necessary, as this decorator will perform authentication
     checking as well.
 
@@ -210,14 +225,17 @@
                 return await ret
             else:
                 return ret
         return wrapper
     return make_wrapper
 
 
+########################################################################################################################
+
+
 def token_attribute_role_mapping_auth(role_attrs, group_attrs=None):
     """Handle RBAC authorization by creating a decorator that maps token
     attributes to roles, then using the decorator to allow access to functions
     by role.  Can also map groups and add that to auth data.
 
     Like :py:func:`authenticated`, this requires the Authorization header
     to be filled with a valid token.  Note that calling both decorators
@@ -353,7 +371,91 @@
                 if isawaitable(ret):
                     return await ret
                 else:
                     return ret
             return wrapper
         return make_wrapper
     return make_decorator
+
+
+########################################################################################################################
+# fmt:on
+
+try:
+    import openapi_core
+    from openapi_core import OpenAPI
+    from openapi_core.contrib import requests as openapi_core_requests
+    from openapi_core.validation.exceptions import ValidationError
+except ImportError:
+    pass  # if client code wants to use these features, then let the built-in errors raise
+
+
+def validate_request(openapi_spec: "OpenAPI"):
+    """Validate request obj against the given OpenAPI spec."""
+
+    def make_wrapper(method):  # type: ignore[no-untyped-def]
+        async def wrapper(zelf: tornado.web.RequestHandler, *args, **kwargs):  # type: ignore[no-untyped-def]
+            LOGGER.info("validating with openapi spec")
+            # NOTE - don't change data (unmarshal) b/c we are downstream of data separation
+            try:
+                # https://openapi-core.readthedocs.io/en/latest/validation.html
+                openapi_spec.validate_request(
+                    _http_server_request_to_openapi_request(zelf.request),
+                )
+            except ValidationError as e:
+                LOGGER.error(f"invalid request: {e.__class__.__name__} - {e}")
+                if isinstance(  # look at the ORIGINAL exception that caused this error
+                    e.__context__,
+                    openapi_core.validation.schemas.exceptions.InvalidSchemaValue,
+                ):
+                    reason = "; ".join(  # to client
+                        # verbose details after newline
+                        str(x).split("\n", maxsplit=1)[0]
+                        for x in e.__context__.schema_errors
+                    )
+                else:
+                    reason = str(e)  # to client
+                if os.getenv("CI"):
+                    # in prod, don't fill up logs w/ traces from invalid data
+                    LOGGER.exception(e)
+                raise tornado.web.HTTPError(
+                    status_code=400,
+                    log_message=f"{e.__class__.__name__}: {e}",  # to stderr
+                    reason=reason,  # to client
+                )
+            except Exception as e:
+                LOGGER.error(f"unexpected exception: {e.__class__.__name__} - {e}")
+                LOGGER.exception(e)
+                raise tornado.web.HTTPError(
+                    status_code=400,
+                    log_message=f"{e.__class__.__name__}: {e}",  # to stderr
+                    reason=None,  # to client (don't send possibly sensitive info)
+                )
+
+            return await method(zelf, *args, **kwargs)
+
+        return wrapper
+
+    return make_wrapper
+
+
+def _http_server_request_to_openapi_request(
+    req: tornado.httputil.HTTPServerRequest,
+) -> "openapi_core_requests.RequestsOpenAPIRequest":
+    """Convert a `tornado.httputil.HTTPServerRequest` to openapi's type."""
+    return openapi_core_requests.RequestsOpenAPIRequest(
+        requests.Request(
+            method=req.method.lower() if req.method else "get",
+            url=f"{req.protocol}://{req.host}{req.uri}",
+            headers=req.headers,
+            files=req.files,
+            data=req.body if not req.body_arguments else None,  # see below
+            params=req.query_arguments,
+            # auth=None,
+            cookies=req.cookies,
+            # hooks=None,
+            json=req.body_arguments if req.body_arguments else None,  # see above
+        )
+    )
+
+
+########################################################################################################################
```

### Comparing `wipac-rest-tools-1.6.1/rest_tools/server/handler.py` & `wipac-rest-tools-1.7.0/rest_tools/server/handler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/server/server.py` & `wipac-rest-tools-1.7.0/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/server/stats.py` & `wipac-rest-tools-1.7.0/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/telemetry.py` & `wipac-rest-tools-1.7.0/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/utils/auth.py` & `wipac-rest-tools-1.7.0/rest_tools/utils/auth.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.7.0/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.7.0/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.6.1/setup.cfg` & `wipac-rest-tools-1.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,16 @@
 	tornado
 	urllib3>=2.0.4
 	wipac-dev-tools
 python_requires = >=3.8, <3.13
 packages = find:
 
 [options.extras_require]
+openapi = 
+	openapi-core
 telemetry = 
 	wipac-telemetry >= 0.2.4
 tests = 
 	coverage
 	flake8
 	httpretty
 	pycycle
@@ -85,14 +87,15 @@
 	pytest-asyncio
 	pytest-mock
 	requests-mock
 	ruff
 	types-requests
 	wheel
 mypy = 
+	%(openapi)s
 	%(telemetry)s
 	%(tests)s
 	%(dev)s
 
 [options.package_data]
 * = py.typed
```

### Comparing `wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.6.1
+Version: 1.7.0
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: openapi
 Provides-Extra: telemetry
 Provides-Extra: tests
 Provides-Extra: dev
 Provides-Extra: mypy
 License-File: LICENSE
 
 <!--- Top of README Badges (automated) --->
```

### Comparing `wipac-rest-tools-1.6.1/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.7.0/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 rest_tools/telemetry.py
 rest_tools/client/__init__.py
 rest_tools/client/client.py
 rest_tools/client/client_credentials.py
 rest_tools/client/device_client.py
 rest_tools/client/openid_client.py
 rest_tools/client/session.py
+rest_tools/client/utils.py
 rest_tools/server/__init__.py
 rest_tools/server/arghandler.py
 rest_tools/server/decorators.py
 rest_tools/server/handler.py
 rest_tools/server/server.py
 rest_tools/server/stats.py
 rest_tools/utils/__init__.py
```

