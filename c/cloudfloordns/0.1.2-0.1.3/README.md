# Comparing `tmp/cloudfloordns-0.1.2.tar.gz` & `tmp/cloudfloordns-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudfloordns-0.1.2.tar", max compression
+gzip compressed data, was "cloudfloordns-0.1.3.tar", max compression
```

## Comparing `cloudfloordns-0.1.2.tar` & `cloudfloordns-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,25 @@
--rw-r--r--   0        0        0     3000 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/README.md
--rw-r--r--   0        0        0      127 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/__init__.py
--rw-r--r--   0        0        0      470 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/__main__.py
--rw-r--r--   0        0        0     2935 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/client.py
--rw-r--r--   0        0        0     7376 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/domain.py
--rw-r--r--   0        0        0     3904 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/domain_registration.py
--rw-r--r--   0        0        0       50 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/pool.py
--rw-r--r--   0        0        0     3623 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/record.py
--rw-r--r--   0        0        0     1813 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/utils/__init__.py
--rw-r--r--   0        0        0     1372 2024-03-19 10:37:20.130236 cloudfloordns-0.1.2/cloudfloordns/utils/mail.py
--rw-r--r--   0        0        0      746 2024-03-19 10:37:20.134236 cloudfloordns-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3575 1970-01-01 00:00:00.000000 cloudfloordns-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     3000 2024-04-15 13:32:53.472219 cloudfloordns-0.1.3/README.md
+-rw-r--r--   0        0        0       89 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/__init__.py
+-rw-r--r--   0        0        0      470 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/__main__.py
+-rw-r--r--   0        0        0       25 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/__init__.py
+-rw-r--r--   0        0        0       27 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/__init__.py
+-rw-r--r--   0        0        0     5506 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/client.py
+-rw-r--r--   0        0        0     7406 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/domain.py
+-rw-r--r--   0        0        0      141 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/domain_registration.py
+-rw-r--r--   0        0        0     1475 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client/sync/groups.py
+-rw-r--r--   0        0        0       50 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/client/sync/pool.py
+-rw-r--r--   0        0        0     1547 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/client/sync/record.py
+-rw-r--r--   0        0        0     3433 2024-04-15 13:32:53.476219 cloudfloordns-0.1.3/cloudfloordns/client.py
+-rw-r--r--   0        0        0     8725 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/domain.py
+-rw-r--r--   0        0        0     3904 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/domain_registration.py
+-rw-r--r--   0        0        0     2050 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/groups.py
+-rw-r--r--   0        0        0       80 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/__init__.py
+-rw-r--r--   0        0        0     1363 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/domain.py
+-rw-r--r--   0        0        0     2611 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/domain_registration.py
+-rw-r--r--   0        0        0      654 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/groups.py
+-rw-r--r--   0        0        0     3439 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/models/record.py
+-rw-r--r--   0        0        0     7196 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/record.py
+-rw-r--r--   0        0        0     1882 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/utils/__init__.py
+-rw-r--r--   0        0        0     2642 2024-04-15 13:32:53.480219 cloudfloordns-0.1.3/cloudfloordns/utils/make_async.py
+-rw-r--r--   0        0        0      765 2024-04-15 13:32:53.484219 cloudfloordns-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3616 1970-01-01 00:00:00.000000 cloudfloordns-0.1.3/PKG-INFO
```

### Comparing `cloudfloordns-0.1.2/README.md` & `cloudfloordns-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.2/cloudfloordns/client.py` & `cloudfloordns-0.1.3/cloudfloordns/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,24 +2,27 @@
 import logging
 import os
 
 import requests
 from ratelimit import RateLimitException, limits, sleep_and_retry
 
 from .domain import Domains
+from .groups import Groups
 from .record import Records
+from .utils.make_async import make_methods_async
 
 DEFAULT_HEADERS = {
     "Accept": "application/json",
     "Content-Type": "application/json",
 }
 
 DEFAULT_BASE_URL = "https://apiv2.mtgsy.net/api/v1"
 
 
+@make_methods_async
 class BaseClient:
     def __init__(self, username=None, apikey=None, url=DEFAULT_BASE_URL) -> None:
         if not username:
             username = os.environ.get("CLOUDFLOOR_USERNAME", "").strip()
         if not username:
             raise Exception("username required")
 
@@ -84,7 +87,17 @@
 
 
 class Client(BaseClient):
     def __init__(self, username=None, apikey=None, url=DEFAULT_BASE_URL) -> None:
         super().__init__(username=username, apikey=apikey, url=url)
         self.records = Records(self)
         self.domains = Domains(self)
+        self.groups = Groups(self)
+
+    def yield_all_domains_records(self, zone_enabled=None):
+        domains = self.domains.list(zone_enabled=zone_enabled)
+        for d in domains:
+            records = self.records.list(d.domainname)
+            yield d, records
+
+    def all_domains_records(self, zone_enabled=None):
+        return dict(self.yield_all_domains_records(zone_enabled=zone_enabled))
```

### Comparing `cloudfloordns-0.1.2/cloudfloordns/domain.py` & `cloudfloordns-0.1.3/cloudfloordns/client/sync/domain.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,61 @@
 # from dataclasses import dataclass, field
-from typing import List
-
-from pydantic import BaseModel, Extra, Field, StringConstraints
-from typing_extensions import Annotated
+from cloudfloordns.models import Domain
 
 from .pool import POOL
 
 DEFAULT_PRIMARY_NS = "ns1.g02.cfdns.net"
 
 
-class Domain(BaseModel):
-    domainname: Annotated[str, StringConstraints(strip_whitespace=True)]
-
-    id: str = None
-    zone: str = None
-    registered: int = None
-    secondary: int = None
-    primary: int = None
-    group_ids: List[str] = Field(default_factory=list)
-
-    class Config:
-        populate_by_name = True
-        extra = Extra.allow
-
-    # def __eq__(self, __value: Record) -> bool:
-    #     if not isinstance(__value, Record):
-    #         return NotImplemented
-    #     fields1 = self.model_dump(exclude_unset=True)
-    #     fields2 = __value.model_dump(exclude_unset=True)
-    #     try:
-    #         return all(fields2[k] == v for k, v in fields1.items())
-    #     except Exception:
-    #         return False
-
-    def is_same(self, right: "Domain") -> bool:
-        """
-        This method check the identity (e.g. same id if defined, or same name/name+value)
-        """
-        if not isinstance(right, Domain):
-            return NotImplemented
-        return self.domainname == self.right
-
-
 class Domains:
     def __init__(self, client) -> None:
         self.client = client
 
     # def create(self, domain: str, record: Record, timeout=None):
     #     url = f"/dns/zone/{domain}/record"
     #     return self.client.post(
     #         url,
     #         data=record.model_dump(),
     #         timeout=timeout,
     #     )
 
-    # def update(self, domain: str, record_id: str, record: Record, timeout=None):
-    #     url = f"/dns/zone/{domain}/record/{record_id}"
-    #     return self.client.patch(
-    #         url,
-    #         data=record.model_dump(exclude_unset=True),
-    #         timeout=timeout,
-    #     )
+    def update(self, domain: "Domain", soa=None, timeout=None):
+        url = "/dns/zone"
+        data = domain.model_dump(exclude_unset=True)
+        if not soa:
+            soa = self.soa(domain)
+
+        data = domain.model_dump(exclude_unset=True)
+        soa_data = {
+            "master": soa["ns"],  # NS: primary name server
+            "retry": soa[
+                "retry"
+            ],  # Retry: How often secondaries attempt to fetch the zone if the first refresh fails
+            "refresh": soa[
+                "refresh"
+            ],  # Refresh:  How often secondaries should check if changes are made to the zone
+            "expire": soa[
+                "expire"
+            ],  # Expire: Secondaries will discard the zone if no refresh could be made within this interval.
+            "min": soa[
+                "minimum"
+            ],  #  Min TTL: default TTL for new records. Also determines how long negative records are cached (record not found)
+            "mbox": soa[
+                "mbox"
+            ],  # RP: Responsible person (email address with period instead of '@')
+            "ttl": soa[
+                "ttl"
+            ],  # SOA TTL: Number of seconds this zone may be cached before the source must be consulted again.
+        }
+        request_data = {**soa_data, **data}
+        return self.client.patch(
+            url,
+            data=request_data,
+            timeout=timeout,
+        )
 
     # def delete(self, domain: str, record_id: str, timeout=None):
     #     url = f"/dns/zone/{domain}/record/{record_id}"
     #     return self.client.delete(
     #         url,
     #         timeout=timeout,
     #     )
```

### Comparing `cloudfloordns-0.1.2/cloudfloordns/domain_registration.py` & `cloudfloordns-0.1.3/cloudfloordns/domain_registration.py`

 * *Files identical despite different names*

### Comparing `cloudfloordns-0.1.2/cloudfloordns/utils/__init__.py` & `cloudfloordns-0.1.3/cloudfloordns/utils/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-import logging
-import math
 import re
-import time
-from functools import wraps
-from threading import Lock
-
-from . import mail
 
 # import unidecode
 
 
 def slugify(text):
     # text = unidecode.unidecode(text)
     return re.sub(r"[\W_]+", "_", text.lower())
@@ -19,14 +12,23 @@
     keep = []
     for e in elements:
         if not any(comp(e, k) for k in keep):
             keep.append(e)
     return keep
 
 
+def groupby(iterable, key):
+    mapping = {}
+    for el in iterable:
+        k = key(el)
+        siblings = mapping.setdefault(k, [])
+        siblings.append(el)
+    return mapping
+
+
 # class OverFlowQueue:
 #     def __init__(self, size):
 #         if size < 1:
 #             raise Exception("Size of OverFlowQueue must greater or equal to 1")
 #         self._size = size
 #         self._elements = []
 #         self._mutex = Lock()
```

### Comparing `cloudfloordns-0.1.2/pyproject.toml` & `cloudfloordns-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloudfloordns"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["David Gallay <david.gallay@nagra.com>"]
 readme = "README.md"
 packages = [{include = "cloudfloordns", from="."}]
 
 # [tool.setuptools.dynamic]
 # version = {attr = "nagra_network_misc_utils.__version__"}
@@ -18,11 +18,12 @@
 # boto3 = {version = "^1.34.52", optional = true}
 
 # [tool.poetry.extras]
 # cli = [
 #     "boto3"
 # ]
 ratelimit = "^2.2.1"
+gevent = "^24.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cloudfloordns-0.1.2/PKG-INFO` & `cloudfloordns-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: cloudfloordns
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: David Gallay
 Author-email: david.gallay@nagra.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gevent (>=24.2.1,<25.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # README
```

