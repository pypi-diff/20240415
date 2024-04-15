# Comparing `tmp/simple-salesforce-1.12.5.tar.gz` & `tmp/simple-salesforce-1.12.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simple-salesforce-1.12.5.tar", last modified: Wed Sep  6 15:13:27 2023, max compression
+gzip compressed data, was "dist\simple-salesforce-1.12.6.tar", last modified: Mon Apr 15 16:19:31 2024, max compression
```

## Comparing `simple-salesforce-1.12.5.tar` & `simple-salesforce-1.12.6.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)    28259 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       67 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1864 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       65 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    29388 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)       18 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1676 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    29388 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-09-06 15:13:27.000000 simple-salesforce-1.12.5/simple_salesforce/
--rw-rw-r--   0 travis    (2000) travis    (2000)   911649 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/metadata.wsdl
--rw-rw-r--   0 travis    (2000) travis    (2000)     2566 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/format.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    42038 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3308 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/messages.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3664 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      514 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/__version__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2684 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34097 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/bulk2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18038 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/bulk.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10779 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/login.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23350 2023-09-06 15:10:37.000000 simple-salesforce-1.12.5/simple_salesforce/metadata.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:19:31.935697 simple-salesforce-1.12.6/
+-rw-rw-rw-   0        0        0     1676 2024-04-15 15:16:46.000000 simple-salesforce-1.12.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       99 2024-04-15 15:16:46.000000 simple-salesforce-1.12.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    36734 2024-04-15 16:19:31.936697 simple-salesforce-1.12.6/PKG-INFO
+-rw-rw-rw-   0        0        0    28276 2024-04-15 15:16:46.000000 simple-salesforce-1.12.6/README.rst
+-rw-rw-rw-   0        0        0      629 2024-04-15 16:19:31.937698 simple-salesforce-1.12.6/setup.cfg
+-rw-rw-rw-   0        0        0     1864 2024-04-15 15:16:46.000000 simple-salesforce-1.12.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:19:31.922694 simple-salesforce-1.12.6/simple_salesforce/
+-rw-rw-rw-   0        0        0      538 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/__init__.py
+-rw-rw-rw-   0        0        0      514 2024-04-15 16:17:25.000000 simple-salesforce-1.12.6/simple_salesforce/__version__.py
+-rw-rw-rw-   0        0        0    52593 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/api.py
+-rw-rw-rw-   0        0        0    26040 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/bulk.py
+-rw-rw-rw-   0        0        0    44504 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/bulk2.py
+-rw-rw-rw-   0        0        0     3884 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/exceptions.py
+-rw-rw-rw-   0        0        0     2677 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/format.py
+-rw-rw-rw-   0        0        0    12407 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/login.py
+-rw-rw-rw-   0        0        0     3308 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/messages.py
+-rw-rw-rw-   0        0        0    25690 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/metadata.py
+-rw-rw-rw-   0        0        0   911649 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/metadata.wsdl
+-rw-rw-rw-   0        0        0        0 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/py.typed
+-rw-rw-rw-   0        0        0     3538 2024-04-15 15:16:47.000000 simple-salesforce-1.12.6/simple_salesforce/util.py
+drwxrwxrwx   0        0        0        0 2024-04-15 16:19:31.934697 simple-salesforce-1.12.6/simple_salesforce.egg-info/
+-rw-rw-rw-   0        0        0    36734 2024-04-15 16:19:31.000000 simple-salesforce-1.12.6/simple_salesforce.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2024-04-15 16:19:31.000000 simple-salesforce-1.12.6/simple_salesforce.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 16:19:31.000000 simple-salesforce-1.12.6/simple_salesforce.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-15 15:27:58.000000 simple-salesforce-1.12.6/simple_salesforce.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       69 2024-04-15 16:19:31.000000 simple-salesforce-1.12.6/simple_salesforce.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 16:19:31.000000 simple-salesforce-1.12.6/simple_salesforce.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `simple-salesforce-1.12.5/README.rst` & `simple-salesforce-1.12.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 .. image:: https://app.travis-ci.com/simple-salesforce/simple-salesforce.svg?branch=master
    :target: https://travis-ci.org/simple-salesforce/simple-salesforce
 
 .. image:: https://readthedocs.org/projects/simple-salesforce/badge/?version=latest
    :target: http://simple-salesforce.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
-Simple Salesforce is a basic Salesforce.com REST API client built for Python 3.6, 3.7 3.8, 3.9, 3.10, and 3.11. The goal is to provide a very low-level interface to the REST Resource and APEX API, returning a dictionary of the API JSON response.
+Simple Salesforce is a basic Salesforce.com REST API client built for Python 3.8, 3.9, 3.10, 3.11, and 3.12. The goal is to provide a very low-level interface to the REST Resource and APEX API, returning a dictionary of the API JSON response.
 You can find out more regarding the format of the results in the `Official Salesforce.com REST API Documentation`_
 
 .. _Official Salesforce.com REST API Documentation: http://www.salesforce.com/us/developer/docs/api_rest/index.htm
 
 
 
 =============
@@ -766,15 +766,15 @@
    import pandas as pd
 
    def sf_api_query(data):
     df = pd.DataFrame(data['records']).drop('attributes', axis=1)
     listColumns = list(df.columns)
     for col in listColumns:
         if any (isinstance (df[col].values[i], dict) for i in range(0, len(df[col].values))):
-            df = pd.concat([df.drop(columns=[col]),df[col].apply(pd.Series).drop('attributes',axis=1).add_prefix(col+'.')],axis=1)
+            df = pd.concat([df.drop(columns=[col]),df[col].apply(pd.Series,dtype=df[col].dtype).drop('attributes',axis=1).add_prefix(col+'.')],axis=1)
             new_columns = np.setdiff1d(df.columns, listColumns)
             for i in new_columns:
                 listColumns.append(i)
     return df
 
    df = sf_api_query(sf.query("SELECT Id, Email,ParentAccount.Name FROM Contact"))
```

### Comparing `simple-salesforce-1.12.5/setup.py` & `simple-salesforce-1.12.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,27 @@
     packages=['simple_salesforce', ],
     url=about['__url__'],
     license=about['__license__'],
     description=about['__description__'],
     long_description=textwrap.dedent((here / 'README.rst').read_text()),
     long_description_content_type='text/x-rst',
     package_data={
-        'simple_salesforce': ['metadata.wsdl'],
+        'simple_salesforce': ['metadata.wsdl', 'py.typed'],
         },
     install_requires = [
        'requests>=2.22.0',
-       'cryptography',
+       'typing-extensions',
        'zeep',
-       'pyjwt',
-       'more-itertools',
-       'pendulum'
+       'pyjwt[crypto]',
+       'more-itertools'
        ],
     tests_require=[
         'pytest',
         'pytz>=2014.1.1',
         'responses>=0.5.1',
-        'cryptography<3.4',
         ],
     test_suite='simple_salesforce.tests',
     keywords=about['__keywords__'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Intended Audience :: Developers',
@@ -52,9 +50,10 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: PyPy'
-        ]
-)
+        ],
+    zip_safe=False,
+)
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce.egg-info/SOURCES.txt` & `simple-salesforce-1.12.6/simple_salesforce.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,13 +10,15 @@
 simple_salesforce/bulk2.py
 simple_salesforce/exceptions.py
 simple_salesforce/format.py
 simple_salesforce/login.py
 simple_salesforce/messages.py
 simple_salesforce/metadata.py
 simple_salesforce/metadata.wsdl
+simple_salesforce/py.typed
 simple_salesforce/util.py
 simple_salesforce.egg-info/PKG-INFO
 simple_salesforce.egg-info/SOURCES.txt
 simple_salesforce.egg-info/dependency_links.txt
+simple_salesforce.egg-info/not-zip-safe
 simple_salesforce.egg-info/requires.txt
 simple_salesforce.egg-info/top_level.txt
```

### Comparing `simple-salesforce-1.12.5/LICENSE.txt` & `simple-salesforce-1.12.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.5/simple_salesforce/metadata.wsdl` & `simple-salesforce-1.12.6/simple_salesforce/metadata.wsdl`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.5/simple_salesforce/format.py` & `simple-salesforce-1.12.6/simple_salesforce/format.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Formatting helpers that perform quoting and escaping """
-
 import urllib.parse
 from datetime import date, datetime, timezone
 from string import Formatter
+from typing import Any, Union
 
 # https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql_select_quotedstringescapes.htm
 soql_escapes = str.maketrans({
     '\\': '\\\\',
     '\'': '\\\'',
     '"': '\\"',
     '\n': '\\n',
@@ -21,36 +21,36 @@
     '_': '\\_',
 })
 
 
 class SoqlFormatter(Formatter):
     """ Custom formatter to apply quoting or the :literal format spec """
 
-    def format_field(self, value, format_spec):
+    def format_field(self, value: Any, format_spec: str) -> Any:
         if not format_spec:
             return quote_soql_value(value)
         if format_spec == 'literal':
             # literal: allows circumventing everything while still using
             # the same format string
             return value
         if format_spec == 'like':
             # like: allows escaping substring used in LIKE expression
             # does not quote
             return (str(value).translate(soql_escapes)
                     .translate(soql_like_escapes))
         return super().format_field(value, format_spec)
 
 
-def format_soql(query, *args, **kwargs):
+def format_soql(query: str, *args: Any, **kwargs: Any) -> str:
     """ Insert values quoted for SOQL into a format string """
     return SoqlFormatter().vformat(query, args, kwargs)
 
 
 # pylint: disable=too-many-return-statements
-def quote_soql_value(value):
+def quote_soql_value(value: Any) -> str:
     """ Quote/escape either an individual value or a list of values
     for a SOQL value expression """
     if isinstance(value, str):
         return "'" + value.translate(soql_escapes) + "'"
     if value is True:
         return 'true'
     if value is False:
@@ -69,10 +69,10 @@
         value = value.astimezone(tz=timezone.utc)
         return value.isoformat()
     if isinstance(value, date):
         return value.isoformat()
     raise ValueError('unquotable value type')
 
 
-def format_external_id(field, value):
+def format_external_id(field: str, value: Union[str, bytes]) -> str:
     """ Create an external ID string for use with get() or upsert() """
     return field + '/' + urllib.parse.quote(value, safe='')
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce/__init__.py` & `simple-salesforce-1.12.6/simple_salesforce/__init__.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.5/simple_salesforce/messages.py` & `simple-salesforce-1.12.6/simple_salesforce/messages.py`

 * *Files identical despite different names*

### Comparing `simple-salesforce-1.12.5/simple_salesforce/exceptions.py` & `simple-salesforce-1.12.6/simple_salesforce/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """All exceptions for Simple Salesforce"""
+from typing import Union
 
 
 class SalesforceError(Exception):
     """Base Salesforce API exception"""
 
-    message = 'Unknown error occurred for {url}. Response content: {content}'
+    message: str = \
+        'Unknown error occurred for {url}. Response content: {content}'
 
-    def __init__(self, url, status, resource_name, content):
+    def __init__(
+            self,
+            url: str,
+            status: int,
+            resource_name: str,
+            content: bytes):
         """Initialize the SalesforceError exception
 
         SalesforceError is the base class of exceptions in simple-salesforce
 
         Args:
             url: Salesforce URL that was called
             status: Status code of the error response
@@ -21,18 +28,18 @@
         # this should be fixed.
         # pylint: disable=super-init-not-called
         self.url = url
         self.status = status
         self.resource_name = resource_name
         self.content = content
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.message.format(url=self.url, content=self.content)
 
-    def __unicode__(self):
+    def __unicode__(self) -> str:
         return self.__str__()
 
 
 class SalesforceMoreThanOneRecord(SalesforceError):
     """
     Error Code: 300
     The value returned when an external ID exists in more than one record. The
@@ -77,43 +84,47 @@
     Error Code: 404
     The requested resource couldn't be found. Check the URI for errors, and
     verify that there are no sharing issues.
     """
 
     message = 'Resource {name} Not Found. Response content: {content}'
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.message.format(name=self.resource_name,
                                    content=self.content)
 
 
 class SalesforceAuthenticationFailed(SalesforceError):
     """
     Thrown to indicate that authentication with Salesforce failed.
     """
 
-    def __init__(self, code, message):
+    def __init__(
+        self,
+        code: Union[str, int, None],
+        message: str
+        ):
         # TODO exceptions don't seem to be using parent constructors at all.
         # this should be fixed.
         # pylint: disable=super-init-not-called
         self.code = code
         self.message = message
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f'{self.code}: {self.message}'
 
 
 class SalesforceGeneralError(SalesforceError):
     """
     A non-specific Salesforce error.
     """
 
     message = 'Error Code {status}. Response content: {content}'
 
-    def __str__(self):
+    def __str__(self) -> str:
         return self.message.format(status=self.status, content=self.content)
 
 
 class SalesforceOperationError(Exception):
     """Base error for Bulk API 2.0 operations"""
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce/__version__.py` & `simple-salesforce-1.12.6/simple_salesforce/__version__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Version details for simple-salesforce
 
 This file shamelessly taken from the requests library"""
 
 __title__ = 'simple-salesforce'
 __description__ = 'A basic Salesforce.com REST API client.'
 __url__ = 'https://github.com/simple-salesforce/simple-salesforce'
-__version__ = '1.12.5'
+__version__ = '1.12.6'
 __author__ = 'Nick Catalano'
 __author_email__ = 'nickcatal@gmail.com'
 __license__ = 'Apache 2.0'
 __maintainer__ = 'Jonathan Wobken'
 __maintainer_email__ = 'jonathanwobken@gmail.com'
 __keywords__ = 'python salesforce salesforce.com'
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce/util.py` & `simple-salesforce-1.12.6/simple_salesforce/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,44 @@
 """Utility functions for simple-salesforce"""
 
+import datetime
 import xml.dom.minidom
+from typing import Any, Iterable, List, Mapping, MutableMapping, NamedTuple, \
+    NoReturn, \
+    Optional, \
+    TypeVar, Union
+
+import requests
 
 from .exceptions import (SalesforceExpiredSession, SalesforceGeneralError,
                          SalesforceMalformedRequest,
                          SalesforceMoreThanOneRecord, SalesforceRefusedRequest,
                          SalesforceResourceNotFound)
 
+Headers = MutableMapping[str, str]
+Proxies = MutableMapping[str, str]
+BulkDataAny = List[Mapping[str, Any]]
+BulkDataStr = List[Mapping[str, str]]
+T = TypeVar('T')
+
+class Usage(NamedTuple):
+    """Usage information for a Salesforce org"""
+    used: int
+    total: int
+
+class PerAppUsage(NamedTuple):
+    """Per App Usage information for a Salesforce org"""
+    used: int
+    total: int
+    name: str
 
 # pylint: disable=invalid-name
-def getUniqueElementValueFromXmlString(xmlString, elementName):
+def getUniqueElementValueFromXmlString(
+        xmlString: Union[str, bytes],
+        elementName: str) -> Optional[str]:
     """
     Extracts an element value from an XML string.
 
     For example, invoking
     getUniqueElementValueFromXmlString(
         '<?xml version="1.0" encoding="UTF-8"?><foo>bar</foo>', 'foo')
     should return the value 'bar'.
@@ -27,26 +52,28 @@
             .toxml()
             .replace('<' + elementName + '>', '')
             .replace('</' + elementName + '>', '')
         )
     return elementValue
 
 
-def date_to_iso8601(date):
+def date_to_iso8601(date: datetime.date) -> str:
     """Returns an ISO8601 string from a date"""
     datetimestr = date.strftime('%Y-%m-%dT%H:%M:%S')
     timezonestr = date.strftime('%z')
     return (
         f'{datetimestr}{timezonestr[0:3]}:{timezonestr[3:5]}'
         .replace(':', '%3A')
         .replace('+', '%2B')
     )
 
 
-def exception_handler(result, name=""):
+def exception_handler(
+        result: requests.Response,
+        name: str = "") -> NoReturn:
     """Exception router. Determines which error to raise for bad results"""
     try:
         response_content = result.json()
     # pylint: disable=broad-except
     except Exception:
         response_content = result.text
 
@@ -58,28 +85,35 @@
         404: SalesforceResourceNotFound,
     }
     exc_cls = exc_map.get(result.status_code, SalesforceGeneralError)
 
     raise exc_cls(result.url, result.status_code, name, response_content)
 
 
-def call_salesforce(url, method, session, headers, **kwargs):
+def call_salesforce(
+        url: str,
+        method: str,
+        session: requests.Session,
+        headers: Headers,
+        **kwargs: Any) -> requests.Response:
     """Utility method for performing HTTP call to Salesforce.
 
     Returns a `requests.result` object.
     """
 
     additional_headers = kwargs.pop('additional_headers', {})
     headers.update(additional_headers or {})
     result = session.request(method, url, headers=headers, **kwargs)
 
     if result.status_code >= 300:
         exception_handler(result)
 
     return result
 
-def list_from_generator(generator_function):
+def list_from_generator(
+        generator_function: Iterable[Iterable[T]]
+) -> List[T]:
     """Utility method for constructing a list from a generator function"""
-    ret_val = []
+    ret_val: List[T] = []
     for list_results in generator_function:
         ret_val.extend(list_results)
     return ret_val
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce/bulk2.py` & `simple-salesforce-1.12.6/simple_salesforce/bulk2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 """ Classes for interacting with Salesforce Bulk 2.0 API """
 
 import copy
 import csv
+import datetime
 import http.client as http
 import io
 import json
+import math
 import os
 import re
 import sys
 import tempfile
 from collections import OrderedDict
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import closing
 from enum import Enum
 from functools import partial
 from time import sleep
-from typing import Dict, Tuple, Union, Generator, List
+from typing import Any, AnyStr, Dict, Generator, List, MutableMapping, \
+    Optional, Tuple, Union
+from typing_extensions import Literal, NotRequired, TypedDict
 
-import math
-import pendulum
 import requests
 from more_itertools import chunked
-from pendulum import DateTime
+from requests import Session
 
 from .exceptions import (
     SalesforceBulkV2ExtractError,
     SalesforceBulkV2LoadError,
     SalesforceOperationError,
     )
 from .util import call_salesforce
 
 
 # pylint: disable=missing-class-docstring,invalid-name,too-many-arguments,
 # too-many-locals
 
 
-class Operation(str, Enum):
+class Operation(str,
+                Enum
+                ):
     insert = "insert"
     upsert = "upsert"
     update = "update"
     delete = "delete"
     hard_delete = "hardDelete"
     query = "query"
     query_all = "queryAll"
 
 
-class JobState(str, Enum):
+class JobState(str,
+               Enum
+               ):
     open = "Open"
     aborted = "Aborted"
     failed = "Failed"
     upload_complete = "UploadComplete"
     in_progress = "InProgress"
     job_complete = "JobComplete"
 
 
-class ColumnDelimiter(str, Enum):
+class ColumnDelimiter(str,
+                      Enum
+                      ):
     BACKQUOTE = "BACKQUOTE"  # (`)
     CARET = "CARET"  # (^)
     COMMA = "COMMA"  # (,)
     PIPE = "PIPE"  # (|)
     SEMICOLON = "SEMICOLON"  # (;)
     TAB = "TAB"  # (\t)
 
@@ -69,133 +77,192 @@
     ColumnDelimiter.COMMA: ",",
     ColumnDelimiter.PIPE: "|",
     ColumnDelimiter.SEMICOLON: ";",
     ColumnDelimiter.TAB: "\t",
     }
 
 
-class LineEnding(str, Enum):
+class LineEnding(str,
+                 Enum
+                 ):
     LF = "LF"
     CRLF = "CRLF"
 
 
-_line_ending_char = {LineEnding.LF: "\n", LineEnding.CRLF: "\r\n"}
+_line_ending_char = {
+    LineEnding.LF: "\n",
+    LineEnding.CRLF: "\r\n"
+    }
 
 
-class ResultsType(str, Enum):
+class ResultsType(str,
+                  Enum
+                  ):
     failed = "failedResults"
     successful = "successfulResults"
     unprocessed = "unprocessedRecords"
 
 
+class QueryParameters(TypedDict,
+                      total=False
+                      ):
+    maxRecords: int
+    locator: str
+
+
+class QueryResult(TypedDict,
+                  total=False
+                  ):
+    locator: str
+    number_of_records: int
+    records: NotRequired[str]
+    file: NotRequired[str]
+
+
 # https://developer.salesforce.com/docs/atlas.en-us.242.0
 # .salesforce_app_limits_cheatsheet.meta/salesforce_app_limits_cheatsheet
 # /salesforce_app_limits_platform_bulkapi.htm
 # https://developer.salesforce.com/docs/atlas.en-us.api_asynch.meta
 # /api_asynch/datafiles_prepare_csv.htm
 MAX_INGEST_JOB_FILE_SIZE = 100 * 1024 * 1024
 MAX_INGEST_JOB_PARALLELISM = 10  # TODO: ? Salesforce limits
 DEFAULT_QUERY_PAGE_SIZE = 50000
 
 
-def _split_csv(filename=None, records=None, max_records: int = None):
+def _split_csv(
+        filename: Optional[str] = None,
+        records: Optional[str] = None,
+        max_records: Optional[int] = None
+        ) -> Generator[Tuple[int, str], None, None]:
     """Split a CSV file into chunks to avoid exceeding the Salesforce
     bulk 2.0 API limits.
 
     Arguments:
         * filename -- csv file
         * max_records -- the number of records per chunk, None for auto size
     """
-    total_records = _count_csv(filename=filename, skip_header=True) if \
+    total_records = _count_csv(filename=filename,
+                               skip_header=True
+                               ) if \
         filename else \
-        _count_csv(data=records, skip_header=True)
+        _count_csv(data=records,
+                   skip_header=True
+                   )
     csv_data_size = os.path.getsize(filename) if filename else sys.getsizeof(
-        records)
-    max_records = max_records or total_records
-    max_records = min(max_records, total_records)
+        records
+        )
+    _max_records: int = max_records or total_records
+    _max_records = min(_max_records,
+                       total_records
+                       )
     max_bytes = min(
-        csv_data_size, MAX_INGEST_JOB_FILE_SIZE - 1 * 1024 * 1024
+        csv_data_size,
+        MAX_INGEST_JOB_FILE_SIZE - 1 * 1024 * 1024
         )  # -1 MB for sentinel
     records_size = 0
     bytes_size = 0
-    buff = []
+    buff: List[str] = []
     if filename:
-        with open(filename, encoding="utf-8") as bis:
+        with open(filename,
+                  encoding="utf-8"
+                  ) as bis:
             header = bis.readline()
             for line in bis:
                 records_size += 1
                 bytes_size += len(line.encode("utf-8"))
-                if records_size > max_records or bytes_size > max_bytes:
+                if records_size > _max_records or bytes_size > max_bytes:
                     if buff:
                         yield records_size - 1, header + "".join(buff)
                     buff = [line]
                     records_size = 1
                     bytes_size = len(line.encode("utf-8"))
                 else:
                     buff.append(line)
             if buff:
                 yield records_size, header + "".join(buff)
     else:
+        assert records is not None
         header = records.splitlines(True)[0]
         for line in records.splitlines(True)[1:]:
             records_size += 1
             bytes_size += len(line.encode("utf-8"))
-            if records_size > max_records or bytes_size > max_bytes:
+            if records_size > _max_records or bytes_size > max_bytes:
                 if buff:
                     yield records_size - 1, header + "".join(buff)
                 buff = [line]
                 records_size = 1
                 bytes_size = len(line.encode("utf-8"))
             else:
                 buff.append(line)
         if buff:
             yield records_size, header + "".join(buff)
 
 
 def _count_csv(
-        filename=None, data=None, skip_header=False, line_ending=LineEnding.LF
-        ):
+        filename: Optional[str] = None,
+        data: Optional[str] = None,
+        skip_header: bool = False,
+        line_ending: LineEnding = LineEnding.LF
+        ) -> int:
     """Count the number of records in a CSV file."""
     if filename:
-        with open(filename, encoding="utf-8") as bis:
+        with open(filename,
+                  encoding="utf-8"
+                  ) as bis:
             count = sum(1 for _ in bis)
     elif data:
         pat = repr(_line_ending_char[line_ending])[1:-1]
-        count = sum(1 for _ in re.finditer(pat, data))
+        count = sum(1 for _ in re.finditer(pat,
+                                           data
+                                           )
+                    )
     else:
         raise ValueError("Either filename or data must be provided")
 
     if skip_header:
         count -= 1
     return count
 
 
-def _convert_dict_to_csv(data, column_delimiter=',', line_ending=LineEnding.LF):
+def _convert_dict_to_csv(
+        data: Optional[List[Dict[str, str]]],
+        column_delimiter: Union[ColumnDelimiter, str] = ColumnDelimiter.COMMA,
+        line_ending: Union[LineEnding, str] = LineEnding.LF
+        ) -> Optional[str]:
     """Converts list of dicts to CSV like object."""
-    if data:
-        keys = set(i for s in [d.keys() for d in data] for i in s)
-        dict_to_csv_file = io.StringIO()
-        writer = csv.DictWriter(dict_to_csv_file, fieldnames=keys,
-                                delimiter=column_delimiter,
-                                lineterminator=line_ending)
-        writer.writeheader()
-        for row in data:
-            writer.writerow(row)
-    return dict_to_csv_file.getvalue() if data else None
+    if not data:
+        return None
+    keys = set(i for s in [d.keys() for d in data] for i in s)
+    dict_to_csv_file = io.StringIO()
+    writer = csv.DictWriter(dict_to_csv_file,
+                            fieldnames=keys,
+                            delimiter=column_delimiter,
+                            lineterminator=line_ending
+                            )
+    writer.writeheader()
+    for row in data:
+        writer.writerow(row)
+    return dict_to_csv_file.getvalue()
 
 
 class SFBulk2Handler:
     """Bulk 2.0 API request handler
     Intermediate class which allows us to use commands,
      such as 'sf.bulk2.Contacts.insert(...)'
     This is really just a middle layer, whose sole purpose is
     to allow the above syntax
     """
 
-    def __init__(self, session_id, bulk2_url, proxies=None, session=None):
+    def __init__(
+            self,
+            session_id: str,
+            bulk2_url: str,
+            proxies: Optional[MutableMapping[str, str]] = None,
+            session: Optional[Session] = None
+            ):
         """Initialize the instance with the given parameters.
 
         Arguments:
 
         * session_id -- the session ID for authenticating to Salesforce
         * bulk2_url -- 2.0 API endpoint set in Salesforce instance
         * proxies -- the optional map of scheme to proxy server
@@ -214,33 +281,41 @@
         # as bulk uses a slightly different format
         self.headers = {
             "Content-Type": "application/json",
             "Authorization": "Bearer " + self.session_id,
             "X-PrettyPrint": "1",
             }
 
-    def __getattr__(self, name):
+    def __getattr__(self,
+                    name: str
+                    ) -> "SFBulk2Type":
         return SFBulk2Type(
             object_name=name,
             bulk2_url=self.bulk2_url,
             headers=self.headers,
             session=self.session,
             )
 
 
 class _Bulk2Client:
     """Bulk 2.0 API client"""
 
     JSON_CONTENT_TYPE = "application/json"
-    CSV_CONTENT_TYPE = "text/csv"
+    CSV_CONTENT_TYPE = "text/csv; charset=UTF-8"
 
     DEFAULT_WAIT_TIMEOUT_SECONDS = 86400  # 24-hour bulk job running time
     MAX_CHECK_INTERVAL_SECONDS = 2.0
 
-    def __init__(self, object_name, bulk2_url, headers, session):
+    def __init__(
+            self,
+            object_name: str,
+            bulk2_url: str,
+            headers: Dict[str, str],
+            session: Session
+            ):
         """
         Arguments:
 
         * object_name -- the name of the type of SObject this represents,
                          e.g. `Lead` or `Contact`
         * bulk2_url -- 2.0 API endpoint set in Salesforce instance
         * headers -- bulk 2.0 API headers
@@ -249,41 +324,50 @@
                      exposed by simple_salesforce.
         """
         self.object_name = object_name
         self.bulk2_url = bulk2_url
         self.session = session
         self.headers = headers
 
-    def _get_headers(self, request_content_type=None, accept_content_type=None):
+    def _get_headers(
+            self,
+            request_content_type: Optional[str] = None,
+            accept_content_type: Optional[str] = None
+            ) -> Dict[str, str]:
         """Get headers for bulk 2.0 API request"""
         headers = copy.deepcopy(self.headers)
         headers["Content-Type"] = request_content_type or self.JSON_CONTENT_TYPE
         headers["ACCEPT"] = accept_content_type or self.JSON_CONTENT_TYPE
         return headers
 
-    def _construct_request_url(self, job_id, is_query: bool):
+    def _construct_request_url(
+            self,
+            job_id: Optional[str],
+            is_query: bool
+            ) -> str:
         """Construct bulk 2.0 API request URL"""
         if not job_id:
             job_id = ""
+        url: str
         if is_query:
             url = self.bulk2_url + "query"
         else:
             url = self.bulk2_url + "ingest"
         if job_id:
             url = f"{url}/{job_id}"
         return url
 
     def create_job(
             self,
-            operation,
-            query=None,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            external_id_field=None,
-            ):
+            operation: Operation,
+            query: Optional[str] = None,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            external_id_field: Optional[str] = None,
+            ) -> Any:
         """Create job
 
         Arguments:
 
         * operation -- Bulk operation to be performed by job
         * query -- SOQL query to be performed by job
         * column_delimiter -- The column delimiter used for CSV job data
@@ -295,50 +379,64 @@
             "columnDelimiter": column_delimiter,
             "lineEnding": line_ending,
             }
         if external_id_field:
             payload["externalIdFieldName"] = external_id_field
 
         is_query = operation in (Operation.query, Operation.query_all)
-        url = self._construct_request_url(None, is_query)
+        url = self._construct_request_url(None,
+                                          is_query
+                                          )
         if is_query:
             headers = self._get_headers(
-                self.JSON_CONTENT_TYPE, self.CSV_CONTENT_TYPE
+                self.JSON_CONTENT_TYPE,
+                self.CSV_CONTENT_TYPE
                 )
             if not query:
                 raise SalesforceBulkV2ExtractError(
                     "Query is required for query jobs"
                     )
             payload["query"] = query
         else:
             headers = self._get_headers(
-                self.JSON_CONTENT_TYPE, self.JSON_CONTENT_TYPE
+                self.JSON_CONTENT_TYPE,
+                self.JSON_CONTENT_TYPE
                 )
             payload["object"] = self.object_name
             payload["contentType"] = "CSV"
         result = call_salesforce(
             url=url,
             method="POST",
             session=self.session,
             headers=headers,
-            data=json.dumps(payload, allow_nan=False),
+            data=json.dumps(payload,
+                            allow_nan=False
+                            ),
             )
         return result.json(object_pairs_hook=OrderedDict)
 
-    def wait_for_job(self, job_id, is_query: bool, wait=0.5):
+    def wait_for_job(
+            self,
+            job_id: str,
+            is_query: bool,
+            wait: float = 0.5
+            ) -> Literal[JobState.job_complete]:
         """Wait for job completion or timeout"""
-        expiration_time: DateTime = pendulum.now().add(
-            seconds=self.DEFAULT_WAIT_TIMEOUT_SECONDS
+        expiration_time: datetime.datetime = (
+            datetime.datetime.now() +
+            datetime.timedelta(seconds=self.DEFAULT_WAIT_TIMEOUT_SECONDS)
             )
         job_status = JobState.in_progress if is_query else JobState.open
         delay_timeout = 0.0
         delay_cnt = 0
         sleep(wait)
-        while pendulum.now() < expiration_time:
-            job_info = self.get_job(job_id, is_query)
+        while datetime.datetime.now() < expiration_time:
+            job_info = self.get_job(job_id,
+                                    is_query
+                                    )
             job_status = job_info["state"]
             if job_status in [
                 JobState.job_complete,
                 JobState.aborted,
                 JobState.failed,
                 ]:
                 if job_status != JobState.job_complete:
@@ -350,128 +448,196 @@
 
             if delay_timeout < self.MAX_CHECK_INTERVAL_SECONDS:
                 delay_timeout = wait + math.exp(delay_cnt) / 1000.0
                 delay_cnt += 1
             sleep(delay_timeout)
         raise SalesforceOperationError(f"Job timeout. Job status: {job_status}")
 
-    def abort_job(self, job_id, is_query: bool):
+    def abort_job(self,
+                  job_id: str,
+                  is_query: bool
+                  ) -> Any:
         """Abort query/ingest job"""
-        return self._set_job_state(job_id, is_query, JobState.aborted)
-
-    def close_job(self, job_id):
+        return self._set_job_state(job_id,
+                                   is_query,
+                                   JobState.aborted
+                                   )
+
+    def close_job(self,
+                  job_id: str
+                  ) -> Any:
         """Close ingest job"""
-        return self._set_job_state(job_id, False, JobState.upload_complete)
+        return self._set_job_state(
+            job_id,
+            False,
+            JobState.upload_complete
+            )
 
-    def delete_job(self, job_id, is_query: bool):
+    def delete_job(self,
+                   job_id: str,
+                   is_query: bool
+                   ) -> Any:
         """Delete query/ingest job"""
-        url = self._construct_request_url(job_id, is_query)
+        url = self._construct_request_url(job_id,
+                                          is_query
+                                          )
         headers = self._get_headers()
         result = call_salesforce(
-            url=url, method="DELETE", session=self.session, headers=headers
+            url=url,
+            method="DELETE",
+            session=self.session,
+            headers=headers
             )
         return result.json(object_pairs_hook=OrderedDict)
 
-    def _set_job_state(self, job_id, is_query: bool, state: str):
+    def _set_job_state(self,
+                       job_id: str,
+                       is_query: bool,
+                       state: str
+                       ) -> Any:
         """Set job state"""
-        url = self._construct_request_url(job_id, is_query)
+        url = self._construct_request_url(job_id,
+                                          is_query
+                                          )
         headers = self._get_headers()
-        payload = {"state": state}
+        payload = {
+            "state": state
+            }
         result = call_salesforce(
             url=url,
             method="PATCH",
             session=self.session,
             headers=headers,
-            data=json.dumps(payload, allow_nan=False),
+            data=json.dumps(payload,
+                            allow_nan=False
+                            ),
             )
         return result.json(object_pairs_hook=OrderedDict)
 
-    def get_job(self, job_id, is_query: bool):
+    def get_job(self,
+                job_id: str,
+                is_query: bool
+                ) -> Any:
         """Get job info"""
-        url = self._construct_request_url(job_id, is_query)
+        url = self._construct_request_url(job_id,
+                                          is_query
+                                          )
 
         result = call_salesforce(
-            url=url, method="GET", session=self.session, headers=self.headers
+            url=url,
+            method="GET",
+            session=self.session,
+            headers=self.headers
             )
         return result.json(object_pairs_hook=OrderedDict)
 
-    def filter_null_bytes(self, b: Union[str, bytes]):
+    def filter_null_bytes(self,
+                          b: AnyStr
+                          ) -> AnyStr:
         """
         https://github.com/airbytehq/airbyte/issues/8300
         """
-        if isinstance(b, str):
-            return b.replace("\x00", "")
-        if isinstance(b, bytes):
-            return b.replace(b"\x00", b"")
+        if isinstance(b,
+                      str
+                      ):
+            return b.replace("\x00",
+                             ""
+                             )
+        if isinstance(b,
+                      bytes
+                      ):
+            return b.replace(b"\x00",
+                             b""
+                             )
         raise TypeError("Expected str or bytes")
 
     def get_query_results(
-            self, job_id, locator: str = "", max_records=DEFAULT_QUERY_PAGE_SIZE
-            ):
+            self,
+            job_id: str,
+            locator: str = "",
+            max_records: int = DEFAULT_QUERY_PAGE_SIZE
+            ) -> QueryResult:
         """Get results for a query job"""
-        url = self._construct_request_url(job_id, True) + "/results"
-        params = {"maxRecords": max_records}
+        url = self._construct_request_url(job_id,
+                                          True
+                                          ) + "/results"
+        params: QueryParameters = {
+            "maxRecords": max_records
+            }
         if locator and locator != "null":
             params["locator"] = locator
         headers = self._get_headers(
-            self.JSON_CONTENT_TYPE, self.CSV_CONTENT_TYPE
+            self.JSON_CONTENT_TYPE,
+            self.CSV_CONTENT_TYPE
             )
         result = call_salesforce(
             url=url,
             method="GET",
             session=self.session,
             headers=headers,
             params=params,
             )
-        locator = result.headers.get("Sforce-Locator", "")
+        locator = result.headers.get("Sforce-Locator",
+                                     ""
+                                     )
         if locator == "null":
             locator = ""
-        number_of_records = int(result.headers.get("Sforce-NumberOfRecords"))
+        number_of_records = int(result.headers["Sforce-NumberOfRecords"])
         return {
             "locator": locator,
             "number_of_records": number_of_records,
-            "records": self.filter_null_bytes(result.text),
+            "records": self.filter_null_bytes(result.content.decode('utf-8')),
             }
 
     def download_job_data(
             self,
-            path,
-            job_id,
+            path: str,
+            job_id: str,
             locator: str = "",
-            max_records=DEFAULT_QUERY_PAGE_SIZE,
-            chunk_size=1024,
-            ):
+            max_records: int = DEFAULT_QUERY_PAGE_SIZE,
+            chunk_size: int = 1024,
+            ) -> QueryResult:
         """Get results for a query job"""
         if not os.path.exists(path):
             raise SalesforceBulkV2LoadError(f"Path does not exist: {path}")
 
-        url = self._construct_request_url(job_id, True) + "/results"
-        params = {"maxRecords": max_records}
+        url = self._construct_request_url(job_id,
+                                          True
+                                          ) + "/results"
+        params: QueryParameters = {
+            "maxRecords": max_records
+            }
         if locator and locator != "null":
             params["locator"] = locator
         headers = self._get_headers(
-            self.JSON_CONTENT_TYPE, self.CSV_CONTENT_TYPE
+            self.JSON_CONTENT_TYPE,
+            self.CSV_CONTENT_TYPE
             )
         with closing(
                 call_salesforce(
                     url=url,
                     method="GET",
                     session=self.session,
                     headers=headers,
                     params=params,
                     stream=True,
                     )
                 ) as result, tempfile.NamedTemporaryFile(
-            "wb", dir=path, suffix=".csv", delete=False
+            "wb",
+            dir=path,
+            suffix=".csv",
+            delete=False
             ) as bos:
-            locator = result.headers.get("Sforce-Locator", "")
+            locator = result.headers.get("Sforce-Locator",
+                                         ""
+                                         )
             if locator == "null":
                 locator = ""
             number_of_records = int(
-                result.headers.get("Sforce-NumberOfRecords")
+                result.headers["Sforce-NumberOfRecords"]
                 )
             for chunk in result.iter_content(chunk_size=chunk_size):
                 bos.write(self.filter_null_bytes(chunk))
             # check the file exists
             if os.path.isfile(bos.name):
                 return {
                     "locator": locator,
@@ -479,85 +645,122 @@
                     "file": bos.name,
                     }
             raise SalesforceBulkV2LoadError(
                 f"The IO/Error occured while verifying binary data. "
                 f"File {bos.name} doesn't exist, url: {url}, "
                 )
 
-    def upload_job_data(self, job_id, data: str, content_url=None):
+    def upload_job_data(
+            self,
+            job_id: str,
+            data: str,
+            content_url: Optional[str] = None
+            ) -> None:
         """Upload job data"""
         if not data:
             raise SalesforceBulkV2LoadError("Data is required for ingest jobs")
 
         # performance reduction here
         data_size = len(data.encode("utf-8"))
         if data_size > MAX_INGEST_JOB_FILE_SIZE:
             raise SalesforceBulkV2LoadError(
                 f"Data size {data_size} exceeds the max file size accepted by "
                 "Bulk V2 (100 MB)"
                 )
 
         url = (
-                content_url
-                or self._construct_request_url(job_id, False) + "/batches"
+                content_url or
+                self._construct_request_url(job_id,
+                                            False
+                                            ) + "/batches"
         )
         headers = self._get_headers(
-            self.CSV_CONTENT_TYPE, self.JSON_CONTENT_TYPE
+            self.CSV_CONTENT_TYPE,
+            self.JSON_CONTENT_TYPE
             )
         result = call_salesforce(
             url=url,
             method="PUT",
             session=self.session,
             headers=headers,
-            data=data,
+            data=data.encode("utf-8"),
             )
         if result.status_code != http.CREATED:
             raise SalesforceBulkV2LoadError(
                 f"Failed to upload job data. Error Code {result.status_code}. "
-                f"Response content: {result.content}"
+                f"Response content: {result.content.decode()}"
                 )
 
-    def get_ingest_results(self, job_id, results_type):
+    def get_ingest_results(self,
+                           job_id: str,
+                           results_type: str
+                           ) -> str:
         """Get record results"""
-        url = self._construct_request_url(job_id, False) + "/" + results_type
+        url = self._construct_request_url(
+            job_id,
+            False
+            ) + "/" + results_type
         headers = self._get_headers(
-            self.JSON_CONTENT_TYPE, self.CSV_CONTENT_TYPE
+            self.JSON_CONTENT_TYPE,
+            self.CSV_CONTENT_TYPE
             )
         result = call_salesforce(
-            url=url, method="GET", session=self.session, headers=headers
+            url=url,
+            method="GET",
+            session=self.session,
+            headers=headers
             )
         return result.text
 
     def download_ingest_results(
-            self, file, job_id, results_type, chunk_size=1024
-            ):
+            self,
+            file: str,
+            job_id: str,
+            results_type: str,
+            chunk_size: int = 1024
+            ) -> None:
         """Download record results to a file"""
-        url = self._construct_request_url(job_id, False) + "/" + results_type
+        url = self._construct_request_url(
+            job_id,
+            False
+            ) + "/" + results_type
         headers = self._get_headers(
-            self.JSON_CONTENT_TYPE, self.CSV_CONTENT_TYPE
+            self.JSON_CONTENT_TYPE,
+            self.CSV_CONTENT_TYPE
             )
         with closing(
                 call_salesforce(
-                    url=url, method="GET", session=self.session, headers=headers
+                    url=url,
+                    method="GET",
+                    session=self.session,
+                    headers=headers
                     )
-                ) as result, open(file, "wb") as bos:
+                ) as result, open(file,
+                                  "wb"
+                                  ) as bos:
             for chunk in result.iter_content(chunk_size=chunk_size):
                 bos.write(self.filter_null_bytes(chunk))
 
         if not os.path.exists(file):
             raise SalesforceBulkV2LoadError(
                 f"The IO/Error occured while verifying binary data. "
                 f"File {file} doesn't exist, url: {url}, "
                 )
 
 
 class SFBulk2Type:
     """Interface to Bulk 2.0 API functions"""
 
-    def __init__(self, object_name, bulk2_url, headers, session):
+    def __init__(
+            self,
+            object_name: str,
+            bulk2_url: str,
+            headers: Dict[str, str],
+            session: Session
+            ):
         """Initialize the instance with the given parameters.
 
         Arguments:
 
         * object_name -- the name of the type of SObject this represents,
                          e.g. `Lead` or `Contact`
         * bulk2_url -- API endpoint set in Salesforce instance
@@ -566,302 +769,422 @@
                      enables the use of requests Session features not otherwise
                      exposed by simple_salesforce.
         """
         self.object_name = object_name
         self.bulk2_url = bulk2_url
         self.session = session
         self.headers = headers
-        self._client = _Bulk2Client(object_name, bulk2_url, headers, session)
+        self._client = _Bulk2Client(object_name,
+                                    bulk2_url,
+                                    headers,
+                                    session
+                                    )
 
     def _upload_data(
             self,
-            operation,
+            operation: Operation,
             data: Union[str, Tuple[int, str]],
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            external_id_field=None,
-            wait=5,
-            ) -> Dict:
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            external_id_field: Optional[str] = None,
+            wait: int = 5,
+            ) -> Dict[str, int]:
         """Upload data to Salesforce"""
-        if len(data) == 2:
-            total, data = data
+        unpacked_data: str
+        if isinstance(data,
+                      tuple
+                      ):
+            total, unpacked_data = data
         else:
             total = _count_csv(
-                data=data, line_ending=line_ending, skip_header=True
+                data=data,
+                line_ending=line_ending,
+                skip_header=True
                 )
+            unpacked_data = data
         res = self._client.create_job(
             operation,
             column_delimiter=column_delimiter,
             line_ending=line_ending,
             external_id_field=external_id_field,
             )
         job_id = res["id"]
         try:
             if res["state"] == JobState.open:
-                self._client.upload_job_data(job_id, data)
+                self._client.upload_job_data(job_id,
+                                             unpacked_data
+                                             )
                 self._client.close_job(job_id)
-                self._client.wait_for_job(job_id, False, wait)
-                res = self._client.get_job(job_id, False)
+                self._client.wait_for_job(job_id,
+                                          False,
+                                          wait
+                                          )
+                res = self._client.get_job(job_id,
+                                           False
+                                           )
                 return {
                     "numberRecordsFailed": int(res["numberRecordsFailed"]),
                     "numberRecordsProcessed": int(
                         res["numberRecordsProcessed"]
                         ),
                     "numberRecordsTotal": int(total),
                     "job_id": job_id,
                     }
             raise SalesforceBulkV2LoadError(
                 f"Failed to upload job data. Response content: {res}"
                 )
         except Exception:
-            res = self._client.get_job(job_id, False)
+            res = self._client.get_job(job_id,
+                                       False
+                                       )
             if res["state"] in (
                     JobState.upload_complete,
                     JobState.in_progress,
                     JobState.open,
                     ):
-                self._client.abort_job(job_id, False)
+                self._client.abort_job(job_id,
+                                       False
+                                       )
             raise
-    #pylint:disable=too-many-locals
+
+    # pylint:disable=too-many-locals
     def _upload_file(
             self,
-            operation,
-            csv_file=None,
-            records=None,
-            batch_size=None,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            external_id_field=None,
-            concurrency=1,
-            wait=5,
-            ) -> List[Dict]:
+            operation: Operation,
+            csv_file: Optional[str] = None,
+            records: Optional[str] = None,
+            batch_size: Optional[int] = None,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            external_id_field: Optional[str] = None,
+            concurrency: int = 1,
+            wait: int = 5,
+            ) -> List[Dict[str, int]]:
         """Upload csv file to Salesforce"""
         if csv_file and records:
             raise SalesforceBulkV2LoadError("Cannot include both file and "
-                                            "records")
+                                            "records"
+                                            )
         if not records and csv_file:
             if not os.path.exists(csv_file):
                 raise SalesforceBulkV2LoadError(csv_file + " not found.")
 
         if operation in (Operation.delete, Operation.hard_delete):
-            with open(csv_file, "r", encoding="utf-8") as bis:
+            assert csv_file is not None
+            with open(csv_file,
+                      "r",
+                      encoding="utf-8"
+                      ) as bis:
                 header = (
                     bis.readline()
                     .rstrip()
                     .split(_delimiter_char[column_delimiter])
                 )
                 if len(header) != 1:
                     raise SalesforceBulkV2LoadError(
                         f"InvalidBatch: The '{operation}' batch must contain "
                         f"only ids, {header}"
                         )
 
         results = []
-        workers = min(concurrency, MAX_INGEST_JOB_PARALLELISM)
-        split_data = _split_csv(filename=csv_file, max_records=batch_size) \
+        workers = min(concurrency,
+                      MAX_INGEST_JOB_PARALLELISM
+                      )
+        split_data = _split_csv(filename=csv_file,
+                                max_records=batch_size
+                                ) \
             if \
-            csv_file else _split_csv(records=records, max_records=batch_size)
+            csv_file else _split_csv(records=records,
+                                     max_records=batch_size
+                                     )
         if workers == 1:
             for data in split_data:
                 result = self._upload_data(
                     operation,
                     data,
                     column_delimiter,
                     line_ending,
                     external_id_field,
                     wait,
                     )
                 results.append(result)
         else:
             # OOM is possible if the file is too large
-            for chunks in chunked(split_data, n=workers):
-                workers = min(workers, len(chunks))
+            for chunks in chunked(split_data,
+                                  n=workers
+                                  ):
+                workers = min(workers,
+                              len(chunks)
+                              )
                 with ThreadPoolExecutor(max_workers=workers) as pool:
                     multi_thread_worker = partial(
                         self._upload_data,
                         operation,
                         column_delimiter=column_delimiter,
                         line_ending=line_ending,
                         external_id_field=external_id_field,
                         wait=wait,
                         )
-                    _results = pool.map(multi_thread_worker, chunks)
+                    _results = pool.map(multi_thread_worker,
+                                        chunks
+                                        )
                 results.extend(list(_results))
         return results
 
     def delete(
             self,
-            csv_file=None,
-            records=None,
-            batch_size=None,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            external_id_field=None,
-            wait=5,
-            ) -> List[Dict]:
+            csv_file: Optional[str] = None,
+            records: Optional[List[Dict[str, str]]] = None,
+            batch_size: Optional[int] = None,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            external_id_field: Optional[str] = None,
+            wait: int = 5,
+            ) -> List[Dict[str, int]]:
         """soft delete records"""
         return self._upload_file(
             Operation.delete,
             csv_file=csv_file,
-            records=_convert_dict_to_csv(records,
-                                         column_delimiter=_delimiter_char.get(
-                                             column_delimiter),
-                                         line_ending=_line_ending_char.get(
-                                             line_ending)),
+            records=_convert_dict_to_csv(
+                records,
+                column_delimiter=_delimiter_char.get(
+                    column_delimiter,
+                    ColumnDelimiter.COMMA
+                    ),
+                line_ending=_line_ending_char.get(
+                    line_ending,
+                    LineEnding.LF
+                    )
+                ),
             batch_size=batch_size,
             column_delimiter=column_delimiter,
             line_ending=line_ending,
             external_id_field=external_id_field,
             wait=wait,
             )
 
     def insert(
             self,
-            csv_file=None,
-            records=None,
-            batch_size=None,
-            concurrency=1,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            wait=5,
-            ) -> List[Dict]:
+            csv_file: Optional[str] = None,
+            records: Optional[List[Dict[str, str]]] = None,
+            batch_size: Optional[int] = None,
+            concurrency: int = 1,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
+            ) -> List[Dict[str, int]]:
         """insert records"""
         return self._upload_file(
             Operation.insert,
             csv_file=csv_file,
-            records=_convert_dict_to_csv(records,
-                                         column_delimiter=_delimiter_char.get(
-                                             column_delimiter),
-                                         line_ending=_line_ending_char.get(
-                                             line_ending)),
+            records=_convert_dict_to_csv(
+                records,
+                column_delimiter=_delimiter_char.get(
+                    column_delimiter,
+                    ColumnDelimiter.COMMA
+                    ),
+                line_ending=_line_ending_char.get(
+                    line_ending,
+                    LineEnding.LF
+                    )
+                ),
             batch_size=batch_size,
             column_delimiter=column_delimiter,
             line_ending=line_ending,
             concurrency=concurrency,
             wait=wait,
             )
 
     def upsert(
             self,
-            csv_file=None,
-            records=None,
-            external_id_field='Id',
-            batch_size=None,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            wait=5,
-            ) -> List[Dict]:
+            csv_file: Optional[str] = None,
+            records: Optional[List[Dict[str, str]]] = None,
+            external_id_field: str = 'Id',
+            batch_size: Optional[int] = None,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
+            ) -> List[Dict[str, int]]:
         """upsert records based on a unique identifier"""
         return self._upload_file(
             Operation.upsert,
             csv_file=csv_file,
-            records=_convert_dict_to_csv(records,
-                                         column_delimiter=_delimiter_char.get(
-                                             column_delimiter),
-                                         line_ending=_line_ending_char.get(
-                                             line_ending)),
+            records=_convert_dict_to_csv(
+                records,
+                column_delimiter=_delimiter_char.get(
+                    column_delimiter,
+                    ColumnDelimiter.COMMA
+                    ),
+                line_ending=_line_ending_char.get(
+                    line_ending,
+                    LineEnding.LF
+                    )
+                ),
             batch_size=batch_size,
             column_delimiter=column_delimiter,
             line_ending=line_ending,
             external_id_field=external_id_field,
             wait=wait,
             )
 
     def update(
             self,
-            csv_file=None,
-            records=None,
-            batch_size=None,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            wait=5,
-            ) -> List[Dict]:
+            csv_file: Optional[str] = None,
+            records: Optional[List[Dict[str, str]]] = None,
+            batch_size: Optional[int] = None,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
+            ) -> List[Dict[str, int]]:
         """update records"""
         return self._upload_file(
             Operation.update,
             csv_file=csv_file,
-            records=_convert_dict_to_csv(records,
-                                         column_delimiter=_delimiter_char.get(
-                                             column_delimiter),
-                                         line_ending=_line_ending_char.get(
-                                             line_ending)),
+            records=_convert_dict_to_csv(
+                records,
+                column_delimiter=_delimiter_char.get(
+                    column_delimiter,
+                    ColumnDelimiter.COMMA
+                    ),
+                line_ending=_line_ending_char.get(
+                    line_ending,
+                    LineEnding.LF
+                    )
+                ),
             batch_size=batch_size,
             column_delimiter=column_delimiter,
             line_ending=line_ending,
             wait=wait,
             )
 
     def hard_delete(
             self,
-            csv_file=None,
-            records=None,
-            batch_size=None,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            wait=5,
-            ) -> List[Dict]:
+            csv_file: Optional[str] = None,
+            records: Optional[List[Dict[str, str]]] = None,
+            batch_size: Optional[int] = None,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
+            ) -> List[Dict[str, int]]:
         """hard delete records"""
         return self._upload_file(
             Operation.hard_delete,
             csv_file=csv_file,
-            records=_convert_dict_to_csv(records,
-                                         column_delimiter=_delimiter_char.get(
-                                             column_delimiter),
-                                         line_ending=_line_ending_char.get(
-                                             line_ending)),
+            records=_convert_dict_to_csv(
+                records,
+                column_delimiter=_delimiter_char.get(
+                    column_delimiter,
+                    ColumnDelimiter.COMMA
+                    ),
+                line_ending=_line_ending_char.get(
+                    line_ending,
+                    LineEnding.LF
+                    )
+                ),
             batch_size=batch_size,
             column_delimiter=column_delimiter,
             line_ending=line_ending,
             wait=wait,
             )
 
     def query(
             self,
+            query: str,
+            max_records: int = DEFAULT_QUERY_PAGE_SIZE,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
+            ) -> Generator[Union[str, int], None, None]:
+        """bulk 2.0 query
+
+        Arguments:
+        * query -- SOQL query
+        * max_records -- max records to retrieve per batch, default 50000
+
+        Returns:
+        * locator  -- the locator for the next set of results
+        * number_of_records -- the number of records in this set
+        * records -- records in this set
+        """
+        res = self._client.create_job(
+            Operation.query,
             query,
-            max_records=DEFAULT_QUERY_PAGE_SIZE,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            wait=5,
+            column_delimiter,
+            line_ending
+            )
+        job_id = res["id"]
+        self._client.wait_for_job(job_id,
+                                  True,
+                                  wait
+                                  )
+
+        locator = "INIT"
+        while locator:
+            if locator == "INIT":
+                locator = ""
+            result = self._client.get_query_results(
+                job_id,
+                locator,
+                max_records
+                )
+            locator = result["locator"]
+            yield result["records"]
+
+    def query_all(
+            self,
+            query: str,
+            max_records: int = DEFAULT_QUERY_PAGE_SIZE,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
             ) -> Generator[str, None, None]:
-        """bulk 2.0 query
+        """bulk 2.0 query_all
 
         Arguments:
         * query -- SOQL query
         * max_records -- max records to retrieve per batch, default 50000
 
         Returns:
         * locator  -- the locator for the next set of results
         * number_of_records -- the number of records in this set
         * records -- records in this set
         """
         res = self._client.create_job(
-            Operation.query, query, column_delimiter, line_ending
+            Operation.query_all,
+            query,
+            column_delimiter,
+            line_ending
             )
         job_id = res["id"]
-        self._client.wait_for_job(job_id, True, wait)
+        self._client.wait_for_job(job_id,
+                                  True,
+                                  wait
+                                  )
 
         locator = "INIT"
         while locator:
             if locator == "INIT":
                 locator = ""
             result = self._client.get_query_results(
-                job_id, locator, max_records
+                job_id,
+                locator,
+                max_records
                 )
             locator = result["locator"]
             yield result["records"]
 
     def download(
             self,
-            query,
-            path,
-            max_records=DEFAULT_QUERY_PAGE_SIZE,
-            column_delimiter=ColumnDelimiter.COMMA,
-            line_ending=LineEnding.LF,
-            wait=5,
-            ) -> List[Dict]:
+            query: str,
+            path: str,
+            max_records: int = DEFAULT_QUERY_PAGE_SIZE,
+            column_delimiter: ColumnDelimiter = ColumnDelimiter.COMMA,
+            line_ending: LineEnding = LineEnding.LF,
+            wait: int = 5,
+            ) -> List[QueryResult]:
         """bulk 2.0 query stream to file, avoiding high memory usage
 
         Arguments:
         * query -- SOQL query
         * max_records -- max records to retrieve per batch, default 50000
 
         Returns:
@@ -869,84 +1192,137 @@
         * number_of_records -- the number of records in this set
         * file -- downloaded file
         """
         if not os.path.exists(path):
             raise SalesforceBulkV2LoadError(f"Path does not exist: {path}")
 
         res = self._client.create_job(
-            Operation.query, query, column_delimiter, line_ending
+            Operation.query,
+            query,
+            column_delimiter,
+            line_ending
             )
         job_id = res["id"]
-        self._client.wait_for_job(job_id, True, wait)
+        self._client.wait_for_job(job_id,
+                                  True,
+                                  wait
+                                  )
 
         results = []
         locator = "INIT"
         while locator:
             if locator == "INIT":
                 locator = ""
             result = self._client.download_job_data(
-                path, job_id, locator, max_records
+                path,
+                job_id,
+                locator,
+                max_records
                 )
             locator = result["locator"]
             results.append(result)
         return results
 
-    def _retrieve_ingest_records(self, job_id, results_type, file=None):
+    def _retrieve_ingest_records(
+            self,
+            job_id: str,
+            results_type: str,
+            file: Optional[str] = None
+            ) -> str:
         """Retrieve the results of an ingest job"""
         if not file:
-            return self._client.get_ingest_results(job_id, results_type)
-        self._client.download_ingest_results(file, job_id, results_type)
+            return self._client.get_ingest_results(job_id,
+                                                   results_type
+                                                   )
+        self._client.download_ingest_results(file,
+                                             job_id,
+                                             results_type
+                                             )
         return ""
 
-    def get_failed_records(self, job_id, file=None):
+    def get_failed_records(
+            self,
+            job_id: str,
+            file: Optional[str] = None
+            ) -> str:
         """Get failed record results
 
         Results Property:
             sf__Id:	[string] ID of the record
             sf__Error:	[Error]	Error code and message
             Fields from the original CSV request data:	various
         """
-        return self._retrieve_ingest_records(job_id, ResultsType.failed, file)
+        return self._retrieve_ingest_records(job_id,
+                                             ResultsType.failed,
+                                             file
+                                             )
 
-    def get_unprocessed_records(self, job_id, file=None):
+    def get_unprocessed_records(
+            self,
+            job_id: str,
+            file: Optional[str] = None
+            ) -> str:
         """Get unprocessed record results
 
         Results Property:
             Fields from the original CSV request data:	[various]
         """
         return self._retrieve_ingest_records(
-            job_id, ResultsType.unprocessed, file
+            job_id,
+            ResultsType.unprocessed,
+            file
             )
 
-    def get_successful_records(self, job_id, file=None):
+    def get_successful_records(
+            self,
+            job_id: str,
+            file: Optional[str] = None
+            ) -> str:
         """Get successful record results.
 
         Results Property:
             sf__Id:	[string] ID of the record
             sf__Created: [boolean] Indicates if the record was created
             Fields from the original CSV request data:	[various]
         """
         return self._retrieve_ingest_records(
-            job_id, ResultsType.successful, file
+            job_id,
+            ResultsType.successful,
+            file
             )
 
-    def get_all_ingest_records(self, job_id, file=None):
+    def get_all_ingest_records(
+            self,
+            job_id: str,
+            file: Optional[str] = None
+            ) -> Dict[str, List[Any]]:
         """Get all ingest record results for job
 
         Results Property:
             sf__Id:	[string] ID of the record
             sf__Created: [boolean] Indicates if the record was created
             Fields from the original CSV request data:	[various]
             Fields: [various] Fields from the original CSV request data
         """
         successful_records = csv.DictReader(self.get_successful_records(
-            job_id=job_id,file=file).splitlines(),delimiter=',',
-            lineterminator='\n',)
+            job_id=job_id,
+            file=file
+            ).splitlines(),
+                                            delimiter=',',
+                                            lineterminator='\n', )
         failed_records = csv.DictReader(self.get_failed_records(
-            job_id=job_id,file=file).splitlines(),delimiter=',',
-            lineterminator='\n',)
+            job_id=job_id,
+            file=file
+            ).splitlines(),
+                                        delimiter=',',
+                                        lineterminator='\n', )
         unprocessed_records = csv.DictReader(self.get_unprocessed_records(
-            job_id=job_id,file=file).splitlines(),delimiter=',',
-            lineterminator='\n',)
-        return {'successfulRecords':list(successful_records),
-                'failedRecords':list(failed_records),
-                'unprocessedRecords':list(unprocessed_records)}
+            job_id=job_id,
+            file=file
+            ).splitlines(),
+                                             delimiter=',',
+                                             lineterminator='\n', )
+        return {
+            'successfulRecords': list(successful_records),
+            'failedRecords': list(failed_records),
+            'unprocessedRecords': list(unprocessed_records)
+            }
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce/login.py` & `simple-salesforce-1.12.6/simple_salesforce/login.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 """Login classes and functions for Simple-Salesforce
 
 Heavily Modified from RestForce 1.0.0
 """
+from typing import Any, Dict, Optional, Tuple, Union, cast
 import base64
 
 DEFAULT_CLIENT_ID_PREFIX = 'simple-salesforce'
 
 import warnings
 from datetime import datetime, timedelta, timezone
 from html import escape, unescape
 from json.decoder import JSONDecodeError
 from pathlib import Path
+from xml.parsers.expat import ExpatError
 
 import requests
 import jwt
 
 from .api import DEFAULT_API_VERSION
 from .exceptions import SalesforceAuthenticationFailed
-from .util import getUniqueElementValueFromXmlString
+from .util import Headers, Proxies, getUniqueElementValueFromXmlString
 
 
 # pylint: disable=invalid-name,too-many-arguments,too-many-locals,too-many-branches
 def SalesforceLogin(
-        username=None,
-        password=None,
-        security_token=None,
-        organizationId=None,
-        sf_version=DEFAULT_API_VERSION,
-        proxies=None,
-        session=None,
-        client_id=None,
-        domain=None,
-        consumer_key=None,
-        consumer_secret=None,
-        privatekey_file=None,
-        privatekey=None,
-        ):
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        security_token: Optional[str] = None,
+        organizationId: Optional[str] = None,
+        sf_version: str = DEFAULT_API_VERSION,
+        proxies: Optional[Proxies] = None,
+        session: Optional[requests.Session] = None,
+        client_id: Optional[str] = None,
+        domain: Optional[str] = None,
+        instance_url: Optional[str] =None,
+        consumer_key: Optional[str] = None,
+        consumer_secret: Optional[str] = None,
+        privatekey_file: Optional[str] = None,
+        privatekey: Optional[str] = None,
+        ) -> Tuple[str, str]:
     """Return a tuple of `(session_id, sf_instance)` where `session_id` is the
     session ID to use for authentication to Salesforce and `sf_instance` is
     the domain of the instance of Salesforce to use for the session.
 
     Arguments:
 
     * username -- the Salesforce username to use for authentication
@@ -54,14 +57,16 @@
                  enables the use of requets Session features not otherwise
                  exposed by simple_salesforce.
     * client_id -- the ID of this client
     * domain -- The domain to using for connecting to Salesforce. Use
                 common domains, such as 'login' or 'test', or
                 Salesforce My domain. If not used, will default to
                 'login'.
+    * instance_url -- Non-standard instance url (instance.my) used
+                for connecting to Salesforce with JWT tokens.
     * consumer_key -- the consumer key generated for the user/app
     * consumer_secret -- the consumer secret generated for the user/app
     * privatekey_file -- the path to the private key file used
                          for signing the JWT token.
     * privatekey -- the private key to use
                          for signing the JWT token.
     """
@@ -165,34 +170,35 @@
             <urn:password>{password}</urn:password>
         </urn:login>
     </soapenv:Body>
 </soapenv:Envelope>"""
     elif username is not None and \
             consumer_key is not None and \
             (privatekey_file is not None or privatekey is not None):
+        token_domain = instance_url if instance_url is not None else domain
         expiration = datetime.now(timezone.utc) + timedelta(minutes=3)
         payload = {
             'iss': consumer_key,
             'sub': unescape(username),
             'aud': f'https://{domain}.salesforce.com',
             'exp': f'{expiration.timestamp():.0f}'
             }
         if privatekey_file is not None:
-            key = Path(privatekey_file).read_bytes()
+            key: Union[bytes, str] = Path(privatekey_file).read_bytes()
         else:
-            key = privatekey
+            key = cast(str, privatekey)
         assertion = jwt.encode(payload, key, algorithm='RS256')
 
         token_data = {
             'grant_type': 'urn:ietf:params:oauth:grant-type:jwt-bearer',
             'assertion': assertion
             }
 
         return token_login(
-            f'https://{domain}.salesforce.com/services/oauth2/token',
+            f'https://{token_domain}.salesforce.com/services/oauth2/token',
             token_data, domain, consumer_key,
             None, proxies, session)
     elif consumer_key is not None and consumer_secret is not None and \
             domain is not None and domain not in ('login', 'test'):
         token_data = {'grant_type': 'client_credentials'}
         authorization = f'{consumer_key}:{consumer_secret}'
         encoded = base64.b64encode(authorization.encode()).decode()
@@ -218,42 +224,68 @@
         'SOAPAction': 'login'
         }
 
     return soap_login(soap_url, login_soap_request_body,
                       login_soap_request_headers, proxies, session)
 
 
-def soap_login(soap_url, request_body, headers, proxies, session=None):
+def soap_login(
+        soap_url: str,
+        request_body: str,
+        headers: Optional[Headers],
+        proxies: Optional[Proxies],
+        session: Optional[requests.Session] = None) -> Tuple[str, str]:
     """Process SOAP specific login workflow."""
     response = (session or requests).post(
         soap_url, request_body, headers=headers, proxies=proxies)
 
     if response.status_code != 200:
-        except_code = getUniqueElementValueFromXmlString(
-            response.content, 'sf:exceptionCode')
-        except_msg = getUniqueElementValueFromXmlString(
-            response.content, 'sf:exceptionMessage')
+        except_code: Union[str, int, None]
+        except_msg: str
+        try:
+            except_code = getUniqueElementValueFromXmlString(
+                response.content, 'sf:exceptionCode')
+            except_msg = (getUniqueElementValueFromXmlString(
+                response.content, 'sf:exceptionMessage')
+                or response.content.decode())
+        except ExpatError:
+            except_code = response.status_code
+            except_msg = response.content.decode()
         raise SalesforceAuthenticationFailed(except_code, except_msg)
 
     session_id = getUniqueElementValueFromXmlString(
         response.content, 'sessionId')
     server_url = getUniqueElementValueFromXmlString(
         response.content, 'serverUrl')
+    if session_id is None or server_url is None:
+        except_code = getUniqueElementValueFromXmlString(
+            response.content, 'sf:exceptionCode'
+        ) or 'UNKNOWN_EXCEPTION_CODE'
+        except_msg = getUniqueElementValueFromXmlString(
+            response.content, 'sf:exceptionMessage'
+        ) or 'UNKNOWN_EXCEPTION_MESSAGE'
+        raise SalesforceAuthenticationFailed(except_code, except_msg)
 
     sf_instance = (server_url
                    .replace('http://', '')
                    .replace('https://', '')
                    .split('/')[0]
                    .replace('-api', ''))
 
     return session_id, sf_instance
 
 
-def token_login(token_url, token_data, domain, consumer_key,
-                headers, proxies, session=None):
+def token_login(
+        token_url: str,
+        token_data: Dict[str, Any],
+        domain: str,
+        consumer_key: str,
+        headers: Optional[Headers],
+        proxies: Optional[Proxies],
+        session: Optional[requests.Session] = None) -> Tuple[Any, Any]:
     """Process OAuth 2.0 JWT Bearer Token Flow."""
     response = (session or requests).post(
         token_url, token_data, headers=headers, proxies=proxies)
 
     try:
         json_response = response.json()
     except JSONDecodeError as exc:
```

### Comparing `simple-salesforce-1.12.5/simple_salesforce/metadata.py` & `simple-salesforce-1.12.6/simple_salesforce/metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 """ Class to work with Salesforce Metadata API """
+
 from base64 import b64encode, b64decode
 from pathlib import Path
+from typing import Any, Dict, IO, List, Mapping, Optional, Tuple, Union
 from xml.etree import ElementTree as ET
-from .util import call_salesforce
+from xml.etree.ElementTree import Element
+
+import requests
+from zeep.proxy import ServiceProxy
+from zeep.xsd import AnySimpleType, ComplexType, CompoundValue
+
+from .util import Headers, call_salesforce
 from .messages import DEPLOY_MSG, CHECK_DEPLOY_STATUS_MSG, \
     CHECK_RETRIEVE_STATUS_MSG, RETRIEVE_MSG
 from zeep import Client, Settings
 
 
 class MetadataType:
     """
     Salesforce Metadata Type
     """
-    def __init__(self, name, service, zeep_type, session_header):
+    def __init__(
+            self,
+            name: str,
+            service: ServiceProxy,
+            zeep_type: Union[ComplexType, AnySimpleType],
+            session_header: CompoundValue):
         """
         Initialize metadata type
 
         :param name: Name of metadata type
         :type name: str
         :param service: Zeep service
         :type service: zeep.proxy.ServiceProxy
@@ -27,15 +40,15 @@
         self._name = name
         self._service = service
         self._zeep_type = zeep_type
         self._session_header = session_header
 
     @staticmethod
     # pylint: disable=broad-exception-raised
-    def _handle_api_response(response):
+    def _handle_api_response(response: List[Any]) -> None:
         """
         Parses SaveResult and DeleteResult objects to identify if there was
         an error, and raises exception accordingly
 
         :param response: List of zeep.objects.SaveResult or
         zeep.objects.DeleteResult objects
         :type response: list
@@ -47,25 +60,25 @@
             if not result.success:
                 err_string += f'\n{result.fullName}: '
                 for error in result.errors:
                     err_string += f'({error.statusCode}, {error.message}), '
         if err_string:
             raise Exception(err_string)
 
-    def __call__(self, *args, **kwargs):
+    def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """
         Creates a new object of this metadata type
 
         :param args: Parameters to pass to zeep.xsd.AnySimpleType
         :param kwargs: Parameters to pass to zeep.xsd.ComplexType
         :returns: An object of type self._name
         """
         return self._zeep_type(*args, **kwargs)
 
-    def create(self, metadata):
+    def create(self, metadata: List[Any]) -> None:
         """
         Performs a createMetadata call
 
         :param metadata: Array of one or more metadata components.
                          Limit: 10. (For CustomMetadata and CustomApplication
                          only, the limit is 200.)
                          You must submit arrays of only one type of
@@ -74,15 +87,15 @@
                          mix of both types.
         :type metadata: list
         """
         response = self._service.createMetadata(metadata, _soapheaders=[
             self._session_header])
         self._handle_api_response(response)
 
-    def read(self, full_names):
+    def read(self, full_names: List[str]) -> Union[List[Any], Any]:
         """
         Performs a readMetadata call
 
         :param full_names: Array of full names of the components to read.
                            Limit: 10. (For CustomMetadata and
                            CustomApplication only, the limit is 200.)
                            You must submit arrays of only one type of
@@ -96,15 +109,15 @@
         response = self._service.readMetadata(self._name, full_names,
                                               _soapheaders=[
                                                   self._session_header])
         if len(response) == 1:
             return response[0]
         return response
 
-    def update(self, metadata):
+    def update(self, metadata: List[Any]) -> None:
         """
         Performs an updateMetadata call. All required fields must be passed
         for each component
 
         :param metadata: Array of one or more metadata components.
                          Limit: 10. (For CustomMetadata and CustomApplication
                          only, the limit is 200.)
@@ -114,15 +127,15 @@
                          mix of both types.
         :type metadata: list
         """
         response = self._service.updateMetadata(metadata, _soapheaders=[
             self._session_header])
         self._handle_api_response(response)
 
-    def upsert(self, metadata):
+    def upsert(self, metadata: List[Any]) -> None:
         """
         Performs an upsertMetadata call. All required fields must be passed
         for each component
 
         :param metadata: Array of one or more metadata components.
                          Limit: 10. (For CustomMetadata and CustomApplication
                          only, the limit is 200.)
@@ -132,15 +145,15 @@
                          mix of both types.
         :type metadata: list
         """
         response = self._service.upsertMetadata(metadata, _soapheaders=[
             self._session_header])
         self._handle_api_response(response)
 
-    def delete(self, full_names):
+    def delete(self, full_names: List[Dict[str, Any]]) -> None:
         """
         Performs a deleteMetadata call
 
         :param full_names: Array of full names of the components to delete.
                            Limit: 10. (For CustomMetadata and
                            CustomApplication only, the limit is 200.)
                            You must submit arrays of only one type of
@@ -150,30 +163,30 @@
         :type full_names: list
         """
         response = self._service.deleteMetadata(self._name, full_names,
                                                 _soapheaders=[
                                                     self._session_header])
         self._handle_api_response(response)
 
-    def rename(self, old_full_name, new_full_name):
+    def rename(self, old_full_name: str, new_full_name: str) -> None:
         """
         Performs a renameMetadata call
 
         :param old_full_name: The current component full name.
         :type old_full_name: str
         :param new_full_name: The new component full name.
         :type new_full_name: str
         """
         result = self._service.renameMetadata(self._name, old_full_name,
                                               new_full_name,
                                               _soapheaders=[
                                                   self._session_header])
         self._handle_api_response([result])
 
-    def describe(self):
+    def describe(self) -> Any:
         """
         Performs a describeValueType call
 
         :returns: DescribeValueTypeResult
         """
         return self._service.describeValueType(
             f'{{http://soap.sforce.com/2006/04/metadata}}{self._name}',
@@ -186,65 +199,84 @@
     _METADATA_API_BASE_URI = "/services/Soap/m/{version}"
     _XML_NAMESPACES = {
         'soapenv': 'http://schemas.xmlsoap.org/soap/envelope/',
         'mt': 'http://soap.sforce.com/2006/04/metadata'
         }
 
     # pylint: disable=R0913
-    def __init__(self, session, session_id, instance, metadata_url, headers,
-                 api_version):
+    def __init__(
+            self,
+            session: requests.Session,
+            session_id: str,
+            instance: str,
+            metadata_url: str,
+            headers: Headers,
+            api_version: Optional[str]):
         """ Initialize and check session """
         self.session = session
         self._session_id = session_id
         self._instance = instance
         self.metadata_url = metadata_url
         self.headers = headers
         self._api_version = api_version
         self._deploy_zip = None
         wsdl_path = Path(__file__).parent / 'metadata.wsdl'
-        self._client = Client(wsdl_path.absolute().as_uri(),
-                              settings=Settings(strict=False,
-                                                xsd_ignore_sequence_order=True))
+        self._client = Client(
+            wsdl_path.absolute().as_uri(),
+            settings=Settings(
+                strict=False,
+                xsd_ignore_sequence_order=True
+            ))  # type: ignore[no-untyped-call]
         self._service = self._client.create_service(
             "{http://soap.sforce.com/2006/04/metadata}MetadataBinding",
-            self.metadata_url)
-        self._session_header = self._client.get_element('ns0:SessionHeader')(
-            sessionId=self._session_id)
-
-    def __getattr__(self, item):
-        return MetadataType(item, self._service,
-                            self._client.get_type('ns0:' + item),
-                            self._session_header)
+            self.metadata_url)  # type: ignore[no-untyped-call]
+        self._session_header = self._client.get_element(
+            'ns0:SessionHeader'  # type: ignore[no-untyped-call]
+        )(sessionId=self._session_id)
+
+    def __getattr__(self, item: str) -> MetadataType:
+        return MetadataType(
+            item,
+            self._service,
+            self._client.get_type(
+                'ns0:' + item),  # type: ignore[no-untyped-call]
+            self._session_header)
 
-    def describe_metadata(self):
+    def describe_metadata(self) -> Any:
         """
         Performs a describeMetadata call
 
         :returns: An object of zeep.objects.DescribeMetadataResult
         """
         return self._service.describeMetadata(self._api_version, _soapheaders=[
             self._session_header])
 
-    def list_metadata(self, queries):
+    def list_metadata(self, queries: List[Any]) -> List[Any]:
         """
         Performs a listMetadata call
 
         :param queries: A list of zeep.objects.ListMetadataQuery that specify
         which components you are interested in.
                         Limit: 3
         :type queries: list
         :returns: List of zeep.objects.FileProperties objects
         :rtype: list
         """
-        return self._service.listMetadata(queries, self._api_version,
-                                          _soapheaders=[self._session_header])
+        return self._service.listMetadata(  # type: ignore[no-any-return]
+            queries,
+            self._api_version,
+            _soapheaders=[self._session_header])
 
     # pylint: disable=R0914
     # pylint: disable-msg=C0103
-    def deploy(self, zipfile, sandbox, **kwargs):
+    def deploy(
+            self,
+            zipfile: Union[str, IO[bytes]],
+            sandbox: bool,
+            **kwargs: Any) -> Tuple[Optional[str], Optional[str]]:
         """ Kicks off async deployment, returns deployment id
         :param zipfile:
         :type zipfile:
         :param kwargs:
         :type kwargs:
         :return:
         :rtype:
@@ -298,41 +330,46 @@
         result = call_salesforce(url=self.metadata_url + 'deployRequest',
                                  method='POST',
                                  session=self.session,
                                  headers=self.headers,
                                  additional_headers=headers,
                                  data=request)
 
-        async_process_id = ET.fromstring(result.text).find(
+        async_process_id = ET.fromstring(result.text).findtext(
             'soapenv:Body/mt:deployResponse/mt:result/mt:id',
-            self._XML_NAMESPACES).text
-        state = ET.fromstring(result.text).find(
+            None,
+            self._XML_NAMESPACES) or None
+        state = ET.fromstring(result.text).findtext(
             'soapenv:Body/mt:deployResponse/mt:result/mt:state',
-            self._XML_NAMESPACES).text
+            None,
+            self._XML_NAMESPACES) or None
 
         return async_process_id, state
 
     @staticmethod
     # pylint: disable=R1732
-    def _read_deploy_zip(zipfile):
+    def _read_deploy_zip(zipfile: Union[str, IO[bytes]]) -> str:
         """
         :param zipfile:
         :type zipfile:
         :return:
         :rtype:
         """
-        if hasattr(zipfile, 'read'):
+        if hasattr(zipfile, 'read') and hasattr(zipfile, 'seek'):
             zipfile.seek(0)
             raw = zipfile.read()
         else:
             raw = Path(zipfile).read_bytes()
         return b64encode(raw).decode()
 
     # pylint: disable=broad-exception-raised
-    def _retrieve_deploy_result(self, async_process_id, **kwargs):
+    def _retrieve_deploy_result(
+            self,
+            async_process_id: str,
+            **kwargs: Any) -> Element:
         """ Retrieves status for specified deployment id
         :param async_process_id:
         :type async_process_id:
         :param kwargs:
         :type kwargs:
         :return:
         :rtype:
@@ -364,114 +401,132 @@
             self._XML_NAMESPACES)
         if result is None:
             raise Exception(f"Result node could not be found: {res.text}")
 
         return result
 
     @staticmethod
-    def get_component_error_count(value):
+    def get_component_error_count(value: str) -> int:
         """Get component error counts"""
         try:
             return int(value)
         except ValueError:
             return 0
 
-    def check_deploy_status(self, async_process_id, **kwargs):
+    def check_deploy_status(
+            self,
+            async_process_id: str,
+            **kwargs: Any
+    ) -> Tuple[Optional[str],
+                Optional[str],
+                Optional[Mapping[str, Any]],
+                Optional[Mapping[str, Any]]]:
         """
         Checks whether deployment succeeded
         :param async_process_id:
         :type async_process_id:
         :param kwargs:
         :type kwargs:
         :return:
         :rtype:
         """
         result = self._retrieve_deploy_result(async_process_id, **kwargs)
 
-        state = result.find('mt:status', self._XML_NAMESPACES).text
-        state_detail = result.find('mt:stateDetail', self._XML_NAMESPACES)
-        if state_detail is not None:
-            state_detail = state_detail.text
+        state = result.findtext(
+            'mt:status', None, self._XML_NAMESPACES) or None
+        state_detail = result.findtext(
+            'mt:stateDetail', None, self._XML_NAMESPACES) or None
 
         unit_test_errors = []
         deployment_errors = []
         failed_count = self.get_component_error_count(
-            result.find('mt:numberComponentErrors', self._XML_NAMESPACES).text)
+            result.findtext(
+                'mt:numberComponentErrors', '', self._XML_NAMESPACES))
         if state == 'Failed' or failed_count > 0:
             # Deployment failures
             failures = result.findall('mt:details/mt:componentFailures',
                                       self._XML_NAMESPACES)
             for failure in failures:
                 deployment_errors.append({
-                    'type': failure.find('mt:componentType',
-                                         self._XML_NAMESPACES).text,
-                    'file': failure.find('mt:fileName',
-                                         self._XML_NAMESPACES).text,
-                    'status': failure.find('mt:problemType',
-                                           self._XML_NAMESPACES).text,
-                    'message': failure.find('mt:problem',
-                                            self._XML_NAMESPACES).text
+                    'type': failure.findtext(
+                        'mt:componentType', None, self._XML_NAMESPACES) or None,
+                    'file': failure.findtext(
+                        'mt:fileName', None, self._XML_NAMESPACES) or None,
+                    'status': failure.findtext(
+                        'mt:problemType', None, self._XML_NAMESPACES) or None,
+                    'message': failure.findtext(
+                        'mt:problem', None, self._XML_NAMESPACES) or None
                     })
             # Unit test failures
             failures = result.findall(
                 'mt:details/mt:runTestResult/mt:failures',
                 self._XML_NAMESPACES)
             for failure in failures:
                 unit_test_errors.append({
-                    'class': failure.find('mt:name', self._XML_NAMESPACES).text,
-                    'method': failure.find('mt:methodName',
-                                           self._XML_NAMESPACES).text,
-                    'message': failure.find('mt:message',
-                                            self._XML_NAMESPACES).text,
-                    'stack_trace': failure.find('mt:stackTrace',
-                                                self._XML_NAMESPACES).text
+                    'class': failure.findtext(
+                        'mt:name', None, self._XML_NAMESPACES) or None,
+                    'method': failure.findtext(
+                        'mt:methodName', None, self._XML_NAMESPACES) or None,
+                    'message': failure.findtext(
+                        'mt:message', None, self._XML_NAMESPACES) or None,
+                    'stack_trace': failure.findtext(
+                        'mt:stackTrace', None, self._XML_NAMESPACES) or None
                     })
 
         deployment_detail = {
-            'total_count': result.find('mt:numberComponentsTotal',
-                                       self._XML_NAMESPACES).text,
-            'failed_count': result.find('mt:numberComponentErrors',
-                                        self._XML_NAMESPACES).text,
-            'deployed_count': result.find('mt:numberComponentsDeployed',
-                                          self._XML_NAMESPACES).text,
+            'total_count': result.findtext('mt:numberComponentsTotal',
+                                           None,
+                                           self._XML_NAMESPACES) or None,
+            'failed_count': result.findtext('mt:numberComponentErrors',
+                                            None,
+                                            self._XML_NAMESPACES) or None,
+            'deployed_count': result.findtext('mt:numberComponentsDeployed',
+                                              None,
+                                              self._XML_NAMESPACES) or None,
             'errors': deployment_errors
             }
         unit_test_detail = {
-            'total_count': result.find('mt:numberTestsTotal',
-                                       self._XML_NAMESPACES).text,
-            'failed_count': result.find('mt:numberTestErrors',
-                                        self._XML_NAMESPACES).text,
-            'completed_count': result.find('mt:numberTestsCompleted',
-                                           self._XML_NAMESPACES).text,
+            'total_count': result.findtext('mt:numberTestsTotal',
+                                           None,
+                                           self._XML_NAMESPACES) or None,
+            'failed_count': result.findtext('mt:numberTestErrors',
+                                            None,
+                                            self._XML_NAMESPACES) or None,
+            'completed_count': result.findtext('mt:numberTestsCompleted',
+                                               None,
+                                               self._XML_NAMESPACES) or None,
             'errors': unit_test_errors
             }
 
         return state, state_detail, deployment_detail, unit_test_detail
 
-    def download_unit_test_logs(self, async_process_id):
+    def download_unit_test_logs(self, async_process_id: str) -> None:
         """ Downloads Apex logs for unit tests executed during specified
         deployment """
         result = self._retrieve_deploy_result(async_process_id)
         print("response:", ET.tostring(result, encoding="us-ascii",
                                        method="xml"))
 
-    def retrieve(self, async_process_id, **kwargs):
+    def retrieve(
+            self,
+            async_process_id: str,
+            **kwargs: Any) -> Tuple[Optional[str], Optional[str]]:
         """ Submits retrieve request """
         # Compose unpackaged XML
         client = kwargs.get('client', 'simple_salesforce_metahelper')
         single_package = kwargs.get('single_package', True)
 
         if not isinstance(single_package, bool):
             raise TypeError('single_package must be bool')
 
         unpackaged = ''
         if kwargs.get('unpackaged'):
-            for metadata_type in kwargs.get('unpackaged'):
+            for metadata_type in kwargs.get('unpackaged', {}):
                 if isinstance(kwargs.get('unpackaged'), dict):
-                    members = kwargs.get('unpackaged')[metadata_type]
+                    members = kwargs.get('unpackaged', {})[metadata_type]
                     unpackaged += '<types>'
                     for member in members:
                         unpackaged += f'<members>{member}</members>'
                     unpackaged += f'<name>{metadata_type}</name></types>'
                 else:
                     raise TypeError('unpackaged metadata types must be a dict')
 
@@ -492,25 +547,31 @@
             method='POST',
             session=self.session,
             headers=self.headers,
             additional_headers=headers,
             data=request)
 
         # Parse response to get async Id and status
-        async_process_id = ET.fromstring(res.text).find(
+        async_process_id_ = ET.fromstring(res.text).findtext(
             'soapenv:Body/mt:retrieveResponse/mt:result/mt:id',
-            self._XML_NAMESPACES).text
-        state = ET.fromstring(res.text).find(
+            None,
+            self._XML_NAMESPACES) or None
+        state = ET.fromstring(res.text).findtext(
             'soapenv:Body/mt:retrieveResponse/mt:result/mt:state',
-            self._XML_NAMESPACES).text
+            None,
+            self._XML_NAMESPACES) or None
 
-        return async_process_id, state
+        return async_process_id_, state
 
     # pylint: disable=broad-exception-raised
-    def retrieve_retrieve_result(self, async_process_id, include_zip, **kwargs):
+    def retrieve_retrieve_result(
+            self,
+            async_process_id: str,
+            include_zip: str,
+            **kwargs: Any) -> Element:
         """ Retrieves status for specified retrieval id """
         client = kwargs.get('client', 'simple_salesforce_metahelper')
         attributes = {
             'client': client,
             'sessionId': self._session_id,
             'asyncProcessId': async_process_id,
             'includeZip': include_zip
@@ -532,52 +593,64 @@
             'soapenv:Body/mt:checkRetrieveStatusResponse/mt:result',
             self._XML_NAMESPACES)
         if result is None:
             raise Exception(f"Result node could not be found: {res.text}")
 
         return result
 
-    def retrieve_zip(self, async_process_id, **kwargs):
+    def retrieve_zip(
+            self,
+            async_process_id: str,
+            **kwargs: Any
+    ) -> Tuple[Optional[str], Optional[str], List[Dict[str, Any]], bytes]:
         """ Retrieves ZIP file """
         result = self.retrieve_retrieve_result(async_process_id, 'true',
                                                **kwargs)
-        state = result.find('mt:status', self._XML_NAMESPACES).text
-        error_message = result.find('mt:errorMessage', self._XML_NAMESPACES)
-        if error_message is not None:
-            error_message = error_message.text
+        state = result.findtext('mt:status', None, self._XML_NAMESPACES) or None
+        error_message = result.findtext(
+            'mt:errorMessage', None, self._XML_NAMESPACES)
 
         # Check if there are any messages
         messages = []
         message_list = result.findall('mt:details/mt:messages',
                                       self._XML_NAMESPACES)
         for message in message_list:
             messages.append({
-                'file': message.find('mt:fileName', self._XML_NAMESPACES).text,
-                'message': message.find('mt:problem', self._XML_NAMESPACES).text
+                'file': message.findtext(
+                    'mt:fileName', None, self._XML_NAMESPACES) or None,
+                'message': message.findtext(
+                    'mt:problem', None, self._XML_NAMESPACES) or None
                 })
 
         # Retrieve base64 encoded ZIP file
-        zipfile_base64 = result.find('mt:zipFile', self._XML_NAMESPACES).text
-        zipfile = b64decode(zipfile_base64)
+        zipfile_base64 = result.findtext(
+            'mt:zipFile', None, self._XML_NAMESPACES
+        ) or None
+        zipfile = b64decode(zipfile_base64)  # type: ignore[arg-type]
 
         return state, error_message, messages, zipfile
 
-    def check_retrieve_status(self, async_process_id, **kwargs):
+    def check_retrieve_status(
+            self,
+            async_process_id: str,
+            **kwargs: Any
+    ) -> Tuple[Optional[str], Optional[str], List[Dict[str, Optional[str]]]]:
         """ Checks whether retrieval succeeded """
         result = self.retrieve_retrieve_result(async_process_id, 'false',
                                                **kwargs)
-        state = result.find('mt:status', self._XML_NAMESPACES).text
-        error_message = result.find('mt:errorMessage', self._XML_NAMESPACES)
-        if error_message is not None:
-            error_message = error_message.text
+        state = result.findtext('mt:status', None, self._XML_NAMESPACES) or None
+        error_message = result.findtext(
+            'mt:errorMessage', None, self._XML_NAMESPACES)
 
         # Check if there are any messages
         messages = []
         message_list = result.findall('mt:details/mt:messages',
                                       self._XML_NAMESPACES)
         for message in message_list:
             messages.append({
-                'file': message.find('mt:fileName', self._XML_NAMESPACES).text,
-                'message': message.find('mt:problem', self._XML_NAMESPACES).text
+                'file': message.findtext(
+                    'mt:fileName', None, self._XML_NAMESPACES) or None,
+                'message': message.findtext(
+                    'mt:problem', None, self._XML_NAMESPACES) or None
                 })
 
         return state, error_message, messages
```

