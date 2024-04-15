# Comparing `tmp/mms_client-1.2.0.tar.gz` & `tmp/mms_client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.2.0.tar", max compression
+gzip compressed data, was "mms_client-1.3.0.tar", max compression
```

## Comparing `mms_client-1.2.0.tar` & `mms_client-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1211 2024-04-12 06:19:54.160302 mms_client-1.2.0/LICENSE
--rw-r--r--   0        0        0    13458 2024-04-12 06:19:54.160302 mms_client-1.2.0/README.md
--rw-r--r--   0        0        0     2913 2024-04-12 06:19:54.164302 mms_client-1.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/__init__.py
--rw-r--r--   0        0        0      571 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    25839 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/services/base.py
--rw-r--r--   0        0        0     6169 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/services/market.py
--rw-r--r--   0        0        0      521 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3419 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      537 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0     9701 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/base.py
--rw-r--r--   0        0        0      464 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    12065 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2588 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/market.py
--rw-r--r--   0        0        0     7693 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-04-12 06:19:54.164302 mms_client-1.2.0/src/mms_client/types/registration.py
--rw-r--r--   0        0        0    66466 2024-04-12 06:19:54.168302 mms_client-1.2.0/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4407 2024-04-12 06:19:54.168302 mms_client-1.2.0/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-04-12 06:19:54.168302 mms_client-1.2.0/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     2306 2024-04-12 06:19:54.168302 mms_client-1.2.0/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    27203 2024-04-12 06:19:54.168302 mms_client-1.2.0/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0     9653 2024-04-12 06:19:54.168302 mms_client-1.2.0/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    14742 1970-01-01 00:00:00.000000 mms_client-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-15 05:26:06.886885 mms_client-1.3.0/LICENSE
+-rw-r--r--   0        0        0    13490 2024-04-15 05:26:06.886885 mms_client-1.3.0/README.md
+-rw-r--r--   0        0        0     2913 2024-04-15 05:26:06.886885 mms_client-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-04-15 05:26:06.886885 mms_client-1.3.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    25839 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     7574 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      521 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3651 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      537 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9701 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0    65974 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4399 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    29534 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0     9653 2024-04-15 05:26:06.890885 mms_client-1.3.0/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    14774 1970-01-01 00:00:00.000000 mms_client-1.3.0/PKG-INFO
```

### Comparing `mms_client-1.2.0/LICENSE` & `mms_client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/README.md` & `mms_client-1.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
 The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
+- MarketQuery_AwardResultsQuery
 - RegistrationSubmit_Resource
 - RegistrationQuery_Resource
 
 We can add support for additional endpoints as time goes on, and independent contribution is, of course, welcome. However, support for attachments is currently limited because none of the endpoints we support currently require them. We have implemented attachment support up to the client level, but we haven't developed an architecture for submitting them through an endpoint yet.
 
 # Installation
 We have a package on PyPI so installation is as easy as doing:
```

### Comparing `mms_client-1.2.0/pyproject.toml` & `mms_client-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.2.0"
+version = "v1.3.0"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mms_client-1.2.0/src/mms_client/client.py` & `mms_client-1.3.0/src/mms_client/client.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.3.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.3.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.3.0/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.3.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.3.0/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.3.0/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.3.0/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/security/certs.py` & `mms_client-1.3.0/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/security/crypto.py` & `mms_client-1.3.0/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/services/base.py` & `mms_client-1.3.0/src/mms_client/services/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/services/omi.py` & `mms_client-1.3.0/src/mms_client/services/omi.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/services/registration.py` & `mms_client-1.3.0/src/mms_client/services/registration.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         This endpoint is only accessible to BSPs.
 
         Arguments:
         request (ResourceData): The resource to register with the MMS server.
 
         Returns:    The resource that has been registered with the MMS server.
         """
+        # NOTE: The return type does not match the method definition but the decorator will return the correct type
         # For some reason, the registration DTOs require that the participant ID exist on the payload rather than on
         # the envelope so we need to set it before we return the envelope.
         request.participant = self.participant
 
         # Create and return the registration submit DTO.
         return RegistrationSubmit()  # type: ignore[return-value]
 
@@ -61,14 +62,15 @@
         request (ResourceQuery):    The query to send to the MMS server.
         action (QueryAction):       The type of query being made. NORMAL for all records or LATEST for the most recent.
         date (Date):                The date of the transaction in the format "YYYY-MM-DD". This value defaults to the
                                     current date.
 
         Returns:    A list of resources that match the query.
         """
+        # NOTE: The return type does not match the method definition but the decorator will return the correct type
         # For some reason, the registration DTOs require that the participant ID exist on the payload rather than on
         # the envelope so we need to set it before we return the envelope.
         request.participant = self.participant
 
         # Inject our parameters into the query and return it.
         return RegistrationQuery(  # type: ignore[return-value]
             action=action,
```

### Comparing `mms_client-1.2.0/src/mms_client/services/report.py` & `mms_client-1.3.0/src/mms_client/services/report.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/types/base.py` & `mms_client-1.3.0/src/mms_client/types/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/types/fields.py` & `mms_client-1.3.0/src/mms_client/types/fields.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,34 @@
         name=alias,
         min_length=8,
         max_length=10,
         pattern=r"^[a-zA-Z0-9]{8,10}$",
     )
 
 
+def offer_id(alias: str, optional: bool = False):
+    """Create a field for an offer ID.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the offer ID.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined,
+        name=alias,
+        min_length=1,
+        max_length=30,
+        pattern=r"^[a-zA-Z0-9_-]*$",
+    )
+
+
 def capacity(alias: str, minimum: int, optional: bool = False):
     """Create a field for a capacity value.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     minimum (int):      The minimum value for the capacity field.
@@ -94,26 +114,27 @@
                         required, with no default.
 
     Returns:    A Pydantic Field object for the power value.
     """
     return attr(default=None if optional else PydanticUndefined, name=alias, gt=0, le=10000000)
 
 
-def price(alias: str, optional: bool = False):
+def price(alias: str, limit: float, optional: bool = False):
     """Create a field for a price value.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
+    limit (int):        The maximum value for the price field.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
                         required, with no default.
 
     Returns:    A Pydantic Field object for the price value.
     """
-    return attr(default=None if optional else PydanticUndefined, name=alias, ge=0.00, lt=10000.00, decimal_places=2)
+    return attr(default=None if optional else PydanticUndefined, name=alias, ge=0.00, le=limit, decimal_places=2)
 
 
 def percentage(alias: str, optional: bool = False):
     """Create a field for a percentage value.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
@@ -136,14 +157,30 @@
                         required, with no default.
 
     Returns:    A Pydantic Field object for the DR pattern number.
     """
     return attr(default=None if optional else PydanticUndefined, name=alias, ge=1, le=20)
 
 
+def dr_pattern_name(alias: str, optional: bool = False):
+    """Create a field for a DR pattern name.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the DR pattern name.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined, name=alias, min_length=1, max_length=20, pattern=JAPANESE_TEXT
+    )
+
+
 def pattern_name(alias: str, optional: bool = False):
     """Create a field for a pattern name.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
@@ -242,14 +279,48 @@
     Returns:    A Pydantic Field object for the resource short name.
     """
     return attr(
         default=None if optional else PydanticUndefined, name=alias, min_length=1, max_length=10, pattern=JAPANESE_TEXT
     )
 
 
+def contract_id(alias: str, optional: bool = False):
+    """Create a field for a contract ID.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the contract ID.
+    """
+    return attr(
+        default=None if optional else PydanticUndefined,
+        name=alias,
+        min_length=19,
+        max_length=19,
+        pattern=r"^[a-zA-Z0-9]**$",
+    )
+
+
+def jbms_id(alias: str, optional: bool = False):
+    """Create a field for a JBMS ID.
+
+    Arguments:
+    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
+                        to the JSON/XML key.
+    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
+                        required, with no default.
+
+    Returns:    A Pydantic Field object for the JBMS ID.
+    """
+    return attr(default=None if optional else PydanticUndefined, name=alias, ge=1, lt=1000000000000000000)
+
+
 def system_code(alias: str, optional: bool = False):
     """Create a field for a system code.
 
     Arguments:
     alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
                         to the JSON/XML key.
     optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
```

### Comparing `mms_client-1.2.0/src/mms_client/types/market.py` & `mms_client-1.3.0/src/mms_client/types/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,33 +29,36 @@
     # the request. This value will be checked against the certificate used to make the request.
     participant: str = participant("ParticipantName")
 
     # The user name of the person making the request. This value is used to track the user who made the request, and
     # will be checked against the certificate used to make the request.
     user: str = attr(name="UserName", min_length=1, max_length=12, pattern=r"^[A-Z0-9]*$")
 
-    # The type of market for which the data is being submitted
-    market_type: Optional[MarketType] = attr(default=None, name="MarketType")
-
 
 class MarketQuery(BaseMarketRequest):
     """Represents the base fields for a market query."""
 
     # If the market type is specified as "DAM" (day-ahead market), the number of days should be specified as "1".
     # Otherwise, this field indicates the number of days ahead for which the data is being queried.
     days: int = attr(default=1, name="NumOfDays", ge=1, le=7)
 
 
 class MarketSubmit(BaseMarketRequest):
     """Represents the base fields for a market registration request."""
 
+    # The type of market for which the data is being submitted
+    market_type: Optional[MarketType] = attr(default=None, name="MarketType")
+
     # If the market type is specified as "DAM" (day-ahead market), the number of days should be specified as "1".
     # Otherwise, this field indicates the number of days ahead for which the data is being submitted.
     days: int = attr(default=1, name="NumOfDays", ge=1, le=31)
 
 
 class MarketCancel(BaseMarketRequest):
     """Represents the base fields for a market cancellation request."""
 
+    # The type of market for which the data is being submitted
+    market_type: MarketType = attr(name="MarketType")
+
     # If the market type is specified as "DAM" (day-ahead market), the number of days should be specified as "1".
     # Otherwise, this field indicates the number of days ahead for which the data is being cancelled.
     days: int = attr(default=1, name="NumOfDays", ge=1, le=31)
```

### Comparing `mms_client-1.2.0/src/mms_client/types/offer.py` & `mms_client-1.3.0/src/mms_client/types/offer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,33 @@
 """Contains objects for MMS offers."""
 
 from decimal import Decimal
-from enum import Enum
 from typing import List
 from typing import Optional
 
-from pydantic_core import PydanticUndefined
 from pydantic_extra_types.pendulum_dt import DateTime
 from pydantic_xml import attr
 from pydantic_xml import element
 
 from mms_client.types.base import Payload
 from mms_client.types.enums import AreaCode
+from mms_client.types.enums import Direction
 from mms_client.types.fields import company_short_name
 from mms_client.types.fields import dr_patter_number
+from mms_client.types.fields import offer_id
 from mms_client.types.fields import operator_code
 from mms_client.types.fields import participant
 from mms_client.types.fields import power_positive
 from mms_client.types.fields import price
 from mms_client.types.fields import resource_name
 from mms_client.types.fields import resource_short_name
 from mms_client.types.fields import system_code
 from mms_client.types.market import MarketType
 
 
-def offer_id(alias: str, optional: bool = False):
-    """Create a field for an offer ID.
-
-    Arguments:
-    alias (str):        The name of the alias to assign to the Pydanitc field. This value will be used to map the field
-                        to the JSON/XML key.
-    optional (bool):    If True, the field will be optional with a default of None. If False, the field will be
-                        required, with no default.
-
-    Returns:    A Pydantic Field object for the offer ID.
-    """
-    return attr(
-        default=None if optional else PydanticUndefined,
-        name=alias,
-        min_length=1,
-        max_length=30,
-        pattern=r"^[a-zA-Z0-9_-]*$",
-    )
-
-
-class Direction(Enum):
-    """Represents the reserve direction of the offer."""
-
-    SELL = "1"  # Increasing the reserves (sell)
-    # Note: Support for the BUY direction was removed from the MMS API
-    # BUY = "2"  # Decreasing the reserves (buy)
-
-
 class OfferStack(Payload):
     """Represents a single price-quantity pair in an offer request.
 
     Notes:
         For the Day-ahead Market, the tertiary 2 sell bidding volume is mandatory.
         For the Week-ahead Market, one of primary, secondary 1, secondary 2, or tertiary 1 sell bidding volumes are
         mandatory.
@@ -90,15 +62,15 @@
     # The first tertiary bid quantity in kW
     tertiary_1_qty_kw: Optional[int] = power_positive("Tertiary1OfferQuantityInKw", True)
 
     # The second tertiary bid quantity in kW.
     tertiary_2_qty_kw: Optional[int] = power_positive("Tertiary2OfferQuantityInKw", True)
 
     # The unit price of the power, in JPY/kW/segment
-    unit_price: Decimal = price("OfferUnitPrice")
+    unit_price: Decimal = price("OfferUnitPrice", 10000.00)
 
     # The ID of the offer to which this stack belongs
     id: Optional[str] = offer_id("OfferId", True)
 
 
 class OfferData(Payload):
     """Describes the data common to both offer requests and responses."""
```

### Comparing `mms_client-1.2.0/src/mms_client/types/registration.py` & `mms_client-1.3.0/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/types/resource.py` & `mms_client-1.3.0/src/mms_client/types/resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 from pydantic_core import PydanticUndefined
 from pydantic_xml import attr
 from pydantic_xml import element
 from pydantic_xml import wrapped
 
 from mms_client.types.base import Payload
 from mms_client.types.enums import AreaCode
+from mms_client.types.enums import BooleanFlag
+from mms_client.types.enums import CommandMonitorMethod
 from mms_client.types.enums import Frequency
+from mms_client.types.enums import ResourceType
 from mms_client.types.fields import ASCII_TEXT
 from mms_client.types.fields import JAPANESE_ASCII_TEXT
 from mms_client.types.fields import JAPANESE_TEXT
 from mms_client.types.fields import address
 from mms_client.types.fields import capacity
 from mms_client.types.fields import hour
 from mms_client.types.fields import minute
@@ -176,43 +179,23 @@
     MARKET_AND_POWER_SUPPLY_2 = "2"
     POWER_SUPPLY_2 = "3"
     ONLY_POWER_SUPPLY_1 = "4"
     MARKET_AND_REMAINING_RESERVE_UTILIZATION = "5"
     REMAINING_RESERVE_UTILIZATION = "6"
 
 
-class ResourceType(Enum):
-    """How the power generation unit produces electricity."""
-
-    THERMAL = "01"
-    HYDRO = "02"
-    PUMP = "03"
-    BATTERY = "04"
-    VPP_GEN = "05"
-    VPP_GEN_AND_DEM = "06"
-    VPP_DEM = "07"
-
-
 class RemainingReserveAvailability(Enum):
     """Describes the availability of remaining reserves for a power generation unit."""
 
     NOT_AVAILABLE = "0"
     AVAILABLE_FOR_UP_ONLY = "1"
     AVAILABLE_FOR_DOWN_ONLY = "2"
     AVAILABLE_FOR_UP_AND_DOWN = "3"
 
 
-class CommandMonitorMethod(Enum):
-    """Describes how the power generation unit is monitored and commanded."""
-
-    DEDICATED_LINE = "1"
-    SIMPLE_COMMAND = "2"
-    OFFLINE = "3"
-
-
 class SignalType(Enum):
     """Describes the type of signal used to monitor and command a power generation unit."""
 
     ACTUAL_OUTPUT_ORDER = "1"
     DIFFERENTIAL_OUTPUT_ORDER = "2"
 
 
@@ -227,25 +210,14 @@
     """Describes the type of thermal power generation unit."""
 
     GT = "1"
     GTCC = "2"
     OTHER = "9"
 
 
-class BooleanFlag(Enum):
-    """Describes a boolean flag.
-
-    This could literally be a Boolean value but it's coded in the reference as an enum and I don't want to create a
-    custom serializer for it.
-    """
-
-    YES = "1"
-    NO = "0"
-
-
 class OverrideOption(Enum):
     """Describes the override option for a power generation unit."""
 
     VIOLATION = "VIOLATION"
     OVERRIDE = "OVERRIDE"
 
 
@@ -757,15 +729,15 @@
     baseline_setting_method: Optional[BaseLineSettingMethod] = attr(default=None, name="BaselineSettingMethod")
 
     # The presence or absences of a POWER_SUPPLY_1 contract. Applies only if the area is Okinawa, in which case it is
     # mandatory. Otherwise, it should not be set.
     has_contract: Optional[BooleanFlag] = attr(default=None, name="ContractExistence")
 
     # The maximum bid price for POWER_SUPPLY_1 power, in JPY/kW/hr
-    declared_maximum_unit_price_kWh: Annotated[Decimal, price("DeclaredMaximumUnitPrice", True)]
+    declared_maximum_unit_price_kWh: Annotated[Decimal, price("DeclaredMaximumUnitPrice", 10000.00, True)]
 
     # Presence of voltage regulation function.
     voltage_adjustable: Optional[BooleanFlag] = attr(default=None, name="VoltageAdjustment")
 
     # Address of the resource. For power sources categorized under POWER_SUPPLY_1, this field is optional, while for
     # all other power sources, it is mandatory.
     address: Optional[str] = address("Address", True)
```

### Comparing `mms_client-1.2.0/src/mms_client/types/transport.py` & `mms_client-1.3.0/src/mms_client/types/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     REPORT = "mp.report"
     OMI = "mp.omi"
 
 
 class RequestDataType(Enum):
     """Represents the type of data to be sent to the MMS server.
 
-    Note that JSON is currently not supported and has been left in for future use.
+    NOTE: JSON is currently not supported and has been left in for future use.
     """
 
     JSON = "JSON"
     XML = "XML"
 
 
 class ResponseDataType(Enum):
     """Represents the type of data to be received from the MMS server.
 
-    Note that JSON is currently not supported and has been left in for future use.
+    NOTE: JSON is currently not supported and has been left in for future use.
     """
 
     XML = "XML"
     HTML = "HTML"
     CSV = "CSV"
     JSON = "JSON"
     TXT = "TXT"
```

### Comparing `mms_client-1.2.0/src/mms_client/utils/errors.py` & `mms_client-1.3.0/src/mms_client/utils/errors.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/src/mms_client/utils/serialization.py` & `mms_client-1.3.0/src/mms_client/utils/serialization.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import get_args
 from typing import get_origin
 
 from lxml.etree import XMLSchema
 from lxml.etree import _Element as Element
 from lxml.etree import parse
 from pydantic_xml import element
+from pydantic_xml.typedefs import EntityLocation
 
 from mms_client.types.base import E
 from mms_client.types.base import Messages
 from mms_client.types.base import MultiResponse
 from mms_client.types.base import P
 from mms_client.types.base import Payload
 from mms_client.types.base import PayloadBase
@@ -65,20 +66,20 @@
             self._payload_key,
             type(request_envelope),
             type(request_data),
             False,  # type: ignore[arg-type]
         )
 
         # Next, inject the payload and data into the payload class
-        # Note: this returns a type that inherits from PayloadBase and the arguments provided to the initializer
+        # NOTE: this returns a type that inherits from PayloadBase and the arguments provided to the initializer
         # here are correct, but mypy thinks they are incorrect because it doesn't understand the the inherited type
         payload = payload_cls(request_envelope, request_data, self._xsd.value)  # type: ignore[call-arg, misc]
 
         # Finally, convert the payload to XML and return it
-        # Note: we provided the encoding here so this will return bytes, not a string
+        # NOTE: we provided the encoding here so this will return bytes, not a string
         return payload.to_xml(skip_empty=True, encoding="utf-8", xml_declaration=True)  # type: ignore[return-value]
 
     def serialize_multi(self, request_envelope: E, request_data: List[P], request_type: Type[P]) -> bytes:
         """Serialize the envelope and data to a byte string for sending to the MMS server.
 
         Arguments:
         request_envelope (Envelope):    The envelope to be serialized.
@@ -89,20 +90,20 @@
         """
         # First, create our payload class from the payload and data types
         payload_cls = _create_request_payload_type(
             self._payload_key, type(request_envelope), request_type, True  # type: ignore[arg-type]
         )
 
         # Next, inject the payload and data into the payload class
-        # Note: this returns a type that inherits from PayloadBase and the arguments provided to the initializer
+        # NOTE: this returns a type that inherits from PayloadBase and the arguments provided to the initializer
         # here are correct, but mypy thinks they are incorrect because it doesn't understand the the inherited type
         payload = payload_cls(request_envelope, request_data, self._xsd.value)  # type: ignore[call-arg, misc]
 
         # Finally, convert the payload to XML and return it
-        # Note: we provided the encoding here so this will return bytes, not a string
+        # NOTE: we provided the encoding here so this will return bytes, not a string
         return payload.to_xml(skip_empty=True, encoding="utf-8", xml_declaration=True)  # type: ignore[return-value]
 
     def deserialize(self, data: bytes, envelope_type: Type[E], data_type: Type[P]) -> Response[E, P]:
         """Deserialize the data to a response object.
 
         Arguments:
         data (bytes):                   The raw data to be deserialized.
@@ -186,15 +187,15 @@
         resp = cls.from_xml_tree(raw)  # type: ignore[arg-type]
 
         # Next, attempt to extract the envelope from the response
         resp.envelope, resp.envelope_validation, env_node = self._from_tree_envelope(raw, envelope_type)
 
         # Now, verify that the response doesn't contain an unexpected data type and then retrieve the payload data
         # from within the envelope
-        # Note: apparently, mypy doesn't know about setter-getter properties either...
+        # NOTE: apparently, mypy doesn't know about setter-getter properties either...
         self._verify_tree_data_tag(env_node, data_type)
         resp.payload = [
             self._from_tree_data(item, data_type) for item in env_node.findall(get_tag(data_type))  # type: ignore[misc]
         ]
 
         # Finally, attempt to extract the messages from within the payload
         resp.messages = self._from_tree_messages(raw, envelope_type, data_type, self._payload_key, True)
@@ -267,15 +268,21 @@
         # Finally, parse and return the data and validation information
         return ResponseData[P](
             data_type.from_xml_tree(raw),  # type: ignore[arg-type]
             common_cls.from_xml_tree(raw),  # type: ignore[arg-type]
         )
 
     def _from_tree_messages(
-        self, raw: Element, envelope_type: Type[E], current_type: Type[P], root: str, multi: bool
+        self,
+        raw: Element,
+        envelope_type: Type[E],
+        current_type: Type[P],
+        root: str,
+        multi: bool,
+        wrapped: bool = False,
     ) -> Dict[str, Messages]:
         """Attempt to extract the messages from within the payload.
 
         Note that this method is called recursively to handle nested payloads and data types. It does not iterate over
         the XML tree to determine the structure of the response; instead, it uses the type annotations to determine the
         structure of the response.
 
@@ -283,14 +290,15 @@
         raw (Element):                  The raw data to be converted.
         envelope_type (Type[Envelope]): The type of envelope being constructed.
         current_type (Type[Payload]):   The type of data being constructed.
         root (str):                     The root of the dictionary, used to create the key for the messages.
         multi (bool):                   Whether we're processing a list of nodes or a single node. If called with the
                                         payload root, this value will determine whether we're processing a multi-
                                         response or a single response.
+        wrapped (bool):                 Whether or not this type is referenced from a wrapped field.
         """
         # First, find the Messages node in the raw data
         message_node = raw.find("Messages")
 
         # Next, create our dictionary of messages and attempt to extract the messages from the raw data at the current
         # level of the response and set it to the root key
         messages = {}
@@ -305,67 +313,76 @@
             messages.update(
                 self._from_tree_messages(
                     _find_or_fail(raw, envelope_type.__name__),
                     envelope_type,
                     current_type,
                     f"{root}.{envelope_type.__name__}",
                     multi,
+                    False,
                 )
             )
-        elif root.endswith(envelope_type.__name__):
+        elif root.endswith(envelope_type.__name__) or wrapped:
             messages.update(
-                self._from_tree_messages_inner(raw, envelope_type, current_type, root, current_type.__name__, multi)
+                self._from_tree_messages_inner(
+                    raw, envelope_type, current_type, root, get_tag(current_type), multi, False
+                )
             )
         else:
             # Iterate over each field on the current type...
             for field in current_type.model_fields.values():
 
-                # First, get the arguments and origin of the field's annotation
-                args = get_args(field.annotation)
-                origin = get_origin(field.annotation)
-                has_args = len(args) > 0
+                # First, get the arguments and origin of the field's annotation. Occaisionally, we'll have an optional
+                # list. In this case, we'll have to do get_args twice to traverse the type tree.
+                arg, multi = _get_field_typing(field.annotation)  # type: ignore[arg-type]
 
                 # Next, check if the annotation is a subclass of Payload or else if it's a collection of Payload. If
                 # neither of these is the case, we can skip this field.
-                # Note: all our fields are annotated so there's no need to check if they're not
-                if not (
-                    (has_args and issubclass(args[0], Payload))
-                    or (not has_args and issubclass(field.annotation, Payload))  # type: ignore[arg-type]
-                ):
+                # NOTE: All our fields are annotated so there's no need to check if they're not
+                if not issubclass(arg, Payload):
                     continue
 
                 # Finally, call this method recursively for the field and update the messages with the results
-                # Note: All our fields are annotated as XmlEntityInfo, so they have the "path" attribute
+                # NOTE: All our fields are annotated as XmlEntityInfo, so they have the "path" and "location" attributes
+                print(field)
                 messages.update(
                     self._from_tree_messages_inner(
                         raw,
                         envelope_type,
-                        args[0],
+                        arg,
                         root,
                         field.path,  # type: ignore[attr-defined]
-                        origin is list,
+                        multi,
+                        field.location == EntityLocation.WRAPPED,  # type: ignore[attr-defined]
                     )
                 )
 
         # Finally, return our dictionary of messages
         return messages
 
     def _from_tree_messages_inner(
-        self, raw: Element, envelope_type: Type[E], current_type: Type[P], root: str, tag: str, multi: bool
+        self,
+        raw: Element,
+        envelope_type: Type[E],
+        current_type: Type[P],
+        root: str,
+        tag: str,
+        multi: bool,
+        wrapped: bool,
     ) -> Dict[str, Messages]:
         """Attempt to extract the messages from within the payload at the current level.
 
         Arguments:
         raw (Element):                  The raw data to be converted.
         envelope_type (Type[Envelope]): The type of envelope being constructed.
         current_type (Type[Payload]):   The type of data being constructed.
         root (str):                     The root of the dictionary, used to create the key for the messages.
         tag (str):                      The tag of the current node being processed.
         multi (bool):                   If True, the payload will be a multi-response; otherwise, it will be a single
                                         response.
+        wrapped (bool):                 Whether or not this field is a wrapped field.
 
         Returns:    A dictionary mapping messages to where they were found in the response.
         """
         # Construct the new root from the existing root and the tag
         path_base = f"{root}.{tag}"
 
         # If we are processing a list, we need to iterate over each node and call this method recursively. Otherwise,
@@ -375,20 +392,28 @@
             nodes = raw.findall(tag)
             if not nodes:
                 return {}
 
             # Otherwise, we'll call this method recursively for each node and update the messages with the results.
             messages = {}
             for i, node in enumerate(nodes):
-                messages.update(self._from_tree_messages(node, envelope_type, current_type, f"{path_base}[{i}]", True))
+                messages.update(
+                    self._from_tree_messages(
+                        node, envelope_type, current_type, path_base if wrapped else f"{path_base}[{i}]", True, wrapped
+                    )
+                )
             return messages
 
         # If we reached this point then we are processing a single item so find the associated
         child = raw.find(tag)
-        return {} if child is None else self._from_tree_messages(child, envelope_type, current_type, path_base, False)
+        return (
+            {}
+            if child is None
+            else self._from_tree_messages(child, envelope_type, current_type, path_base, False, wrapped)
+        )
 
     def _from_xml(self, data: bytes) -> Element:
         """Parse the XML file, returning the resulting XML tree.
 
         Arguments:
         data:       The raw XML data to be parsed.
 
@@ -543,14 +568,53 @@
     """
     found = node.find(tag)
     if found is None:
         raise ValueError(f"Expected tag '{tag}' not found in node")  # pragma: no cover
     return found
 
 
+def _get_field_typing(typ: Type) -> Tuple[Type, bool]:
+    """Retrieve the field's actual type and whether or not the field is a collection.
+
+    This method is designed to find the inner type of fields in the following cases:
+    1. Fundamental types and classes (e.g. int, str, Award, Offer, etc.)
+    2. Nullable fundamental types and classes
+    3. Collections of fundamental types and classes
+    4. Nullable collections of fundamental types and classes
+
+    Arguments:
+    typ (Type): The type of the field to retrieve the inner type for.
+
+    Returns:
+    Type:   The inner type of the field.
+    bool:   Whether or not the field is a collection.
+    """
+    # First, check for the case where we have a fundamental type. If we do then we can return the type and False.
+    init = get_args(typ)
+    if len(init) == 0:
+        return typ, False
+
+    # Next, iterate over the type hierarchy and repeat the operation until we find the leaf type.
+    args = [get_args(typ)]
+    while len(args[-1]) > 1:
+        temp = get_args(args[-1][0])
+        if len(temp) == 0:
+            break
+        args.append(temp)
+
+    # Now, find the origin type of the field. This will be the lowest type in the hierarchy that isn't a multi-type.
+    # If there aren't any of these, then we'll just use the original type.
+    origin_type = next(
+        filter(lambda x: x is not None, map(lambda arg: arg[0] if len(arg) > 1 else None, reversed(args))), typ
+    )
+
+    # Finally, return the inner type and whether or not the origin type is a list
+    return args[-1][0] if len(args) > 0 else typ, get_origin(origin_type) is list  # typing: ignore[return-value]
+
+
 def get_tag(data_type: Type[P]) -> str:
     """Get the tag for the given data type.
 
     Arguments:
     data_type (Type[Payload]):  The data type to get the tag for.
 
     Returns:    The tag for the given data type.
```

### Comparing `mms_client-1.2.0/src/mms_client/utils/web.py` & `mms_client-1.3.0/src/mms_client/utils/web.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.2.0/PKG-INFO` & `mms_client-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -194,14 +194,15 @@
 The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
 
 # Completeness
 This client is not complete. Currently, it supports the following endpoints:
 - MarketSubmit_OfferData
 - MarketQuery_OfferQuery
 - MarketCancel_OfferCancel
+- MarketQuery_AwardResultsQuery
 - RegistrationSubmit_Resource
 - RegistrationQuery_Resource
 
 We can add support for additional endpoints as time goes on, and independent contribution is, of course, welcome. However, support for attachments is currently limited because none of the endpoints we support currently require them. We have implemented attachment support up to the client level, but we haven't developed an architecture for submitting them through an endpoint yet.
 
 # Installation
 We have a package on PyPI so installation is as easy as doing:
```

