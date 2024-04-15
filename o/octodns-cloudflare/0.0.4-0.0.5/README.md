# Comparing `tmp/octodns-cloudflare-0.0.4.tar.gz` & `tmp/octodns_cloudflare-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octodns-cloudflare-0.0.4.tar", last modified: Thu Feb  8 16:09:03 2024, max compression
+gzip compressed data, was "octodns_cloudflare-0.0.5.tar", last modified: Mon Apr 15 14:24:27 2024, max compression
```

## Comparing `octodns-cloudflare-0.0.4.tar` & `octodns_cloudflare-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-02-08 16:09:03.011424 octodns-cloudflare-0.0.4/
--rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:28.000000 octodns-cloudflare-0.0.4/LICENSE
--rw-r--r--   0 ross       (501) staff       (20)     5557 2024-02-08 16:09:03.010427 octodns-cloudflare-0.0.4/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)     4502 2024-02-08 16:03:27.000000 octodns-cloudflare-0.0.4/README.md
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-02-08 16:09:03.001504 octodns-cloudflare-0.0.4/octodns_cloudflare/
--rw-r--r--   0 ross       (501) staff       (20)    39227 2024-02-08 16:08:53.000000 octodns-cloudflare-0.0.4/octodns_cloudflare/__init__.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-02-08 16:09:03.006775 octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/
--rw-r--r--   0 ross       (501) staff       (20)     5557 2024-02-08 16:09:02.000000 octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/PKG-INFO
--rw-r--r--   0 ross       (501) staff       (20)      323 2024-02-08 16:09:02.000000 octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/SOURCES.txt
--rw-r--r--   0 ross       (501) staff       (20)        1 2024-02-08 16:09:02.000000 octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/dependency_links.txt
--rw-r--r--   0 ross       (501) staff       (20)      246 2024-02-08 16:09:02.000000 octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/requires.txt
--rw-r--r--   0 ross       (501) staff       (20)       19 2024-02-08 16:09:02.000000 octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/top_level.txt
--rw-r--r--   0 ross       (501) staff       (20)      431 2023-11-29 21:54:17.000000 octodns-cloudflare-0.0.4/pyproject.toml
--rw-r--r--   0 ross       (501) staff       (20)       38 2024-02-08 16:09:03.011698 octodns-cloudflare-0.0.4/setup.cfg
--rwxr-xr-x   0 ross       (501) staff       (20)     1661 2023-11-13 15:49:01.000000 octodns-cloudflare-0.0.4/setup.py
-drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-02-08 16:09:03.005946 octodns-cloudflare-0.0.4/tests/
--rw-r--r--   0 ross       (501) staff       (20)    88014 2024-01-11 18:04:57.000000 octodns-cloudflare-0.0.4/tests/test_octodns_provider_cloudflare.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.327114 octodns_cloudflare-0.0.5/
+-rw-r--r--   0 ross       (501) staff       (20)     1129 2023-10-19 01:55:28.000000 octodns_cloudflare-0.0.5/LICENSE
+-rw-r--r--   0 ross       (501) staff       (20)     6709 2024-04-15 14:24:27.325736 octodns_cloudflare-0.0.5/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)     5654 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/README.md
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.307160 octodns_cloudflare-0.0.5/octodns_cloudflare/
+-rw-r--r--   0 ross       (501) staff       (20)    40769 2024-04-15 14:24:19.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/__init__.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.316381 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/
+-rw-r--r--   0 ross       (501) staff       (20)        6 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/__init__.py
+-rw-r--r--   0 ross       (501) staff       (20)     2632 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/proxycname.py
+-rw-r--r--   0 ross       (501) staff       (20)     1145 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.5/octodns_cloudflare/processor/ttl.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.320279 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/
+-rw-r--r--   0 ross       (501) staff       (20)     6709 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/PKG-INFO
+-rw-r--r--   0 ross       (501) staff       (20)      562 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/SOURCES.txt
+-rw-r--r--   0 ross       (501) staff       (20)        1 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/dependency_links.txt
+-rw-r--r--   0 ross       (501) staff       (20)      246 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/requires.txt
+-rw-r--r--   0 ross       (501) staff       (20)       19 2024-04-15 14:24:27.000000 octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/top_level.txt
+-rw-r--r--   0 ross       (501) staff       (20)      431 2023-11-29 21:54:17.000000 octodns_cloudflare-0.0.5/pyproject.toml
+-rw-r--r--   0 ross       (501) staff       (20)       38 2024-04-15 14:24:27.327378 octodns_cloudflare-0.0.5/setup.cfg
+-rwxr-xr-x   0 ross       (501) staff       (20)     1661 2024-03-21 02:14:57.000000 octodns_cloudflare-0.0.5/setup.py
+drwxr-xr-x   0 ross       (501) staff       (20)        0 2024-04-15 14:24:27.319384 octodns_cloudflare-0.0.5/tests/
+-rw-r--r--   0 ross       (501) staff       (20)    98587 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare.py
+-rw-r--r--   0 ross       (501) staff       (20)     4631 2024-04-15 14:07:25.000000 octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare_processor_proxycname.py
+-rw-r--r--   0 ross       (501) staff       (20)     1670 2024-03-20 21:28:12.000000 octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare_processor_ttl.py
```

### Comparing `octodns-cloudflare-0.0.4/LICENSE` & `octodns_cloudflare-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `octodns-cloudflare-0.0.4/PKG-INFO` & `octodns_cloudflare-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-cloudflare
-Version: 0.0.4
+Version: 0.0.5
 Summary:  Cloudflare provider for octoDNS
 Home-page: https://github.com/octodns/octodns-cloudflare
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: octodns>=0.9.20
 Requires-Dist: requests>=2.27.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
@@ -62,18 +62,20 @@
 
 ### Configuration
 
 ```yaml
 providers:
   cloudflare:
     class: octodns_cloudflare.CloudflareProvider
-    # Your Cloudflare account email address (required, optional if using token)
+    # Your Cloudflare account email address (not needed if using token)
+    # setting email along with an API Token will raise an error.
     email: env/CLOUDFLARE_EMAIL
     # The API Token or API Key.
-    # Required permissions for API Tokens are Zone:Read, DNS:Read and DNS:Key.
+    # Required permissions for API Tokens are Zone:Read, DNS:Read and DNS:Edit.
+    # Page Rules:Edit is required for managing Page Rules (URLFWD) records.
     token: env/CLOUDFLARE_TOKEN
     # Optional. Filter by account ID in environments where a token has access
     # across more than the permitted number of accounts allowed by Cloudflare.
     account_id: env/CLOUDFLARE_ACCOUNT_ID
     # Import CDN enabled records as CNAME to {}.cdn.cloudflare.net. Records
     # ending at .cdn.cloudflare.net. will be ignored when this provider is
     # not used as the source and the cdn option is enabled.
@@ -109,15 +111,15 @@
             #auto-ttl: true
     # with proxied=true, the TTL here will be ignored by CloudflareProvider
     ttl: 120
     type: A
     value: 1.2.3.4
 ```
 
-Note: All record types support "auto" ttl, which is effecitvely equivilent to 300s.
+Note: All record types support "auto" ttl, which is effectively equivalent to 300s.
 
 ```yaml
 name:
     octodns:
         cloudflare:
             auto-ttl: true
     # with proxied=true, the TTL here will be ignored by CloudflareProvider
@@ -138,17 +140,31 @@
 
 #### Dynamic
 
 CloudflareProvider does not support dynamic records.
 
 #### Required API Token Permissions
 
-Required Permissions for API Token are Zone:Read, DNS:Read, and DNS:Edit.
+Required Permissions for API Token are Zone:Read, DNS:Read, and DNS:Edit.  
+Page Rules:Edit is also required for managing Page Rules (URLFWD) records, otherwise an authentication error will be raised.
+
+**Important Note:** When using a CloudFlare token you should **NOT** provide an email address or you will receive an error.
+
+An example when using Page Rules (URLFWD) records -
+
+![Cloudflare API token config example screenshot](./docs/assets/cf_token_example.PNG)
 
 #### TTL
 
 Cloudflare has a different minimum TTL for enterprise and non-enterprise zones. See the [documentation](https://developers.cloudflare.com/dns/manage-dns-records/reference/ttl) for more information.
-In the past the CloudflareProvider had a fixed minimum TTL set to 120 seconds and for backwards compatbility this is the current default.
+In the past the CloudflareProvider had a fixed minimum TTL set to 120 seconds and for backwards compatibility this is the current default.
+
+### Processors
+
+| Processor | Description |
+|--|--|
+| [ProxyCNAME](/octodns_cloudflare/processor/proxycname.py) | Allows Cloudflare proxied records to be used on other providers without exposing the proxied record value. Points other providers to the relevant `.cdn.cloudflare.net` subdomain. Useful to allow split authority with a secondary provider while still retaining Cloudflare benefits for certain records. |
+| [TtlToProxy ](/octodns_cloudflare/processor/ttl.py) | Ensure Cloudflare's proxy status is setup depending on the TTL set for the record. This can be helpful for `octodns_bind.ZoneFileSource` or the like. |
 
 ### Developement
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
```

### Comparing `octodns-cloudflare-0.0.4/README.md` & `octodns_cloudflare-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 
 ### Configuration
 
 ```yaml
 providers:
   cloudflare:
     class: octodns_cloudflare.CloudflareProvider
-    # Your Cloudflare account email address (required, optional if using token)
+    # Your Cloudflare account email address (not needed if using token)
+    # setting email along with an API Token will raise an error.
     email: env/CLOUDFLARE_EMAIL
     # The API Token or API Key.
-    # Required permissions for API Tokens are Zone:Read, DNS:Read and DNS:Key.
+    # Required permissions for API Tokens are Zone:Read, DNS:Read and DNS:Edit.
+    # Page Rules:Edit is required for managing Page Rules (URLFWD) records.
     token: env/CLOUDFLARE_TOKEN
     # Optional. Filter by account ID in environments where a token has access
     # across more than the permitted number of accounts allowed by Cloudflare.
     account_id: env/CLOUDFLARE_ACCOUNT_ID
     # Import CDN enabled records as CNAME to {}.cdn.cloudflare.net. Records
     # ending at .cdn.cloudflare.net. will be ignored when this provider is
     # not used as the source and the cdn option is enabled.
@@ -79,15 +81,15 @@
             #auto-ttl: true
     # with proxied=true, the TTL here will be ignored by CloudflareProvider
     ttl: 120
     type: A
     value: 1.2.3.4
 ```
 
-Note: All record types support "auto" ttl, which is effecitvely equivilent to 300s.
+Note: All record types support "auto" ttl, which is effectively equivalent to 300s.
 
 ```yaml
 name:
     octodns:
         cloudflare:
             auto-ttl: true
     # with proxied=true, the TTL here will be ignored by CloudflareProvider
@@ -108,17 +110,31 @@
 
 #### Dynamic
 
 CloudflareProvider does not support dynamic records.
 
 #### Required API Token Permissions
 
-Required Permissions for API Token are Zone:Read, DNS:Read, and DNS:Edit.
+Required Permissions for API Token are Zone:Read, DNS:Read, and DNS:Edit.  
+Page Rules:Edit is also required for managing Page Rules (URLFWD) records, otherwise an authentication error will be raised.
+
+**Important Note:** When using a CloudFlare token you should **NOT** provide an email address or you will receive an error.
+
+An example when using Page Rules (URLFWD) records -
+
+![Cloudflare API token config example screenshot](./docs/assets/cf_token_example.PNG)
 
 #### TTL
 
 Cloudflare has a different minimum TTL for enterprise and non-enterprise zones. See the [documentation](https://developers.cloudflare.com/dns/manage-dns-records/reference/ttl) for more information.
-In the past the CloudflareProvider had a fixed minimum TTL set to 120 seconds and for backwards compatbility this is the current default.
+In the past the CloudflareProvider had a fixed minimum TTL set to 120 seconds and for backwards compatibility this is the current default.
+
+### Processors
+
+| Processor | Description |
+|--|--|
+| [ProxyCNAME](/octodns_cloudflare/processor/proxycname.py) | Allows Cloudflare proxied records to be used on other providers without exposing the proxied record value. Points other providers to the relevant `.cdn.cloudflare.net` subdomain. Useful to allow split authority with a secondary provider while still retaining Cloudflare benefits for certain records. |
+| [TtlToProxy ](/octodns_cloudflare/processor/ttl.py) | Ensure Cloudflare's proxy status is setup depending on the TTL set for the record. This can be helpful for `octodns_bind.ZoneFileSource` or the like. |
 
 ### Developement
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
```

### Comparing `octodns-cloudflare-0.0.4/octodns_cloudflare/__init__.py` & `octodns_cloudflare-0.0.5/octodns_cloudflare/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from octodns import __VERSION__ as octodns_version
 from octodns.idna import IdnaDict
 from octodns.provider import ProviderException, SupportsException
 from octodns.provider.base import BaseProvider
 from octodns.record import Create, Record, Update
 
 # TODO: remove __VERSION__ with the next major version release
-__version__ = __VERSION__ = '0.0.4'
+__version__ = __VERSION__ = '0.0.5'
 
 
 class CloudflareError(ProviderException):
     def __init__(self, data):
         try:
             message = data['errors'][0]['message']
         except (IndexError, KeyError, TypeError):
@@ -270,17 +270,17 @@
 
     def _data_for_MX(self, _type, records):
         values = []
         for r in records:
             values.append(
                 {
                     'preference': r['priority'],
-                    'exchange': f'{r["content"]}.'
-                    if r['content'] != '.'
-                    else '.',
+                    'exchange': (
+                        f'{r["content"]}.' if r['content'] != '.' else '.'
+                    ),
                 }
             )
         return {
             'ttl': self._ttl_data(records[0]['ttl']),
             'type': _type,
             'values': values,
         }
@@ -444,14 +444,30 @@
             record._octodns['cloudflare'] = {'proxied': True, 'auto-ttl': True}
         elif auto_ttl:
             # auto-ttl can still be set on any record type, signaled by a ttl=1,
             # even if proxied is false.
             self.log.debug('_record_for: auto-ttl=True')
             record._octodns['cloudflare'] = {'auto-ttl': True}
 
+        # update record comment
+        if records[0].get('comment'):
+            try:
+                record._octodns['cloudflare']['comment'] = records[0]['comment']
+            except KeyError:
+                record._octodns['cloudflare'] = {
+                    'comment': records[0]['comment']
+                }
+
+        # update record tags
+        if records[0].get('tags'):
+            try:
+                record._octodns['cloudflare']['tags'] = records[0]['tags']
+            except KeyError:
+                record._octodns['cloudflare'] = {'tags': records[0]['tags']}
+
         return record
 
     def list_zones(self):
         return sorted(self.zones.keys())
 
     def populate(self, zone, target=False, lenient=False):
         self.log.debug(
@@ -724,14 +740,22 @@
         'This tests if it is strictly auto-ttl and not proxied'
         return (
             not self._record_is_proxied(record)
             and not self.cdn
             and record._octodns.get('cloudflare', {}).get('auto-ttl', False)
         )
 
+    def _record_comment(self, record):
+        'Returns record comment'
+        return record._octodns.get('cloudflare', {}).get('comment', '')
+
+    def _record_tags(self, record):
+        'Returns nonduplicate record tags'
+        return set(record._octodns.get('cloudflare', {}).get('tags', []))
+
     def _gen_data(self, record):
         name = record.fqdn[:-1]
         _type = record._type
         proxied = self._record_is_proxied(record)
         if proxied or self._record_is_just_auto_ttl(record):
             # proxied implies auto-ttl, and auto-ttl can be enabled on its own,
             # when either is the case we tell Cloudflare with ttl=1
@@ -751,14 +775,20 @@
             contents_for = getattr(self, f'_contents_for_{_type}')
             for content in contents_for(record):
                 content.update({'name': name, 'type': _type, 'ttl': ttl})
 
                 if _type in _PROXIABLE_RECORD_TYPES:
                     content.update({'proxied': self._record_is_proxied(record)})
 
+                if self._record_comment(record):
+                    content.update({'comment': self._record_comment(record)})
+
+                if self._record_tags(record):
+                    content.update({'tags': list(self._record_tags(record))})
+
                 yield content
 
     def _gen_key(self, data):
         # Note that most CF record data has a `content` field the value of
         # which is a unique/hashable string for the record's. It includes all
         # the "value" bits, but not the secondary stuff like TTL's. E.g.  for
         # an A it'll include the value, for a CAA it'll include the flags, tag,
@@ -1061,8 +1091,18 @@
                 != self._record_is_proxied(desired_record)
             ) or (
                 self._record_is_just_auto_ttl(existing_record)
                 != self._record_is_just_auto_ttl(desired_record)
             ):
                 extra_changes.append(Update(existing_record, desired_record))
 
+            if self._record_comment(existing_record) != self._record_comment(
+                desired_record
+            ):
+                extra_changes.append(Update(existing_record, desired_record))
+
+            if self._record_tags(existing_record) != self._record_tags(
+                desired_record
+            ):
+                extra_changes.append(Update(existing_record, desired_record))
+
         return extra_changes
```

### Comparing `octodns-cloudflare-0.0.4/octodns_cloudflare.egg-info/PKG-INFO` & `octodns_cloudflare-0.0.5/octodns_cloudflare.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octodns-cloudflare
-Version: 0.0.4
+Version: 0.0.5
 Summary:  Cloudflare provider for octoDNS
 Home-page: https://github.com/octodns/octodns-cloudflare
 Author: Ross McFarland
 Author-email: rwmcfa1@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -12,15 +12,15 @@
 Requires-Dist: octodns>=0.9.20
 Requires-Dist: requests>=2.27.0
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-network; extra == "dev"
 Requires-Dist: requests_mock; extra == "dev"
-Requires-Dist: black<24.0.0,>=23.1.0; extra == "dev"
+Requires-Dist: black<25.0.0,>=24.3.0; extra == "dev"
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: isort>=5.11.5; extra == "dev"
 Requires-Dist: pyflakes>=2.2.0; extra == "dev"
 Requires-Dist: readme_renderer[md]>=26.0; extra == "dev"
 Requires-Dist: twine>=3.4.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
@@ -62,18 +62,20 @@
 
 ### Configuration
 
 ```yaml
 providers:
   cloudflare:
     class: octodns_cloudflare.CloudflareProvider
-    # Your Cloudflare account email address (required, optional if using token)
+    # Your Cloudflare account email address (not needed if using token)
+    # setting email along with an API Token will raise an error.
     email: env/CLOUDFLARE_EMAIL
     # The API Token or API Key.
-    # Required permissions for API Tokens are Zone:Read, DNS:Read and DNS:Key.
+    # Required permissions for API Tokens are Zone:Read, DNS:Read and DNS:Edit.
+    # Page Rules:Edit is required for managing Page Rules (URLFWD) records.
     token: env/CLOUDFLARE_TOKEN
     # Optional. Filter by account ID in environments where a token has access
     # across more than the permitted number of accounts allowed by Cloudflare.
     account_id: env/CLOUDFLARE_ACCOUNT_ID
     # Import CDN enabled records as CNAME to {}.cdn.cloudflare.net. Records
     # ending at .cdn.cloudflare.net. will be ignored when this provider is
     # not used as the source and the cdn option is enabled.
@@ -109,15 +111,15 @@
             #auto-ttl: true
     # with proxied=true, the TTL here will be ignored by CloudflareProvider
     ttl: 120
     type: A
     value: 1.2.3.4
 ```
 
-Note: All record types support "auto" ttl, which is effecitvely equivilent to 300s.
+Note: All record types support "auto" ttl, which is effectively equivalent to 300s.
 
 ```yaml
 name:
     octodns:
         cloudflare:
             auto-ttl: true
     # with proxied=true, the TTL here will be ignored by CloudflareProvider
@@ -138,17 +140,31 @@
 
 #### Dynamic
 
 CloudflareProvider does not support dynamic records.
 
 #### Required API Token Permissions
 
-Required Permissions for API Token are Zone:Read, DNS:Read, and DNS:Edit.
+Required Permissions for API Token are Zone:Read, DNS:Read, and DNS:Edit.  
+Page Rules:Edit is also required for managing Page Rules (URLFWD) records, otherwise an authentication error will be raised.
+
+**Important Note:** When using a CloudFlare token you should **NOT** provide an email address or you will receive an error.
+
+An example when using Page Rules (URLFWD) records -
+
+![Cloudflare API token config example screenshot](./docs/assets/cf_token_example.PNG)
 
 #### TTL
 
 Cloudflare has a different minimum TTL for enterprise and non-enterprise zones. See the [documentation](https://developers.cloudflare.com/dns/manage-dns-records/reference/ttl) for more information.
-In the past the CloudflareProvider had a fixed minimum TTL set to 120 seconds and for backwards compatbility this is the current default.
+In the past the CloudflareProvider had a fixed minimum TTL set to 120 seconds and for backwards compatibility this is the current default.
+
+### Processors
+
+| Processor | Description |
+|--|--|
+| [ProxyCNAME](/octodns_cloudflare/processor/proxycname.py) | Allows Cloudflare proxied records to be used on other providers without exposing the proxied record value. Points other providers to the relevant `.cdn.cloudflare.net` subdomain. Useful to allow split authority with a secondary provider while still retaining Cloudflare benefits for certain records. |
+| [TtlToProxy ](/octodns_cloudflare/processor/ttl.py) | Ensure Cloudflare's proxy status is setup depending on the TTL set for the record. This can be helpful for `octodns_bind.ZoneFileSource` or the like. |
 
 ### Developement
 
 See the [/script/](/script/) directory for some tools to help with the development process. They generally follow the [Script to rule them all](https://github.com/github/scripts-to-rule-them-all) pattern. Most useful is `./script/bootstrap` which will create a venv and install both the runtime and development related requirements. It will also hook up a pre-commit hook that covers most of what's run by CI.
```

### Comparing `octodns-cloudflare-0.0.4/setup.py` & `octodns_cloudflare-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     extras_require={
         'dev': tests_require
         + (
             # we need to manually/explicitely bump major versions as they're
             # likely to result in formatting changes that should happen in their
             # own PR. This will basically happen yearly
             # https://black.readthedocs.io/en/stable/the_black_code_style/index.html#stability-policy
-            'black>=23.1.0,<24.0.0',
+            'black>=24.3.0,<25.0.0',
             'build>=0.7.0',
             'isort>=5.11.5',
             'pyflakes>=2.2.0',
             'readme_renderer[md]>=26.0',
             'twine>=3.4.2',
         ),
         'test': tests_require,
```

### Comparing `octodns-cloudflare-0.0.4/tests/test_octodns_provider_cloudflare.py` & `octodns_cloudflare-0.0.5/tests/test_octodns_provider_cloudflare.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,5446 +56,6107 @@
 00000370: 3d20 6175 746f 5f74 746c 0a20 2020 2065  = auto_ttl.    e
 00000380: 7863 6570 7420 4b65 7945 7272 6f72 3a0a  xcept KeyError:.
 00000390: 2020 2020 2020 2020 7265 636f 7264 2e5f          record._
 000003a0: 6f63 746f 646e 735b 2763 6c6f 7564 666c  octodns['cloudfl
 000003b0: 6172 6527 5d20 3d20 7b27 6175 746f 2d74  are'] = {'auto-t
 000003c0: 746c 273a 2061 7574 6f5f 7474 6c7d 0a0a  tl': auto_ttl}..
 000003d0: 2020 2020 7265 7475 726e 2072 6563 6f72      return recor
-000003e0: 640a 0a0a 636c 6173 7320 5465 7374 436c  d...class TestCl
-000003f0: 6f75 6466 6c61 7265 5072 6f76 6964 6572  oudflareProvider
-00000400: 2854 6573 7443 6173 6529 3a0a 2020 2020  (TestCase):.    
-00000410: 6578 7065 6374 6564 203d 205a 6f6e 6528  expected = Zone(
-00000420: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-00000430: 5d29 0a20 2020 2073 6f75 7263 6520 3d20  ]).    source = 
-00000440: 5961 6d6c 5072 6f76 6964 6572 2827 7465  YamlProvider('te
-00000450: 7374 272c 206a 6f69 6e28 6469 726e 616d  st', join(dirnam
-00000460: 6528 5f5f 6669 6c65 5f5f 292c 2027 636f  e(__file__), 'co
-00000470: 6e66 6967 2729 290a 2020 2020 736f 7572  nfig')).    sour
-00000480: 6365 2e70 6f70 756c 6174 6528 6578 7065  ce.populate(expe
-00000490: 6374 6564 290a 0a20 2020 2023 204f 7572  cted)..    # Our
-000004a0: 2074 6573 7420 7375 6974 6520 6469 6666   test suite diff
-000004b0: 6572 7320 6120 6269 742c 2061 6464 206f  ers a bit, add o
-000004c0: 7572 204e 5320 616e 6420 7265 6d6f 7665  ur NS and remove
-000004d0: 2074 6865 2073 696d 706c 6520 6f6e 650a   the simple one.
-000004e0: 2020 2020 6578 7065 6374 6564 2e61 6464      expected.add
-000004f0: 5f72 6563 6f72 6428 0a20 2020 2020 2020  _record(.       
-00000500: 2052 6563 6f72 642e 6e65 7728 0a20 2020   Record.new(.   
-00000510: 2020 2020 2020 2020 2065 7870 6563 7465           expecte
-00000520: 642c 0a20 2020 2020 2020 2020 2020 2027  d,.            '
-00000530: 756e 6465 7227 2c0a 2020 2020 2020 2020  under',.        
-00000540: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00000550: 2020 2020 2020 2774 746c 273a 2033 3630        'ttl': 360
-00000560: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00000570: 2020 2027 7479 7065 273a 2027 4e53 272c     'type': 'NS',
-00000580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000590: 2027 7661 6c75 6573 273a 205b 276e 7331   'values': ['ns1
-000005a0: 2e75 6e69 742e 7465 7374 732e 272c 2027  .unit.tests.', '
-000005b0: 6e73 322e 756e 6974 2e74 6573 7473 2e27  ns2.unit.tests.'
-000005c0: 5d2c 0a20 2020 2020 2020 2020 2020 207d  ],.            }
-000005d0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-000005e0: 290a 2020 2020 666f 7220 7265 636f 7264  ).    for record
-000005f0: 2069 6e20 6c69 7374 2865 7870 6563 7465   in list(expecte
-00000600: 642e 7265 636f 7264 7329 3a0a 2020 2020  d.records):.    
-00000610: 2020 2020 6966 2072 6563 6f72 642e 6e61      if record.na
-00000620: 6d65 203d 3d20 2773 7562 2720 616e 6420  me == 'sub' and 
-00000630: 7265 636f 7264 2e5f 7479 7065 203d 3d20  record._type == 
-00000640: 274e 5327 3a0a 2020 2020 2020 2020 2020  'NS':.          
-00000650: 2020 6578 7065 6374 6564 2e5f 7265 6d6f    expected._remo
-00000660: 7665 5f72 6563 6f72 6428 7265 636f 7264  ve_record(record
-00000670: 290a 2020 2020 2020 2020 2020 2020 6272  ).            br
-00000680: 6561 6b0a 0a20 2020 2065 6d70 7479 203d  eak..    empty =
-00000690: 207b 2772 6573 756c 7427 3a20 5b5d 2c20   {'result': [], 
-000006a0: 2772 6573 756c 745f 696e 666f 273a 207b  'result_info': {
-000006b0: 2763 6f75 6e74 273a 2030 2c20 2770 6572  'count': 0, 'per
-000006c0: 5f70 6167 6527 3a20 307d 7d0a 0a20 2020  _page': 0}}..   
-000006d0: 2064 6566 2074 6573 745f 706f 7075 6c61   def test_popula
-000006e0: 7465 2873 656c 6629 3a0a 2020 2020 2020  te(self):.      
-000006f0: 2020 7072 6f76 6964 6572 203d 2043 6c6f    provider = Clo
-00000700: 7564 666c 6172 6550 726f 7669 6465 7228  udflareProvider(
-00000710: 2774 6573 7427 2c20 2765 6d61 696c 272c  'test', 'email',
-00000720: 2027 746f 6b65 6e27 2c20 7265 7472 795f   'token', retry_
-00000730: 7065 7269 6f64 3d30 290a 0a20 2020 2020  period=0)..     
-00000740: 2020 2023 2042 6164 2072 6571 7565 7374     # Bad request
-00000750: 730a 2020 2020 2020 2020 7769 7468 2072  s.        with r
-00000760: 6571 7565 7374 735f 6d6f 636b 2829 2061  equests_mock() a
-00000770: 7320 6d6f 636b 3a0a 2020 2020 2020 2020  s mock:.        
-00000780: 2020 2020 6d6f 636b 2e67 6574 280a 2020      mock.get(.  
-00000790: 2020 2020 2020 2020 2020 2020 2020 414e                AN
-000007a0: 592c 0a20 2020 2020 2020 2020 2020 2020  Y,.             
-000007b0: 2020 2073 7461 7475 735f 636f 6465 3d34     status_code=4
-000007c0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-000007d0: 2020 2020 7465 7874 3d27 7b22 7375 6363      text='{"succ
-000007e0: 6573 7322 3a66 616c 7365 2c22 6572 726f  ess":false,"erro
-000007f0: 7273 223a 5b7b 2263 6f64 6522 3a31 3130  rs":[{"code":110
-00000800: 312c 270a 2020 2020 2020 2020 2020 2020  1,'.            
-00000810: 2020 2020 2722 6d65 7373 6167 6522 3a22      '"message":"
-00000820: 7265 7175 6573 7420 7761 7320 696e 7661  request was inva
-00000830: 6c69 6422 7d5d 2c27 0a20 2020 2020 2020  lid"}],'.       
-00000840: 2020 2020 2020 2020 2027 226d 6573 7361           '"messa
-00000850: 6765 7322 3a5b 5d2c 2272 6573 756c 7422  ges":[],"result"
-00000860: 3a6e 756c 6c7d 272c 0a20 2020 2020 2020  :null}',.       
-00000870: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00000880: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
-00000890: 7365 7274 5261 6973 6573 2845 7863 6570  sertRaises(Excep
-000008a0: 7469 6f6e 2920 6173 2063 7478 3a0a 2020  tion) as ctx:.  
-000008b0: 2020 2020 2020 2020 2020 2020 2020 7a6f                zo
-000008c0: 6e65 203d 205a 6f6e 6528 2775 6e69 742e  ne = Zone('unit.
-000008d0: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
-000008e0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
-000008f0: 7669 6465 722e 706f 7075 6c61 7465 287a  vider.populate(z
-00000900: 6f6e 6529 0a0a 2020 2020 2020 2020 2020  one)..          
-00000910: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00000920: 616c 2827 436c 6f75 6466 6c61 7265 4572  al('CloudflareEr
-00000930: 726f 7227 2c20 7479 7065 2863 7478 2e65  ror', type(ctx.e
-00000940: 7863 6570 7469 6f6e 292e 5f5f 6e61 6d65  xception).__name
-00000950: 5f5f 290a 2020 2020 2020 2020 2020 2020  __).            
-00000960: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00000970: 2827 7265 7175 6573 7420 7761 7320 696e  ('request was in
-00000980: 7661 6c69 6427 2c20 7374 7228 6374 782e  valid', str(ctx.
-00000990: 6578 6365 7074 696f 6e29 290a 0a20 2020  exception))..   
-000009a0: 2020 2020 2023 2042 6164 2061 7574 680a       # Bad auth.
-000009b0: 2020 2020 2020 2020 7769 7468 2072 6571          with req
-000009c0: 7565 7374 735f 6d6f 636b 2829 2061 7320  uests_mock() as 
-000009d0: 6d6f 636b 3a0a 2020 2020 2020 2020 2020  mock:.          
-000009e0: 2020 6d6f 636b 2e67 6574 280a 2020 2020    mock.get(.    
-000009f0: 2020 2020 2020 2020 2020 2020 414e 592c              ANY,
-00000a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000a10: 2073 7461 7475 735f 636f 6465 3d34 3033   status_code=403
-00000a20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000a30: 2020 7465 7874 3d27 7b22 7375 6363 6573    text='{"succes
-00000a40: 7322 3a66 616c 7365 2c22 6572 726f 7273  s":false,"errors
-00000a50: 223a 5b7b 2263 6f64 6522 3a39 3130 332c  ":[{"code":9103,
-00000a60: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-00000a70: 2020 2722 6d65 7373 6167 6522 3a22 556e    '"message":"Un
-00000a80: 6b6e 6f77 6e20 582d 4175 7468 2d4b 6579  known X-Auth-Key
-00000a90: 206f 7220 582d 4175 7468 2d45 6d61 696c   or X-Auth-Email
-00000aa0: 227d 5d2c 270a 2020 2020 2020 2020 2020  "}],'.          
-00000ab0: 2020 2020 2020 2722 6d65 7373 6167 6573        '"messages
-00000ac0: 223a 5b5d 2c22 7265 7375 6c74 223a 6e75  ":[],"result":nu
-00000ad0: 6c6c 7d27 2c0a 2020 2020 2020 2020 2020  ll}',.          
-00000ae0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00000af0: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
-00000b00: 7452 6169 7365 7328 4578 6365 7074 696f  tRaises(Exceptio
-00000b10: 6e29 2061 7320 6374 783a 0a20 2020 2020  n) as ctx:.     
-00000b20: 2020 2020 2020 2020 2020 207a 6f6e 6520             zone 
-00000b30: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
-00000b40: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
-00000b50: 2020 2020 2020 2020 2020 7072 6f76 6964            provid
-00000b60: 6572 2e70 6f70 756c 6174 6528 7a6f 6e65  er.populate(zone
-00000b70: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00000b80: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 2743 6c6f 7564 666c 6172 6541 7574 6865  'CloudflareAuthe
-00000bb0: 6e74 6963 6174 696f 6e45 7272 6f72 272c  nticationError',
-00000bc0: 2074 7970 6528 6374 782e 6578 6365 7074   type(ctx.except
-00000bd0: 696f 6e29 2e5f 5f6e 616d 655f 5f0a 2020  ion).__name__.  
-00000be0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00000bf0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00000c00: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-00000c10: 2020 2020 2020 2020 2020 2755 6e6b 6e6f            'Unkno
-00000c20: 776e 2058 2d41 7574 682d 4b65 7920 6f72  wn X-Auth-Key or
-00000c30: 2058 2d41 7574 682d 456d 6169 6c27 2c20   X-Auth-Email', 
-00000c40: 7374 7228 6374 782e 6578 6365 7074 696f  str(ctx.exceptio
-00000c50: 6e29 0a20 2020 2020 2020 2020 2020 2029  n).            )
-00000c60: 0a0a 2020 2020 2020 2020 2320 4261 6420  ..        # Bad 
-00000c70: 6175 7468 2c20 756e 6b6e 6f77 6e20 7265  auth, unknown re
-00000c80: 7370 0a20 2020 2020 2020 2077 6974 6820  sp.        with 
-00000c90: 7265 7175 6573 7473 5f6d 6f63 6b28 2920  requests_mock() 
-00000ca0: 6173 206d 6f63 6b3a 0a20 2020 2020 2020  as mock:.       
-00000cb0: 2020 2020 206d 6f63 6b2e 6765 7428 414e       mock.get(AN
-00000cc0: 592c 2073 7461 7475 735f 636f 6465 3d34  Y, status_code=4
-00000cd0: 3033 2c20 7465 7874 3d27 7b7d 2729 0a0a  03, text='{}')..
-00000ce0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00000cf0: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
-00000d00: 6573 2845 7863 6570 7469 6f6e 2920 6173  es(Exception) as
-00000d10: 2063 7478 3a0a 2020 2020 2020 2020 2020   ctx:.          
-00000d20: 2020 2020 2020 7a6f 6e65 203d 205a 6f6e        zone = Zon
-00000d30: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
-00000d40: 205b 5d29 0a20 2020 2020 2020 2020 2020   []).           
-00000d50: 2020 2020 2070 726f 7669 6465 722e 706f       provider.po
-00000d60: 7075 6c61 7465 287a 6f6e 6529 0a20 2020  pulate(zone).   
-00000d70: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-00000d80: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-00000d90: 2020 2020 2020 2020 2020 2027 436c 6f75             'Clou
-00000da0: 6466 6c61 7265 4175 7468 656e 7469 6361  dflareAuthentica
-00000db0: 7469 6f6e 4572 726f 7227 2c20 7479 7065  tionError', type
-00000dc0: 2863 7478 2e65 7863 6570 7469 6f6e 292e  (ctx.exception).
-00000dd0: 5f5f 6e61 6d65 5f5f 0a20 2020 2020 2020  __name__.       
-00000de0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00000df0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-00000e00: 7561 6c28 2743 6c6f 7564 666c 6172 6520  ual('Cloudflare 
-00000e10: 6572 726f 7227 2c20 7374 7228 6374 782e  error', str(ctx.
-00000e20: 6578 6365 7074 696f 6e29 290a 0a20 2020  exception))..   
-00000e30: 2020 2020 2023 2047 656e 6572 616c 2065       # General e
-00000e40: 7272 6f72 0a20 2020 2020 2020 2077 6974  rror.        wit
-00000e50: 6820 7265 7175 6573 7473 5f6d 6f63 6b28  h requests_mock(
-00000e60: 2920 6173 206d 6f63 6b3a 0a20 2020 2020  ) as mock:.     
-00000e70: 2020 2020 2020 206d 6f63 6b2e 6765 7428         mock.get(
-00000e80: 414e 592c 2073 7461 7475 735f 636f 6465  ANY, status_code
-00000e90: 3d35 3032 2c20 7465 7874 3d27 5468 696e  =502, text='Thin
-00000ea0: 6773 2063 6175 6768 7420 6669 7265 2729  gs caught fire')
-00000eb0: 0a0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
-00000ec0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-00000ed0: 6973 6573 2848 5454 5045 7272 6f72 2920  ises(HTTPError) 
-00000ee0: 6173 2063 7478 3a0a 2020 2020 2020 2020  as ctx:.        
-00000ef0: 2020 2020 2020 2020 7a6f 6e65 203d 205a          zone = Z
-00000f00: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
-00000f10: 272c 205b 5d29 0a20 2020 2020 2020 2020  ', []).         
-00000f20: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00000f30: 706f 7075 6c61 7465 287a 6f6e 6529 0a20  populate(zone). 
-00000f40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00000f50: 6173 7365 7274 4571 7561 6c28 3530 322c  assertEqual(502,
-00000f60: 2063 7478 2e65 7863 6570 7469 6f6e 2e72   ctx.exception.r
-00000f70: 6573 706f 6e73 652e 7374 6174 7573 5f63  esponse.status_c
-00000f80: 6f64 6529 0a0a 2020 2020 2020 2020 2320  ode)..        # 
-00000f90: 5261 7465 204c 696d 6974 2065 7272 6f72  Rate Limit error
-00000fa0: 0a20 2020 2020 2020 2077 6974 6820 7265  .        with re
-00000fb0: 7175 6573 7473 5f6d 6f63 6b28 2920 6173  quests_mock() as
-00000fc0: 206d 6f63 6b3a 0a20 2020 2020 2020 2020   mock:.         
-00000fd0: 2020 206d 6f63 6b2e 6765 7428 0a20 2020     mock.get(.   
-00000fe0: 2020 2020 2020 2020 2020 2020 2041 4e59               ANY
-00000ff0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001000: 2020 7374 6174 7573 5f63 6f64 653d 3432    status_code=42
-00001010: 392c 0a20 2020 2020 2020 2020 2020 2020  9,.             
-00001020: 2020 2074 6578 743d 277b 2273 7563 6365     text='{"succe
-00001030: 7373 223a 6661 6c73 652c 2265 7272 6f72  ss":false,"error
-00001040: 7322 3a5b 7b22 636f 6465 223a 3130 3130  s":[{"code":1010
-00001050: 302c 270a 2020 2020 2020 2020 2020 2020  0,'.            
-00001060: 2020 2020 2722 6d65 7373 6167 6522 3a22      '"message":"
-00001070: 4d6f 7265 2074 6861 6e20 3132 3030 2072  More than 1200 r
-00001080: 6571 7565 7374 7320 7065 7220 3330 3020  equests per 300 
-00001090: 7365 636f 6e64 7320 270a 2020 2020 2020  seconds '.      
-000010a0: 2020 2020 2020 2020 2020 2772 6561 6368            'reach
-000010b0: 6564 2e20 506c 6561 7365 2077 6169 7420  ed. Please wait 
-000010c0: 616e 6420 636f 6e73 6964 6572 2074 6872  and consider thr
-000010d0: 6f74 746c 696e 6720 796f 7572 2027 0a20  ottling your '. 
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000010f0: 7265 7175 6573 7420 7370 6565 6422 7d5d  request speed"}]
-00001100: 2c22 6d65 7373 6167 6573 223a 5b5d 2c22  ,"messages":[],"
-00001110: 7265 7375 6c74 223a 6e75 6c6c 7d27 2c0a  result":null}',.
-00001120: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00001130: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00001140: 7365 6c66 2e61 7373 6572 7452 6169 7365  self.assertRaise
-00001150: 7328 4578 6365 7074 696f 6e29 2061 7320  s(Exception) as 
-00001160: 6374 783a 0a20 2020 2020 2020 2020 2020  ctx:.           
-00001170: 2020 2020 207a 6f6e 6520 3d20 5a6f 6e65       zone = Zone
-00001180: 2827 756e 6974 2e74 6573 7473 2e27 2c20  ('unit.tests.', 
-00001190: 5b5d 290a 2020 2020 2020 2020 2020 2020  []).            
-000011a0: 2020 2020 7072 6f76 6964 6572 2e70 6f70      provider.pop
-000011b0: 756c 6174 6528 7a6f 6e65 290a 0a20 2020  ulate(zone)..   
-000011c0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000011d0: 7365 7274 4571 7561 6c28 0a20 2020 2020  sertEqual(.     
-000011e0: 2020 2020 2020 2020 2020 2027 436c 6f75             'Clou
-000011f0: 6466 6c61 7265 5261 7465 4c69 6d69 7445  dflareRateLimitE
-00001200: 7272 6f72 272c 2074 7970 6528 6374 782e  rror', type(ctx.
-00001210: 6578 6365 7074 696f 6e29 2e5f 5f6e 616d  exception).__nam
-00001220: 655f 5f0a 2020 2020 2020 2020 2020 2020  e__.            
-00001230: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00001240: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 274d 6f72 6520 7468 616e 2031 3230 3020  'More than 1200 
-00001270: 7265 7175 6573 7473 2070 6572 2033 3030  requests per 300
-00001280: 2073 6563 6f6e 6473 2027 0a20 2020 2020   seconds '.     
-00001290: 2020 2020 2020 2020 2020 2027 7265 6163             'reac
-000012a0: 6865 642e 2050 6c65 6173 6520 7761 6974  hed. Please wait
-000012b0: 2061 6e64 2063 6f6e 7369 6465 7220 7468   and consider th
-000012c0: 726f 7474 6c69 6e67 2027 0a20 2020 2020  rottling '.     
-000012d0: 2020 2020 2020 2020 2020 2027 796f 7572             'your
-000012e0: 2072 6571 7565 7374 2073 7065 6564 272c   request speed',
-000012f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001300: 2073 7472 2863 7478 2e65 7863 6570 7469   str(ctx.excepti
-00001310: 6f6e 292c 0a20 2020 2020 2020 2020 2020  on),.           
-00001320: 2029 0a0a 2020 2020 2020 2020 2320 5261   )..        # Ra
-00001330: 7465 204c 696d 6974 2065 7272 6f72 2c20  te Limit error, 
-00001340: 756e 6b6e 6f77 6e20 7265 7370 0a20 2020  unknown resp.   
-00001350: 2020 2020 2077 6974 6820 7265 7175 6573       with reques
-00001360: 7473 5f6d 6f63 6b28 2920 6173 206d 6f63  ts_mock() as moc
-00001370: 6b3a 0a20 2020 2020 2020 2020 2020 206d  k:.            m
-00001380: 6f63 6b2e 6765 7428 414e 592c 2073 7461  ock.get(ANY, sta
-00001390: 7475 735f 636f 6465 3d34 3239 2c20 7465  tus_code=429, te
-000013a0: 7874 3d27 7b7d 2729 0a0a 2020 2020 2020  xt='{}')..      
-000013b0: 2020 2020 2020 7769 7468 2073 656c 662e        with self.
-000013c0: 6173 7365 7274 5261 6973 6573 2845 7863  assertRaises(Exc
-000013d0: 6570 7469 6f6e 2920 6173 2063 7478 3a0a  eption) as ctx:.
-000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013f0: 7a6f 6e65 203d 205a 6f6e 6528 2775 6e69  zone = Zone('uni
-00001400: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
-00001410: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00001420: 726f 7669 6465 722e 706f 7075 6c61 7465  rovider.populate
-00001430: 287a 6f6e 6529 0a0a 2020 2020 2020 2020  (zone)..        
-00001440: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00001450: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-00001460: 2020 2020 2020 2743 6c6f 7564 666c 6172        'Cloudflar
-00001470: 6552 6174 654c 696d 6974 4572 726f 7227  eRateLimitError'
-00001480: 2c20 7479 7065 2863 7478 2e65 7863 6570  , type(ctx.excep
-00001490: 7469 6f6e 292e 5f5f 6e61 6d65 5f5f 0a20  tion).__name__. 
-000014a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000014b0: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-000014c0: 7365 7274 4571 7561 6c28 2743 6c6f 7564  sertEqual('Cloud
-000014d0: 666c 6172 6520 6572 726f 7227 2c20 7374  flare error', st
-000014e0: 7228 6374 782e 6578 6365 7074 696f 6e29  r(ctx.exception)
-000014f0: 290a 0a20 2020 2020 2020 2023 204e 6f6e  )..        # Non
-00001500: 2d65 7869 7374 656e 7420 7a6f 6e65 2064  -existent zone d
-00001510: 6f65 736e 2774 2070 6f70 756c 6174 6520  oesn't populate 
-00001520: 616e 7974 6869 6e67 0a20 2020 2020 2020  anything.       
-00001530: 2077 6974 6820 7265 7175 6573 7473 5f6d   with requests_m
-00001540: 6f63 6b28 2920 6173 206d 6f63 6b3a 0a20  ock() as mock:. 
-00001550: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
-00001560: 6765 7428 414e 592c 2073 7461 7475 735f  get(ANY, status_
-00001570: 636f 6465 3d32 3030 2c20 6a73 6f6e 3d73  code=200, json=s
-00001580: 656c 662e 656d 7074 7929 0a0a 2020 2020  elf.empty)..    
-00001590: 2020 2020 2020 2020 7a6f 6e65 203d 205a          zone = Z
-000015a0: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
-000015b0: 272c 205b 5d29 0a20 2020 2020 2020 2020  ', []).         
-000015c0: 2020 2070 726f 7669 6465 722e 706f 7075     provider.popu
-000015d0: 6c61 7465 287a 6f6e 6529 0a20 2020 2020  late(zone).     
-000015e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-000015f0: 7274 4571 7561 6c28 7365 7428 292c 207a  rtEqual(set(), z
-00001600: 6f6e 652e 7265 636f 7264 7329 0a0a 2020  one.records)..  
-00001610: 2020 2020 2020 2320 7265 2d70 6f70 756c        # re-popul
-00001620: 6174 696e 6720 7468 6520 7361 6d65 206e  ating the same n
-00001630: 6f6e 2d65 7869 7374 656e 7420 7a6f 6e65  on-existent zone
-00001640: 2075 7365 7320 6361 6368 6520 616e 6420   uses cache and 
-00001650: 6d61 6b65 7320 6e6f 0a20 2020 2020 2020  makes no.       
-00001660: 2023 2063 616c 6c73 0a20 2020 2020 2020   # calls.       
-00001670: 2061 6761 696e 203d 205a 6f6e 6528 2775   again = Zone('u
-00001680: 6e69 742e 7465 7374 732e 272c 205b 5d29  nit.tests.', [])
-00001690: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
-000016a0: 722e 706f 7075 6c61 7465 2861 6761 696e  r.populate(again
-000016b0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-000016c0: 7373 6572 7445 7175 616c 2873 6574 2829  ssertEqual(set()
-000016d0: 2c20 6167 6169 6e2e 7265 636f 7264 7329  , again.records)
-000016e0: 0a0a 2020 2020 2020 2020 2320 6275 7374  ..        # bust
-000016f0: 207a 6f6e 6520 6361 6368 650a 2020 2020   zone cache.    
-00001700: 2020 2020 7072 6f76 6964 6572 2e5f 7a6f      provider._zo
-00001710: 6e65 7320 3d20 4e6f 6e65 0a0a 2020 2020  nes = None..    
-00001720: 2020 2020 2320 6578 6973 7469 6e67 207a      # existing z
-00001730: 6f6e 6520 7769 7468 2064 6174 610a 2020  one with data.  
-00001740: 2020 2020 2020 7769 7468 2072 6571 7565        with reque
-00001750: 7374 735f 6d6f 636b 2829 2061 7320 6d6f  sts_mock() as mo
-00001760: 636b 3a0a 2020 2020 2020 2020 2020 2020  ck:.            
-00001770: 6261 7365 203d 2027 6874 7470 733a 2f2f  base = 'https://
-00001780: 6170 692e 636c 6f75 6466 6c61 7265 2e63  api.cloudflare.c
-00001790: 6f6d 2f63 6c69 656e 742f 7634 2f7a 6f6e  om/client/v4/zon
-000017a0: 6573 270a 0a20 2020 2020 2020 2020 2020  es'..           
-000017b0: 2023 207a 6f6e 6573 0a20 2020 2020 2020   # zones.       
-000017c0: 2020 2020 2077 6974 6820 6f70 656e 2827       with open('
-000017d0: 7465 7374 732f 6669 7874 7572 6573 2f63  tests/fixtures/c
-000017e0: 6c6f 7564 666c 6172 652d 7a6f 6e65 732d  loudflare-zones-
-000017f0: 7061 6765 2d31 2e6a 736f 6e27 2920 6173  page-1.json') as
-00001800: 2066 683a 0a20 2020 2020 2020 2020 2020   fh:.           
-00001810: 2020 2020 206d 6f63 6b2e 6765 7428 6627       mock.get(f'
-00001820: 7b62 6173 657d 3f70 6167 653d 3127 2c20  {base}?page=1', 
-00001830: 7374 6174 7573 5f63 6f64 653d 3230 302c  status_code=200,
-00001840: 2074 6578 743d 6668 2e72 6561 6428 2929   text=fh.read())
-00001850: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00001860: 6820 6f70 656e 2827 7465 7374 732f 6669  h open('tests/fi
-00001870: 7874 7572 6573 2f63 6c6f 7564 666c 6172  xtures/cloudflar
-00001880: 652d 7a6f 6e65 732d 7061 6765 2d32 2e6a  e-zones-page-2.j
-00001890: 736f 6e27 2920 6173 2066 683a 0a20 2020  son') as fh:.   
-000018a0: 2020 2020 2020 2020 2020 2020 206d 6f63               moc
-000018b0: 6b2e 6765 7428 6627 7b62 6173 657d 3f70  k.get(f'{base}?p
-000018c0: 6167 653d 3227 2c20 7374 6174 7573 5f63  age=2', status_c
-000018d0: 6f64 653d 3230 302c 2074 6578 743d 6668  ode=200, text=fh
-000018e0: 2e72 6561 6428 2929 0a20 2020 2020 2020  .read()).       
-000018f0: 2020 2020 2077 6974 6820 6f70 656e 2827       with open('
-00001900: 7465 7374 732f 6669 7874 7572 6573 2f63  tests/fixtures/c
-00001910: 6c6f 7564 666c 6172 652d 7a6f 6e65 732d  loudflare-zones-
-00001920: 7061 6765 2d33 2e6a 736f 6e27 2920 6173  page-3.json') as
-00001930: 2066 683a 0a20 2020 2020 2020 2020 2020   fh:.           
-00001940: 2020 2020 206d 6f63 6b2e 6765 7428 6627       mock.get(f'
-00001950: 7b62 6173 657d 3f70 6167 653d 3327 2c20  {base}?page=3', 
-00001960: 7374 6174 7573 5f63 6f64 653d 3230 302c  status_code=200,
-00001970: 2074 6578 743d 6668 2e72 6561 6428 2929   text=fh.read())
-00001980: 0a20 2020 2020 2020 2020 2020 206d 6f63  .            moc
-00001990: 6b2e 6765 7428 0a20 2020 2020 2020 2020  k.get(.         
-000019a0: 2020 2020 2020 2066 277b 6261 7365 7d3f         f'{base}?
-000019b0: 7061 6765 3d34 272c 0a20 2020 2020 2020  page=4',.       
-000019c0: 2020 2020 2020 2020 2073 7461 7475 735f           status_
-000019d0: 636f 6465 3d32 3030 2c0a 2020 2020 2020  code=200,.      
-000019e0: 2020 2020 2020 2020 2020 6a73 6f6e 3d7b            json={
-000019f0: 2772 6573 756c 7427 3a20 5b5d 2c20 2772  'result': [], 'r
-00001a00: 6573 756c 745f 696e 666f 273a 207b 2763  esult_info': {'c
-00001a10: 6f75 6e74 273a 2030 2c20 2770 6572 5f70  ount': 0, 'per_p
-00001a20: 6167 6527 3a20 307d 7d2c 0a20 2020 2020  age': 0}},.     
-00001a30: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00001a40: 2020 2020 2020 6261 7365 203d 2066 277b        base = f'{
-00001a50: 6261 7365 7d2f 3233 3432 3334 3234 3334  base}/2342342434
-00001a60: 3233 6161 6162 6233 3334 3334 3261 6161  23aaabb334342aaa
-00001a70: 3334 3334 3335 270a 0a20 2020 2020 2020  343435'..       
-00001a80: 2020 2020 2023 2070 6167 6572 756c 6573       # pagerules
-00001a90: 2f55 524c 4657 440a 2020 2020 2020 2020  /URLFWD.        
-00001aa0: 2020 2020 7769 7468 206f 7065 6e28 2774      with open('t
-00001ab0: 6573 7473 2f66 6978 7475 7265 732f 636c  ests/fixtures/cl
-00001ac0: 6f75 6466 6c61 7265 2d70 6167 6572 756c  oudflare-pagerul
-00001ad0: 6573 2e6a 736f 6e27 2920 6173 2066 683a  es.json') as fh:
-00001ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001af0: 206d 6f63 6b2e 6765 7428 0a20 2020 2020   mock.get(.     
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00001b10: 277b 6261 7365 7d2f 7061 6765 7275 6c65  '{base}/pagerule
-00001b20: 733f 7374 6174 7573 3d61 6374 6976 6527  s?status=active'
-00001b30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001b40: 2020 2020 2020 7374 6174 7573 5f63 6f64        status_cod
-00001b50: 653d 3230 302c 0a20 2020 2020 2020 2020  e=200,.         
-00001b60: 2020 2020 2020 2020 2020 2074 6578 743d             text=
-00001b70: 6668 2e72 6561 6428 292c 0a20 2020 2020  fh.read(),.     
-00001b80: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00001b90: 2020 2020 2020 2020 2020 2320 7265 636f            # reco
-00001ba0: 7264 730a 2020 2020 2020 2020 2020 2020  rds.            
-00001bb0: 6261 7365 203d 2066 277b 6261 7365 7d2f  base = f'{base}/
-00001bc0: 646e 735f 7265 636f 7264 7327 0a20 2020  dns_records'.   
-00001bd0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-00001be0: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
-00001bf0: 2020 2020 2774 6573 7473 2f66 6978 7475      'tests/fixtu
-00001c00: 7265 732f 636c 6f75 6466 6c61 7265 2d64  res/cloudflare-d
-00001c10: 6e73 5f72 6563 6f72 6473 2d70 6167 652d  ns_records-page-
-00001c20: 312e 6a73 6f6e 270a 2020 2020 2020 2020  1.json'.        
-00001c30: 2020 2020 2920 6173 2066 683a 0a20 2020      ) as fh:.   
-00001c40: 2020 2020 2020 2020 2020 2020 206d 6f63               moc
-00001c50: 6b2e 6765 7428 6627 7b62 6173 657d 3f70  k.get(f'{base}?p
-00001c60: 6167 653d 3127 2c20 7374 6174 7573 5f63  age=1', status_c
-00001c70: 6f64 653d 3230 302c 2074 6578 743d 6668  ode=200, text=fh
-00001c80: 2e72 6561 6428 2929 0a20 2020 2020 2020  .read()).       
-00001c90: 2020 2020 2077 6974 6820 6f70 656e 280a       with open(.
-00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 2774 6573 7473 2f66 6978 7475 7265 732f  'tests/fixtures/
-00001cc0: 636c 6f75 6466 6c61 7265 2d64 6e73 5f72  cloudflare-dns_r
-00001cd0: 6563 6f72 6473 2d70 6167 652d 322e 6a73  ecords-page-2.js
-00001ce0: 6f6e 270a 2020 2020 2020 2020 2020 2020  on'.            
-00001cf0: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
-00001d00: 2020 2020 2020 2020 206d 6f63 6b2e 6765           mock.ge
-00001d10: 7428 6627 7b62 6173 657d 3f70 6167 653d  t(f'{base}?page=
-00001d20: 3227 2c20 7374 6174 7573 5f63 6f64 653d  2', status_code=
-00001d30: 3230 302c 2074 6578 743d 6668 2e72 6561  200, text=fh.rea
-00001d40: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
-00001d50: 2077 6974 6820 6f70 656e 280a 2020 2020   with open(.    
-00001d60: 2020 2020 2020 2020 2020 2020 2774 6573              'tes
-00001d70: 7473 2f66 6978 7475 7265 732f 636c 6f75  ts/fixtures/clou
-00001d80: 6466 6c61 7265 2d64 6e73 5f72 6563 6f72  dflare-dns_recor
-00001d90: 6473 2d70 6167 652d 332e 6a73 6f6e 270a  ds-page-3.json'.
-00001da0: 2020 2020 2020 2020 2020 2020 2920 6173              ) as
-00001db0: 2066 683a 0a20 2020 2020 2020 2020 2020   fh:.           
-00001dc0: 2020 2020 206d 6f63 6b2e 6765 7428 6627       mock.get(f'
-00001dd0: 7b62 6173 657d 3f70 6167 653d 3327 2c20  {base}?page=3', 
-00001de0: 7374 6174 7573 5f63 6f64 653d 3230 302c  status_code=200,
-00001df0: 2074 6578 743d 6668 2e72 6561 6428 2929   text=fh.read())
-00001e00: 0a0a 2020 2020 2020 2020 2020 2020 7a6f  ..            zo
-00001e10: 6e65 203d 205a 6f6e 6528 2775 6e69 742e  ne = Zone('unit.
-00001e20: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
-00001e30: 2020 2020 2020 2020 2070 726f 7669 6465           provide
-00001e40: 722e 706f 7075 6c61 7465 287a 6f6e 6529  r.populate(zone)
-00001e50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001e60: 662e 6173 7365 7274 4571 7561 6c28 3232  f.assertEqual(22
-00001e70: 2c20 6c65 6e28 7a6f 6e65 2e72 6563 6f72  , len(zone.recor
-00001e80: 6473 2929 0a0a 2020 2020 2020 2020 2020  ds))..          
-00001e90: 2020 6368 616e 6765 7320 3d20 7365 6c66    changes = self
-00001ea0: 2e65 7870 6563 7465 642e 6368 616e 6765  .expected.change
-00001eb0: 7328 7a6f 6e65 2c20 7072 6f76 6964 6572  s(zone, provider
-00001ec0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00001ed0: 2064 656c 6574 6520 6120 7572 6c66 7764   delete a urlfwd
-00001ee0: 2c20 6372 6561 7465 2033 2075 726c 6677  , create 3 urlfw
-00001ef0: 642c 2061 6e64 2063 7265 6174 6520 3120  d, and create 1 
-00001f00: 7370 660a 2020 2020 2020 2020 2020 2020  spf.            
-00001f10: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00001f20: 2839 2c20 6c65 6e28 6368 616e 6765 7329  (9, len(changes)
-00001f30: 290a 0a20 2020 2020 2020 2023 2072 652d  )..        # re-
-00001f40: 706f 7075 6c61 7469 6e67 2074 6865 2073  populating the s
-00001f50: 616d 6520 7a6f 6e65 2f72 6563 6f72 6473  ame zone/records
-00001f60: 2063 6f6d 6573 206f 7574 206f 6620 6361   comes out of ca
-00001f70: 6368 652c 206e 6f20 6361 6c6c 730a 2020  che, no calls.  
-00001f80: 2020 2020 2020 6167 6169 6e20 3d20 5a6f        again = Zo
-00001f90: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
-00001fa0: 2c20 5b5d 290a 2020 2020 2020 2020 7072  , []).        pr
-00001fb0: 6f76 6964 6572 2e70 6f70 756c 6174 6528  ovider.populate(
-00001fc0: 6167 6169 6e29 0a20 2020 2020 2020 2073  again).        s
-00001fd0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00001fe0: 3232 2c20 6c65 6e28 6167 6169 6e2e 7265  22, len(again.re
-00001ff0: 636f 7264 7329 290a 0a20 2020 2064 6566  cords))..    def
-00002000: 2074 6573 745f 6170 706c 7928 7365 6c66   test_apply(self
-00002010: 293a 0a20 2020 2020 2020 2070 726f 7669  ):.        provi
-00002020: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
-00002030: 5072 6f76 6964 6572 280a 2020 2020 2020  Provider(.      
-00002040: 2020 2020 2020 2774 6573 7427 2c20 2765        'test', 'e
-00002050: 6d61 696c 272c 2027 746f 6b65 6e27 2c20  mail', 'token', 
-00002060: 7265 7472 795f 7065 7269 6f64 3d30 2c20  retry_period=0, 
-00002070: 7374 7269 6374 5f73 7570 706f 7274 733d  strict_supports=
-00002080: 4661 6c73 650a 2020 2020 2020 2020 290a  False.        ).
-00002090: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
-000020a0: 722e 5f72 6571 7565 7374 203d 204d 6f63  r._request = Moc
-000020b0: 6b28 290a 0a20 2020 2020 2020 2070 726f  k()..        pro
-000020c0: 7669 6465 722e 5f72 6571 7565 7374 2e73  vider._request.s
-000020d0: 6964 655f 6566 6665 6374 203d 205b 0a20  ide_effect = [. 
-000020e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000020f0: 656d 7074 792c 2020 2320 6e6f 207a 6f6e  empty,  # no zon
-00002100: 6573 0a20 2020 2020 2020 2020 2020 207b  es.            {
-00002110: 2772 6573 756c 7427 3a20 7b27 6964 273a  'result': {'id':
-00002120: 2034 327d 7d2c 2020 2320 7a6f 6e65 2063   42}},  # zone c
-00002130: 7265 6174 650a 2020 2020 2020 2020 5d20  reate.        ] 
-00002140: 2b20 5b0a 2020 2020 2020 2020 2020 2020  + [.            
-00002150: 4e6f 6e65 0a20 2020 2020 2020 205d 202a  None.        ] *
-00002160: 2033 3020 2023 2069 6e64 6976 6964 7561   30  # individua
-00002170: 6c20 7265 636f 7264 2063 7265 6174 6573  l record creates
-00002180: 0a0a 2020 2020 2020 2020 2320 6e6f 6e2d  ..        # non-
-00002190: 6578 6973 7465 6e74 207a 6f6e 652c 2063  existent zone, c
-000021a0: 7265 6174 6520 6576 6572 7974 6869 6e67  reate everything
-000021b0: 0a20 2020 2020 2020 2070 6c61 6e20 3d20  .        plan = 
-000021c0: 7072 6f76 6964 6572 2e70 6c61 6e28 7365  provider.plan(se
-000021d0: 6c66 2e65 7870 6563 7465 6429 0a20 2020  lf.expected).   
-000021e0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000021f0: 4571 7561 6c28 3138 2c20 6c65 6e28 706c  Equal(18, len(pl
-00002200: 616e 2e63 6861 6e67 6573 2929 0a20 2020  an.changes)).   
-00002210: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00002220: 4571 7561 6c28 3138 2c20 7072 6f76 6964  Equal(18, provid
-00002230: 6572 2e61 7070 6c79 2870 6c61 6e29 290a  er.apply(plan)).
-00002240: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00002250: 6572 7446 616c 7365 2870 6c61 6e2e 6578  ertFalse(plan.ex
-00002260: 6973 7473 290a 0a20 2020 2020 2020 2070  ists)..        p
-00002270: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
-00002280: 2e61 7373 6572 745f 6861 735f 6361 6c6c  .assert_has_call
-00002290: 7328 0a20 2020 2020 2020 2020 2020 205b  s(.            [
-000022a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000022b0: 2023 2063 7265 6174 6564 2074 6865 2064   # created the d
-000022c0: 6f6d 6169 6e0a 2020 2020 2020 2020 2020  omain.          
-000022d0: 2020 2020 2020 6361 6c6c 280a 2020 2020        call(.    
-000022e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022f0: 2750 4f53 5427 2c0a 2020 2020 2020 2020  'POST',.        
-00002300: 2020 2020 2020 2020 2020 2020 272f 7a6f              '/zo
-00002310: 6e65 7327 2c0a 2020 2020 2020 2020 2020  nes',.          
-00002320: 2020 2020 2020 2020 2020 6461 7461 3d7b            data={
-00002330: 276a 756d 705f 7374 6172 7427 3a20 4661  'jump_start': Fa
-00002340: 6c73 652c 2027 6e61 6d65 273a 2027 756e  lse, 'name': 'un
-00002350: 6974 2e74 6573 7473 277d 2c0a 2020 2020  it.tests'},.    
-00002360: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00002370: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002380: 2063 7265 6174 6564 2061 7420 6c65 6173   created at leas
-00002390: 7420 6f6e 6520 6f66 2074 6865 2072 6563  t one of the rec
-000023a0: 6f72 6420 7769 7468 2065 7870 6563 7465  ord with expecte
-000023b0: 6420 6461 7461 0a20 2020 2020 2020 2020  d data.         
-000023c0: 2020 2020 2020 2063 616c 6c28 0a20 2020         call(.   
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2027 504f 5354 272c 0a20 2020 2020 2020   'POST',.       
-000023f0: 2020 2020 2020 2020 2020 2020 2027 2f7a               '/z
-00002400: 6f6e 6573 2f34 322f 646e 735f 7265 636f  ones/42/dns_reco
-00002410: 7264 7327 2c0a 2020 2020 2020 2020 2020  rds',.          
-00002420: 2020 2020 2020 2020 2020 6461 7461 3d7b            data={
-00002430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002440: 2020 2020 2020 2020 2027 636f 6e74 656e           'conten
-00002450: 7427 3a20 276e 7331 2e75 6e69 742e 7465  t': 'ns1.unit.te
-00002460: 7374 732e 272c 0a20 2020 2020 2020 2020  sts.',.         
-00002470: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00002480: 7479 7065 273a 2027 4e53 272c 0a20 2020  type': 'NS',.   
+000003e0: 640a 0a0a 6465 6620 7365 745f 7265 636f  d...def set_reco
+000003f0: 7264 5f63 6f6d 6d65 6e74 2872 6563 6f72  rd_comment(recor
+00000400: 642c 2063 6f6d 6d65 6e74 293a 0a20 2020  d, comment):.   
+00000410: 2074 7279 3a0a 2020 2020 2020 2020 7265   try:.        re
+00000420: 636f 7264 2e5f 6f63 746f 646e 735b 2763  cord._octodns['c
+00000430: 6c6f 7564 666c 6172 6527 5d5b 2763 6f6d  loudflare']['com
+00000440: 6d65 6e74 275d 203d 2063 6f6d 6d65 6e74  ment'] = comment
+00000450: 0a20 2020 2065 7863 6570 7420 4b65 7945  .    except KeyE
+00000460: 7272 6f72 3a0a 2020 2020 2020 2020 7265  rror:.        re
+00000470: 636f 7264 2e5f 6f63 746f 646e 735b 2763  cord._octodns['c
+00000480: 6c6f 7564 666c 6172 6527 5d20 3d20 7b27  loudflare'] = {'
+00000490: 636f 6d6d 656e 7427 3a20 636f 6d6d 656e  comment': commen
+000004a0: 747d 0a0a 2020 2020 7265 7475 726e 2072  t}..    return r
+000004b0: 6563 6f72 640a 0a0a 6465 6620 7365 745f  ecord...def set_
+000004c0: 7265 636f 7264 5f74 6167 7328 7265 636f  record_tags(reco
+000004d0: 7264 2c20 7461 6773 293a 0a20 2020 2074  rd, tags):.    t
+000004e0: 7279 3a0a 2020 2020 2020 2020 7265 636f  ry:.        reco
+000004f0: 7264 2e5f 6f63 746f 646e 735b 2763 6c6f  rd._octodns['clo
+00000500: 7564 666c 6172 6527 5d5b 2774 6167 7327  udflare']['tags'
+00000510: 5d20 3d20 7461 6773 0a20 2020 2065 7863  ] = tags.    exc
+00000520: 6570 7420 4b65 7945 7272 6f72 3a0a 2020  ept KeyError:.  
+00000530: 2020 2020 2020 7265 636f 7264 2e5f 6f63        record._oc
+00000540: 746f 646e 735b 2763 6c6f 7564 666c 6172  todns['cloudflar
+00000550: 6527 5d20 3d20 7b27 7461 6773 273a 2074  e'] = {'tags': t
+00000560: 6167 737d 0a0a 2020 2020 7265 7475 726e  ags}..    return
+00000570: 2072 6563 6f72 640a 0a0a 636c 6173 7320   record...class 
+00000580: 5465 7374 436c 6f75 6466 6c61 7265 5072  TestCloudflarePr
+00000590: 6f76 6964 6572 2854 6573 7443 6173 6529  ovider(TestCase)
+000005a0: 3a0a 2020 2020 6578 7065 6374 6564 203d  :.    expected =
+000005b0: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+000005c0: 732e 272c 205b 5d29 0a20 2020 2073 6f75  s.', []).    sou
+000005d0: 7263 6520 3d20 5961 6d6c 5072 6f76 6964  rce = YamlProvid
+000005e0: 6572 2827 7465 7374 272c 206a 6f69 6e28  er('test', join(
+000005f0: 6469 726e 616d 6528 5f5f 6669 6c65 5f5f  dirname(__file__
+00000600: 292c 2027 636f 6e66 6967 2729 290a 2020  ), 'config')).  
+00000610: 2020 736f 7572 6365 2e70 6f70 756c 6174    source.populat
+00000620: 6528 6578 7065 6374 6564 290a 0a20 2020  e(expected)..   
+00000630: 2023 204f 7572 2074 6573 7420 7375 6974   # Our test suit
+00000640: 6520 6469 6666 6572 7320 6120 6269 742c  e differs a bit,
+00000650: 2061 6464 206f 7572 204e 5320 616e 6420   add our NS and 
+00000660: 7265 6d6f 7665 2074 6865 2073 696d 706c  remove the simpl
+00000670: 6520 6f6e 650a 2020 2020 6578 7065 6374  e one.    expect
+00000680: 6564 2e61 6464 5f72 6563 6f72 6428 0a20  ed.add_record(. 
+00000690: 2020 2020 2020 2052 6563 6f72 642e 6e65         Record.ne
+000006a0: 7728 0a20 2020 2020 2020 2020 2020 2065  w(.            e
+000006b0: 7870 6563 7465 642c 0a20 2020 2020 2020  xpected,.       
+000006c0: 2020 2020 2027 756e 6465 7227 2c0a 2020       'under',.  
+000006d0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000006e0: 2020 2020 2020 2020 2020 2020 2774 746c              'ttl
+000006f0: 273a 2033 3630 302c 0a20 2020 2020 2020  ': 3600,.       
+00000700: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+00000710: 2027 4e53 272c 0a20 2020 2020 2020 2020   'NS',.         
+00000720: 2020 2020 2020 2027 7661 6c75 6573 273a         'values':
+00000730: 205b 276e 7331 2e75 6e69 742e 7465 7374   ['ns1.unit.test
+00000740: 732e 272c 2027 6e73 322e 756e 6974 2e74  s.', 'ns2.unit.t
+00000750: 6573 7473 2e27 5d2c 0a20 2020 2020 2020  ests.'],.       
+00000760: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000770: 290a 2020 2020 290a 2020 2020 666f 7220  ).    ).    for 
+00000780: 7265 636f 7264 2069 6e20 6c69 7374 2865  record in list(e
+00000790: 7870 6563 7465 642e 7265 636f 7264 7329  xpected.records)
+000007a0: 3a0a 2020 2020 2020 2020 6966 2072 6563  :.        if rec
+000007b0: 6f72 642e 6e61 6d65 203d 3d20 2773 7562  ord.name == 'sub
+000007c0: 2720 616e 6420 7265 636f 7264 2e5f 7479  ' and record._ty
+000007d0: 7065 203d 3d20 274e 5327 3a0a 2020 2020  pe == 'NS':.    
+000007e0: 2020 2020 2020 2020 6578 7065 6374 6564          expected
+000007f0: 2e5f 7265 6d6f 7665 5f72 6563 6f72 6428  ._remove_record(
+00000800: 7265 636f 7264 290a 2020 2020 2020 2020  record).        
+00000810: 2020 2020 6272 6561 6b0a 0a20 2020 2065      break..    e
+00000820: 6d70 7479 203d 207b 2772 6573 756c 7427  mpty = {'result'
+00000830: 3a20 5b5d 2c20 2772 6573 756c 745f 696e  : [], 'result_in
+00000840: 666f 273a 207b 2763 6f75 6e74 273a 2030  fo': {'count': 0
+00000850: 2c20 2770 6572 5f70 6167 6527 3a20 307d  , 'per_page': 0}
+00000860: 7d0a 0a20 2020 2064 6566 2074 6573 745f  }..    def test_
+00000870: 706f 7075 6c61 7465 2873 656c 6629 3a0a  populate(self):.
+00000880: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00000890: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
+000008a0: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
+000008b0: 6d61 696c 272c 2027 746f 6b65 6e27 2c20  mail', 'token', 
+000008c0: 7265 7472 795f 7065 7269 6f64 3d30 290a  retry_period=0).
+000008d0: 0a20 2020 2020 2020 2023 2042 6164 2072  .        # Bad r
+000008e0: 6571 7565 7374 730a 2020 2020 2020 2020  equests.        
+000008f0: 7769 7468 2072 6571 7565 7374 735f 6d6f  with requests_mo
+00000900: 636b 2829 2061 7320 6d6f 636b 3a0a 2020  ck() as mock:.  
+00000910: 2020 2020 2020 2020 2020 6d6f 636b 2e67            mock.g
+00000920: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00000930: 2020 2020 414e 592c 0a20 2020 2020 2020      ANY,.       
+00000940: 2020 2020 2020 2020 2073 7461 7475 735f           status_
+00000950: 636f 6465 3d34 3030 2c0a 2020 2020 2020  code=400,.      
+00000960: 2020 2020 2020 2020 2020 7465 7874 3d27            text='
+00000970: 7b22 7375 6363 6573 7322 3a66 616c 7365  {"success":false
+00000980: 2c22 6572 726f 7273 223a 5b7b 2263 6f64  ,"errors":[{"cod
+00000990: 6522 3a31 3130 312c 270a 2020 2020 2020  e":1101,'.      
+000009a0: 2020 2020 2020 2020 2020 2722 6d65 7373            '"mess
+000009b0: 6167 6522 3a22 7265 7175 6573 7420 7761  age":"request wa
+000009c0: 7320 696e 7661 6c69 6422 7d5d 2c27 0a20  s invalid"}],'. 
+000009d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000009e0: 226d 6573 7361 6765 7322 3a5b 5d2c 2272  "messages":[],"r
+000009f0: 6573 756c 7422 3a6e 756c 6c7d 272c 0a20  esult":null}',. 
+00000a00: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00000a10: 2020 2020 2020 2020 2020 7769 7468 2073            with s
+00000a20: 656c 662e 6173 7365 7274 5261 6973 6573  elf.assertRaises
+00000a30: 2845 7863 6570 7469 6f6e 2920 6173 2063  (Exception) as c
+00000a40: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
+00000a50: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
+00000a60: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
+00000a70: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+00000a80: 2020 2070 726f 7669 6465 722e 706f 7075     provider.popu
+00000a90: 6c61 7465 287a 6f6e 6529 0a0a 2020 2020  late(zone)..    
+00000aa0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00000ab0: 6572 7445 7175 616c 2827 436c 6f75 6466  ertEqual('Cloudf
+00000ac0: 6c61 7265 4572 726f 7227 2c20 7479 7065  lareError', type
+00000ad0: 2863 7478 2e65 7863 6570 7469 6f6e 292e  (ctx.exception).
+00000ae0: 5f5f 6e61 6d65 5f5f 290a 2020 2020 2020  __name__).      
+00000af0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00000b00: 7445 7175 616c 2827 7265 7175 6573 7420  tEqual('request 
+00000b10: 7761 7320 696e 7661 6c69 6427 2c20 7374  was invalid', st
+00000b20: 7228 6374 782e 6578 6365 7074 696f 6e29  r(ctx.exception)
+00000b30: 290a 0a20 2020 2020 2020 2023 2042 6164  )..        # Bad
+00000b40: 2061 7574 680a 2020 2020 2020 2020 7769   auth.        wi
+00000b50: 7468 2072 6571 7565 7374 735f 6d6f 636b  th requests_mock
+00000b60: 2829 2061 7320 6d6f 636b 3a0a 2020 2020  () as mock:.    
+00000b70: 2020 2020 2020 2020 6d6f 636b 2e67 6574          mock.get
+00000b80: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00000b90: 2020 414e 592c 0a20 2020 2020 2020 2020    ANY,.         
+00000ba0: 2020 2020 2020 2073 7461 7475 735f 636f         status_co
+00000bb0: 6465 3d34 3033 2c0a 2020 2020 2020 2020  de=403,.        
+00000bc0: 2020 2020 2020 2020 7465 7874 3d27 7b22          text='{"
+00000bd0: 7375 6363 6573 7322 3a66 616c 7365 2c22  success":false,"
+00000be0: 6572 726f 7273 223a 5b7b 2263 6f64 6522  errors":[{"code"
+00000bf0: 3a39 3130 332c 270a 2020 2020 2020 2020  :9103,'.        
+00000c00: 2020 2020 2020 2020 2722 6d65 7373 6167          '"messag
+00000c10: 6522 3a22 556e 6b6e 6f77 6e20 582d 4175  e":"Unknown X-Au
+00000c20: 7468 2d4b 6579 206f 7220 582d 4175 7468  th-Key or X-Auth
+00000c30: 2d45 6d61 696c 227d 5d2c 270a 2020 2020  -Email"}],'.    
+00000c40: 2020 2020 2020 2020 2020 2020 2722 6d65              '"me
+00000c50: 7373 6167 6573 223a 5b5d 2c22 7265 7375  ssages":[],"resu
+00000c60: 6c74 223a 6e75 6c6c 7d27 2c0a 2020 2020  lt":null}',.    
+00000c70: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00000c80: 2020 2020 2020 2077 6974 6820 7365 6c66         with self
+00000c90: 2e61 7373 6572 7452 6169 7365 7328 4578  .assertRaises(Ex
+00000ca0: 6365 7074 696f 6e29 2061 7320 6374 783a  ception) as ctx:
+00000cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000cc0: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
+00000cd0: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cf0: 7072 6f76 6964 6572 2e70 6f70 756c 6174  provider.populat
+00000d00: 6528 7a6f 6e65 290a 2020 2020 2020 2020  e(zone).        
+00000d10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00000d20: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
+00000d30: 2020 2020 2020 2743 6c6f 7564 666c 6172        'Cloudflar
+00000d40: 6541 7574 6865 6e74 6963 6174 696f 6e45  eAuthenticationE
+00000d50: 7272 6f72 272c 2074 7970 6528 6374 782e  rror', type(ctx.
+00000d60: 6578 6365 7074 696f 6e29 2e5f 5f6e 616d  exception).__nam
+00000d70: 655f 5f0a 2020 2020 2020 2020 2020 2020  e__.            
+00000d80: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+00000d90: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 2755 6e6b 6e6f 776e 2058 2d41 7574 682d  'Unknown X-Auth-
+00000dc0: 4b65 7920 6f72 2058 2d41 7574 682d 456d  Key or X-Auth-Em
+00000dd0: 6169 6c27 2c20 7374 7228 6374 782e 6578  ail', str(ctx.ex
+00000de0: 6365 7074 696f 6e29 0a20 2020 2020 2020  ception).       
+00000df0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00000e00: 2320 4261 6420 6175 7468 2c20 756e 6b6e  # Bad auth, unkn
+00000e10: 6f77 6e20 7265 7370 0a20 2020 2020 2020  own resp.       
+00000e20: 2077 6974 6820 7265 7175 6573 7473 5f6d   with requests_m
+00000e30: 6f63 6b28 2920 6173 206d 6f63 6b3a 0a20  ock() as mock:. 
+00000e40: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
+00000e50: 6765 7428 414e 592c 2073 7461 7475 735f  get(ANY, status_
+00000e60: 636f 6465 3d34 3033 2c20 7465 7874 3d27  code=403, text='
+00000e70: 7b7d 2729 0a0a 2020 2020 2020 2020 2020  {}')..          
+00000e80: 2020 7769 7468 2073 656c 662e 6173 7365    with self.asse
+00000e90: 7274 5261 6973 6573 2845 7863 6570 7469  rtRaises(Excepti
+00000ea0: 6f6e 2920 6173 2063 7478 3a0a 2020 2020  on) as ctx:.    
+00000eb0: 2020 2020 2020 2020 2020 2020 7a6f 6e65              zone
+00000ec0: 203d 205a 6f6e 6528 2775 6e69 742e 7465   = Zone('unit.te
+00000ed0: 7374 732e 272c 205b 5d29 0a20 2020 2020  sts.', []).     
+00000ee0: 2020 2020 2020 2020 2020 2070 726f 7669             provi
+00000ef0: 6465 722e 706f 7075 6c61 7465 287a 6f6e  der.populate(zon
+00000f00: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
+00000f10: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00000f20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000f30: 2027 436c 6f75 6466 6c61 7265 4175 7468   'CloudflareAuth
+00000f40: 656e 7469 6361 7469 6f6e 4572 726f 7227  enticationError'
+00000f50: 2c20 7479 7065 2863 7478 2e65 7863 6570  , type(ctx.excep
+00000f60: 7469 6f6e 292e 5f5f 6e61 6d65 5f5f 0a20  tion).__name__. 
+00000f70: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00000f80: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
+00000f90: 7365 7274 4571 7561 6c28 2743 6c6f 7564  sertEqual('Cloud
+00000fa0: 666c 6172 6520 6572 726f 7227 2c20 7374  flare error', st
+00000fb0: 7228 6374 782e 6578 6365 7074 696f 6e29  r(ctx.exception)
+00000fc0: 290a 0a20 2020 2020 2020 2023 2047 656e  )..        # Gen
+00000fd0: 6572 616c 2065 7272 6f72 0a20 2020 2020  eral error.     
+00000fe0: 2020 2077 6974 6820 7265 7175 6573 7473     with requests
+00000ff0: 5f6d 6f63 6b28 2920 6173 206d 6f63 6b3a  _mock() as mock:
+00001000: 0a20 2020 2020 2020 2020 2020 206d 6f63  .            moc
+00001010: 6b2e 6765 7428 414e 592c 2073 7461 7475  k.get(ANY, statu
+00001020: 735f 636f 6465 3d35 3032 2c20 7465 7874  s_code=502, text
+00001030: 3d27 5468 696e 6773 2063 6175 6768 7420  ='Things caught 
+00001040: 6669 7265 2729 0a0a 2020 2020 2020 2020  fire')..        
+00001050: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+00001060: 7365 7274 5261 6973 6573 2848 5454 5045  sertRaises(HTTPE
+00001070: 7272 6f72 2920 6173 2063 7478 3a0a 2020  rror) as ctx:.  
+00001080: 2020 2020 2020 2020 2020 2020 2020 7a6f                zo
+00001090: 6e65 203d 205a 6f6e 6528 2775 6e69 742e  ne = Zone('unit.
+000010a0: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
+000010b0: 2020 2020 2020 2020 2020 2020 2070 726f               pro
+000010c0: 7669 6465 722e 706f 7075 6c61 7465 287a  vider.populate(z
+000010d0: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+000010e0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000010f0: 6c28 3530 322c 2063 7478 2e65 7863 6570  l(502, ctx.excep
+00001100: 7469 6f6e 2e72 6573 706f 6e73 652e 7374  tion.response.st
+00001110: 6174 7573 5f63 6f64 6529 0a0a 2020 2020  atus_code)..    
+00001120: 2020 2020 2320 5261 7465 204c 696d 6974      # Rate Limit
+00001130: 2065 7272 6f72 0a20 2020 2020 2020 2077   error.        w
+00001140: 6974 6820 7265 7175 6573 7473 5f6d 6f63  ith requests_moc
+00001150: 6b28 2920 6173 206d 6f63 6b3a 0a20 2020  k() as mock:.   
+00001160: 2020 2020 2020 2020 206d 6f63 6b2e 6765           mock.ge
+00001170: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00001180: 2020 2041 4e59 2c0a 2020 2020 2020 2020     ANY,.        
+00001190: 2020 2020 2020 2020 7374 6174 7573 5f63          status_c
+000011a0: 6f64 653d 3432 392c 0a20 2020 2020 2020  ode=429,.       
+000011b0: 2020 2020 2020 2020 2074 6578 743d 277b           text='{
+000011c0: 2273 7563 6365 7373 223a 6661 6c73 652c  "success":false,
+000011d0: 2265 7272 6f72 7322 3a5b 7b22 636f 6465  "errors":[{"code
+000011e0: 223a 3130 3130 302c 270a 2020 2020 2020  ":10100,'.      
+000011f0: 2020 2020 2020 2020 2020 2722 6d65 7373            '"mess
+00001200: 6167 6522 3a22 4d6f 7265 2074 6861 6e20  age":"More than 
+00001210: 3132 3030 2072 6571 7565 7374 7320 7065  1200 requests pe
+00001220: 7220 3330 3020 7365 636f 6e64 7320 270a  r 300 seconds '.
+00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001240: 2772 6561 6368 6564 2e20 506c 6561 7365  'reached. Please
+00001250: 2077 6169 7420 616e 6420 636f 6e73 6964   wait and consid
+00001260: 6572 2074 6872 6f74 746c 696e 6720 796f  er throttling yo
+00001270: 7572 2027 0a20 2020 2020 2020 2020 2020  ur '.           
+00001280: 2020 2020 2027 7265 7175 6573 7420 7370       'request sp
+00001290: 6565 6422 7d5d 2c22 6d65 7373 6167 6573  eed"}],"messages
+000012a0: 223a 5b5d 2c22 7265 7375 6c74 223a 6e75  ":[],"result":nu
+000012b0: 6c6c 7d27 2c0a 2020 2020 2020 2020 2020  ll}',.          
+000012c0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+000012d0: 2077 6974 6820 7365 6c66 2e61 7373 6572   with self.asser
+000012e0: 7452 6169 7365 7328 4578 6365 7074 696f  tRaises(Exceptio
+000012f0: 6e29 2061 7320 6374 783a 0a20 2020 2020  n) as ctx:.     
+00001300: 2020 2020 2020 2020 2020 207a 6f6e 6520             zone 
+00001310: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
+00001320: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
+00001330: 2020 2020 2020 2020 2020 7072 6f76 6964            provid
+00001340: 6572 2e70 6f70 756c 6174 6528 7a6f 6e65  er.populate(zone
+00001350: 290a 0a20 2020 2020 2020 2020 2020 2073  )..            s
+00001360: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00001370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001380: 2027 436c 6f75 6466 6c61 7265 5261 7465   'CloudflareRate
+00001390: 4c69 6d69 7445 7272 6f72 272c 2074 7970  LimitError', typ
+000013a0: 6528 6374 782e 6578 6365 7074 696f 6e29  e(ctx.exception)
+000013b0: 2e5f 5f6e 616d 655f 5f0a 2020 2020 2020  .__name__.      
+000013c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000013d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+000013e0: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
+000013f0: 2020 2020 2020 274d 6f72 6520 7468 616e        'More than
+00001400: 2031 3230 3020 7265 7175 6573 7473 2070   1200 requests p
+00001410: 6572 2033 3030 2073 6563 6f6e 6473 2027  er 300 seconds '
+00001420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001430: 2027 7265 6163 6865 642e 2050 6c65 6173   'reached. Pleas
+00001440: 6520 7761 6974 2061 6e64 2063 6f6e 7369  e wait and consi
+00001450: 6465 7220 7468 726f 7474 6c69 6e67 2027  der throttling '
+00001460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001470: 2027 796f 7572 2072 6571 7565 7374 2073   'your request s
+00001480: 7065 6564 272c 0a20 2020 2020 2020 2020  peed',.         
+00001490: 2020 2020 2020 2073 7472 2863 7478 2e65         str(ctx.e
+000014a0: 7863 6570 7469 6f6e 292c 0a20 2020 2020  xception),.     
+000014b0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+000014c0: 2020 2320 5261 7465 204c 696d 6974 2065    # Rate Limit e
+000014d0: 7272 6f72 2c20 756e 6b6e 6f77 6e20 7265  rror, unknown re
+000014e0: 7370 0a20 2020 2020 2020 2077 6974 6820  sp.        with 
+000014f0: 7265 7175 6573 7473 5f6d 6f63 6b28 2920  requests_mock() 
+00001500: 6173 206d 6f63 6b3a 0a20 2020 2020 2020  as mock:.       
+00001510: 2020 2020 206d 6f63 6b2e 6765 7428 414e       mock.get(AN
+00001520: 592c 2073 7461 7475 735f 636f 6465 3d34  Y, status_code=4
+00001530: 3239 2c20 7465 7874 3d27 7b7d 2729 0a0a  29, text='{}')..
+00001540: 2020 2020 2020 2020 2020 2020 7769 7468              with
+00001550: 2073 656c 662e 6173 7365 7274 5261 6973   self.assertRais
+00001560: 6573 2845 7863 6570 7469 6f6e 2920 6173  es(Exception) as
+00001570: 2063 7478 3a0a 2020 2020 2020 2020 2020   ctx:.          
+00001580: 2020 2020 2020 7a6f 6e65 203d 205a 6f6e        zone = Zon
+00001590: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
+000015a0: 205b 5d29 0a20 2020 2020 2020 2020 2020   []).           
+000015b0: 2020 2020 2070 726f 7669 6465 722e 706f       provider.po
+000015c0: 7075 6c61 7465 287a 6f6e 6529 0a0a 2020  pulate(zone)..  
+000015d0: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+000015e0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+000015f0: 2020 2020 2020 2020 2020 2020 2743 6c6f              'Clo
+00001600: 7564 666c 6172 6552 6174 654c 696d 6974  udflareRateLimit
+00001610: 4572 726f 7227 2c20 7479 7065 2863 7478  Error', type(ctx
+00001620: 2e65 7863 6570 7469 6f6e 292e 5f5f 6e61  .exception).__na
+00001630: 6d65 5f5f 0a20 2020 2020 2020 2020 2020  me__.           
+00001640: 2029 0a20 2020 2020 2020 2020 2020 2073   ).            s
+00001650: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00001660: 2743 6c6f 7564 666c 6172 6520 6572 726f  'Cloudflare erro
+00001670: 7227 2c20 7374 7228 6374 782e 6578 6365  r', str(ctx.exce
+00001680: 7074 696f 6e29 290a 0a20 2020 2020 2020  ption))..       
+00001690: 2023 204e 6f6e 2d65 7869 7374 656e 7420   # Non-existent 
+000016a0: 7a6f 6e65 2064 6f65 736e 2774 2070 6f70  zone doesn't pop
+000016b0: 756c 6174 6520 616e 7974 6869 6e67 0a20  ulate anything. 
+000016c0: 2020 2020 2020 2077 6974 6820 7265 7175         with requ
+000016d0: 6573 7473 5f6d 6f63 6b28 2920 6173 206d  ests_mock() as m
+000016e0: 6f63 6b3a 0a20 2020 2020 2020 2020 2020  ock:.           
+000016f0: 206d 6f63 6b2e 6765 7428 414e 592c 2073   mock.get(ANY, s
+00001700: 7461 7475 735f 636f 6465 3d32 3030 2c20  tatus_code=200, 
+00001710: 6a73 6f6e 3d73 656c 662e 656d 7074 7929  json=self.empty)
+00001720: 0a0a 2020 2020 2020 2020 2020 2020 7a6f  ..            zo
+00001730: 6e65 203d 205a 6f6e 6528 2775 6e69 742e  ne = Zone('unit.
+00001740: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
+00001750: 2020 2020 2020 2020 2070 726f 7669 6465           provide
+00001760: 722e 706f 7075 6c61 7465 287a 6f6e 6529  r.populate(zone)
+00001770: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00001780: 662e 6173 7365 7274 4571 7561 6c28 7365  f.assertEqual(se
+00001790: 7428 292c 207a 6f6e 652e 7265 636f 7264  t(), zone.record
+000017a0: 7329 0a0a 2020 2020 2020 2020 2320 7265  s)..        # re
+000017b0: 2d70 6f70 756c 6174 696e 6720 7468 6520  -populating the 
+000017c0: 7361 6d65 206e 6f6e 2d65 7869 7374 656e  same non-existen
+000017d0: 7420 7a6f 6e65 2075 7365 7320 6361 6368  t zone uses cach
+000017e0: 6520 616e 6420 6d61 6b65 7320 6e6f 0a20  e and makes no. 
+000017f0: 2020 2020 2020 2023 2063 616c 6c73 0a20         # calls. 
+00001800: 2020 2020 2020 2061 6761 696e 203d 205a         again = Z
+00001810: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
+00001820: 272c 205b 5d29 0a20 2020 2020 2020 2070  ', []).        p
+00001830: 726f 7669 6465 722e 706f 7075 6c61 7465  rovider.populate
+00001840: 2861 6761 696e 290a 2020 2020 2020 2020  (again).        
+00001850: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+00001860: 2873 6574 2829 2c20 6167 6169 6e2e 7265  (set(), again.re
+00001870: 636f 7264 7329 0a0a 2020 2020 2020 2020  cords)..        
+00001880: 2320 6275 7374 207a 6f6e 6520 6361 6368  # bust zone cach
+00001890: 650a 2020 2020 2020 2020 7072 6f76 6964  e.        provid
+000018a0: 6572 2e5f 7a6f 6e65 7320 3d20 4e6f 6e65  er._zones = None
+000018b0: 0a0a 2020 2020 2020 2020 2320 6578 6973  ..        # exis
+000018c0: 7469 6e67 207a 6f6e 6520 7769 7468 2064  ting zone with d
+000018d0: 6174 610a 2020 2020 2020 2020 7769 7468  ata.        with
+000018e0: 2072 6571 7565 7374 735f 6d6f 636b 2829   requests_mock()
+000018f0: 2061 7320 6d6f 636b 3a0a 2020 2020 2020   as mock:.      
+00001900: 2020 2020 2020 6261 7365 203d 2027 6874        base = 'ht
+00001910: 7470 733a 2f2f 6170 692e 636c 6f75 6466  tps://api.cloudf
+00001920: 6c61 7265 2e63 6f6d 2f63 6c69 656e 742f  lare.com/client/
+00001930: 7634 2f7a 6f6e 6573 270a 0a20 2020 2020  v4/zones'..     
+00001940: 2020 2020 2020 2023 207a 6f6e 6573 0a20         # zones. 
+00001950: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00001960: 6f70 656e 2827 7465 7374 732f 6669 7874  open('tests/fixt
+00001970: 7572 6573 2f63 6c6f 7564 666c 6172 652d  ures/cloudflare-
+00001980: 7a6f 6e65 732d 7061 6765 2d31 2e6a 736f  zones-page-1.jso
+00001990: 6e27 2920 6173 2066 683a 0a20 2020 2020  n') as fh:.     
+000019a0: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
+000019b0: 6765 7428 6627 7b62 6173 657d 3f70 6167  get(f'{base}?pag
+000019c0: 653d 3127 2c20 7374 6174 7573 5f63 6f64  e=1', status_cod
+000019d0: 653d 3230 302c 2074 6578 743d 6668 2e72  e=200, text=fh.r
+000019e0: 6561 6428 2929 0a20 2020 2020 2020 2020  ead()).         
+000019f0: 2020 2077 6974 6820 6f70 656e 2827 7465     with open('te
+00001a00: 7374 732f 6669 7874 7572 6573 2f63 6c6f  sts/fixtures/clo
+00001a10: 7564 666c 6172 652d 7a6f 6e65 732d 7061  udflare-zones-pa
+00001a20: 6765 2d32 2e6a 736f 6e27 2920 6173 2066  ge-2.json') as f
+00001a30: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00001a40: 2020 206d 6f63 6b2e 6765 7428 6627 7b62     mock.get(f'{b
+00001a50: 6173 657d 3f70 6167 653d 3227 2c20 7374  ase}?page=2', st
+00001a60: 6174 7573 5f63 6f64 653d 3230 302c 2074  atus_code=200, t
+00001a70: 6578 743d 6668 2e72 6561 6428 2929 0a20  ext=fh.read()). 
+00001a80: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00001a90: 6f70 656e 2827 7465 7374 732f 6669 7874  open('tests/fixt
+00001aa0: 7572 6573 2f63 6c6f 7564 666c 6172 652d  ures/cloudflare-
+00001ab0: 7a6f 6e65 732d 7061 6765 2d33 2e6a 736f  zones-page-3.jso
+00001ac0: 6e27 2920 6173 2066 683a 0a20 2020 2020  n') as fh:.     
+00001ad0: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
+00001ae0: 6765 7428 6627 7b62 6173 657d 3f70 6167  get(f'{base}?pag
+00001af0: 653d 3327 2c20 7374 6174 7573 5f63 6f64  e=3', status_cod
+00001b00: 653d 3230 302c 2074 6578 743d 6668 2e72  e=200, text=fh.r
+00001b10: 6561 6428 2929 0a20 2020 2020 2020 2020  ead()).         
+00001b20: 2020 206d 6f63 6b2e 6765 7428 0a20 2020     mock.get(.   
+00001b30: 2020 2020 2020 2020 2020 2020 2066 277b               f'{
+00001b40: 6261 7365 7d3f 7061 6765 3d34 272c 0a20  base}?page=4',. 
+00001b50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001b60: 7461 7475 735f 636f 6465 3d32 3030 2c0a  tatus_code=200,.
+00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b80: 6a73 6f6e 3d7b 2772 6573 756c 7427 3a20  json={'result': 
+00001b90: 5b5d 2c20 2772 6573 756c 745f 696e 666f  [], 'result_info
+00001ba0: 273a 207b 2763 6f75 6e74 273a 2030 2c20  ': {'count': 0, 
+00001bb0: 2770 6572 5f70 6167 6527 3a20 307d 7d2c  'per_page': 0}},
+00001bc0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00001bd0: 2020 2020 2020 2020 2020 2020 6261 7365              base
+00001be0: 203d 2066 277b 6261 7365 7d2f 3233 3432   = f'{base}/2342
+00001bf0: 3334 3234 3334 3233 6161 6162 6233 3334  34243423aaabb334
+00001c00: 3334 3261 6161 3334 3334 3335 270a 0a20  342aaa343435'.. 
+00001c10: 2020 2020 2020 2020 2020 2023 2070 6167             # pag
+00001c20: 6572 756c 6573 2f55 524c 4657 440a 2020  erules/URLFWD.  
+00001c30: 2020 2020 2020 2020 2020 7769 7468 206f            with o
+00001c40: 7065 6e28 2774 6573 7473 2f66 6978 7475  pen('tests/fixtu
+00001c50: 7265 732f 636c 6f75 6466 6c61 7265 2d70  res/cloudflare-p
+00001c60: 6167 6572 756c 6573 2e6a 736f 6e27 2920  agerules.json') 
+00001c70: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
+00001c80: 2020 2020 2020 206d 6f63 6b2e 6765 7428         mock.get(
+00001c90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ca0: 2020 2020 2066 277b 6261 7365 7d2f 7061       f'{base}/pa
+00001cb0: 6765 7275 6c65 733f 7374 6174 7573 3d61  gerules?status=a
+00001cc0: 6374 6976 6527 2c0a 2020 2020 2020 2020  ctive',.        
+00001cd0: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00001ce0: 7573 5f63 6f64 653d 3230 302c 0a20 2020  us_code=200,.   
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d00: 2074 6578 743d 6668 2e72 6561 6428 292c   text=fh.read(),
+00001d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001d20: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+00001d30: 2320 7265 636f 7264 730a 2020 2020 2020  # records.      
+00001d40: 2020 2020 2020 6261 7365 203d 2066 277b        base = f'{
+00001d50: 6261 7365 7d2f 646e 735f 7265 636f 7264  base}/dns_record
+00001d60: 7327 0a20 2020 2020 2020 2020 2020 2077  s'.            w
+00001d70: 6974 6820 6f70 656e 280a 2020 2020 2020  ith open(.      
+00001d80: 2020 2020 2020 2020 2020 2774 6573 7473            'tests
+00001d90: 2f66 6978 7475 7265 732f 636c 6f75 6466  /fixtures/cloudf
+00001da0: 6c61 7265 2d64 6e73 5f72 6563 6f72 6473  lare-dns_records
+00001db0: 2d70 6167 652d 312e 6a73 6f6e 270a 2020  -page-1.json'.  
+00001dc0: 2020 2020 2020 2020 2020 2920 6173 2066            ) as f
+00001dd0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00001de0: 2020 206d 6f63 6b2e 6765 7428 6627 7b62     mock.get(f'{b
+00001df0: 6173 657d 3f70 6167 653d 3127 2c20 7374  ase}?page=1', st
+00001e00: 6174 7573 5f63 6f64 653d 3230 302c 2074  atus_code=200, t
+00001e10: 6578 743d 6668 2e72 6561 6428 2929 0a20  ext=fh.read()). 
+00001e20: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00001e30: 6f70 656e 280a 2020 2020 2020 2020 2020  open(.          
+00001e40: 2020 2020 2020 2774 6573 7473 2f66 6978        'tests/fix
+00001e50: 7475 7265 732f 636c 6f75 6466 6c61 7265  tures/cloudflare
+00001e60: 2d64 6e73 5f72 6563 6f72 6473 2d70 6167  -dns_records-pag
+00001e70: 652d 322e 6a73 6f6e 270a 2020 2020 2020  e-2.json'.      
+00001e80: 2020 2020 2020 2920 6173 2066 683a 0a20        ) as fh:. 
+00001e90: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00001ea0: 6f63 6b2e 6765 7428 6627 7b62 6173 657d  ock.get(f'{base}
+00001eb0: 3f70 6167 653d 3227 2c20 7374 6174 7573  ?page=2', status
+00001ec0: 5f63 6f64 653d 3230 302c 2074 6578 743d  _code=200, text=
+00001ed0: 6668 2e72 6561 6428 2929 0a20 2020 2020  fh.read()).     
+00001ee0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00001ef0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00001f00: 2020 2774 6573 7473 2f66 6978 7475 7265    'tests/fixture
+00001f10: 732f 636c 6f75 6466 6c61 7265 2d64 6e73  s/cloudflare-dns
+00001f20: 5f72 6563 6f72 6473 2d70 6167 652d 332e  _records-page-3.
+00001f30: 6a73 6f6e 270a 2020 2020 2020 2020 2020  json'.          
+00001f40: 2020 2920 6173 2066 683a 0a20 2020 2020    ) as fh:.     
+00001f50: 2020 2020 2020 2020 2020 206d 6f63 6b2e             mock.
+00001f60: 6765 7428 6627 7b62 6173 657d 3f70 6167  get(f'{base}?pag
+00001f70: 653d 3327 2c20 7374 6174 7573 5f63 6f64  e=3', status_cod
+00001f80: 653d 3230 302c 2074 6578 743d 6668 2e72  e=200, text=fh.r
+00001f90: 6561 6428 2929 0a0a 2020 2020 2020 2020  ead())..        
+00001fa0: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
+00001fb0: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
+00001fc0: 5d29 0a20 2020 2020 2020 2020 2020 2070  ]).            p
+00001fd0: 726f 7669 6465 722e 706f 7075 6c61 7465  rovider.populate
+00001fe0: 287a 6f6e 6529 0a20 2020 2020 2020 2020  (zone).         
+00001ff0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00002000: 7561 6c28 3232 2c20 6c65 6e28 7a6f 6e65  ual(22, len(zone
+00002010: 2e72 6563 6f72 6473 2929 0a0a 2020 2020  .records))..    
+00002020: 2020 2020 2020 2020 6368 616e 6765 7320          changes 
+00002030: 3d20 7365 6c66 2e65 7870 6563 7465 642e  = self.expected.
+00002040: 6368 616e 6765 7328 7a6f 6e65 2c20 7072  changes(zone, pr
+00002050: 6f76 6964 6572 290a 0a20 2020 2020 2020  ovider)..       
+00002060: 2020 2020 2023 2064 656c 6574 6520 6120       # delete a 
+00002070: 7572 6c66 7764 2c20 6372 6561 7465 2033  urlfwd, create 3
+00002080: 2075 726c 6677 642c 2061 6e64 2063 7265   urlfwd, and cre
+00002090: 6174 6520 3120 7370 660a 2020 2020 2020  ate 1 spf.      
+000020a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000020b0: 7445 7175 616c 2839 2c20 6c65 6e28 6368  tEqual(9, len(ch
+000020c0: 616e 6765 7329 290a 0a20 2020 2020 2020  anges))..       
+000020d0: 2023 2072 652d 706f 7075 6c61 7469 6e67   # re-populating
+000020e0: 2074 6865 2073 616d 6520 7a6f 6e65 2f72   the same zone/r
+000020f0: 6563 6f72 6473 2063 6f6d 6573 206f 7574  ecords comes out
+00002100: 206f 6620 6361 6368 652c 206e 6f20 6361   of cache, no ca
+00002110: 6c6c 730a 2020 2020 2020 2020 6167 6169  lls.        agai
+00002120: 6e20 3d20 5a6f 6e65 2827 756e 6974 2e74  n = Zone('unit.t
+00002130: 6573 7473 2e27 2c20 5b5d 290a 2020 2020  ests.', []).    
+00002140: 2020 2020 7072 6f76 6964 6572 2e70 6f70      provider.pop
+00002150: 756c 6174 6528 6167 6169 6e29 0a20 2020  ulate(again).   
+00002160: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00002170: 4571 7561 6c28 3232 2c20 6c65 6e28 6167  Equal(22, len(ag
+00002180: 6169 6e2e 7265 636f 7264 7329 290a 0a20  ain.records)).. 
+00002190: 2020 2064 6566 2074 6573 745f 6170 706c     def test_appl
+000021a0: 7928 7365 6c66 293a 0a20 2020 2020 2020  y(self):.       
+000021b0: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
+000021c0: 6466 6c61 7265 5072 6f76 6964 6572 280a  dflareProvider(.
+000021d0: 2020 2020 2020 2020 2020 2020 2774 6573              'tes
+000021e0: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
+000021f0: 6b65 6e27 2c20 7265 7472 795f 7065 7269  ken', retry_peri
+00002200: 6f64 3d30 2c20 7374 7269 6374 5f73 7570  od=0, strict_sup
+00002210: 706f 7274 733d 4661 6c73 650a 2020 2020  ports=False.    
+00002220: 2020 2020 290a 0a20 2020 2020 2020 2070      )..        p
+00002230: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
+00002240: 203d 204d 6f63 6b28 290a 0a20 2020 2020   = Mock()..     
+00002250: 2020 2070 726f 7669 6465 722e 5f72 6571     provider._req
+00002260: 7565 7374 2e73 6964 655f 6566 6665 6374  uest.side_effect
+00002270: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00002280: 2073 656c 662e 656d 7074 792c 2020 2320   self.empty,  # 
+00002290: 6e6f 207a 6f6e 6573 0a20 2020 2020 2020  no zones.       
+000022a0: 2020 2020 207b 2772 6573 756c 7427 3a20       {'result': 
+000022b0: 7b27 6964 273a 2034 327d 7d2c 2020 2320  {'id': 42}},  # 
+000022c0: 7a6f 6e65 2063 7265 6174 650a 2020 2020  zone create.    
+000022d0: 2020 2020 5d20 2b20 5b0a 2020 2020 2020      ] + [.      
+000022e0: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
+000022f0: 2020 205d 202a 2033 3020 2023 2069 6e64     ] * 30  # ind
+00002300: 6976 6964 7561 6c20 7265 636f 7264 2063  ividual record c
+00002310: 7265 6174 6573 0a0a 2020 2020 2020 2020  reates..        
+00002320: 2320 6e6f 6e2d 6578 6973 7465 6e74 207a  # non-existent z
+00002330: 6f6e 652c 2063 7265 6174 6520 6576 6572  one, create ever
+00002340: 7974 6869 6e67 0a20 2020 2020 2020 2070  ything.        p
+00002350: 6c61 6e20 3d20 7072 6f76 6964 6572 2e70  lan = provider.p
+00002360: 6c61 6e28 7365 6c66 2e65 7870 6563 7465  lan(self.expecte
+00002370: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
+00002380: 6173 7365 7274 4571 7561 6c28 3138 2c20  assertEqual(18, 
+00002390: 6c65 6e28 706c 616e 2e63 6861 6e67 6573  len(plan.changes
+000023a0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+000023b0: 6173 7365 7274 4571 7561 6c28 3138 2c20  assertEqual(18, 
+000023c0: 7072 6f76 6964 6572 2e61 7070 6c79 2870  provider.apply(p
+000023d0: 6c61 6e29 290a 2020 2020 2020 2020 7365  lan)).        se
+000023e0: 6c66 2e61 7373 6572 7446 616c 7365 2870  lf.assertFalse(p
+000023f0: 6c61 6e2e 6578 6973 7473 290a 0a20 2020  lan.exists)..   
+00002400: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
+00002410: 6571 7565 7374 2e61 7373 6572 745f 6861  equest.assert_ha
+00002420: 735f 6361 6c6c 7328 0a20 2020 2020 2020  s_calls(.       
+00002430: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+00002440: 2020 2020 2020 2023 2063 7265 6174 6564         # created
+00002450: 2074 6865 2064 6f6d 6169 6e0a 2020 2020   the domain.    
+00002460: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+00002470: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002480: 2020 2020 2020 2750 4f53 5427 2c0a 2020        'POST',.  
 00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2027 6e61 6d65 273a 2027 756e       'name': 'un
-000024b0: 6465 722e 756e 6974 2e74 6573 7473 272c  der.unit.tests',
-000024c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000024d0: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
-000024e0: 3336 3030 2c0a 2020 2020 2020 2020 2020  3600,.          
-000024f0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00002500: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00002510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002520: 2320 6d61 6b65 2073 7572 6520 7365 6d69  # make sure semi
-00002530: 636f 6c6f 6e73 2061 7265 206e 6f74 2065  colons are not e
-00002540: 7363 6170 6564 2077 6865 6e20 7365 6e64  scaped when send
-00002550: 696e 6720 6461 7461 0a20 2020 2020 2020  ing data.       
-00002560: 2020 2020 2020 2020 2063 616c 6c28 0a20           call(. 
-00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002580: 2020 2027 504f 5354 272c 0a20 2020 2020     'POST',.     
-00002590: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000025a0: 2f7a 6f6e 6573 2f34 322f 646e 735f 7265  /zones/42/dns_re
-000025b0: 636f 7264 7327 2c0a 2020 2020 2020 2020  cords',.        
-000025c0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-000025d0: 3d7b 0a20 2020 2020 2020 2020 2020 2020  ={.             
-000025e0: 2020 2020 2020 2020 2020 2027 636f 6e74             'cont
-000025f0: 656e 7427 3a20 2776 3d44 4b49 4d31 3b6b  ent': 'v=DKIM1;k
-00002600: 3d72 7361 3b73 3d65 6d61 696c 3b68 3d73  =rsa;s=email;h=s
-00002610: 6861 3235 363b 270a 2020 2020 2020 2020  ha256;'.        
-00002620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002630: 2770 3d41 2f6b 696e 6461 2b6f 662f 6c6f  'p=A/kinda+of/lo
-00002640: 6e67 2f73 7472 696e 672b 7769 7468 2b6e  ng/string+with+n
-00002650: 756d 6233 7273 272c 0a20 2020 2020 2020  umb3rs',.       
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2027 7479 7065 273a 2027 5458 5427 2c0a   'type': 'TXT',.
+000024a0: 2020 272f 7a6f 6e65 7327 2c0a 2020 2020    '/zones',.    
+000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000024c0: 6461 7461 3d7b 276a 756d 705f 7374 6172  data={'jump_star
+000024d0: 7427 3a20 4661 6c73 652c 2027 6e61 6d65  t': False, 'name
+000024e0: 273a 2027 756e 6974 2e74 6573 7473 277d  ': 'unit.tests'}
+000024f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002500: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00002510: 2020 2020 2023 2063 7265 6174 6564 2061       # created a
+00002520: 7420 6c65 6173 7420 6f6e 6520 6f66 2074  t least one of t
+00002530: 6865 2072 6563 6f72 6420 7769 7468 2065  he record with e
+00002540: 7870 6563 7465 6420 6461 7461 0a20 2020  xpected data.   
+00002550: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+00002560: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00002570: 2020 2020 2020 2027 504f 5354 272c 0a20         'POST',. 
+00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002590: 2020 2027 2f7a 6f6e 6573 2f34 322f 646e     '/zones/42/dn
+000025a0: 735f 7265 636f 7264 7327 2c0a 2020 2020  s_records',.    
+000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025c0: 6461 7461 3d7b 0a20 2020 2020 2020 2020  data={.         
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000025e0: 636f 6e74 656e 7427 3a20 276e 7331 2e75  content': 'ns1.u
+000025f0: 6e69 742e 7465 7374 732e 272c 0a20 2020  nit.tests.',.   
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 2020 2020 2027 7479 7065 273a 2027 4e53       'type': 'NS
+00002620: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00002630: 2020 2020 2020 2020 2020 2027 6e61 6d65             'name
+00002640: 273a 2027 756e 6465 722e 756e 6974 2e74  ': 'under.unit.t
+00002650: 6573 7473 272c 0a20 2020 2020 2020 2020  ests',.         
+00002660: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00002670: 7474 6c27 3a20 3336 3030 2c0a 2020 2020  ttl': 3600,.    
 00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
-000026a0: 2774 7874 2e75 6e69 742e 7465 7374 7327  'txt.unit.tests'
-000026b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000026c0: 2020 2020 2020 2020 2020 2774 746c 273a            'ttl':
-000026d0: 2036 3030 2c0a 2020 2020 2020 2020 2020   600,.          
-000026e0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000026f0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
-00002700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002710: 2320 6372 6561 7465 2061 7420 6c65 6173  # create at leas
-00002720: 7420 6f6e 6520 7061 6765 7275 6c65 730a  t one pagerules.
-00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002740: 6361 6c6c 280a 2020 2020 2020 2020 2020  call(.          
-00002750: 2020 2020 2020 2020 2020 2750 4f53 5427            'POST'
-00002760: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002770: 2020 2020 2020 272f 7a6f 6e65 732f 3432        '/zones/42
-00002780: 2f70 6167 6572 756c 6573 272c 0a20 2020  /pagerules',.   
-00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027a0: 2064 6174 613d 7b0a 2020 2020 2020 2020   data={.        
+00002690: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+000026a0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+000026b0: 2020 2020 2020 2320 6d61 6b65 2073 7572        # make sur
+000026c0: 6520 7365 6d69 636f 6c6f 6e73 2061 7265  e semicolons are
+000026d0: 206e 6f74 2065 7363 6170 6564 2077 6865   not escaped whe
+000026e0: 6e20 7365 6e64 696e 6720 6461 7461 0a20  n sending data. 
+000026f0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00002700: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
+00002710: 2020 2020 2020 2020 2027 504f 5354 272c           'POST',
+00002720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002730: 2020 2020 2027 2f7a 6f6e 6573 2f34 322f       '/zones/42/
+00002740: 646e 735f 7265 636f 7264 7327 2c0a 2020  dns_records',.  
+00002750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002760: 2020 6461 7461 3d7b 0a20 2020 2020 2020    data={.       
+00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002780: 2027 636f 6e74 656e 7427 3a20 2776 3d44   'content': 'v=D
+00002790: 4b49 4d31 3b6b 3d72 7361 3b73 3d65 6d61  KIM1;k=rsa;s=ema
+000027a0: 696c 3b68 3d73 6861 3235 363b 270a 2020  il;h=sha256;'.  
 000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2774 6172 6765 7473 273a 205b 0a20 2020  'targets': [.   
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000027c0: 2020 2020 2020 2770 3d41 2f6b 696e 6461        'p=A/kinda
+000027d0: 2b6f 662f 6c6f 6e67 2f73 7472 696e 672b  +of/long/string+
+000027e0: 7769 7468 2b6e 756d 6233 7273 272c 0a20  with+numb3rs',. 
 000027f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002800: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
-00002810: 6574 273a 2027 7572 6c27 2c0a 2020 2020  et': 'url',.    
-00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002830: 2020 2020 2020 2020 2020 2020 2763 6f6e              'con
-00002840: 7374 7261 696e 7427 3a20 7b0a 2020 2020  straint': {.    
+00002800: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
+00002810: 5458 5427 2c0a 2020 2020 2020 2020 2020  TXT',.          
+00002820: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+00002830: 616d 6527 3a20 2774 7874 2e75 6e69 742e  ame': 'txt.unit.
+00002840: 7465 7374 7327 2c0a 2020 2020 2020 2020  tests',.        
 00002850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002870: 276f 7065 7261 746f 7227 3a20 276d 6174  'operator': 'mat
-00002880: 6368 6573 272c 0a20 2020 2020 2020 2020  ches',.         
-00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028a0: 2020 2020 2020 2020 2020 2027 7661 6c75             'valu
-000028b0: 6527 3a20 2775 726c 6677 642e 756e 6974  e': 'urlfwd.unit
-000028c0: 2e74 6573 7473 2f27 2c0a 2020 2020 2020  .tests/',.      
-000028d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028e0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-00002910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002920: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-00002930: 2020 2020 2020 2020 2020 2020 2020 2761                'a
-00002940: 6374 696f 6e73 273a 205b 0a20 2020 2020  ctions': [.     
-00002950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002960: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 2020 2020 2020 2027 6964 273a 2027           'id': '
-00002990: 666f 7277 6172 6469 6e67 5f75 726c 272c  forwarding_url',
-000029a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2027 7661 6c75 6527 3a20 7b0a 2020 2020   'value': {.    
-000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2775 726c 273a 2027 6874 7470 3a2f 2f77  'url': 'http://w
-00002a00: 7777 2e75 6e69 742e 7465 7374 7327 2c0a  ww.unit.tests',.
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002860: 2774 746c 273a 2036 3030 2c0a 2020 2020  'ttl': 600,.    
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00002890: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
+000028a0: 2020 2020 2020 2320 6372 6561 7465 2061        # create a
+000028b0: 7420 6c65 6173 7420 6f6e 6520 7061 6765  t least one page
+000028c0: 7275 6c65 730a 2020 2020 2020 2020 2020  rules.          
+000028d0: 2020 2020 2020 6361 6c6c 280a 2020 2020        call(.    
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2750 4f53 5427 2c0a 2020 2020 2020 2020  'POST',.        
+00002900: 2020 2020 2020 2020 2020 2020 272f 7a6f              '/zo
+00002910: 6e65 732f 3432 2f70 6167 6572 756c 6573  nes/42/pagerules
+00002920: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00002930: 2020 2020 2020 2064 6174 613d 7b0a 2020         data={.  
+00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002950: 2020 2020 2020 2774 6172 6765 7473 273a        'targets':
+00002960: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+00002970: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 2027 7461 7267 6574 273a 2027 7572 6c27   'target': 'url'
+000029b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000029c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029d0: 2020 2763 6f6e 7374 7261 696e 7427 3a20    'constraint': 
+000029e0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+000029f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a00: 2020 2020 2020 276f 7065 7261 746f 7227        'operator'
+00002a10: 3a20 276d 6174 6368 6573 272c 0a20 2020  : 'matches',.   
 00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a30: 2020 2020 2773 7461 7475 735f 636f 6465      'status_code
-00002a40: 273a 2033 3032 2c0a 2020 2020 2020 2020  ': 302,.        
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a40: 2027 7661 6c75 6527 3a20 2775 726c 6677   'value': 'urlfw
+00002a50: 642e 756e 6974 2e74 6573 7473 2f27 2c0a  d.unit.tests/',.
+00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002aa0: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00002ab0: 2020 2020 2020 2020 2020 2020 2773 7461              'sta
-00002ac0: 7475 7327 3a20 2761 6374 6976 6527 2c0a  tus': 'active',.
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ae0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00002af0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00002b00: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00002b10: 2020 2020 2054 7275 652c 0a20 2020 2020       True,.     
-00002b20: 2020 2029 0a20 2020 2020 2020 2023 2065     ).        # e
-00002b30: 7870 6563 7465 6420 6e75 6d62 6572 206f  xpected number o
-00002b40: 6620 746f 7461 6c20 6361 6c6c 730a 2020  f total calls.  
-00002b50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00002b60: 7445 7175 616c 2833 322c 2070 726f 7669  tEqual(32, provi
-00002b70: 6465 722e 5f72 6571 7565 7374 2e63 616c  der._request.cal
-00002b80: 6c5f 636f 756e 7429 0a0a 2020 2020 2020  l_count)..      
-00002b90: 2020 7072 6f76 6964 6572 2e5f 7265 7175    provider._requ
-00002ba0: 6573 742e 7265 7365 745f 6d6f 636b 2829  est.reset_mock()
-00002bb0: 0a0a 2020 2020 2020 2020 7072 6f76 6964  ..        provid
-00002bc0: 6572 2e7a 6f6e 655f 7265 636f 7264 7320  er.zone_records 
-00002bd0: 3d20 4d6f 636b 280a 2020 2020 2020 2020  = Mock(.        
-00002be0: 2020 2020 7265 7475 726e 5f76 616c 7565      return_value
-00002bf0: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
-00002c00: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00002c10: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-00002c20: 6663 3132 6162 3334 6364 3536 3131 3333  fc12ab34cd561133
-00002c30: 3434 3232 6162 3333 3232 3939 3736 3533  4422ab3322997653
-00002c40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002c50: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-00002c60: 4122 2c0a 2020 2020 2020 2020 2020 2020  A",.            
-00002c70: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-00002c80: 2277 7777 2e75 6e69 742e 7465 7374 7322  "www.unit.tests"
-00002c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002ca0: 2020 2020 2020 2263 6f6e 7465 6e74 223a        "content":
-00002cb0: 2022 312e 322e 332e 3422 2c0a 2020 2020   "1.2.3.4",.    
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2270 726f 7869 6162 6c65 223a 2054 7275  "proxiable": Tru
-00002ce0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00002cf0: 2020 2020 2020 2022 7072 6f78 6965 6422         "proxied"
-00002d00: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00002d10: 2020 2020 2020 2020 2020 2020 2022 7474               "tt
-00002d20: 6c22 3a20 3330 302c 0a20 2020 2020 2020  l": 300,.       
-00002d30: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
-00002d40: 636b 6564 223a 2046 616c 7365 2c0a 2020  cked": False,.  
-00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d60: 2020 227a 6f6e 655f 6964 223a 2022 6666    "zone_id": "ff
-00002d70: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
-00002d80: 3232 6162 3333 3232 3939 3736 3530 222c  22ab3322997650",
-00002d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002da0: 2020 2020 2022 7a6f 6e65 5f6e 616d 6522       "zone_name"
-00002db0: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
-00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dd0: 2020 2020 226d 6f64 6966 6965 645f 6f6e      "modified_on
-00002de0: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
-00002df0: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
-00002e00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002e10: 2020 2020 2020 2263 7265 6174 6564 5f6f        "created_o
-00002e20: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
-00002e30: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
-00002e40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00002e50: 2020 2020 2020 2022 6d65 7461 223a 207b         "meta": {
-00002e60: 2261 7574 6f5f 6164 6465 6422 3a20 4661  "auto_added": Fa
-00002e70: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
-00002e80: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00002e90: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00002ea0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002eb0: 6964 223a 2022 6663 3132 6162 3334 6364  id": "fc12ab34cd
-00002ec0: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
-00002ed0: 3939 3736 3534 222c 0a20 2020 2020 2020  997654",.       
-00002ee0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-00002ef0: 7065 223a 2022 4122 2c0a 2020 2020 2020  pe": "A",.      
-00002f00: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00002f10: 616d 6522 3a20 2277 7777 2e75 6e69 742e  ame": "www.unit.
-00002f20: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
-00002f30: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-00002f40: 7465 6e74 223a 2022 322e 322e 332e 3422  tent": "2.2.3.4"
-00002f50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002f60: 2020 2020 2020 2270 726f 7869 6162 6c65        "proxiable
-00002f70: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00002f80: 2020 2020 2020 2020 2020 2020 2022 7072               "pr
-00002f90: 6f78 6965 6422 3a20 4661 6c73 652c 0a20  oxied": False,. 
-00002fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fb0: 2020 2022 7474 6c22 3a20 3330 302c 0a20     "ttl": 300,. 
-00002fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fd0: 2020 2022 6c6f 636b 6564 223a 2046 616c     "locked": Fal
-00002fe0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00002ff0: 2020 2020 2020 2020 227a 6f6e 655f 6964          "zone_id
-00003000: 223a 2022 6666 3132 6162 3334 6364 3536  ": "ff12ab34cd56
-00003010: 3131 3333 3434 3232 6162 3333 3232 3939  11334422ab332299
-00003020: 3736 3530 222c 0a20 2020 2020 2020 2020  7650",.         
-00003030: 2020 2020 2020 2020 2020 2022 7a6f 6e65             "zone
-00003040: 5f6e 616d 6522 3a20 2275 6e69 742e 7465  _name": "unit.te
-00003050: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
-00003060: 2020 2020 2020 2020 2020 226d 6f64 6966            "modif
-00003070: 6965 645f 6f6e 223a 2022 3230 3137 2d30  ied_on": "2017-0
-00003080: 332d 3131 5431 383a 3031 3a34 342e 3033  3-11T18:01:44.03
-00003090: 3030 3434 5a22 2c0a 2020 2020 2020 2020  0044Z",.        
-000030a0: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
-000030b0: 6174 6564 5f6f 6e22 3a20 2232 3031 372d  ated_on": "2017-
-000030c0: 3033 2d31 3154 3138 3a30 313a 3434 2e30  03-11T18:01:44.0
-000030d0: 3330 3034 345a 222c 0a20 2020 2020 2020  30044Z",.       
-000030e0: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
-000030f0: 7461 223a 207b 2261 7574 6f5f 6164 6465  ta": {"auto_adde
-00003100: 6422 3a20 4661 6c73 657d 2c0a 2020 2020  d": False},.    
-00003110: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00003120: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00003130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003140: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
-00003150: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-00003160: 6162 3333 3232 3939 3736 3535 222c 0a20  ab3322997655",. 
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2022 7479 7065 223a 2022 4122 2c0a     "type": "A",.
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 226e 616d 6522 3a20 226e 632e      "name": "nc.
-000031b0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+00002a80: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+00002a90: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00002aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ab0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 2761 6374 696f 6e73 273a 205b      'actions': [
+00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002af0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00002b20: 6964 273a 2027 666f 7277 6172 6469 6e67  id': 'forwarding
+00002b30: 5f75 726c 272c 0a20 2020 2020 2020 2020  _url',.         
+00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b50: 2020 2020 2020 2027 7661 6c75 6527 3a20         'value': 
+00002b60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b80: 2020 2020 2020 2775 726c 273a 2027 6874        'url': 'ht
+00002b90: 7470 3a2f 2f77 7777 2e75 6e69 742e 7465  tp://www.unit.te
+00002ba0: 7374 7327 2c0a 2020 2020 2020 2020 2020  sts',.          
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bc0: 2020 2020 2020 2020 2020 2773 7461 7475            'statu
+00002bd0: 735f 636f 6465 273a 2033 3032 2c0a 2020  s_code': 302,.  
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00002c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002c10: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c30: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00002c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c50: 2020 2773 7461 7475 7327 3a20 2761 6374    'status': 'act
+00002c60: 6976 6527 2c0a 2020 2020 2020 2020 2020  ive',.          
+00002c70: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00002c80: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00002c90: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00002ca0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
+00002cb0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00002cc0: 2020 2023 2065 7870 6563 7465 6420 6e75     # expected nu
+00002cd0: 6d62 6572 206f 6620 746f 7461 6c20 6361  mber of total ca
+00002ce0: 6c6c 730a 2020 2020 2020 2020 7365 6c66  lls.        self
+00002cf0: 2e61 7373 6572 7445 7175 616c 2833 322c  .assertEqual(32,
+00002d00: 2070 726f 7669 6465 722e 5f72 6571 7565   provider._reque
+00002d10: 7374 2e63 616c 6c5f 636f 756e 7429 0a0a  st.call_count)..
+00002d20: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00002d30: 2e5f 7265 7175 6573 742e 7265 7365 745f  ._request.reset_
+00002d40: 6d6f 636b 2829 0a0a 2020 2020 2020 2020  mock()..        
+00002d50: 7072 6f76 6964 6572 2e7a 6f6e 655f 7265  provider.zone_re
+00002d60: 636f 7264 7320 3d20 4d6f 636b 280a 2020  cords = Mock(.  
+00002d70: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002d80: 5f76 616c 7565 3d5b 0a20 2020 2020 2020  _value=[.       
+00002d90: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00002db0: 6964 223a 2022 6663 3132 6162 3334 6364  id": "fc12ab34cd
+00002dc0: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
+00002dd0: 3939 3736 3533 222c 0a20 2020 2020 2020  997653",.       
+00002de0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00002df0: 7065 223a 2022 4122 2c0a 2020 2020 2020  pe": "A",.      
+00002e00: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00002e10: 616d 6522 3a20 2277 7777 2e75 6e69 742e  ame": "www.unit.
+00002e20: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
+00002e30: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00002e40: 7465 6e74 223a 2022 312e 322e 332e 3422  tent": "1.2.3.4"
+00002e50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002e60: 2020 2020 2020 2270 726f 7869 6162 6c65        "proxiable
+00002e70: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
+00002e80: 2020 2020 2020 2020 2020 2020 2022 7072               "pr
+00002e90: 6f78 6965 6422 3a20 4661 6c73 652c 0a20  oxied": False,. 
+00002ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002eb0: 2020 2022 7474 6c22 3a20 3330 302c 0a20     "ttl": 300,. 
+00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ed0: 2020 2022 6c6f 636b 6564 223a 2046 616c     "locked": Fal
+00002ee0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00002ef0: 2020 2020 2020 2020 227a 6f6e 655f 6964          "zone_id
+00002f00: 223a 2022 6666 3132 6162 3334 6364 3536  ": "ff12ab34cd56
+00002f10: 3131 3333 3434 3232 6162 3333 3232 3939  11334422ab332299
+00002f20: 3736 3530 222c 0a20 2020 2020 2020 2020  7650",.         
+00002f30: 2020 2020 2020 2020 2020 2022 7a6f 6e65             "zone
+00002f40: 5f6e 616d 6522 3a20 2275 6e69 742e 7465  _name": "unit.te
+00002f50: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+00002f60: 2020 2020 2020 2020 2020 226d 6f64 6966            "modif
+00002f70: 6965 645f 6f6e 223a 2022 3230 3137 2d30  ied_on": "2017-0
+00002f80: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
+00002f90: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
+00002fa0: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
+00002fb0: 6174 6564 5f6f 6e22 3a20 2232 3031 372d  ated_on": "2017-
+00002fc0: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
+00002fd0: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
+00002fe0: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
+00002ff0: 7461 223a 207b 2261 7574 6f5f 6164 6465  ta": {"auto_adde
+00003000: 6422 3a20 4661 6c73 657d 2c0a 2020 2020  d": False},.    
+00003010: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00003020: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00003030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003040: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
+00003050: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
+00003060: 6162 3333 3232 3939 3736 3534 222c 0a20  ab3322997654",. 
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2022 7479 7065 223a 2022 4122 2c0a     "type": "A",.
+00003090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030a0: 2020 2020 226e 616d 6522 3a20 2277 7777      "name": "www
+000030b0: 2e75 6e69 742e 7465 7374 7322 2c0a 2020  .unit.tests",.  
+000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030d0: 2020 2263 6f6e 7465 6e74 223a 2022 322e    "content": "2.
+000030e0: 322e 332e 3422 2c0a 2020 2020 2020 2020  2.3.4",.        
+000030f0: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
+00003100: 7869 6162 6c65 223a 2054 7275 652c 0a20  xiable": True,. 
+00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003120: 2020 2022 7072 6f78 6965 6422 3a20 4661     "proxied": Fa
+00003130: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00003140: 2020 2020 2020 2020 2022 7474 6c22 3a20           "ttl": 
+00003150: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
+00003160: 2020 2020 2020 2020 2022 6c6f 636b 6564           "locked
+00003170: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+00003180: 2020 2020 2020 2020 2020 2020 2020 227a                "z
+00003190: 6f6e 655f 6964 223a 2022 6666 3132 6162  one_id": "ff12ab
+000031a0: 3334 6364 3536 3131 3333 3434 3232 6162  34cd5611334422ab
+000031b0: 3333 3232 3939 3736 3530 222c 0a20 2020  3322997650",.   
 000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2022 636f 6e74 656e 7422 3a20 2233 2e32   "content": "3.2
-000031e0: 2e33 2e34 222c 0a20 2020 2020 2020 2020  .3.4",.         
-000031f0: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
-00003200: 6961 626c 6522 3a20 5472 7565 2c0a 2020  iable": True,.  
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2020 2270 726f 7869 6564 223a 2046 616c    "proxied": Fal
-00003230: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-00003240: 2020 2020 2020 2020 2274 746c 223a 2031          "ttl": 1
-00003250: 3230 2c0a 2020 2020 2020 2020 2020 2020  20,.            
-00003260: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
-00003270: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00003280: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
-00003290: 6e65 5f69 6422 3a20 2266 6631 3261 6233  ne_id": "ff12ab3
-000032a0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
-000032b0: 3332 3239 3937 3635 3022 2c0a 2020 2020  322997650",.    
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 227a 6f6e 655f 6e61 6d65 223a 2022 756e  "zone_name": "un
-000032e0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003300: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
-00003310: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
-00003320: 3434 2e30 3330 3034 345a 222c 0a20 2020  44.030044Z",.   
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2022 6372 6561 7465 645f 6f6e 223a 2022   "created_on": "
-00003350: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
-00003360: 3a34 342e 3033 3030 3434 5a22 2c0a 2020  :44.030044Z",.  
-00003370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003380: 2020 226d 6574 6122 3a20 7b22 6175 746f    "meta": {"auto
-00003390: 5f61 6464 6564 223a 2046 616c 7365 7d2c  _added": False},
-000033a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033b0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-000033c0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-000033d0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-000033e0: 2266 6331 3261 6233 3463 6435 3631 3133  "fc12ab34cd56113
-000033f0: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
-00003400: 3522 2c0a 2020 2020 2020 2020 2020 2020  5",.            
-00003410: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00003420: 2241 222c 0a20 2020 2020 2020 2020 2020  "A",.           
-00003430: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-00003440: 2022 7474 6c2e 756e 6974 2e74 6573 7473   "ttl.unit.tests
-00003450: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003460: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
-00003470: 3a20 2234 2e32 2e33 2e34 222c 0a20 2020  : "4.2.3.4",.   
-00003480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003490: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
-000034a0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-000034b0: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
-000034c0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
-000034d0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000034e0: 746c 223a 2036 3030 2c0a 2020 2020 2020  tl": 600,.      
-000034f0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00003500: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
-00003530: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
-00003540: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
-00003550: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003560: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
-00003570: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
-00003580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003590: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
-000035a0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
-000035b0: 3138 3a30 313a 3434 2e30 3330 3034 345a  18:01:44.030044Z
-000035c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000035d0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-000035e0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
-000035f0: 5431 383a 3031 3a34 342e 3033 3030 3434  T18:01:44.030044
-00003600: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-00003610: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
-00003620: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
-00003630: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-00003640: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00003650: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000031d0: 2022 7a6f 6e65 5f6e 616d 6522 3a20 2275   "zone_name": "u
+000031e0: 6e69 742e 7465 7374 7322 2c0a 2020 2020  nit.tests",.    
+000031f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003200: 226d 6f64 6966 6965 645f 6f6e 223a 2022  "modified_on": "
+00003210: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
+00003220: 3a34 342e 3033 3030 3434 5a22 2c0a 2020  :44.030044Z",.  
+00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003240: 2020 2263 7265 6174 6564 5f6f 6e22 3a20    "created_on": 
+00003250: 2232 3031 372d 3033 2d31 3154 3138 3a30  "2017-03-11T18:0
+00003260: 313a 3434 2e30 3330 3034 345a 222c 0a20  1:44.030044Z",. 
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 2020 2022 6d65 7461 223a 207b 2261 7574     "meta": {"aut
+00003290: 6f5f 6164 6465 6422 3a20 4661 6c73 657d  o_added": False}
+000032a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000032b0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+000032c0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000032d0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+000032e0: 2022 6663 3132 6162 3334 6364 3536 3131   "fc12ab34cd5611
+000032f0: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+00003300: 3535 222c 0a20 2020 2020 2020 2020 2020  55",.           
+00003310: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00003320: 2022 4122 2c0a 2020 2020 2020 2020 2020   "A",.          
+00003330: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00003340: 3a20 226e 632e 756e 6974 2e74 6573 7473  : "nc.unit.tests
+00003350: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003360: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
+00003370: 3a20 2233 2e32 2e33 2e34 222c 0a20 2020  : "3.2.3.4",.   
+00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003390: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
+000033a0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000033b0: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
+000033c0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+000033d0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000033e0: 746c 223a 2031 3230 2c0a 2020 2020 2020  tl": 120,.      
+000033f0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+00003400: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
+00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003420: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
+00003430: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
+00003440: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
+00003450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003460: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
+00003470: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
+00003480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003490: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
+000034a0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
+000034b0: 3138 3a30 313a 3434 2e30 3330 3034 345a  18:01:44.030044Z
+000034c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000034d0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
+000034e0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
+000034f0: 5431 383a 3031 3a34 342e 3033 3030 3434  T18:01:44.030044
+00003500: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
+00003510: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
+00003520: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
+00003530: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
+00003540: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00003550: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003570: 2269 6422 3a20 2266 6331 3261 6233 3463  "id": "fc12ab34c
+00003580: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
+00003590: 3239 3937 3635 3522 2c0a 2020 2020 2020  2997655",.      
+000035a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000035b0: 7970 6522 3a20 2241 222c 0a20 2020 2020  ype": "A",.     
+000035c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000035d0: 6e61 6d65 223a 2022 7474 6c2e 756e 6974  name": "ttl.unit
+000035e0: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
+000035f0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00003600: 6e74 656e 7422 3a20 2234 2e32 2e33 2e34  ntent": "4.2.3.4
+00003610: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003620: 2020 2020 2020 2022 7072 6f78 6961 626c         "proxiabl
+00003630: 6522 3a20 5472 7565 2c0a 2020 2020 2020  e": True,.      
+00003640: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00003650: 726f 7869 6564 223a 2046 616c 7365 2c0a  roxied": False,.
 00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003670: 2269 6422 3a20 2232 6139 3134 3062 3137  "id": "2a9140b17
-00003680: 6666 6230 6536 6165 6438 3236 3034 3965  ffb0e6aed826049e
-00003690: 6563 3937 3062 3722 2c0a 2020 2020 2020  ec970b7",.      
-000036a0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000036b0: 6172 6765 7473 223a 205b 0a20 2020 2020  argets": [.     
-000036c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036d0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-000036e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036f0: 2022 7461 7267 6574 223a 2022 7572 6c22   "target": "url"
-00003700: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003710: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-00003720: 6f6e 7374 7261 696e 7422 3a20 7b0a 2020  onstraint": {.  
-00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003740: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-00003750: 7065 7261 746f 7222 3a20 226d 6174 6368  perator": "match
-00003760: 6573 222c 0a20 2020 2020 2020 2020 2020  es",.           
-00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003780: 2020 2020 2022 7661 6c75 6522 3a20 2275       "value": "u
-00003790: 726c 6677 642e 756e 6974 2e74 6573 7473  rlfwd.unit.tests
-000037a0: 2f22 2c0a 2020 2020 2020 2020 2020 2020  /",.            
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000037d0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00003670: 2020 2020 2274 746c 223a 2036 3030 2c0a      "ttl": 600,.
+00003680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003690: 2020 2020 226c 6f63 6b65 6422 3a20 4661      "locked": Fa
+000036a0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000036b0: 2020 2020 2020 2020 2022 7a6f 6e65 5f69           "zone_i
+000036c0: 6422 3a20 2266 6631 3261 6233 3463 6435  d": "ff12ab34cd5
+000036d0: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
+000036e0: 3937 3635 3022 2c0a 2020 2020 2020 2020  97650",.        
+000036f0: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+00003700: 655f 6e61 6d65 223a 2022 756e 6974 2e74  e_name": "unit.t
+00003710: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+00003720: 2020 2020 2020 2020 2020 2022 6d6f 6469             "modi
+00003730: 6669 6564 5f6f 6e22 3a20 2232 3031 372d  fied_on": "2017-
+00003740: 3033 2d31 3154 3138 3a30 313a 3434 2e30  03-11T18:01:44.0
+00003750: 3330 3034 345a 222c 0a20 2020 2020 2020  30044Z",.       
+00003760: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+00003770: 6561 7465 645f 6f6e 223a 2022 3230 3137  eated_on": "2017
+00003780: 2d30 332d 3131 5431 383a 3031 3a34 342e  -03-11T18:01:44.
+00003790: 3033 3030 3434 5a22 2c0a 2020 2020 2020  030044Z",.      
+000037a0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+000037b0: 6574 6122 3a20 7b22 6175 746f 5f61 6464  eta": {"auto_add
+000037c0: 6564 223a 2046 616c 7365 7d2c 0a20 2020  ed": False},.   
+000037d0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
 000037e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037f0: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00003800: 2020 2020 2020 2020 2261 6374 696f 6e73          "actions
-00003810: 223a 205b 0a20 2020 2020 2020 2020 2020  ": [.           
-00003820: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+000037f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003800: 2020 2020 2020 2269 6422 3a20 2232 6139        "id": "2a9
+00003810: 3134 3062 3137 6666 6230 6536 6165 6438  140b17ffb0e6aed8
+00003820: 3236 3034 3965 6563 3937 3062 3722 2c0a  26049eec970b7",.
 00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00003850: 2022 666f 7277 6172 6469 6e67 5f75 726c   "forwarding_url
-00003860: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003870: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003880: 7661 6c75 6522 3a20 7b0a 2020 2020 2020  value": {.      
-00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2020 2020 2020 2020 2020 2275 726c 223a            "url":
-000038b0: 2022 6874 7470 733a 2f2f 7777 772e 756e   "https://www.un
-000038c0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
+00003840: 2020 2020 2274 6172 6765 7473 223a 205b      "targets": [
+00003850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003860: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00003870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003880: 2020 2020 2020 2022 7461 7267 6574 223a         "target":
+00003890: 2022 7572 6c22 2c0a 2020 2020 2020 2020   "url",.        
+000038a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038b0: 2020 2020 2263 6f6e 7374 7261 696e 7422      "constraint"
+000038c0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
 000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2020 2020 2020 2022 7374 6174             "stat
-000038f0: 7573 5f63 6f64 6522 3a20 3330 322c 0a20  us_code": 302,. 
+000038e0: 2020 2020 226f 7065 7261 746f 7222 3a20      "operator": 
+000038f0: 226d 6174 6368 6573 222c 0a20 2020 2020  "matches",.     
 00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00003920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003930: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00003940: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
-00003950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003960: 2020 2022 7072 696f 7269 7479 223a 2031     "priority": 1
-00003970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003980: 2020 2020 2020 2273 7461 7475 7322 3a20        "status": 
-00003990: 2261 6374 6976 6522 2c0a 2020 2020 2020  "active",.      
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000039b0: 7265 6174 6564 5f6f 6e22 3a20 2232 3032  reated_on": "202
-000039c0: 312d 3036 2d32 3554 3230 3a31 303a 3530  1-06-25T20:10:50
-000039d0: 2e30 3030 3030 305a 222c 0a20 2020 2020  .000000Z",.     
-000039e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000039f0: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
-00003a00: 3032 312d 3036 2d32 3854 3232 3a33 383a  021-06-28T22:38:
-00003a10: 3130 2e30 3030 3030 305a 222c 0a20 2020  10.000000Z",.   
-00003a20: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00003910: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00003920: 6522 3a20 2275 726c 6677 642e 756e 6974  e": "urlfwd.unit
+00003930: 2e74 6573 7473 2f22 2c0a 2020 2020 2020  .tests/",.      
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003970: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00003980: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+00003990: 2020 2020 2020 2020 2020 2020 2020 2261                "a
+000039a0: 6374 696f 6e73 223a 205b 0a20 2020 2020  ctions": [.     
+000039b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039c0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039e0: 2022 6964 223a 2022 666f 7277 6172 6469   "id": "forwardi
+000039f0: 6e67 5f75 726c 222c 0a20 2020 2020 2020  ng_url",.       
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 2020 2022 7661 6c75 6522 3a20 7b0a       "value": {.
+00003a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003a50: 2020 2020 2020 2269 6422 3a20 2232 6139        "id": "2a9
-00003a60: 3134 3162 3138 6666 6230 6536 6165 6438  141b18ffb0e6aed8
-00003a70: 3236 3035 3065 6563 3937 3062 3822 2c0a  26050eec970b8",.
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a90: 2020 2020 2274 6172 6765 7473 223a 205b      "targets": [
-00003aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003ab0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00003ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ad0: 2020 2020 2020 2022 7461 7267 6574 223a         "target":
-00003ae0: 2022 7572 6c22 2c0a 2020 2020 2020 2020   "url",.        
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2020 2020 2263 6f6e 7374 7261 696e 7422      "constraint"
-00003b10: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00003b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b30: 2020 2020 226f 7065 7261 746f 7222 3a20      "operator": 
-00003b40: 226d 6174 6368 6573 222c 0a20 2020 2020  "matches",.     
-00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b60: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
-00003b70: 6522 3a20 2275 726c 6677 646f 7468 6572  e": "urlfwdother
-00003b80: 2e75 6e69 742e 7465 7374 732f 7461 7267  .unit.tests/targ
-00003b90: 6574 222c 0a20 2020 2020 2020 2020 2020  et",.           
-00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00003bc0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-00003bf0: 2020 2020 2020 2020 2022 6163 7469 6f6e           "action
-00003c00: 7322 3a20 5b0a 2020 2020 2020 2020 2020  s": [.          
-00003c10: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c30: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-00003c40: 3a20 2266 6f72 7761 7264 696e 675f 7572  : "forwarding_ur
-00003c50: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c70: 2276 616c 7565 223a 207b 0a20 2020 2020  "value": {.     
+00003a40: 2275 726c 223a 2022 6874 7470 733a 2f2f  "url": "https://
+00003a50: 7777 772e 756e 6974 2e74 6573 7473 222c  www.unit.tests",
+00003a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a80: 2022 7374 6174 7573 5f63 6f64 6522 3a20   "status_code": 
+00003a90: 3330 322c 0a20 2020 2020 2020 2020 2020  302,.           
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ab0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00003ac0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+00003af0: 2020 2020 2020 2020 2022 7072 696f 7269           "priori
+00003b00: 7479 223a 2031 2c0a 2020 2020 2020 2020  ty": 1,.        
+00003b10: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+00003b20: 7475 7322 3a20 2261 6374 6976 6522 2c0a  tus": "active",.
+00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b40: 2020 2020 2263 7265 6174 6564 5f6f 6e22      "created_on"
+00003b50: 3a20 2232 3032 312d 3036 2d32 3554 3230  : "2021-06-25T20
+00003b60: 3a31 303a 3530 2e30 3030 3030 305a 222c  :10:50.000000Z",
+00003b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b80: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
+00003b90: 6e22 3a20 2232 3032 312d 3036 2d32 3854  n": "2021-06-28T
+00003ba0: 3232 3a33 383a 3130 2e30 3030 3030 305a  22:38:10.000000Z
+00003bb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00003bc0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00003bd0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00003be0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00003bf0: 3a20 2232 6139 3134 3162 3138 6666 6230  : "2a9141b18ffb0
+00003c00: 6536 6165 6438 3236 3035 3065 6563 3937  e6aed826050eec97
+00003c10: 3062 3822 2c0a 2020 2020 2020 2020 2020  0b8",.          
+00003c20: 2020 2020 2020 2020 2020 2274 6172 6765            "targe
+00003c30: 7473 223a 205b 0a20 2020 2020 2020 2020  ts": [.         
+00003c40: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00003c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c60: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
+00003c70: 7267 6574 223a 2022 7572 6c22 2c0a 2020  rget": "url",.  
 00003c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c90: 2020 2020 2020 2020 2020 2022 7572 6c22             "url"
-00003ca0: 3a20 2268 7474 7073 3a2f 2f74 6172 6765  : "https://targe
-00003cb0: 742e 756e 6974 2e74 6573 7473 222c 0a20  t.unit.tests",. 
-00003cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cd0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003ce0: 7374 6174 7573 5f63 6f64 6522 3a20 3330  status_code": 30
-00003cf0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00003d00: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00003d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00003d20: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00003c90: 2020 2020 2020 2020 2020 2263 6f6e 7374            "const
+00003ca0: 7261 696e 7422 3a20 7b0a 2020 2020 2020  raint": {.      
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cc0: 2020 2020 2020 2020 2020 226f 7065 7261            "opera
+00003cd0: 746f 7222 3a20 226d 6174 6368 6573 222c  tor": "matches",
+00003ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 2022 7661 6c75 6522 3a20 2275 726c 6677   "value": "urlfw
+00003d10: 646f 7468 6572 2e75 6e69 742e 7465 7374  dother.unit.test
+00003d20: 732f 7461 7267 6574 222c 0a20 2020 2020  s/target",.     
 00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00003d50: 2020 2020 2020 2022 7072 696f 7269 7479         "priority
-00003d60: 223a 2032 2c0a 2020 2020 2020 2020 2020  ": 2,.          
-00003d70: 2020 2020 2020 2020 2020 2273 7461 7475            "statu
-00003d80: 7322 3a20 2261 6374 6976 6522 2c0a 2020  s": "active",.  
-00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003da0: 2020 2263 7265 6174 6564 5f6f 6e22 3a20    "created_on": 
-00003db0: 2232 3032 312d 3036 2d32 3554 3230 3a31  "2021-06-25T20:1
-00003dc0: 303a 3530 2e30 3030 3030 305a 222c 0a20  0:50.000000Z",. 
-00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 2022 6d6f 6469 6669 6564 5f6f 6e22     "modified_on"
-00003df0: 3a20 2232 3032 312d 3036 2d32 3854 3232  : "2021-06-28T22
-00003e00: 3a33 383a 3130 2e30 3030 3030 305a 222c  :38:10.000000Z",
+00003d40: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00003d70: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00003d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003d90: 6163 7469 6f6e 7322 3a20 5b0a 2020 2020  actions": [.    
+00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003db0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00003dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003dd0: 2020 2269 6422 3a20 2266 6f72 7761 7264    "id": "forward
+00003de0: 696e 675f 7572 6c22 2c0a 2020 2020 2020  ing_url",.      
+00003df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e00: 2020 2020 2020 2276 616c 7565 223a 207b        "value": {
 00003e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003e20: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00003e30: 5d0a 2020 2020 2020 2020 290a 0a20 2020  ].        )..   
-00003e40: 2020 2020 2023 2077 6520 646f 6e27 7420       # we don't 
-00003e50: 6361 7265 2061 626f 7574 2074 6865 2050  care about the P
-00003e60: 4f53 542f 6372 6561 7465 2072 6574 7572  OST/create retur
-00003e70: 6e20 7661 6c75 6573 0a20 2020 2020 2020  n values.       
-00003e80: 2070 726f 7669 6465 722e 5f72 6571 7565   provider._reque
-00003e90: 7374 2e72 6574 7572 6e5f 7661 6c75 6520  st.return_value 
-00003ea0: 3d20 7b7d 0a0a 2020 2020 2020 2020 2320  = {}..        # 
-00003eb0: 5465 7374 206f 7574 2074 6865 2063 7265  Test out the cre
-00003ec0: 6174 6520 7261 7465 2d6c 696d 6974 2068  ate rate-limit h
-00003ed0: 616e 646c 696e 672c 2074 6865 6e20 3920  andling, then 9 
-00003ee0: 7375 6363 6573 7365 730a 2020 2020 2020  successes.      
-00003ef0: 2020 7072 6f76 6964 6572 2e5f 7265 7175    provider._requ
-00003f00: 6573 742e 7369 6465 5f65 6666 6563 7420  est.side_effect 
-00003f10: 3d20 5b43 6c6f 7564 666c 6172 6552 6174  = [CloudflareRat
-00003f20: 654c 696d 6974 4572 726f 7228 277b 7d27  eLimitError('{}'
-00003f30: 295d 202b 2028 0a20 2020 2020 2020 2020  )] + (.         
-00003f40: 2020 205b 4e6f 6e65 5d20 2a20 350a 2020     [None] * 5.  
-00003f50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00003f60: 2077 616e 7465 6420 3d20 5a6f 6e65 2827   wanted = Zone('
-00003f70: 756e 6974 2e74 6573 7473 2e27 2c20 5b5d  unit.tests.', []
-00003f80: 290a 2020 2020 2020 2020 7761 6e74 6564  ).        wanted
-00003f90: 2e61 6464 5f72 6563 6f72 6428 0a20 2020  .add_record(.   
-00003fa0: 2020 2020 2020 2020 2052 6563 6f72 642e           Record.
-00003fb0: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
-00003fc0: 2020 2020 2077 616e 7465 642c 0a20 2020       wanted,.   
-00003fd0: 2020 2020 2020 2020 2020 2020 2027 6e63               'nc
-00003fe0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00003ff0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00004000: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
-00004010: 3630 2c20 2023 2054 544c 2069 7320 6265  60,  # TTL is be
-00004020: 6c6f 7720 7468 6569 7220 6d69 6e0a 2020  low their min.  
-00004030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004040: 2020 2774 7970 6527 3a20 2741 272c 0a20    'type': 'A',. 
-00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004060: 2020 2027 7661 6c75 6527 3a20 2733 2e32     'value': '3.2
-00004070: 2e33 2e34 272c 0a20 2020 2020 2020 2020  .3.4',.         
-00004080: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00004090: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000040a0: 290a 2020 2020 2020 2020 7761 6e74 6564  ).        wanted
-000040b0: 2e61 6464 5f72 6563 6f72 6428 0a20 2020  .add_record(.   
-000040c0: 2020 2020 2020 2020 2052 6563 6f72 642e           Record.
-000040d0: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
-000040e0: 2020 2020 2077 616e 7465 642c 0a20 2020       wanted,.   
-000040f0: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
-00004100: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-00004110: 2020 2020 7b27 7474 6c27 3a20 3330 302c      {'ttl': 300,
-00004120: 2027 7479 7065 273a 2027 4127 2c20 2776   'type': 'A', 'v
-00004130: 616c 7565 273a 2027 332e 322e 332e 3427  alue': '3.2.3.4'
-00004140: 7d2c 2020 2320 5454 4c20 6368 616e 6765  },  # TTL change
-00004150: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00004160: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004170: 2077 616e 7465 642e 6164 645f 7265 636f   wanted.add_reco
-00004180: 7264 280a 2020 2020 2020 2020 2020 2020  rd(.            
-00004190: 5265 636f 7264 2e6e 6577 280a 2020 2020  Record.new(.    
-000041a0: 2020 2020 2020 2020 2020 2020 7761 6e74              want
-000041b0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
-000041c0: 2020 2020 2775 726c 6677 6427 2c0a 2020      'urlfwd',.  
-000041d0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-000041e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041f0: 2020 2020 2774 746c 273a 2033 3030 2c0a      'ttl': 300,.
-00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004210: 2020 2020 2774 7970 6527 3a20 2755 524c      'type': 'URL
-00004220: 4657 4427 2c0a 2020 2020 2020 2020 2020  FWD',.          
-00004230: 2020 2020 2020 2020 2020 2776 616c 7565            'value
-00004240: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
-00004250: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
-00004260: 7468 273a 2027 2f2a 272c 2020 2320 7061  th': '/*',  # pa
-00004270: 7468 2063 6861 6e67 650a 2020 2020 2020  th change.      
-00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004290: 2020 2774 6172 6765 7427 3a20 2768 7474    'target': 'htt
-000042a0: 7073 3a2f 2f77 7777 2e75 6e69 742e 7465  ps://www.unit.te
-000042b0: 7374 732f 272c 2020 2320 7461 7267 6574  sts/',  # target
-000042c0: 2063 6861 6e67 650a 2020 2020 2020 2020   change.        
-000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042e0: 2763 6f64 6527 3a20 3330 312c 2020 2320  'code': 301,  # 
-000042f0: 7374 6174 7573 5f63 6f64 6520 6368 616e  status_code chan
-00004300: 6765 0a20 2020 2020 2020 2020 2020 2020  ge.             
-00004310: 2020 2020 2020 2020 2020 2027 6d61 736b             'mask
-00004320: 696e 6727 3a20 2732 272c 0a20 2020 2020  ing': '2',.     
-00004330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004340: 2020 2027 7175 6572 7927 3a20 302c 0a20     'query': 0,. 
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004360: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00004370: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00004380: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
-00004390: 0a0a 2020 2020 2020 2020 706c 616e 203d  ..        plan =
-000043a0: 2070 726f 7669 6465 722e 706c 616e 2877   provider.plan(w
-000043b0: 616e 7465 6429 0a20 2020 2020 2020 2023  anted).        #
-000043c0: 206f 6e6c 7920 7365 6520 7468 6520 6465   only see the de
-000043d0: 6c65 7465 2026 2074 746c 2075 7064 6174  lete & ttl updat
-000043e0: 652c 2062 656c 6f77 206d 696e 2d74 746c  e, below min-ttl
-000043f0: 2069 7320 6669 6c74 6572 6564 206f 7574   is filtered out
-00004400: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00004410: 7365 7274 4571 7561 6c28 342c 206c 656e  sertEqual(4, len
-00004420: 2870 6c61 6e2e 6368 616e 6765 7329 290a  (plan.changes)).
-00004430: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-00004440: 6572 7445 7175 616c 2834 2c20 7072 6f76  ertEqual(4, prov
-00004450: 6964 6572 2e61 7070 6c79 2870 6c61 6e29  ider.apply(plan)
-00004460: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00004470: 7373 6572 7454 7275 6528 706c 616e 2e65  ssertTrue(plan.e
-00004480: 7869 7374 7329 0a20 2020 2020 2020 2023  xists).        #
-00004490: 2063 7265 6174 6573 2061 2074 6865 206e   creates a the n
-000044a0: 6577 2076 616c 7565 2061 6e64 2074 6865  ew value and the
-000044b0: 6e20 6465 6c65 7465 7320 616c 6c20 7468  n deletes all th
-000044c0: 6520 6f6c 640a 2020 2020 2020 2020 7072  e old.        pr
-000044d0: 6f76 6964 6572 2e5f 7265 7175 6573 742e  ovider._request.
-000044e0: 6173 7365 7274 5f68 6173 5f63 616c 6c73  assert_has_calls
-000044f0: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
-00004500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004510: 6361 6c6c 280a 2020 2020 2020 2020 2020  call(.          
-00004520: 2020 2020 2020 2020 2020 2744 454c 4554            'DELET
-00004530: 4527 2c0a 2020 2020 2020 2020 2020 2020  E',.            
-00004540: 2020 2020 2020 2020 272f 7a6f 6e65 732f          '/zones/
-00004550: 3432 2f70 6167 6572 756c 6573 2f32 6139  42/pagerules/2a9
-00004560: 3134 3162 3138 6666 6230 6536 6165 6438  141b18ffb0e6aed8
-00004570: 3236 3035 3065 6563 3937 3062 3827 2c0a  26050eec970b8',.
-00004580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004590: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000045a0: 2020 2063 616c 6c28 0a20 2020 2020 2020     call(.       
-000045b0: 2020 2020 2020 2020 2020 2020 2027 4445               'DE
-000045c0: 4c45 5445 272c 0a20 2020 2020 2020 2020  LETE',.         
-000045d0: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
-000045e0: 6573 2f66 6631 3261 6233 3463 6435 3631  es/ff12ab34cd561
-000045f0: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
-00004600: 3635 302f 270a 2020 2020 2020 2020 2020  650/'.          
-00004610: 2020 2020 2020 2020 2020 2764 6e73 5f72            'dns_r
-00004620: 6563 6f72 6473 2f66 6331 3261 6233 3463  ecords/fc12ab34c
-00004630: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
-00004640: 3239 3937 3635 3327 2c0a 2020 2020 2020  2997653',.      
-00004650: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00004660: 2020 2020 2020 2020 2020 2020 2063 616c               cal
-00004670: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00004680: 2020 2020 2020 2027 4445 4c45 5445 272c         'DELETE',
-00004690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000046a0: 2020 2020 2027 2f7a 6f6e 6573 2f66 6631       '/zones/ff1
-000046b0: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
-000046c0: 3261 6233 3332 3239 3937 3635 302f 270a  2ab3322997650/'.
-000046d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046e0: 2020 2020 2764 6e73 5f72 6563 6f72 6473      'dns_records
-000046f0: 2f66 6331 3261 6233 3463 6435 3631 3133  /fc12ab34cd56113
-00004700: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
-00004710: 3427 2c0a 2020 2020 2020 2020 2020 2020  4',.            
-00004720: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00004730: 2020 2020 2020 2063 616c 6c28 0a20 2020         call(.   
+00003e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e30: 2022 7572 6c22 3a20 2268 7474 7073 3a2f   "url": "https:/
+00003e40: 2f74 6172 6765 742e 756e 6974 2e74 6573  /target.unit.tes
+00003e50: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
+00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e70: 2020 2020 2022 7374 6174 7573 5f63 6f64       "status_cod
+00003e80: 6522 3a20 3330 312c 0a20 2020 2020 2020  e": 301,.       
+00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ea0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00003eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ec0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00003ed0: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00003ee0: 2020 2020 2020 2020 2020 2020 2022 7072               "pr
+00003ef0: 696f 7269 7479 223a 2032 2c0a 2020 2020  iority": 2,.    
+00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f10: 2273 7461 7475 7322 3a20 2261 6374 6976  "status": "activ
+00003f20: 6522 2c0a 2020 2020 2020 2020 2020 2020  e",.            
+00003f30: 2020 2020 2020 2020 2263 7265 6174 6564          "created
+00003f40: 5f6f 6e22 3a20 2232 3032 312d 3036 2d32  _on": "2021-06-2
+00003f50: 3554 3230 3a31 303a 3530 2e30 3030 3030  5T20:10:50.00000
+00003f60: 305a 222c 0a20 2020 2020 2020 2020 2020  0Z",.           
+00003f70: 2020 2020 2020 2020 2022 6d6f 6469 6669           "modifi
+00003f80: 6564 5f6f 6e22 3a20 2232 3032 312d 3036  ed_on": "2021-06
+00003f90: 2d32 3854 3232 3a33 383a 3130 2e30 3030  -28T22:38:10.000
+00003fa0: 3030 305a 222c 0a20 2020 2020 2020 2020  000Z",.         
+00003fb0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00003fc0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00003fd0: 290a 0a20 2020 2020 2020 2023 2077 6520  )..        # we 
+00003fe0: 646f 6e27 7420 6361 7265 2061 626f 7574  don't care about
+00003ff0: 2074 6865 2050 4f53 542f 6372 6561 7465   the POST/create
+00004000: 2072 6574 7572 6e20 7661 6c75 6573 0a20   return values. 
+00004010: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
+00004020: 5f72 6571 7565 7374 2e72 6574 7572 6e5f  _request.return_
+00004030: 7661 6c75 6520 3d20 7b7d 0a0a 2020 2020  value = {}..    
+00004040: 2020 2020 2320 5465 7374 206f 7574 2074      # Test out t
+00004050: 6865 2063 7265 6174 6520 7261 7465 2d6c  he create rate-l
+00004060: 696d 6974 2068 616e 646c 696e 672c 2074  imit handling, t
+00004070: 6865 6e20 3920 7375 6363 6573 7365 730a  hen 9 successes.
+00004080: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00004090: 2e5f 7265 7175 6573 742e 7369 6465 5f65  ._request.side_e
+000040a0: 6666 6563 7420 3d20 5b43 6c6f 7564 666c  ffect = [Cloudfl
+000040b0: 6172 6552 6174 654c 696d 6974 4572 726f  areRateLimitErro
+000040c0: 7228 277b 7d27 295d 202b 2028 0a20 2020  r('{}')] + (.   
+000040d0: 2020 2020 2020 2020 205b 4e6f 6e65 5d20           [None] 
+000040e0: 2a20 350a 2020 2020 2020 2020 290a 0a20  * 5.        ).. 
+000040f0: 2020 2020 2020 2077 616e 7465 6420 3d20         wanted = 
+00004100: 5a6f 6e65 2827 756e 6974 2e74 6573 7473  Zone('unit.tests
+00004110: 2e27 2c20 5b5d 290a 2020 2020 2020 2020  .', []).        
+00004120: 7761 6e74 6564 2e61 6464 5f72 6563 6f72  wanted.add_recor
+00004130: 6428 0a20 2020 2020 2020 2020 2020 2052  d(.            R
+00004140: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
+00004150: 2020 2020 2020 2020 2020 2077 616e 7465             wante
+00004160: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00004170: 2020 2027 6e63 272c 0a20 2020 2020 2020     'nc',.       
+00004180: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00004190: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000041a0: 7474 6c27 3a20 3630 2c20 2023 2054 544c  ttl': 60,  # TTL
+000041b0: 2069 7320 6265 6c6f 7720 7468 6569 7220   is below their 
+000041c0: 6d69 6e0a 2020 2020 2020 2020 2020 2020  min.            
+000041d0: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
+000041e0: 2741 272c 0a20 2020 2020 2020 2020 2020  'A',.           
+000041f0: 2020 2020 2020 2020 2027 7661 6c75 6527           'value'
+00004200: 3a20 2733 2e32 2e33 2e34 272c 0a20 2020  : '3.2.3.4',.   
+00004210: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00004220: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00004230: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00004240: 7761 6e74 6564 2e61 6464 5f72 6563 6f72  wanted.add_recor
+00004250: 6428 0a20 2020 2020 2020 2020 2020 2052  d(.            R
+00004260: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
+00004270: 2020 2020 2020 2020 2020 2077 616e 7465             wante
+00004280: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+00004290: 2020 2027 7474 6c27 2c0a 2020 2020 2020     'ttl',.      
+000042a0: 2020 2020 2020 2020 2020 7b27 7474 6c27            {'ttl'
+000042b0: 3a20 3330 302c 2027 7479 7065 273a 2027  : 300, 'type': '
+000042c0: 4127 2c20 2776 616c 7565 273a 2027 332e  A', 'value': '3.
+000042d0: 322e 332e 3427 7d2c 2020 2320 5454 4c20  2.3.4'},  # TTL 
+000042e0: 6368 616e 6765 0a20 2020 2020 2020 2020  change.         
+000042f0: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
+00004300: 2020 2020 2020 2077 616e 7465 642e 6164         wanted.ad
+00004310: 645f 7265 636f 7264 280a 2020 2020 2020  d_record(.      
+00004320: 2020 2020 2020 5265 636f 7264 2e6e 6577        Record.new
+00004330: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00004340: 2020 7761 6e74 6564 2c0a 2020 2020 2020    wanted,.      
+00004350: 2020 2020 2020 2020 2020 2775 726c 6677            'urlfw
+00004360: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+00004370: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00004380: 2020 2020 2020 2020 2020 2774 746c 273a            'ttl':
+00004390: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
+000043a0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+000043b0: 3a20 2755 524c 4657 4427 2c0a 2020 2020  : 'URLFWD',.    
+000043c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043d0: 2776 616c 7565 273a 207b 0a20 2020 2020  'value': {.     
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 2027 7061 7468 273a 2027 2f2a 272c     'path': '/*',
+00004400: 2020 2320 7061 7468 2063 6861 6e67 650a    # path change.
+00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004420: 2020 2020 2020 2020 2774 6172 6765 7427          'target'
+00004430: 3a20 2768 7474 7073 3a2f 2f77 7777 2e75  : 'https://www.u
+00004440: 6e69 742e 7465 7374 732f 272c 2020 2320  nit.tests/',  # 
+00004450: 7461 7267 6574 2063 6861 6e67 650a 2020  target change.  
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 2020 2763 6f64 6527 3a20 3330        'code': 30
+00004480: 312c 2020 2320 7374 6174 7573 5f63 6f64  1,  # status_cod
+00004490: 6520 6368 616e 6765 0a20 2020 2020 2020  e change.       
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044b0: 2027 6d61 736b 696e 6727 3a20 2732 272c   'masking': '2',
+000044c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000044d0: 2020 2020 2020 2020 2027 7175 6572 7927           'query'
+000044e0: 3a20 302c 0a20 2020 2020 2020 2020 2020  : 0,.           
+000044f0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00004500: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00004510: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00004520: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00004530: 706c 616e 203d 2070 726f 7669 6465 722e  plan = provider.
+00004540: 706c 616e 2877 616e 7465 6429 0a20 2020  plan(wanted).   
+00004550: 2020 2020 2023 206f 6e6c 7920 7365 6520       # only see 
+00004560: 7468 6520 6465 6c65 7465 2026 2074 746c  the delete & ttl
+00004570: 2075 7064 6174 652c 2062 656c 6f77 206d   update, below m
+00004580: 696e 2d74 746c 2069 7320 6669 6c74 6572  in-ttl is filter
+00004590: 6564 206f 7574 0a20 2020 2020 2020 2073  ed out.        s
+000045a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000045b0: 342c 206c 656e 2870 6c61 6e2e 6368 616e  4, len(plan.chan
+000045c0: 6765 7329 290a 2020 2020 2020 2020 7365  ges)).        se
+000045d0: 6c66 2e61 7373 6572 7445 7175 616c 2834  lf.assertEqual(4
+000045e0: 2c20 7072 6f76 6964 6572 2e61 7070 6c79  , provider.apply
+000045f0: 2870 6c61 6e29 290a 2020 2020 2020 2020  (plan)).        
+00004600: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+00004610: 706c 616e 2e65 7869 7374 7329 0a20 2020  plan.exists).   
+00004620: 2020 2020 2023 2063 7265 6174 6573 2061       # creates a
+00004630: 2074 6865 206e 6577 2076 616c 7565 2061   the new value a
+00004640: 6e64 2074 6865 6e20 6465 6c65 7465 7320  nd then deletes 
+00004650: 616c 6c20 7468 6520 6f6c 640a 2020 2020  all the old.    
+00004660: 2020 2020 7072 6f76 6964 6572 2e5f 7265      provider._re
+00004670: 7175 6573 742e 6173 7365 7274 5f68 6173  quest.assert_has
+00004680: 5f63 616c 6c73 280a 2020 2020 2020 2020  _calls(.        
+00004690: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+000046a0: 2020 2020 2020 6361 6c6c 280a 2020 2020        call(.    
+000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046c0: 2744 454c 4554 4527 2c0a 2020 2020 2020  'DELETE',.      
+000046d0: 2020 2020 2020 2020 2020 2020 2020 272f                '/
+000046e0: 7a6f 6e65 732f 3432 2f70 6167 6572 756c  zones/42/pagerul
+000046f0: 6573 2f32 6139 3134 3162 3138 6666 6230  es/2a9141b18ffb0
+00004700: 6536 6165 6438 3236 3035 3065 6563 3937  e6aed826050eec97
+00004710: 3062 3827 2c0a 2020 2020 2020 2020 2020  0b8',.          
+00004720: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00004730: 2020 2020 2020 2020 2063 616c 6c28 0a20           call(. 
 00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 2027 5055 5427 2c0a 2020 2020 2020 2020   'PUT',.        
-00004760: 2020 2020 2020 2020 2020 2020 272f 7a6f              '/zo
-00004770: 6e65 732f 3432 2f64 6e73 5f72 6563 6f72  nes/42/dns_recor
-00004780: 6473 2f66 6331 3261 6233 3463 6435 3631  ds/fc12ab34cd561
-00004790: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
-000047a0: 3635 3527 2c0a 2020 2020 2020 2020 2020  655',.          
-000047b0: 2020 2020 2020 2020 2020 6461 7461 3d7b            data={
-000047c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000047d0: 2020 2020 2020 2020 2027 636f 6e74 656e           'conten
-000047e0: 7427 3a20 2733 2e32 2e33 2e34 272c 0a20  t': '3.2.3.4',. 
-000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
-00004810: 4127 2c0a 2020 2020 2020 2020 2020 2020  A',.            
-00004820: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
-00004830: 6527 3a20 2774 746c 2e75 6e69 742e 7465  e': 'ttl.unit.te
-00004840: 7374 7327 2c0a 2020 2020 2020 2020 2020  sts',.          
-00004850: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-00004860: 726f 7869 6564 273a 2046 616c 7365 2c0a  roxied': False,.
-00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 2020 2774 746c 273a 2033          'ttl': 3
-00004890: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-000048a0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000048b0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-000048c0: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-000048d0: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-000048e0: 2020 2020 2020 2020 2750 5554 272c 0a20          'PUT',. 
+00004750: 2020 2027 4445 4c45 5445 272c 0a20 2020     'DELETE',.   
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2027 2f7a 6f6e 6573 2f66 6631 3261 6233   '/zones/ff12ab3
+00004780: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+00004790: 3332 3239 3937 3635 302f 270a 2020 2020  322997650/'.    
+000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047b0: 2764 6e73 5f72 6563 6f72 6473 2f66 6331  'dns_records/fc1
+000047c0: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
+000047d0: 3261 6233 3332 3239 3937 3635 3327 2c0a  2ab3322997653',.
+000047e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000047f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00004800: 2020 2063 616c 6c28 0a20 2020 2020 2020     call(.       
+00004810: 2020 2020 2020 2020 2020 2020 2027 4445               'DE
+00004820: 4c45 5445 272c 0a20 2020 2020 2020 2020  LETE',.         
+00004830: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
+00004840: 6573 2f66 6631 3261 6233 3463 6435 3631  es/ff12ab34cd561
+00004850: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
+00004860: 3635 302f 270a 2020 2020 2020 2020 2020  650/'.          
+00004870: 2020 2020 2020 2020 2020 2764 6e73 5f72            'dns_r
+00004880: 6563 6f72 6473 2f66 6331 3261 6233 3463  ecords/fc12ab34c
+00004890: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
+000048a0: 3239 3937 3635 3427 2c0a 2020 2020 2020  2997654',.      
+000048b0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+000048c0: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+000048d0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+000048e0: 2020 2020 2020 2027 5055 5427 2c0a 2020         'PUT',.  
 000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 2020 2027 2f7a 6f6e 6573 2f34 322f 7061     '/zones/42/pa
-00004910: 6765 7275 6c65 732f 3261 3931 3430 6231  gerules/2a9140b1
-00004920: 3766 6662 3065 3661 6564 3832 3630 3439  7ffb0e6aed826049
-00004930: 6565 6339 3730 6237 272c 0a20 2020 2020  eec970b7',.     
-00004940: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004950: 6174 613d 7b0a 2020 2020 2020 2020 2020  ata={.          
-00004960: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00004970: 6172 6765 7473 273a 205b 0a20 2020 2020  argets': [.     
-00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004990: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049b0: 2020 2020 2020 2020 2027 7461 7267 6574           'target
-000049c0: 273a 2027 7572 6c27 2c0a 2020 2020 2020  ': 'url',.      
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 2020 2020 2020 2763 6f6e 7374            'const
-000049f0: 7261 696e 7427 3a20 7b0a 2020 2020 2020  raint': {.      
-00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a10: 2020 2020 2020 2020 2020 2020 2020 276f                'o
-00004a20: 7065 7261 746f 7227 3a20 276d 6174 6368  perator': 'match
-00004a30: 6573 272c 0a20 2020 2020 2020 2020 2020  es',.           
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 2020 2020 2020 2027 7661 6c75 6527           'value'
-00004a60: 3a20 2775 726c 6677 642e 756e 6974 2e74  : 'urlfwd.unit.t
-00004a70: 6573 7473 2f2a 272c 0a20 2020 2020 2020  ests/*',.       
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ab0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-00004ae0: 2020 2020 2020 2020 2020 2020 2027 6163               'ac
-00004af0: 7469 6f6e 7327 3a20 5b0a 2020 2020 2020  tions': [.      
-00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b10: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00004b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b30: 2020 2020 2020 2020 2769 6427 3a20 2766          'id': 'f
-00004b40: 6f72 7761 7264 696e 675f 7572 6c27 2c0a  orwarding_url',.
-00004b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004900: 2020 272f 7a6f 6e65 732f 3432 2f64 6e73    '/zones/42/dns
+00004910: 5f72 6563 6f72 6473 2f66 6331 3261 6233  _records/fc12ab3
+00004920: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+00004930: 3332 3239 3937 3635 3527 2c0a 2020 2020  322997655',.    
+00004940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004950: 6461 7461 3d7b 0a20 2020 2020 2020 2020  data={.         
+00004960: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004970: 636f 6e74 656e 7427 3a20 2733 2e32 2e33  content': '3.2.3
+00004980: 2e34 272c 0a20 2020 2020 2020 2020 2020  .4',.           
+00004990: 2020 2020 2020 2020 2020 2020 2027 7479               'ty
+000049a0: 7065 273a 2027 4127 2c0a 2020 2020 2020  pe': 'A',.      
+000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049c0: 2020 276e 616d 6527 3a20 2774 746c 2e75    'name': 'ttl.u
+000049d0: 6e69 742e 7465 7374 7327 2c0a 2020 2020  nit.tests',.    
+000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049f0: 2020 2020 2770 726f 7869 6564 273a 2046      'proxied': F
+00004a00: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2774                't
+00004a20: 746c 273a 2033 3030 2c0a 2020 2020 2020  tl': 300,.      
+00004a30: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00004a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004a50: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00004a60: 2020 2020 6361 6c6c 280a 2020 2020 2020      call(.      
+00004a70: 2020 2020 2020 2020 2020 2020 2020 2750                'P
+00004a80: 5554 272c 0a20 2020 2020 2020 2020 2020  UT',.           
+00004a90: 2020 2020 2020 2020 2027 2f7a 6f6e 6573           '/zones
+00004aa0: 2f34 322f 7061 6765 7275 6c65 732f 3261  /42/pagerules/2a
+00004ab0: 3931 3430 6231 3766 6662 3065 3661 6564  9140b17ffb0e6aed
+00004ac0: 3832 3630 3439 6565 6339 3730 6237 272c  826049eec970b7',
+00004ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ae0: 2020 2020 2064 6174 613d 7b0a 2020 2020       data={.    
+00004af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b00: 2020 2020 2774 6172 6765 7473 273a 205b      'targets': [
+00004b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b20: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004b50: 7461 7267 6574 273a 2027 7572 6c27 2c0a  target': 'url',.
 00004b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b70: 2776 616c 7565 273a 207b 0a20 2020 2020  'value': {.     
-00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00004ba0: 7572 6c27 3a20 2768 7474 7073 3a2f 2f77  url': 'https://w
-00004bb0: 7777 2e75 6e69 742e 7465 7374 732f 272c  ww.unit.tests/',
-00004bc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b80: 2763 6f6e 7374 7261 696e 7427 3a20 7b0a  'constraint': {.
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bb0: 2020 2020 276f 7065 7261 746f 7227 3a20      'operator': 
+00004bc0: 276d 6174 6368 6573 272c 0a20 2020 2020  'matches',.     
 00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2020 2020 2027 7374 6174 7573 5f63 6f64       'status_cod
-00004bf0: 6527 3a20 3330 312c 0a20 2020 2020 2020  e': 301,.       
-00004c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c10: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-00004c60: 2020 2020 2020 2020 2020 2020 2027 7374               'st
-00004c70: 6174 7573 273a 2027 6163 7469 7665 272c  atus': 'active',
-00004c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004c90: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00004ca0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00004cb0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00004cc0: 2029 0a0a 2020 2020 2020 2020 2320 5275   )..        # Ru
-00004cd0: 6e20 7468 6520 6261 7369 6320 6170 706c  n the basic appl
-00004ce0: 7920 7465 7374 7320 6275 7420 7769 7468  y tests but with
-00004cf0: 2061 6e20 6163 636f 756e 745f 6964 0a20   an account_id. 
-00004d00: 2020 2020 2020 2070 726f 7669 6465 7220         provider 
-00004d10: 3d20 436c 6f75 6466 6c61 7265 5072 6f76  = CloudflareProv
-00004d20: 6964 6572 280a 2020 2020 2020 2020 2020  ider(.          
-00004d30: 2020 2774 6573 7427 2c0a 2020 2020 2020    'test',.      
-00004d40: 2020 2020 2020 2765 6d61 696c 272c 0a20        'email',. 
-00004d50: 2020 2020 2020 2020 2020 2027 746f 6b65             'toke
-00004d60: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00004d70: 6163 636f 756e 745f 6964 3d27 3333 3432  account_id='3342
-00004d80: 3334 3234 3334 3233 6161 6162 6233 3334  34243423aaabb334
-00004d90: 3334 3261 6161 3334 3334 3333 272c 0a20  342aaa343433',. 
-00004da0: 2020 2020 2020 2020 2020 2072 6574 7279             retry
-00004db0: 5f70 6572 696f 643d 302c 0a20 2020 2020  _period=0,.     
-00004dc0: 2020 2020 2020 2073 7472 6963 745f 7375         strict_su
-00004dd0: 7070 6f72 7473 3d46 616c 7365 2c0a 2020  pports=False,.  
-00004de0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00004df0: 2070 726f 7669 6465 722e 5f72 6571 7565   provider._reque
-00004e00: 7374 203d 204d 6f63 6b28 290a 0a20 2020  st = Mock()..   
-00004e10: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
-00004e20: 6571 7565 7374 2e73 6964 655f 6566 6665  equest.side_effe
-00004e30: 6374 203d 205b 0a20 2020 2020 2020 2020  ct = [.         
-00004e40: 2020 2073 656c 662e 656d 7074 792c 2020     self.empty,  
-00004e50: 2320 6e6f 207a 6f6e 6573 0a20 2020 2020  # no zones.     
-00004e60: 2020 2020 2020 207b 2772 6573 756c 7427         {'result'
-00004e70: 3a20 7b27 6964 273a 2034 327d 7d2c 2020  : {'id': 42}},  
-00004e80: 2320 7a6f 6e65 2063 7265 6174 650a 2020  # zone create.  
-00004e90: 2020 2020 2020 5d20 2b20 5b0a 2020 2020        ] + [.    
-00004ea0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-00004eb0: 2020 2020 205d 202a 2033 3020 2023 2069       ] * 30  # i
-00004ec0: 6e64 6976 6964 7561 6c20 7265 636f 7264  ndividual record
-00004ed0: 2063 7265 6174 6573 0a0a 2020 2020 2020   creates..      
-00004ee0: 2020 2320 6e6f 6e2d 6578 6973 7465 6e74    # non-existent
-00004ef0: 207a 6f6e 652c 2063 7265 6174 6520 6576   zone, create ev
-00004f00: 6572 7974 6869 6e67 0a20 2020 2020 2020  erything.       
-00004f10: 2070 6c61 6e20 3d20 7072 6f76 6964 6572   plan = provider
-00004f20: 2e70 6c61 6e28 7365 6c66 2e65 7870 6563  .plan(self.expec
-00004f30: 7465 6429 0a20 2020 2020 2020 2073 656c  ted).        sel
-00004f40: 662e 6173 7365 7274 4571 7561 6c28 3138  f.assertEqual(18
-00004f50: 2c20 6c65 6e28 706c 616e 2e63 6861 6e67  , len(plan.chang
-00004f60: 6573 2929 0a20 2020 2020 2020 2073 656c  es)).        sel
-00004f70: 662e 6173 7365 7274 4571 7561 6c28 3138  f.assertEqual(18
-00004f80: 2c20 7072 6f76 6964 6572 2e61 7070 6c79  , provider.apply
-00004f90: 2870 6c61 6e29 290a 2020 2020 2020 2020  (plan)).        
-00004fa0: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
-00004fb0: 2870 6c61 6e2e 6578 6973 7473 290a 0a20  (plan.exists).. 
-00004fc0: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00004fd0: 5f72 6571 7565 7374 2e61 7373 6572 745f  _request.assert_
-00004fe0: 6861 735f 6361 6c6c 7328 0a20 2020 2020  has_calls(.     
-00004ff0: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
-00005000: 2020 2020 2020 2020 2023 2063 7265 6174           # creat
-00005010: 6564 2074 6865 2064 6f6d 6169 6e0a 2020  ed the domain.  
-00005020: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00005030: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00005040: 2020 2020 2020 2020 2750 4f53 5427 2c0a          'POST',.
-00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005060: 2020 2020 272f 7a6f 6e65 7327 2c0a 2020      '/zones',.  
-00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005080: 2020 6461 7461 3d7b 0a20 2020 2020 2020    data={.       
-00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050a0: 2027 6a75 6d70 5f73 7461 7274 273a 2046   'jump_start': F
-000050b0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000050c0: 2020 2020 2020 2020 2020 2020 2020 276e                'n
-000050d0: 616d 6527 3a20 2775 6e69 742e 7465 7374  ame': 'unit.test
-000050e0: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-000050f0: 2020 2020 2020 2020 2020 2020 2761 6363              'acc
-00005100: 6f75 6e74 273a 207b 2769 6427 3a20 2733  ount': {'id': '3
-00005110: 3334 3233 3432 3433 3432 3361 6161 6262  34234243423aaabb
-00005120: 3333 3433 3432 6161 6133 3433 3433 3327  334342aaa343433'
-00005130: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00005140: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00005150: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00005160: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-00005170: 7265 6174 6564 2061 7420 6c65 6173 7420  reated at least 
-00005180: 6f6e 6520 6f66 2074 6865 2072 6563 6f72  one of the recor
-00005190: 6420 7769 7468 2065 7870 6563 7465 6420  d with expected 
-000051a0: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
-000051b0: 2020 2020 2063 616c 6c28 0a20 2020 2020       call(.     
-000051c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000051d0: 504f 5354 272c 0a20 2020 2020 2020 2020  POST',.         
-000051e0: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
-000051f0: 6573 2f34 322f 646e 735f 7265 636f 7264  es/42/dns_record
+00004be0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00004bf0: 7661 6c75 6527 3a20 2775 726c 6677 642e  value': 'urlfwd.
+00004c00: 756e 6974 2e74 6573 7473 2f2a 272c 0a20  unit.tests/*',. 
+00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c20: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00004c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004c40: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c80: 2020 2027 6163 7469 6f6e 7327 3a20 5b0a     'actions': [.
+00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ca0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2769                'i
+00004cd0: 6427 3a20 2766 6f72 7761 7264 696e 675f  d': 'forwarding_
+00004ce0: 7572 6c27 2c0a 2020 2020 2020 2020 2020  url',.          
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d00: 2020 2020 2020 2776 616c 7565 273a 207b        'value': {
+00004d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d30: 2020 2020 2027 7572 6c27 3a20 2768 7474       'url': 'htt
+00004d40: 7073 3a2f 2f77 7777 2e75 6e69 742e 7465  ps://www.unit.te
+00004d50: 7374 732f 272c 0a20 2020 2020 2020 2020  sts/',.         
+00004d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d70: 2020 2020 2020 2020 2020 2027 7374 6174             'stat
+00004d80: 7573 5f63 6f64 6527 3a20 3330 312c 0a20  us_code': 301,. 
+00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004da0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00004db0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00004dc0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004de0: 2020 2020 2020 2020 5d2c 0a20 2020 2020          ],.     
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e00: 2020 2027 7374 6174 7573 273a 2027 6163     'status': 'ac
+00004e10: 7469 7665 272c 0a20 2020 2020 2020 2020  tive',.         
+00004e20: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+00004e30: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00004e40: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00004e50: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00004e60: 2020 2320 5275 6e20 7468 6520 6261 7369    # Run the basi
+00004e70: 6320 6170 706c 7920 7465 7374 7320 6275  c apply tests bu
+00004e80: 7420 7769 7468 2061 6e20 6163 636f 756e  t with an accoun
+00004e90: 745f 6964 0a20 2020 2020 2020 2070 726f  t_id.        pro
+00004ea0: 7669 6465 7220 3d20 436c 6f75 6466 6c61  vider = Cloudfla
+00004eb0: 7265 5072 6f76 6964 6572 280a 2020 2020  reProvider(.    
+00004ec0: 2020 2020 2020 2020 2774 6573 7427 2c0a          'test',.
+00004ed0: 2020 2020 2020 2020 2020 2020 2765 6d61              'ema
+00004ee0: 696c 272c 0a20 2020 2020 2020 2020 2020  il',.           
+00004ef0: 2027 746f 6b65 6e27 2c0a 2020 2020 2020   'token',.      
+00004f00: 2020 2020 2020 6163 636f 756e 745f 6964        account_id
+00004f10: 3d27 3333 3432 3334 3234 3334 3233 6161  ='334234243423aa
+00004f20: 6162 6233 3334 3334 3261 6161 3334 3334  abb334342aaa3434
+00004f30: 3333 272c 0a20 2020 2020 2020 2020 2020  33',.           
+00004f40: 2072 6574 7279 5f70 6572 696f 643d 302c   retry_period=0,
+00004f50: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00004f60: 6963 745f 7375 7070 6f72 7473 3d46 616c  ict_supports=Fal
+00004f70: 7365 2c0a 2020 2020 2020 2020 290a 0a20  se,.        ).. 
+00004f80: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
+00004f90: 5f72 6571 7565 7374 203d 204d 6f63 6b28  _request = Mock(
+00004fa0: 290a 0a20 2020 2020 2020 2070 726f 7669  )..        provi
+00004fb0: 6465 722e 5f72 6571 7565 7374 2e73 6964  der._request.sid
+00004fc0: 655f 6566 6665 6374 203d 205b 0a20 2020  e_effect = [.   
+00004fd0: 2020 2020 2020 2020 2073 656c 662e 656d           self.em
+00004fe0: 7074 792c 2020 2320 6e6f 207a 6f6e 6573  pty,  # no zones
+00004ff0: 0a20 2020 2020 2020 2020 2020 207b 2772  .            {'r
+00005000: 6573 756c 7427 3a20 7b27 6964 273a 2034  esult': {'id': 4
+00005010: 327d 7d2c 2020 2320 7a6f 6e65 2063 7265  2}},  # zone cre
+00005020: 6174 650a 2020 2020 2020 2020 5d20 2b20  ate.        ] + 
+00005030: 5b0a 2020 2020 2020 2020 2020 2020 4e6f  [.            No
+00005040: 6e65 0a20 2020 2020 2020 205d 202a 2033  ne.        ] * 3
+00005050: 3020 2023 2069 6e64 6976 6964 7561 6c20  0  # individual 
+00005060: 7265 636f 7264 2063 7265 6174 6573 0a0a  record creates..
+00005070: 2020 2020 2020 2020 2320 6e6f 6e2d 6578          # non-ex
+00005080: 6973 7465 6e74 207a 6f6e 652c 2063 7265  istent zone, cre
+00005090: 6174 6520 6576 6572 7974 6869 6e67 0a20  ate everything. 
+000050a0: 2020 2020 2020 2070 6c61 6e20 3d20 7072         plan = pr
+000050b0: 6f76 6964 6572 2e70 6c61 6e28 7365 6c66  ovider.plan(self
+000050c0: 2e65 7870 6563 7465 6429 0a20 2020 2020  .expected).     
+000050d0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+000050e0: 7561 6c28 3138 2c20 6c65 6e28 706c 616e  ual(18, len(plan
+000050f0: 2e63 6861 6e67 6573 2929 0a20 2020 2020  .changes)).     
+00005100: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00005110: 7561 6c28 3138 2c20 7072 6f76 6964 6572  ual(18, provider
+00005120: 2e61 7070 6c79 2870 6c61 6e29 290a 2020  .apply(plan)).  
+00005130: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00005140: 7446 616c 7365 2870 6c61 6e2e 6578 6973  tFalse(plan.exis
+00005150: 7473 290a 0a20 2020 2020 2020 2070 726f  ts)..        pro
+00005160: 7669 6465 722e 5f72 6571 7565 7374 2e61  vider._request.a
+00005170: 7373 6572 745f 6861 735f 6361 6c6c 7328  ssert_has_calls(
+00005180: 0a20 2020 2020 2020 2020 2020 205b 0a20  .            [. 
+00005190: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+000051a0: 2063 7265 6174 6564 2074 6865 2064 6f6d   created the dom
+000051b0: 6169 6e0a 2020 2020 2020 2020 2020 2020  ain.            
+000051c0: 2020 2020 6361 6c6c 280a 2020 2020 2020      call(.      
+000051d0: 2020 2020 2020 2020 2020 2020 2020 2750                'P
+000051e0: 4f53 5427 2c0a 2020 2020 2020 2020 2020  OST',.          
+000051f0: 2020 2020 2020 2020 2020 272f 7a6f 6e65            '/zone
 00005200: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
 00005210: 2020 2020 2020 2020 6461 7461 3d7b 0a20          data={. 
 00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005230: 2020 2020 2020 2027 636f 6e74 656e 7427         'content'
-00005240: 3a20 276e 7331 2e75 6e69 742e 7465 7374  : 'ns1.unit.test
-00005250: 732e 272c 0a20 2020 2020 2020 2020 2020  s.',.           
-00005260: 2020 2020 2020 2020 2020 2020 2027 7479               'ty
-00005270: 7065 273a 2027 4e53 272c 0a20 2020 2020  pe': 'NS',.     
+00005230: 2020 2020 2020 2027 6a75 6d70 5f73 7461         'jump_sta
+00005240: 7274 273a 2046 616c 7365 2c0a 2020 2020  rt': False,.    
+00005250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005260: 2020 2020 276e 616d 6527 3a20 2775 6e69      'name': 'uni
+00005270: 742e 7465 7374 7327 2c0a 2020 2020 2020  t.tests',.      
 00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005290: 2020 2027 6e61 6d65 273a 2027 756e 6465     'name': 'unde
-000052a0: 722e 756e 6974 2e74 6573 7473 272c 0a20  r.unit.tests',. 
-000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052c0: 2020 2020 2020 2027 7474 6c27 3a20 3336         'ttl': 36
-000052d0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-000052e0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000052f0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00005300: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00005310: 6d61 6b65 2073 7572 6520 7365 6d69 636f  make sure semico
-00005320: 6c6f 6e73 2061 7265 206e 6f74 2065 7363  lons are not esc
-00005330: 6170 6564 2077 6865 6e20 7365 6e64 696e  aped when sendin
-00005340: 6720 6461 7461 0a20 2020 2020 2020 2020  g data.         
-00005350: 2020 2020 2020 2063 616c 6c28 0a20 2020         call(.   
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 2027 504f 5354 272c 0a20 2020 2020 2020   'POST',.       
-00005380: 2020 2020 2020 2020 2020 2020 2027 2f7a               '/z
-00005390: 6f6e 6573 2f34 322f 646e 735f 7265 636f  ones/42/dns_reco
-000053a0: 7264 7327 2c0a 2020 2020 2020 2020 2020  rds',.          
-000053b0: 2020 2020 2020 2020 2020 6461 7461 3d7b            data={
-000053c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000053d0: 2020 2020 2020 2020 2027 636f 6e74 656e           'conten
-000053e0: 7427 3a20 2776 3d44 4b49 4d31 3b6b 3d72  t': 'v=DKIM1;k=r
-000053f0: 7361 3b73 3d65 6d61 696c 3b68 3d73 6861  sa;s=email;h=sha
-00005400: 3235 363b 270a 2020 2020 2020 2020 2020  256;'.          
-00005410: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-00005420: 3d41 2f6b 696e 6461 2b6f 662f 6c6f 6e67  =A/kinda+of/long
-00005430: 2f73 7472 696e 672b 7769 7468 2b6e 756d  /string+with+num
-00005440: 6233 7273 272c 0a20 2020 2020 2020 2020  b3rs',.         
-00005450: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005460: 7479 7065 273a 2027 5458 5427 2c0a 2020  type': 'TXT',.  
-00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005480: 2020 2020 2020 276e 616d 6527 3a20 2774        'name': 't
-00005490: 7874 2e75 6e69 742e 7465 7374 7327 2c0a  xt.unit.tests',.
-000054a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054b0: 2020 2020 2020 2020 2774 746c 273a 2036          'ttl': 6
-000054c0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-000054d0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000054e0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-000054f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00005500: 6372 6561 7465 2061 7420 6c65 6173 7420  create at least 
-00005510: 6f6e 6520 7061 6765 7275 6c65 730a 2020  one pagerules.  
-00005520: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00005530: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00005540: 2020 2020 2020 2020 2750 4f53 5427 2c0a          'POST',.
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 2020 2020 272f 7a6f 6e65 732f 3432 2f70      '/zones/42/p
-00005570: 6167 6572 756c 6573 272c 0a20 2020 2020  agerules',.     
-00005580: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005590: 6174 613d 7b0a 2020 2020 2020 2020 2020  ata={.          
-000055a0: 2020 2020 2020 2020 2020 2020 2020 2774                't
-000055b0: 6172 6765 7473 273a 205b 0a20 2020 2020  argets': [.     
-000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055d0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00005290: 2020 2761 6363 6f75 6e74 273a 207b 2769    'account': {'i
+000052a0: 6427 3a20 2733 3334 3233 3432 3433 3432  d': '33423424342
+000052b0: 3361 6161 6262 3333 3433 3432 6161 6133  3aaabb334342aaa3
+000052c0: 3433 3433 3327 7d2c 0a20 2020 2020 2020  43433'},.       
+000052d0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00005300: 2020 2023 2063 7265 6174 6564 2061 7420     # created at 
+00005310: 6c65 6173 7420 6f6e 6520 6f66 2074 6865  least one of the
+00005320: 2072 6563 6f72 6420 7769 7468 2065 7870   record with exp
+00005330: 6563 7465 6420 6461 7461 0a20 2020 2020  ected data.     
+00005340: 2020 2020 2020 2020 2020 2063 616c 6c28             call(
+00005350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005360: 2020 2020 2027 504f 5354 272c 0a20 2020       'POST',.   
+00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 2027 2f7a 6f6e 6573 2f34 322f 646e 735f   '/zones/42/dns_
+00005390: 7265 636f 7264 7327 2c0a 2020 2020 2020  records',.      
+000053a0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000053b0: 7461 3d7b 0a20 2020 2020 2020 2020 2020  ta={.           
+000053c0: 2020 2020 2020 2020 2020 2020 2027 636f               'co
+000053d0: 6e74 656e 7427 3a20 276e 7331 2e75 6e69  ntent': 'ns1.uni
+000053e0: 742e 7465 7374 732e 272c 0a20 2020 2020  t.tests.',.     
+000053f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005400: 2020 2027 7479 7065 273a 2027 4e53 272c     'type': 'NS',
+00005410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005420: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
+00005430: 2027 756e 6465 722e 756e 6974 2e74 6573   'under.unit.tes
+00005440: 7473 272c 0a20 2020 2020 2020 2020 2020  ts',.           
+00005450: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
+00005460: 6c27 3a20 3336 3030 2c0a 2020 2020 2020  l': 3600,.      
+00005470: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00005480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005490: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+000054a0: 2020 2020 2320 6d61 6b65 2073 7572 6520      # make sure 
+000054b0: 7365 6d69 636f 6c6f 6e73 2061 7265 206e  semicolons are n
+000054c0: 6f74 2065 7363 6170 6564 2077 6865 6e20  ot escaped when 
+000054d0: 7365 6e64 696e 6720 6461 7461 0a20 2020  sending data.   
+000054e0: 2020 2020 2020 2020 2020 2020 2063 616c               cal
+000054f0: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00005500: 2020 2020 2020 2027 504f 5354 272c 0a20         'POST',. 
+00005510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005520: 2020 2027 2f7a 6f6e 6573 2f34 322f 646e     '/zones/42/dn
+00005530: 735f 7265 636f 7264 7327 2c0a 2020 2020  s_records',.    
+00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005550: 6461 7461 3d7b 0a20 2020 2020 2020 2020  data={.         
+00005560: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005570: 636f 6e74 656e 7427 3a20 2776 3d44 4b49  content': 'v=DKI
+00005580: 4d31 3b6b 3d72 7361 3b73 3d65 6d61 696c  M1;k=rsa;s=email
+00005590: 3b68 3d73 6861 3235 363b 270a 2020 2020  ;h=sha256;'.    
+000055a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055b0: 2020 2020 2770 3d41 2f6b 696e 6461 2b6f      'p=A/kinda+o
+000055c0: 662f 6c6f 6e67 2f73 7472 696e 672b 7769  f/long/string+wi
+000055d0: 7468 2b6e 756d 6233 7273 272c 0a20 2020  th+numb3rs',.   
 000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055f0: 2020 2020 2020 2020 2027 7461 7267 6574           'target
-00005600: 273a 2027 7572 6c27 2c0a 2020 2020 2020  ': 'url',.      
-00005610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005620: 2020 2020 2020 2020 2020 2763 6f6e 7374            'const
-00005630: 7261 696e 7427 3a20 7b0a 2020 2020 2020  raint': {.      
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005650: 2020 2020 2020 2020 2020 2020 2020 276f                'o
-00005660: 7065 7261 746f 7227 3a20 276d 6174 6368  perator': 'match
-00005670: 6573 272c 0a20 2020 2020 2020 2020 2020  es',.           
-00005680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005690: 2020 2020 2020 2020 2027 7661 6c75 6527           'value'
-000056a0: 3a20 2775 726c 6677 642e 756e 6974 2e74  : 'urlfwd.unit.t
-000056b0: 6573 7473 2f27 2c0a 2020 2020 2020 2020  ests/',.        
-000056c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056d0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005710: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00005720: 2020 2020 2020 2020 2020 2020 2761 6374              'act
-00005730: 696f 6e73 273a 205b 0a20 2020 2020 2020  ions': [.       
-00005740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005750: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 2020 2027 6964 273a 2027 666f         'id': 'fo
-00005780: 7277 6172 6469 6e67 5f75 726c 272c 0a20  rwarding_url',. 
-00005790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000057b0: 7661 6c75 6527 3a20 7b0a 2020 2020 2020  value': {.      
-000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2775                'u
-000057e0: 726c 273a 2027 6874 7470 3a2f 2f77 7777  rl': 'http://www
-000057f0: 2e75 6e69 742e 7465 7374 7327 2c0a 2020  .unit.tests',.  
-00005800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 2027 7479 7065 273a 2027 5458       'type': 'TX
+00005600: 5427 2c0a 2020 2020 2020 2020 2020 2020  T',.            
+00005610: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
+00005620: 6527 3a20 2774 7874 2e75 6e69 742e 7465  e': 'txt.unit.te
+00005630: 7374 7327 2c0a 2020 2020 2020 2020 2020  sts',.          
+00005640: 2020 2020 2020 2020 2020 2020 2020 2774                't
+00005650: 746c 273a 2036 3030 2c0a 2020 2020 2020  tl': 600,.      
+00005660: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00005670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005680: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00005690: 2020 2020 2320 6372 6561 7465 2061 7420      # create at 
+000056a0: 6c65 6173 7420 6f6e 6520 7061 6765 7275  least one pageru
+000056b0: 6c65 730a 2020 2020 2020 2020 2020 2020  les.            
+000056c0: 2020 2020 6361 6c6c 280a 2020 2020 2020      call(.      
+000056d0: 2020 2020 2020 2020 2020 2020 2020 2750                'P
+000056e0: 4f53 5427 2c0a 2020 2020 2020 2020 2020  OST',.          
+000056f0: 2020 2020 2020 2020 2020 272f 7a6f 6e65            '/zone
+00005700: 732f 3432 2f70 6167 6572 756c 6573 272c  s/42/pagerules',
+00005710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005720: 2020 2020 2064 6174 613d 7b0a 2020 2020       data={.    
+00005730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005740: 2020 2020 2774 6172 6765 7473 273a 205b      'targets': [
+00005750: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005760: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005790: 7461 7267 6574 273a 2027 7572 6c27 2c0a  target': 'url',.
+000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057c0: 2763 6f6e 7374 7261 696e 7427 3a20 7b0a  'constraint': {.
+000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057f0: 2020 2020 276f 7065 7261 746f 7227 3a20      'operator': 
+00005800: 276d 6174 6368 6573 272c 0a20 2020 2020  'matches',.     
 00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2773 7461 7475 735f 636f 6465 273a    'status_code':
-00005830: 2033 3032 2c0a 2020 2020 2020 2020 2020   302,.          
-00005840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005850: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
-00005880: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00005890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000058a0: 2020 2020 2020 2020 2020 2773 7461 7475            'statu
-000058b0: 7327 3a20 2761 6374 6976 6527 2c0a 2020  s': 'active',.  
-000058c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058d0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-000058e0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-000058f0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
-00005900: 2020 2054 7275 652c 0a20 2020 2020 2020     True,.       
-00005910: 2029 0a20 2020 2020 2020 2023 2065 7870   ).        # exp
-00005920: 6563 7465 6420 6e75 6d62 6572 206f 6620  ected number of 
-00005930: 746f 7461 6c20 6361 6c6c 730a 2020 2020  total calls.    
-00005940: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00005950: 7175 616c 2833 322c 2070 726f 7669 6465  qual(32, provide
-00005960: 722e 5f72 6571 7565 7374 2e63 616c 6c5f  r._request.call_
-00005970: 636f 756e 7429 0a0a 2020 2020 6465 6620  count)..    def 
-00005980: 7465 7374 5f75 7064 6174 655f 6164 645f  test_update_add_
-00005990: 7377 6170 2873 656c 6629 3a0a 2020 2020  swap(self):.    
-000059a0: 2020 2020 7072 6f76 6964 6572 203d 2043      provider = C
-000059b0: 6c6f 7564 666c 6172 6550 726f 7669 6465  loudflareProvide
-000059c0: 7228 2774 6573 7427 2c20 2765 6d61 696c  r('test', 'email
-000059d0: 272c 2027 746f 6b65 6e27 2c20 7265 7472  ', 'token', retr
-000059e0: 795f 7065 7269 6f64 3d30 290a 0a20 2020  y_period=0)..   
-000059f0: 2020 2020 2070 726f 7669 6465 722e 7a6f       provider.zo
-00005a00: 6e65 5f72 6563 6f72 6473 203d 204d 6f63  ne_records = Moc
-00005a10: 6b28 0a20 2020 2020 2020 2020 2020 2072  k(.            r
-00005a20: 6574 7572 6e5f 7661 6c75 653d 5b0a 2020  eturn_value=[.  
-00005a30: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2269 6422 3a20 2266 6331 3261      "id": "fc12a
-00005a60: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-00005a70: 6233 3332 3239 3937 3635 3322 2c0a 2020  b3322997653",.  
-00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2274 7970 6522 3a20 2241 222c 0a20    "type": "A",. 
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2022 6e61 6d65 223a 2022 612e 756e     "name": "a.un
-00005ac0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
-00005ad0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005ae0: 636f 6e74 656e 7422 3a20 2231 2e31 2e31  content": "1.1.1
-00005af0: 2e31 222c 0a20 2020 2020 2020 2020 2020  .1",.           
-00005b00: 2020 2020 2020 2020 2022 7072 6f78 6961           "proxia
-00005b10: 626c 6522 3a20 5472 7565 2c0a 2020 2020  ble": True,.    
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2270 726f 7869 6564 223a 2046 616c 7365  "proxied": False
-00005b40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005b50: 2020 2020 2020 2274 746c 223a 2033 3030        "ttl": 300
-00005b60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005b70: 2020 2020 2020 226c 6f63 6b65 6422 3a20        "locked": 
-00005b80: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00005b90: 2020 2020 2020 2020 2020 2022 7a6f 6e65             "zone
-00005ba0: 5f69 6422 3a20 2266 6631 3261 6233 3463  _id": "ff12ab34c
-00005bb0: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
-00005bc0: 3239 3937 3635 3022 2c0a 2020 2020 2020  2997650",.      
-00005bd0: 2020 2020 2020 2020 2020 2020 2020 227a                "z
-00005be0: 6f6e 655f 6e61 6d65 223a 2022 756e 6974  one_name": "unit
-00005bf0: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
-00005c00: 2020 2020 2020 2020 2020 2020 2022 6d6f               "mo
-00005c10: 6469 6669 6564 5f6f 6e22 3a20 2232 3031  dified_on": "201
-00005c20: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
-00005c30: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
-00005c40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005c50: 6372 6561 7465 645f 6f6e 223a 2022 3230  created_on": "20
-00005c60: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
-00005c70: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
-00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c90: 226d 6574 6122 3a20 7b22 6175 746f 5f61  "meta": {"auto_a
-00005ca0: 6464 6564 223a 2046 616c 7365 7d2c 0a20  dded": False},. 
-00005cb0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00005cc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005cd0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00005ce0: 2020 2020 2020 2020 2269 6422 3a20 2266          "id": "f
-00005cf0: 6331 3261 6233 3463 6435 3631 3133 3334  c12ab34cd5611334
-00005d00: 3432 3261 6233 3332 3239 3937 3635 3422  422ab3322997654"
-00005d10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005d20: 2020 2020 2020 2274 7970 6522 3a20 2241        "type": "A
-00005d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005d40: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-00005d50: 612e 756e 6974 2e74 6573 7473 222c 0a20  a.unit.tests",. 
+00005820: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00005830: 7661 6c75 6527 3a20 2775 726c 6677 642e  value': 'urlfwd.
+00005840: 756e 6974 2e74 6573 7473 2f27 2c0a 2020  unit.tests/',.  
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00005870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005880: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00005890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058a0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2761 6374 696f 6e73 273a 205b 0a20    'actions': [. 
+000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058e0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2020 2020 2020 2020 2020 2027 6964               'id
+00005910: 273a 2027 666f 7277 6172 6469 6e67 5f75  ': 'forwarding_u
+00005920: 726c 272c 0a20 2020 2020 2020 2020 2020  rl',.           
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 2027 7661 6c75 6527 3a20 7b0a       'value': {.
+00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005970: 2020 2020 2775 726c 273a 2027 6874 7470      'url': 'http
+00005980: 3a2f 2f77 7777 2e75 6e69 742e 7465 7374  ://www.unit.test
+00005990: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 2020 2020 2020 2020 2773 7461 7475 735f          'status_
+000059c0: 636f 6465 273a 2033 3032 2c0a 2020 2020  code': 302,.    
+000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059e0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000059f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a00: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
+00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a40: 2773 7461 7475 7327 3a20 2761 6374 6976  'status': 'activ
+00005a50: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00005a60: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00005a70: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00005a80: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+00005a90: 2020 2020 2020 2020 2054 7275 652c 0a20           True,. 
+00005aa0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005ab0: 2023 2065 7870 6563 7465 6420 6e75 6d62   # expected numb
+00005ac0: 6572 206f 6620 746f 7461 6c20 6361 6c6c  er of total call
+00005ad0: 730a 2020 2020 2020 2020 7365 6c66 2e61  s.        self.a
+00005ae0: 7373 6572 7445 7175 616c 2833 322c 2070  ssertEqual(32, p
+00005af0: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
+00005b00: 2e63 616c 6c5f 636f 756e 7429 0a0a 2020  .call_count)..  
+00005b10: 2020 6465 6620 7465 7374 5f75 7064 6174    def test_updat
+00005b20: 655f 6164 645f 7377 6170 2873 656c 6629  e_add_swap(self)
+00005b30: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
+00005b40: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
+00005b50: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
+00005b60: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
+00005b70: 2c20 7265 7472 795f 7065 7269 6f64 3d30  , retry_period=0
+00005b80: 290a 0a20 2020 2020 2020 2070 726f 7669  )..        provi
+00005b90: 6465 722e 7a6f 6e65 5f72 6563 6f72 6473  der.zone_records
+00005ba0: 203d 204d 6f63 6b28 0a20 2020 2020 2020   = Mock(.       
+00005bb0: 2020 2020 2072 6574 7572 6e5f 7661 6c75       return_valu
+00005bc0: 653d 5b0a 2020 2020 2020 2020 2020 2020  e=[.            
+00005bd0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00005be0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+00005bf0: 2266 6331 3261 6233 3463 6435 3631 3133  "fc12ab34cd56113
+00005c00: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
+00005c10: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
+00005c20: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00005c30: 2241 222c 0a20 2020 2020 2020 2020 2020  "A",.           
+00005c40: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+00005c50: 2022 612e 756e 6974 2e74 6573 7473 222c   "a.unit.tests",
+00005c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005c70: 2020 2020 2022 636f 6e74 656e 7422 3a20       "content": 
+00005c80: 2231 2e31 2e31 2e31 222c 0a20 2020 2020  "1.1.1.1",.     
+00005c90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00005ca0: 7072 6f78 6961 626c 6522 3a20 5472 7565  proxiable": True
+00005cb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005cc0: 2020 2020 2020 2270 726f 7869 6564 223a        "proxied":
+00005cd0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00005ce0: 2020 2020 2020 2020 2020 2020 2274 746c              "ttl
+00005cf0: 223a 2033 3030 2c0a 2020 2020 2020 2020  ": 300,.        
+00005d00: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
+00005d10: 6b65 6422 3a20 4661 6c73 652c 0a20 2020  ked": False,.   
+00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d30: 2022 7a6f 6e65 5f69 6422 3a20 2266 6631   "zone_id": "ff1
+00005d40: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
+00005d50: 3261 6233 3332 3239 3937 3635 3022 2c0a  2ab3322997650",.
 00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2020 2022 636f 6e74 656e 7422 3a20 2232     "content": "2
-00005d80: 2e32 2e32 2e32 222c 0a20 2020 2020 2020  .2.2.2",.       
-00005d90: 2020 2020 2020 2020 2020 2020 2022 7072               "pr
-00005da0: 6f78 6961 626c 6522 3a20 5472 7565 2c0a  oxiable": True,.
-00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dc0: 2020 2020 2270 726f 7869 6564 223a 2046      "proxied": F
-00005dd0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00005de0: 2020 2020 2020 2020 2020 2274 746c 223a            "ttl":
-00005df0: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
-00005e00: 2020 2020 2020 2020 2020 226c 6f63 6b65            "locke
-00005e10: 6422 3a20 4661 6c73 652c 0a20 2020 2020  d": False,.     
-00005e20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00005e30: 7a6f 6e65 5f69 6422 3a20 2266 6631 3261  zone_id": "ff12a
-00005e40: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-00005e50: 6233 3332 3239 3937 3635 3022 2c0a 2020  b3322997650",.  
-00005e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e70: 2020 227a 6f6e 655f 6e61 6d65 223a 2022    "zone_name": "
-00005e80: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-00005e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ea0: 2022 6d6f 6469 6669 6564 5f6f 6e22 3a20   "modified_on": 
-00005eb0: 2232 3031 372d 3033 2d31 3154 3138 3a30  "2017-03-11T18:0
-00005ec0: 313a 3433 2e34 3230 3638 395a 222c 0a20  1:43.420689Z",. 
-00005ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ee0: 2020 2022 6372 6561 7465 645f 6f6e 223a     "created_on":
-00005ef0: 2022 3230 3137 2d30 332d 3131 5431 383a   "2017-03-11T18:
-00005f00: 3031 3a34 332e 3432 3036 3839 5a22 2c0a  01:43.420689Z",.
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 2020 2020 226d 6574 6122 3a20 7b22 6175      "meta": {"au
-00005f30: 746f 5f61 6464 6564 223a 2046 616c 7365  to_added": False
-00005f40: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00005f50: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-00005f60: 2020 5d0a 2020 2020 2020 2020 290a 0a20    ].        ).. 
-00005f70: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00005f80: 5f72 6571 7565 7374 203d 204d 6f63 6b28  _request = Mock(
-00005f90: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
-00005fa0: 6572 2e5f 7265 7175 6573 742e 7369 6465  er._request.side
-00005fb0: 5f65 6666 6563 7420 3d20 5b0a 2020 2020  _effect = [.    
-00005fc0: 2020 2020 2020 2020 436c 6f75 6466 6c61          Cloudfla
-00005fd0: 7265 5261 7465 4c69 6d69 7445 7272 6f72  reRateLimitError
-00005fe0: 2827 7b7d 2729 2c0a 2020 2020 2020 2020  ('{}'),.        
-00005ff0: 2020 2020 7365 6c66 2e65 6d70 7479 2c20      self.empty, 
-00006000: 2023 206e 6f20 7a6f 6e65 730a 2020 2020   # no zones.    
-00006010: 2020 2020 2020 2020 7b27 7265 7375 6c74          {'result
-00006020: 273a 207b 2769 6427 3a20 3432 7d7d 2c20  ': {'id': 42}}, 
-00006030: 2023 207a 6f6e 6520 6372 6561 7465 0a20   # zone create. 
-00006040: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
-00006050: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
-00006060: 652c 0a20 2020 2020 2020 2020 2020 204e  e,.            N
-00006070: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00006080: 204e 6f6e 652c 0a20 2020 2020 2020 205d   None,.        ]
-00006090: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
-000060a0: 736f 6d65 7468 696e 6720 616e 6420 6465  something and de
-000060b0: 6c65 7465 2073 6f6d 6574 6869 6e67 0a20  lete something. 
-000060c0: 2020 2020 2020 207a 6f6e 6520 3d20 5a6f         zone = Zo
-000060d0: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
-000060e0: 2c20 5b5d 290a 2020 2020 2020 2020 6578  , []).        ex
-000060f0: 6973 7469 6e67 203d 2052 6563 6f72 642e  isting = Record.
-00006100: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
-00006110: 207a 6f6e 652c 0a20 2020 2020 2020 2020   zone,.         
-00006120: 2020 2027 6127 2c0a 2020 2020 2020 2020     'a',.        
-00006130: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00006140: 2020 2020 2020 2774 746c 273a 2033 3030        'ttl': 300
-00006150: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006160: 2020 2774 7970 6527 3a20 2741 272c 0a20    'type': 'A',. 
-00006170: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00006180: 2054 6869 7320 6d61 7463 6865 7320 7468   This matches th
-00006190: 6520 7a6f 6e65 2064 6174 6120 6162 6f76  e zone data abov
-000061a0: 652c 206f 6e65 2074 6f20 7377 6170 2c20  e, one to swap, 
-000061b0: 6f6e 6520 746f 206c 6561 7665 0a20 2020  one to leave.   
-000061c0: 2020 2020 2020 2020 2020 2020 2027 7661               'va
-000061d0: 6c75 6573 273a 205b 2731 2e31 2e31 2e31  lues': ['1.1.1.1
-000061e0: 272c 2027 322e 322e 322e 3227 5d2c 0a20  ', '2.2.2.2'],. 
-000061f0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00006200: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00006210: 6e65 7720 3d20 5265 636f 7264 2e6e 6577  new = Record.new
-00006220: 280a 2020 2020 2020 2020 2020 2020 7a6f  (.            zo
-00006230: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00006240: 2761 272c 0a20 2020 2020 2020 2020 2020  'a',.           
-00006250: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00006260: 2020 2027 7474 6c27 3a20 3330 302c 0a20     'ttl': 300,. 
-00006270: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006280: 7479 7065 273a 2027 4127 2c0a 2020 2020  type': 'A',.    
-00006290: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
-000062a0: 6973 206c 6561 7665 7320 6f6e 652c 2073  is leaves one, s
-000062b0: 7761 7073 206f 6e65 732c 2061 6e64 2061  waps ones, and a
-000062c0: 6464 7320 6f6e 650a 2020 2020 2020 2020  dds one.        
-000062d0: 2020 2020 2020 2020 2776 616c 7565 7327          'values'
-000062e0: 3a20 5b27 322e 322e 322e 3227 2c20 2733  : ['2.2.2.2', '3
-000062f0: 2e33 2e33 2e33 272c 2027 342e 342e 342e  .3.3.3', '4.4.4.
-00006300: 3427 5d2c 0a20 2020 2020 2020 2020 2020  4'],.           
-00006310: 207d 2c0a 2020 2020 2020 2020 290a 2020   },.        ).  
-00006320: 2020 2020 2020 6368 616e 6765 203d 2055        change = U
-00006330: 7064 6174 6528 6578 6973 7469 6e67 2c20  pdate(existing, 
-00006340: 6e65 7729 0a20 2020 2020 2020 2070 6c61  new).        pla
-00006350: 6e20 3d20 506c 616e 287a 6f6e 652c 207a  n = Plan(zone, z
-00006360: 6f6e 652c 205b 6368 616e 6765 5d2c 2054  one, [change], T
-00006370: 7275 6529 0a20 2020 2020 2020 2070 726f  rue).        pro
-00006380: 7669 6465 722e 5f61 7070 6c79 2870 6c61  vider._apply(pla
-00006390: 6e29 0a0a 2020 2020 2020 2020 2320 6765  n)..        # ge
-000063a0: 7420 7468 6520 6c69 7374 206f 6620 7a6f  t the list of zo
-000063b0: 6e65 732c 2063 7265 6174 6520 6120 7a6f  nes, create a zo
-000063c0: 6e65 2c20 6164 6420 736f 6d65 2072 6563  ne, add some rec
-000063d0: 6f72 6473 2c20 7570 6461 7465 0a20 2020  ords, update.   
-000063e0: 2020 2020 2023 2073 6f6d 6574 6869 6e67       # something
-000063f0: 2c20 616e 6420 6465 6c65 7465 2073 6f6d  , and delete som
-00006400: 6574 6869 6e67 0a20 2020 2020 2020 2070  ething.        p
-00006410: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
-00006420: 2e61 7373 6572 745f 6861 735f 6361 6c6c  .assert_has_call
-00006430: 7328 0a20 2020 2020 2020 2020 2020 205b  s(.            [
-00006440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006450: 2063 616c 6c28 2747 4554 272c 2027 2f7a   call('GET', '/z
-00006460: 6f6e 6573 272c 2070 6172 616d 733d 7b27  ones', params={'
-00006470: 7061 6765 273a 2031 2c20 2770 6572 5f70  page': 1, 'per_p
-00006480: 6167 6527 3a20 3530 7d29 2c0a 2020 2020  age': 50}),.    
-00006490: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
-000064a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000064b0: 2020 2020 2020 2750 4f53 5427 2c0a 2020        'POST',.  
-000064c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064d0: 2020 272f 7a6f 6e65 7327 2c0a 2020 2020    '/zones',.    
-000064e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064f0: 6461 7461 3d7b 276a 756d 705f 7374 6172  data={'jump_star
-00006500: 7427 3a20 4661 6c73 652c 2027 6e61 6d65  t': False, 'name
-00006510: 273a 2027 756e 6974 2e74 6573 7473 277d  ': 'unit.tests'}
-00006520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006530: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00006540: 2020 2020 2063 616c 6c28 0a20 2020 2020       call(.     
-00006550: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006560: 504f 5354 272c 0a20 2020 2020 2020 2020  POST',.         
-00006570: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
-00006580: 6573 2f34 322f 646e 735f 7265 636f 7264  es/42/dns_record
-00006590: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
-000065a0: 2020 2020 2020 2020 6461 7461 3d7b 0a20          data={. 
-000065b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065c0: 2020 2020 2020 2027 636f 6e74 656e 7427         'content'
-000065d0: 3a20 2734 2e34 2e34 2e34 272c 0a20 2020  : '4.4.4.4',.   
-000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065f0: 2020 2020 2027 7479 7065 273a 2027 4127       'type': 'A'
-00006600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006610: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
-00006620: 3a20 2761 2e75 6e69 742e 7465 7374 7327  : 'a.unit.tests'
-00006630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006640: 2020 2020 2020 2020 2020 2770 726f 7869            'proxi
-00006650: 6564 273a 2046 616c 7365 2c0a 2020 2020  ed': False,.    
-00006660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006670: 2020 2020 2774 746c 273a 2033 3030 2c0a      'ttl': 300,.
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000066a0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-000066b0: 2020 2020 2020 2020 2020 6361 6c6c 280a            call(.
-000066c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066d0: 2020 2020 2750 5554 272c 0a20 2020 2020      'PUT',.     
-000066e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000066f0: 2f7a 6f6e 6573 2f34 322f 646e 735f 7265  /zones/42/dns_re
-00006700: 636f 7264 732f 6663 3132 6162 3334 6364  cords/fc12ab34cd
-00006710: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
-00006720: 3939 3736 3534 272c 0a20 2020 2020 2020  997654',.       
-00006730: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00006740: 613d 7b0a 2020 2020 2020 2020 2020 2020  a={.            
-00006750: 2020 2020 2020 2020 2020 2020 2763 6f6e              'con
-00006760: 7465 6e74 273a 2027 322e 322e 322e 3227  tent': '2.2.2.2'
-00006770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006780: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
-00006790: 3a20 2741 272c 0a20 2020 2020 2020 2020  : 'A',.         
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000067b0: 6e61 6d65 273a 2027 612e 756e 6974 2e74  name': 'a.unit.t
-000067c0: 6573 7473 272c 0a20 2020 2020 2020 2020  ests',.         
-000067d0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-000067e0: 7072 6f78 6965 6427 3a20 4661 6c73 652c  proxied': False,
-000067f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006800: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
-00006810: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
-00006820: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00006830: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00006840: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00006850: 616c 6c28 0a20 2020 2020 2020 2020 2020  all(.           
-00006860: 2020 2020 2020 2020 2027 5055 5427 2c0a           'PUT',.
-00006870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006880: 2020 2020 272f 7a6f 6e65 732f 3432 2f64      '/zones/42/d
-00006890: 6e73 5f72 6563 6f72 6473 2f66 6331 3261  ns_records/fc12a
-000068a0: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-000068b0: 6233 3332 3239 3937 3635 3327 2c0a 2020  b3322997653',.  
+00005d70: 2020 2020 227a 6f6e 655f 6e61 6d65 223a      "zone_name":
+00005d80: 2022 756e 6974 2e74 6573 7473 222c 0a20   "unit.tests",. 
+00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005da0: 2020 2022 6d6f 6469 6669 6564 5f6f 6e22     "modified_on"
+00005db0: 3a20 2232 3031 372d 3033 2d31 3154 3138  : "2017-03-11T18
+00005dc0: 3a30 313a 3433 2e34 3230 3638 395a 222c  :01:43.420689Z",
+00005dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005de0: 2020 2020 2022 6372 6561 7465 645f 6f6e       "created_on
+00005df0: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
+00005e00: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
+00005e10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00005e20: 2020 2020 2020 226d 6574 6122 3a20 7b22        "meta": {"
+00005e30: 6175 746f 5f61 6464 6564 223a 2046 616c  auto_added": Fal
+00005e40: 7365 7d2c 0a20 2020 2020 2020 2020 2020  se},.           
+00005e50: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00005e60: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00005e80: 6422 3a20 2266 6331 3261 6233 3463 6435  d": "fc12ab34cd5
+00005e90: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
+00005ea0: 3937 3635 3422 2c0a 2020 2020 2020 2020  97654",.        
+00005eb0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00005ec0: 6522 3a20 2241 222c 0a20 2020 2020 2020  e": "A",.       
+00005ed0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+00005ee0: 6d65 223a 2022 612e 756e 6974 2e74 6573  me": "a.unit.tes
+00005ef0: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
+00005f00: 2020 2020 2020 2020 2022 636f 6e74 656e           "conten
+00005f10: 7422 3a20 2232 2e32 2e32 2e32 222c 0a20  t": "2.2.2.2",. 
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 2020 2022 7072 6f78 6961 626c 6522 3a20     "proxiable": 
+00005f40: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00005f50: 2020 2020 2020 2020 2020 2270 726f 7869            "proxi
+00005f60: 6564 223a 2046 616c 7365 2c0a 2020 2020  ed": False,.    
+00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f80: 2274 746c 223a 2033 3030 2c0a 2020 2020  "ttl": 300,.    
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 226c 6f63 6b65 6422 3a20 4661 6c73 652c  "locked": False,
+00005fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005fc0: 2020 2020 2022 7a6f 6e65 5f69 6422 3a20       "zone_id": 
+00005fd0: 2266 6631 3261 6233 3463 6435 3631 3133  "ff12ab34cd56113
+00005fe0: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
+00005ff0: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+00006000: 2020 2020 2020 2020 227a 6f6e 655f 6e61          "zone_na
+00006010: 6d65 223a 2022 756e 6974 2e74 6573 7473  me": "unit.tests
+00006020: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006030: 2020 2020 2020 2022 6d6f 6469 6669 6564         "modified
+00006040: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
+00006050: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
+00006060: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
+00006070: 2020 2020 2020 2020 2022 6372 6561 7465           "create
+00006080: 645f 6f6e 223a 2022 3230 3137 2d30 332d  d_on": "2017-03-
+00006090: 3131 5431 383a 3031 3a34 332e 3432 3036  11T18:01:43.4206
+000060a0: 3839 5a22 2c0a 2020 2020 2020 2020 2020  89Z",.          
+000060b0: 2020 2020 2020 2020 2020 226d 6574 6122            "meta"
+000060c0: 3a20 7b22 6175 746f 5f61 6464 6564 223a  : {"auto_added":
+000060d0: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+000060e0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+000060f0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00006100: 2020 290a 0a20 2020 2020 2020 2070 726f    )..        pro
+00006110: 7669 6465 722e 5f72 6571 7565 7374 203d  vider._request =
+00006120: 204d 6f63 6b28 290a 2020 2020 2020 2020   Mock().        
+00006130: 7072 6f76 6964 6572 2e5f 7265 7175 6573  provider._reques
+00006140: 742e 7369 6465 5f65 6666 6563 7420 3d20  t.side_effect = 
+00006150: 5b0a 2020 2020 2020 2020 2020 2020 436c  [.            Cl
+00006160: 6f75 6466 6c61 7265 5261 7465 4c69 6d69  oudflareRateLimi
+00006170: 7445 7272 6f72 2827 7b7d 2729 2c0a 2020  tError('{}'),.  
+00006180: 2020 2020 2020 2020 2020 7365 6c66 2e65            self.e
+00006190: 6d70 7479 2c20 2023 206e 6f20 7a6f 6e65  mpty,  # no zone
+000061a0: 730a 2020 2020 2020 2020 2020 2020 7b27  s.            {'
+000061b0: 7265 7375 6c74 273a 207b 2769 6427 3a20  result': {'id': 
+000061c0: 3432 7d7d 2c20 2023 207a 6f6e 6520 6372  42}},  # zone cr
+000061d0: 6561 7465 0a20 2020 2020 2020 2020 2020  eate.           
+000061e0: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+000061f0: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
+00006200: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
+00006210: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
+00006220: 2020 2020 205d 0a0a 2020 2020 2020 2020       ]..        
+00006230: 2320 4164 6420 736f 6d65 7468 696e 6720  # Add something 
+00006240: 616e 6420 6465 6c65 7465 2073 6f6d 6574  and delete somet
+00006250: 6869 6e67 0a20 2020 2020 2020 207a 6f6e  hing.        zon
+00006260: 6520 3d20 5a6f 6e65 2827 756e 6974 2e74  e = Zone('unit.t
+00006270: 6573 7473 2e27 2c20 5b5d 290a 2020 2020  ests.', []).    
+00006280: 2020 2020 6578 6973 7469 6e67 203d 2052      existing = R
+00006290: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
+000062a0: 2020 2020 2020 207a 6f6e 652c 0a20 2020         zone,.   
+000062b0: 2020 2020 2020 2020 2027 6127 2c0a 2020           'a',.  
+000062c0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000062d0: 2020 2020 2020 2020 2020 2020 2774 746c              'ttl
+000062e0: 273a 2033 3030 2c0a 2020 2020 2020 2020  ': 300,.        
+000062f0: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
+00006300: 2741 272c 0a20 2020 2020 2020 2020 2020  'A',.           
+00006310: 2020 2020 2023 2054 6869 7320 6d61 7463       # This matc
+00006320: 6865 7320 7468 6520 7a6f 6e65 2064 6174  hes the zone dat
+00006330: 6120 6162 6f76 652c 206f 6e65 2074 6f20  a above, one to 
+00006340: 7377 6170 2c20 6f6e 6520 746f 206c 6561  swap, one to lea
+00006350: 7665 0a20 2020 2020 2020 2020 2020 2020  ve.             
+00006360: 2020 2027 7661 6c75 6573 273a 205b 2731     'values': ['1
+00006370: 2e31 2e31 2e31 272c 2027 322e 322e 322e  .1.1.1', '2.2.2.
+00006380: 3227 5d2c 0a20 2020 2020 2020 2020 2020  2'],.           
+00006390: 207d 2c0a 2020 2020 2020 2020 290a 2020   },.        ).  
+000063a0: 2020 2020 2020 6e65 7720 3d20 5265 636f        new = Reco
+000063b0: 7264 2e6e 6577 280a 2020 2020 2020 2020  rd.new(.        
+000063c0: 2020 2020 7a6f 6e65 2c0a 2020 2020 2020      zone,.      
+000063d0: 2020 2020 2020 2761 272c 0a20 2020 2020        'a',.     
+000063e0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000063f0: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
+00006400: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
+00006410: 2020 2020 2027 7479 7065 273a 2027 4127       'type': 'A'
+00006420: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006430: 2020 2320 5468 6973 206c 6561 7665 7320    # This leaves 
+00006440: 6f6e 652c 2073 7761 7073 206f 6e65 732c  one, swaps ones,
+00006450: 2061 6e64 2061 6464 7320 6f6e 650a 2020   and adds one.  
+00006460: 2020 2020 2020 2020 2020 2020 2020 2776                'v
+00006470: 616c 7565 7327 3a20 5b27 322e 322e 322e  alues': ['2.2.2.
+00006480: 3227 2c20 2733 2e33 2e33 2e33 272c 2027  2', '3.3.3.3', '
+00006490: 342e 342e 342e 3427 5d2c 0a20 2020 2020  4.4.4.4'],.     
+000064a0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000064b0: 2020 290a 2020 2020 2020 2020 6368 616e    ).        chan
+000064c0: 6765 203d 2055 7064 6174 6528 6578 6973  ge = Update(exis
+000064d0: 7469 6e67 2c20 6e65 7729 0a20 2020 2020  ting, new).     
+000064e0: 2020 2070 6c61 6e20 3d20 506c 616e 287a     plan = Plan(z
+000064f0: 6f6e 652c 207a 6f6e 652c 205b 6368 616e  one, zone, [chan
+00006500: 6765 5d2c 2054 7275 6529 0a20 2020 2020  ge], True).     
+00006510: 2020 2070 726f 7669 6465 722e 5f61 7070     provider._app
+00006520: 6c79 2870 6c61 6e29 0a0a 2020 2020 2020  ly(plan)..      
+00006530: 2020 2320 6765 7420 7468 6520 6c69 7374    # get the list
+00006540: 206f 6620 7a6f 6e65 732c 2063 7265 6174   of zones, creat
+00006550: 6520 6120 7a6f 6e65 2c20 6164 6420 736f  e a zone, add so
+00006560: 6d65 2072 6563 6f72 6473 2c20 7570 6461  me records, upda
+00006570: 7465 0a20 2020 2020 2020 2023 2073 6f6d  te.        # som
+00006580: 6574 6869 6e67 2c20 616e 6420 6465 6c65  ething, and dele
+00006590: 7465 2073 6f6d 6574 6869 6e67 0a20 2020  te something.   
+000065a0: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
+000065b0: 6571 7565 7374 2e61 7373 6572 745f 6861  equest.assert_ha
+000065c0: 735f 6361 6c6c 7328 0a20 2020 2020 2020  s_calls(.       
+000065d0: 2020 2020 205b 0a20 2020 2020 2020 2020       [.         
+000065e0: 2020 2020 2020 2063 616c 6c28 2747 4554         call('GET
+000065f0: 272c 2027 2f7a 6f6e 6573 272c 2070 6172  ', '/zones', par
+00006600: 616d 733d 7b27 7061 6765 273a 2031 2c20  ams={'page': 1, 
+00006610: 2770 6572 5f70 6167 6527 3a20 3530 7d29  'per_page': 50})
+00006620: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006630: 2020 6361 6c6c 280a 2020 2020 2020 2020    call(.        
+00006640: 2020 2020 2020 2020 2020 2020 2750 4f53              'POS
+00006650: 5427 2c0a 2020 2020 2020 2020 2020 2020  T',.            
+00006660: 2020 2020 2020 2020 272f 7a6f 6e65 7327          '/zones'
+00006670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006680: 2020 2020 2020 6461 7461 3d7b 276a 756d        data={'jum
+00006690: 705f 7374 6172 7427 3a20 4661 6c73 652c  p_start': False,
+000066a0: 2027 6e61 6d65 273a 2027 756e 6974 2e74   'name': 'unit.t
+000066b0: 6573 7473 277d 2c0a 2020 2020 2020 2020  ests'},.        
+000066c0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+000066d0: 2020 2020 2020 2020 2020 2063 616c 6c28             call(
+000066e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000066f0: 2020 2020 2027 504f 5354 272c 0a20 2020       'POST',.   
+00006700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006710: 2027 2f7a 6f6e 6573 2f34 322f 646e 735f   '/zones/42/dns_
+00006720: 7265 636f 7264 7327 2c0a 2020 2020 2020  records',.      
+00006730: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00006740: 7461 3d7b 0a20 2020 2020 2020 2020 2020  ta={.           
+00006750: 2020 2020 2020 2020 2020 2020 2027 636f               'co
+00006760: 6e74 656e 7427 3a20 2734 2e34 2e34 2e34  ntent': '4.4.4.4
+00006770: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00006780: 2020 2020 2020 2020 2020 2027 7479 7065             'type
+00006790: 273a 2027 4127 2c0a 2020 2020 2020 2020  ': 'A',.        
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 276e 616d 6527 3a20 2761 2e75 6e69 742e  'name': 'a.unit.
+000067c0: 7465 7374 7327 2c0a 2020 2020 2020 2020  tests',.        
+000067d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067e0: 2770 726f 7869 6564 273a 2046 616c 7365  'proxied': False
+000067f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006800: 2020 2020 2020 2020 2020 2774 746c 273a            'ttl':
+00006810: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
+00006820: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00006830: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006850: 6361 6c6c 280a 2020 2020 2020 2020 2020  call(.          
+00006860: 2020 2020 2020 2020 2020 2750 5554 272c            'PUT',
+00006870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006880: 2020 2020 2027 2f7a 6f6e 6573 2f34 322f       '/zones/42/
+00006890: 646e 735f 7265 636f 7264 732f 6663 3132  dns_records/fc12
+000068a0: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
+000068b0: 6162 3333 3232 3939 3736 3534 272c 0a20  ab3322997654',. 
 000068c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068d0: 2020 6461 7461 3d7b 0a20 2020 2020 2020    data={.       
+000068d0: 2020 2064 6174 613d 7b0a 2020 2020 2020     data={.      
 000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2027 636f 6e74 656e 7427 3a20 2733 2e33   'content': '3.3
-00006900: 2e33 2e33 272c 0a20 2020 2020 2020 2020  .3.3',.         
-00006910: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00006920: 7479 7065 273a 2027 4127 2c0a 2020 2020  type': 'A',.    
+000068f0: 2020 2763 6f6e 7465 6e74 273a 2027 322e    'content': '2.
+00006900: 322e 322e 3227 2c0a 2020 2020 2020 2020  2.2.2',.        
+00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006920: 2774 7970 6527 3a20 2741 272c 0a20 2020  'type': 'A',.   
 00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006940: 2020 2020 276e 616d 6527 3a20 2761 2e75      'name': 'a.u
-00006950: 6e69 742e 7465 7374 7327 2c0a 2020 2020  nit.tests',.    
+00006940: 2020 2020 2027 6e61 6d65 273a 2027 612e       'name': 'a.
+00006950: 756e 6974 2e74 6573 7473 272c 0a20 2020  unit.tests',.   
 00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 2020 2020 2770 726f 7869 6564 273a 2046      'proxied': F
-00006980: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-00006990: 2020 2020 2020 2020 2020 2020 2020 2774                't
-000069a0: 746c 273a 2033 3030 2c0a 2020 2020 2020  tl': 300,.      
-000069b0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
-000069c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000069d0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-000069e0: 5d0a 2020 2020 2020 2020 290a 0a20 2020  ].        )..   
-000069f0: 2064 6566 2074 6573 745f 7570 6461 7465   def test_update
-00006a00: 5f64 656c 6574 6528 7365 6c66 293a 0a20  _delete(self):. 
-00006a10: 2020 2020 2020 2023 2057 6520 6e65 6564         # We need
-00006a20: 2061 6e6f 7468 6572 2072 756e 2073 6f20   another run so 
-00006a30: 7468 6174 2077 6520 6361 6e20 6465 6c65  that we can dele
-00006a40: 7465 2c20 7765 2063 616e 2774 2062 6f74  te, we can't bot
-00006a50: 6820 6164 6420 616e 640a 2020 2020 2020  h add and.      
-00006a60: 2020 2320 6465 6c65 7465 2069 6e20 6f6e    # delete in on
-00006a70: 6520 676f 2062 2f63 206f 6620 7377 6170  e go b/c of swap
-00006a80: 730a 2020 2020 2020 2020 7072 6f76 6964  s.        provid
-00006a90: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
-00006aa0: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
-00006ab0: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
-00006ac0: 2c20 7265 7472 795f 7065 7269 6f64 3d30  , retry_period=0
-00006ad0: 290a 0a20 2020 2020 2020 2070 726f 7669  )..        provi
-00006ae0: 6465 722e 7a6f 6e65 5f72 6563 6f72 6473  der.zone_records
-00006af0: 203d 204d 6f63 6b28 0a20 2020 2020 2020   = Mock(.       
-00006b00: 2020 2020 2072 6574 7572 6e5f 7661 6c75       return_valu
-00006b10: 653d 5b0a 2020 2020 2020 2020 2020 2020  e=[.            
-00006b20: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
-00006b30: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
-00006b40: 2266 6331 3261 6233 3463 6435 3631 3133  "fc12ab34cd56113
-00006b50: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
-00006b60: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-00006b70: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
-00006b80: 224e 5322 2c0a 2020 2020 2020 2020 2020  "NS",.          
-00006b90: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-00006ba0: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bc0: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-00006bd0: 6e73 312e 666f 6f2e 6261 7222 2c0a 2020  ns1.foo.bar",.  
-00006be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006bf0: 2020 2270 726f 7869 6162 6c65 223a 2054    "proxiable": T
-00006c00: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-00006c10: 2020 2020 2020 2020 2022 7072 6f78 6965           "proxie
-00006c20: 6422 3a20 4661 6c73 652c 0a20 2020 2020  d": False,.     
-00006c30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006c40: 7474 6c22 3a20 3330 302c 0a20 2020 2020  ttl": 300,.     
-00006c50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006c60: 6c6f 636b 6564 223a 2046 616c 7365 2c0a  locked": False,.
-00006c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c80: 2020 2020 227a 6f6e 655f 6964 223a 2022      "zone_id": "
-00006c90: 6666 3132 6162 3334 6364 3536 3131 3333  ff12ab34cd561133
-00006ca0: 3434 3232 6162 3333 3232 3939 3736 3530  4422ab3322997650
-00006cb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00006cc0: 2020 2020 2020 2022 7a6f 6e65 5f6e 616d         "zone_nam
-00006cd0: 6522 3a20 2275 6e69 742e 7465 7374 7322  e": "unit.tests"
-00006ce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006cf0: 2020 2020 2020 226d 6f64 6966 6965 645f        "modified_
-00006d00: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
-00006d10: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
-00006d20: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-00006d30: 2020 2020 2020 2020 2263 7265 6174 6564          "created
-00006d40: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
-00006d50: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
-00006d60: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
-00006d70: 2020 2020 2020 2020 2022 6d65 7461 223a           "meta":
-00006d80: 207b 2261 7574 6f5f 6164 6465 6422 3a20   {"auto_added": 
-00006d90: 4661 6c73 657d 2c0a 2020 2020 2020 2020  False},.        
-00006da0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00006db0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dd0: 2022 6964 223a 2022 6663 3132 6162 3334   "id": "fc12ab34
-00006de0: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
-00006df0: 3232 3939 3736 3534 222c 0a20 2020 2020  22997654",.     
-00006e00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006e10: 7479 7065 223a 2022 4e53 222c 0a20 2020  type": "NS",.   
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2022 6e61 6d65 223a 2022 756e 6974 2e74   "name": "unit.t
-00006e40: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
-00006e50: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
-00006e60: 656e 7422 3a20 226e 7332 2e66 6f6f 2e62  ent": "ns2.foo.b
-00006e70: 6172 222c 0a20 2020 2020 2020 2020 2020  ar",.           
-00006e80: 2020 2020 2020 2020 2022 7072 6f78 6961           "proxia
-00006e90: 626c 6522 3a20 5472 7565 2c0a 2020 2020  ble": True,.    
-00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006eb0: 2270 726f 7869 6564 223a 2046 616c 7365  "proxied": False
-00006ec0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006ed0: 2020 2020 2020 2274 746c 223a 2033 3030        "ttl": 300
-00006ee0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00006ef0: 2020 2020 2020 226c 6f63 6b65 6422 3a20        "locked": 
-00006f00: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00006f10: 2020 2020 2020 2020 2020 2022 7a6f 6e65             "zone
-00006f20: 5f69 6422 3a20 2266 6631 3261 6233 3463  _id": "ff12ab34c
-00006f30: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
-00006f40: 3239 3937 3635 3022 2c0a 2020 2020 2020  2997650",.      
-00006f50: 2020 2020 2020 2020 2020 2020 2020 227a                "z
-00006f60: 6f6e 655f 6e61 6d65 223a 2022 756e 6974  one_name": "unit
-00006f70: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
-00006f80: 2020 2020 2020 2020 2020 2020 2022 6d6f               "mo
-00006f90: 6469 6669 6564 5f6f 6e22 3a20 2232 3031  dified_on": "201
-00006fa0: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
-00006fb0: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
-00006fc0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00006fd0: 6372 6561 7465 645f 6f6e 223a 2022 3230  created_on": "20
-00006fe0: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
-00006ff0: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
-00007000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007010: 226d 6574 6122 3a20 7b22 6175 746f 5f61  "meta": {"auto_a
-00007020: 6464 6564 223a 2046 616c 7365 7d2c 0a20  dded": False},. 
-00007030: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007040: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007050: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-00007060: 2020 2020 2020 2020 2269 6422 3a20 2232          "id": "2
-00007070: 6139 3134 3062 3137 6666 6230 6536 6165  a9140b17ffb0e6ae
-00007080: 6438 3236 3034 3965 6563 3937 3462 3722  d826049eec974b7"
-00007090: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000070a0: 2020 2020 2020 2274 6172 6765 7473 223a        "targets":
-000070b0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000070c0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070e0: 2020 2020 2020 2020 2022 7461 7267 6574           "target
-000070f0: 223a 2022 7572 6c22 2c0a 2020 2020 2020  ": "url",.      
-00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007110: 2020 2020 2020 2263 6f6e 7374 7261 696e        "constrain
-00007120: 7422 3a20 7b0a 2020 2020 2020 2020 2020  t": {.          
-00007130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007140: 2020 2020 2020 226f 7065 7261 746f 7222        "operator"
-00007150: 3a20 226d 6174 6368 6573 222c 0a20 2020  : "matches",.   
-00007160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007170: 2020 2020 2020 2020 2020 2020 2022 7661               "va
-00007180: 6c75 6522 3a20 2275 726c 6677 6431 2e75  lue": "urlfwd1.u
-00007190: 6e69 742e 7465 7374 732f 222c 0a20 2020  nit.tests/",.   
-000071a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071b0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-000071e0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-000071f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007200: 2022 6163 7469 6f6e 7322 3a20 5b0a 2020   "actions": [.  
-00007210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007220: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00007230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007240: 2020 2020 2269 6422 3a20 2266 6f72 7761      "id": "forwa
-00007250: 7264 696e 675f 7572 6c22 2c0a 2020 2020  rding_url",.    
-00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007270: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-00007280: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00006970: 2020 2020 2027 7072 6f78 6965 6427 3a20       'proxied': 
+00006980: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00006990: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000069a0: 7474 6c27 3a20 3330 302c 0a20 2020 2020  ttl': 300,.     
+000069b0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+000069c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000069d0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+000069e0: 2020 2020 2063 616c 6c28 0a20 2020 2020       call(.     
+000069f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006a00: 5055 5427 2c0a 2020 2020 2020 2020 2020  PUT',.          
+00006a10: 2020 2020 2020 2020 2020 272f 7a6f 6e65            '/zone
+00006a20: 732f 3432 2f64 6e73 5f72 6563 6f72 6473  s/42/dns_records
+00006a30: 2f66 6331 3261 6233 3463 6435 3631 3133  /fc12ab34cd56113
+00006a40: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
+00006a50: 3327 2c0a 2020 2020 2020 2020 2020 2020  3',.            
+00006a60: 2020 2020 2020 2020 6461 7461 3d7b 0a20          data={. 
+00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a80: 2020 2020 2020 2027 636f 6e74 656e 7427         'content'
+00006a90: 3a20 2733 2e33 2e33 2e33 272c 0a20 2020  : '3.3.3.3',.   
+00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ab0: 2020 2020 2027 7479 7065 273a 2027 4127       'type': 'A'
+00006ac0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006ad0: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+00006ae0: 3a20 2761 2e75 6e69 742e 7465 7374 7327  : 'a.unit.tests'
+00006af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00006b00: 2020 2020 2020 2020 2020 2770 726f 7869            'proxi
+00006b10: 6564 273a 2046 616c 7365 2c0a 2020 2020  ed': False,.    
+00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b30: 2020 2020 2774 746c 273a 2033 3030 2c0a      'ttl': 300,.
+00006b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b50: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+00006b60: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00006b70: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00006b80: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+00006b90: 7570 6461 7465 5f64 656c 6574 6528 7365  update_delete(se
+00006ba0: 6c66 293a 0a20 2020 2020 2020 2023 2057  lf):.        # W
+00006bb0: 6520 6e65 6564 2061 6e6f 7468 6572 2072  e need another r
+00006bc0: 756e 2073 6f20 7468 6174 2077 6520 6361  un so that we ca
+00006bd0: 6e20 6465 6c65 7465 2c20 7765 2063 616e  n delete, we can
+00006be0: 2774 2062 6f74 6820 6164 6420 616e 640a  't both add and.
+00006bf0: 2020 2020 2020 2020 2320 6465 6c65 7465          # delete
+00006c00: 2069 6e20 6f6e 6520 676f 2062 2f63 206f   in one go b/c o
+00006c10: 6620 7377 6170 730a 2020 2020 2020 2020  f swaps.        
+00006c20: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
+00006c30: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
+00006c40: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
+00006c50: 746f 6b65 6e27 2c20 7265 7472 795f 7065  token', retry_pe
+00006c60: 7269 6f64 3d30 290a 0a20 2020 2020 2020  riod=0)..       
+00006c70: 2070 726f 7669 6465 722e 7a6f 6e65 5f72   provider.zone_r
+00006c80: 6563 6f72 6473 203d 204d 6f63 6b28 0a20  ecords = Mock(. 
+00006c90: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006ca0: 6e5f 7661 6c75 653d 5b0a 2020 2020 2020  n_value=[.      
+00006cb0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+00006cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006cd0: 2269 6422 3a20 2266 6331 3261 6233 3463  "id": "fc12ab34c
+00006ce0: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
+00006cf0: 3239 3937 3635 3322 2c0a 2020 2020 2020  2997653",.      
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+00006d10: 7970 6522 3a20 224e 5322 2c0a 2020 2020  ype": "NS",.    
+00006d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d30: 226e 616d 6522 3a20 2275 6e69 742e 7465  "name": "unit.te
+00006d40: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+00006d50: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00006d60: 6e74 223a 2022 6e73 312e 666f 6f2e 6261  nt": "ns1.foo.ba
+00006d70: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
+00006d80: 2020 2020 2020 2020 2270 726f 7869 6162          "proxiab
+00006d90: 6c65 223a 2054 7275 652c 0a20 2020 2020  le": True,.     
+00006da0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006db0: 7072 6f78 6965 6422 3a20 4661 6c73 652c  proxied": False,
+00006dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006dd0: 2020 2020 2022 7474 6c22 3a20 3330 302c       "ttl": 300,
+00006de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006df0: 2020 2020 2022 6c6f 636b 6564 223a 2046       "locked": F
+00006e00: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00006e10: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
+00006e20: 6964 223a 2022 6666 3132 6162 3334 6364  id": "ff12ab34cd
+00006e30: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
+00006e40: 3939 3736 3530 222c 0a20 2020 2020 2020  997650",.       
+00006e50: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+00006e60: 6e65 5f6e 616d 6522 3a20 2275 6e69 742e  ne_name": "unit.
+00006e70: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
+00006e80: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
+00006e90: 6966 6965 645f 6f6e 223a 2022 3230 3137  ified_on": "2017
+00006ea0: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+00006eb0: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+00006ec0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00006ed0: 7265 6174 6564 5f6f 6e22 3a20 2232 3031  reated_on": "201
+00006ee0: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
+00006ef0: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
+00006f00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00006f10: 6d65 7461 223a 207b 2261 7574 6f5f 6164  meta": {"auto_ad
+00006f20: 6465 6422 3a20 4661 6c73 657d 2c0a 2020  ded": False},.  
+00006f30: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00006f40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006f50: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00006f60: 2020 2020 2020 2022 6964 223a 2022 6663         "id": "fc
+00006f70: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
+00006f80: 3232 6162 3333 3232 3939 3736 3534 222c  22ab3322997654",
+00006f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006fa0: 2020 2020 2022 7479 7065 223a 2022 4e53       "type": "NS
+00006fb0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00006fc0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00006fd0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ff0: 2022 636f 6e74 656e 7422 3a20 226e 7332   "content": "ns2
+00007000: 2e66 6f6f 2e62 6172 222c 0a20 2020 2020  .foo.bar",.     
+00007010: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007020: 7072 6f78 6961 626c 6522 3a20 5472 7565  proxiable": True
+00007030: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007040: 2020 2020 2020 2270 726f 7869 6564 223a        "proxied":
+00007050: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00007060: 2020 2020 2020 2020 2020 2020 2274 746c              "ttl
+00007070: 223a 2033 3030 2c0a 2020 2020 2020 2020  ": 300,.        
+00007080: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
+00007090: 6b65 6422 3a20 4661 6c73 652c 0a20 2020  ked": False,.   
+000070a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070b0: 2022 7a6f 6e65 5f69 6422 3a20 2266 6631   "zone_id": "ff1
+000070c0: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
+000070d0: 3261 6233 3332 3239 3937 3635 3022 2c0a  2ab3322997650",.
+000070e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070f0: 2020 2020 227a 6f6e 655f 6e61 6d65 223a      "zone_name":
+00007100: 2022 756e 6974 2e74 6573 7473 222c 0a20   "unit.tests",. 
+00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007120: 2020 2022 6d6f 6469 6669 6564 5f6f 6e22     "modified_on"
+00007130: 3a20 2232 3031 372d 3033 2d31 3154 3138  : "2017-03-11T18
+00007140: 3a30 313a 3433 2e34 3230 3638 395a 222c  :01:43.420689Z",
+00007150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007160: 2020 2020 2022 6372 6561 7465 645f 6f6e       "created_on
+00007170: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
+00007180: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
+00007190: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000071a0: 2020 2020 2020 226d 6574 6122 3a20 7b22        "meta": {"
+000071b0: 6175 746f 5f61 6464 6564 223a 2046 616c  auto_added": Fal
+000071c0: 7365 7d2c 0a20 2020 2020 2020 2020 2020  se},.           
+000071d0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+000071e0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000071f0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+00007200: 6422 3a20 2232 6139 3134 3062 3137 6666  d": "2a9140b17ff
+00007210: 6230 6536 6165 6438 3236 3034 3965 6563  b0e6aed826049eec
+00007220: 3937 3462 3722 2c0a 2020 2020 2020 2020  974b7",.        
+00007230: 2020 2020 2020 2020 2020 2020 2274 6172              "tar
+00007240: 6765 7473 223a 205b 0a20 2020 2020 2020  gets": [.       
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00007270: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00007280: 7461 7267 6574 223a 2022 7572 6c22 2c0a  target": "url",.
 00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2022 7572 6c22 3a20 2268 7474 7073     "url": "https
-000072b0: 3a2f 2f77 7777 2e75 6e69 742e 7465 7374  ://www.unit.test
-000072c0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 2020 2020 2273 7461 7475 735f 636f 6465      "status_code
-000072f0: 223a 2033 3032 2c0a 2020 2020 2020 2020  ": 302,.        
+000072a0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+000072b0: 7374 7261 696e 7422 3a20 7b0a 2020 2020  straint": {.    
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 2020 2020 2020 2020 2020 2020 226f 7065              "ope
+000072e0: 7261 746f 7222 3a20 226d 6174 6368 6573  rator": "matches
+000072f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
 00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00007320: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007340: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00007350: 2020 2020 2020 2020 2020 2020 2270 7269              "pri
-00007360: 6f72 6974 7922 3a20 312c 0a20 2020 2020  ority": 1,.     
-00007370: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007380: 7374 6174 7573 223a 2022 6163 7469 7665  status": "active
-00007390: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000073a0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-000073b0: 6f6e 223a 2022 3230 3231 2d30 362d 3235  on": "2021-06-25
-000073c0: 5432 303a 3130 3a35 302e 3030 3030 3030  T20:10:50.000000
-000073d0: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-000073e0: 2020 2020 2020 2020 226d 6f64 6966 6965          "modifie
-000073f0: 645f 6f6e 223a 2022 3230 3231 2d30 362d  d_on": "2021-06-
-00007400: 3238 5432 323a 3338 3a31 302e 3030 3030  28T22:38:10.0000
-00007410: 3030 5a22 2c0a 2020 2020 2020 2020 2020  00Z",.          
-00007420: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00007430: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00007440: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007450: 6964 223a 2022 3261 3931 3431 6231 3866  id": "2a9141b18f
-00007460: 6662 3065 3661 6564 3832 3630 3534 6565  fb0e6aed826054ee
-00007470: 6339 3730 6238 222c 0a20 2020 2020 2020  c970b8",.       
-00007480: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
-00007490: 7267 6574 7322 3a20 5b0a 2020 2020 2020  rgets": [.      
-000074a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074b0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074d0: 2274 6172 6765 7422 3a20 2275 726c 222c  "target": "url",
-000074e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000074f0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00007500: 6e73 7472 6169 6e74 223a 207b 0a20 2020  nstraint": {.   
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 2020 2020 2020 2020 2022 6f70               "op
-00007530: 6572 6174 6f72 223a 2022 6d61 7463 6865  erator": "matche
-00007540: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00007550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007560: 2020 2020 2276 616c 7565 223a 2022 7572      "value": "ur
-00007570: 6c66 7764 312e 756e 6974 2e74 6573 7473  lfwd1.unit.tests
-00007580: 2f74 6172 6765 7422 2c0a 2020 2020 2020  /target",.      
-00007590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075a0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-000075b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075c0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-000075d0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-000075e0: 2020 2020 2020 2020 2020 2020 2020 2261                "a
-000075f0: 6374 696f 6e73 223a 205b 0a20 2020 2020  ctions": [.     
-00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00007620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007630: 2022 6964 223a 2022 666f 7277 6172 6469   "id": "forwardi
-00007640: 6e67 5f75 726c 222c 0a20 2020 2020 2020  ng_url",.       
+00007310: 2020 2022 7661 6c75 6522 3a20 2275 726c     "value": "url
+00007320: 6677 6431 2e75 6e69 742e 7465 7374 732f  fwd1.unit.tests/
+00007330: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00007340: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00007350: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007360: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007380: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00007390: 2020 2020 2020 2022 6163 7469 6f6e 7322         "actions"
+000073a0: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+000073b0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+000073e0: 2266 6f72 7761 7264 696e 675f 7572 6c22  "forwarding_url"
+000073f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007400: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00007410: 616c 7565 223a 207b 0a20 2020 2020 2020  alue": {.       
+00007420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007430: 2020 2020 2020 2020 2022 7572 6c22 3a20           "url": 
+00007440: 2268 7474 7073 3a2f 2f77 7777 2e75 6e69  "https://www.uni
+00007450: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+00007460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007470: 2020 2020 2020 2020 2020 2273 7461 7475            "statu
+00007480: 735f 636f 6465 223a 2033 3032 2c0a 2020  s_code": 302,.  
+00007490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074a0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000074b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074c0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+000074d0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+000074e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074f0: 2020 2270 7269 6f72 6974 7922 3a20 312c    "priority": 1,
+00007500: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007510: 2020 2020 2022 7374 6174 7573 223a 2022       "status": "
+00007520: 6163 7469 7665 222c 0a20 2020 2020 2020  active",.       
+00007530: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+00007540: 6561 7465 645f 6f6e 223a 2022 3230 3231  eated_on": "2021
+00007550: 2d30 362d 3235 5432 303a 3130 3a35 302e  -06-25T20:10:50.
+00007560: 3030 3030 3030 5a22 2c0a 2020 2020 2020  000000Z",.      
+00007570: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00007580: 6f64 6966 6965 645f 6f6e 223a 2022 3230  odified_on": "20
+00007590: 3231 2d30 362d 3238 5432 323a 3338 3a31  21-06-28T22:38:1
+000075a0: 302e 3030 3030 3030 5a22 2c0a 2020 2020  0.000000Z",.    
+000075b0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000075c0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000075d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000075e0: 2020 2020 2022 6964 223a 2022 3261 3931       "id": "2a91
+000075f0: 3431 6231 3866 6662 3065 3661 6564 3832  41b18ffb0e6aed82
+00007600: 3630 3534 6565 6339 3730 6238 222c 0a20  6054eec970b8",. 
+00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007620: 2020 2022 7461 7267 6574 7322 3a20 5b0a     "targets": [.
+00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007640: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
 00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007660: 2020 2020 2022 7661 6c75 6522 3a20 7b0a       "value": {.
-00007670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 2020 2020 2274 6172 6765 7422 3a20        "target": 
+00007670: 2275 726c 222c 0a20 2020 2020 2020 2020  "url",.         
 00007680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007690: 2275 726c 223a 2022 6874 7470 733a 2f2f  "url": "https://
-000076a0: 7461 7267 6574 2e75 6e69 742e 7465 7374  target.unit.test
-000076b0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2273 7461 7475 735f 636f 6465      "status_code
-000076e0: 223a 2033 3031 2c0a 2020 2020 2020 2020  ": 301,.        
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-00007710: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00007720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007730: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00007740: 2020 2020 2020 2020 2020 2020 2270 7269              "pri
-00007750: 6f72 6974 7922 3a20 322c 0a20 2020 2020  ority": 2,.     
-00007760: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00007770: 7374 6174 7573 223a 2022 6163 7469 7665  status": "active
-00007780: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00007790: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-000077a0: 6f6e 223a 2022 3230 3231 2d30 362d 3235  on": "2021-06-25
-000077b0: 5432 303a 3130 3a35 302e 3030 3030 3030  T20:10:50.000000
-000077c0: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-000077d0: 2020 2020 2020 2020 226d 6f64 6966 6965          "modifie
-000077e0: 645f 6f6e 223a 2022 3230 3231 2d30 362d  d_on": "2021-06-
-000077f0: 3238 5432 323a 3338 3a31 302e 3030 3030  28T22:38:10.0000
-00007800: 3030 5a22 2c0a 2020 2020 2020 2020 2020  00Z",.          
-00007810: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00007820: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
-00007830: 0a0a 2020 2020 2020 2020 7072 6f76 6964  ..        provid
-00007840: 6572 2e5f 7265 7175 6573 7420 3d20 4d6f  er._request = Mo
-00007850: 636b 2829 0a20 2020 2020 2020 2070 726f  ck().        pro
-00007860: 7669 6465 722e 5f72 6571 7565 7374 2e73  vider._request.s
-00007870: 6964 655f 6566 6665 6374 203d 205b 0a20  ide_effect = [. 
-00007880: 2020 2020 2020 2020 2020 2043 6c6f 7564             Cloud
-00007890: 666c 6172 6552 6174 654c 696d 6974 4572  flareRateLimitEr
-000078a0: 726f 7228 277b 7d27 292c 0a20 2020 2020  ror('{}'),.     
-000078b0: 2020 2020 2020 2073 656c 662e 656d 7074         self.empt
-000078c0: 792c 2020 2320 6e6f 207a 6f6e 6573 0a20  y,  # no zones. 
-000078d0: 2020 2020 2020 2020 2020 207b 2772 6573             {'res
-000078e0: 756c 7427 3a20 7b27 6964 273a 2034 327d  ult': {'id': 42}
-000078f0: 7d2c 2020 2320 7a6f 6e65 2063 7265 6174  },  # zone creat
-00007900: 650a 2020 2020 2020 2020 2020 2020 4e6f  e.            No
-00007910: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00007920: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-00007930: 2020 4e6f 6e65 2c0a 2020 2020 2020 2020    None,.        
-00007940: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
-00007950: 2020 5d0a 0a20 2020 2020 2020 2023 2041    ]..        # A
-00007960: 6464 2073 6f6d 6574 6869 6e67 2061 6e64  dd something and
-00007970: 2064 656c 6574 6520 736f 6d65 7468 696e   delete somethin
-00007980: 670a 2020 2020 2020 2020 7a6f 6e65 203d  g.        zone =
-00007990: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
-000079a0: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
-000079b0: 2065 7869 7374 696e 6720 3d20 5265 636f   existing = Reco
-000079c0: 7264 2e6e 6577 280a 2020 2020 2020 2020  rd.new(.        
-000079d0: 2020 2020 7a6f 6e65 2c0a 2020 2020 2020      zone,.      
-000079e0: 2020 2020 2020 2727 2c0a 2020 2020 2020        '',.      
-000079f0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00007a00: 2020 2020 2020 2020 2774 746c 273a 2033          'ttl': 3
-00007a10: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-00007a20: 2020 2020 2774 7970 6527 3a20 274e 5327      'type': 'NS'
-00007a30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007a40: 2020 2320 5468 6973 206d 6174 6368 6573    # This matches
-00007a50: 2074 6865 207a 6f6e 6520 6461 7461 2061   the zone data a
-00007a60: 626f 7665 2c20 6f6e 6520 746f 2064 656c  bove, one to del
-00007a70: 6574 652c 206f 6e65 2074 6f20 6c65 6176  ete, one to leav
-00007a80: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00007a90: 2020 2776 616c 7565 7327 3a20 5b27 6e73    'values': ['ns
-00007aa0: 312e 666f 6f2e 6261 722e 272c 2027 6e73  1.foo.bar.', 'ns
-00007ab0: 322e 666f 6f2e 6261 722e 275d 2c0a 2020  2.foo.bar.'],.  
-00007ac0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007ad0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-00007ae0: 7873 7469 6e67 7572 6c66 7764 203d 2052  xstingurlfwd = R
-00007af0: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
-00007b00: 2020 2020 2020 207a 6f6e 652c 0a20 2020         zone,.   
-00007b10: 2020 2020 2020 2020 2027 7572 6c66 7764           'urlfwd
-00007b20: 3127 2c0a 2020 2020 2020 2020 2020 2020  1',.            
-00007b30: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00007b40: 2020 2774 746c 273a 2033 3030 2c0a 2020    'ttl': 300,.  
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00007b60: 7970 6527 3a20 2755 524c 4657 4427 2c0a  ype': 'URLFWD',.
-00007b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b80: 2776 616c 7565 7327 3a20 5b0a 2020 2020  'values': [.    
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00007bb0: 2020 2020 2020 2020 2020 2770 6174 6827            'path'
-00007bc0: 3a20 272f 272c 0a20 2020 2020 2020 2020  : '/',.         
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00007be0: 7461 7267 6574 273a 2027 6874 7470 733a  target': 'https:
-00007bf0: 2f2f 7777 772e 756e 6974 2e74 6573 7473  //www.unit.tests
-00007c00: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00007c10: 2020 2020 2020 2020 2020 2027 636f 6465             'code
-00007c20: 273a 2033 3032 2c0a 2020 2020 2020 2020  ': 302,.        
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c40: 276d 6173 6b69 6e67 273a 2027 3227 2c0a  'masking': '2',.
-00007c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c60: 2020 2020 2020 2020 2771 7565 7279 273a          'query':
-00007c70: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
-00007c80: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00007c90: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00007ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007cb0: 2020 2020 2020 2020 2027 7061 7468 273a           'path':
-00007cc0: 2027 2f74 6172 6765 7427 2c0a 2020 2020   '/target',.    
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ce0: 2020 2020 2774 6172 6765 7427 3a20 2768      'target': 'h
-00007cf0: 7474 7073 3a2f 2f74 6172 6765 742e 756e  ttps://target.un
-00007d00: 6974 2e74 6573 7473 272c 0a20 2020 2020  it.tests',.     
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2027 636f 6465 273a 2033 3031 2c0a     'code': 301,.
-00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d40: 2020 2020 2020 2020 276d 6173 6b69 6e67          'masking
-00007d50: 273a 2027 3227 2c0a 2020 2020 2020 2020  ': '2',.        
+00007690: 2020 2022 636f 6e73 7472 6169 6e74 223a     "constraint":
+000076a0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+000076b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076c0: 2020 2022 6f70 6572 6174 6f72 223a 2022     "operator": "
+000076d0: 6d61 7463 6865 7322 2c0a 2020 2020 2020  matches",.      
+000076e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000076f0: 2020 2020 2020 2020 2020 2276 616c 7565            "value
+00007700: 223a 2022 7572 6c66 7764 312e 756e 6974  ": "urlfwd1.unit
+00007710: 2e74 6573 7473 2f74 6172 6765 7422 2c0a  .tests/target",.
+00007720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007730: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+00007740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007750: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00007760: 2020 2020 2020 2020 2020 2020 205d 2c0a               ],.
+00007770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007780: 2020 2020 2261 6374 696f 6e73 223a 205b      "actions": [
+00007790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000077a0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077c0: 2020 2020 2020 2022 6964 223a 2022 666f         "id": "fo
+000077d0: 7277 6172 6469 6e67 5f75 726c 222c 0a20  rwarding_url",. 
+000077e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077f0: 2020 2020 2020 2020 2020 2022 7661 6c75             "valu
+00007800: 6522 3a20 7b0a 2020 2020 2020 2020 2020  e": {.          
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2020 2020 2275 726c 223a 2022 6874        "url": "ht
+00007830: 7470 733a 2f2f 7461 7267 6574 2e75 6e69  tps://target.uni
+00007840: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+00007850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007860: 2020 2020 2020 2020 2020 2273 7461 7475            "statu
+00007870: 735f 636f 6465 223a 2033 3031 2c0a 2020  s_code": 301,.  
+00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007890: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000078a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078b0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+000078c0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078e0: 2020 2270 7269 6f72 6974 7922 3a20 322c    "priority": 2,
+000078f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007900: 2020 2020 2022 7374 6174 7573 223a 2022       "status": "
+00007910: 6163 7469 7665 222c 0a20 2020 2020 2020  active",.       
+00007920: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+00007930: 6561 7465 645f 6f6e 223a 2022 3230 3231  eated_on": "2021
+00007940: 2d30 362d 3235 5432 303a 3130 3a35 302e  -06-25T20:10:50.
+00007950: 3030 3030 3030 5a22 2c0a 2020 2020 2020  000000Z",.      
+00007960: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00007970: 6f64 6966 6965 645f 6f6e 223a 2022 3230  odified_on": "20
+00007980: 3231 2d30 362d 3238 5432 323a 3338 3a31  21-06-28T22:38:1
+00007990: 302e 3030 3030 3030 5a22 2c0a 2020 2020  0.000000Z",.    
+000079a0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000079b0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+000079c0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+000079d0: 7072 6f76 6964 6572 2e5f 7265 7175 6573  provider._reques
+000079e0: 7420 3d20 4d6f 636b 2829 0a20 2020 2020  t = Mock().     
+000079f0: 2020 2070 726f 7669 6465 722e 5f72 6571     provider._req
+00007a00: 7565 7374 2e73 6964 655f 6566 6665 6374  uest.side_effect
+00007a10: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00007a20: 2043 6c6f 7564 666c 6172 6552 6174 654c   CloudflareRateL
+00007a30: 696d 6974 4572 726f 7228 277b 7d27 292c  imitError('{}'),
+00007a40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00007a50: 662e 656d 7074 792c 2020 2320 6e6f 207a  f.empty,  # no z
+00007a60: 6f6e 6573 0a20 2020 2020 2020 2020 2020  ones.           
+00007a70: 207b 2772 6573 756c 7427 3a20 7b27 6964   {'result': {'id
+00007a80: 273a 2034 327d 7d2c 2020 2320 7a6f 6e65  ': 42}},  # zone
+00007a90: 2063 7265 6174 650a 2020 2020 2020 2020   create.        
+00007aa0: 2020 2020 4e6f 6e65 2c0a 2020 2020 2020      None,.      
+00007ab0: 2020 2020 2020 4e6f 6e65 2c0a 2020 2020        None,.    
+00007ac0: 2020 2020 2020 2020 4e6f 6e65 2c0a 2020          None,.  
+00007ad0: 2020 2020 2020 2020 2020 4e6f 6e65 2c0a            None,.
+00007ae0: 2020 2020 2020 2020 5d0a 0a20 2020 2020          ]..     
+00007af0: 2020 2023 2041 6464 2073 6f6d 6574 6869     # Add somethi
+00007b00: 6e67 2061 6e64 2064 656c 6574 6520 736f  ng and delete so
+00007b10: 6d65 7468 696e 670a 2020 2020 2020 2020  mething.        
+00007b20: 7a6f 6e65 203d 205a 6f6e 6528 2775 6e69  zone = Zone('uni
+00007b30: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
+00007b40: 2020 2020 2020 2065 7869 7374 696e 6720         existing 
+00007b50: 3d20 5265 636f 7264 2e6e 6577 280a 2020  = Record.new(.  
+00007b60: 2020 2020 2020 2020 2020 7a6f 6e65 2c0a            zone,.
+00007b70: 2020 2020 2020 2020 2020 2020 2727 2c0a              '',.
+00007b80: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00007b90: 2020 2020 2020 2020 2020 2020 2020 2774                't
+00007ba0: 746c 273a 2033 3030 2c0a 2020 2020 2020  tl': 300,.      
+00007bb0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+00007bc0: 3a20 274e 5327 2c0a 2020 2020 2020 2020  : 'NS',.        
+00007bd0: 2020 2020 2020 2020 2320 5468 6973 206d          # This m
+00007be0: 6174 6368 6573 2074 6865 207a 6f6e 6520  atches the zone 
+00007bf0: 6461 7461 2061 626f 7665 2c20 6f6e 6520  data above, one 
+00007c00: 746f 2064 656c 6574 652c 206f 6e65 2074  to delete, one t
+00007c10: 6f20 6c65 6176 650a 2020 2020 2020 2020  o leave.        
+00007c20: 2020 2020 2020 2020 2776 616c 7565 7327          'values'
+00007c30: 3a20 5b27 6e73 312e 666f 6f2e 6261 722e  : ['ns1.foo.bar.
+00007c40: 272c 2027 6e73 322e 666f 6f2e 6261 722e  ', 'ns2.foo.bar.
+00007c50: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00007c60: 7d2c 0a20 2020 2020 2020 2029 0a20 2020  },.        ).   
+00007c70: 2020 2020 2065 7873 7469 6e67 7572 6c66       exstingurlf
+00007c80: 7764 203d 2052 6563 6f72 642e 6e65 7728  wd = Record.new(
+00007c90: 0a20 2020 2020 2020 2020 2020 207a 6f6e  .            zon
+00007ca0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+00007cb0: 7572 6c66 7764 3127 2c0a 2020 2020 2020  urlfwd1',.      
+00007cc0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00007cd0: 2020 2020 2020 2020 2774 746c 273a 2033          'ttl': 3
+00007ce0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+00007cf0: 2020 2020 2774 7970 6527 3a20 2755 524c      'type': 'URL
+00007d00: 4657 4427 2c0a 2020 2020 2020 2020 2020  FWD',.          
+00007d10: 2020 2020 2020 2776 616c 7565 7327 3a20        'values': 
+00007d20: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00007d30: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d50: 2770 6174 6827 3a20 272f 272c 0a20 2020  'path': '/',.   
 00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d70: 2771 7565 7279 273a 2030 2c0a 2020 2020  'query': 0,.    
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d90: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00007da0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-00007db0: 2020 7d2c 0a20 2020 2020 2020 2029 0a20    },.        ). 
-00007dc0: 2020 2020 2020 206e 6577 203d 2052 6563         new = Rec
-00007dd0: 6f72 642e 6e65 7728 0a20 2020 2020 2020  ord.new(.       
-00007de0: 2020 2020 207a 6f6e 652c 0a20 2020 2020       zone,.     
-00007df0: 2020 2020 2020 2027 272c 0a20 2020 2020         '',.     
-00007e00: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-00007e10: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
-00007e20: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
-00007e30: 2020 2020 2027 7479 7065 273a 2027 4e53       'type': 'NS
-00007e40: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00007e50: 2020 2023 2054 6869 7320 6c65 6176 6573     # This leaves
-00007e60: 206f 6e65 2061 6e64 2064 656c 6574 6573   one and deletes
-00007e70: 206f 6e65 0a20 2020 2020 2020 2020 2020   one.           
-00007e80: 2020 2020 2027 7661 6c75 6527 3a20 276e       'value': 'n
-00007e90: 7332 2e66 6f6f 2e62 6172 2e27 2c0a 2020  s2.foo.bar.',.  
-00007ea0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00007eb0: 2020 2020 2029 0a20 2020 2020 2020 206e       ).        n
-00007ec0: 6577 7572 6c66 7764 203d 2052 6563 6f72  ewurlfwd = Recor
-00007ed0: 642e 6e65 7728 0a20 2020 2020 2020 2020  d.new(.         
-00007ee0: 2020 207a 6f6e 652c 0a20 2020 2020 2020     zone,.       
-00007ef0: 2020 2020 2027 7572 6c66 7764 3127 2c0a       'urlfwd1',.
-00007f00: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-00007f10: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00007f20: 746c 273a 2033 3030 2c0a 2020 2020 2020  tl': 300,.      
-00007f30: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
-00007f40: 3a20 2755 524c 4657 4427 2c0a 2020 2020  : 'URLFWD',.    
-00007f50: 2020 2020 2020 2020 2020 2020 2776 616c              'val
-00007f60: 7565 273a 207b 0a20 2020 2020 2020 2020  ue': {.         
-00007f70: 2020 2020 2020 2020 2020 2027 7061 7468             'path
-00007f80: 273a 2027 2f27 2c0a 2020 2020 2020 2020  ': '/',.        
-00007f90: 2020 2020 2020 2020 2020 2020 2774 6172              'tar
-00007fa0: 6765 7427 3a20 2768 7474 7073 3a2f 2f77  get': 'https://w
-00007fb0: 7777 2e75 6e69 742e 7465 7374 7327 2c0a  ww.unit.tests',.
-00007fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fd0: 2020 2020 2763 6f64 6527 3a20 3330 322c      'code': 302,
-00007fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007ff0: 2020 2020 2027 6d61 736b 696e 6727 3a20       'masking': 
-00008000: 2732 272c 0a20 2020 2020 2020 2020 2020  '2',.           
-00008010: 2020 2020 2020 2020 2027 7175 6572 7927           'query'
-00008020: 3a20 302c 0a20 2020 2020 2020 2020 2020  : 0,.           
-00008030: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-00008040: 2020 2020 7d2c 0a20 2020 2020 2020 2029      },.        )
-00008050: 0a20 2020 2020 2020 2063 6861 6e67 6520  .        change 
-00008060: 3d20 5570 6461 7465 2865 7869 7374 696e  = Update(existin
-00008070: 672c 206e 6577 290a 2020 2020 2020 2020  g, new).        
-00008080: 6368 616e 6765 7572 6c66 7764 203d 2055  changeurlfwd = U
-00008090: 7064 6174 6528 6578 7374 696e 6775 726c  pdate(exstingurl
-000080a0: 6677 642c 206e 6577 7572 6c66 7764 290a  fwd, newurlfwd).
-000080b0: 2020 2020 2020 2020 706c 616e 203d 2050          plan = P
-000080c0: 6c61 6e28 7a6f 6e65 2c20 7a6f 6e65 2c20  lan(zone, zone, 
-000080d0: 5b63 6861 6e67 652c 2063 6861 6e67 6575  [change, changeu
-000080e0: 726c 6677 645d 2c20 5472 7565 290a 2020  rlfwd], True).  
-000080f0: 2020 2020 2020 7072 6f76 6964 6572 2e5f        provider._
-00008100: 6170 706c 7928 706c 616e 290a 0a20 2020  apply(plan)..   
-00008110: 2020 2020 2023 2047 6574 207a 6f6e 6573       # Get zones
-00008120: 2c20 6372 6561 7465 207a 6f6e 652c 2063  , create zone, c
-00008130: 7265 6174 6520 6120 7265 636f 7264 2c20  reate a record, 
-00008140: 6465 6c65 7465 2061 2072 6563 6f72 640a  delete a record.
-00008150: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
-00008160: 2e5f 7265 7175 6573 742e 6173 7365 7274  ._request.assert
-00008170: 5f68 6173 5f63 616c 6c73 280a 2020 2020  _has_calls(.    
-00008180: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-00008190: 2020 2020 2020 2020 2020 6361 6c6c 2827            call('
-000081a0: 4745 5427 2c20 272f 7a6f 6e65 7327 2c20  GET', '/zones', 
-000081b0: 7061 7261 6d73 3d7b 2770 6167 6527 3a20  params={'page': 
-000081c0: 312c 2027 7065 725f 7061 6765 273a 2035  1, 'per_page': 5
-000081d0: 307d 292c 0a20 2020 2020 2020 2020 2020  0}),.           
-000081e0: 2020 2020 2063 616c 6c28 0a20 2020 2020       call(.     
-000081f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00008200: 504f 5354 272c 0a20 2020 2020 2020 2020  POST',.         
-00008210: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
-00008220: 6573 272c 0a20 2020 2020 2020 2020 2020  es',.           
-00008230: 2020 2020 2020 2020 2064 6174 613d 7b27           data={'
-00008240: 6a75 6d70 5f73 7461 7274 273a 2046 616c  jump_start': Fal
-00008250: 7365 2c20 276e 616d 6527 3a20 2775 6e69  se, 'name': 'uni
-00008260: 742e 7465 7374 7327 7d2c 0a20 2020 2020  t.tests'},.     
-00008270: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00008280: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00008290: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-000082a0: 2020 2020 2020 2020 2750 5554 272c 0a20          'PUT',. 
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 2020 2027 2f7a 6f6e 6573 2f34 322f 646e     '/zones/42/dn
-000082d0: 735f 7265 636f 7264 732f 6663 3132 6162  s_records/fc12ab
-000082e0: 3334 6364 3536 3131 3333 3434 3232 6162  34cd5611334422ab
-000082f0: 3333 3232 3939 3736 3534 272c 0a20 2020  3322997654',.   
-00008300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008310: 2064 6174 613d 7b0a 2020 2020 2020 2020   data={.        
+00007d70: 2020 2020 2027 7461 7267 6574 273a 2027       'target': '
+00007d80: 6874 7470 733a 2f2f 7777 772e 756e 6974  https://www.unit
+00007d90: 2e74 6573 7473 272c 0a20 2020 2020 2020  .tests',.       
+00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007db0: 2027 636f 6465 273a 2033 3032 2c0a 2020   'code': 302,.  
+00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007dd0: 2020 2020 2020 276d 6173 6b69 6e67 273a        'masking':
+00007de0: 2027 3227 2c0a 2020 2020 2020 2020 2020   '2',.          
+00007df0: 2020 2020 2020 2020 2020 2020 2020 2771                'q
+00007e00: 7565 7279 273a 2030 2c0a 2020 2020 2020  uery': 0,.      
+00007e10: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00007e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007e30: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00007e40: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00007e50: 7061 7468 273a 2027 2f74 6172 6765 7427  path': '/target'
+00007e60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007e70: 2020 2020 2020 2020 2020 2774 6172 6765            'targe
+00007e80: 7427 3a20 2768 7474 7073 3a2f 2f74 6172  t': 'https://tar
+00007e90: 6765 742e 756e 6974 2e74 6573 7473 272c  get.unit.tests',
+00007ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007eb0: 2020 2020 2020 2020 2027 636f 6465 273a           'code':
+00007ec0: 2033 3031 2c0a 2020 2020 2020 2020 2020   301,.          
+00007ed0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+00007ee0: 6173 6b69 6e67 273a 2027 3227 2c0a 2020  asking': '2',.  
+00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f00: 2020 2020 2020 2771 7565 7279 273a 2030        'query': 0
+00007f10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007f20: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00007f30: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00007f40: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00007f50: 2020 2029 0a20 2020 2020 2020 206e 6577     ).        new
+00007f60: 203d 2052 6563 6f72 642e 6e65 7728 0a20   = Record.new(. 
+00007f70: 2020 2020 2020 2020 2020 207a 6f6e 652c             zone,
+00007f80: 0a20 2020 2020 2020 2020 2020 2027 272c  .            '',
+00007f90: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
+00007fa0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00007fb0: 7474 6c27 3a20 3330 302c 0a20 2020 2020  ttl': 300,.     
+00007fc0: 2020 2020 2020 2020 2020 2027 7479 7065             'type
+00007fd0: 273a 2027 4e53 272c 0a20 2020 2020 2020  ': 'NS',.       
+00007fe0: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
+00007ff0: 6c65 6176 6573 206f 6e65 2061 6e64 2064  leaves one and d
+00008000: 656c 6574 6573 206f 6e65 0a20 2020 2020  eletes one.     
+00008010: 2020 2020 2020 2020 2020 2027 7661 6c75             'valu
+00008020: 6527 3a20 276e 7332 2e66 6f6f 2e62 6172  e': 'ns2.foo.bar
+00008030: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
+00008040: 7d2c 0a20 2020 2020 2020 2029 0a20 2020  },.        ).   
+00008050: 2020 2020 206e 6577 7572 6c66 7764 203d       newurlfwd =
+00008060: 2052 6563 6f72 642e 6e65 7728 0a20 2020   Record.new(.   
+00008070: 2020 2020 2020 2020 207a 6f6e 652c 0a20           zone,. 
+00008080: 2020 2020 2020 2020 2020 2027 7572 6c66             'urlf
+00008090: 7764 3127 2c0a 2020 2020 2020 2020 2020  wd1',.          
+000080a0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+000080b0: 2020 2020 2774 746c 273a 2033 3030 2c0a      'ttl': 300,.
+000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080d0: 2774 7970 6527 3a20 2755 524c 4657 4427  'type': 'URLFWD'
+000080e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000080f0: 2020 2776 616c 7565 273a 207b 0a20 2020    'value': {.   
+00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008110: 2027 7061 7468 273a 2027 2f27 2c0a 2020   'path': '/',.  
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 2020 2774 6172 6765 7427 3a20 2768 7474    'target': 'htt
+00008140: 7073 3a2f 2f77 7777 2e75 6e69 742e 7465  ps://www.unit.te
+00008150: 7374 7327 2c0a 2020 2020 2020 2020 2020  sts',.          
+00008160: 2020 2020 2020 2020 2020 2763 6f64 6527            'code'
+00008170: 3a20 3330 322c 0a20 2020 2020 2020 2020  : 302,.         
+00008180: 2020 2020 2020 2020 2020 2027 6d61 736b             'mask
+00008190: 696e 6727 3a20 2732 272c 0a20 2020 2020  ing': '2',.     
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000081b0: 7175 6572 7927 3a20 302c 0a20 2020 2020  query': 0,.     
+000081c0: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+000081d0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+000081e0: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
+000081f0: 6861 6e67 6520 3d20 5570 6461 7465 2865  hange = Update(e
+00008200: 7869 7374 696e 672c 206e 6577 290a 2020  xisting, new).  
+00008210: 2020 2020 2020 6368 616e 6765 7572 6c66        changeurlf
+00008220: 7764 203d 2055 7064 6174 6528 6578 7374  wd = Update(exst
+00008230: 696e 6775 726c 6677 642c 206e 6577 7572  ingurlfwd, newur
+00008240: 6c66 7764 290a 2020 2020 2020 2020 706c  lfwd).        pl
+00008250: 616e 203d 2050 6c61 6e28 7a6f 6e65 2c20  an = Plan(zone, 
+00008260: 7a6f 6e65 2c20 5b63 6861 6e67 652c 2063  zone, [change, c
+00008270: 6861 6e67 6575 726c 6677 645d 2c20 5472  hangeurlfwd], Tr
+00008280: 7565 290a 2020 2020 2020 2020 7072 6f76  ue).        prov
+00008290: 6964 6572 2e5f 6170 706c 7928 706c 616e  ider._apply(plan
+000082a0: 290a 0a20 2020 2020 2020 2023 2047 6574  )..        # Get
+000082b0: 207a 6f6e 6573 2c20 6372 6561 7465 207a   zones, create z
+000082c0: 6f6e 652c 2063 7265 6174 6520 6120 7265  one, create a re
+000082d0: 636f 7264 2c20 6465 6c65 7465 2061 2072  cord, delete a r
+000082e0: 6563 6f72 640a 2020 2020 2020 2020 7072  ecord.        pr
+000082f0: 6f76 6964 6572 2e5f 7265 7175 6573 742e  ovider._request.
+00008300: 6173 7365 7274 5f68 6173 5f63 616c 6c73  assert_has_calls
+00008310: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
 00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008330: 2763 6f6e 7465 6e74 273a 2027 6e73 322e  'content': 'ns2.
-00008340: 666f 6f2e 6261 722e 272c 0a20 2020 2020  foo.bar.',.     
-00008350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008360: 2020 2027 7479 7065 273a 2027 4e53 272c     'type': 'NS',
-00008370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008380: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
-00008390: 2027 756e 6974 2e74 6573 7473 272c 0a20   'unit.tests',. 
+00008330: 6361 6c6c 2827 4745 5427 2c20 272f 7a6f  call('GET', '/zo
+00008340: 6e65 7327 2c20 7061 7261 6d73 3d7b 2770  nes', params={'p
+00008350: 6167 6527 3a20 312c 2027 7065 725f 7061  age': 1, 'per_pa
+00008360: 6765 273a 2035 307d 292c 0a20 2020 2020  ge': 50}),.     
+00008370: 2020 2020 2020 2020 2020 2063 616c 6c28             call(
+00008380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008390: 2020 2020 2027 504f 5354 272c 0a20 2020       'POST',.   
 000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083b0: 2020 2020 2020 2027 7474 6c27 3a20 3330         'ttl': 30
-000083c0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-000083d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000083e0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000083f0: 2020 2020 2020 2020 2020 2020 2063 616c               cal
-00008400: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00008410: 2020 2020 2020 2027 4445 4c45 5445 272c         'DELETE',
-00008420: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008430: 2020 2020 2027 2f7a 6f6e 6573 2f34 322f       '/zones/42/
-00008440: 646e 735f 7265 636f 7264 732f 6663 3132  dns_records/fc12
-00008450: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-00008460: 6162 3333 3232 3939 3736 3533 272c 0a20  ab3322997653',. 
-00008470: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008480: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008490: 2020 6361 6c6c 280a 2020 2020 2020 2020    call(.        
-000084a0: 2020 2020 2020 2020 2020 2020 2750 5554              'PUT
-000084b0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-000084c0: 2020 2020 2020 2027 2f7a 6f6e 6573 2f34         '/zones/4
-000084d0: 322f 7061 6765 7275 6c65 732f 3261 3931  2/pagerules/2a91
-000084e0: 3430 6231 3766 6662 3065 3661 6564 3832  40b17ffb0e6aed82
-000084f0: 3630 3439 6565 6339 3734 6237 272c 0a20  6049eec974b7',. 
-00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2020 2064 6174 613d 7b0a 2020 2020 2020     data={.      
-00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2020 2774 6172 6765 7473 273a 205b 0a20    'targets': [. 
-00008540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008550: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008570: 2020 2020 2020 2020 2020 2020 2027 7461               'ta
-00008580: 7267 6574 273a 2027 7572 6c27 2c0a 2020  rget': 'url',.  
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2020 2020 2020 2020 2020 2020 2763                'c
-000085b0: 6f6e 7374 7261 696e 7427 3a20 7b0a 2020  onstraint': {.  
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085e0: 2020 276f 7065 7261 746f 7227 3a20 276d    'operator': 'm
-000085f0: 6174 6368 6573 272c 0a20 2020 2020 2020  atches',.       
-00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008610: 2020 2020 2020 2020 2020 2020 2027 7661               'va
-00008620: 6c75 6527 3a20 2775 726c 6677 6431 2e75  lue': 'urlfwd1.u
-00008630: 6e69 742e 7465 7374 732f 272c 0a20 2020  nit.tests/',.   
-00008640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008650: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-00008660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008670: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008690: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086b0: 2027 6163 7469 6f6e 7327 3a20 5b0a 2020   'actions': [.  
-000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086d0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
+000083b0: 2027 2f7a 6f6e 6573 272c 0a20 2020 2020   '/zones',.     
+000083c0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000083d0: 6174 613d 7b27 6a75 6d70 5f73 7461 7274  ata={'jump_start
+000083e0: 273a 2046 616c 7365 2c20 276e 616d 6527  ': False, 'name'
+000083f0: 3a20 2775 6e69 742e 7465 7374 7327 7d2c  : 'unit.tests'},
+00008400: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008410: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00008420: 2020 2020 6361 6c6c 280a 2020 2020 2020      call(.      
+00008430: 2020 2020 2020 2020 2020 2020 2020 2750                'P
+00008440: 5554 272c 0a20 2020 2020 2020 2020 2020  UT',.           
+00008450: 2020 2020 2020 2020 2027 2f7a 6f6e 6573           '/zones
+00008460: 2f34 322f 646e 735f 7265 636f 7264 732f  /42/dns_records/
+00008470: 6663 3132 6162 3334 6364 3536 3131 3333  fc12ab34cd561133
+00008480: 3434 3232 6162 3333 3232 3939 3736 3534  4422ab3322997654
+00008490: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+000084a0: 2020 2020 2020 2064 6174 613d 7b0a 2020         data={.  
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 2020 2020 2763 6f6e 7465 6e74 273a        'content':
+000084d0: 2027 6e73 322e 666f 6f2e 6261 722e 272c   'ns2.foo.bar.',
+000084e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000084f0: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+00008500: 2027 4e53 272c 0a20 2020 2020 2020 2020   'NS',.         
+00008510: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00008520: 6e61 6d65 273a 2027 756e 6974 2e74 6573  name': 'unit.tes
+00008530: 7473 272c 0a20 2020 2020 2020 2020 2020  ts',.           
+00008540: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
+00008550: 6c27 3a20 3330 302c 0a20 2020 2020 2020  l': 300,.       
+00008560: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
+00008570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008580: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00008590: 2020 2063 616c 6c28 0a20 2020 2020 2020     call(.       
+000085a0: 2020 2020 2020 2020 2020 2020 2027 4445               'DE
+000085b0: 4c45 5445 272c 0a20 2020 2020 2020 2020  LETE',.         
+000085c0: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
+000085d0: 6573 2f34 322f 646e 735f 7265 636f 7264  es/42/dns_record
+000085e0: 732f 6663 3132 6162 3334 6364 3536 3131  s/fc12ab34cd5611
+000085f0: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+00008600: 3533 272c 0a20 2020 2020 2020 2020 2020  53',.           
+00008610: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00008620: 2020 2020 2020 2020 6361 6c6c 280a 2020          call(.  
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008640: 2020 2750 5554 272c 0a20 2020 2020 2020    'PUT',.       
+00008650: 2020 2020 2020 2020 2020 2020 2027 2f7a               '/z
+00008660: 6f6e 6573 2f34 322f 7061 6765 7275 6c65  ones/42/pagerule
+00008670: 732f 3261 3931 3430 6231 3766 6662 3065  s/2a9140b17ffb0e
+00008680: 3661 6564 3832 3630 3439 6565 6339 3734  6aed826049eec974
+00008690: 6237 272c 0a20 2020 2020 2020 2020 2020  b7',.           
+000086a0: 2020 2020 2020 2020 2064 6174 613d 7b0a           data={.
+000086b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086c0: 2020 2020 2020 2020 2774 6172 6765 7473          'targets
+000086d0: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
 000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086f0: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
-00008700: 3a20 2766 6f72 7761 7264 696e 675f 7572  : 'forwarding_ur
-00008710: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
-00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008730: 2020 2020 2776 616c 7565 273a 207b 0a20      'value': {. 
-00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008760: 2020 2027 7572 6c27 3a20 2768 7474 7073     'url': 'https
-00008770: 3a2f 2f77 7777 2e75 6e69 742e 7465 7374  ://www.unit.test
-00008780: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+000086f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 2027 7461 7267 6574 273a 2027 7572     'target': 'ur
+00008720: 6c27 2c0a 2020 2020 2020 2020 2020 2020  l',.            
+00008730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008740: 2020 2020 2763 6f6e 7374 7261 696e 7427      'constraint'
+00008750: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2020 2020 2020 2020 276f 7065 7261 746f          'operato
+00008780: 7227 3a20 276d 6174 6368 6573 272c 0a20  r': 'matches',. 
 00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 2020 2020 2773 7461 7475 735f          'status_
-000087b0: 636f 6465 273a 2033 3032 2c0a 2020 2020  code': 302,.    
-000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087d0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087b0: 2020 2027 7661 6c75 6527 3a20 2775 726c     'value': 'url
+000087c0: 6677 6431 2e75 6e69 742e 7465 7374 732f  fwd1.unit.tests/
+000087d0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
 000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087f0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+000087f0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
 00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008810: 2020 2020 205d 2c0a 2020 2020 2020 2020       ],.        
-00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2773 7461 7475 7327 3a20 2761 6374 6976  'status': 'activ
-00008840: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
-00008850: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00008860: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00008870: 2020 2020 2020 2020 2020 2020 2020 6361                ca
-00008880: 6c6c 280a 2020 2020 2020 2020 2020 2020  ll(.            
-00008890: 2020 2020 2020 2020 2744 454c 4554 4527          'DELETE'
-000088a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000088b0: 2020 2020 2020 272f 7a6f 6e65 732f 3432        '/zones/42
-000088c0: 2f70 6167 6572 756c 6573 2f32 6139 3134  /pagerules/2a914
-000088d0: 3162 3138 6666 6230 6536 6165 6438 3236  1b18ffb0e6aed826
-000088e0: 3035 3465 6563 3937 3062 3827 2c0a 2020  054eec970b8',.  
-000088f0: 2020 2020 2020 2020 2020 2020 2020 292c                ),
-00008900: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00008910: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-00008920: 6620 7465 7374 5f70 6167 6572 756c 6573  f test_pagerules
-00008930: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00008940: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
-00008950: 666c 6172 6550 726f 7669 6465 7228 0a20  flareProvider(. 
-00008960: 2020 2020 2020 2020 2020 2027 7465 7374             'test
-00008970: 272c 2027 656d 6169 6c27 2c20 2774 6f6b  ', 'email', 'tok
-00008980: 656e 272c 2072 6574 7279 5f70 6572 696f  en', retry_perio
-00008990: 643d 302c 2070 6167 6572 756c 6573 3d46  d=0, pagerules=F
-000089a0: 616c 7365 0a20 2020 2020 2020 2029 0a0a  alse.        )..
-000089b0: 2020 2020 2020 2020 2320 5365 7420 7468          # Set th
-000089c0: 696e 6773 2075 7020 746f 2070 7265 6578  ings up to preex
-000089d0: 6973 742f 6d6f 636b 2061 7320 6e65 6365  ist/mock as nece
-000089e0: 7373 6172 790a 2020 2020 2020 2020 7a6f  ssary.        zo
-000089f0: 6e65 203d 205a 6f6e 6528 2775 6e69 742e  ne = Zone('unit.
-00008a00: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
-00008a10: 2020 2020 2023 2053 7475 6666 2061 2066       # Stuff a f
-00008a20: 616b 6520 7a6f 6e65 2069 6420 696e 2070  ake zone id in p
-00008a30: 6c61 6365 0a20 2020 2020 2020 2070 726f  lace.        pro
-00008a40: 7669 6465 722e 5f7a 6f6e 6573 203d 207b  vider._zones = {
-00008a50: 7a6f 6e65 2e6e 616d 653a 2027 3432 277d  zone.name: '42'}
-00008a60: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
-00008a70: 722e 5f72 6571 7565 7374 203d 204d 6f63  r._request = Moc
-00008a80: 6b28 290a 2020 2020 2020 2020 7369 6465  k().        side
-00008a90: 5f65 6666 6563 7420 3d20 5b0a 2020 2020  _effect = [.    
-00008aa0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00008ab0: 2020 2020 2020 2020 2020 2772 6573 756c            'resul
-00008ac0: 7427 3a20 5b5d 2c0a 2020 2020 2020 2020  t': [],.        
-00008ad0: 2020 2020 2020 2020 2772 6573 756c 745f          'result_
-00008ae0: 696e 666f 273a 207b 2763 6f75 6e74 273a  info': {'count':
-00008af0: 2030 2c20 2770 6572 5f70 6167 6527 3a20   0, 'per_page': 
-00008b00: 3530 7d2c 0a20 2020 2020 2020 2020 2020  50},.           
-00008b10: 2020 2020 2023 202f 7a6f 6e65 732f 3432       # /zones/42
-00008b20: 2f64 6e73 5f72 6563 6f72 6473 0a20 2020  /dns_records.   
-00008b30: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00008b40: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00008b50: 2020 2020 2020 2020 2020 2772 6573 756c            'resul
-00008b60: 7427 3a20 5b0a 2020 2020 2020 2020 2020  t': [.          
-00008b70: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b90: 2020 2020 2269 6422 3a20 2232 6139 3134      "id": "2a914
-00008ba0: 3062 3137 6666 6230 6536 6165 6438 3236  0b17ffb0e6aed826
-00008bb0: 3034 3965 6563 3937 3462 3722 2c0a 2020  049eec974b7",.  
-00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bd0: 2020 2020 2020 2274 6172 6765 7473 223a        "targets":
-00008be0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-00008bf0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-00008c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c20: 2022 7461 7267 6574 223a 2022 7572 6c22   "target": "url"
-00008c30: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008810: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
+00008820: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008840: 2020 2020 2020 2027 6163 7469 6f6e 7327         'actions'
+00008850: 3a20 5b0a 2020 2020 2020 2020 2020 2020  : [.            
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00008880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008890: 2020 2769 6427 3a20 2766 6f72 7761 7264    'id': 'forward
+000088a0: 696e 675f 7572 6c27 2c0a 2020 2020 2020  ing_url',.      
+000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088c0: 2020 2020 2020 2020 2020 2776 616c 7565            'value
+000088d0: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
+000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088f0: 2020 2020 2020 2020 2027 7572 6c27 3a20           'url': 
+00008900: 2768 7474 7073 3a2f 2f77 7777 2e75 6e69  'https://www.uni
+00008910: 742e 7465 7374 7327 2c0a 2020 2020 2020  t.tests',.      
+00008920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008930: 2020 2020 2020 2020 2020 2020 2020 2773                's
+00008940: 7461 7475 735f 636f 6465 273a 2033 3032  tatus_code': 302
+00008950: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008990: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+000089a0: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
+000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089c0: 2020 2020 2020 2773 7461 7475 7327 3a20        'status': 
+000089d0: 2761 6374 6976 6527 2c0a 2020 2020 2020  'active',.      
+000089e0: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+000089f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008a00: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00008a10: 2020 2020 6361 6c6c 280a 2020 2020 2020      call(.      
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2744                'D
+00008a30: 454c 4554 4527 2c0a 2020 2020 2020 2020  ELETE',.        
+00008a40: 2020 2020 2020 2020 2020 2020 272f 7a6f              '/zo
+00008a50: 6e65 732f 3432 2f70 6167 6572 756c 6573  nes/42/pagerules
+00008a60: 2f32 6139 3134 3162 3138 6666 6230 6536  /2a9141b18ffb0e6
+00008a70: 6165 6438 3236 3035 3465 6563 3937 3062  aed826054eec970b
+00008a80: 3827 2c0a 2020 2020 2020 2020 2020 2020  8',.            
+00008a90: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00008aa0: 2020 205d 0a20 2020 2020 2020 2029 0a0a     ].        )..
+00008ab0: 2020 2020 6465 6620 7465 7374 5f70 6167      def test_pag
+00008ac0: 6572 756c 6573 2873 656c 6629 3a0a 2020  erules(self):.  
+00008ad0: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
+00008ae0: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
+00008af0: 6465 7228 0a20 2020 2020 2020 2020 2020  der(.           
+00008b00: 2027 7465 7374 272c 2027 656d 6169 6c27   'test', 'email'
+00008b10: 2c20 2774 6f6b 656e 272c 2072 6574 7279  , 'token', retry
+00008b20: 5f70 6572 696f 643d 302c 2070 6167 6572  _period=0, pager
+00008b30: 756c 6573 3d46 616c 7365 0a20 2020 2020  ules=False.     
+00008b40: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+00008b50: 5365 7420 7468 696e 6773 2075 7020 746f  Set things up to
+00008b60: 2070 7265 6578 6973 742f 6d6f 636b 2061   preexist/mock a
+00008b70: 7320 6e65 6365 7373 6172 790a 2020 2020  s necessary.    
+00008b80: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
+00008b90: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
+00008ba0: 5d29 0a20 2020 2020 2020 2023 2053 7475  ]).        # Stu
+00008bb0: 6666 2061 2066 616b 6520 7a6f 6e65 2069  ff a fake zone i
+00008bc0: 6420 696e 2070 6c61 6365 0a20 2020 2020  d in place.     
+00008bd0: 2020 2070 726f 7669 6465 722e 5f7a 6f6e     provider._zon
+00008be0: 6573 203d 207b 7a6f 6e65 2e6e 616d 653a  es = {zone.name:
+00008bf0: 2027 3432 277d 0a20 2020 2020 2020 2070   '42'}.        p
+00008c00: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
+00008c10: 203d 204d 6f63 6b28 290a 2020 2020 2020   = Mock().      
+00008c20: 2020 7369 6465 5f65 6666 6563 7420 3d20    side_effect = 
+00008c30: 5b0a 2020 2020 2020 2020 2020 2020 7b0a  [.            {.
 00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c50: 2020 2263 6f6e 7374 7261 696e 7422 3a20    "constraint": 
-00008c60: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c80: 2020 2020 2020 226f 7065 7261 746f 7222        "operator"
-00008c90: 3a20 226d 6174 6368 6573 222c 0a20 2020  : "matches",.   
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cc0: 2022 7661 6c75 6522 3a20 2275 726c 6677   "value": "urlfw
-00008cd0: 6431 2e75 6e69 742e 7465 7374 732f 222c  d1.unit.tests/",
-00008ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00008d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d20: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00008d30: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 2020 2020 2022 6163 7469 6f6e 7322 3a20       "actions": 
-00008d60: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00008d70: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+00008c50: 2772 6573 756c 7427 3a20 5b5d 2c0a 2020  'result': [],.  
+00008c60: 2020 2020 2020 2020 2020 2020 2020 2772                'r
+00008c70: 6573 756c 745f 696e 666f 273a 207b 2763  esult_info': {'c
+00008c80: 6f75 6e74 273a 2030 2c20 2770 6572 5f70  ount': 0, 'per_p
+00008c90: 6167 6527 3a20 3530 7d2c 0a20 2020 2020  age': 50},.     
+00008ca0: 2020 2020 2020 2020 2020 2023 202f 7a6f             # /zo
+00008cb0: 6e65 732f 3432 2f64 6e73 5f72 6563 6f72  nes/42/dns_recor
+00008cc0: 6473 0a20 2020 2020 2020 2020 2020 207d  ds.            }
+00008cd0: 2c0a 2020 2020 2020 2020 2020 2020 7b0a  ,.            {.
+00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008cf0: 2772 6573 756c 7427 3a20 5b0a 2020 2020  'result': [.    
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00008d20: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+00008d30: 2232 6139 3134 3062 3137 6666 6230 6536  "2a9140b17ffb0e6
+00008d40: 6165 6438 3236 3034 3965 6563 3937 3462  aed826049eec974b
+00008d50: 3722 2c0a 2020 2020 2020 2020 2020 2020  7",.            
+00008d60: 2020 2020 2020 2020 2020 2020 2274 6172              "tar
+00008d70: 6765 7473 223a 205b 0a20 2020 2020 2020  gets": [.       
 00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008da0: 2269 6422 3a20 2266 6f72 7761 7264 696e  "id": "forwardin
-00008db0: 675f 7572 6c22 2c0a 2020 2020 2020 2020  g_url",.        
-00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2020 2020 2020 2020 2276 616c 7565 223a          "value":
-00008de0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00008df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e00: 2020 2020 2020 2022 7572 6c22 3a20 2268         "url": "h
-00008e10: 7474 7073 3a2f 2f77 7777 2e75 6e69 742e  ttps://www.unit.
-00008e20: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
-00008e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e40: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
-00008e50: 7475 735f 636f 6465 223a 2033 3032 2c0a  tus_code": 302,.
-00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e80: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-00008e90: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00008ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008eb0: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00008d90: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2020 2020 2020 2022 7461 7267 6574 223a         "target":
+00008dc0: 2022 7572 6c22 2c0a 2020 2020 2020 2020   "url",.        
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 2020 2020 2263 6f6e 7374 7261          "constra
+00008df0: 696e 7422 3a20 7b0a 2020 2020 2020 2020  int": {.        
+00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e10: 2020 2020 2020 2020 2020 2020 226f 7065              "ope
+00008e20: 7261 746f 7222 3a20 226d 6174 6368 6573  rator": "matches
+00008e30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e50: 2020 2020 2020 2022 7661 6c75 6522 3a20         "value": 
+00008e60: 2275 726c 6677 6431 2e75 6e69 742e 7465  "urlfwd1.unit.te
+00008e70: 7374 732f 222c 0a20 2020 2020 2020 2020  sts/",.         
+00008e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e90: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008eb0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
 00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ed0: 2020 2020 2270 7269 6f72 6974 7922 3a20      "priority": 
-00008ee0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-00008ef0: 2020 2020 2020 2020 2020 2022 7374 6174             "stat
-00008f00: 7573 223a 2022 6163 7469 7665 222c 0a20  us": "active",. 
-00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f20: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-00008f30: 6f6e 223a 2022 3230 3231 2d30 362d 3235  on": "2021-06-25
-00008f40: 5432 303a 3130 3a35 302e 3030 3030 3030  T20:10:50.000000
-00008f50: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-00008f60: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
-00008f70: 6966 6965 645f 6f6e 223a 2022 3230 3231  ified_on": "2021
-00008f80: 2d30 362d 3238 5432 323a 3338 3a31 302e  -06-28T22:38:10.
-00008f90: 3030 3030 3030 5a22 2c0a 2020 2020 2020  000000Z",.      
-00008fa0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fc0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00008fd0: 2020 2027 7265 7375 6c74 5f69 6e66 6f27     'result_info'
-00008fe0: 3a20 7b27 636f 756e 7427 3a20 312c 2027  : {'count': 1, '
-00008ff0: 7065 725f 7061 6765 273a 2035 307d 2c0a  per_page': 50},.
+00008ed0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00008ee0: 2020 2020 2020 2020 2020 2022 6163 7469             "acti
+00008ef0: 6f6e 7322 3a20 5b0a 2020 2020 2020 2020  ons": [.        
+00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f10: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f30: 2020 2020 2020 2269 6422 3a20 2266 6f72        "id": "for
+00008f40: 7761 7264 696e 675f 7572 6c22 2c0a 2020  warding_url",.  
+00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f60: 2020 2020 2020 2020 2020 2020 2020 2276                "v
+00008f70: 616c 7565 223a 207b 0a20 2020 2020 2020  alue": {.       
+00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f90: 2020 2020 2020 2020 2020 2020 2022 7572               "ur
+00008fa0: 6c22 3a20 2268 7474 7073 3a2f 2f77 7777  l": "https://www
+00008fb0: 2e75 6e69 742e 7465 7374 7322 2c0a 2020  .unit.tests",.  
+00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 2020 2273 7461 7475 735f 636f 6465 223a    "status_code":
+00008ff0: 2033 3032 2c0a 2020 2020 2020 2020 2020   302,.          
 00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009010: 2320 2f7a 6f6e 6573 2f34 322f 7061 6765  # /zones/42/page
-00009020: 7275 6c65 730a 2020 2020 2020 2020 2020  rules.          
-00009030: 2020 7d2c 0a20 2020 2020 2020 205d 0a20    },.        ]. 
-00009040: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00009050: 5f72 6571 7565 7374 2e73 6964 655f 6566  _request.side_ef
-00009060: 6665 6374 203d 2073 6964 655f 6566 6665  fect = side_effe
-00009070: 6374 0a0a 2020 2020 2020 2020 2320 4e6f  ct..        # No
-00009080: 7720 7765 2070 6f70 756c 6174 652c 2061  w we populate, a
-00009090: 6e64 2065 7870 6563 7420 746f 2073 6565  nd expect to see
-000090a0: 206e 6f74 6869 6e67 0a20 2020 2020 2020   nothing.       
-000090b0: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-000090c0: 6528 7072 6f76 6964 6572 2e70 6c61 6e28  e(provider.plan(
-000090d0: 7a6f 6e65 2929 0a20 2020 2020 2020 2023  zone)).        #
-000090e0: 2057 6520 7368 6f75 6c64 2068 6176 6520   We should have 
-000090f0: 6861 6420 6f6e 6c79 2061 2073 696e 676c  had only a singl
-00009100: 6520 6361 6c6c 2074 6f20 6765 7420 7468  e call to get th
-00009110: 6520 646e 735f 7265 636f 7264 732c 206e  e dns_records, n
-00009120: 6f0a 2020 2020 2020 2020 2320 6361 6c6c  o.        # call
-00009130: 7320 746f 2070 6167 6572 756c 6573 0a20  s to pagerules. 
-00009140: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00009150: 5f72 6571 7565 7374 2e61 7373 6572 745f  _request.assert_
-00009160: 6361 6c6c 6564 5f6f 6e63 6528 290a 0a20  called_once().. 
-00009170: 2020 2020 2020 2023 2072 6573 6574 2074         # reset t
-00009180: 6869 6e67 730a 2020 2020 2020 2020 7072  hings.        pr
-00009190: 6f76 6964 6572 2e5f 7a6f 6e65 5f72 6563  ovider._zone_rec
-000091a0: 6f72 6473 203d 207b 7d0a 2020 2020 2020  ords = {}.      
-000091b0: 2020 7072 6f76 6964 6572 2e53 5550 504f    provider.SUPPO
-000091c0: 5254 532e 6164 6428 2755 524c 4657 4427  RTS.add('URLFWD'
-000091d0: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
-000091e0: 6572 2e5f 7265 7175 6573 742e 7369 6465  er._request.side
-000091f0: 5f65 6666 6563 7420 3d20 7369 6465 5f65  _effect = side_e
-00009200: 6666 6563 740a 2020 2020 2020 2020 2320  ffect.        # 
-00009210: 656e 6162 6c65 2070 6167 6572 756c 6573  enable pagerules
-00009220: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
-00009230: 722e 7061 6765 7275 6c65 7320 3d20 5472  r.pagerules = Tr
-00009240: 7565 0a20 2020 2020 2020 2023 2070 6c61  ue.        # pla
-00009250: 6e20 6167 6169 6e2c 2074 6869 7320 7469  n again, this ti
-00009260: 6d65 2077 6520 6578 7065 6374 2062 6f74  me we expect bot
-00009270: 6820 6361 6c6c 7320 616e 6420 6120 7265  h calls and a re
-00009280: 636f 7264 0a20 2020 2020 2020 2070 6c61  cord.        pla
-00009290: 6e20 3d20 7072 6f76 6964 6572 2e70 6c61  n = provider.pla
-000092a0: 6e28 7a6f 6e65 290a 2020 2020 2020 2020  n(zone).        
-000092b0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000092c0: 2831 2c20 6c65 6e28 706c 616e 2e63 6861  (1, len(plan.cha
-000092d0: 6e67 6573 2929 0a20 2020 2020 2020 2063  nges)).        c
-000092e0: 6861 6e67 6520 3d20 6c69 7374 2870 6c61  hange = list(pla
-000092f0: 6e2e 6368 616e 6765 7329 5b30 5d0a 2020  n.changes)[0].  
-00009300: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00009310: 7445 7175 616c 2827 5552 4c46 5744 272c  tEqual('URLFWD',
-00009320: 2063 6861 6e67 652e 7265 636f 7264 2e5f   change.record._
-00009330: 7479 7065 290a 2020 2020 2020 2020 7072  type).        pr
-00009340: 6f76 6964 6572 2e5f 7265 7175 6573 742e  ovider._request.
-00009350: 6173 7365 7274 5f68 6173 5f63 616c 6c73  assert_has_calls
-00009360: 280a 2020 2020 2020 2020 2020 2020 5b0a  (.            [.
-00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009380: 6361 6c6c 280a 2020 2020 2020 2020 2020  call(.          
-00009390: 2020 2020 2020 2020 2020 2747 4554 272c            'GET',
-000093a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000093b0: 2020 2020 2027 2f7a 6f6e 6573 2f34 322f       '/zones/42/
-000093c0: 646e 735f 7265 636f 7264 7327 2c0a 2020  dns_records',.  
-000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093e0: 2020 7061 7261 6d73 3d7b 2770 6167 6527    params={'page'
-000093f0: 3a20 312c 2027 7065 725f 7061 6765 273a  : 1, 'per_page':
-00009400: 2031 3030 7d2c 0a20 2020 2020 2020 2020   100},.         
-00009410: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00009420: 2020 2020 2020 2020 2020 6361 6c6c 2827            call('
-00009430: 4745 5427 2c20 272f 7a6f 6e65 732f 3432  GET', '/zones/42
-00009440: 2f70 6167 6572 756c 6573 272c 2070 6172  /pagerules', par
-00009450: 616d 733d 7b27 7374 6174 7573 273a 2027  ams={'status': '
-00009460: 6163 7469 7665 277d 292c 0a20 2020 2020  active'}),.     
-00009470: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
-00009480: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
-00009490: 5f70 7472 2873 656c 6629 3a0a 2020 2020  _ptr(self):.    
-000094a0: 2020 2020 7072 6f76 6964 6572 203d 2043      provider = C
-000094b0: 6c6f 7564 666c 6172 6550 726f 7669 6465  loudflareProvide
-000094c0: 7228 2774 6573 7427 2c20 2765 6d61 696c  r('test', 'email
-000094d0: 272c 2027 746f 6b65 6e27 290a 0a20 2020  ', 'token')..   
-000094e0: 2020 2020 207a 6f6e 6520 3d20 5a6f 6e65       zone = Zone
-000094f0: 2827 756e 6974 2e74 6573 7473 2e27 2c20  ('unit.tests.', 
-00009500: 5b5d 290a 2020 2020 2020 2020 2320 5054  []).        # PT
-00009510: 5220 7265 636f 7264 0a20 2020 2020 2020  R record.       
-00009520: 2070 7472 5f72 6563 6f72 6420 3d20 5265   ptr_record = Re
-00009530: 636f 7264 2e6e 6577 280a 2020 2020 2020  cord.new(.      
-00009540: 2020 2020 2020 7a6f 6e65 2c20 2770 7472        zone, 'ptr
-00009550: 272c 207b 2774 746c 273a 2033 3030 2c20  ', {'ttl': 300, 
-00009560: 2774 7970 6527 3a20 2750 5452 272c 2027  'type': 'PTR', '
-00009570: 7661 6c75 6527 3a20 2766 6f6f 2e62 6172  value': 'foo.bar
-00009580: 2e63 6f6d 2e27 7d0a 2020 2020 2020 2020  .com.'}.        
-00009590: 290a 0a20 2020 2020 2020 2070 7472 5f72  )..        ptr_r
-000095a0: 6563 6f72 645f 636f 6e74 656e 7473 203d  ecord_contents =
-000095b0: 2070 726f 7669 6465 722e 5f67 656e 5f64   provider._gen_d
-000095c0: 6174 6128 7074 725f 7265 636f 7264 290a  ata(ptr_record).
-000095d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-000095e0: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
-000095f0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-00009600: 2020 2020 2020 2020 276e 616d 6527 3a20          'name': 
-00009610: 2770 7472 2e75 6e69 742e 7465 7374 7327  'ptr.unit.tests'
-00009620: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009630: 2020 2774 746c 273a 2033 3030 2c0a 2020    'ttl': 300,.  
-00009640: 2020 2020 2020 2020 2020 2020 2020 2774                't
-00009650: 7970 6527 3a20 2750 5452 272c 0a20 2020  ype': 'PTR',.   
-00009660: 2020 2020 2020 2020 2020 2020 2027 636f               'co
-00009670: 6e74 656e 7427 3a20 2766 6f6f 2e62 6172  ntent': 'foo.bar
-00009680: 2e63 6f6d 2e27 2c0a 2020 2020 2020 2020  .com.',.        
-00009690: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-000096a0: 2020 206c 6973 7428 7074 725f 7265 636f     list(ptr_reco
-000096b0: 7264 5f63 6f6e 7465 6e74 7329 5b30 5d2c  rd_contents)[0],
-000096c0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-000096d0: 6465 6620 7465 7374 5f6c 6f63 2873 656c  def test_loc(sel
-000096e0: 6629 3a0a 2020 2020 2020 2020 7365 6c66  f):.        self
-000096f0: 2e6d 6178 4469 6666 203d 204e 6f6e 650a  .maxDiff = None.
-00009700: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
-00009710: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
-00009720: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
-00009730: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
-00009740: 0a20 2020 2020 2020 207a 6f6e 6520 3d20  .        zone = 
-00009750: 5a6f 6e65 2827 756e 6974 2e74 6573 7473  Zone('unit.tests
-00009760: 2e27 2c20 5b5d 290a 2020 2020 2020 2020  .', []).        
-00009770: 2320 4c4f 4320 7265 636f 7264 0a20 2020  # LOC record.   
-00009780: 2020 2020 206c 6f63 5f72 6563 6f72 6420       loc_record 
-00009790: 3d20 5265 636f 7264 2e6e 6577 280a 2020  = Record.new(.  
-000097a0: 2020 2020 2020 2020 2020 7a6f 6e65 2c0a            zone,.
-000097b0: 2020 2020 2020 2020 2020 2020 2765 7861              'exa
-000097c0: 6d70 6c65 272c 0a20 2020 2020 2020 2020  mple',.         
-000097d0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-000097e0: 2020 2020 2027 7474 6c27 3a20 3330 302c       'ttl': 300,
-000097f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009800: 2027 7479 7065 273a 2027 4c4f 4327 2c0a   'type': 'LOC',.
-00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2776 616c 7565 273a 207b 0a20 2020 2020  'value': {.     
-00009830: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00009840: 6c61 745f 6465 6772 6565 7327 3a20 3331  lat_degrees': 31
-00009850: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009860: 2020 2020 2020 276c 6174 5f6d 696e 7574        'lat_minut
-00009870: 6573 273a 2035 382c 0a20 2020 2020 2020  es': 58,.       
-00009880: 2020 2020 2020 2020 2020 2020 2027 6c61               'la
-00009890: 745f 7365 636f 6e64 7327 3a20 3532 2e31  t_seconds': 52.1
-000098a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000098b0: 2020 2020 2020 276c 6174 5f64 6972 6563        'lat_direc
-000098c0: 7469 6f6e 273a 2027 5327 2c0a 2020 2020  tion': 'S',.    
-000098d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098e0: 276c 6f6e 675f 6465 6772 6565 7327 3a20  'long_degrees': 
-000098f0: 3131 352c 0a20 2020 2020 2020 2020 2020  115,.           
-00009900: 2020 2020 2020 2020 2027 6c6f 6e67 5f6d           'long_m
-00009910: 696e 7574 6573 273a 2034 392c 0a20 2020  inutes': 49,.   
-00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009930: 2027 6c6f 6e67 5f73 6563 6f6e 6473 273a   'long_seconds':
-00009940: 2031 312e 372c 0a20 2020 2020 2020 2020   11.7,.         
-00009950: 2020 2020 2020 2020 2020 2027 6c6f 6e67             'long
-00009960: 5f64 6972 6563 7469 6f6e 273a 2027 4527  _direction': 'E'
-00009970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00009980: 2020 2020 2020 2761 6c74 6974 7564 6527        'altitude'
-00009990: 3a20 3230 2c0a 2020 2020 2020 2020 2020  : 20,.          
-000099a0: 2020 2020 2020 2020 2020 2773 697a 6527            'size'
-000099b0: 3a20 3130 2c0a 2020 2020 2020 2020 2020  : 10,.          
-000099c0: 2020 2020 2020 2020 2020 2770 7265 6369            'preci
-000099d0: 7369 6f6e 5f68 6f72 7a27 3a20 3130 2c0a  sion_horz': 10,.
-000099e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099f0: 2020 2020 2770 7265 6369 7369 6f6e 5f76      'precision_v
-00009a00: 6572 7427 3a20 322c 0a20 2020 2020 2020  ert': 2,.       
-00009a10: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00009a20: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00009a30: 2020 2029 0a0a 2020 2020 2020 2020 6c6f     )..        lo
-00009a40: 635f 7265 636f 7264 5f63 6f6e 7465 6e74  c_record_content
-00009a50: 7320 3d20 7072 6f76 6964 6572 2e5f 6765  s = provider._ge
-00009a60: 6e5f 6461 7461 286c 6f63 5f72 6563 6f72  n_data(loc_recor
-00009a70: 6429 0a20 2020 2020 2020 2073 656c 662e  d).        self.
-00009a80: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-00009a90: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-00009aa0: 2020 2020 2020 2020 2020 2027 6e61 6d65             'name
-00009ab0: 273a 2027 6578 616d 706c 652e 756e 6974  ': 'example.unit
-00009ac0: 2e74 6573 7473 272c 0a20 2020 2020 2020  .tests',.       
-00009ad0: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
-00009ae0: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
-00009af0: 2020 2020 2027 7479 7065 273a 2027 4c4f       'type': 'LO
-00009b00: 4327 2c0a 2020 2020 2020 2020 2020 2020  C',.            
-00009b10: 2020 2020 2764 6174 6127 3a20 7b0a 2020      'data': {.  
-00009b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b30: 2020 276c 6174 5f64 6567 7265 6573 273a    'lat_degrees':
-00009b40: 2033 312c 0a20 2020 2020 2020 2020 2020   31,.           
-00009b50: 2020 2020 2020 2020 2027 6c61 745f 6d69           'lat_mi
-00009b60: 6e75 7465 7327 3a20 3538 2c0a 2020 2020  nutes': 58,.    
-00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 276c 6174 5f73 6563 6f6e 6473 273a 2035  'lat_seconds': 5
-00009b90: 322e 312c 0a20 2020 2020 2020 2020 2020  2.1,.           
-00009ba0: 2020 2020 2020 2020 2027 6c61 745f 6469           'lat_di
-00009bb0: 7265 6374 696f 6e27 3a20 2753 272c 0a20  rection': 'S',. 
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 2020 2027 6c6f 6e67 5f64 6567 7265 6573     'long_degrees
-00009be0: 273a 2031 3135 2c0a 2020 2020 2020 2020  ': 115,.        
-00009bf0: 2020 2020 2020 2020 2020 2020 276c 6f6e              'lon
-00009c00: 675f 6d69 6e75 7465 7327 3a20 3439 2c0a  g_minutes': 49,.
-00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c20: 2020 2020 276c 6f6e 675f 7365 636f 6e64      'long_second
-00009c30: 7327 3a20 3131 2e37 2c0a 2020 2020 2020  s': 11.7,.      
-00009c40: 2020 2020 2020 2020 2020 2020 2020 276c                'l
-00009c50: 6f6e 675f 6469 7265 6374 696f 6e27 3a20  ong_direction': 
-00009c60: 2745 272c 0a20 2020 2020 2020 2020 2020  'E',.           
-00009c70: 2020 2020 2020 2020 2027 616c 7469 7475           'altitu
-00009c80: 6465 273a 2032 302c 0a20 2020 2020 2020  de': 20,.       
-00009c90: 2020 2020 2020 2020 2020 2020 2027 7369               'si
-00009ca0: 7a65 273a 2031 302c 0a20 2020 2020 2020  ze': 10,.       
-00009cb0: 2020 2020 2020 2020 2020 2020 2027 7072               'pr
-00009cc0: 6563 6973 696f 6e5f 686f 727a 273a 2031  ecision_horz': 1
-00009cd0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00009ce0: 2020 2020 2020 2027 7072 6563 6973 696f         'precisio
-00009cf0: 6e5f 7665 7274 273a 2032 2c0a 2020 2020  n_vert': 2,.    
-00009d00: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00009d10: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-00009d20: 2020 2020 2020 2020 2020 6c69 7374 286c            list(l
-00009d30: 6f63 5f72 6563 6f72 645f 636f 6e74 656e  oc_record_conten
-00009d40: 7473 295b 305d 2c0a 2020 2020 2020 2020  ts)[0],.        
-00009d50: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00009d60: 6e61 7074 7228 7365 6c66 293a 0a20 2020  naptr(self):.   
-00009d70: 2020 2020 2073 656c 662e 6d61 7844 6966       self.maxDif
-00009d80: 6620 3d20 4e6f 6e65 0a20 2020 2020 2020  f = None.       
-00009d90: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
-00009da0: 6466 6c61 7265 5072 6f76 6964 6572 2827  dflareProvider('
-00009db0: 7465 7374 272c 2027 656d 6169 6c27 2c20  test', 'email', 
-00009dc0: 2774 6f6b 656e 2729 0a0a 2020 2020 2020  'token')..      
-00009dd0: 2020 6366 5f64 6174 6120 3d20 7b0a 2020    cf_data = {.  
-00009de0: 2020 2020 2020 2020 2020 2763 6f6d 6d65            'comme
-00009df0: 6e74 273a 204e 6f6e 652c 0a20 2020 2020  nt': None,.     
-00009e00: 2020 2020 2020 2027 636f 6e74 656e 7427         'content'
-00009e10: 3a20 2732 3020 3130 3020 2253 2220 2253  : '20 100 "S" "S
-00009e20: 4950 2b44 3255 2220 2222 205f 7369 702e  IP+D2U" "" _sip.
-00009e30: 5f75 6470 2e75 6e69 742e 7465 7374 732e  _udp.unit.tests.
-00009e40: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00009e50: 6372 6561 7465 645f 6f6e 273a 2027 3230  created_on': '20
-00009e60: 3233 2d30 312d 3038 5430 313a 3032 3a33  23-01-08T01:02:3
-00009e70: 342e 3536 3739 3835 5a27 2c0a 2020 2020  4.567985Z',.    
-00009e80: 2020 2020 2020 2020 2764 6174 6127 3a20          'data': 
-00009e90: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00009ea0: 2020 2766 6c61 6773 273a 2027 5327 2c0a    'flags': 'S',.
-00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ec0: 276f 7264 6572 273a 2032 302c 0a20 2020  'order': 20,.   
-00009ed0: 2020 2020 2020 2020 2020 2020 2027 7072               'pr
-00009ee0: 6566 6572 656e 6365 273a 2031 3030 2c0a  eference': 100,.
-00009ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f00: 2772 6567 6578 273a 2027 272c 0a20 2020  'regex': '',.   
-00009f10: 2020 2020 2020 2020 2020 2020 2027 7265               're
-00009f20: 706c 6163 656d 656e 7427 3a20 275f 7369  placement': '_si
-00009f30: 702e 5f75 6470 2e75 6e69 742e 7465 7374  p._udp.unit.test
-00009f40: 732e 272c 0a20 2020 2020 2020 2020 2020  s.',.           
-00009f50: 2020 2020 2027 7365 7276 6963 6527 3a20       'service': 
-00009f60: 2753 4950 2b44 3255 272c 0a20 2020 2020  'SIP+D2U',.     
-00009f70: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-00009f80: 2020 2020 2020 2769 6427 3a20 2738 6236        'id': '8b6
-00009f90: 3063 3835 3138 6430 3934 3635 6666 6337  0c8518d09465ffc7
-00009fa0: 3734 3162 3761 3461 3433 3166 3938 272c  741b7a4a431f98',
-00009fb0: 0a20 2020 2020 2020 2020 2020 2027 6c6f  .            'lo
-00009fc0: 636b 6564 273a 2046 616c 7365 2c0a 2020  cked': False,.  
-00009fd0: 2020 2020 2020 2020 2020 276d 6574 6127            'meta'
-00009fe0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-00009ff0: 2020 2020 2761 7574 6f5f 6164 6465 6427      'auto_added'
-0000a000: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-0000a010: 2020 2020 2020 2020 2027 6d61 6e61 6765           'manage
-0000a020: 645f 6279 5f61 7070 7327 3a20 4661 6c73  d_by_apps': Fals
-0000a030: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000a040: 2020 2027 6d61 6e61 6765 645f 6279 5f61     'managed_by_a
-0000a050: 7267 6f5f 7475 6e6e 656c 273a 2046 616c  rgo_tunnel': Fal
-0000a060: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0000a070: 2020 2020 2773 6f75 7263 6527 3a20 2770      'source': 'p
-0000a080: 7269 6d61 7279 272c 0a20 2020 2020 2020  rimary',.       
-0000a090: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
-0000a0a0: 2020 2020 276d 6f64 6966 6965 645f 6f6e      'modified_on
-0000a0b0: 273a 2027 3230 3233 2d30 312d 3038 5430  ': '2023-01-08T0
-0000a0c0: 313a 3032 3a33 342e 3536 3739 3835 5a27  1:02:34.567985Z'
-0000a0d0: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-0000a0e0: 616d 6527 3a20 276e 6170 7472 2e75 6e69  ame': 'naptr.uni
-0000a0f0: 742e 7465 7374 7327 2c0a 2020 2020 2020  t.tests',.      
-0000a100: 2020 2020 2020 2770 726f 7869 6162 6c65        'proxiable
-0000a110: 273a 2046 616c 7365 2c0a 2020 2020 2020  ': False,.      
-0000a120: 2020 2020 2020 2770 726f 7869 6564 273a        'proxied':
-0000a130: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-0000a140: 2020 2020 2774 6167 7327 3a20 5b5d 2c0a      'tags': [],.
-0000a150: 2020 2020 2020 2020 2020 2020 2774 746c              'ttl
-0000a160: 273a 2031 2c0a 2020 2020 2020 2020 2020  ': 1,.          
-0000a170: 2020 2774 7970 6527 3a20 274e 4150 5452    'type': 'NAPTR
-0000a180: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-0000a190: 7a6f 6e65 5f69 6427 3a20 2764 3531 3564  zone_id': 'd515d
-0000a1a0: 6566 6534 3162 3137 3362 6565 3934 3838  efe41b173bee9488
-0000a1b0: 6439 6134 6235 6635 6465 3966 272c 0a20  d9a4b5f5de9f',. 
-0000a1c0: 2020 2020 2020 2020 2020 2027 7a6f 6e65             'zone
-0000a1d0: 5f6e 616d 6527 3a20 2775 6e69 742e 7465  _name': 'unit.te
-0000a1e0: 7374 7327 2c0a 2020 2020 2020 2020 7d0a  sts',.        }.
-0000a1f0: 2020 2020 2020 2020 6461 7461 203d 2070          data = p
-0000a200: 726f 7669 6465 722e 5f64 6174 615f 666f  rovider._data_fo
-0000a210: 725f 4e41 5054 5228 274e 4150 5452 272c  r_NAPTR('NAPTR',
-0000a220: 205b 6366 5f64 6174 615d 290a 2020 2020   [cf_data]).    
-0000a230: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000a240: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-0000a250: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-0000a260: 2020 2020 2774 746c 273a 2033 3030 2c0a      'ttl': 300,.
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a280: 2774 7970 6527 3a20 274e 4150 5452 272c  'type': 'NAPTR',
-0000a290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a2a0: 2027 7661 6c75 6573 273a 205b 0a20 2020   'values': [.   
-0000a2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2c0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0000a2d0: 2020 2020 2020 2020 2020 2027 666c 6167             'flag
-0000a2e0: 7327 3a20 2753 272c 0a20 2020 2020 2020  s': 'S',.       
-0000a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a300: 2027 6f72 6465 7227 3a20 3230 2c0a 2020   'order': 20,.  
-0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a320: 2020 2020 2020 2770 7265 6665 7265 6e63        'preferenc
-0000a330: 6527 3a20 3130 302c 0a20 2020 2020 2020  e': 100,.       
-0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a350: 2027 7265 6765 7870 273a 2027 272c 0a20   'regexp': '',. 
-0000a360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a370: 2020 2020 2020 2027 7265 706c 6163 656d         'replacem
-0000a380: 656e 7427 3a20 275f 7369 702e 5f75 6470  ent': '_sip._udp
-0000a390: 2e75 6e69 742e 7465 7374 732e 272c 0a20  .unit.tests.',. 
-0000a3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3b0: 2020 2020 2020 2027 7365 7276 6963 6527         'service'
-0000a3c0: 3a20 2753 4950 2b44 3255 272c 0a20 2020  : 'SIP+D2U',.   
-0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a3e0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-0000a3f0: 2020 205d 2c0a 2020 2020 2020 2020 2020     ],.          
-0000a400: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-0000a410: 2064 6174 612c 0a20 2020 2020 2020 2029   data,.        )
-0000a420: 0a0a 2020 2020 2020 2020 7a6f 6e65 203d  ..        zone =
-0000a430: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
-0000a440: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
-0000a450: 2072 6563 6f72 6420 3d20 5265 636f 7264   record = Record
-0000a460: 2e6e 6577 287a 6f6e 652c 2027 6e61 7074  .new(zone, 'napt
-0000a470: 7227 2c20 6461 7461 290a 2020 2020 2020  r', data).      
-0000a480: 2020 636f 6e74 656e 7473 203d 206c 6973    contents = lis
-0000a490: 7428 7072 6f76 6964 6572 2e5f 636f 6e74  t(provider._cont
-0000a4a0: 656e 7473 5f66 6f72 5f4e 4150 5452 2872  ents_for_NAPTR(r
-0000a4b0: 6563 6f72 6429 290a 2020 2020 2020 2020  ecord)).        
-0000a4c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000a4d0: 285b 7b27 6461 7461 273a 2063 665f 6461  ([{'data': cf_da
-0000a4e0: 7461 5b27 6461 7461 275d 7d5d 2c20 636f  ta['data']}], co
-0000a4f0: 6e74 656e 7473 290a 0a20 2020 2020 2020  ntents)..       
-0000a500: 206b 6579 203d 2070 726f 7669 6465 722e   key = provider.
-0000a510: 5f67 656e 5f6b 6579 2863 665f 6461 7461  _gen_key(cf_data
-0000a520: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-0000a530: 7373 6572 7445 7175 616c 2827 3230 2031  ssertEqual('20 1
-0000a540: 3030 2022 5322 2022 5349 502b 4432 5522  00 "S" "SIP+D2U"
-0000a550: 2022 2220 5f73 6970 2e5f 7564 702e 756e   "" _sip._udp.un
-0000a560: 6974 2e74 6573 7473 2e27 2c20 6b65 7929  it.tests.', key)
-0000a570: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
-0000a580: 7276 2873 656c 6629 3a0a 2020 2020 2020  rv(self):.      
-0000a590: 2020 7072 6f76 6964 6572 203d 2043 6c6f    provider = Clo
-0000a5a0: 7564 666c 6172 6550 726f 7669 6465 7228  udflareProvider(
-0000a5b0: 2774 6573 7427 2c20 2765 6d61 696c 272c  'test', 'email',
-0000a5c0: 2027 746f 6b65 6e27 290a 0a20 2020 2020   'token')..     
-0000a5d0: 2020 207a 6f6e 6520 3d20 5a6f 6e65 2827     zone = Zone('
-0000a5e0: 756e 6974 2e74 6573 7473 2e27 2c20 5b5d  unit.tests.', []
-0000a5f0: 290a 2020 2020 2020 2020 2320 5352 5620  ).        # SRV 
-0000a600: 7265 636f 7264 206e 6f74 2075 6e64 6572  record not under
-0000a610: 2061 2073 7562 2d64 6f6d 6169 6e0a 2020   a sub-domain.  
-0000a620: 2020 2020 2020 7372 765f 7265 636f 7264        srv_record
-0000a630: 203d 2052 6563 6f72 642e 6e65 7728 0a20   = Record.new(. 
-0000a640: 2020 2020 2020 2020 2020 207a 6f6e 652c             zone,
-0000a650: 0a20 2020 2020 2020 2020 2020 2027 5f65  .            '_e
-0000a660: 7861 6d70 6c65 2e5f 7463 7027 2c0a 2020  xample._tcp',.  
-0000a670: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-0000a680: 2020 2020 2020 2020 2020 2020 2774 746c              'ttl
-0000a690: 273a 2033 3030 2c0a 2020 2020 2020 2020  ': 300,.        
-0000a6a0: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
-0000a6b0: 2753 5256 272c 0a20 2020 2020 2020 2020  'SRV',.         
-0000a6c0: 2020 2020 2020 2027 7661 6c75 6527 3a20         'value': 
-0000a6d0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0000a6e0: 2020 2020 2020 2770 6f72 7427 3a20 3132        'port': 12
-0000a6f0: 3334 2c0a 2020 2020 2020 2020 2020 2020  34,.            
-0000a700: 2020 2020 2020 2020 2770 7269 6f72 6974          'priorit
-0000a710: 7927 3a20 302c 0a20 2020 2020 2020 2020  y': 0,.         
-0000a720: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
-0000a730: 6574 273a 2027 6e63 2e75 6e69 742e 7465  et': 'nc.unit.te
-0000a740: 7374 732e 272c 0a20 2020 2020 2020 2020  sts.',.         
-0000a750: 2020 2020 2020 2020 2020 2027 7765 6967             'weig
-0000a760: 6874 273a 2035 2c0a 2020 2020 2020 2020  ht': 5,.        
-0000a770: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-0000a780: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-0000a790: 2020 290a 2020 2020 2020 2020 2320 5352    ).        # SR
-0000a7a0: 5620 7265 636f 7264 2075 6e64 6572 2061  V record under a
-0000a7b0: 2073 7562 2d64 6f6d 6169 6e0a 2020 2020   sub-domain.    
-0000a7c0: 2020 2020 7372 765f 7265 636f 7264 5f77      srv_record_w
-0000a7d0: 6974 685f 7375 6220 3d20 5265 636f 7264  ith_sub = Record
-0000a7e0: 2e6e 6577 280a 2020 2020 2020 2020 2020  .new(.          
-0000a7f0: 2020 7a6f 6e65 2c0a 2020 2020 2020 2020    zone,.        
-0000a800: 2020 2020 275f 6578 616d 706c 652e 5f74      '_example._t
-0000a810: 6370 2e73 7562 272c 0a20 2020 2020 2020  cp.sub',.       
-0000a820: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-0000a830: 2020 2020 2020 2027 7474 6c27 3a20 3330         'ttl': 30
-0000a840: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0000a850: 2020 2027 7479 7065 273a 2027 5352 5627     'type': 'SRV'
-0000a860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a870: 2020 2776 616c 7565 273a 207b 0a20 2020    'value': {.   
-0000a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a890: 2027 706f 7274 273a 2031 3233 342c 0a20   'port': 1234,. 
-0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8b0: 2020 2027 7072 696f 7269 7479 273a 2030     'priority': 0
-0000a8c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a8d0: 2020 2020 2020 2774 6172 6765 7427 3a20        'target': 
-0000a8e0: 276e 632e 756e 6974 2e74 6573 7473 2e27  'nc.unit.tests.'
-0000a8f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a900: 2020 2020 2020 2777 6569 6768 7427 3a20        'weight': 
-0000a910: 352c 0a20 2020 2020 2020 2020 2020 2020  5,.             
-0000a920: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-0000a930: 2020 7d2c 0a20 2020 2020 2020 2029 0a0a    },.        )..
-0000a940: 2020 2020 2020 2020 7372 765f 7265 636f          srv_reco
-0000a950: 7264 5f63 6f6e 7465 6e74 7320 3d20 7072  rd_contents = pr
-0000a960: 6f76 6964 6572 2e5f 6765 6e5f 6461 7461  ovider._gen_data
-0000a970: 2873 7276 5f72 6563 6f72 6429 0a20 2020  (srv_record).   
-0000a980: 2020 2020 2073 7276 5f72 6563 6f72 645f       srv_record_
-0000a990: 7769 7468 5f73 7562 5f63 6f6e 7465 6e74  with_sub_content
-0000a9a0: 7320 3d20 7072 6f76 6964 6572 2e5f 6765  s = provider._ge
-0000a9b0: 6e5f 6461 7461 2873 7276 5f72 6563 6f72  n_data(srv_recor
-0000a9c0: 645f 7769 7468 5f73 7562 290a 2020 2020  d_with_sub).    
-0000a9d0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000a9e0: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
-0000a9f0: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
-0000aa00: 2020 2020 276e 616d 6527 3a20 275f 6578      'name': '_ex
-0000aa10: 616d 706c 652e 5f74 6370 2e75 6e69 742e  ample._tcp.unit.
-0000aa20: 7465 7374 7327 2c0a 2020 2020 2020 2020  tests',.        
-0000aa30: 2020 2020 2020 2020 2774 746c 273a 2033          'ttl': 3
-0000aa40: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-0000aa50: 2020 2020 2774 7970 6527 3a20 2753 5256      'type': 'SRV
-0000aa60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000aa70: 2020 2027 6461 7461 273a 207b 0a20 2020     'data': {.   
-0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aa90: 2027 7365 7276 6963 6527 3a20 275f 6578   'service': '_ex
-0000aaa0: 616d 706c 6527 2c0a 2020 2020 2020 2020  ample',.        
-0000aab0: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
-0000aac0: 746f 273a 2027 5f74 6370 272c 0a20 2020  to': '_tcp',.   
-0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aae0: 2027 6e61 6d65 273a 2027 756e 6974 2e74   'name': 'unit.t
-0000aaf0: 6573 7473 2e27 2c0a 2020 2020 2020 2020  ests.',.        
-0000ab00: 2020 2020 2020 2020 2020 2020 2770 7269              'pri
-0000ab10: 6f72 6974 7927 3a20 302c 0a20 2020 2020  ority': 0,.     
-0000ab20: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000ab30: 7765 6967 6874 273a 2035 2c0a 2020 2020  weight': 5,.    
-0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab50: 2770 6f72 7427 3a20 3132 3334 2c0a 2020  'port': 1234,.  
-0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab70: 2020 2774 6172 6765 7427 3a20 276e 632e    'target': 'nc.
-0000ab80: 756e 6974 2e74 6573 7473 272c 0a20 2020  unit.tests',.   
-0000ab90: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-0000aba0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-0000abb0: 2020 2020 2020 2020 2020 206c 6973 7428             list(
-0000abc0: 7372 765f 7265 636f 7264 5f63 6f6e 7465  srv_record_conte
-0000abd0: 6e74 7329 5b30 5d2c 0a20 2020 2020 2020  nts)[0],.       
-0000abe0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-0000abf0: 6173 7365 7274 4571 7561 6c28 0a20 2020  assertEqual(.   
-0000ac00: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-0000ac10: 2020 2020 2020 2020 2020 2027 6e61 6d65             'name
-0000ac20: 273a 2027 5f65 7861 6d70 6c65 2e5f 7463  ': '_example._tc
-0000ac30: 702e 7375 622e 756e 6974 2e74 6573 7473  p.sub.unit.tests
-0000ac40: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000ac50: 2020 2027 7474 6c27 3a20 3330 302c 0a20     'ttl': 300,. 
-0000ac60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000ac70: 7479 7065 273a 2027 5352 5627 2c0a 2020  type': 'SRV',.  
-0000ac80: 2020 2020 2020 2020 2020 2020 2020 2764                'd
-0000ac90: 6174 6127 3a20 7b0a 2020 2020 2020 2020  ata': {.        
-0000aca0: 2020 2020 2020 2020 2020 2020 2773 6572              'ser
-0000acb0: 7669 6365 273a 2027 5f65 7861 6d70 6c65  vice': '_example
-0000acc0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000acd0: 2020 2020 2020 2027 7072 6f74 6f27 3a20         'proto': 
-0000ace0: 275f 7463 7027 2c0a 2020 2020 2020 2020  '_tcp',.        
-0000acf0: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
-0000ad00: 6527 3a20 2773 7562 272c 0a20 2020 2020  e': 'sub',.     
-0000ad10: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000ad20: 7072 696f 7269 7479 273a 2030 2c0a 2020  priority': 0,.  
-0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad40: 2020 2777 6569 6768 7427 3a20 352c 0a20    'weight': 5,. 
-0000ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad60: 2020 2027 706f 7274 273a 2031 3233 342c     'port': 1234,
-0000ad70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ad80: 2020 2020 2027 7461 7267 6574 273a 2027       'target': '
-0000ad90: 6e63 2e75 6e69 742e 7465 7374 7327 2c0a  nc.unit.tests',.
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 7d2c 0a20 2020 2020 2020 2020 2020 207d  },.            }
-0000adc0: 2c0a 2020 2020 2020 2020 2020 2020 6c69  ,.            li
-0000add0: 7374 2873 7276 5f72 6563 6f72 645f 7769  st(srv_record_wi
-0000ade0: 7468 5f73 7562 5f63 6f6e 7465 6e74 7329  th_sub_contents)
-0000adf0: 5b30 5d2c 0a20 2020 2020 2020 2029 0a0a  [0],.        )..
-0000ae00: 2020 2020 6465 6620 7465 7374 5f74 7874      def test_txt
-0000ae10: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000ae20: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
-0000ae30: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
-0000ae40: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
-0000ae50: 746f 6b65 6e27 290a 0a20 2020 2020 2020  token')..       
-0000ae60: 2023 2073 696e 676c 6520 7265 636f 7264   # single record
-0000ae70: 2077 2f63 6f6e 7465 6e74 0a20 2020 2020   w/content.     
-0000ae80: 2020 2064 6174 6120 3d20 7072 6f76 6964     data = provid
-0000ae90: 6572 2e5f 6461 7461 5f66 6f72 5f54 5854  er._data_for_TXT
-0000aea0: 280a 2020 2020 2020 2020 2020 2020 2754  (.            'T
-0000aeb0: 5854 272c 205b 7b27 7474 6c27 3a20 3432  XT', [{'ttl': 42
-0000aec0: 2c20 2763 6f6e 7465 6e74 273a 2027 6865  , 'content': 'he
-0000aed0: 6c6c 6f20 776f 726c 6427 7d5d 0a20 2020  llo world'}].   
-0000aee0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
-0000aef0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000af00: 0a20 2020 2020 2020 2020 2020 207b 2774  .            {'t
-0000af10: 746c 273a 2034 322c 2027 7479 7065 273a  tl': 42, 'type':
-0000af20: 2027 5458 5427 2c20 2776 616c 7565 7327   'TXT', 'values'
-0000af30: 3a20 5b27 6865 6c6c 6f20 776f 726c 6427  : ['hello world'
-0000af40: 5d7d 2c20 6461 7461 0a20 2020 2020 2020  ]}, data.       
-0000af50: 2029 0a0a 2020 2020 2020 2020 2320 6d69   )..        # mi
-0000af60: 7373 696e 6720 636f 6e74 656e 742c 2065  ssing content, e
-0000af70: 7175 6976 696c 656e 7420 746f 2065 6d70  quivilent to emp
-0000af80: 7479 2066 726f 6d20 4346 0a20 2020 2020  ty from CF.     
-0000af90: 2020 2064 6174 6120 3d20 7072 6f76 6964     data = provid
-0000afa0: 6572 2e5f 6461 7461 5f66 6f72 5f54 5854  er._data_for_TXT
-0000afb0: 2827 5458 5427 2c20 5b7b 2774 746c 273a  ('TXT', [{'ttl':
-0000afc0: 2034 327d 5d29 0a20 2020 2020 2020 2066   42}]).        f
-0000afd0: 726f 6d20 7070 7269 6e74 2069 6d70 6f72  rom pprint impor
-0000afe0: 7420 7070 7269 6e74 0a0a 2020 2020 2020  t pprint..      
-0000aff0: 2020 7070 7269 6e74 2864 6174 6129 0a0a    pprint(data)..
-0000b000: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
-0000b010: 6572 7445 7175 616c 287b 2774 746c 273a  ertEqual({'ttl':
-0000b020: 2034 322c 2027 7479 7065 273a 2027 5458   42, 'type': 'TX
-0000b030: 5427 2c20 2776 616c 7565 7327 3a20 5b27  T', 'values': ['
-0000b040: 275d 7d2c 2064 6174 6129 0a0a 2020 2020  ']}, data)..    
-0000b050: 6465 6620 7465 7374 5f61 6c69 6173 2873  def test_alias(s
-0000b060: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-0000b070: 6f76 6964 6572 203d 2043 6c6f 7564 666c  ovider = Cloudfl
-0000b080: 6172 6550 726f 7669 6465 7228 2774 6573  areProvider('tes
-0000b090: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
-0000b0a0: 6b65 6e27 290a 0a20 2020 2020 2020 2023  ken')..        #
-0000b0b0: 2041 2043 4e41 4d45 2066 6f72 2075 7320   A CNAME for us 
-0000b0c0: 746f 2074 7261 6e73 666f 726d 2074 6f20  to transform to 
-0000b0d0: 414c 4941 530a 2020 2020 2020 2020 7072  ALIAS.        pr
-0000b0e0: 6f76 6964 6572 2e7a 6f6e 655f 7265 636f  ovider.zone_reco
-0000b0f0: 7264 7320 3d20 4d6f 636b 280a 2020 2020  rds = Mock(.    
-0000b100: 2020 2020 2020 2020 7265 7475 726e 5f76          return_v
-0000b110: 616c 7565 3d5b 0a20 2020 2020 2020 2020  alue=[.         
-0000b120: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-0000b130: 2020 2020 2020 2020 2020 2020 2022 6964               "id
-0000b140: 223a 2022 6663 3132 6162 3334 6364 3536  ": "fc12ab34cd56
-0000b150: 3131 3333 3434 3232 6162 3333 3232 3939  11334422ab332299
-0000b160: 3736 3432 222c 0a20 2020 2020 2020 2020  7642",.         
-0000b170: 2020 2020 2020 2020 2020 2022 7479 7065             "type
-0000b180: 223a 2022 434e 414d 4522 2c0a 2020 2020  ": "CNAME",.    
-0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1a0: 226e 616d 6522 3a20 2275 6e69 742e 7465  "name": "unit.te
-0000b1b0: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
-0000b1c0: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
-0000b1d0: 6e74 223a 2022 7777 772e 756e 6974 2e74  nt": "www.unit.t
-0000b1e0: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
-0000b1f0: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
-0000b200: 6961 626c 6522 3a20 5472 7565 2c0a 2020  iable": True,.  
-0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b220: 2020 2270 726f 7869 6564 223a 2046 616c    "proxied": Fal
-0000b230: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0000b240: 2020 2020 2020 2020 2274 746c 223a 2033          "ttl": 3
-0000b250: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
-0000b260: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
-0000b270: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-0000b280: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
-0000b290: 6e65 5f69 6422 3a20 2266 6631 3261 6233  ne_id": "ff12ab3
-0000b2a0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
-0000b2b0: 3332 3239 3937 3635 3022 2c0a 2020 2020  322997650",.    
+00009010: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009030: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00009040: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00009050: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009060: 2020 2020 2020 2020 2020 2270 7269 6f72            "prior
+00009070: 6974 7922 3a20 312c 0a20 2020 2020 2020  ity": 1,.       
+00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009090: 2022 7374 6174 7573 223a 2022 6163 7469   "status": "acti
+000090a0: 7665 222c 0a20 2020 2020 2020 2020 2020  ve",.           
+000090b0: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+000090c0: 6561 7465 645f 6f6e 223a 2022 3230 3231  eated_on": "2021
+000090d0: 2d30 362d 3235 5432 303a 3130 3a35 302e  -06-25T20:10:50.
+000090e0: 3030 3030 3030 5a22 2c0a 2020 2020 2020  000000Z",.      
+000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009100: 2020 226d 6f64 6966 6965 645f 6f6e 223a    "modified_on":
+00009110: 2022 3230 3231 2d30 362d 3238 5432 323a   "2021-06-28T22:
+00009120: 3338 3a31 302e 3030 3030 3030 5a22 2c0a  38:10.000000Z",.
+00009130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009140: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00009150: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
+00009160: 2020 2020 2020 2020 2027 7265 7375 6c74           'result
+00009170: 5f69 6e66 6f27 3a20 7b27 636f 756e 7427  _info': {'count'
+00009180: 3a20 312c 2027 7065 725f 7061 6765 273a  : 1, 'per_page':
+00009190: 2035 307d 2c0a 2020 2020 2020 2020 2020   50},.          
+000091a0: 2020 2020 2020 2320 2f7a 6f6e 6573 2f34        # /zones/4
+000091b0: 322f 7061 6765 7275 6c65 730a 2020 2020  2/pagerules.    
+000091c0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+000091d0: 2020 205d 0a20 2020 2020 2020 2070 726f     ].        pro
+000091e0: 7669 6465 722e 5f72 6571 7565 7374 2e73  vider._request.s
+000091f0: 6964 655f 6566 6665 6374 203d 2073 6964  ide_effect = sid
+00009200: 655f 6566 6665 6374 0a0a 2020 2020 2020  e_effect..      
+00009210: 2020 2320 4e6f 7720 7765 2070 6f70 756c    # Now we popul
+00009220: 6174 652c 2061 6e64 2065 7870 6563 7420  ate, and expect 
+00009230: 746f 2073 6565 206e 6f74 6869 6e67 0a20  to see nothing. 
+00009240: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00009250: 7274 4661 6c73 6528 7072 6f76 6964 6572  rtFalse(provider
+00009260: 2e70 6c61 6e28 7a6f 6e65 2929 0a20 2020  .plan(zone)).   
+00009270: 2020 2020 2023 2057 6520 7368 6f75 6c64       # We should
+00009280: 2068 6176 6520 6861 6420 6f6e 6c79 2061   have had only a
+00009290: 2073 696e 676c 6520 6361 6c6c 2074 6f20   single call to 
+000092a0: 6765 7420 7468 6520 646e 735f 7265 636f  get the dns_reco
+000092b0: 7264 732c 206e 6f0a 2020 2020 2020 2020  rds, no.        
+000092c0: 2320 6361 6c6c 7320 746f 2070 6167 6572  # calls to pager
+000092d0: 756c 6573 0a20 2020 2020 2020 2070 726f  ules.        pro
+000092e0: 7669 6465 722e 5f72 6571 7565 7374 2e61  vider._request.a
+000092f0: 7373 6572 745f 6361 6c6c 6564 5f6f 6e63  ssert_called_onc
+00009300: 6528 290a 0a20 2020 2020 2020 2023 2072  e()..        # r
+00009310: 6573 6574 2074 6869 6e67 730a 2020 2020  eset things.    
+00009320: 2020 2020 7072 6f76 6964 6572 2e5f 7a6f      provider._zo
+00009330: 6e65 5f72 6563 6f72 6473 203d 207b 7d0a  ne_records = {}.
+00009340: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00009350: 2e53 5550 504f 5254 532e 6164 6428 2755  .SUPPORTS.add('U
+00009360: 524c 4657 4427 290a 2020 2020 2020 2020  RLFWD').        
+00009370: 7072 6f76 6964 6572 2e5f 7265 7175 6573  provider._reques
+00009380: 742e 7369 6465 5f65 6666 6563 7420 3d20  t.side_effect = 
+00009390: 7369 6465 5f65 6666 6563 740a 2020 2020  side_effect.    
+000093a0: 2020 2020 2320 656e 6162 6c65 2070 6167      # enable pag
+000093b0: 6572 756c 6573 0a20 2020 2020 2020 2070  erules.        p
+000093c0: 726f 7669 6465 722e 7061 6765 7275 6c65  rovider.pagerule
+000093d0: 7320 3d20 5472 7565 0a20 2020 2020 2020  s = True.       
+000093e0: 2023 2070 6c61 6e20 6167 6169 6e2c 2074   # plan again, t
+000093f0: 6869 7320 7469 6d65 2077 6520 6578 7065  his time we expe
+00009400: 6374 2062 6f74 6820 6361 6c6c 7320 616e  ct both calls an
+00009410: 6420 6120 7265 636f 7264 0a20 2020 2020  d a record.     
+00009420: 2020 2070 6c61 6e20 3d20 7072 6f76 6964     plan = provid
+00009430: 6572 2e70 6c61 6e28 7a6f 6e65 290a 2020  er.plan(zone).  
+00009440: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00009450: 7445 7175 616c 2831 2c20 6c65 6e28 706c  tEqual(1, len(pl
+00009460: 616e 2e63 6861 6e67 6573 2929 0a20 2020  an.changes)).   
+00009470: 2020 2020 2063 6861 6e67 6520 3d20 6c69       change = li
+00009480: 7374 2870 6c61 6e2e 6368 616e 6765 7329  st(plan.changes)
+00009490: 5b30 5d0a 2020 2020 2020 2020 7365 6c66  [0].        self
+000094a0: 2e61 7373 6572 7445 7175 616c 2827 5552  .assertEqual('UR
+000094b0: 4c46 5744 272c 2063 6861 6e67 652e 7265  LFWD', change.re
+000094c0: 636f 7264 2e5f 7479 7065 290a 2020 2020  cord._type).    
+000094d0: 2020 2020 7072 6f76 6964 6572 2e5f 7265      provider._re
+000094e0: 7175 6573 742e 6173 7365 7274 5f68 6173  quest.assert_has
+000094f0: 5f63 616c 6c73 280a 2020 2020 2020 2020  _calls(.        
+00009500: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
+00009510: 2020 2020 2020 6361 6c6c 280a 2020 2020        call(.    
+00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009530: 2747 4554 272c 0a20 2020 2020 2020 2020  'GET',.         
+00009540: 2020 2020 2020 2020 2020 2027 2f7a 6f6e             '/zon
+00009550: 6573 2f34 322f 646e 735f 7265 636f 7264  es/42/dns_record
+00009560: 7327 2c0a 2020 2020 2020 2020 2020 2020  s',.            
+00009570: 2020 2020 2020 2020 7061 7261 6d73 3d7b          params={
+00009580: 2770 6167 6527 3a20 312c 2027 7065 725f  'page': 1, 'per_
+00009590: 7061 6765 273a 2031 3030 7d2c 0a20 2020  page': 100},.   
+000095a0: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 6361 6c6c 2827 4745 5427 2c20 272f 7a6f  call('GET', '/zo
+000095d0: 6e65 732f 3432 2f70 6167 6572 756c 6573  nes/42/pagerules
+000095e0: 272c 2070 6172 616d 733d 7b27 7374 6174  ', params={'stat
+000095f0: 7573 273a 2027 6163 7469 7665 277d 292c  us': 'active'}),
+00009600: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
+00009610: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00009620: 6620 7465 7374 5f70 7472 2873 656c 6629  f test_ptr(self)
+00009630: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
+00009640: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
+00009650: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
+00009660: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
+00009670: 290a 0a20 2020 2020 2020 207a 6f6e 6520  )..        zone 
+00009680: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
+00009690: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
+000096a0: 2020 2320 5054 5220 7265 636f 7264 0a20    # PTR record. 
+000096b0: 2020 2020 2020 2070 7472 5f72 6563 6f72         ptr_recor
+000096c0: 6420 3d20 5265 636f 7264 2e6e 6577 280a  d = Record.new(.
+000096d0: 2020 2020 2020 2020 2020 2020 7a6f 6e65              zone
+000096e0: 2c20 2770 7472 272c 207b 2774 746c 273a  , 'ptr', {'ttl':
+000096f0: 2033 3030 2c20 2774 7970 6527 3a20 2750   300, 'type': 'P
+00009700: 5452 272c 2027 7661 6c75 6527 3a20 2766  TR', 'value': 'f
+00009710: 6f6f 2e62 6172 2e63 6f6d 2e27 7d0a 2020  oo.bar.com.'}.  
+00009720: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00009730: 2070 7472 5f72 6563 6f72 645f 636f 6e74   ptr_record_cont
+00009740: 656e 7473 203d 2070 726f 7669 6465 722e  ents = provider.
+00009750: 5f67 656e 5f64 6174 6128 7074 725f 7265  _gen_data(ptr_re
+00009760: 636f 7264 290a 2020 2020 2020 2020 7365  cord).        se
+00009770: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+00009780: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00009790: 2020 2020 2020 2020 2020 2020 2020 276e                'n
+000097a0: 616d 6527 3a20 2770 7472 2e75 6e69 742e  ame': 'ptr.unit.
+000097b0: 7465 7374 7327 2c0a 2020 2020 2020 2020  tests',.        
+000097c0: 2020 2020 2020 2020 2774 746c 273a 2033          'ttl': 3
+000097d0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+000097e0: 2020 2020 2774 7970 6527 3a20 2750 5452      'type': 'PTR
+000097f0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00009800: 2020 2027 636f 6e74 656e 7427 3a20 2766     'content': 'f
+00009810: 6f6f 2e62 6172 2e63 6f6d 2e27 2c0a 2020  oo.bar.com.',.  
+00009820: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00009830: 2020 2020 2020 2020 206c 6973 7428 7074           list(pt
+00009840: 725f 7265 636f 7264 5f63 6f6e 7465 6e74  r_record_content
+00009850: 7329 5b30 5d2c 0a20 2020 2020 2020 2029  s)[0],.        )
+00009860: 0a0a 2020 2020 6465 6620 7465 7374 5f6c  ..    def test_l
+00009870: 6f63 2873 656c 6629 3a0a 2020 2020 2020  oc(self):.      
+00009880: 2020 7365 6c66 2e6d 6178 4469 6666 203d    self.maxDiff =
+00009890: 204e 6f6e 650a 2020 2020 2020 2020 7072   None.        pr
+000098a0: 6f76 6964 6572 203d 2043 6c6f 7564 666c  ovider = Cloudfl
+000098b0: 6172 6550 726f 7669 6465 7228 2774 6573  areProvider('tes
+000098c0: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
+000098d0: 6b65 6e27 290a 0a20 2020 2020 2020 207a  ken')..        z
+000098e0: 6f6e 6520 3d20 5a6f 6e65 2827 756e 6974  one = Zone('unit
+000098f0: 2e74 6573 7473 2e27 2c20 5b5d 290a 2020  .tests.', []).  
+00009900: 2020 2020 2020 2320 4c4f 4320 7265 636f        # LOC reco
+00009910: 7264 0a20 2020 2020 2020 206c 6f63 5f72  rd.        loc_r
+00009920: 6563 6f72 6420 3d20 5265 636f 7264 2e6e  ecord = Record.n
+00009930: 6577 280a 2020 2020 2020 2020 2020 2020  ew(.            
+00009940: 7a6f 6e65 2c0a 2020 2020 2020 2020 2020  zone,.          
+00009950: 2020 2765 7861 6d70 6c65 272c 0a20 2020    'example',.   
+00009960: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00009970: 2020 2020 2020 2020 2020 2027 7474 6c27             'ttl'
+00009980: 3a20 3330 302c 0a20 2020 2020 2020 2020  : 300,.         
+00009990: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
+000099a0: 4c4f 4327 2c0a 2020 2020 2020 2020 2020  LOC',.          
+000099b0: 2020 2020 2020 2776 616c 7565 273a 207b        'value': {
+000099c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000099d0: 2020 2020 2027 6c61 745f 6465 6772 6565       'lat_degree
+000099e0: 7327 3a20 3331 2c0a 2020 2020 2020 2020  s': 31,.        
+000099f0: 2020 2020 2020 2020 2020 2020 276c 6174              'lat
+00009a00: 5f6d 696e 7574 6573 273a 2035 382c 0a20  _minutes': 58,. 
+00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a20: 2020 2027 6c61 745f 7365 636f 6e64 7327     'lat_seconds'
+00009a30: 3a20 3532 2e31 2c0a 2020 2020 2020 2020  : 52.1,.        
+00009a40: 2020 2020 2020 2020 2020 2020 276c 6174              'lat
+00009a50: 5f64 6972 6563 7469 6f6e 273a 2027 5327  _direction': 'S'
+00009a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009a70: 2020 2020 2020 276c 6f6e 675f 6465 6772        'long_degr
+00009a80: 6565 7327 3a20 3131 352c 0a20 2020 2020  ees': 115,.     
+00009a90: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009aa0: 6c6f 6e67 5f6d 696e 7574 6573 273a 2034  long_minutes': 4
+00009ab0: 392c 0a20 2020 2020 2020 2020 2020 2020  9,.             
+00009ac0: 2020 2020 2020 2027 6c6f 6e67 5f73 6563         'long_sec
+00009ad0: 6f6e 6473 273a 2031 312e 372c 0a20 2020  onds': 11.7,.   
+00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009af0: 2027 6c6f 6e67 5f64 6972 6563 7469 6f6e   'long_direction
+00009b00: 273a 2027 4527 2c0a 2020 2020 2020 2020  ': 'E',.        
+00009b10: 2020 2020 2020 2020 2020 2020 2761 6c74              'alt
+00009b20: 6974 7564 6527 3a20 3230 2c0a 2020 2020  itude': 20,.    
+00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b40: 2773 697a 6527 3a20 3130 2c0a 2020 2020  'size': 10,.    
+00009b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b60: 2770 7265 6369 7369 6f6e 5f68 6f72 7a27  'precision_horz'
+00009b70: 3a20 3130 2c0a 2020 2020 2020 2020 2020  : 10,.          
+00009b80: 2020 2020 2020 2020 2020 2770 7265 6369            'preci
+00009b90: 7369 6f6e 5f76 6572 7427 3a20 322c 0a20  sion_vert': 2,. 
+00009ba0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00009bb0: 2c0a 2020 2020 2020 2020 2020 2020 7d2c  ,.            },
+00009bc0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00009bd0: 2020 2020 6c6f 635f 7265 636f 7264 5f63      loc_record_c
+00009be0: 6f6e 7465 6e74 7320 3d20 7072 6f76 6964  ontents = provid
+00009bf0: 6572 2e5f 6765 6e5f 6461 7461 286c 6f63  er._gen_data(loc
+00009c00: 5f72 6563 6f72 6429 0a20 2020 2020 2020  _record).       
+00009c10: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00009c20: 6c28 0a20 2020 2020 2020 2020 2020 207b  l(.            {
+00009c30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c40: 2027 6e61 6d65 273a 2027 6578 616d 706c   'name': 'exampl
+00009c50: 652e 756e 6974 2e74 6573 7473 272c 0a20  e.unit.tests',. 
+00009c60: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009c70: 7474 6c27 3a20 3330 302c 0a20 2020 2020  ttl': 300,.     
+00009c80: 2020 2020 2020 2020 2020 2027 7479 7065             'type
+00009c90: 273a 2027 4c4f 4327 2c0a 2020 2020 2020  ': 'LOC',.      
+00009ca0: 2020 2020 2020 2020 2020 2764 6174 6127            'data'
+00009cb0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
+00009cc0: 2020 2020 2020 2020 276c 6174 5f64 6567          'lat_deg
+00009cd0: 7265 6573 273a 2033 312c 0a20 2020 2020  rees': 31,.     
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009cf0: 6c61 745f 6d69 6e75 7465 7327 3a20 3538  lat_minutes': 58
+00009d00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009d10: 2020 2020 2020 276c 6174 5f73 6563 6f6e        'lat_secon
+00009d20: 6473 273a 2035 322e 312c 0a20 2020 2020  ds': 52.1,.     
+00009d30: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009d40: 6c61 745f 6469 7265 6374 696f 6e27 3a20  lat_direction': 
+00009d50: 2753 272c 0a20 2020 2020 2020 2020 2020  'S',.           
+00009d60: 2020 2020 2020 2020 2027 6c6f 6e67 5f64           'long_d
+00009d70: 6567 7265 6573 273a 2031 3135 2c0a 2020  egrees': 115,.  
+00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d90: 2020 276c 6f6e 675f 6d69 6e75 7465 7327    'long_minutes'
+00009da0: 3a20 3439 2c0a 2020 2020 2020 2020 2020  : 49,.          
+00009db0: 2020 2020 2020 2020 2020 276c 6f6e 675f            'long_
+00009dc0: 7365 636f 6e64 7327 3a20 3131 2e37 2c0a  seconds': 11.7,.
+00009dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009de0: 2020 2020 276c 6f6e 675f 6469 7265 6374      'long_direct
+00009df0: 696f 6e27 3a20 2745 272c 0a20 2020 2020  ion': 'E',.     
+00009e00: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00009e10: 616c 7469 7475 6465 273a 2032 302c 0a20  altitude': 20,. 
+00009e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e30: 2020 2027 7369 7a65 273a 2031 302c 0a20     'size': 10,. 
+00009e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e50: 2020 2027 7072 6563 6973 696f 6e5f 686f     'precision_ho
+00009e60: 727a 273a 2031 302c 0a20 2020 2020 2020  rz': 10,.       
+00009e70: 2020 2020 2020 2020 2020 2020 2027 7072               'pr
+00009e80: 6563 6973 696f 6e5f 7665 7274 273a 2032  ecision_vert': 2
+00009e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009ea0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00009eb0: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+00009ec0: 6c69 7374 286c 6f63 5f72 6563 6f72 645f  list(loc_record_
+00009ed0: 636f 6e74 656e 7473 295b 305d 2c0a 2020  contents)[0],.  
+00009ee0: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00009ef0: 2074 6573 745f 6e61 7074 7228 7365 6c66   test_naptr(self
+00009f00: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
+00009f10: 6d61 7844 6966 6620 3d20 4e6f 6e65 0a20  maxDiff = None. 
+00009f20: 2020 2020 2020 2070 726f 7669 6465 7220         provider 
+00009f30: 3d20 436c 6f75 6466 6c61 7265 5072 6f76  = CloudflareProv
+00009f40: 6964 6572 2827 7465 7374 272c 2027 656d  ider('test', 'em
+00009f50: 6169 6c27 2c20 2774 6f6b 656e 2729 0a0a  ail', 'token')..
+00009f60: 2020 2020 2020 2020 6366 5f64 6174 6120          cf_data 
+00009f70: 3d20 7b0a 2020 2020 2020 2020 2020 2020  = {.            
+00009f80: 2763 6f6d 6d65 6e74 273a 204e 6f6e 652c  'comment': None,
+00009f90: 0a20 2020 2020 2020 2020 2020 2027 636f  .            'co
+00009fa0: 6e74 656e 7427 3a20 2732 3020 3130 3020  ntent': '20 100 
+00009fb0: 2253 2220 2253 4950 2b44 3255 2220 2222  "S" "SIP+D2U" ""
+00009fc0: 205f 7369 702e 5f75 6470 2e75 6e69 742e   _sip._udp.unit.
+00009fd0: 7465 7374 732e 272c 0a20 2020 2020 2020  tests.',.       
+00009fe0: 2020 2020 2027 6372 6561 7465 645f 6f6e       'created_on
+00009ff0: 273a 2027 3230 3233 2d30 312d 3038 5430  ': '2023-01-08T0
+0000a000: 313a 3032 3a33 342e 3536 3739 3835 5a27  1:02:34.567985Z'
+0000a010: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
+0000a020: 6174 6127 3a20 7b0a 2020 2020 2020 2020  ata': {.        
+0000a030: 2020 2020 2020 2020 2766 6c61 6773 273a          'flags':
+0000a040: 2027 5327 2c0a 2020 2020 2020 2020 2020   'S',.          
+0000a050: 2020 2020 2020 276f 7264 6572 273a 2032        'order': 2
+0000a060: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+0000a070: 2020 2027 7072 6566 6572 656e 6365 273a     'preference':
+0000a080: 2031 3030 2c0a 2020 2020 2020 2020 2020   100,.          
+0000a090: 2020 2020 2020 2772 6567 6578 273a 2027        'regex': '
+0000a0a0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000a0b0: 2020 2027 7265 706c 6163 656d 656e 7427     'replacement'
+0000a0c0: 3a20 275f 7369 702e 5f75 6470 2e75 6e69  : '_sip._udp.uni
+0000a0d0: 742e 7465 7374 732e 272c 0a20 2020 2020  t.tests.',.     
+0000a0e0: 2020 2020 2020 2020 2020 2027 7365 7276             'serv
+0000a0f0: 6963 6527 3a20 2753 4950 2b44 3255 272c  ice': 'SIP+D2U',
+0000a100: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+0000a110: 2020 2020 2020 2020 2020 2020 2769 6427              'id'
+0000a120: 3a20 2738 6236 3063 3835 3138 6430 3934  : '8b60c8518d094
+0000a130: 3635 6666 6337 3734 3162 3761 3461 3433  65ffc7741b7a4a43
+0000a140: 3166 3938 272c 0a20 2020 2020 2020 2020  1f98',.         
+0000a150: 2020 2027 6c6f 636b 6564 273a 2046 616c     'locked': Fal
+0000a160: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+0000a170: 276d 6574 6127 3a20 7b0a 2020 2020 2020  'meta': {.      
+0000a180: 2020 2020 2020 2020 2020 2761 7574 6f5f            'auto_
+0000a190: 6164 6465 6427 3a20 4661 6c73 652c 0a20  added': False,. 
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000a1b0: 6d61 6e61 6765 645f 6279 5f61 7070 7327  managed_by_apps'
+0000a1c0: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+0000a1d0: 2020 2020 2020 2020 2027 6d61 6e61 6765           'manage
+0000a1e0: 645f 6279 5f61 7267 6f5f 7475 6e6e 656c  d_by_argo_tunnel
+0000a1f0: 273a 2046 616c 7365 2c0a 2020 2020 2020  ': False,.      
+0000a200: 2020 2020 2020 2020 2020 2773 6f75 7263            'sourc
+0000a210: 6527 3a20 2770 7269 6d61 7279 272c 0a20  e': 'primary',. 
+0000a220: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
+0000a230: 2020 2020 2020 2020 2020 276d 6f64 6966            'modif
+0000a240: 6965 645f 6f6e 273a 2027 3230 3233 2d30  ied_on': '2023-0
+0000a250: 312d 3038 5430 313a 3032 3a33 342e 3536  1-08T01:02:34.56
+0000a260: 3739 3835 5a27 2c0a 2020 2020 2020 2020  7985Z',.        
+0000a270: 2020 2020 276e 616d 6527 3a20 276e 6170      'name': 'nap
+0000a280: 7472 2e75 6e69 742e 7465 7374 7327 2c0a  tr.unit.tests',.
+0000a290: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
+0000a2a0: 7869 6162 6c65 273a 2046 616c 7365 2c0a  xiable': False,.
+0000a2b0: 2020 2020 2020 2020 2020 2020 2770 726f              'pro
+0000a2c0: 7869 6564 273a 2046 616c 7365 2c0a 2020  xied': False,.  
+0000a2d0: 2020 2020 2020 2020 2020 2774 6167 7327            'tags'
+0000a2e0: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+0000a2f0: 2020 2774 746c 273a 2031 2c0a 2020 2020    'ttl': 1,.    
+0000a300: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
+0000a310: 274e 4150 5452 272c 0a20 2020 2020 2020  'NAPTR',.       
+0000a320: 2020 2020 2027 7a6f 6e65 5f69 6427 3a20       'zone_id': 
+0000a330: 2764 3531 3564 6566 6534 3162 3137 3362  'd515defe41b173b
+0000a340: 6565 3934 3838 6439 6134 6235 6635 6465  ee9488d9a4b5f5de
+0000a350: 3966 272c 0a20 2020 2020 2020 2020 2020  9f',.           
+0000a360: 2027 7a6f 6e65 5f6e 616d 6527 3a20 2775   'zone_name': 'u
+0000a370: 6e69 742e 7465 7374 7327 2c0a 2020 2020  nit.tests',.    
+0000a380: 2020 2020 7d0a 2020 2020 2020 2020 6461      }.        da
+0000a390: 7461 203d 2070 726f 7669 6465 722e 5f64  ta = provider._d
+0000a3a0: 6174 615f 666f 725f 4e41 5054 5228 274e  ata_for_NAPTR('N
+0000a3b0: 4150 5452 272c 205b 6366 5f64 6174 615d  APTR', [cf_data]
+0000a3c0: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000a3d0: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+0000a3e0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+0000a3f0: 2020 2020 2020 2020 2020 2774 746c 273a            'ttl':
+0000a400: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
+0000a410: 2020 2020 2020 2774 7970 6527 3a20 274e        'type': 'N
+0000a420: 4150 5452 272c 0a20 2020 2020 2020 2020  APTR',.         
+0000a430: 2020 2020 2020 2027 7661 6c75 6573 273a         'values':
+0000a440: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0000a450: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000a460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a470: 2027 666c 6167 7327 3a20 2753 272c 0a20   'flags': 'S',. 
+0000a480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a490: 2020 2020 2020 2027 6f72 6465 7227 3a20         'order': 
+0000a4a0: 3230 2c0a 2020 2020 2020 2020 2020 2020  20,.            
+0000a4b0: 2020 2020 2020 2020 2020 2020 2770 7265              'pre
+0000a4c0: 6665 7265 6e63 6527 3a20 3130 302c 0a20  ference': 100,. 
+0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4e0: 2020 2020 2020 2027 7265 6765 7870 273a         'regexp':
+0000a4f0: 2027 272c 0a20 2020 2020 2020 2020 2020   '',.           
+0000a500: 2020 2020 2020 2020 2020 2020 2027 7265               're
+0000a510: 706c 6163 656d 656e 7427 3a20 275f 7369  placement': '_si
+0000a520: 702e 5f75 6470 2e75 6e69 742e 7465 7374  p._udp.unit.test
+0000a530: 732e 272c 0a20 2020 2020 2020 2020 2020  s.',.           
+0000a540: 2020 2020 2020 2020 2020 2020 2027 7365               'se
+0000a550: 7276 6963 6527 3a20 2753 4950 2b44 3255  rvice': 'SIP+D2U
+0000a560: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000a570: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0000a580: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+0000a590: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+0000a5a0: 2020 2020 2020 2064 6174 612c 0a20 2020         data,.   
+0000a5b0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000a5c0: 7a6f 6e65 203d 205a 6f6e 6528 2775 6e69  zone = Zone('uni
+0000a5d0: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
+0000a5e0: 2020 2020 2020 2072 6563 6f72 6420 3d20         record = 
+0000a5f0: 5265 636f 7264 2e6e 6577 287a 6f6e 652c  Record.new(zone,
+0000a600: 2027 6e61 7074 7227 2c20 6461 7461 290a   'naptr', data).
+0000a610: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
+0000a620: 203d 206c 6973 7428 7072 6f76 6964 6572   = list(provider
+0000a630: 2e5f 636f 6e74 656e 7473 5f66 6f72 5f4e  ._contents_for_N
+0000a640: 4150 5452 2872 6563 6f72 6429 290a 2020  APTR(record)).  
+0000a650: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000a660: 7445 7175 616c 285b 7b27 6461 7461 273a  tEqual([{'data':
+0000a670: 2063 665f 6461 7461 5b27 6461 7461 275d   cf_data['data']
+0000a680: 7d5d 2c20 636f 6e74 656e 7473 290a 0a20  }], contents).. 
+0000a690: 2020 2020 2020 206b 6579 203d 2070 726f         key = pro
+0000a6a0: 7669 6465 722e 5f67 656e 5f6b 6579 2863  vider._gen_key(c
+0000a6b0: 665f 6461 7461 290a 2020 2020 2020 2020  f_data).        
+0000a6c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+0000a6d0: 2827 3230 2031 3030 2022 5322 2022 5349  ('20 100 "S" "SI
+0000a6e0: 502b 4432 5522 2022 2220 5f73 6970 2e5f  P+D2U" "" _sip._
+0000a6f0: 7564 702e 756e 6974 2e74 6573 7473 2e27  udp.unit.tests.'
+0000a700: 2c20 6b65 7929 0a0a 2020 2020 6465 6620  , key)..    def 
+0000a710: 7465 7374 5f73 7276 2873 656c 6629 3a0a  test_srv(self):.
+0000a720: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+0000a730: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
+0000a740: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
+0000a750: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
+0000a760: 0a20 2020 2020 2020 207a 6f6e 6520 3d20  .        zone = 
+0000a770: 5a6f 6e65 2827 756e 6974 2e74 6573 7473  Zone('unit.tests
+0000a780: 2e27 2c20 5b5d 290a 2020 2020 2020 2020  .', []).        
+0000a790: 2320 5352 5620 7265 636f 7264 206e 6f74  # SRV record not
+0000a7a0: 2075 6e64 6572 2061 2073 7562 2d64 6f6d   under a sub-dom
+0000a7b0: 6169 6e0a 2020 2020 2020 2020 7372 765f  ain.        srv_
+0000a7c0: 7265 636f 7264 203d 2052 6563 6f72 642e  record = Record.
+0000a7d0: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
+0000a7e0: 207a 6f6e 652c 0a20 2020 2020 2020 2020   zone,.         
+0000a7f0: 2020 2027 5f65 7861 6d70 6c65 2e5f 7463     '_example._tc
+0000a800: 7027 2c0a 2020 2020 2020 2020 2020 2020  p',.            
+0000a810: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0000a820: 2020 2774 746c 273a 2033 3030 2c0a 2020    'ttl': 300,.  
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0000a840: 7970 6527 3a20 2753 5256 272c 0a20 2020  ype': 'SRV',.   
+0000a850: 2020 2020 2020 2020 2020 2020 2027 7661               'va
+0000a860: 6c75 6527 3a20 7b0a 2020 2020 2020 2020  lue': {.        
+0000a870: 2020 2020 2020 2020 2020 2020 2770 6f72              'por
+0000a880: 7427 3a20 3132 3334 2c0a 2020 2020 2020  t': 1234,.      
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2770                'p
+0000a8a0: 7269 6f72 6974 7927 3a20 302c 0a20 2020  riority': 0,.   
+0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8c0: 2027 7461 7267 6574 273a 2027 6e63 2e75   'target': 'nc.u
+0000a8d0: 6e69 742e 7465 7374 732e 272c 0a20 2020  nit.tests.',.   
+0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8f0: 2027 7765 6967 6874 273a 2035 2c0a 2020   'weight': 5,.  
+0000a900: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+0000a910: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
+0000a920: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000a930: 2020 2320 5352 5620 7265 636f 7264 2075    # SRV record u
+0000a940: 6e64 6572 2061 2073 7562 2d64 6f6d 6169  nder a sub-domai
+0000a950: 6e0a 2020 2020 2020 2020 7372 765f 7265  n.        srv_re
+0000a960: 636f 7264 5f77 6974 685f 7375 6220 3d20  cord_with_sub = 
+0000a970: 5265 636f 7264 2e6e 6577 280a 2020 2020  Record.new(.    
+0000a980: 2020 2020 2020 2020 7a6f 6e65 2c0a 2020          zone,.  
+0000a990: 2020 2020 2020 2020 2020 275f 6578 616d            '_exam
+0000a9a0: 706c 652e 5f74 6370 2e73 7562 272c 0a20  ple._tcp.sub',. 
+0000a9b0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+0000a9c0: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
+0000a9d0: 6c27 3a20 3330 302c 0a20 2020 2020 2020  l': 300,.       
+0000a9e0: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+0000a9f0: 2027 5352 5627 2c0a 2020 2020 2020 2020   'SRV',.        
+0000aa00: 2020 2020 2020 2020 2776 616c 7565 273a          'value':
+0000aa10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0000aa20: 2020 2020 2020 2027 706f 7274 273a 2031         'port': 1
+0000aa30: 3233 342c 0a20 2020 2020 2020 2020 2020  234,.           
+0000aa40: 2020 2020 2020 2020 2027 7072 696f 7269           'priori
+0000aa50: 7479 273a 2030 2c0a 2020 2020 2020 2020  ty': 0,.        
+0000aa60: 2020 2020 2020 2020 2020 2020 2774 6172              'tar
+0000aa70: 6765 7427 3a20 276e 632e 756e 6974 2e74  get': 'nc.unit.t
+0000aa80: 6573 7473 2e27 2c0a 2020 2020 2020 2020  ests.',.        
+0000aa90: 2020 2020 2020 2020 2020 2020 2777 6569              'wei
+0000aaa0: 6768 7427 3a20 352c 0a20 2020 2020 2020  ght': 5,.       
+0000aab0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0000aac0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+0000aad0: 2020 2029 0a0a 2020 2020 2020 2020 7372     )..        sr
+0000aae0: 765f 7265 636f 7264 5f63 6f6e 7465 6e74  v_record_content
+0000aaf0: 7320 3d20 7072 6f76 6964 6572 2e5f 6765  s = provider._ge
+0000ab00: 6e5f 6461 7461 2873 7276 5f72 6563 6f72  n_data(srv_recor
+0000ab10: 6429 0a20 2020 2020 2020 2073 7276 5f72  d).        srv_r
+0000ab20: 6563 6f72 645f 7769 7468 5f73 7562 5f63  ecord_with_sub_c
+0000ab30: 6f6e 7465 6e74 7320 3d20 7072 6f76 6964  ontents = provid
+0000ab40: 6572 2e5f 6765 6e5f 6461 7461 2873 7276  er._gen_data(srv
+0000ab50: 5f72 6563 6f72 645f 7769 7468 5f73 7562  _record_with_sub
+0000ab60: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000ab70: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+0000ab80: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+0000ab90: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
+0000aba0: 3a20 275f 6578 616d 706c 652e 5f74 6370  : '_example._tcp
+0000abb0: 2e75 6e69 742e 7465 7374 7327 2c0a 2020  .unit.tests',.  
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2774                't
+0000abd0: 746c 273a 2033 3030 2c0a 2020 2020 2020  tl': 300,.      
+0000abe0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+0000abf0: 3a20 2753 5256 272c 0a20 2020 2020 2020  : 'SRV',.       
+0000ac00: 2020 2020 2020 2020 2027 6461 7461 273a           'data':
+0000ac10: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+0000ac20: 2020 2020 2020 2027 7365 7276 6963 6527         'service'
+0000ac30: 3a20 275f 6578 616d 706c 6527 2c0a 2020  : '_example',.  
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2770 726f 746f 273a 2027 5f74 6370    'proto': '_tcp
+0000ac60: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000ac70: 2020 2020 2020 2027 6e61 6d65 273a 2027         'name': '
+0000ac80: 756e 6974 2e74 6573 7473 2e27 2c0a 2020  unit.tests.',.  
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2020 2770 7269 6f72 6974 7927 3a20 302c    'priority': 0,
+0000acb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000acc0: 2020 2020 2027 7765 6967 6874 273a 2035       'weight': 5
+0000acd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ace0: 2020 2020 2020 2770 6f72 7427 3a20 3132        'port': 12
+0000acf0: 3334 2c0a 2020 2020 2020 2020 2020 2020  34,.            
+0000ad00: 2020 2020 2020 2020 2774 6172 6765 7427          'target'
+0000ad10: 3a20 276e 632e 756e 6974 2e74 6573 7473  : 'nc.unit.tests
+0000ad20: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000ad30: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+0000ad40: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+0000ad50: 206c 6973 7428 7372 765f 7265 636f 7264   list(srv_record
+0000ad60: 5f63 6f6e 7465 6e74 7329 5b30 5d2c 0a20  _contents)[0],. 
+0000ad70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ad80: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000ad90: 6c28 0a20 2020 2020 2020 2020 2020 207b  l(.            {
+0000ada0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000adb0: 2027 6e61 6d65 273a 2027 5f65 7861 6d70   'name': '_examp
+0000adc0: 6c65 2e5f 7463 702e 7375 622e 756e 6974  le._tcp.sub.unit
+0000add0: 2e74 6573 7473 272c 0a20 2020 2020 2020  .tests',.       
+0000ade0: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
+0000adf0: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
+0000ae00: 2020 2020 2027 7479 7065 273a 2027 5352       'type': 'SR
+0000ae10: 5627 2c0a 2020 2020 2020 2020 2020 2020  V',.            
+0000ae20: 2020 2020 2764 6174 6127 3a20 7b0a 2020      'data': {.  
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 2020 2773 6572 7669 6365 273a 2027 5f65    'service': '_e
+0000ae50: 7861 6d70 6c65 272c 0a20 2020 2020 2020  xample',.       
+0000ae60: 2020 2020 2020 2020 2020 2020 2027 7072               'pr
+0000ae70: 6f74 6f27 3a20 275f 7463 7027 2c0a 2020  oto': '_tcp',.  
+0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae90: 2020 276e 616d 6527 3a20 2773 7562 272c    'name': 'sub',
+0000aea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aeb0: 2020 2020 2027 7072 696f 7269 7479 273a       'priority':
+0000aec0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+0000aed0: 2020 2020 2020 2020 2777 6569 6768 7427          'weight'
+0000aee0: 3a20 352c 0a20 2020 2020 2020 2020 2020  : 5,.           
+0000aef0: 2020 2020 2020 2020 2027 706f 7274 273a           'port':
+0000af00: 2031 3233 342c 0a20 2020 2020 2020 2020   1234,.         
+0000af10: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
+0000af20: 6574 273a 2027 6e63 2e75 6e69 742e 7465  et': 'nc.unit.te
+0000af30: 7374 7327 2c0a 2020 2020 2020 2020 2020  sts',.          
+0000af40: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0000af50: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+0000af60: 2020 2020 6c69 7374 2873 7276 5f72 6563      list(srv_rec
+0000af70: 6f72 645f 7769 7468 5f73 7562 5f63 6f6e  ord_with_sub_con
+0000af80: 7465 6e74 7329 5b30 5d2c 0a20 2020 2020  tents)[0],.     
+0000af90: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
+0000afa0: 7374 5f74 7874 2873 656c 6629 3a0a 2020  st_txt(self):.  
+0000afb0: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
+0000afc0: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
+0000afd0: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
+0000afe0: 696c 272c 2027 746f 6b65 6e27 290a 0a20  il', 'token').. 
+0000aff0: 2020 2020 2020 2023 2073 696e 676c 6520         # single 
+0000b000: 7265 636f 7264 2077 2f63 6f6e 7465 6e74  record w/content
+0000b010: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0000b020: 7072 6f76 6964 6572 2e5f 6461 7461 5f66  provider._data_f
+0000b030: 6f72 5f54 5854 280a 2020 2020 2020 2020  or_TXT(.        
+0000b040: 2020 2020 2754 5854 272c 205b 7b27 7474      'TXT', [{'tt
+0000b050: 6c27 3a20 3432 2c20 2763 6f6e 7465 6e74  l': 42, 'content
+0000b060: 273a 2027 6865 6c6c 6f20 776f 726c 6427  ': 'hello world'
+0000b070: 7d5d 0a20 2020 2020 2020 2029 0a20 2020  }].        ).   
+0000b080: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000b090: 4571 7561 6c28 0a20 2020 2020 2020 2020  Equal(.         
+0000b0a0: 2020 207b 2774 746c 273a 2034 322c 2027     {'ttl': 42, '
+0000b0b0: 7479 7065 273a 2027 5458 5427 2c20 2776  type': 'TXT', 'v
+0000b0c0: 616c 7565 7327 3a20 5b27 6865 6c6c 6f20  alues': ['hello 
+0000b0d0: 776f 726c 6427 5d7d 2c20 6461 7461 0a20  world']}, data. 
+0000b0e0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000b0f0: 2020 2320 6d69 7373 696e 6720 636f 6e74    # missing cont
+0000b100: 656e 742c 2065 7175 6976 696c 656e 7420  ent, equivilent 
+0000b110: 746f 2065 6d70 7479 2066 726f 6d20 4346  to empty from CF
+0000b120: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
+0000b130: 7072 6f76 6964 6572 2e5f 6461 7461 5f66  provider._data_f
+0000b140: 6f72 5f54 5854 2827 5458 5427 2c20 5b7b  or_TXT('TXT', [{
+0000b150: 2774 746c 273a 2034 327d 5d29 0a20 2020  'ttl': 42}]).   
+0000b160: 2020 2020 2066 726f 6d20 7070 7269 6e74       from pprint
+0000b170: 2069 6d70 6f72 7420 7070 7269 6e74 0a0a   import pprint..
+0000b180: 2020 2020 2020 2020 7070 7269 6e74 2864          pprint(d
+0000b190: 6174 6129 0a0a 2020 2020 2020 2020 7365  ata)..        se
+0000b1a0: 6c66 2e61 7373 6572 7445 7175 616c 287b  lf.assertEqual({
+0000b1b0: 2774 746c 273a 2034 322c 2027 7479 7065  'ttl': 42, 'type
+0000b1c0: 273a 2027 5458 5427 2c20 2776 616c 7565  ': 'TXT', 'value
+0000b1d0: 7327 3a20 5b27 275d 7d2c 2064 6174 6129  s': ['']}, data)
+0000b1e0: 0a0a 2020 2020 6465 6620 7465 7374 5f61  ..    def test_a
+0000b1f0: 6c69 6173 2873 656c 6629 3a0a 2020 2020  lias(self):.    
+0000b200: 2020 2020 7072 6f76 6964 6572 203d 2043      provider = C
+0000b210: 6c6f 7564 666c 6172 6550 726f 7669 6465  loudflareProvide
+0000b220: 7228 2774 6573 7427 2c20 2765 6d61 696c  r('test', 'email
+0000b230: 272c 2027 746f 6b65 6e27 290a 0a20 2020  ', 'token')..   
+0000b240: 2020 2020 2023 2041 2043 4e41 4d45 2066       # A CNAME f
+0000b250: 6f72 2075 7320 746f 2074 7261 6e73 666f  or us to transfo
+0000b260: 726d 2074 6f20 414c 4941 530a 2020 2020  rm to ALIAS.    
+0000b270: 2020 2020 7072 6f76 6964 6572 2e7a 6f6e      provider.zon
+0000b280: 655f 7265 636f 7264 7320 3d20 4d6f 636b  e_records = Mock
+0000b290: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+0000b2a0: 7475 726e 5f76 616c 7565 3d5b 0a20 2020  turn_value=[.   
+0000b2b0: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
 0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2d0: 227a 6f6e 655f 6e61 6d65 223a 2022 756e  "zone_name": "un
-0000b2e0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
-0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000b300: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
-0000b310: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
-0000b320: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
-0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b340: 2022 6372 6561 7465 645f 6f6e 223a 2022   "created_on": "
-0000b350: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
-0000b360: 3a34 332e 3432 3036 3839 5a22 2c0a 2020  :43.420689Z",.  
-0000b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b380: 2020 226d 6574 6122 3a20 7b22 6175 746f    "meta": {"auto
-0000b390: 5f61 6464 6564 223a 2046 616c 7365 7d2c  _added": False},
-0000b3a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b3b0: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
-0000b3c0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000b3d0: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
-0000b3e0: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-0000b3f0: 5d29 0a20 2020 2020 2020 2070 726f 7669  ]).        provi
-0000b400: 6465 722e 706f 7075 6c61 7465 287a 6f6e  der.populate(zon
-0000b410: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-0000b420: 6173 7365 7274 4571 7561 6c28 312c 206c  assertEqual(1, l
-0000b430: 656e 287a 6f6e 652e 7265 636f 7264 7329  en(zone.records)
-0000b440: 290a 2020 2020 2020 2020 7265 636f 7264  ).        record
-0000b450: 203d 206c 6973 7428 7a6f 6e65 2e72 6563   = list(zone.rec
-0000b460: 6f72 6473 295b 305d 0a20 2020 2020 2020  ords)[0].       
-0000b470: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000b480: 6c28 2727 2c20 7265 636f 7264 2e6e 616d  l('', record.nam
-0000b490: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
-0000b4a0: 6173 7365 7274 4571 7561 6c28 2775 6e69  assertEqual('uni
-0000b4b0: 742e 7465 7374 732e 272c 2072 6563 6f72  t.tests.', recor
-0000b4c0: 642e 6671 646e 290a 2020 2020 2020 2020  d.fqdn).        
-0000b4d0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000b4e0: 2827 414c 4941 5327 2c20 7265 636f 7264  ('ALIAS', record
-0000b4f0: 2e5f 7479 7065 290a 2020 2020 2020 2020  ._type).        
-0000b500: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000b510: 2827 7777 772e 756e 6974 2e74 6573 7473  ('www.unit.tests
-0000b520: 2e27 2c20 7265 636f 7264 2e76 616c 7565  .', record.value
-0000b530: 290a 0a20 2020 2020 2020 2023 204d 616b  )..        # Mak
-0000b540: 6520 7375 7265 2077 6520 7472 616e 7366  e sure we transf
-0000b550: 6f72 6d20 6261 636b 2074 6f20 434e 414d  orm back to CNAM
-0000b560: 4520 676f 696e 6720 7468 6520 6f74 6865  E going the othe
-0000b570: 7220 7761 790a 2020 2020 2020 2020 636f  r way.        co
-0000b580: 6e74 656e 7473 203d 2070 726f 7669 6465  ntents = provide
-0000b590: 722e 5f67 656e 5f64 6174 6128 7265 636f  r._gen_data(reco
-0000b5a0: 7264 290a 2020 2020 2020 2020 7365 6c66  rd).        self
-0000b5b0: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
-0000b5c0: 2020 2020 2020 2020 2020 7b0a 2020 2020            {.    
-0000b5d0: 2020 2020 2020 2020 2020 2020 2763 6f6e              'con
-0000b5e0: 7465 6e74 273a 2027 7777 772e 756e 6974  tent': 'www.unit
-0000b5f0: 2e74 6573 7473 2e27 2c0a 2020 2020 2020  .tests.',.      
-0000b600: 2020 2020 2020 2020 2020 276e 616d 6527            'name'
-0000b610: 3a20 2775 6e69 742e 7465 7374 7327 2c0a  : 'unit.tests',.
-0000b620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b630: 2770 726f 7869 6564 273a 2046 616c 7365  'proxied': False
-0000b640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b650: 2020 2774 746c 273a 2033 3030 2c0a 2020    'ttl': 300,.  
-0000b660: 2020 2020 2020 2020 2020 2020 2020 2774                't
-0000b670: 7970 6527 3a20 2743 4e41 4d45 272c 0a20  ype': 'CNAME',. 
-0000b680: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-0000b690: 2020 2020 2020 2020 2020 6c69 7374 2863            list(c
-0000b6a0: 6f6e 7465 6e74 7329 5b30 5d2c 0a20 2020  ontents)[0],.   
-0000b6b0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-0000b6c0: 7465 7374 5f67 656e 5f6b 6579 2873 656c  test_gen_key(sel
-0000b6d0: 6629 3a0a 2020 2020 2020 2020 7072 6f76  f):.        prov
-0000b6e0: 6964 6572 203d 2043 6c6f 7564 666c 6172  ider = Cloudflar
-0000b6f0: 6550 726f 7669 6465 7228 2774 6573 7427  eProvider('test'
-0000b700: 2c20 2765 6d61 696c 272c 2027 746f 6b65  , 'email', 'toke
-0000b710: 6e27 290a 0a20 2020 2020 2020 2066 6f72  n')..        for
-0000b720: 2065 7870 6563 7465 642c 2064 6174 6120   expected, data 
-0000b730: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
-0000b740: 2028 2766 6f6f 2e62 6172 2e63 6f6d 2e27   ('foo.bar.com.'
-0000b750: 2c20 7b27 636f 6e74 656e 7427 3a20 2766  , {'content': 'f
-0000b760: 6f6f 2e62 6172 2e63 6f6d 2e27 2c20 2774  oo.bar.com.', 't
-0000b770: 7970 6527 3a20 2743 4e41 4d45 277d 292c  ype': 'CNAME'}),
-0000b780: 0a20 2020 2020 2020 2020 2020 2028 0a20  .            (. 
-0000b790: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000b7a0: 3130 2066 6f6f 2e62 6172 2e63 6f6d 2e27  10 foo.bar.com.'
-0000b7b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b7c0: 2020 7b27 636f 6e74 656e 7427 3a20 2766    {'content': 'f
-0000b7d0: 6f6f 2e62 6172 2e63 6f6d 2e27 2c20 2770  oo.bar.com.', 'p
-0000b7e0: 7269 6f72 6974 7927 3a20 3130 2c20 2774  riority': 10, 't
-0000b7f0: 7970 6527 3a20 274d 5827 7d2c 0a20 2020  ype': 'MX'},.   
-0000b800: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-0000b810: 2020 2020 2020 2020 280a 2020 2020 2020          (.      
-0000b820: 2020 2020 2020 2020 2020 2730 2074 6167            '0 tag
-0000b830: 2073 6f6d 652d 7661 6c75 6527 2c0a 2020   some-value',.  
-0000b840: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b860: 2020 2020 2764 6174 6127 3a20 7b27 666c      'data': {'fl
-0000b870: 6167 7327 3a20 302c 2027 7461 6727 3a20  ags': 0, 'tag': 
-0000b880: 2774 6167 272c 2027 7661 6c75 6527 3a20  'tag', 'value': 
-0000b890: 2773 6f6d 652d 7661 6c75 6527 7d2c 0a20  'some-value'},. 
-0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8b0: 2020 2027 7479 7065 273a 2027 4341 4127     'type': 'CAA'
-0000b8c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b8d0: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
-0000b8e0: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
-0000b8f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b900: 2020 2734 3220 3130 3020 7468 696e 672d    '42 100 thing-
-0000b910: 7765 7265 2d70 6f69 6e74 6564 2e61 7420  were-pointed.at 
-0000b920: 3130 3127 2c0a 2020 2020 2020 2020 2020  101',.          
-0000b930: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0000b940: 2020 2020 2020 2020 2020 2020 2764 6174              'dat
-0000b950: 6127 3a20 7b0a 2020 2020 2020 2020 2020  a': {.          
-0000b960: 2020 2020 2020 2020 2020 2020 2020 2770                'p
-0000b970: 6f72 7427 3a20 3432 2c0a 2020 2020 2020  ort': 42,.      
-0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b990: 2020 2770 7269 6f72 6974 7927 3a20 3130    'priority': 10
-0000b9a0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0000b9b0: 2020 2020 2020 2020 2020 2027 7461 7267             'targ
-0000b9c0: 6574 273a 2027 7468 696e 672d 7765 7265  et': 'thing-were
-0000b9d0: 2d70 6f69 6e74 6564 2e61 7427 2c0a 2020  -pointed.at',.  
-0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b9f0: 2020 2020 2020 2777 6569 6768 7427 3a20        'weight': 
-0000ba00: 3130 312c 0a20 2020 2020 2020 2020 2020  101,.           
-0000ba10: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2774 7970 6527 3a20 2753 5256 272c 0a20  'type': 'SRV',. 
-0000ba40: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-0000ba50: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-0000ba60: 0a20 2020 2020 2020 2020 2020 2028 0a20  .            (. 
-0000ba70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000ba80: 3331 2035 3820 3532 2e31 2053 2031 3135  31 58 52.1 S 115
-0000ba90: 2034 3920 3131 2e37 2045 2032 3020 3130   49 11.7 E 20 10
-0000baa0: 2031 3020 3227 2c0a 2020 2020 2020 2020   10 2',.        
-0000bab0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-0000bac0: 2020 2020 2020 2020 2020 2020 2020 2764                'd
-0000bad0: 6174 6127 3a20 7b0a 2020 2020 2020 2020  ata': {.        
-0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000baf0: 276c 6174 5f64 6567 7265 6573 273a 2033  'lat_degrees': 3
-0000bb00: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-0000bb10: 2020 2020 2020 2020 2020 2027 6c61 745f             'lat_
-0000bb20: 6d69 6e75 7465 7327 3a20 3538 2c0a 2020  minutes': 58,.  
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb40: 2020 2020 2020 276c 6174 5f73 6563 6f6e        'lat_secon
-0000bb50: 6473 273a 2035 322e 312c 0a20 2020 2020  ds': 52.1,.     
-0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2020 2027 6c61 745f 6469 7265 6374 696f     'lat_directio
-0000bb80: 6e27 3a20 2753 272c 0a20 2020 2020 2020  n': 'S',.       
-0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bba0: 2027 6c6f 6e67 5f64 6567 7265 6573 273a   'long_degrees':
-0000bbb0: 2031 3135 2c0a 2020 2020 2020 2020 2020   115,.          
-0000bbc0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
-0000bbd0: 6f6e 675f 6d69 6e75 7465 7327 3a20 3439  ong_minutes': 49
-0000bbe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000bbf0: 2020 2020 2020 2020 2020 276c 6f6e 675f            'long_
-0000bc00: 7365 636f 6e64 7327 3a20 3131 2e37 2c0a  seconds': 11.7,.
-0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc20: 2020 2020 2020 2020 276c 6f6e 675f 6469          'long_di
-0000bc30: 7265 6374 696f 6e27 3a20 2745 272c 0a20  rection': 'E',. 
-0000bc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc50: 2020 2020 2020 2027 616c 7469 7475 6465         'altitude
-0000bc60: 273a 2032 302c 0a20 2020 2020 2020 2020  ': 20,.         
-0000bc70: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000bc80: 7369 7a65 273a 2031 302c 0a20 2020 2020  size': 10,.     
-0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bca0: 2020 2027 7072 6563 6973 696f 6e5f 686f     'precision_ho
-0000bcb0: 727a 273a 2031 302c 0a20 2020 2020 2020  rz': 10,.       
-0000bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcd0: 2027 7072 6563 6973 696f 6e5f 7665 7274   'precision_vert
-0000bce0: 273a 2032 2c0a 2020 2020 2020 2020 2020  ': 2,.          
-0000bcf0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd10: 2027 7479 7065 273a 2027 4c4f 4327 2c0a   'type': 'LOC',.
+0000b2d0: 2020 2022 6964 223a 2022 6663 3132 6162     "id": "fc12ab
+0000b2e0: 3334 6364 3536 3131 3333 3434 3232 6162  34cd5611334422ab
+0000b2f0: 3333 3232 3939 3736 3432 222c 0a20 2020  3322997642",.   
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2022 7479 7065 223a 2022 434e 414d 4522   "type": "CNAME"
+0000b320: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b330: 2020 2020 2020 226e 616d 6522 3a20 2275        "name": "u
+0000b340: 6e69 742e 7465 7374 7322 2c0a 2020 2020  nit.tests",.    
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b360: 2263 6f6e 7465 6e74 223a 2022 7777 772e  "content": "www.
+0000b370: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
+0000b3a0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000b3b0: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
+0000b3c0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+0000b3e0: 746c 223a 2033 3030 2c0a 2020 2020 2020  tl": 300,.      
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+0000b400: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
+0000b410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b420: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
+0000b430: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
+0000b440: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
+0000b450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b460: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
+0000b470: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
+0000b480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b490: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
+0000b4a0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
+0000b4b0: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
+0000b4c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000b4d0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
+0000b4e0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
+0000b4f0: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
+0000b500: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
+0000b510: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
+0000b520: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
+0000b530: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
+0000b540: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0000b550: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
+0000b560: 0a0a 2020 2020 2020 2020 7a6f 6e65 203d  ..        zone =
+0000b570: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+0000b580: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
+0000b590: 2070 726f 7669 6465 722e 706f 7075 6c61   provider.popula
+0000b5a0: 7465 287a 6f6e 6529 0a20 2020 2020 2020  te(zone).       
+0000b5b0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000b5c0: 6c28 312c 206c 656e 287a 6f6e 652e 7265  l(1, len(zone.re
+0000b5d0: 636f 7264 7329 290a 2020 2020 2020 2020  cords)).        
+0000b5e0: 7265 636f 7264 203d 206c 6973 7428 7a6f  record = list(zo
+0000b5f0: 6e65 2e72 6563 6f72 6473 295b 305d 0a20  ne.records)[0]. 
+0000b600: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000b610: 7274 4571 7561 6c28 2727 2c20 7265 636f  rtEqual('', reco
+0000b620: 7264 2e6e 616d 6529 0a20 2020 2020 2020  rd.name).       
+0000b630: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000b640: 6c28 2775 6e69 742e 7465 7374 732e 272c  l('unit.tests.',
+0000b650: 2072 6563 6f72 642e 6671 646e 290a 2020   record.fqdn).  
+0000b660: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000b670: 7445 7175 616c 2827 414c 4941 5327 2c20  tEqual('ALIAS', 
+0000b680: 7265 636f 7264 2e5f 7479 7065 290a 2020  record._type).  
+0000b690: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000b6a0: 7445 7175 616c 2827 7777 772e 756e 6974  tEqual('www.unit
+0000b6b0: 2e74 6573 7473 2e27 2c20 7265 636f 7264  .tests.', record
+0000b6c0: 2e76 616c 7565 290a 0a20 2020 2020 2020  .value)..       
+0000b6d0: 2023 204d 616b 6520 7375 7265 2077 6520   # Make sure we 
+0000b6e0: 7472 616e 7366 6f72 6d20 6261 636b 2074  transform back t
+0000b6f0: 6f20 434e 414d 4520 676f 696e 6720 7468  o CNAME going th
+0000b700: 6520 6f74 6865 7220 7761 790a 2020 2020  e other way.    
+0000b710: 2020 2020 636f 6e74 656e 7473 203d 2070      contents = p
+0000b720: 726f 7669 6465 722e 5f67 656e 5f64 6174  rovider._gen_dat
+0000b730: 6128 7265 636f 7264 290a 2020 2020 2020  a(record).      
+0000b740: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+0000b750: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+0000b760: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+0000b770: 2020 2763 6f6e 7465 6e74 273a 2027 7777    'content': 'ww
+0000b780: 772e 756e 6974 2e74 6573 7473 2e27 2c0a  w.unit.tests.',.
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 276e 616d 6527 3a20 2775 6e69 742e 7465  'name': 'unit.te
+0000b7b0: 7374 7327 2c0a 2020 2020 2020 2020 2020  sts',.          
+0000b7c0: 2020 2020 2020 2770 726f 7869 6564 273a        'proxied':
+0000b7d0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+0000b7e0: 2020 2020 2020 2020 2774 746c 273a 2033          'ttl': 3
+0000b7f0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+0000b800: 2020 2020 2774 7970 6527 3a20 2743 4e41      'type': 'CNA
+0000b810: 4d45 272c 0a20 2020 2020 2020 2020 2020  ME',.           
+0000b820: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+0000b830: 6c69 7374 2863 6f6e 7465 6e74 7329 5b30  list(contents)[0
+0000b840: 5d2c 0a20 2020 2020 2020 2029 0a0a 2020  ],.        )..  
+0000b850: 2020 6465 6620 7465 7374 5f67 656e 5f6b    def test_gen_k
+0000b860: 6579 2873 656c 6629 3a0a 2020 2020 2020  ey(self):.      
+0000b870: 2020 7072 6f76 6964 6572 203d 2043 6c6f    provider = Clo
+0000b880: 7564 666c 6172 6550 726f 7669 6465 7228  udflareProvider(
+0000b890: 2774 6573 7427 2c20 2765 6d61 696c 272c  'test', 'email',
+0000b8a0: 2027 746f 6b65 6e27 290a 0a20 2020 2020   'token')..     
+0000b8b0: 2020 2066 6f72 2065 7870 6563 7465 642c     for expected,
+0000b8c0: 2064 6174 6120 696e 2028 0a20 2020 2020   data in (.     
+0000b8d0: 2020 2020 2020 2028 2766 6f6f 2e62 6172         ('foo.bar
+0000b8e0: 2e63 6f6d 2e27 2c20 7b27 636f 6e74 656e  .com.', {'conten
+0000b8f0: 7427 3a20 2766 6f6f 2e62 6172 2e63 6f6d  t': 'foo.bar.com
+0000b900: 2e27 2c20 2774 7970 6527 3a20 2743 4e41  .', 'type': 'CNA
+0000b910: 4d45 277d 292c 0a20 2020 2020 2020 2020  ME'}),.         
+0000b920: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+0000b930: 2020 2020 2027 3130 2066 6f6f 2e62 6172       '10 foo.bar
+0000b940: 2e63 6f6d 2e27 2c0a 2020 2020 2020 2020  .com.',.        
+0000b950: 2020 2020 2020 2020 7b27 636f 6e74 656e          {'conten
+0000b960: 7427 3a20 2766 6f6f 2e62 6172 2e63 6f6d  t': 'foo.bar.com
+0000b970: 2e27 2c20 2770 7269 6f72 6974 7927 3a20  .', 'priority': 
+0000b980: 3130 2c20 2774 7970 6527 3a20 274d 5827  10, 'type': 'MX'
+0000b990: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
+0000b9a0: 2c0a 2020 2020 2020 2020 2020 2020 280a  ,.            (.
+0000b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9c0: 2730 2074 6167 2073 6f6d 652d 7661 6c75  '0 tag some-valu
+0000b9d0: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+0000b9e0: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000b9f0: 2020 2020 2020 2020 2020 2764 6174 6127            'data'
+0000ba00: 3a20 7b27 666c 6167 7327 3a20 302c 2027  : {'flags': 0, '
+0000ba10: 7461 6727 3a20 2774 6167 272c 2027 7661  tag': 'tag', 'va
+0000ba20: 6c75 6527 3a20 2773 6f6d 652d 7661 6c75  lue': 'some-valu
+0000ba30: 6527 7d2c 0a20 2020 2020 2020 2020 2020  e'},.           
+0000ba40: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+0000ba50: 2027 4341 4127 2c0a 2020 2020 2020 2020   'CAA',.        
+0000ba60: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+0000ba70: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+0000ba80: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+0000ba90: 2020 2020 2020 2020 2734 3220 3130 3020          '42 100 
+0000baa0: 7468 696e 672d 7765 7265 2d70 6f69 6e74  thing-were-point
+0000bab0: 6564 2e61 7420 3130 3127 2c0a 2020 2020  ed.at 101',.    
+0000bac0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2764 6174 6127 3a20 7b0a 2020 2020    'data': {.    
+0000baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb00: 2020 2020 2770 6f72 7427 3a20 3432 2c0a      'port': 42,.
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2020 2020 2770 7269 6f72 6974          'priorit
+0000bb30: 7927 3a20 3130 302c 0a20 2020 2020 2020  y': 100,.       
+0000bb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb50: 2027 7461 7267 6574 273a 2027 7468 696e   'target': 'thin
+0000bb60: 672d 7765 7265 2d70 6f69 6e74 6564 2e61  g-were-pointed.a
+0000bb70: 7427 2c0a 2020 2020 2020 2020 2020 2020  t',.            
+0000bb80: 2020 2020 2020 2020 2020 2020 2777 6569              'wei
+0000bb90: 6768 7427 3a20 3130 312c 0a20 2020 2020  ght': 101,.     
+0000bba0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+0000bbb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000bbc0: 2020 2020 2020 2774 7970 6527 3a20 2753        'type': 'S
+0000bbd0: 5256 272c 0a20 2020 2020 2020 2020 2020  RV',.           
+0000bbe0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+0000bbf0: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+0000bc00: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
+0000bc10: 2020 2020 2027 3331 2035 3820 3532 2e31       '31 58 52.1
+0000bc20: 2053 2031 3135 2034 3920 3131 2e37 2045   S 115 49 11.7 E
+0000bc30: 2032 3020 3130 2031 3020 3227 2c0a 2020   20 10 10 2',.  
+0000bc40: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
+0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc60: 2020 2020 2764 6174 6127 3a20 7b0a 2020      'data': {.  
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 276c 6174 5f64 6567 7265        'lat_degre
+0000bc90: 6573 273a 2033 312c 0a20 2020 2020 2020  es': 31,.       
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2027 6c61 745f 6d69 6e75 7465 7327 3a20   'lat_minutes': 
+0000bcc0: 3538 2c0a 2020 2020 2020 2020 2020 2020  58,.            
+0000bcd0: 2020 2020 2020 2020 2020 2020 276c 6174              'lat
+0000bce0: 5f73 6563 6f6e 6473 273a 2035 322e 312c  _seconds': 52.1,
+0000bcf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bd00: 2020 2020 2020 2020 2027 6c61 745f 6469           'lat_di
+0000bd10: 7265 6374 696f 6e27 3a20 2753 272c 0a20  rection': 'S',. 
 0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
-0000bd40: 2c0a 2020 2020 2020 2020 293a 0a20 2020  ,.        ):.   
-0000bd50: 2020 2020 2020 2020 2073 656c 662e 6173           self.as
-0000bd60: 7365 7274 4571 7561 6c28 6578 7065 6374  sertEqual(expect
-0000bd70: 6564 2c20 7072 6f76 6964 6572 2e5f 6765  ed, provider._ge
-0000bd80: 6e5f 6b65 7928 6461 7461 2929 0a0a 2020  n_key(data))..  
-0000bd90: 2020 6465 6620 7465 7374 5f63 646e 2873    def test_cdn(s
-0000bda0: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-0000bdb0: 6f76 6964 6572 203d 2043 6c6f 7564 666c  ovider = Cloudfl
-0000bdc0: 6172 6550 726f 7669 6465 7228 0a20 2020  areProvider(.   
-0000bdd0: 2020 2020 2020 2020 2027 7465 7374 272c           'test',
-0000bde0: 2027 656d 6169 6c27 2c20 2774 6f6b 656e   'email', 'token
-0000bdf0: 272c 2027 6163 636f 756e 745f 6964 272c  ', 'account_id',
-0000be00: 2054 7275 650a 2020 2020 2020 2020 290a   True.        ).
-0000be10: 0a20 2020 2020 2020 2023 2041 2043 4e41  .        # A CNA
-0000be20: 4d45 2066 6f72 2075 7320 746f 2074 7261  ME for us to tra
-0000be30: 6e73 666f 726d 2074 6f20 414c 4941 530a  nsform to ALIAS.
-0000be40: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
-0000be50: 2e7a 6f6e 655f 7265 636f 7264 7320 3d20  .zone_records = 
-0000be60: 4d6f 636b 280a 2020 2020 2020 2020 2020  Mock(.          
-0000be70: 2020 7265 7475 726e 5f76 616c 7565 3d5b    return_value=[
-0000be80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000be90: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0000bea0: 2020 2020 2020 2022 6964 223a 2022 6663         "id": "fc
-0000beb0: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
-0000bec0: 3232 6162 3333 3232 3939 3736 3432 222c  22ab3322997642",
-0000bed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bee0: 2020 2020 2022 7479 7065 223a 2022 434e       "type": "CN
-0000bef0: 414d 4522 2c0a 2020 2020 2020 2020 2020  AME",.          
-0000bf00: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
-0000bf10: 3a20 2263 6e61 6d65 2e75 6e69 742e 7465  : "cname.unit.te
-0000bf20: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
-0000bf30: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
-0000bf40: 6e74 223a 2022 7777 772e 756e 6974 2e74  nt": "www.unit.t
-0000bf50: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
-0000bf60: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
-0000bf70: 6961 626c 6522 3a20 5472 7565 2c0a 2020  iable": True,.  
-0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf90: 2020 2270 726f 7869 6564 223a 2054 7275    "proxied": Tru
-0000bfa0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000bfb0: 2020 2020 2020 2022 7474 6c22 3a20 3330         "ttl": 30
-0000bfc0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0000bfd0: 2020 2020 2020 2022 6c6f 636b 6564 223a         "locked":
-0000bfe0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-0000bff0: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
-0000c000: 655f 6964 223a 2022 6666 3132 6162 3334  e_id": "ff12ab34
-0000c010: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
-0000c020: 3232 3939 3736 3530 222c 0a20 2020 2020  22997650",.     
-0000c030: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c040: 7a6f 6e65 5f6e 616d 6522 3a20 2275 6e69  zone_name": "uni
-0000c050: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
-0000c060: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0000c070: 6f64 6966 6965 645f 6f6e 223a 2022 3230  odified_on": "20
-0000c080: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
-0000c090: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
-0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0b0: 2263 7265 6174 6564 5f6f 6e22 3a20 2232  "created_on": "2
-0000c0c0: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
-0000c0d0: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
-0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0f0: 2022 6d65 7461 223a 207b 2261 7574 6f5f   "meta": {"auto_
-0000c100: 6164 6465 6422 3a20 4661 6c73 657d 2c0a  added": False},.
-0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c120: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-0000c130: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-0000c140: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-0000c150: 6663 3132 6162 3334 6364 3536 3131 3333  fc12ab34cd561133
-0000c160: 3434 3232 6162 3333 3232 3939 3736 3432  4422ab3322997642
-0000c170: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000c180: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-0000c190: 4122 2c0a 2020 2020 2020 2020 2020 2020  A",.            
-0000c1a0: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-0000c1b0: 2261 2e75 6e69 742e 7465 7374 7322 2c0a  "a.unit.tests",.
-0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1d0: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-0000c1e0: 312e 312e 312e 3122 2c0a 2020 2020 2020  1.1.1.1",.      
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-0000c200: 726f 7869 6162 6c65 223a 2054 7275 652c  roxiable": True,
-0000c210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c220: 2020 2020 2022 7072 6f78 6965 6422 3a20       "proxied": 
-0000c230: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000c240: 2020 2020 2020 2020 2020 2274 746c 223a            "ttl":
-0000c250: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
-0000c260: 2020 2020 2020 2020 2020 226c 6f63 6b65            "locke
-0000c270: 6422 3a20 4661 6c73 652c 0a20 2020 2020  d": False,.     
-0000c280: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c290: 7a6f 6e65 5f69 6422 3a20 2266 6631 3261  zone_id": "ff12a
-0000c2a0: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-0000c2b0: 6233 3332 3239 3937 3635 3022 2c0a 2020  b3322997650",.  
-0000c2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2d0: 2020 227a 6f6e 655f 6e61 6d65 223a 2022    "zone_name": "
-0000c2e0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c300: 2022 6d6f 6469 6669 6564 5f6f 6e22 3a20   "modified_on": 
-0000c310: 2232 3031 372d 3033 2d31 3154 3138 3a30  "2017-03-11T18:0
-0000c320: 313a 3433 2e34 3230 3638 395a 222c 0a20  1:43.420689Z",. 
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2020 2022 6372 6561 7465 645f 6f6e 223a     "created_on":
-0000c350: 2022 3230 3137 2d30 332d 3131 5431 383a   "2017-03-11T18:
-0000c360: 3031 3a34 332e 3432 3036 3839 5a22 2c0a  01:43.420689Z",.
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2020 2020 226d 6574 6122 3a20 7b22 6175      "meta": {"au
-0000c390: 746f 5f61 6464 6564 223a 2046 616c 7365  to_added": False
-0000c3a0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-0000c3b0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-0000c3c0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-0000c3d0: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
-0000c3e0: 3a20 2266 6331 3261 6233 3463 6435 3631  : "fc12ab34cd561
-0000c3f0: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
-0000c400: 3634 3222 2c0a 2020 2020 2020 2020 2020  642",.          
-0000c410: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-0000c420: 3a20 2241 222c 0a20 2020 2020 2020 2020  : "A",.         
-0000c430: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-0000c440: 223a 2022 612e 756e 6974 2e74 6573 7473  ": "a.unit.tests
-0000c450: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000c460: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
-0000c470: 3a20 2231 2e31 2e31 2e32 222c 0a20 2020  : "1.1.1.2",.   
-0000c480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c490: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
-0000c4a0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000c4b0: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
-0000c4c0: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-0000c4d0: 2020 2020 2020 2020 2020 2020 2022 7474               "tt
-0000c4e0: 6c22 3a20 3330 302c 0a20 2020 2020 2020  l": 300,.       
-0000c4f0: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
-0000c500: 636b 6564 223a 2046 616c 7365 2c0a 2020  cked": False,.  
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2020 227a 6f6e 655f 6964 223a 2022 6666    "zone_id": "ff
-0000c530: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
-0000c540: 3232 6162 3333 3232 3939 3736 3530 222c  22ab3322997650",
-0000c550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c560: 2020 2020 2022 7a6f 6e65 5f6e 616d 6522       "zone_name"
-0000c570: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
-0000c580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c590: 2020 2020 226d 6f64 6966 6965 645f 6f6e      "modified_on
-0000c5a0: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
-0000c5b0: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
-0000c5c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000c5d0: 2020 2020 2020 2263 7265 6174 6564 5f6f        "created_o
-0000c5e0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
-0000c5f0: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
-0000c600: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000c610: 2020 2020 2020 2022 6d65 7461 223a 207b         "meta": {
-0000c620: 2261 7574 6f5f 6164 6465 6422 3a20 4661  "auto_added": Fa
-0000c630: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
-0000c640: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-0000c650: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
-0000c660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c670: 6964 223a 2022 6663 3132 6162 3334 6364  id": "fc12ab34cd
-0000c680: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
-0000c690: 3939 3736 3432 222c 0a20 2020 2020 2020  997642",.       
-0000c6a0: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
-0000c6b0: 7065 223a 2022 4122 2c0a 2020 2020 2020  pe": "A",.      
-0000c6c0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-0000c6d0: 616d 6522 3a20 226d 756c 7469 2e75 6e69  ame": "multi.uni
-0000c6e0: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-0000c700: 6f6e 7465 6e74 223a 2022 312e 312e 312e  ontent": "1.1.1.
-0000c710: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
-0000c720: 2020 2020 2020 2020 2270 726f 7869 6162          "proxiab
-0000c730: 6c65 223a 2054 7275 652c 0a20 2020 2020  le": True,.     
-0000c740: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c750: 7072 6f78 6965 6422 3a20 5472 7565 2c0a  proxied": True,.
-0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c770: 2020 2020 2274 746c 223a 2033 3030 2c0a      "ttl": 300,.
-0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c790: 2020 2020 226c 6f63 6b65 6422 3a20 4661      "locked": Fa
-0000c7a0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-0000c7b0: 2020 2020 2020 2020 2022 7a6f 6e65 5f69           "zone_i
-0000c7c0: 6422 3a20 2266 6631 3261 6233 3463 6435  d": "ff12ab34cd5
-0000c7d0: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
-0000c7e0: 3937 3635 3022 2c0a 2020 2020 2020 2020  97650",.        
-0000c7f0: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
-0000c800: 655f 6e61 6d65 223a 2022 756e 6974 2e74  e_name": "unit.t
-0000c810: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
-0000c820: 2020 2020 2020 2020 2020 2022 6d6f 6469             "modi
-0000c830: 6669 6564 5f6f 6e22 3a20 2232 3031 372d  fied_on": "2017-
-0000c840: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
-0000c850: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
-0000c860: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
-0000c870: 6561 7465 645f 6f6e 223a 2022 3230 3137  eated_on": "2017
-0000c880: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
-0000c890: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
-0000c8a0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-0000c8b0: 6574 6122 3a20 7b22 6175 746f 5f61 6464  eta": {"auto_add
-0000c8c0: 6564 223a 2046 616c 7365 7d2c 0a20 2020  ed": False},.   
-0000c8d0: 2020 2020 2020 2020 2020 2020 207d 2c0a               },.
-0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c8f0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0000c900: 2020 2020 2020 2269 6422 3a20 2266 6331        "id": "fc1
-0000c910: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
-0000c920: 3261 6233 3332 3239 3937 3634 3222 2c0a  2ab3322997642",.
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c940: 2020 2020 2274 7970 6522 3a20 2241 4141      "type": "AAA
-0000c950: 4122 2c0a 2020 2020 2020 2020 2020 2020  A",.            
-0000c960: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-0000c970: 226d 756c 7469 2e75 6e69 742e 7465 7374  "multi.unit.test
-0000c980: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-0000c990: 2020 2020 2020 2020 2263 6f6e 7465 6e74          "content
-0000c9a0: 223a 2022 3a3a 3122 2c0a 2020 2020 2020  ": "::1",.      
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-0000c9c0: 726f 7869 6162 6c65 223a 2054 7275 652c  roxiable": True,
-0000c9d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c9e0: 2020 2020 2022 7072 6f78 6965 6422 3a20       "proxied": 
-0000c9f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000ca00: 2020 2020 2020 2020 2020 2274 746c 223a            "ttl":
-0000ca10: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
-0000ca20: 2020 2020 2020 2020 2020 226c 6f63 6b65            "locke
-0000ca30: 6422 3a20 4661 6c73 652c 0a20 2020 2020  d": False,.     
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000ca50: 7a6f 6e65 5f69 6422 3a20 2266 6631 3261  zone_id": "ff12a
-0000ca60: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-0000ca70: 6233 3332 3239 3937 3635 3022 2c0a 2020  b3322997650",.  
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2020 227a 6f6e 655f 6e61 6d65 223a 2022    "zone_name": "
-0000caa0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 2022 6d6f 6469 6669 6564 5f6f 6e22 3a20   "modified_on": 
-0000cad0: 2232 3031 372d 3033 2d31 3154 3138 3a30  "2017-03-11T18:0
-0000cae0: 313a 3433 2e34 3230 3638 395a 222c 0a20  1:43.420689Z",. 
-0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb00: 2020 2022 6372 6561 7465 645f 6f6e 223a     "created_on":
-0000cb10: 2022 3230 3137 2d30 332d 3131 5431 383a   "2017-03-11T18:
-0000cb20: 3031 3a34 332e 3432 3036 3839 5a22 2c0a  01:43.420689Z",.
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb40: 2020 2020 226d 6574 6122 3a20 7b22 6175      "meta": {"au
-0000cb50: 746f 5f61 6464 6564 223a 2046 616c 7365  to_added": False
-0000cb60: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-0000cb70: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-0000cb80: 2020 5d0a 2020 2020 2020 2020 290a 0a20    ].        ).. 
-0000cb90: 2020 2020 2020 207a 6f6e 6520 3d20 5a6f         zone = Zo
-0000cba0: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
-0000cbb0: 2c20 5b5d 290a 2020 2020 2020 2020 7072  , []).        pr
-0000cbc0: 6f76 6964 6572 2e70 6f70 756c 6174 6528  ovider.populate(
-0000cbd0: 7a6f 6e65 290a 0a20 2020 2020 2020 2023  zone)..        #
-0000cbe0: 2074 6865 2074 776f 2041 2072 6563 6f72   the two A recor
-0000cbf0: 6473 2067 6574 206d 6572 6765 6420 696e  ds get merged in
-0000cc00: 746f 206f 6e65 2043 4e41 4d45 2072 6563  to one CNAME rec
-0000cc10: 6f72 6420 706f 696e 7469 6e67 2074 6f0a  ord pointing to.
-0000cc20: 2020 2020 2020 2020 2320 7468 6520 4344          # the CD
-0000cc30: 4e2e 0a20 2020 2020 2020 2073 656c 662e  N..        self.
-0000cc40: 6173 7365 7274 4571 7561 6c28 332c 206c  assertEqual(3, l
-0000cc50: 656e 287a 6f6e 652e 7265 636f 7264 7329  en(zone.records)
-0000cc60: 290a 0a20 2020 2020 2020 206f 7264 6572  )..        order
-0000cc70: 6564 203d 2073 6f72 7465 6428 7a6f 6e65  ed = sorted(zone
-0000cc80: 2e72 6563 6f72 6473 2c20 6b65 793d 6c61  .records, key=la
-0000cc90: 6d62 6461 2072 3a20 722e 6e61 6d65 290a  mbda r: r.name).
-0000cca0: 0a20 2020 2020 2020 2072 6563 6f72 6420  .        record 
-0000ccb0: 3d20 6f72 6465 7265 645b 305d 0a20 2020  = ordered[0].   
-0000ccc0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000ccd0: 4571 7561 6c28 2761 272c 2072 6563 6f72  Equal('a', recor
-0000cce0: 642e 6e61 6d65 290a 2020 2020 2020 2020  d.name).        
-0000ccf0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-0000cd00: 2827 612e 756e 6974 2e74 6573 7473 2e27  ('a.unit.tests.'
-0000cd10: 2c20 7265 636f 7264 2e66 7164 6e29 0a20  , record.fqdn). 
-0000cd20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000cd30: 7274 4571 7561 6c28 2743 4e41 4d45 272c  rtEqual('CNAME',
-0000cd40: 2072 6563 6f72 642e 5f74 7970 6529 0a20   record._type). 
-0000cd50: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000cd60: 7274 4571 7561 6c28 2761 2e75 6e69 742e  rtEqual('a.unit.
-0000cd70: 7465 7374 732e 6364 6e2e 636c 6f75 6466  tests.cdn.cloudf
-0000cd80: 6c61 7265 2e6e 6574 2e27 2c20 7265 636f  lare.net.', reco
-0000cd90: 7264 2e76 616c 7565 290a 0a20 2020 2020  rd.value)..     
-0000cda0: 2020 2072 6563 6f72 6420 3d20 6f72 6465     record = orde
-0000cdb0: 7265 645b 315d 0a20 2020 2020 2020 2073  red[1].        s
-0000cdc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000cdd0: 2763 6e61 6d65 272c 2072 6563 6f72 642e  'cname', record.
-0000cde0: 6e61 6d65 290a 2020 2020 2020 2020 7365  name).        se
-0000cdf0: 6c66 2e61 7373 6572 7445 7175 616c 2827  lf.assertEqual('
-0000ce00: 636e 616d 652e 756e 6974 2e74 6573 7473  cname.unit.tests
-0000ce10: 2e27 2c20 7265 636f 7264 2e66 7164 6e29  .', record.fqdn)
-0000ce20: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000ce30: 7365 7274 4571 7561 6c28 2743 4e41 4d45  sertEqual('CNAME
-0000ce40: 272c 2072 6563 6f72 642e 5f74 7970 6529  ', record._type)
-0000ce50: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000ce60: 7365 7274 4571 7561 6c28 2763 6e61 6d65  sertEqual('cname
-0000ce70: 2e75 6e69 742e 7465 7374 732e 6364 6e2e  .unit.tests.cdn.
-0000ce80: 636c 6f75 6466 6c61 7265 2e6e 6574 2e27  cloudflare.net.'
-0000ce90: 2c20 7265 636f 7264 2e76 616c 7565 290a  , record.value).
-0000cea0: 0a20 2020 2020 2020 2072 6563 6f72 6420  .        record 
-0000ceb0: 3d20 6f72 6465 7265 645b 325d 0a20 2020  = ordered[2].   
-0000cec0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000ced0: 4571 7561 6c28 276d 756c 7469 272c 2072  Equal('multi', r
-0000cee0: 6563 6f72 642e 6e61 6d65 290a 2020 2020  ecord.name).    
-0000cef0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-0000cf00: 7175 616c 2827 6d75 6c74 692e 756e 6974  qual('multi.unit
-0000cf10: 2e74 6573 7473 2e27 2c20 7265 636f 7264  .tests.', record
-0000cf20: 2e66 7164 6e29 0a20 2020 2020 2020 2073  .fqdn).        s
-0000cf30: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000cf40: 2743 4e41 4d45 272c 2072 6563 6f72 642e  'CNAME', record.
-0000cf50: 5f74 7970 6529 0a20 2020 2020 2020 2073  _type).        s
-0000cf60: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-0000cf70: 276d 756c 7469 2e75 6e69 742e 7465 7374  'multi.unit.test
-0000cf80: 732e 6364 6e2e 636c 6f75 6466 6c61 7265  s.cdn.cloudflare
-0000cf90: 2e6e 6574 2e27 2c20 7265 636f 7264 2e76  .net.', record.v
-0000cfa0: 616c 7565 290a 0a20 2020 2020 2020 2023  alue)..        #
-0000cfb0: 2043 444e 2065 6e61 626c 6564 2072 6563   CDN enabled rec
-0000cfc0: 6f72 6473 2063 616e 2774 2062 6520 7570  ords can't be up
-0000cfd0: 6461 7465 642c 2077 6520 646f 6e27 7420  dated, we don't 
-0000cfe0: 6b6e 6f77 2074 6865 2072 6561 6c20 7661  know the real va
-0000cff0: 6c75 6573 0a20 2020 2020 2020 2023 206e  lues.        # n
-0000d000: 6576 6572 2070 6f69 6e74 2061 2043 6c6f  ever point a Clo
-0000d010: 7564 666c 6172 6520 7265 636f 7264 2074  udflare record t
-0000d020: 6f20 6974 7365 6c66 2e0a 2020 2020 2020  o itself..      
-0000d030: 2020 7761 6e74 6564 203d 205a 6f6e 6528    wanted = Zone(
-0000d040: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-0000d050: 5d29 0a20 2020 2020 2020 2077 616e 7465  ]).        wante
-0000d060: 642e 6164 645f 7265 636f 7264 280a 2020  d.add_record(.  
-0000d070: 2020 2020 2020 2020 2020 5265 636f 7264            Record
-0000d080: 2e6e 6577 280a 2020 2020 2020 2020 2020  .new(.          
-0000d090: 2020 2020 2020 7761 6e74 6564 2c0a 2020        wanted,.  
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2763                'c
-0000d0b0: 6e61 6d65 272c 0a20 2020 2020 2020 2020  name',.         
-0000d0c0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-0000d0d0: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
-0000d0e0: 6c27 3a20 3330 302c 0a20 2020 2020 2020  l': 300,.       
-0000d0f0: 2020 2020 2020 2020 2020 2020 2027 7479               'ty
-0000d100: 7065 273a 2027 434e 414d 4527 2c0a 2020  pe': 'CNAME',.  
-0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2020 2776 616c 7565 273a 2027 6368 616e    'value': 'chan
-0000d130: 6765 2e75 6e69 742e 7465 7374 732e 6364  ge.unit.tests.cd
-0000d140: 6e2e 636c 6f75 6466 6c61 7265 2e6e 6574  n.cloudflare.net
-0000d150: 2e27 2c0a 2020 2020 2020 2020 2020 2020  .',.            
-0000d160: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
-0000d170: 2020 2029 0a20 2020 2020 2020 2029 0a20     ).        ). 
-0000d180: 2020 2020 2020 2077 616e 7465 642e 6164         wanted.ad
-0000d190: 645f 7265 636f 7264 280a 2020 2020 2020  d_record(.      
-0000d1a0: 2020 2020 2020 5265 636f 7264 2e6e 6577        Record.new
-0000d1b0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d1c0: 2020 7761 6e74 6564 2c0a 2020 2020 2020    wanted,.      
-0000d1d0: 2020 2020 2020 2020 2020 276e 6577 272c            'new',
-0000d1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d1f0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-0000d200: 2020 2020 2020 2027 7474 6c27 3a20 3330         'ttl': 30
-0000d210: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0000d220: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
-0000d230: 434e 414d 4527 2c0a 2020 2020 2020 2020  CNAME',.        
-0000d240: 2020 2020 2020 2020 2020 2020 2776 616c              'val
-0000d250: 7565 273a 2027 6e65 772e 756e 6974 2e74  ue': 'new.unit.t
-0000d260: 6573 7473 2e63 646e 2e63 6c6f 7564 666c  ests.cdn.cloudfl
-0000d270: 6172 652e 6e65 742e 272c 0a20 2020 2020  are.net.',.     
-0000d280: 2020 2020 2020 2020 2020 207d 2c0a 2020             },.  
-0000d290: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000d2a0: 2020 2020 290a 2020 2020 2020 2020 7761      ).        wa
-0000d2b0: 6e74 6564 2e61 6464 5f72 6563 6f72 6428  nted.add_record(
-0000d2c0: 0a20 2020 2020 2020 2020 2020 2052 6563  .            Rec
-0000d2d0: 6f72 642e 6e65 7728 0a20 2020 2020 2020  ord.new(.       
-0000d2e0: 2020 2020 2020 2020 2077 616e 7465 642c           wanted,
-0000d2f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d300: 2027 6372 6561 7465 6427 2c0a 2020 2020   'created',.    
-0000d310: 2020 2020 2020 2020 2020 2020 7b27 7474              {'tt
-0000d320: 6c27 3a20 3330 302c 2027 7479 7065 273a  l': 300, 'type':
-0000d330: 2027 434e 414d 4527 2c20 2776 616c 7565   'CNAME', 'value
-0000d340: 273a 2027 7777 772e 756e 6974 2e74 6573  ': 'www.unit.tes
-0000d350: 7473 2e27 7d2c 0a20 2020 2020 2020 2020  ts.'},.         
-0000d360: 2020 2029 0a20 2020 2020 2020 2029 0a0a     ).        )..
-0000d370: 2020 2020 2020 2020 706c 616e 203d 2070          plan = p
-0000d380: 726f 7669 6465 722e 706c 616e 2877 616e  rovider.plan(wan
-0000d390: 7465 6429 0a20 2020 2020 2020 2073 656c  ted).        sel
-0000d3a0: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
-0000d3b0: 206c 656e 2870 6c61 6e2e 6368 616e 6765   len(plan.change
-0000d3c0: 7329 290a 0a20 2020 2064 6566 2074 6573  s))..    def tes
-0000d3d0: 745f 6364 6e5f 616c 6961 7328 7365 6c66  t_cdn_alias(self
-0000d3e0: 293a 0a20 2020 2020 2020 2070 726f 7669  ):.        provi
-0000d3f0: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
-0000d400: 5072 6f76 6964 6572 280a 2020 2020 2020  Provider(.      
-0000d410: 2020 2020 2020 2774 6573 7427 2c20 2765        'test', 'e
-0000d420: 6d61 696c 272c 2027 746f 6b65 6e27 2c20  mail', 'token', 
-0000d430: 2761 6363 6f75 6e74 5f69 6427 2c20 5472  'account_id', Tr
-0000d440: 7565 0a20 2020 2020 2020 2029 0a0a 2020  ue.        )..  
-0000d450: 2020 2020 2020 2320 4120 434e 414d 4520        # A CNAME 
-0000d460: 666f 7220 7573 2074 6f20 7472 616e 7366  for us to transf
-0000d470: 6f72 6d20 746f 2041 4c49 4153 0a20 2020  orm to ALIAS.   
-0000d480: 2020 2020 2070 726f 7669 6465 722e 7a6f       provider.zo
-0000d490: 6e65 5f72 6563 6f72 6473 203d 204d 6f63  ne_records = Moc
-0000d4a0: 6b28 0a20 2020 2020 2020 2020 2020 2072  k(.            r
-0000d4b0: 6574 7572 6e5f 7661 6c75 653d 5b0a 2020  eturn_value=[.  
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 2020 2020 2269 6422 3a20 2266 6331 3261      "id": "fc12a
-0000d4f0: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-0000d500: 6233 3332 3239 3937 3634 3222 2c0a 2020  b3322997642",.  
-0000d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d520: 2020 2274 7970 6522 3a20 2243 4e41 4d45    "type": "CNAME
-0000d530: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000d540: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
-0000d550: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-0000d560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d570: 2022 636f 6e74 656e 7422 3a20 2277 7777   "content": "www
-0000d580: 2e75 6e69 742e 7465 7374 7322 2c0a 2020  .unit.tests",.  
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 2270 726f 7869 6162 6c65 223a 2054    "proxiable": T
-0000d5b0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0000d5c0: 2020 2020 2020 2020 2022 7072 6f78 6965           "proxie
-0000d5d0: 6422 3a20 5472 7565 2c0a 2020 2020 2020  d": True,.      
-0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-0000d5f0: 746c 223a 2033 3030 2c0a 2020 2020 2020  tl": 300,.      
-0000d600: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-0000d610: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d630: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
-0000d640: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
-0000d650: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
-0000d660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d670: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
-0000d680: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
-0000d690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d6a0: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
-0000d6b0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
-0000d6c0: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
-0000d6d0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000d6e0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-0000d6f0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
-0000d700: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
-0000d710: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-0000d720: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
-0000d730: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
-0000d740: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-0000d750: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0000d760: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
-0000d770: 0a0a 2020 2020 2020 2020 7a6f 6e65 203d  ..        zone =
-0000d780: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
-0000d790: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
-0000d7a0: 2070 726f 7669 6465 722e 706f 7075 6c61   provider.popula
-0000d7b0: 7465 287a 6f6e 6529 0a20 2020 2020 2020  te(zone).       
-0000d7c0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000d7d0: 6c28 312c 206c 656e 287a 6f6e 652e 7265  l(1, len(zone.re
-0000d7e0: 636f 7264 7329 290a 2020 2020 2020 2020  cords)).        
-0000d7f0: 7265 636f 7264 203d 206c 6973 7428 7a6f  record = list(zo
-0000d800: 6e65 2e72 6563 6f72 6473 295b 305d 0a20  ne.records)[0]. 
-0000d810: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000d820: 7274 4571 7561 6c28 2727 2c20 7265 636f  rtEqual('', reco
-0000d830: 7264 2e6e 616d 6529 0a20 2020 2020 2020  rd.name).       
-0000d840: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
-0000d850: 6c28 2775 6e69 742e 7465 7374 732e 272c  l('unit.tests.',
-0000d860: 2072 6563 6f72 642e 6671 646e 290a 2020   record.fqdn).  
-0000d870: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000d880: 7445 7175 616c 2827 414c 4941 5327 2c20  tEqual('ALIAS', 
-0000d890: 7265 636f 7264 2e5f 7479 7065 290a 2020  record._type).  
-0000d8a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-0000d8b0: 7445 7175 616c 2827 756e 6974 2e74 6573  tEqual('unit.tes
-0000d8c0: 7473 2e63 646e 2e63 6c6f 7564 666c 6172  ts.cdn.cloudflar
-0000d8d0: 652e 6e65 742e 272c 2072 6563 6f72 642e  e.net.', record.
-0000d8e0: 7661 6c75 6529 0a0a 2020 2020 2020 2020  value)..        
-0000d8f0: 2320 4344 4e20 656e 6162 6c65 6420 7265  # CDN enabled re
-0000d900: 636f 7264 7320 6361 6e27 7420 6265 2075  cords can't be u
-0000d910: 7064 6174 6564 2c20 7765 2064 6f6e 2774  pdated, we don't
-0000d920: 206b 6e6f 7720 7468 6520 7265 616c 2076   know the real v
-0000d930: 616c 7565 730a 2020 2020 2020 2020 2320  alues.        # 
-0000d940: 6e65 7665 7220 706f 696e 7420 6120 436c  never point a Cl
-0000d950: 6f75 6466 6c61 7265 2072 6563 6f72 6420  oudflare record 
-0000d960: 746f 2069 7473 656c 662e 0a20 2020 2020  to itself..     
-0000d970: 2020 2077 616e 7465 6420 3d20 5a6f 6e65     wanted = Zone
-0000d980: 2827 756e 6974 2e74 6573 7473 2e27 2c20  ('unit.tests.', 
-0000d990: 5b5d 290a 2020 2020 2020 2020 7761 6e74  []).        want
-0000d9a0: 6564 2e61 6464 5f72 6563 6f72 6428 0a20  ed.add_record(. 
-0000d9b0: 2020 2020 2020 2020 2020 2052 6563 6f72             Recor
-0000d9c0: 642e 6e65 7728 0a20 2020 2020 2020 2020  d.new(.         
-0000d9d0: 2020 2020 2020 2077 616e 7465 642c 0a20         wanted,. 
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-0000d9f0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0000da00: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-0000da10: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
-0000da20: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
-0000da30: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
-0000da40: 2027 414c 4941 5327 2c0a 2020 2020 2020   'ALIAS',.      
-0000da50: 2020 2020 2020 2020 2020 2020 2020 2776                'v
-0000da60: 616c 7565 273a 2027 6368 616e 6765 2e75  alue': 'change.u
-0000da70: 6e69 742e 7465 7374 732e 6364 6e2e 636c  nit.tests.cdn.cl
-0000da80: 6f75 6466 6c61 7265 2e6e 6574 2e27 2c0a  oudflare.net.',.
-0000da90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000daa0: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
-0000dab0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000dac0: 2020 2020 706c 616e 203d 2070 726f 7669      plan = provi
-0000dad0: 6465 722e 706c 616e 2877 616e 7465 6429  der.plan(wanted)
-0000dae0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000daf0: 7365 7274 4571 7561 6c28 4661 6c73 652c  sertEqual(False,
-0000db00: 2068 6173 6174 7472 2870 6c61 6e2c 2027   hasattr(plan, '
-0000db10: 6368 616e 6765 7327 2929 0a0a 2020 2020  changes'))..    
-0000db20: 6465 6620 7465 7374 5f75 6e70 726f 7869  def test_unproxi
-0000db30: 6162 6c65 7479 7065 5f72 6563 6f72 6466  abletype_recordf
-0000db40: 6f72 5f72 6574 7572 6e73 7265 636f 7264  or_returnsrecord
-0000db50: 7769 7468 6e6f 636c 6f75 6466 6c61 7265  withnocloudflare
-0000db60: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000db70: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
-0000db80: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
-0000db90: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
-0000dba0: 746f 6b65 6e27 290a 2020 2020 2020 2020  token').        
-0000dbb0: 6e61 6d65 203d 2022 756e 6974 2e74 6573  name = "unit.tes
-0000dbc0: 7473 220a 2020 2020 2020 2020 5f74 7970  ts".        _typ
-0000dbd0: 6520 3d20 224e 5322 0a20 2020 2020 2020  e = "NS".       
-0000dbe0: 207a 6f6e 655f 7265 636f 7264 7320 3d20   zone_records = 
-0000dbf0: 5b0a 2020 2020 2020 2020 2020 2020 7b0a  [.            {.
-0000dc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc10: 2269 6422 3a20 2266 6331 3261 6233 3463  "id": "fc12ab34c
-0000dc20: 6435 3631 3133 3334 3432 3261 6233 3332  d5611334422ab332
-0000dc30: 3239 3937 3635 3422 2c0a 2020 2020 2020  2997654",.      
-0000dc40: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
-0000dc50: 3a20 5f74 7970 652c 0a20 2020 2020 2020  : _type,.       
-0000dc60: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-0000dc70: 206e 616d 652c 0a20 2020 2020 2020 2020   name,.         
-0000dc80: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
-0000dc90: 3a20 226e 7332 2e66 6f6f 2e62 6172 222c  : "ns2.foo.bar",
-0000dca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dcb0: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
-0000dcc0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-0000dcd0: 2020 2020 2270 726f 7869 6564 223a 2046      "proxied": F
-0000dce0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-0000dcf0: 2020 2020 2020 2274 746c 223a 2033 3030        "ttl": 300
-0000dd00: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dd10: 2020 226c 6f63 6b65 6422 3a20 4661 6c73    "locked": Fals
-0000dd20: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000dd30: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
-0000dd40: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
-0000dd50: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
-0000dd60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000dd70: 2020 227a 6f6e 655f 6e61 6d65 223a 2022    "zone_name": "
-0000dd80: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-0000dd90: 2020 2020 2020 2020 2020 2020 2022 6d6f               "mo
-0000dda0: 6469 6669 6564 5f6f 6e22 3a20 2232 3031  dified_on": "201
-0000ddb0: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
-0000ddc0: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
-0000ddd0: 2020 2020 2020 2020 2020 2022 6372 6561             "crea
-0000dde0: 7465 645f 6f6e 223a 2022 3230 3137 2d30  ted_on": "2017-0
-0000ddf0: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
-0000de00: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
-0000de10: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
-0000de20: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
-0000de30: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-0000de40: 2020 207d 0a20 2020 2020 2020 205d 0a20     }.        ]. 
-0000de50: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-0000de60: 7a6f 6e65 5f72 6563 6f72 6473 203d 204d  zone_records = M
-0000de70: 6f63 6b28 7265 7475 726e 5f76 616c 7565  ock(return_value
-0000de80: 3d7a 6f6e 655f 7265 636f 7264 7329 0a20  =zone_records). 
-0000de90: 2020 2020 2020 207a 6f6e 6520 3d20 5a6f         zone = Zo
-0000dea0: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
-0000deb0: 2c20 5b5d 290a 2020 2020 2020 2020 7072  , []).        pr
-0000dec0: 6f76 6964 6572 2e70 6f70 756c 6174 6528  ovider.populate(
-0000ded0: 7a6f 6e65 290a 0a20 2020 2020 2020 2072  zone)..        r
-0000dee0: 6563 6f72 6420 3d20 7072 6f76 6964 6572  ecord = provider
-0000def0: 2e5f 7265 636f 7264 5f66 6f72 287a 6f6e  ._record_for(zon
-0000df00: 652c 206e 616d 652c 205f 7479 7065 2c20  e, name, _type, 
-0000df10: 7a6f 6e65 5f72 6563 6f72 6473 2c20 4661  zone_records, Fa
-0000df20: 6c73 6529 0a0a 2020 2020 2020 2020 7365  lse)..        se
-0000df30: 6c66 2e61 7373 6572 7446 616c 7365 2872  lf.assertFalse(r
-0000df40: 6563 6f72 642e 5f6f 6374 6f64 6e73 2e67  ecord._octodns.g
-0000df50: 6574 2827 6175 746f 2d74 746c 272c 2046  et('auto-ttl', F
-0000df60: 616c 7365 2929 0a20 2020 2020 2020 2073  alse)).        s
-0000df70: 656c 662e 6173 7365 7274 4661 6c73 6528  elf.assertFalse(
-0000df80: 7265 636f 7264 2e5f 6f63 746f 646e 732e  record._octodns.
-0000df90: 6765 7428 2770 726f 7869 6564 272c 2046  get('proxied', F
-0000dfa0: 616c 7365 2929 0a0a 2020 2020 6465 6620  alse))..    def 
-0000dfb0: 7465 7374 5f70 726f 7869 6162 6c65 7479  test_proxiablety
-0000dfc0: 7065 5f72 6563 6f72 6466 6f72 5f72 6574  pe_recordfor_ret
-0000dfd0: 7265 636f 7264 7769 7468 636c 6f75 6466  recordwithcloudf
-0000dfe0: 6c61 7265 756e 7072 6f78 6965 6428 7365  lareunproxied(se
-0000dff0: 6c66 293a 0a20 2020 2020 2020 2070 726f  lf):.        pro
-0000e000: 7669 6465 7220 3d20 436c 6f75 6466 6c61  vider = Cloudfla
-0000e010: 7265 5072 6f76 6964 6572 2827 7465 7374  reProvider('test
-0000e020: 272c 2027 656d 6169 6c27 2c20 2774 6f6b  ', 'email', 'tok
-0000e030: 656e 2729 0a20 2020 2020 2020 206e 616d  en').        nam
-0000e040: 6520 3d20 226d 756c 7469 2e75 6e69 742e  e = "multi.unit.
-0000e050: 7465 7374 7322 0a20 2020 2020 2020 205f  tests".        _
-0000e060: 7479 7065 203d 2022 4141 4141 220a 2020  type = "AAAA".  
-0000e070: 2020 2020 2020 7a6f 6e65 5f72 6563 6f72        zone_recor
-0000e080: 6473 203d 205b 0a20 2020 2020 2020 2020  ds = [.         
-0000e090: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-0000e0a0: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
-0000e0b0: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-0000e0c0: 6162 3333 3232 3939 3736 3432 222c 0a20  ab3322997642",. 
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e0e0: 7479 7065 223a 205f 7479 7065 2c0a 2020  type": _type,.  
-0000e0f0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-0000e100: 616d 6522 3a20 6e61 6d65 2c0a 2020 2020  ame": name,.    
-0000e110: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
-0000e120: 7465 6e74 223a 2022 3a3a 3122 2c0a 2020  tent": "::1",.  
-0000e130: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-0000e140: 726f 7869 6162 6c65 223a 2054 7275 652c  roxiable": True,
-0000e150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e160: 2022 7072 6f78 6965 6422 3a20 4661 6c73   "proxied": Fals
-0000e170: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000e180: 2020 2022 7474 6c22 3a20 3330 302c 0a20     "ttl": 300,. 
-0000e190: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e1a0: 6c6f 636b 6564 223a 2046 616c 7365 2c0a  locked": False,.
-0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e1c0: 227a 6f6e 655f 6964 223a 2022 6666 3132  "zone_id": "ff12
-0000e1d0: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-0000e1e0: 6162 3333 3232 3939 3736 3530 222c 0a20  ab3322997650",. 
-0000e1f0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e200: 7a6f 6e65 5f6e 616d 6522 3a20 2275 6e69  zone_name": "uni
-0000e210: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
-0000e220: 2020 2020 2020 2020 2020 226d 6f64 6966            "modif
-0000e230: 6965 645f 6f6e 223a 2022 3230 3137 2d30  ied_on": "2017-0
-0000e240: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
-0000e250: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
-0000e260: 2020 2020 2020 2020 2263 7265 6174 6564          "created
-0000e270: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
-0000e280: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
-0000e290: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
-0000e2a0: 2020 2020 2022 6d65 7461 223a 207b 2261       "meta": {"a
-0000e2b0: 7574 6f5f 6164 6465 6422 3a20 4661 6c73  uto_added": Fals
-0000e2c0: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
-0000e2d0: 7d0a 2020 2020 2020 2020 5d0a 2020 2020  }.        ].    
-0000e2e0: 2020 2020 7072 6f76 6964 6572 2e7a 6f6e      provider.zon
-0000e2f0: 655f 7265 636f 7264 7320 3d20 4d6f 636b  e_records = Mock
-0000e300: 2872 6574 7572 6e5f 7661 6c75 653d 7a6f  (return_value=zo
-0000e310: 6e65 5f72 6563 6f72 6473 290a 2020 2020  ne_records).    
-0000e320: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
-0000e330: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-0000e340: 5d29 0a20 2020 2020 2020 2070 726f 7669  ]).        provi
-0000e350: 6465 722e 706f 7075 6c61 7465 287a 6f6e  der.populate(zon
-0000e360: 6529 0a0a 2020 2020 2020 2020 7265 636f  e)..        reco
-0000e370: 7264 203d 2070 726f 7669 6465 722e 5f72  rd = provider._r
-0000e380: 6563 6f72 645f 666f 7228 7a6f 6e65 2c20  ecord_for(zone, 
-0000e390: 6e61 6d65 2c20 5f74 7970 652c 207a 6f6e  name, _type, zon
-0000e3a0: 655f 7265 636f 7264 732c 2046 616c 7365  e_records, False
-0000e3b0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-0000e3c0: 6173 7365 7274 4661 6c73 6528 0a20 2020  assertFalse(.   
-0000e3d0: 2020 2020 2020 2020 2072 6563 6f72 642e           record.
-0000e3e0: 5f6f 6374 6f64 6e73 2e67 6574 2827 636c  _octodns.get('cl
-0000e3f0: 6f75 6466 6c61 7265 272c 207b 7d29 2e67  oudflare', {}).g
-0000e400: 6574 2827 7072 6f78 6965 6427 2c20 4661  et('proxied', Fa
-0000e410: 6c73 6529 0a20 2020 2020 2020 2029 0a0a  lse).        )..
-0000e420: 2020 2020 6465 6620 7465 7374 5f70 726f      def test_pro
-0000e430: 7869 6162 6c65 7479 7065 5f72 6563 6f72  xiabletype_recor
-0000e440: 6466 6f72 5f72 6574 7572 6e73 7265 636f  dfor_returnsreco
-0000e450: 7264 7769 7468 636c 6f75 6466 6c61 7265  rdwithcloudflare
-0000e460: 7072 6f78 6965 6428 7365 6c66 293a 0a20  proxied(self):. 
-0000e470: 2020 2020 2020 2070 726f 7669 6465 7220         provider 
-0000e480: 3d20 436c 6f75 6466 6c61 7265 5072 6f76  = CloudflareProv
-0000e490: 6964 6572 2827 7465 7374 272c 2027 656d  ider('test', 'em
-0000e4a0: 6169 6c27 2c20 2774 6f6b 656e 2729 0a20  ail', 'token'). 
-0000e4b0: 2020 2020 2020 206e 616d 6520 3d20 226d         name = "m
-0000e4c0: 756c 7469 2e75 6e69 742e 7465 7374 7322  ulti.unit.tests"
-0000e4d0: 0a20 2020 2020 2020 205f 7479 7065 203d  .        _type =
-0000e4e0: 2022 4141 4141 220a 2020 2020 2020 2020   "AAAA".        
-0000e4f0: 7a6f 6e65 5f72 6563 6f72 6473 203d 205b  zone_records = [
-0000e500: 0a20 2020 2020 2020 2020 2020 207b 0a20  .            {. 
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e520: 6964 223a 2022 6663 3132 6162 3334 6364  id": "fc12ab34cd
-0000e530: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
-0000e540: 3939 3736 3432 222c 0a20 2020 2020 2020  997642",.       
-0000e550: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-0000e560: 205f 7479 7065 2c0a 2020 2020 2020 2020   _type,.        
-0000e570: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-0000e580: 6e61 6d65 2c0a 2020 2020 2020 2020 2020  name,.          
-0000e590: 2020 2020 2020 2263 6f6e 7465 6e74 223a        "content":
-0000e5a0: 2022 3a3a 3122 2c0a 2020 2020 2020 2020   "::1",.        
-0000e5b0: 2020 2020 2020 2020 2270 726f 7869 6162          "proxiab
-0000e5c0: 6c65 223a 2054 7275 652c 0a20 2020 2020  le": True,.     
-0000e5d0: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
-0000e5e0: 6965 6422 3a20 5472 7565 2c0a 2020 2020  ied": True,.    
-0000e5f0: 2020 2020 2020 2020 2020 2020 2274 746c              "ttl
-0000e600: 223a 2031 2c0a 2020 2020 2020 2020 2020  ": 1,.          
-0000e610: 2020 2020 2020 226c 6f63 6b65 6422 3a20        "locked": 
-0000e620: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-0000e630: 2020 2020 2020 2022 7a6f 6e65 5f69 6422         "zone_id"
-0000e640: 3a20 2266 6631 3261 6233 3463 6435 3631  : "ff12ab34cd561
-0000e650: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
-0000e660: 3635 3022 2c0a 2020 2020 2020 2020 2020  650",.          
-0000e670: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
-0000e680: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
-0000e690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e6a0: 2022 6d6f 6469 6669 6564 5f6f 6e22 3a20   "modified_on": 
-0000e6b0: 2232 3031 372d 3033 2d31 3154 3138 3a30  "2017-03-11T18:0
-0000e6c0: 313a 3433 2e34 3230 3638 395a 222c 0a20  1:43.420689Z",. 
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e6e0: 6372 6561 7465 645f 6f6e 223a 2022 3230  created_on": "20
-0000e6f0: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
-0000e700: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
-0000e710: 2020 2020 2020 2020 2020 2020 226d 6574              "met
-0000e720: 6122 3a20 7b22 6175 746f 5f61 6464 6564  a": {"auto_added
-0000e730: 223a 2046 616c 7365 7d2c 0a20 2020 2020  ": False},.     
-0000e740: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-0000e750: 205d 0a20 2020 2020 2020 2070 726f 7669   ].        provi
-0000e760: 6465 722e 7a6f 6e65 5f72 6563 6f72 6473  der.zone_records
-0000e770: 203d 204d 6f63 6b28 7265 7475 726e 5f76   = Mock(return_v
-0000e780: 616c 7565 3d7a 6f6e 655f 7265 636f 7264  alue=zone_record
-0000e790: 7329 0a20 2020 2020 2020 207a 6f6e 6520  s).        zone 
-0000e7a0: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
-0000e7b0: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
-0000e7c0: 2020 7072 6f76 6964 6572 2e70 6f70 756c    provider.popul
-0000e7d0: 6174 6528 7a6f 6e65 290a 0a20 2020 2020  ate(zone)..     
-0000e7e0: 2020 2072 6563 6f72 6420 3d20 7072 6f76     record = prov
-0000e7f0: 6964 6572 2e5f 7265 636f 7264 5f66 6f72  ider._record_for
-0000e800: 287a 6f6e 652c 206e 616d 652c 205f 7479  (zone, name, _ty
-0000e810: 7065 2c20 7a6f 6e65 5f72 6563 6f72 6473  pe, zone_records
-0000e820: 2c20 4661 6c73 6529 0a0a 2020 2020 2020  , False)..      
-0000e830: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
-0000e840: 6528 7265 636f 7264 2e5f 6f63 746f 646e  e(record._octodn
-0000e850: 735b 2763 6c6f 7564 666c 6172 6527 5d5b  s['cloudflare'][
-0000e860: 2761 7574 6f2d 7474 6c27 5d29 0a20 2020  'auto-ttl']).   
-0000e870: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000e880: 5472 7565 2872 6563 6f72 642e 5f6f 6374  True(record._oct
-0000e890: 6f64 6e73 5b27 636c 6f75 6466 6c61 7265  odns['cloudflare
-0000e8a0: 275d 5b27 7072 6f78 6965 6427 5d29 0a0a  ']['proxied'])..
-0000e8b0: 2020 2020 6465 6620 7465 7374 5f72 6563      def test_rec
-0000e8c0: 6f72 645f 666f 725f 6175 746f 5f74 746c  ord_for_auto_ttl
-0000e8d0: 5f6e 6f5f 7072 6f78 6965 6428 7365 6c66  _no_proxied(self
-0000e8e0: 293a 0a20 2020 2020 2020 2070 726f 7669  ):.        provi
-0000e8f0: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
-0000e900: 5072 6f76 6964 6572 2827 7465 7374 272c  Provider('test',
-0000e910: 2027 656d 6169 6c27 2c20 2774 6f6b 656e   'email', 'token
-0000e920: 2729 0a20 2020 2020 2020 206e 616d 6520  ').        name 
-0000e930: 3d20 2270 726f 7869 6564 2e75 6e69 742e  = "proxied.unit.
-0000e940: 7465 7374 7322 0a20 2020 2020 2020 205f  tests".        _
-0000e950: 7479 7065 203d 2022 4122 0a20 2020 2020  type = "A".     
-0000e960: 2020 207a 6f6e 655f 7265 636f 7264 7320     zone_records 
-0000e970: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-0000e980: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-0000e990: 2020 2269 6422 3a20 2266 6331 3261 6233    "id": "fc12ab3
-0000e9a0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
-0000e9b0: 3332 3239 3937 3634 3222 2c0a 2020 2020  322997642",.    
-0000e9c0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-0000e9d0: 6522 3a20 5f74 7970 652c 0a20 2020 2020  e": _type,.     
-0000e9e0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
-0000e9f0: 223a 206e 616d 652c 0a20 2020 2020 2020  ": name,.       
-0000ea00: 2020 2020 2020 2020 2022 636f 6e74 656e           "conten
-0000ea10: 7422 3a20 2234 2e33 2e32 2e31 222c 0a20  t": "4.3.2.1",. 
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000ea30: 7072 6f78 6961 626c 6522 3a20 5472 7565  proxiable": True
-0000ea40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ea50: 2020 2270 726f 7869 6564 223a 2046 616c    "proxied": Fal
-0000ea60: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-0000ea70: 2020 2020 2274 746c 223a 2031 2c0a 2020      "ttl": 1,.  
-0000ea80: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-0000ea90: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000eab0: 7a6f 6e65 5f69 6422 3a20 2266 6631 3261  zone_id": "ff12a
-0000eac0: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
-0000ead0: 6233 3332 3239 3937 3635 3022 2c0a 2020  b3322997650",.  
-0000eae0: 2020 2020 2020 2020 2020 2020 2020 227a                "z
-0000eaf0: 6f6e 655f 6e61 6d65 223a 2022 756e 6974  one_name": "unit
-0000eb00: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
-0000eb10: 2020 2020 2020 2020 2022 6d6f 6469 6669           "modifi
-0000eb20: 6564 5f6f 6e22 3a20 2232 3031 372d 3033  ed_on": "2017-03
-0000eb30: 2d31 3154 3138 3a30 313a 3433 2e34 3230  -11T18:01:43.420
-0000eb40: 3638 395a 222c 0a20 2020 2020 2020 2020  689Z",.         
-0000eb50: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-0000eb60: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
-0000eb70: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
-0000eb80: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-0000eb90: 2020 2020 226d 6574 6122 3a20 7b22 6175      "meta": {"au
-0000eba0: 746f 5f61 6464 6564 223a 2046 616c 7365  to_added": False
-0000ebb0: 7d2c 0a20 2020 2020 2020 2020 2020 207d  },.            }
-0000ebc0: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
-0000ebd0: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
-0000ebe0: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-0000ebf0: 5d29 0a20 2020 2020 2020 2072 6563 6f72  ]).        recor
-0000ec00: 6420 3d20 7072 6f76 6964 6572 2e5f 7265  d = provider._re
-0000ec10: 636f 7264 5f66 6f72 287a 6f6e 652c 206e  cord_for(zone, n
-0000ec20: 616d 652c 205f 7479 7065 2c20 7a6f 6e65  ame, _type, zone
-0000ec30: 5f72 6563 6f72 6473 2c20 4661 6c73 6529  _records, False)
-0000ec40: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-0000ec50: 7373 6572 7454 7275 6528 7265 636f 7264  ssertTrue(record
-0000ec60: 2e5f 6f63 746f 646e 735b 2763 6c6f 7564  ._octodns['cloud
-0000ec70: 666c 6172 6527 5d5b 2761 7574 6f2d 7474  flare']['auto-tt
-0000ec80: 6c27 5d29 0a20 2020 2020 2020 2073 656c  l']).        sel
-0000ec90: 662e 6173 7365 7274 4661 6c73 6528 7265  f.assertFalse(re
-0000eca0: 636f 7264 2e5f 6f63 746f 646e 735b 2763  cord._octodns['c
-0000ecb0: 6c6f 7564 666c 6172 6527 5d2e 6765 7428  loudflare'].get(
-0000ecc0: 2770 726f 7869 6564 272c 2046 616c 7365  'proxied', False
-0000ecd0: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
-0000ece0: 5f70 726f 7869 6564 7265 636f 7264 616e  _proxiedrecordan
-0000ecf0: 646e 6577 7474 6c5f 696e 636c 7564 6563  dnewttl_includec
-0000ed00: 6861 6e67 655f 7265 7475 726e 7366 616c  hange_returnsfal
-0000ed10: 7365 2873 656c 6629 3a0a 2020 2020 2020  se(self):.      
-0000ed20: 2020 7072 6f76 6964 6572 203d 2043 6c6f    provider = Clo
-0000ed30: 7564 666c 6172 6550 726f 7669 6465 7228  udflareProvider(
-0000ed40: 2774 6573 7427 2c20 2765 6d61 696c 272c  'test', 'email',
-0000ed50: 2027 746f 6b65 6e27 290a 2020 2020 2020   'token').      
-0000ed60: 2020 7a6f 6e65 203d 205a 6f6e 6528 2775    zone = Zone('u
-0000ed70: 6e69 742e 7465 7374 732e 272c 205b 5d29  nit.tests.', [])
-0000ed80: 0a20 2020 2020 2020 2065 7869 7374 696e  .        existin
-0000ed90: 6720 3d20 7365 745f 7265 636f 7264 5f70  g = set_record_p
-0000eda0: 726f 7869 6564 5f66 6c61 6728 0a20 2020  roxied_flag(.   
-0000edb0: 2020 2020 2020 2020 2052 6563 6f72 642e           Record.
-0000edc0: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
-0000edd0: 2020 2020 207a 6f6e 652c 0a20 2020 2020       zone,.     
-0000ede0: 2020 2020 2020 2020 2020 2027 6127 2c0a             'a',.
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee00: 7b27 7474 6c27 3a20 312c 2027 7479 7065  {'ttl': 1, 'type
-0000ee10: 273a 2027 4127 2c20 2776 616c 7565 7327  ': 'A', 'values'
-0000ee20: 3a20 5b27 312e 312e 312e 3127 2c20 2732  : ['1.1.1.1', '2
-0000ee30: 2e32 2e32 2e32 275d 7d2c 0a20 2020 2020  .2.2.2']},.     
-0000ee40: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-0000ee50: 2020 2020 2020 5472 7565 2c0a 2020 2020        True,.    
-0000ee60: 2020 2020 290a 2020 2020 2020 2020 6e65      ).        ne
-0000ee70: 7720 3d20 7365 745f 7265 636f 7264 5f70  w = set_record_p
-0000ee80: 726f 7869 6564 5f66 6c61 6728 0a20 2020  roxied_flag(.   
-0000ee90: 2020 2020 2020 2020 2052 6563 6f72 642e           Record.
-0000eea0: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
-0000eeb0: 2020 2020 207a 6f6e 652c 0a20 2020 2020       zone,.     
-0000eec0: 2020 2020 2020 2020 2020 2027 6127 2c0a             'a',.
-0000eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eee0: 7b27 7474 6c27 3a20 3330 302c 2027 7479  {'ttl': 300, 'ty
-0000eef0: 7065 273a 2027 4127 2c20 2776 616c 7565  pe': 'A', 'value
-0000ef00: 7327 3a20 5b27 312e 312e 312e 3127 2c20  s': ['1.1.1.1', 
-0000ef10: 2732 2e32 2e32 2e32 275d 7d2c 0a20 2020  '2.2.2.2']},.   
-0000ef20: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-0000ef30: 2020 2020 2020 2020 5472 7565 2c0a 2020          True,.  
-0000ef40: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000ef50: 6368 616e 6765 203d 2055 7064 6174 6528  change = Update(
-0000ef60: 6578 6973 7469 6e67 2c20 6e65 7729 0a0a  existing, new)..
-0000ef70: 2020 2020 2020 2020 696e 636c 7564 655f          include_
-0000ef80: 6368 616e 6765 203d 2070 726f 7669 6465  change = provide
-0000ef90: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
-0000efa0: 6528 6368 616e 6765 290a 0a20 2020 2020  e(change)..     
-0000efb0: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
-0000efc0: 6c73 6528 696e 636c 7564 655f 6368 616e  lse(include_chan
-0000efd0: 6765 290a 0a20 2020 2064 6566 2074 6573  ge)..    def tes
-0000efe0: 745f 6175 746f 5f74 746c 5f69 676e 6f72  t_auto_ttl_ignor
-0000eff0: 6573 5f74 746c 5f63 6861 6e67 6528 7365  es_ttl_change(se
-0000f000: 6c66 293a 0a20 2020 2020 2020 2070 726f  lf):.        pro
-0000f010: 7669 6465 7220 3d20 436c 6f75 6466 6c61  vider = Cloudfla
-0000f020: 7265 5072 6f76 6964 6572 2827 7465 7374  reProvider('test
-0000f030: 272c 2027 656d 6169 6c27 2c20 2774 6f6b  ', 'email', 'tok
-0000f040: 656e 2729 0a20 2020 2020 2020 207a 6f6e  en').        zon
-0000f050: 6520 3d20 5a6f 6e65 2827 756e 6974 2e74  e = Zone('unit.t
-0000f060: 6573 7473 2e27 2c20 5b5d 290a 2020 2020  ests.', []).    
-0000f070: 2020 2020 6578 6973 7469 6e67 203d 2073      existing = s
-0000f080: 6574 5f72 6563 6f72 645f 6175 746f 5f74  et_record_auto_t
-0000f090: 746c 5f66 6c61 6728 0a20 2020 2020 2020  tl_flag(.       
-0000f0a0: 2020 2020 2052 6563 6f72 642e 6e65 7728       Record.new(
-0000f0b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f0c0: 207a 6f6e 652c 0a20 2020 2020 2020 2020   zone,.         
-0000f0d0: 2020 2020 2020 2027 6127 2c0a 2020 2020         'a',.    
-0000f0e0: 2020 2020 2020 2020 2020 2020 7b27 7474              {'tt
-0000f0f0: 6c27 3a20 312c 2027 7479 7065 273a 2027  l': 1, 'type': '
-0000f100: 4127 2c20 2776 616c 7565 7327 3a20 5b27  A', 'values': ['
-0000f110: 312e 312e 312e 3127 2c20 2732 2e32 2e32  1.1.1.1', '2.2.2
-0000f120: 2e32 275d 7d2c 0a20 2020 2020 2020 2020  .2']},.         
-0000f130: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-0000f140: 2020 5472 7565 2c0a 2020 2020 2020 2020    True,.        
-0000f150: 290a 2020 2020 2020 2020 6e65 7720 3d20  ).        new = 
-0000f160: 7365 745f 7265 636f 7264 5f61 7574 6f5f  set_record_auto_
-0000f170: 7474 6c5f 666c 6167 280a 2020 2020 2020  ttl_flag(.      
-0000f180: 2020 2020 2020 5265 636f 7264 2e6e 6577        Record.new
-0000f190: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f1a0: 2020 7a6f 6e65 2c0a 2020 2020 2020 2020    zone,.        
-0000f1b0: 2020 2020 2020 2020 2761 272c 0a20 2020          'a',.   
-0000f1c0: 2020 2020 2020 2020 2020 2020 207b 2774               {'t
-0000f1d0: 746c 273a 2033 3030 2c20 2774 7970 6527  tl': 300, 'type'
-0000f1e0: 3a20 2741 272c 2027 7661 6c75 6573 273a  : 'A', 'values':
-0000f1f0: 205b 2731 2e31 2e31 2e31 272c 2027 322e   ['1.1.1.1', '2.
-0000f200: 322e 322e 3227 5d7d 2c0a 2020 2020 2020  2.2.2']},.      
-0000f210: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
-0000f220: 2020 2020 2054 7275 652c 0a20 2020 2020       True,.     
-0000f230: 2020 2029 0a20 2020 2020 2020 2063 6861     ).        cha
-0000f240: 6e67 6520 3d20 5570 6461 7465 2865 7869  nge = Update(exi
-0000f250: 7374 696e 672c 206e 6577 290a 0a20 2020  sting, new)..   
-0000f260: 2020 2020 2069 6e63 6c75 6465 5f63 6861       include_cha
-0000f270: 6e67 6520 3d20 7072 6f76 6964 6572 2e5f  nge = provider._
-0000f280: 696e 636c 7564 655f 6368 616e 6765 2863  include_change(c
-0000f290: 6861 6e67 6529 0a0a 2020 2020 2020 2020  hange)..        
-0000f2a0: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
-0000f2b0: 2869 6e63 6c75 6465 5f63 6861 6e67 6529  (include_change)
-0000f2c0: 0a0a 2020 2020 2020 2020 2320 6966 2066  ..        # if f
-0000f2d0: 6c61 6720 6973 2066 616c 7365 2c20 776f  lag is false, wo
-0000f2e0: 756c 6420 7265 7475 726e 2074 6865 2063  uld return the c
-0000f2f0: 6861 6e67 650a 2020 2020 2020 2020 6578  hange.        ex
-0000f300: 6973 7469 6e67 203d 2073 6574 5f72 6563  isting = set_rec
-0000f310: 6f72 645f 6175 746f 5f74 746c 5f66 6c61  ord_auto_ttl_fla
-0000f320: 6728 6578 6973 7469 6e67 2c20 4661 6c73  g(existing, Fals
-0000f330: 6529 0a20 2020 2020 2020 2069 6e63 6c75  e).        inclu
-0000f340: 6465 5f63 6861 6e67 6520 3d20 7072 6f76  de_change = prov
-0000f350: 6964 6572 2e5f 696e 636c 7564 655f 6368  ider._include_ch
-0000f360: 616e 6765 2863 6861 6e67 6529 0a20 2020  ange(change).   
-0000f370: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000f380: 5472 7565 2869 6e63 6c75 6465 5f63 6861  True(include_cha
-0000f390: 6e67 6529 0a0a 2020 2020 6465 6620 7465  nge)..    def te
-0000f3a0: 7374 5f69 6e63 6c75 6465 5f63 6861 6e67  st_include_chang
-0000f3b0: 655f 7370 6563 6961 6c5f 666c 6167 7328  e_special_flags(
-0000f3c0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-0000f3d0: 726f 7669 6465 7220 3d20 436c 6f75 6466  rovider = Cloudf
-0000f3e0: 6c61 7265 5072 6f76 6964 6572 2827 7465  lareProvider('te
-0000f3f0: 7374 272c 2027 656d 6169 6c27 2c20 2774  st', 'email', 't
-0000f400: 6f6b 656e 2729 0a0a 2020 2020 2020 2020  oken')..        
-0000f410: 7a6f 6e65 203d 205a 6f6e 6528 2775 6e69  zone = Zone('uni
-0000f420: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
-0000f430: 2020 2020 2020 2061 315f 706c 6169 6e20         a1_plain 
-0000f440: 3d20 5265 636f 7264 2e6e 6577 280a 2020  = Record.new(.  
-0000f450: 2020 2020 2020 2020 2020 7a6f 6e65 2c20            zone, 
-0000f460: 2777 7777 272c 207b 2774 746c 273a 2033  'www', {'ttl': 3
-0000f470: 3030 2c20 2774 7970 6527 3a20 2741 272c  00, 'type': 'A',
-0000f480: 2027 7661 6c75 6527 3a20 2731 2e32 2e33   'value': '1.2.3
-0000f490: 2e34 277d 0a20 2020 2020 2020 2029 0a20  .4'}.        ). 
-0000f4a0: 2020 2020 2020 2061 315f 7072 6f78 6965         a1_proxie
-0000f4b0: 6420 3d20 7365 745f 7265 636f 7264 5f70  d = set_record_p
-0000f4c0: 726f 7869 6564 5f66 6c61 6728 0a20 2020  roxied_flag(.   
-0000f4d0: 2020 2020 2020 2020 2052 6563 6f72 642e           Record.
-0000f4e0: 6e65 7728 0a20 2020 2020 2020 2020 2020  new(.           
-0000f4f0: 2020 2020 207a 6f6e 652c 2027 7777 7727       zone, 'www'
-0000f500: 2c20 7b27 7474 6c27 3a20 3330 302c 2027  , {'ttl': 300, '
-0000f510: 7479 7065 273a 2027 4127 2c20 2776 616c  type': 'A', 'val
-0000f520: 7565 273a 2027 312e 322e 332e 3427 7d0a  ue': '1.2.3.4'}.
-0000f530: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-0000f540: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-0000f550: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000f560: 2020 2061 315f 6175 746f 5f74 746c 203d     a1_auto_ttl =
-0000f570: 2073 6574 5f72 6563 6f72 645f 6175 746f   set_record_auto
-0000f580: 5f74 746c 5f66 6c61 6728 0a20 2020 2020  _ttl_flag(.     
-0000f590: 2020 2020 2020 2052 6563 6f72 642e 6e65         Record.ne
-0000f5a0: 7728 0a20 2020 2020 2020 2020 2020 2020  w(.             
-0000f5b0: 2020 207a 6f6e 652c 2027 7777 7727 2c20     zone, 'www', 
-0000f5c0: 7b27 7474 6c27 3a20 3330 302c 2027 7479  {'ttl': 300, 'ty
-0000f5d0: 7065 273a 2027 4127 2c20 2776 616c 7565  pe': 'A', 'value
-0000f5e0: 273a 2027 312e 322e 332e 3427 7d0a 2020  ': '1.2.3.4'}.  
-0000f5f0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-0000f600: 2020 2020 2020 2020 2054 7275 652c 0a20           True,. 
-0000f610: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000f620: 2020 2320 706c 6169 6e20 3c2d 3e20 7072    # plain <-> pr
-0000f630: 6f78 6965 640a 2020 2020 2020 2020 7365  oxied.        se
-0000f640: 6c66 2e61 7373 6572 7454 7275 6528 7072  lf.assertTrue(pr
-0000f650: 6f76 6964 6572 2e5f 696e 636c 7564 655f  ovider._include_
-0000f660: 6368 616e 6765 2855 7064 6174 6528 6131  change(Update(a1
-0000f670: 5f70 6c61 696e 2c20 6131 5f70 726f 7869  _plain, a1_proxi
-0000f680: 6564 2929 290a 2020 2020 2020 2020 7365  ed))).        se
-0000f690: 6c66 2e61 7373 6572 7454 7275 6528 7072  lf.assertTrue(pr
-0000f6a0: 6f76 6964 6572 2e5f 696e 636c 7564 655f  ovider._include_
-0000f6b0: 6368 616e 6765 2855 7064 6174 6528 6131  change(Update(a1
-0000f6c0: 5f70 726f 7869 6564 2c20 6131 5f70 6c61  _proxied, a1_pla
-0000f6d0: 696e 2929 290a 2020 2020 2020 2020 2320  in))).        # 
-0000f6e0: 706c 6169 6e20 3c2d 3e20 6175 746f 2d74  plain <-> auto-t
-0000f6f0: 746c 0a20 2020 2020 2020 2073 656c 662e  tl.        self.
-0000f700: 6173 7365 7274 5472 7565 2870 726f 7669  assertTrue(provi
-0000f710: 6465 722e 5f69 6e63 6c75 6465 5f63 6861  der._include_cha
-0000f720: 6e67 6528 5570 6461 7465 2861 315f 706c  nge(Update(a1_pl
-0000f730: 6169 6e2c 2061 315f 6175 746f 5f74 746c  ain, a1_auto_ttl
-0000f740: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-0000f750: 2e61 7373 6572 7454 7275 6528 7072 6f76  .assertTrue(prov
-0000f760: 6964 6572 2e5f 696e 636c 7564 655f 6368  ider._include_ch
-0000f770: 616e 6765 2855 7064 6174 6528 6131 5f61  ange(Update(a1_a
-0000f780: 7574 6f5f 7474 6c2c 2061 315f 706c 6169  uto_ttl, a1_plai
-0000f790: 6e29 2929 0a20 2020 2020 2020 2023 2070  n))).        # p
-0000f7a0: 726f 7869 6564 203c 2d3e 2061 7574 6f2d  roxied <-> auto-
-0000f7b0: 7474 6c0a 2020 2020 2020 2020 7365 6c66  ttl.        self
-0000f7c0: 2e61 7373 6572 7454 7275 6528 0a20 2020  .assertTrue(.   
-0000f7d0: 2020 2020 2020 2020 2070 726f 7669 6465           provide
-0000f7e0: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
-0000f7f0: 6528 5570 6461 7465 2861 315f 7072 6f78  e(Update(a1_prox
-0000f800: 6965 642c 2061 315f 6175 746f 5f74 746c  ied, a1_auto_ttl
-0000f810: 2929 0a20 2020 2020 2020 2029 0a20 2020  )).        ).   
-0000f820: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000f830: 5472 7565 280a 2020 2020 2020 2020 2020  True(.          
-0000f840: 2020 7072 6f76 6964 6572 2e5f 696e 636c    provider._incl
-0000f850: 7564 655f 6368 616e 6765 2855 7064 6174  ude_change(Updat
-0000f860: 6528 6131 5f61 7574 6f5f 7474 6c2c 2061  e(a1_auto_ttl, a
-0000f870: 315f 7072 6f78 6965 6429 290a 2020 2020  1_proxied)).    
-0000f880: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
-0000f890: 206e 6f20 7370 6563 6961 6c20 666c 6167   no special flag
-0000f8a0: 2063 6861 6e67 6573 0a20 2020 2020 2020   changes.       
-0000f8b0: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-0000f8c0: 6528 7072 6f76 6964 6572 2e5f 696e 636c  e(provider._incl
-0000f8d0: 7564 655f 6368 616e 6765 2855 7064 6174  ude_change(Updat
-0000f8e0: 6528 6131 5f70 6c61 696e 2c20 6131 5f70  e(a1_plain, a1_p
-0000f8f0: 6c61 696e 2929 290a 2020 2020 2020 2020  lain))).        
-0000f900: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
-0000f910: 280a 2020 2020 2020 2020 2020 2020 7072  (.            pr
-0000f920: 6f76 6964 6572 2e5f 696e 636c 7564 655f  ovider._include_
-0000f930: 6368 616e 6765 2855 7064 6174 6528 6131  change(Update(a1
-0000f940: 5f70 726f 7869 6564 2c20 6131 5f70 726f  _proxied, a1_pro
-0000f950: 7869 6564 2929 0a20 2020 2020 2020 2029  xied)).        )
-0000f960: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000f970: 7365 7274 4661 6c73 6528 0a20 2020 2020  sertFalse(.     
-0000f980: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-0000f990: 5f69 6e63 6c75 6465 5f63 6861 6e67 6528  _include_change(
-0000f9a0: 5570 6461 7465 2861 315f 6175 746f 5f74  Update(a1_auto_t
-0000f9b0: 746c 2c20 6131 5f61 7574 6f5f 7474 6c29  tl, a1_auto_ttl)
-0000f9c0: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
-0000f9d0: 2064 6566 2074 6573 745f 696e 636c 7564   def test_includ
-0000f9e0: 655f 6368 616e 6765 5f6d 696e 5f74 746c  e_change_min_ttl
-0000f9f0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-0000fa00: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
-0000fa10: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
-0000fa20: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
-0000fa30: 746f 6b65 6e27 290a 0a20 2020 2020 2020  token')..       
-0000fa40: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
-0000fa50: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
-0000fa60: 2020 2020 2020 2020 6265 6c6f 7731 203d          below1 =
-0000fa70: 2052 6563 6f72 642e 6e65 7728 0a20 2020   Record.new(.   
-0000fa80: 2020 2020 2020 2020 207a 6f6e 652c 2027           zone, '
-0000fa90: 7777 7727 2c20 7b27 7474 6c27 3a20 3432  www', {'ttl': 42
-0000faa0: 2c20 2774 7970 6527 3a20 2741 272c 2027  , 'type': 'A', '
-0000fab0: 7661 6c75 6527 3a20 2731 2e32 2e33 2e34  value': '1.2.3.4
-0000fac0: 277d 0a20 2020 2020 2020 2029 0a20 2020  '}.        ).   
-0000fad0: 2020 2020 2062 656c 6f77 3220 3d20 5265       below2 = Re
-0000fae0: 636f 7264 2e6e 6577 280a 2020 2020 2020  cord.new(.      
-0000faf0: 2020 2020 2020 7a6f 6e65 2c20 2777 7777        zone, 'www
-0000fb00: 272c 207b 2774 746c 273a 2031 3139 2c20  ', {'ttl': 119, 
-0000fb10: 2774 7970 6527 3a20 2741 272c 2027 7661  'type': 'A', 'va
-0000fb20: 6c75 6527 3a20 2731 2e32 2e33 2e34 277d  lue': '1.2.3.4'}
-0000fb30: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-0000fb40: 2020 2065 6467 6520 3d20 5265 636f 7264     edge = Record
-0000fb50: 2e6e 6577 280a 2020 2020 2020 2020 2020  .new(.          
-0000fb60: 2020 7a6f 6e65 2c20 2777 7777 272c 207b    zone, 'www', {
-0000fb70: 2774 746c 273a 2031 3230 2c20 2774 7970  'ttl': 120, 'typ
-0000fb80: 6527 3a20 2741 272c 2027 7661 6c75 6527  e': 'A', 'value'
-0000fb90: 3a20 2731 2e32 2e33 2e34 277d 0a20 2020  : '1.2.3.4'}.   
-0000fba0: 2020 2020 2029 0a20 2020 2020 2020 2061       ).        a
-0000fbb0: 626f 7665 3120 3d20 5265 636f 7264 2e6e  bove1 = Record.n
-0000fbc0: 6577 280a 2020 2020 2020 2020 2020 2020  ew(.            
-0000fbd0: 7a6f 6e65 2c20 2777 7777 272c 207b 2774  zone, 'www', {'t
-0000fbe0: 746c 273a 2031 3231 2c20 2774 7970 6527  tl': 121, 'type'
-0000fbf0: 3a20 2741 272c 2027 7661 6c75 6527 3a20  : 'A', 'value': 
-0000fc00: 2731 2e32 2e33 2e34 277d 0a20 2020 2020  '1.2.3.4'}.     
-0000fc10: 2020 2029 0a20 2020 2020 2020 2061 626f     ).        abo
-0000fc20: 7665 3220 3d20 5265 636f 7264 2e6e 6577  ve2 = Record.new
-0000fc30: 280a 2020 2020 2020 2020 2020 2020 7a6f  (.            zo
-0000fc40: 6e65 2c20 2777 7777 272c 207b 2774 746c  ne, 'www', {'ttl
-0000fc50: 273a 2035 3030 2c20 2774 7970 6527 3a20  ': 500, 'type': 
-0000fc60: 2741 272c 2027 7661 6c75 6527 3a20 2731  'A', 'value': '1
-0000fc70: 2e32 2e33 2e34 277d 0a20 2020 2020 2020  .2.3.4'}.       
-0000fc80: 2029 0a0a 2020 2020 2020 2020 2320 626f   )..        # bo
-0000fc90: 7468 2062 656c 6f77 0a20 2020 2020 2020  th below.       
-0000fca0: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
-0000fcb0: 6528 7072 6f76 6964 6572 2e5f 696e 636c  e(provider._incl
-0000fcc0: 7564 655f 6368 616e 6765 2855 7064 6174  ude_change(Updat
-0000fcd0: 6528 6265 6c6f 7731 2c20 6265 6c6f 7731  e(below1, below1
-0000fce0: 2929 290a 2020 2020 2020 2020 7365 6c66  ))).        self
-0000fcf0: 2e61 7373 6572 7446 616c 7365 2870 726f  .assertFalse(pro
-0000fd00: 7669 6465 722e 5f69 6e63 6c75 6465 5f63  vider._include_c
-0000fd10: 6861 6e67 6528 5570 6461 7465 2862 656c  hange(Update(bel
-0000fd20: 6f77 312c 2062 656c 6f77 3229 2929 0a20  ow1, below2))). 
-0000fd30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000fd40: 7274 4661 6c73 6528 7072 6f76 6964 6572  rtFalse(provider
-0000fd50: 2e5f 696e 636c 7564 655f 6368 616e 6765  ._include_change
-0000fd60: 2855 7064 6174 6528 6265 6c6f 7732 2c20  (Update(below2, 
-0000fd70: 6265 6c6f 7731 2929 290a 2020 2020 2020  below1))).      
-0000fd80: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
-0000fd90: 7365 2870 726f 7669 6465 722e 5f69 6e63  se(provider._inc
-0000fda0: 6c75 6465 5f63 6861 6e67 6528 5570 6461  lude_change(Upda
-0000fdb0: 7465 2862 656c 6f77 322c 2062 656c 6f77  te(below2, below
-0000fdc0: 3229 2929 0a0a 2020 2020 2020 2020 2320  2)))..        # 
-0000fdd0: 6f6e 6520 6265 6c6f 772c 206f 7468 6572  one below, other
-0000fde0: 2061 740a 2020 2020 2020 2020 7365 6c66   at.        self
-0000fdf0: 2e61 7373 6572 7446 616c 7365 2870 726f  .assertFalse(pro
-0000fe00: 7669 6465 722e 5f69 6e63 6c75 6465 5f63  vider._include_c
-0000fe10: 6861 6e67 6528 5570 6461 7465 2862 656c  hange(Update(bel
-0000fe20: 6f77 312c 2065 6467 6529 2929 0a20 2020  ow1, edge))).   
-0000fe30: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-0000fe40: 4661 6c73 6528 7072 6f76 6964 6572 2e5f  False(provider._
-0000fe50: 696e 636c 7564 655f 6368 616e 6765 2855  include_change(U
-0000fe60: 7064 6174 6528 6265 6c6f 7732 2c20 6564  pdate(below2, ed
-0000fe70: 6765 2929 290a 2020 2020 2020 2020 7365  ge))).        se
-0000fe80: 6c66 2e61 7373 6572 7446 616c 7365 2870  lf.assertFalse(p
-0000fe90: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
-0000fea0: 5f63 6861 6e67 6528 5570 6461 7465 2865  _change(Update(e
-0000feb0: 6467 652c 2062 656c 6f77 3129 2929 0a20  dge, below1))). 
-0000fec0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-0000fed0: 7274 4661 6c73 6528 7072 6f76 6964 6572  rtFalse(provider
-0000fee0: 2e5f 696e 636c 7564 655f 6368 616e 6765  ._include_change
-0000fef0: 2855 7064 6174 6528 6564 6765 2c20 6265  (Update(edge, be
-0000ff00: 6c6f 7732 2929 290a 0a20 2020 2020 2020  low2)))..       
-0000ff10: 2023 2062 6f74 6820 6174 0a20 2020 2020   # both at.     
-0000ff20: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
-0000ff30: 6c73 6528 7072 6f76 6964 6572 2e5f 696e  lse(provider._in
-0000ff40: 636c 7564 655f 6368 616e 6765 2855 7064  clude_change(Upd
-0000ff50: 6174 6528 6564 6765 2c20 6564 6765 2929  ate(edge, edge))
-0000ff60: 290a 0a20 2020 2020 2020 2023 206f 6e65  )..        # one
-0000ff70: 2061 742c 206f 7468 6572 2061 626f 7665   at, other above
-0000ff80: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-0000ff90: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
-0000ffa0: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
-0000ffb0: 6528 5570 6461 7465 2865 6467 652c 2061  e(Update(edge, a
-0000ffc0: 626f 7665 3129 2929 0a20 2020 2020 2020  bove1))).       
-0000ffd0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-0000ffe0: 2870 726f 7669 6465 722e 5f69 6e63 6c75  (provider._inclu
-0000fff0: 6465 5f63 6861 6e67 6528 5570 6461 7465  de_change(Update
-00010000: 2865 6467 652c 2061 626f 7665 3229 2929  (edge, above2)))
-00010010: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00010020: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
-00010030: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
-00010040: 6528 5570 6461 7465 2861 626f 7665 312c  e(Update(above1,
-00010050: 2065 6467 6529 2929 0a20 2020 2020 2020   edge))).       
-00010060: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
-00010070: 2870 726f 7669 6465 722e 5f69 6e63 6c75  (provider._inclu
-00010080: 6465 5f63 6861 6e67 6528 5570 6461 7465  de_change(Update
-00010090: 2861 626f 7665 322c 2065 6467 6529 2929  (above2, edge)))
-000100a0: 0a0a 2020 2020 2020 2020 2320 626f 7468  ..        # both
-000100b0: 2061 626f 7665 0a20 2020 2020 2020 2073   above.        s
-000100c0: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
-000100d0: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
-000100e0: 5f63 6861 6e67 6528 5570 6461 7465 2861  _change(Update(a
-000100f0: 626f 7665 312c 2061 626f 7665 3229 2929  bove1, above2)))
-00010100: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00010110: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
-00010120: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
-00010130: 6528 5570 6461 7465 2861 626f 7665 322c  e(Update(above2,
-00010140: 2061 626f 7665 3129 2929 0a20 2020 2020   above1))).     
-00010150: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
-00010160: 6c73 6528 7072 6f76 6964 6572 2e5f 696e  lse(provider._in
-00010170: 636c 7564 655f 6368 616e 6765 2855 7064  clude_change(Upd
-00010180: 6174 6528 6162 6f76 6531 2c20 6162 6f76  ate(above1, abov
-00010190: 6531 2929 290a 2020 2020 2020 2020 7365  e1))).        se
-000101a0: 6c66 2e61 7373 6572 7446 616c 7365 2870  lf.assertFalse(p
-000101b0: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
-000101c0: 5f63 6861 6e67 6528 5570 6461 7465 2861  _change(Update(a
-000101d0: 626f 7665 322c 2061 626f 7665 3229 2929  bove2, above2)))
-000101e0: 0a0a 2020 2020 2020 2020 2320 6f6e 6520  ..        # one 
-000101f0: 6265 6c6f 772c 206f 6e65 2061 626f 7665  below, one above
-00010200: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00010210: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
-00010220: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
-00010230: 6528 5570 6461 7465 2862 656c 6f77 322c  e(Update(below2,
-00010240: 2061 626f 7665 3129 2929 0a20 2020 2020   above1))).     
-00010250: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00010260: 7565 2870 726f 7669 6465 722e 5f69 6e63  ue(provider._inc
-00010270: 6c75 6465 5f63 6861 6e67 6528 5570 6461  lude_change(Upda
-00010280: 7465 2861 626f 7665 312c 2062 656c 6f77  te(above1, below
-00010290: 3229 2929 0a0a 2020 2020 6465 6620 7465  2)))..    def te
-000102a0: 7374 5f75 6e70 726f 7869 6162 6c65 7479  st_unproxiablety
-000102b0: 7065 5f67 656e 6461 7461 5f72 6574 7572  pe_gendata_retur
-000102c0: 6e73 6e6f 7072 6f78 6965 6428 7365 6c66  nsnoproxied(self
-000102d0: 293a 0a20 2020 2020 2020 2070 726f 7669  ):.        provi
-000102e0: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
-000102f0: 5072 6f76 6964 6572 2827 7465 7374 272c  Provider('test',
-00010300: 2027 656d 6169 6c27 2c20 2774 6f6b 656e   'email', 'token
-00010310: 2729 0a20 2020 2020 2020 207a 6f6e 6520  ').        zone 
-00010320: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
-00010330: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
-00010340: 2020 7265 636f 7264 203d 2052 6563 6f72    record = Recor
-00010350: 642e 6e65 7728 0a20 2020 2020 2020 2020  d.new(.         
-00010360: 2020 207a 6f6e 652c 2027 6127 2c20 7b27     zone, 'a', {'
-00010370: 7474 6c27 3a20 3336 3030 2c20 2774 7970  ttl': 3600, 'typ
-00010380: 6527 3a20 274e 5327 2c20 2776 616c 7565  e': 'NS', 'value
-00010390: 273a 2027 6e73 312e 756e 6974 2e74 6573  ': 'ns1.unit.tes
-000103a0: 7473 2e27 7d0a 2020 2020 2020 2020 290a  ts.'}.        ).
-000103b0: 0a20 2020 2020 2020 2064 6174 6120 3d20  .        data = 
-000103c0: 6e65 7874 2870 726f 7669 6465 722e 5f67  next(provider._g
-000103d0: 656e 5f64 6174 6128 7265 636f 7264 2929  en_data(record))
-000103e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000103f0: 7373 6572 7446 616c 7365 2827 7072 6f78  ssertFalse('prox
-00010400: 6965 6427 2069 6e20 6461 7461 290a 0a20  ied' in data).. 
-00010410: 2020 2064 6566 2074 6573 745f 7072 6f78     def test_prox
-00010420: 6961 626c 6574 7970 655f 6765 6e64 6174  iabletype_gendat
-00010430: 615f 7265 7475 726e 7375 6e70 726f 7869  a_returnsunproxi
-00010440: 6564 2873 656c 6629 3a0a 2020 2020 2020  ed(self):.      
-00010450: 2020 7072 6f76 6964 6572 203d 2043 6c6f    provider = Clo
-00010460: 7564 666c 6172 6550 726f 7669 6465 7228  udflareProvider(
-00010470: 2774 6573 7427 2c20 2765 6d61 696c 272c  'test', 'email',
-00010480: 2027 746f 6b65 6e27 290a 2020 2020 2020   'token').      
-00010490: 2020 7a6f 6e65 203d 205a 6f6e 6528 2775    zone = Zone('u
-000104a0: 6e69 742e 7465 7374 732e 272c 205b 5d29  nit.tests.', [])
-000104b0: 0a20 2020 2020 2020 2072 6563 6f72 6420  .        record 
-000104c0: 3d20 7365 745f 7265 636f 7264 5f70 726f  = set_record_pro
-000104d0: 7869 6564 5f66 6c61 6728 0a20 2020 2020  xied_flag(.     
-000104e0: 2020 2020 2020 2052 6563 6f72 642e 6e65         Record.ne
-000104f0: 7728 0a20 2020 2020 2020 2020 2020 2020  w(.             
-00010500: 2020 207a 6f6e 652c 2027 6127 2c20 7b27     zone, 'a', {'
-00010510: 7474 6c27 3a20 3330 302c 2027 7479 7065  ttl': 300, 'type
-00010520: 273a 2027 4127 2c20 2776 616c 7565 273a  ': 'A', 'value':
-00010530: 2027 312e 322e 332e 3427 7d0a 2020 2020   '1.2.3.4'}.    
-00010540: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00010550: 2020 2020 2020 2046 616c 7365 2c0a 2020         False,.  
-00010560: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00010570: 2064 6174 6120 3d20 6e65 7874 2870 726f   data = next(pro
-00010580: 7669 6465 722e 5f67 656e 5f64 6174 6128  vider._gen_data(
-00010590: 7265 636f 7264 2929 0a0a 2020 2020 2020  record))..      
-000105a0: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
-000105b0: 7365 2864 6174 615b 2770 726f 7869 6564  se(data['proxied
-000105c0: 275d 290a 0a20 2020 2064 6566 2074 6573  '])..    def tes
-000105d0: 745f 7072 6f78 6961 626c 6574 7970 655f  t_proxiabletype_
-000105e0: 6765 6e64 6174 615f 7265 7475 726e 7370  gendata_returnsp
-000105f0: 726f 7869 6564 2873 656c 6629 3a0a 2020  roxied(self):.  
-00010600: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
-00010610: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
-00010620: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
-00010630: 696c 272c 2027 746f 6b65 6e27 290a 2020  il', 'token').  
-00010640: 2020 2020 2020 7a6f 6e65 203d 205a 6f6e        zone = Zon
-00010650: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
-00010660: 205b 5d29 0a20 2020 2020 2020 2072 6563   []).        rec
-00010670: 6f72 6420 3d20 7365 745f 7265 636f 7264  ord = set_record
-00010680: 5f70 726f 7869 6564 5f66 6c61 6728 0a20  _proxied_flag(. 
-00010690: 2020 2020 2020 2020 2020 2052 6563 6f72             Recor
-000106a0: 642e 6e65 7728 0a20 2020 2020 2020 2020  d.new(.         
-000106b0: 2020 2020 2020 207a 6f6e 652c 2027 6127         zone, 'a'
-000106c0: 2c20 7b27 7474 6c27 3a20 3330 302c 2027  , {'ttl': 300, '
-000106d0: 7479 7065 273a 2027 4127 2c20 2776 616c  type': 'A', 'val
-000106e0: 7565 273a 2027 312e 322e 332e 3427 7d0a  ue': '1.2.3.4'}.
-000106f0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-00010700: 2020 2020 2020 2020 2020 2054 7275 652c             True,
-00010710: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00010720: 2020 2020 6461 7461 203d 206e 6578 7428      data = next(
-00010730: 7072 6f76 6964 6572 2e5f 6765 6e5f 6461  provider._gen_da
-00010740: 7461 2872 6563 6f72 6429 290a 0a20 2020  ta(record))..   
-00010750: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00010760: 5472 7565 2864 6174 615b 2770 726f 7869  True(data['proxi
-00010770: 6564 275d 290a 0a20 2020 2064 6566 2074  ed'])..    def t
-00010780: 6573 745f 6372 6561 7465 7265 636f 7264  est_createrecord
-00010790: 5f65 7874 7261 6368 616e 6765 735f 7265  _extrachanges_re
-000107a0: 7475 726e 7365 6d70 7479 6c69 7374 2873  turnsemptylist(s
-000107b0: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-000107c0: 6f76 6964 6572 203d 2043 6c6f 7564 666c  ovider = Cloudfl
-000107d0: 6172 6550 726f 7669 6465 7228 2774 6573  areProvider('tes
-000107e0: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
-000107f0: 6b65 6e27 290a 2020 2020 2020 2020 7072  ken').        pr
-00010800: 6f76 6964 6572 2e7a 6f6e 655f 7265 636f  ovider.zone_reco
-00010810: 7264 7320 3d20 4d6f 636b 2872 6574 7572  rds = Mock(retur
-00010820: 6e5f 7661 6c75 653d 5b5d 290a 2020 2020  n_value=[]).    
-00010830: 2020 2020 6578 6973 7469 6e67 203d 205a      existing = Z
-00010840: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
-00010850: 272c 205b 5d29 0a20 2020 2020 2020 2070  ', []).        p
-00010860: 726f 7669 6465 722e 706f 7075 6c61 7465  rovider.populate
-00010870: 2865 7869 7374 696e 6729 0a20 2020 2020  (existing).     
-00010880: 2020 2070 726f 7669 6465 722e 7a6f 6e65     provider.zone
-00010890: 5f72 6563 6f72 6473 203d 204d 6f63 6b28  _records = Mock(
-000108a0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000108b0: 7572 6e5f 7661 6c75 653d 5b0a 2020 2020  urn_value=[.    
-000108c0: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
-000108d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000108e0: 2020 2269 6422 3a20 2266 6331 3261 6233    "id": "fc12ab3
-000108f0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
-00010900: 3332 3239 3937 3634 3222 2c0a 2020 2020  322997642",.    
-00010910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010920: 2274 7970 6522 3a20 2243 4e41 4d45 222c  "type": "CNAME",
-00010930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010940: 2020 2020 2022 6e61 6d65 223a 2022 612e       "name": "a.
-00010950: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-00010960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010970: 2022 636f 6e74 656e 7422 3a20 2277 7777   "content": "www
-00010980: 2e75 6e69 742e 7465 7374 7322 2c0a 2020  .unit.tests",.  
-00010990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000109a0: 2020 2270 726f 7869 6162 6c65 223a 2054    "proxiable": T
-000109b0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-000109c0: 2020 2020 2020 2020 2022 7072 6f78 6965           "proxie
-000109d0: 6422 3a20 5472 7565 2c0a 2020 2020 2020  d": True,.      
-000109e0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-000109f0: 746c 223a 2033 3030 2c0a 2020 2020 2020  tl": 300,.      
-00010a00: 2020 2020 2020 2020 2020 2020 2020 226c                "l
-00010a10: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
-00010a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010a30: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
-00010a40: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
-00010a50: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
-00010a60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010a70: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
-00010a80: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
-00010a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010aa0: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
-00010ab0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
-00010ac0: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
-00010ad0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010ae0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
-00010af0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
-00010b00: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
-00010b10: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
-00010b20: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
-00010b30: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
-00010b40: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
-00010b50: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00010b60: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
-00010b70: 0a20 2020 2020 2020 2064 6573 6972 6564  .        desired
-00010b80: 203d 205a 6f6e 6528 2775 6e69 742e 7465   = Zone('unit.te
-00010b90: 7374 732e 272c 205b 5d29 0a20 2020 2020  sts.', []).     
-00010ba0: 2020 2070 726f 7669 6465 722e 706f 7075     provider.popu
-00010bb0: 6c61 7465 2864 6573 6972 6564 290a 2020  late(desired).  
-00010bc0: 2020 2020 2020 6368 616e 6765 7320 3d20        changes = 
-00010bd0: 6578 6973 7469 6e67 2e63 6861 6e67 6573  existing.changes
-00010be0: 2864 6573 6972 6564 2c20 7072 6f76 6964  (desired, provid
-00010bf0: 6572 290a 0a20 2020 2020 2020 2065 7874  er)..        ext
-00010c00: 7261 5f63 6861 6e67 6573 203d 2070 726f  ra_changes = pro
-00010c10: 7669 6465 722e 5f65 7874 7261 5f63 6861  vider._extra_cha
-00010c20: 6e67 6573 2865 7869 7374 696e 672c 2064  nges(existing, d
-00010c30: 6573 6972 6564 2c20 6368 616e 6765 7329  esired, changes)
-00010c40: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00010c50: 7373 6572 7446 616c 7365 2865 7874 7261  ssertFalse(extra
-00010c60: 5f63 6861 6e67 6573 290a 0a20 2020 2064  _changes)..    d
-00010c70: 6566 2074 6573 745f 7570 6461 7465 7265  ef test_updatere
-00010c80: 636f 7264 5f65 7874 7261 6368 616e 6765  cord_extrachange
-00010c90: 735f 7265 7475 726e 7365 6d70 7479 6c69  s_returnsemptyli
-00010ca0: 7374 2873 656c 6629 3a0a 2020 2020 2020  st(self):.      
-00010cb0: 2020 7072 6f76 6964 6572 203d 2043 6c6f    provider = Clo
-00010cc0: 7564 666c 6172 6550 726f 7669 6465 7228  udflareProvider(
-00010cd0: 2774 6573 7427 2c20 2765 6d61 696c 272c  'test', 'email',
-00010ce0: 2027 746f 6b65 6e27 290a 2020 2020 2020   'token').      
-00010cf0: 2020 7072 6f76 6964 6572 2e7a 6f6e 655f    provider.zone_
-00010d00: 7265 636f 7264 7320 3d20 4d6f 636b 280a  records = Mock(.
-00010d10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010d20: 726e 5f76 616c 7565 3d5b 0a20 2020 2020  rn_value=[.     
-00010d30: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
-00010d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d50: 2022 6964 223a 2022 6663 3132 6162 3334   "id": "fc12ab34
-00010d60: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
-00010d70: 3232 3939 3736 3432 222c 0a20 2020 2020  22997642",.     
-00010d80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00010d90: 7479 7065 223a 2022 434e 414d 4522 2c0a  type": "CNAME",.
-00010da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010db0: 2020 2020 226e 616d 6522 3a20 2261 2e75      "name": "a.u
-00010dc0: 6e69 742e 7465 7374 7322 2c0a 2020 2020  nit.tests",.    
-00010dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010de0: 2263 6f6e 7465 6e74 223a 2022 7777 772e  "content": "www.
-00010df0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
-00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e10: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
-00010e20: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00010e30: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
-00010e40: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00010e50: 2020 2020 2020 2020 2020 2020 2022 7474               "tt
-00010e60: 6c22 3a20 3132 302c 0a20 2020 2020 2020  l": 120,.       
-00010e70: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
-00010e80: 636b 6564 223a 2046 616c 7365 2c0a 2020  cked": False,.  
-00010e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ea0: 2020 227a 6f6e 655f 6964 223a 2022 6666    "zone_id": "ff
-00010eb0: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
-00010ec0: 3232 6162 3333 3232 3939 3736 3530 222c  22ab3322997650",
-00010ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010ee0: 2020 2020 2022 7a6f 6e65 5f6e 616d 6522       "zone_name"
-00010ef0: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
-00010f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f10: 2020 2020 226d 6f64 6966 6965 645f 6f6e      "modified_on
-00010f20: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
-00010f30: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
-00010f40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010f50: 2020 2020 2020 2263 7265 6174 6564 5f6f        "created_o
-00010f60: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
-00010f70: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
-00010f80: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00010f90: 2020 2020 2020 2022 6d65 7461 223a 207b         "meta": {
-00010fa0: 2261 7574 6f5f 6164 6465 6422 3a20 4661  "auto_added": Fa
-00010fb0: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
-00010fc0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00010fd0: 2020 2020 5d0a 2020 2020 2020 2020 290a      ].        ).
-00010fe0: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
-00010ff0: 203d 205a 6f6e 6528 2775 6e69 742e 7465   = Zone('unit.te
-00011000: 7374 732e 272c 205b 5d29 0a20 2020 2020  sts.', []).     
-00011010: 2020 2070 726f 7669 6465 722e 706f 7075     provider.popu
-00011020: 6c61 7465 2865 7869 7374 696e 6729 0a20  late(existing). 
-00011030: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00011040: 7a6f 6e65 5f72 6563 6f72 6473 203d 204d  zone_records = M
-00011050: 6f63 6b28 0a20 2020 2020 2020 2020 2020  ock(.           
-00011060: 2072 6574 7572 6e5f 7661 6c75 653d 5b0a   return_value=[.
-00011070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011080: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00011090: 2020 2020 2020 2269 6422 3a20 2266 6331        "id": "fc1
-000110a0: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
-000110b0: 3261 6233 3332 3239 3937 3634 3222 2c0a  2ab3322997642",.
-000110c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000110d0: 2020 2020 2274 7970 6522 3a20 2243 4e41      "type": "CNA
-000110e0: 4d45 222c 0a20 2020 2020 2020 2020 2020  ME",.           
-000110f0: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
-00011100: 2022 612e 756e 6974 2e74 6573 7473 222c   "a.unit.tests",
-00011110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011120: 2020 2020 2022 636f 6e74 656e 7422 3a20       "content": 
-00011130: 2277 7777 2e75 6e69 742e 7465 7374 7322  "www.unit.tests"
-00011140: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011150: 2020 2020 2020 2270 726f 7869 6162 6c65        "proxiable
-00011160: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
-00011170: 2020 2020 2020 2020 2020 2020 2022 7072               "pr
-00011180: 6f78 6965 6422 3a20 5472 7565 2c0a 2020  oxied": True,.  
-00011190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111a0: 2020 2274 746c 223a 2033 3030 2c0a 2020    "ttl": 300,.  
-000111b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111c0: 2020 226c 6f63 6b65 6422 3a20 4661 6c73    "locked": Fals
-000111d0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000111e0: 2020 2020 2020 2022 7a6f 6e65 5f69 6422         "zone_id"
-000111f0: 3a20 2266 6631 3261 6233 3463 6435 3631  : "ff12ab34cd561
-00011200: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
-00011210: 3635 3022 2c0a 2020 2020 2020 2020 2020  650",.          
-00011220: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
-00011230: 6e61 6d65 223a 2022 756e 6974 2e74 6573  name": "unit.tes
-00011240: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-00011250: 2020 2020 2020 2020 2022 6d6f 6469 6669           "modifi
-00011260: 6564 5f6f 6e22 3a20 2232 3031 372d 3033  ed_on": "2017-03
-00011270: 2d31 3154 3138 3a30 313a 3433 2e34 3230  -11T18:01:43.420
-00011280: 3638 395a 222c 0a20 2020 2020 2020 2020  689Z",.         
-00011290: 2020 2020 2020 2020 2020 2022 6372 6561             "crea
-000112a0: 7465 645f 6f6e 223a 2022 3230 3137 2d30  ted_on": "2017-0
-000112b0: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
-000112c0: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
-000112d0: 2020 2020 2020 2020 2020 2020 226d 6574              "met
-000112e0: 6122 3a20 7b22 6175 746f 5f61 6464 6564  a": {"auto_added
-000112f0: 223a 2046 616c 7365 7d2c 0a20 2020 2020  ": False},.     
-00011300: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00011310: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00011320: 2020 2029 0a20 2020 2020 2020 2064 6573     ).        des
-00011330: 6972 6564 203d 205a 6f6e 6528 2775 6e69  ired = Zone('uni
-00011340: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
-00011350: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-00011360: 706f 7075 6c61 7465 2864 6573 6972 6564  populate(desired
-00011370: 290a 2020 2020 2020 2020 6368 616e 6765  ).        change
-00011380: 7320 3d20 6578 6973 7469 6e67 2e63 6861  s = existing.cha
-00011390: 6e67 6573 2864 6573 6972 6564 2c20 7072  nges(desired, pr
-000113a0: 6f76 6964 6572 290a 0a20 2020 2020 2020  ovider)..       
-000113b0: 2065 7874 7261 5f63 6861 6e67 6573 203d   extra_changes =
-000113c0: 2070 726f 7669 6465 722e 5f65 7874 7261   provider._extra
-000113d0: 5f63 6861 6e67 6573 2865 7869 7374 696e  _changes(existin
-000113e0: 672c 2064 6573 6972 6564 2c20 6368 616e  g, desired, chan
-000113f0: 6765 7329 0a0a 2020 2020 2020 2020 7365  ges)..        se
-00011400: 6c66 2e61 7373 6572 7446 616c 7365 2865  lf.assertFalse(e
-00011410: 7874 7261 5f63 6861 6e67 6573 290a 0a20  xtra_changes).. 
-00011420: 2020 2064 6566 2074 6573 745f 6465 6c65     def test_dele
-00011430: 7465 7265 636f 7264 5f65 7874 7261 6368  terecord_extrach
-00011440: 616e 6765 735f 7265 7475 726e 7365 6d70  anges_returnsemp
-00011450: 7479 6c69 7374 2873 656c 6629 3a0a 2020  tylist(self):.  
-00011460: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
-00011470: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
-00011480: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
-00011490: 696c 272c 2027 746f 6b65 6e27 290a 2020  il', 'token').  
-000114a0: 2020 2020 2020 7072 6f76 6964 6572 2e7a        provider.z
-000114b0: 6f6e 655f 7265 636f 7264 7320 3d20 4d6f  one_records = Mo
-000114c0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
-000114d0: 7265 7475 726e 5f76 616c 7565 3d5b 0a20  return_value=[. 
-000114e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000114f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011500: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
-00011510: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-00011520: 6162 3333 3232 3939 3736 3432 222c 0a20  ab3322997642",. 
-00011530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011540: 2020 2022 7479 7065 223a 2022 434e 414d     "type": "CNAM
-00011550: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
-00011560: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-00011570: 2261 2e75 6e69 742e 7465 7374 7322 2c0a  "a.unit.tests",.
-00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011590: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-000115a0: 7777 772e 756e 6974 2e74 6573 7473 222c  www.unit.tests",
-000115b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000115c0: 2020 2020 2022 7072 6f78 6961 626c 6522       "proxiable"
-000115d0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
-000115e0: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
-000115f0: 7869 6564 223a 2054 7275 652c 0a20 2020  xied": True,.   
-00011600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011610: 2022 7474 6c22 3a20 3330 302c 0a20 2020   "ttl": 300,.   
-00011620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011630: 2022 6c6f 636b 6564 223a 2046 616c 7365   "locked": False
-00011640: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011650: 2020 2020 2020 227a 6f6e 655f 6964 223a        "zone_id":
-00011660: 2022 6666 3132 6162 3334 6364 3536 3131   "ff12ab34cd5611
-00011670: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
-00011680: 3530 222c 0a20 2020 2020 2020 2020 2020  50",.           
-00011690: 2020 2020 2020 2020 2022 7a6f 6e65 5f6e           "zone_n
-000116a0: 616d 6522 3a20 2275 6e69 742e 7465 7374  ame": "unit.test
-000116b0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-000116c0: 2020 2020 2020 2020 226d 6f64 6966 6965          "modifie
-000116d0: 645f 6f6e 223a 2022 3230 3137 2d30 332d  d_on": "2017-03-
-000116e0: 3131 5431 383a 3031 3a34 332e 3432 3036  11T18:01:43.4206
-000116f0: 3839 5a22 2c0a 2020 2020 2020 2020 2020  89Z",.          
-00011700: 2020 2020 2020 2020 2020 2263 7265 6174            "creat
-00011710: 6564 5f6f 6e22 3a20 2232 3031 372d 3033  ed_on": "2017-03
-00011720: 2d31 3154 3138 3a30 313a 3433 2e34 3230  -11T18:01:43.420
-00011730: 3638 395a 222c 0a20 2020 2020 2020 2020  689Z",.         
-00011740: 2020 2020 2020 2020 2020 2022 6d65 7461             "meta
-00011750: 223a 207b 2261 7574 6f5f 6164 6465 6422  ": {"auto_added"
-00011760: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
-00011770: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00011780: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00011790: 2020 290a 2020 2020 2020 2020 6578 6973    ).        exis
-000117a0: 7469 6e67 203d 205a 6f6e 6528 2775 6e69  ting = Zone('uni
-000117b0: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
-000117c0: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-000117d0: 706f 7075 6c61 7465 2865 7869 7374 696e  populate(existin
-000117e0: 6729 0a20 2020 2020 2020 2070 726f 7669  g).        provi
-000117f0: 6465 722e 7a6f 6e65 5f72 6563 6f72 6473  der.zone_records
-00011800: 203d 204d 6f63 6b28 7265 7475 726e 5f76   = Mock(return_v
-00011810: 616c 7565 3d5b 5d29 0a20 2020 2020 2020  alue=[]).       
-00011820: 2064 6573 6972 6564 203d 205a 6f6e 6528   desired = Zone(
-00011830: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-00011840: 5d29 0a20 2020 2020 2020 2070 726f 7669  ]).        provi
-00011850: 6465 722e 706f 7075 6c61 7465 2864 6573  der.populate(des
-00011860: 6972 6564 290a 2020 2020 2020 2020 6368  ired).        ch
-00011870: 616e 6765 7320 3d20 6578 6973 7469 6e67  anges = existing
-00011880: 2e63 6861 6e67 6573 2864 6573 6972 6564  .changes(desired
-00011890: 2c20 7072 6f76 6964 6572 290a 0a20 2020  , provider)..   
-000118a0: 2020 2020 2065 7874 7261 5f63 6861 6e67       extra_chang
-000118b0: 6573 203d 2070 726f 7669 6465 722e 5f65  es = provider._e
-000118c0: 7874 7261 5f63 6861 6e67 6573 2865 7869  xtra_changes(exi
-000118d0: 7374 696e 672c 2064 6573 6972 6564 2c20  sting, desired, 
-000118e0: 6368 616e 6765 7329 0a0a 2020 2020 2020  changes)..      
-000118f0: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
-00011900: 7365 2865 7874 7261 5f63 6861 6e67 6573  se(extra_changes
-00011910: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00011920: 7072 6f78 6966 795f 6578 7472 6163 6861  proxify_extracha
-00011930: 6e67 6573 5f72 6574 7572 6e73 7570 6461  nges_returnsupda
-00011940: 7465 6c69 7374 2873 656c 6629 3a0a 2020  telist(self):.  
-00011950: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
-00011960: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
-00011970: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
-00011980: 696c 272c 2027 746f 6b65 6e27 290a 2020  il', 'token').  
-00011990: 2020 2020 2020 7072 6f76 6964 6572 2e7a        provider.z
-000119a0: 6f6e 655f 7265 636f 7264 7320 3d20 4d6f  one_records = Mo
-000119b0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
-000119c0: 7265 7475 726e 5f76 616c 7565 3d5b 0a20  return_value=[. 
-000119d0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000119e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000119f0: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
-00011a00: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-00011a10: 6162 3333 3232 3939 3736 3432 222c 0a20  ab3322997642",. 
-00011a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a30: 2020 2022 7479 7065 223a 2022 434e 414d     "type": "CNAM
-00011a40: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
-00011a50: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
-00011a60: 2261 2e75 6e69 742e 7465 7374 7322 2c0a  "a.unit.tests",.
-00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
-00011a90: 7777 772e 756e 6974 2e74 6573 7473 222c  www.unit.tests",
-00011aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ab0: 2020 2020 2022 7072 6f78 6961 626c 6522       "proxiable"
-00011ac0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
-00011ad0: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
-00011ae0: 7869 6564 223a 2046 616c 7365 2c0a 2020  xied": False,.  
-00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b00: 2020 2274 746c 223a 2033 3030 2c0a 2020    "ttl": 300,.  
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2020 226c 6f63 6b65 6422 3a20 4661 6c73    "locked": Fals
-00011b30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00011b40: 2020 2020 2020 2022 7a6f 6e65 5f69 6422         "zone_id"
-00011b50: 3a20 2266 6631 3261 6233 3463 6435 3631  : "ff12ab34cd561
-00011b60: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
-00011b70: 3635 3022 2c0a 2020 2020 2020 2020 2020  650",.          
-00011b80: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
-00011b90: 6e61 6d65 223a 2022 756e 6974 2e74 6573  name": "unit.tes
-00011ba0: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-00011bb0: 2020 2020 2020 2020 2022 6d6f 6469 6669           "modifi
-00011bc0: 6564 5f6f 6e22 3a20 2232 3031 372d 3033  ed_on": "2017-03
-00011bd0: 2d31 3154 3138 3a30 313a 3433 2e34 3230  -11T18:01:43.420
-00011be0: 3638 395a 222c 0a20 2020 2020 2020 2020  689Z",.         
-00011bf0: 2020 2020 2020 2020 2020 2022 6372 6561             "crea
-00011c00: 7465 645f 6f6e 223a 2022 3230 3137 2d30  ted_on": "2017-0
-00011c10: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
-00011c20: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
-00011c30: 2020 2020 2020 2020 2020 2020 226d 6574              "met
-00011c40: 6122 3a20 7b22 6175 746f 5f61 6464 6564  a": {"auto_added
-00011c50: 223a 2046 616c 7365 7d2c 0a20 2020 2020  ": False},.     
-00011c60: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-00011c70: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00011c80: 2020 2029 0a20 2020 2020 2020 2065 7869     ).        exi
-00011c90: 7374 696e 6720 3d20 5a6f 6e65 2827 756e  sting = Zone('un
-00011ca0: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
-00011cb0: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
-00011cc0: 2e70 6f70 756c 6174 6528 6578 6973 7469  .populate(existi
-00011cd0: 6e67 290a 2020 2020 2020 2020 7072 6f76  ng).        prov
-00011ce0: 6964 6572 2e7a 6f6e 655f 7265 636f 7264  ider.zone_record
-00011cf0: 7320 3d20 4d6f 636b 280a 2020 2020 2020  s = Mock(.      
-00011d00: 2020 2020 2020 7265 7475 726e 5f76 616c        return_val
-00011d10: 7565 3d5b 0a20 2020 2020 2020 2020 2020  ue=[.           
-00011d20: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00011d30: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
-00011d40: 2022 6663 3132 6162 3334 6364 3536 3131   "fc12ab34cd5611
-00011d50: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
-00011d60: 3432 222c 0a20 2020 2020 2020 2020 2020  42",.           
-00011d70: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
-00011d80: 2022 434e 414d 4522 2c0a 2020 2020 2020   "CNAME",.      
-00011d90: 2020 2020 2020 2020 2020 2020 2020 226e                "n
-00011da0: 616d 6522 3a20 2261 2e75 6e69 742e 7465  ame": "a.unit.te
-00011db0: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
-00011dc0: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
-00011dd0: 6e74 223a 2022 7777 772e 756e 6974 2e74  nt": "www.unit.t
-00011de0: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
-00011df0: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
-00011e00: 6961 626c 6522 3a20 5472 7565 2c0a 2020  iable": True,.  
-00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e20: 2020 2270 726f 7869 6564 223a 2054 7275    "proxied": Tru
-00011e30: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00011e40: 2020 2020 2020 2022 7474 6c22 3a20 3330         "ttl": 30
-00011e50: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00011e60: 2020 2020 2020 2022 6c6f 636b 6564 223a         "locked":
-00011e70: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00011e80: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
-00011e90: 655f 6964 223a 2022 6666 3132 6162 3334  e_id": "ff12ab34
-00011ea0: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
-00011eb0: 3232 3939 3736 3530 222c 0a20 2020 2020  22997650",.     
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00011ed0: 7a6f 6e65 5f6e 616d 6522 3a20 2275 6e69  zone_name": "uni
-00011ee0: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
-00011ef0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
-00011f00: 6f64 6966 6965 645f 6f6e 223a 2022 3230  odified_on": "20
-00011f10: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
-00011f20: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
-00011f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f40: 2263 7265 6174 6564 5f6f 6e22 3a20 2232  "created_on": "2
-00011f50: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
-00011f60: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2022 6d65 7461 223a 207b 2261 7574 6f5f   "meta": {"auto_
-00011f90: 6164 6465 6422 3a20 4661 6c73 657d 2c0a  added": False},.
-00011fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fb0: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
-00011fc0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00011fd0: 2020 6465 7369 7265 6420 3d20 5a6f 6e65    desired = Zone
-00011fe0: 2827 756e 6974 2e74 6573 7473 2e27 2c20  ('unit.tests.', 
-00011ff0: 5b5d 290a 2020 2020 2020 2020 7072 6f76  []).        prov
-00012000: 6964 6572 2e70 6f70 756c 6174 6528 6465  ider.populate(de
-00012010: 7369 7265 6429 0a20 2020 2020 2020 2063  sired).        c
-00012020: 6861 6e67 6573 203d 2065 7869 7374 696e  hanges = existin
-00012030: 672e 6368 616e 6765 7328 6465 7369 7265  g.changes(desire
-00012040: 642c 2070 726f 7669 6465 7229 0a0a 2020  d, provider)..  
-00012050: 2020 2020 2020 6578 7472 615f 6368 616e        extra_chan
-00012060: 6765 7320 3d20 7072 6f76 6964 6572 2e5f  ges = provider._
-00012070: 6578 7472 615f 6368 616e 6765 7328 6578  extra_changes(ex
-00012080: 6973 7469 6e67 2c20 6465 7369 7265 642c  isting, desired,
-00012090: 2063 6861 6e67 6573 290a 0a20 2020 2020   changes)..     
-000120a0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
-000120b0: 7561 6c28 312c 206c 656e 2865 7874 7261  ual(1, len(extra
-000120c0: 5f63 6861 6e67 6573 2929 0a20 2020 2020  _changes)).     
-000120d0: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
-000120e0: 6c73 6528 0a20 2020 2020 2020 2020 2020  lse(.           
-000120f0: 2065 7874 7261 5f63 6861 6e67 6573 5b30   extra_changes[0
-00012100: 5d0a 2020 2020 2020 2020 2020 2020 2e65  ].            .e
-00012110: 7869 7374 696e 672e 5f6f 6374 6f64 6e73  xisting._octodns
-00012120: 2e67 6574 2827 636c 6f75 6466 6c61 7265  .get('cloudflare
-00012130: 272c 207b 7d29 0a20 2020 2020 2020 2020  ', {}).         
-00012140: 2020 202e 6765 7428 2770 726f 7869 6564     .get('proxied
-00012150: 272c 2046 616c 7365 290a 2020 2020 2020  ', False).      
-00012160: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-00012170: 2e61 7373 6572 7454 7275 6528 6578 7472  .assertTrue(extr
-00012180: 615f 6368 616e 6765 735b 305d 2e6e 6577  a_changes[0].new
-00012190: 2e5f 6f63 746f 646e 735b 2763 6c6f 7564  ._octodns['cloud
-000121a0: 666c 6172 6527 5d5b 2770 726f 7869 6564  flare']['proxied
-000121b0: 275d 290a 0a20 2020 2064 6566 2074 6573  '])..    def tes
-000121c0: 745f 756e 7072 6f78 6966 795f 6578 7472  t_unproxify_extr
-000121d0: 6163 6861 6e67 6573 5f72 6574 7572 6e73  achanges_returns
-000121e0: 7570 6461 7465 6c69 7374 2873 656c 6629  updatelist(self)
-000121f0: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
-00012200: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
-00012210: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
-00012220: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
-00012230: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
-00012240: 6572 2e7a 6f6e 655f 7265 636f 7264 7320  er.zone_records 
-00012250: 3d20 4d6f 636b 280a 2020 2020 2020 2020  = Mock(.        
-00012260: 2020 2020 7265 7475 726e 5f76 616c 7565      return_value
-00012270: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
-00012280: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00012290: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
-000122a0: 6663 3132 6162 3334 6364 3536 3131 3333  fc12ab34cd561133
-000122b0: 3434 3232 6162 3333 3232 3939 3736 3432  4422ab3322997642
-000122c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-000122d0: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
-000122e0: 434e 414d 4522 2c0a 2020 2020 2020 2020  CNAME",.        
-000122f0: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
-00012300: 6522 3a20 2261 2e75 6e69 742e 7465 7374  e": "a.unit.test
-00012310: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00012320: 2020 2020 2020 2020 2263 6f6e 7465 6e74          "content
-00012330: 223a 2022 7777 772e 756e 6974 2e74 6573  ": "www.unit.tes
-00012340: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-00012350: 2020 2020 2020 2020 2022 7072 6f78 6961           "proxia
-00012360: 626c 6522 3a20 5472 7565 2c0a 2020 2020  ble": True,.    
-00012370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012380: 2270 726f 7869 6564 223a 2054 7275 652c  "proxied": True,
-00012390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000123a0: 2020 2020 2022 7474 6c22 3a20 3330 302c       "ttl": 300,
-000123b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000123c0: 2020 2020 2022 6c6f 636b 6564 223a 2046       "locked": F
-000123d0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000123e0: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
-000123f0: 6964 223a 2022 6666 3132 6162 3334 6364  id": "ff12ab34cd
-00012400: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
-00012410: 3939 3736 3530 222c 0a20 2020 2020 2020  997650",.       
-00012420: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
-00012430: 6e65 5f6e 616d 6522 3a20 2275 6e69 742e  ne_name": "unit.
-00012440: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
-00012450: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
-00012460: 6966 6965 645f 6f6e 223a 2022 3230 3137  ified_on": "2017
-00012470: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
-00012480: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
-00012490: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000124a0: 7265 6174 6564 5f6f 6e22 3a20 2232 3031  reated_on": "201
-000124b0: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
-000124c0: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
-000124d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000124e0: 6d65 7461 223a 207b 2261 7574 6f5f 6164  meta": {"auto_ad
-000124f0: 6465 6422 3a20 4661 6c73 657d 2c0a 2020  ded": False},.  
-00012500: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00012510: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-00012520: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00012530: 6578 6973 7469 6e67 203d 205a 6f6e 6528  existing = Zone(
-00012540: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
-00012550: 5d29 0a20 2020 2020 2020 2070 726f 7669  ]).        provi
-00012560: 6465 722e 706f 7075 6c61 7465 2865 7869  der.populate(exi
-00012570: 7374 696e 6729 0a20 2020 2020 2020 2070  sting).        p
-00012580: 726f 7669 6465 722e 7a6f 6e65 5f72 6563  rovider.zone_rec
-00012590: 6f72 6473 203d 204d 6f63 6b28 0a20 2020  ords = Mock(.   
-000125a0: 2020 2020 2020 2020 2072 6574 7572 6e5f           return_
-000125b0: 7661 6c75 653d 5b0a 2020 2020 2020 2020  value=[.        
-000125c0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000125d0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-000125e0: 6422 3a20 2266 6331 3261 6233 3463 6435  d": "fc12ab34cd5
-000125f0: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
-00012600: 3937 3634 3222 2c0a 2020 2020 2020 2020  97642",.        
-00012610: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
-00012620: 6522 3a20 2243 4e41 4d45 222c 0a20 2020  e": "CNAME",.   
-00012630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012640: 2022 6e61 6d65 223a 2022 612e 756e 6974   "name": "a.unit
-00012650: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
-00012660: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00012670: 6e74 656e 7422 3a20 2277 7777 2e75 6e69  ntent": "www.uni
-00012680: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
-00012690: 2020 2020 2020 2020 2020 2020 2020 2270                "p
-000126a0: 726f 7869 6162 6c65 223a 2054 7275 652c  roxiable": True,
-000126b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000126c0: 2020 2020 2022 7072 6f78 6965 6422 3a20       "proxied": 
-000126d0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-000126e0: 2020 2020 2020 2020 2020 2022 7474 6c22             "ttl"
-000126f0: 3a20 3330 302c 0a20 2020 2020 2020 2020  : 300,.         
-00012700: 2020 2020 2020 2020 2020 2022 6c6f 636b             "lock
-00012710: 6564 223a 2046 616c 7365 2c0a 2020 2020  ed": False,.    
-00012720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012730: 227a 6f6e 655f 6964 223a 2022 6666 3132  "zone_id": "ff12
-00012740: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
-00012750: 6162 3333 3232 3939 3736 3530 222c 0a20  ab3322997650",. 
+0000bd30: 2020 2020 2020 2027 6c6f 6e67 5f64 6567         'long_deg
+0000bd40: 7265 6573 273a 2031 3135 2c0a 2020 2020  rees': 115,.    
+0000bd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd60: 2020 2020 276c 6f6e 675f 6d69 6e75 7465      'long_minute
+0000bd70: 7327 3a20 3439 2c0a 2020 2020 2020 2020  s': 49,.        
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd90: 276c 6f6e 675f 7365 636f 6e64 7327 3a20  'long_seconds': 
+0000bda0: 3131 2e37 2c0a 2020 2020 2020 2020 2020  11.7,.          
+0000bdb0: 2020 2020 2020 2020 2020 2020 2020 276c                'l
+0000bdc0: 6f6e 675f 6469 7265 6374 696f 6e27 3a20  ong_direction': 
+0000bdd0: 2745 272c 0a20 2020 2020 2020 2020 2020  'E',.           
+0000bde0: 2020 2020 2020 2020 2020 2020 2027 616c               'al
+0000bdf0: 7469 7475 6465 273a 2032 302c 0a20 2020  titude': 20,.   
+0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be10: 2020 2020 2027 7369 7a65 273a 2031 302c       'size': 10,
+0000be20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000be30: 2020 2020 2020 2020 2027 7072 6563 6973           'precis
+0000be40: 696f 6e5f 686f 727a 273a 2031 302c 0a20  ion_horz': 10,. 
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2020 2020 2020 2027 7072 6563 6973 696f         'precisio
+0000be70: 6e5f 7665 7274 273a 2032 2c0a 2020 2020  n_vert': 2,.    
+0000be80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be90: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+0000bea0: 2020 2020 2020 2027 7479 7065 273a 2027         'type': '
+0000beb0: 4c4f 4327 2c0a 2020 2020 2020 2020 2020  LOC',.          
+0000bec0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0000bed0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+0000bee0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
+0000bef0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000bf00: 6578 7065 6374 6564 2c20 7072 6f76 6964  expected, provid
+0000bf10: 6572 2e5f 6765 6e5f 6b65 7928 6461 7461  er._gen_key(data
+0000bf20: 2929 0a0a 2020 2020 6465 6620 7465 7374  ))..    def test
+0000bf30: 5f63 646e 2873 656c 6629 3a0a 2020 2020  _cdn(self):.    
+0000bf40: 2020 2020 7072 6f76 6964 6572 203d 2043      provider = C
+0000bf50: 6c6f 7564 666c 6172 6550 726f 7669 6465  loudflareProvide
+0000bf60: 7228 0a20 2020 2020 2020 2020 2020 2027  r(.            '
+0000bf70: 7465 7374 272c 2027 656d 6169 6c27 2c20  test', 'email', 
+0000bf80: 2774 6f6b 656e 272c 2027 6163 636f 756e  'token', 'accoun
+0000bf90: 745f 6964 272c 2054 7275 650a 2020 2020  t_id', True.    
+0000bfa0: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+0000bfb0: 2041 2043 4e41 4d45 2066 6f72 2075 7320   A CNAME for us 
+0000bfc0: 746f 2074 7261 6e73 666f 726d 2074 6f20  to transform to 
+0000bfd0: 414c 4941 530a 2020 2020 2020 2020 7072  ALIAS.        pr
+0000bfe0: 6f76 6964 6572 2e7a 6f6e 655f 7265 636f  ovider.zone_reco
+0000bff0: 7264 7320 3d20 4d6f 636b 280a 2020 2020  rds = Mock(.    
+0000c000: 2020 2020 2020 2020 7265 7475 726e 5f76          return_v
+0000c010: 616c 7565 3d5b 0a20 2020 2020 2020 2020  alue=[.         
+0000c020: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000c030: 2020 2020 2020 2020 2020 2020 2022 6964               "id
+0000c040: 223a 2022 6663 3132 6162 3334 6364 3536  ": "fc12ab34cd56
+0000c050: 3131 3333 3434 3232 6162 3333 3232 3939  11334422ab332299
+0000c060: 3736 3432 222c 0a20 2020 2020 2020 2020  7642",.         
+0000c070: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+0000c080: 223a 2022 434e 414d 4522 2c0a 2020 2020  ": "CNAME",.    
+0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0a0: 226e 616d 6522 3a20 2263 6e61 6d65 2e75  "name": "cname.u
+0000c0b0: 6e69 742e 7465 7374 7322 2c0a 2020 2020  nit.tests",.    
+0000c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0d0: 2263 6f6e 7465 6e74 223a 2022 7777 772e  "content": "www.
+0000c0e0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+0000c0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c100: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
+0000c110: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000c120: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
+0000c130: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
+0000c140: 2020 2020 2020 2020 2020 2020 2022 7474               "tt
+0000c150: 6c22 3a20 3330 302c 0a20 2020 2020 2020  l": 300,.       
+0000c160: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
+0000c170: 636b 6564 223a 2046 616c 7365 2c0a 2020  cked": False,.  
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 227a 6f6e 655f 6964 223a 2022 6666    "zone_id": "ff
+0000c1a0: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
+0000c1b0: 3232 6162 3333 3232 3939 3736 3530 222c  22ab3322997650",
+0000c1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1d0: 2020 2020 2022 7a6f 6e65 5f6e 616d 6522       "zone_name"
+0000c1e0: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 2020 2020 226d 6f64 6966 6965 645f 6f6e      "modified_on
+0000c210: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
+0000c220: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
+0000c230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c240: 2020 2020 2020 2263 7265 6174 6564 5f6f        "created_o
+0000c250: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
+0000c260: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
+0000c270: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000c280: 2020 2020 2020 2022 6d65 7461 223a 207b         "meta": {
+0000c290: 2261 7574 6f5f 6164 6465 6422 3a20 4661  "auto_added": Fa
+0000c2a0: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
+0000c2b0: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0000c2c0: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c2e0: 6964 223a 2022 6663 3132 6162 3334 6364  id": "fc12ab34cd
+0000c2f0: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
+0000c300: 3939 3736 3432 222c 0a20 2020 2020 2020  997642",.       
+0000c310: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+0000c320: 7065 223a 2022 4122 2c0a 2020 2020 2020  pe": "A",.      
+0000c330: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+0000c340: 616d 6522 3a20 2261 2e75 6e69 742e 7465  ame": "a.unit.te
+0000c350: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+0000c360: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+0000c370: 6e74 223a 2022 312e 312e 312e 3122 2c0a  nt": "1.1.1.1",.
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 2020 2270 726f 7869 6162 6c65 223a      "proxiable":
+0000c3a0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+0000c3b0: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
+0000c3c0: 6965 6422 3a20 5472 7565 2c0a 2020 2020  ied": True,.    
+0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3e0: 2274 746c 223a 2033 3030 2c0a 2020 2020  "ttl": 300,.    
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 226c 6f63 6b65 6422 3a20 4661 6c73 652c  "locked": False,
+0000c410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c420: 2020 2020 2022 7a6f 6e65 5f69 6422 3a20       "zone_id": 
+0000c430: 2266 6631 3261 6233 3463 6435 3631 3133  "ff12ab34cd56113
+0000c440: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
+0000c450: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+0000c460: 2020 2020 2020 2020 227a 6f6e 655f 6e61          "zone_na
+0000c470: 6d65 223a 2022 756e 6974 2e74 6573 7473  me": "unit.tests
+0000c480: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000c490: 2020 2020 2020 2022 6d6f 6469 6669 6564         "modified
+0000c4a0: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
+0000c4b0: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
+0000c4c0: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
+0000c4d0: 2020 2020 2020 2020 2022 6372 6561 7465           "create
+0000c4e0: 645f 6f6e 223a 2022 3230 3137 2d30 332d  d_on": "2017-03-
+0000c4f0: 3131 5431 383a 3031 3a34 332e 3432 3036  11T18:01:43.4206
+0000c500: 3839 5a22 2c0a 2020 2020 2020 2020 2020  89Z",.          
+0000c510: 2020 2020 2020 2020 2020 226d 6574 6122            "meta"
+0000c520: 3a20 7b22 6175 746f 5f61 6464 6564 223a  : {"auto_added":
+0000c530: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+0000c540: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0000c550: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2269 6422 3a20 2266 6331 3261 6233    "id": "fc12ab3
+0000c580: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+0000c590: 3332 3239 3937 3634 3222 2c0a 2020 2020  322997642",.    
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 2274 7970 6522 3a20 2241 222c 0a20 2020  "type": "A",.   
+0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5d0: 2022 6e61 6d65 223a 2022 612e 756e 6974   "name": "a.unit
+0000c5e0: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
+0000c5f0: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+0000c600: 6e74 656e 7422 3a20 2231 2e31 2e31 2e32  ntent": "1.1.1.2
+0000c610: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000c620: 2020 2020 2020 2022 7072 6f78 6961 626c         "proxiabl
+0000c630: 6522 3a20 5472 7565 2c0a 2020 2020 2020  e": True,.      
+0000c640: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0000c650: 726f 7869 6564 223a 2054 7275 652c 0a20  roxied": True,. 
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c670: 2020 2022 7474 6c22 3a20 3330 302c 0a20     "ttl": 300,. 
+0000c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c690: 2020 2022 6c6f 636b 6564 223a 2046 616c     "locked": Fal
+0000c6a0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+0000c6b0: 2020 2020 2020 2020 227a 6f6e 655f 6964          "zone_id
+0000c6c0: 223a 2022 6666 3132 6162 3334 6364 3536  ": "ff12ab34cd56
+0000c6d0: 3131 3333 3434 3232 6162 3333 3232 3939  11334422ab332299
+0000c6e0: 3736 3530 222c 0a20 2020 2020 2020 2020  7650",.         
+0000c6f0: 2020 2020 2020 2020 2020 2022 7a6f 6e65             "zone
+0000c700: 5f6e 616d 6522 3a20 2275 6e69 742e 7465  _name": "unit.te
+0000c710: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+0000c720: 2020 2020 2020 2020 2020 226d 6f64 6966            "modif
+0000c730: 6965 645f 6f6e 223a 2022 3230 3137 2d30  ied_on": "2017-0
+0000c740: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
+0000c750: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
+0000c760: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
+0000c770: 6174 6564 5f6f 6e22 3a20 2232 3031 372d  ated_on": "2017-
+0000c780: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
+0000c790: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
+0000c7a0: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
+0000c7b0: 7461 223a 207b 2261 7574 6f5f 6164 6465  ta": {"auto_adde
+0000c7c0: 6422 3a20 4661 6c73 657d 2c0a 2020 2020  d": False},.    
+0000c7d0: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+0000c7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c800: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
+0000c810: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
+0000c820: 6162 3333 3232 3939 3736 3432 222c 0a20  ab3322997642",. 
+0000c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c840: 2020 2022 7479 7065 223a 2022 4122 2c0a     "type": "A",.
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 226e 616d 6522 3a20 226d 756c      "name": "mul
+0000c870: 7469 2e75 6e69 742e 7465 7374 7322 2c0a  ti.unit.tests",.
+0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c890: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
+0000c8a0: 312e 312e 312e 3322 2c0a 2020 2020 2020  1.1.1.3",.      
+0000c8b0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0000c8c0: 726f 7869 6162 6c65 223a 2054 7275 652c  roxiable": True,
+0000c8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c8e0: 2020 2020 2022 7072 6f78 6965 6422 3a20       "proxied": 
+0000c8f0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+0000c900: 2020 2020 2020 2020 2020 2274 746c 223a            "ttl":
+0000c910: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
+0000c920: 2020 2020 2020 2020 2020 226c 6f63 6b65            "locke
+0000c930: 6422 3a20 4661 6c73 652c 0a20 2020 2020  d": False,.     
+0000c940: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000c950: 7a6f 6e65 5f69 6422 3a20 2266 6631 3261  zone_id": "ff12a
+0000c960: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
+0000c970: 6233 3332 3239 3937 3635 3022 2c0a 2020  b3322997650",.  
+0000c980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c990: 2020 227a 6f6e 655f 6e61 6d65 223a 2022    "zone_name": "
+0000c9a0: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9c0: 2022 6d6f 6469 6669 6564 5f6f 6e22 3a20   "modified_on": 
+0000c9d0: 2232 3031 372d 3033 2d31 3154 3138 3a30  "2017-03-11T18:0
+0000c9e0: 313a 3433 2e34 3230 3638 395a 222c 0a20  1:43.420689Z",. 
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 2020 2022 6372 6561 7465 645f 6f6e 223a     "created_on":
+0000ca10: 2022 3230 3137 2d30 332d 3131 5431 383a   "2017-03-11T18:
+0000ca20: 3031 3a34 332e 3432 3036 3839 5a22 2c0a  01:43.420689Z",.
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 2020 2020 226d 6574 6122 3a20 7b22 6175      "meta": {"au
+0000ca50: 746f 5f61 6464 6564 223a 2046 616c 7365  to_added": False
+0000ca60: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
+0000ca70: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+0000ca80: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0000ca90: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+0000caa0: 3a20 2266 6331 3261 6233 3463 6435 3631  : "fc12ab34cd561
+0000cab0: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
+0000cac0: 3634 3222 2c0a 2020 2020 2020 2020 2020  642",.          
+0000cad0: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+0000cae0: 3a20 2241 4141 4122 2c0a 2020 2020 2020  : "AAAA",.      
+0000caf0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+0000cb00: 616d 6522 3a20 226d 756c 7469 2e75 6e69  ame": "multi.uni
+0000cb10: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+0000cb20: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+0000cb30: 6f6e 7465 6e74 223a 2022 3a3a 3122 2c0a  ontent": "::1",.
+0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb50: 2020 2020 2270 726f 7869 6162 6c65 223a      "proxiable":
+0000cb60: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+0000cb70: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
+0000cb80: 6965 6422 3a20 5472 7565 2c0a 2020 2020  ied": True,.    
+0000cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cba0: 2274 746c 223a 2033 3030 2c0a 2020 2020  "ttl": 300,.    
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 226c 6f63 6b65 6422 3a20 4661 6c73 652c  "locked": False,
+0000cbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cbe0: 2020 2020 2022 7a6f 6e65 5f69 6422 3a20       "zone_id": 
+0000cbf0: 2266 6631 3261 6233 3463 6435 3631 3133  "ff12ab34cd56113
+0000cc00: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
+0000cc10: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+0000cc20: 2020 2020 2020 2020 227a 6f6e 655f 6e61          "zone_na
+0000cc30: 6d65 223a 2022 756e 6974 2e74 6573 7473  me": "unit.tests
+0000cc40: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000cc50: 2020 2020 2020 2022 6d6f 6469 6669 6564         "modified
+0000cc60: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
+0000cc70: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
+0000cc80: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
+0000cc90: 2020 2020 2020 2020 2022 6372 6561 7465           "create
+0000cca0: 645f 6f6e 223a 2022 3230 3137 2d30 332d  d_on": "2017-03-
+0000ccb0: 3131 5431 383a 3031 3a34 332e 3432 3036  11T18:01:43.4206
+0000ccc0: 3839 5a22 2c0a 2020 2020 2020 2020 2020  89Z",.          
+0000ccd0: 2020 2020 2020 2020 2020 226d 6574 6122            "meta"
+0000cce0: 3a20 7b22 6175 746f 5f61 6464 6564 223a  : {"auto_added":
+0000ccf0: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+0000cd00: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+0000cd10: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+0000cd20: 2020 290a 0a20 2020 2020 2020 207a 6f6e    )..        zon
+0000cd30: 6520 3d20 5a6f 6e65 2827 756e 6974 2e74  e = Zone('unit.t
+0000cd40: 6573 7473 2e27 2c20 5b5d 290a 2020 2020  ests.', []).    
+0000cd50: 2020 2020 7072 6f76 6964 6572 2e70 6f70      provider.pop
+0000cd60: 756c 6174 6528 7a6f 6e65 290a 0a20 2020  ulate(zone)..   
+0000cd70: 2020 2020 2023 2074 6865 2074 776f 2041       # the two A
+0000cd80: 2072 6563 6f72 6473 2067 6574 206d 6572   records get mer
+0000cd90: 6765 6420 696e 746f 206f 6e65 2043 4e41  ged into one CNA
+0000cda0: 4d45 2072 6563 6f72 6420 706f 696e 7469  ME record pointi
+0000cdb0: 6e67 2074 6f0a 2020 2020 2020 2020 2320  ng to.        # 
+0000cdc0: 7468 6520 4344 4e2e 0a20 2020 2020 2020  the CDN..       
+0000cdd0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+0000cde0: 6c28 332c 206c 656e 287a 6f6e 652e 7265  l(3, len(zone.re
+0000cdf0: 636f 7264 7329 290a 0a20 2020 2020 2020  cords))..       
+0000ce00: 206f 7264 6572 6564 203d 2073 6f72 7465   ordered = sorte
+0000ce10: 6428 7a6f 6e65 2e72 6563 6f72 6473 2c20  d(zone.records, 
+0000ce20: 6b65 793d 6c61 6d62 6461 2072 3a20 722e  key=lambda r: r.
+0000ce30: 6e61 6d65 290a 0a20 2020 2020 2020 2072  name)..        r
+0000ce40: 6563 6f72 6420 3d20 6f72 6465 7265 645b  ecord = ordered[
+0000ce50: 305d 0a20 2020 2020 2020 2073 656c 662e  0].        self.
+0000ce60: 6173 7365 7274 4571 7561 6c28 2761 272c  assertEqual('a',
+0000ce70: 2072 6563 6f72 642e 6e61 6d65 290a 2020   record.name).  
+0000ce80: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000ce90: 7445 7175 616c 2827 612e 756e 6974 2e74  tEqual('a.unit.t
+0000cea0: 6573 7473 2e27 2c20 7265 636f 7264 2e66  ests.', record.f
+0000ceb0: 7164 6e29 0a20 2020 2020 2020 2073 656c  qdn).        sel
+0000cec0: 662e 6173 7365 7274 4571 7561 6c28 2743  f.assertEqual('C
+0000ced0: 4e41 4d45 272c 2072 6563 6f72 642e 5f74  NAME', record._t
+0000cee0: 7970 6529 0a20 2020 2020 2020 2073 656c  ype).        sel
+0000cef0: 662e 6173 7365 7274 4571 7561 6c28 2761  f.assertEqual('a
+0000cf00: 2e75 6e69 742e 7465 7374 732e 6364 6e2e  .unit.tests.cdn.
+0000cf10: 636c 6f75 6466 6c61 7265 2e6e 6574 2e27  cloudflare.net.'
+0000cf20: 2c20 7265 636f 7264 2e76 616c 7565 290a  , record.value).
+0000cf30: 0a20 2020 2020 2020 2072 6563 6f72 6420  .        record 
+0000cf40: 3d20 6f72 6465 7265 645b 315d 0a20 2020  = ordered[1].   
+0000cf50: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000cf60: 4571 7561 6c28 2763 6e61 6d65 272c 2072  Equal('cname', r
+0000cf70: 6563 6f72 642e 6e61 6d65 290a 2020 2020  ecord.name).    
+0000cf80: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+0000cf90: 7175 616c 2827 636e 616d 652e 756e 6974  qual('cname.unit
+0000cfa0: 2e74 6573 7473 2e27 2c20 7265 636f 7264  .tests.', record
+0000cfb0: 2e66 7164 6e29 0a20 2020 2020 2020 2073  .fqdn).        s
+0000cfc0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000cfd0: 2743 4e41 4d45 272c 2072 6563 6f72 642e  'CNAME', record.
+0000cfe0: 5f74 7970 6529 0a20 2020 2020 2020 2073  _type).        s
+0000cff0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000d000: 2763 6e61 6d65 2e75 6e69 742e 7465 7374  'cname.unit.test
+0000d010: 732e 6364 6e2e 636c 6f75 6466 6c61 7265  s.cdn.cloudflare
+0000d020: 2e6e 6574 2e27 2c20 7265 636f 7264 2e76  .net.', record.v
+0000d030: 616c 7565 290a 0a20 2020 2020 2020 2072  alue)..        r
+0000d040: 6563 6f72 6420 3d20 6f72 6465 7265 645b  ecord = ordered[
+0000d050: 325d 0a20 2020 2020 2020 2073 656c 662e  2].        self.
+0000d060: 6173 7365 7274 4571 7561 6c28 276d 756c  assertEqual('mul
+0000d070: 7469 272c 2072 6563 6f72 642e 6e61 6d65  ti', record.name
+0000d080: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+0000d090: 7373 6572 7445 7175 616c 2827 6d75 6c74  ssertEqual('mult
+0000d0a0: 692e 756e 6974 2e74 6573 7473 2e27 2c20  i.unit.tests.', 
+0000d0b0: 7265 636f 7264 2e66 7164 6e29 0a20 2020  record.fqdn).   
+0000d0c0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000d0d0: 4571 7561 6c28 2743 4e41 4d45 272c 2072  Equal('CNAME', r
+0000d0e0: 6563 6f72 642e 5f74 7970 6529 0a20 2020  ecord._type).   
+0000d0f0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000d100: 4571 7561 6c28 276d 756c 7469 2e75 6e69  Equal('multi.uni
+0000d110: 742e 7465 7374 732e 6364 6e2e 636c 6f75  t.tests.cdn.clou
+0000d120: 6466 6c61 7265 2e6e 6574 2e27 2c20 7265  dflare.net.', re
+0000d130: 636f 7264 2e76 616c 7565 290a 0a20 2020  cord.value)..   
+0000d140: 2020 2020 2023 2043 444e 2065 6e61 626c       # CDN enabl
+0000d150: 6564 2072 6563 6f72 6473 2063 616e 2774  ed records can't
+0000d160: 2062 6520 7570 6461 7465 642c 2077 6520   be updated, we 
+0000d170: 646f 6e27 7420 6b6e 6f77 2074 6865 2072  don't know the r
+0000d180: 6561 6c20 7661 6c75 6573 0a20 2020 2020  eal values.     
+0000d190: 2020 2023 206e 6576 6572 2070 6f69 6e74     # never point
+0000d1a0: 2061 2043 6c6f 7564 666c 6172 6520 7265   a Cloudflare re
+0000d1b0: 636f 7264 2074 6f20 6974 7365 6c66 2e0a  cord to itself..
+0000d1c0: 2020 2020 2020 2020 7761 6e74 6564 203d          wanted =
+0000d1d0: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+0000d1e0: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
+0000d1f0: 2077 616e 7465 642e 6164 645f 7265 636f   wanted.add_reco
+0000d200: 7264 280a 2020 2020 2020 2020 2020 2020  rd(.            
+0000d210: 5265 636f 7264 2e6e 6577 280a 2020 2020  Record.new(.    
+0000d220: 2020 2020 2020 2020 2020 2020 7761 6e74              want
+0000d230: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
+0000d240: 2020 2020 2763 6e61 6d65 272c 0a20 2020      'cname',.   
+0000d250: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d270: 2020 2027 7474 6c27 3a20 3330 302c 0a20     'ttl': 300,. 
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2027 7479 7065 273a 2027 434e 414d     'type': 'CNAM
+0000d2a0: 4527 2c0a 2020 2020 2020 2020 2020 2020  E',.            
+0000d2b0: 2020 2020 2020 2020 2776 616c 7565 273a          'value':
+0000d2c0: 2027 6368 616e 6765 2e75 6e69 742e 7465   'change.unit.te
+0000d2d0: 7374 732e 6364 6e2e 636c 6f75 6466 6c61  sts.cdn.cloudfla
+0000d2e0: 7265 2e6e 6574 2e27 2c0a 2020 2020 2020  re.net.',.      
+0000d2f0: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+0000d300: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d310: 2020 2029 0a20 2020 2020 2020 2077 616e     ).        wan
+0000d320: 7465 642e 6164 645f 7265 636f 7264 280a  ted.add_record(.
+0000d330: 2020 2020 2020 2020 2020 2020 5265 636f              Reco
+0000d340: 7264 2e6e 6577 280a 2020 2020 2020 2020  rd.new(.        
+0000d350: 2020 2020 2020 2020 7761 6e74 6564 2c0a          wanted,.
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 276e 6577 272c 0a20 2020 2020 2020 2020  'new',.         
+0000d380: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+0000d390: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
+0000d3a0: 6c27 3a20 3330 302c 0a20 2020 2020 2020  l': 300,.       
+0000d3b0: 2020 2020 2020 2020 2020 2020 2027 7479               'ty
+0000d3c0: 7065 273a 2027 434e 414d 4527 2c0a 2020  pe': 'CNAME',.  
+0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3e0: 2020 2776 616c 7565 273a 2027 6e65 772e    'value': 'new.
+0000d3f0: 756e 6974 2e74 6573 7473 2e63 646e 2e63  unit.tests.cdn.c
+0000d400: 6c6f 7564 666c 6172 652e 6e65 742e 272c  loudflare.net.',
+0000d410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d420: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
+0000d430: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+0000d440: 2020 2020 7761 6e74 6564 2e61 6464 5f72      wanted.add_r
+0000d450: 6563 6f72 6428 0a20 2020 2020 2020 2020  ecord(.         
+0000d460: 2020 2052 6563 6f72 642e 6e65 7728 0a20     Record.new(. 
+0000d470: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000d480: 616e 7465 642c 0a20 2020 2020 2020 2020  anted,.         
+0000d490: 2020 2020 2020 2027 6372 6561 7465 6427         'created'
+0000d4a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d4b0: 2020 7b27 7474 6c27 3a20 3330 302c 2027    {'ttl': 300, '
+0000d4c0: 7479 7065 273a 2027 434e 414d 4527 2c20  type': 'CNAME', 
+0000d4d0: 2776 616c 7565 273a 2027 7777 772e 756e  'value': 'www.un
+0000d4e0: 6974 2e74 6573 7473 2e27 7d2c 0a20 2020  it.tests.'},.   
+0000d4f0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d500: 2020 2029 0a0a 2020 2020 2020 2020 706c     )..        pl
+0000d510: 616e 203d 2070 726f 7669 6465 722e 706c  an = provider.pl
+0000d520: 616e 2877 616e 7465 6429 0a20 2020 2020  an(wanted).     
+0000d530: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+0000d540: 7561 6c28 312c 206c 656e 2870 6c61 6e2e  ual(1, len(plan.
+0000d550: 6368 616e 6765 7329 290a 0a20 2020 2064  changes))..    d
+0000d560: 6566 2074 6573 745f 6364 6e5f 616c 6961  ef test_cdn_alia
+0000d570: 7328 7365 6c66 293a 0a20 2020 2020 2020  s(self):.       
+0000d580: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
+0000d590: 6466 6c61 7265 5072 6f76 6964 6572 280a  dflareProvider(.
+0000d5a0: 2020 2020 2020 2020 2020 2020 2774 6573              'tes
+0000d5b0: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
+0000d5c0: 6b65 6e27 2c20 2761 6363 6f75 6e74 5f69  ken', 'account_i
+0000d5d0: 6427 2c20 5472 7565 0a20 2020 2020 2020  d', True.       
+0000d5e0: 2029 0a0a 2020 2020 2020 2020 2320 4120   )..        # A 
+0000d5f0: 434e 414d 4520 666f 7220 7573 2074 6f20  CNAME for us to 
+0000d600: 7472 616e 7366 6f72 6d20 746f 2041 4c49  transform to ALI
+0000d610: 4153 0a20 2020 2020 2020 2070 726f 7669  AS.        provi
+0000d620: 6465 722e 7a6f 6e65 5f72 6563 6f72 6473  der.zone_records
+0000d630: 203d 204d 6f63 6b28 0a20 2020 2020 2020   = Mock(.       
+0000d640: 2020 2020 2072 6574 7572 6e5f 7661 6c75       return_valu
+0000d650: 653d 5b0a 2020 2020 2020 2020 2020 2020  e=[.            
+0000d660: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000d670: 2020 2020 2020 2020 2020 2269 6422 3a20            "id": 
+0000d680: 2266 6331 3261 6233 3463 6435 3631 3133  "fc12ab34cd56113
+0000d690: 3334 3432 3261 6233 3332 3239 3937 3634  34422ab332299764
+0000d6a0: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+0000d6b0: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+0000d6c0: 2243 4e41 4d45 222c 0a20 2020 2020 2020  "CNAME",.       
+0000d6d0: 2020 2020 2020 2020 2020 2020 2022 6e61               "na
+0000d6e0: 6d65 223a 2022 756e 6974 2e74 6573 7473  me": "unit.tests
+0000d6f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000d700: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
+0000d710: 3a20 2277 7777 2e75 6e69 742e 7465 7374  : "www.unit.test
+0000d720: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+0000d730: 2020 2020 2020 2020 2270 726f 7869 6162          "proxiab
+0000d740: 6c65 223a 2054 7275 652c 0a20 2020 2020  le": True,.     
+0000d750: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000d760: 7072 6f78 6965 6422 3a20 5472 7565 2c0a  proxied": True,.
+0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d780: 2020 2020 2274 746c 223a 2033 3030 2c0a      "ttl": 300,.
+0000d790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7a0: 2020 2020 226c 6f63 6b65 6422 3a20 4661      "locked": Fa
+0000d7b0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0000d7c0: 2020 2020 2020 2020 2022 7a6f 6e65 5f69           "zone_i
+0000d7d0: 6422 3a20 2266 6631 3261 6233 3463 6435  d": "ff12ab34cd5
+0000d7e0: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
+0000d7f0: 3937 3635 3022 2c0a 2020 2020 2020 2020  97650",.        
+0000d800: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+0000d810: 655f 6e61 6d65 223a 2022 756e 6974 2e74  e_name": "unit.t
+0000d820: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+0000d830: 2020 2020 2020 2020 2020 2022 6d6f 6469             "modi
+0000d840: 6669 6564 5f6f 6e22 3a20 2232 3031 372d  fied_on": "2017-
+0000d850: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
+0000d860: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
+0000d870: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+0000d880: 6561 7465 645f 6f6e 223a 2022 3230 3137  eated_on": "2017
+0000d890: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+0000d8a0: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0000d8c0: 6574 6122 3a20 7b22 6175 746f 5f61 6464  eta": {"auto_add
+0000d8d0: 6564 223a 2046 616c 7365 7d2c 0a20 2020  ed": False},.   
+0000d8e0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+0000d8f0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+0000d900: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000d910: 7a6f 6e65 203d 205a 6f6e 6528 2775 6e69  zone = Zone('uni
+0000d920: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
+0000d930: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
+0000d940: 706f 7075 6c61 7465 287a 6f6e 6529 0a20  populate(zone). 
+0000d950: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000d960: 7274 4571 7561 6c28 312c 206c 656e 287a  rtEqual(1, len(z
+0000d970: 6f6e 652e 7265 636f 7264 7329 290a 2020  one.records)).  
+0000d980: 2020 2020 2020 7265 636f 7264 203d 206c        record = l
+0000d990: 6973 7428 7a6f 6e65 2e72 6563 6f72 6473  ist(zone.records
+0000d9a0: 295b 305d 0a20 2020 2020 2020 2073 656c  )[0].        sel
+0000d9b0: 662e 6173 7365 7274 4571 7561 6c28 2727  f.assertEqual(''
+0000d9c0: 2c20 7265 636f 7264 2e6e 616d 6529 0a20  , record.name). 
+0000d9d0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000d9e0: 7274 4571 7561 6c28 2775 6e69 742e 7465  rtEqual('unit.te
+0000d9f0: 7374 732e 272c 2072 6563 6f72 642e 6671  sts.', record.fq
+0000da00: 646e 290a 2020 2020 2020 2020 7365 6c66  dn).        self
+0000da10: 2e61 7373 6572 7445 7175 616c 2827 414c  .assertEqual('AL
+0000da20: 4941 5327 2c20 7265 636f 7264 2e5f 7479  IAS', record._ty
+0000da30: 7065 290a 2020 2020 2020 2020 7365 6c66  pe).        self
+0000da40: 2e61 7373 6572 7445 7175 616c 2827 756e  .assertEqual('un
+0000da50: 6974 2e74 6573 7473 2e63 646e 2e63 6c6f  it.tests.cdn.clo
+0000da60: 7564 666c 6172 652e 6e65 742e 272c 2072  udflare.net.', r
+0000da70: 6563 6f72 642e 7661 6c75 6529 0a0a 2020  ecord.value)..  
+0000da80: 2020 2020 2020 2320 4344 4e20 656e 6162        # CDN enab
+0000da90: 6c65 6420 7265 636f 7264 7320 6361 6e27  led records can'
+0000daa0: 7420 6265 2075 7064 6174 6564 2c20 7765  t be updated, we
+0000dab0: 2064 6f6e 2774 206b 6e6f 7720 7468 6520   don't know the 
+0000dac0: 7265 616c 2076 616c 7565 730a 2020 2020  real values.    
+0000dad0: 2020 2020 2320 6e65 7665 7220 706f 696e      # never poin
+0000dae0: 7420 6120 436c 6f75 6466 6c61 7265 2072  t a Cloudflare r
+0000daf0: 6563 6f72 6420 746f 2069 7473 656c 662e  ecord to itself.
+0000db00: 0a20 2020 2020 2020 2077 616e 7465 6420  .        wanted 
+0000db10: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
+0000db20: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
+0000db30: 2020 7761 6e74 6564 2e61 6464 5f72 6563    wanted.add_rec
+0000db40: 6f72 6428 0a20 2020 2020 2020 2020 2020  ord(.           
+0000db50: 2052 6563 6f72 642e 6e65 7728 0a20 2020   Record.new(.   
+0000db60: 2020 2020 2020 2020 2020 2020 2077 616e               wan
+0000db70: 7465 642c 0a20 2020 2020 2020 2020 2020  ted,.           
+0000db80: 2020 2020 2027 272c 0a20 2020 2020 2020       '',.       
+0000db90: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0000dba0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000dbb0: 7474 6c27 3a20 3330 302c 0a20 2020 2020  ttl': 300,.     
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0000dbd0: 7479 7065 273a 2027 414c 4941 5327 2c0a  type': 'ALIAS',.
+0000dbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbf0: 2020 2020 2776 616c 7565 273a 2027 6368      'value': 'ch
+0000dc00: 616e 6765 2e75 6e69 742e 7465 7374 732e  ange.unit.tests.
+0000dc10: 6364 6e2e 636c 6f75 6466 6c61 7265 2e6e  cdn.cloudflare.n
+0000dc20: 6574 2e27 2c0a 2020 2020 2020 2020 2020  et.',.          
+0000dc30: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+0000dc40: 2020 2020 2029 0a20 2020 2020 2020 2029       ).        )
+0000dc50: 0a0a 2020 2020 2020 2020 706c 616e 203d  ..        plan =
+0000dc60: 2070 726f 7669 6465 722e 706c 616e 2877   provider.plan(w
+0000dc70: 616e 7465 6429 0a20 2020 2020 2020 2073  anted).        s
+0000dc80: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+0000dc90: 4661 6c73 652c 2068 6173 6174 7472 2870  False, hasattr(p
+0000dca0: 6c61 6e2c 2027 6368 616e 6765 7327 2929  lan, 'changes'))
+0000dcb0: 0a0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
+0000dcc0: 6e70 726f 7869 6162 6c65 7479 7065 5f72  nproxiabletype_r
+0000dcd0: 6563 6f72 6466 6f72 5f72 6574 7572 6e73  ecordfor_returns
+0000dce0: 7265 636f 7264 7769 7468 6e6f 636c 6f75  recordwithnoclou
+0000dcf0: 6466 6c61 7265 2873 656c 6629 3a0a 2020  dflare(self):.  
+0000dd00: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
+0000dd10: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
+0000dd20: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
+0000dd30: 696c 272c 2027 746f 6b65 6e27 290a 2020  il', 'token').  
+0000dd40: 2020 2020 2020 6e61 6d65 203d 2022 756e        name = "un
+0000dd50: 6974 2e74 6573 7473 220a 2020 2020 2020  it.tests".      
+0000dd60: 2020 5f74 7970 6520 3d20 224e 5322 0a20    _type = "NS". 
+0000dd70: 2020 2020 2020 207a 6f6e 655f 7265 636f         zone_reco
+0000dd80: 7264 7320 3d20 5b0a 2020 2020 2020 2020  rds = [.        
+0000dd90: 2020 2020 7b0a 2020 2020 2020 2020 2020      {.          
+0000dda0: 2020 2020 2020 2269 6422 3a20 2266 6331        "id": "fc1
+0000ddb0: 3261 6233 3463 6435 3631 3133 3334 3432  2ab34cd561133442
+0000ddc0: 3261 6233 3332 3239 3937 3635 3422 2c0a  2ab3322997654",.
+0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dde0: 2274 7970 6522 3a20 5f74 7970 652c 0a20  "type": _type,. 
+0000ddf0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000de00: 6e61 6d65 223a 206e 616d 652c 0a20 2020  name": name,.   
+0000de10: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+0000de20: 6e74 656e 7422 3a20 226e 7332 2e66 6f6f  ntent": "ns2.foo
+0000de30: 2e62 6172 222c 0a20 2020 2020 2020 2020  .bar",.         
+0000de40: 2020 2020 2020 2022 7072 6f78 6961 626c         "proxiabl
+0000de50: 6522 3a20 5472 7565 2c0a 2020 2020 2020  e": True,.      
+0000de60: 2020 2020 2020 2020 2020 2270 726f 7869            "proxi
+0000de70: 6564 223a 2046 616c 7365 2c0a 2020 2020  ed": False,.    
+0000de80: 2020 2020 2020 2020 2020 2020 2274 746c              "ttl
+0000de90: 223a 2033 3030 2c0a 2020 2020 2020 2020  ": 300,.        
+0000dea0: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
+0000deb0: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+0000dec0: 2020 2020 2020 2020 2022 7a6f 6e65 5f69           "zone_i
+0000ded0: 6422 3a20 2266 6631 3261 6233 3463 6435  d": "ff12ab34cd5
+0000dee0: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
+0000def0: 3937 3635 3022 2c0a 2020 2020 2020 2020  97650",.        
+0000df00: 2020 2020 2020 2020 227a 6f6e 655f 6e61          "zone_na
+0000df10: 6d65 223a 2022 756e 6974 2e74 6573 7473  me": "unit.tests
+0000df20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000df30: 2020 2022 6d6f 6469 6669 6564 5f6f 6e22     "modified_on"
+0000df40: 3a20 2232 3031 372d 3033 2d31 3154 3138  : "2017-03-11T18
+0000df50: 3a30 313a 3433 2e34 3230 3638 395a 222c  :01:43.420689Z",
+0000df60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df70: 2022 6372 6561 7465 645f 6f6e 223a 2022   "created_on": "
+0000df80: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
+0000df90: 3a34 332e 3432 3036 3839 5a22 2c0a 2020  :43.420689Z",.  
+0000dfa0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+0000dfb0: 6574 6122 3a20 7b22 6175 746f 5f61 6464  eta": {"auto_add
+0000dfc0: 6564 223a 2046 616c 7365 7d2c 0a20 2020  ed": False},.   
+0000dfd0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+0000dfe0: 2020 205d 0a20 2020 2020 2020 2070 726f     ].        pro
+0000dff0: 7669 6465 722e 7a6f 6e65 5f72 6563 6f72  vider.zone_recor
+0000e000: 6473 203d 204d 6f63 6b28 7265 7475 726e  ds = Mock(return
+0000e010: 5f76 616c 7565 3d7a 6f6e 655f 7265 636f  _value=zone_reco
+0000e020: 7264 7329 0a20 2020 2020 2020 207a 6f6e  rds).        zon
+0000e030: 6520 3d20 5a6f 6e65 2827 756e 6974 2e74  e = Zone('unit.t
+0000e040: 6573 7473 2e27 2c20 5b5d 290a 2020 2020  ests.', []).    
+0000e050: 2020 2020 7072 6f76 6964 6572 2e70 6f70      provider.pop
+0000e060: 756c 6174 6528 7a6f 6e65 290a 0a20 2020  ulate(zone)..   
+0000e070: 2020 2020 2072 6563 6f72 6420 3d20 7072       record = pr
+0000e080: 6f76 6964 6572 2e5f 7265 636f 7264 5f66  ovider._record_f
+0000e090: 6f72 287a 6f6e 652c 206e 616d 652c 205f  or(zone, name, _
+0000e0a0: 7479 7065 2c20 7a6f 6e65 5f72 6563 6f72  type, zone_recor
+0000e0b0: 6473 2c20 4661 6c73 6529 0a0a 2020 2020  ds, False)..    
+0000e0c0: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
+0000e0d0: 616c 7365 2872 6563 6f72 642e 5f6f 6374  alse(record._oct
+0000e0e0: 6f64 6e73 2e67 6574 2827 6175 746f 2d74  odns.get('auto-t
+0000e0f0: 746c 272c 2046 616c 7365 2929 0a20 2020  tl', False)).   
+0000e100: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+0000e110: 4661 6c73 6528 7265 636f 7264 2e5f 6f63  False(record._oc
+0000e120: 746f 646e 732e 6765 7428 2770 726f 7869  todns.get('proxi
+0000e130: 6564 272c 2046 616c 7365 2929 0a0a 2020  ed', False))..  
+0000e140: 2020 6465 6620 7465 7374 5f70 726f 7869    def test_proxi
+0000e150: 6162 6c65 7479 7065 5f72 6563 6f72 6466  abletype_recordf
+0000e160: 6f72 5f72 6574 7265 636f 7264 7769 7468  or_retrecordwith
+0000e170: 636c 6f75 6466 6c61 7265 756e 7072 6f78  cloudflareunprox
+0000e180: 6965 6428 7365 6c66 293a 0a20 2020 2020  ied(self):.     
+0000e190: 2020 2070 726f 7669 6465 7220 3d20 436c     provider = Cl
+0000e1a0: 6f75 6466 6c61 7265 5072 6f76 6964 6572  oudflareProvider
+0000e1b0: 2827 7465 7374 272c 2027 656d 6169 6c27  ('test', 'email'
+0000e1c0: 2c20 2774 6f6b 656e 2729 0a20 2020 2020  , 'token').     
+0000e1d0: 2020 206e 616d 6520 3d20 226d 756c 7469     name = "multi
+0000e1e0: 2e75 6e69 742e 7465 7374 7322 0a20 2020  .unit.tests".   
+0000e1f0: 2020 2020 205f 7479 7065 203d 2022 4141       _type = "AA
+0000e200: 4141 220a 2020 2020 2020 2020 7a6f 6e65  AA".        zone
+0000e210: 5f72 6563 6f72 6473 203d 205b 0a20 2020  _records = [.   
+0000e220: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+0000e230: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+0000e240: 2022 6663 3132 6162 3334 6364 3536 3131   "fc12ab34cd5611
+0000e250: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+0000e260: 3432 222c 0a20 2020 2020 2020 2020 2020  42",.           
+0000e270: 2020 2020 2022 7479 7065 223a 205f 7479       "type": _ty
+0000e280: 7065 2c0a 2020 2020 2020 2020 2020 2020  pe,.            
+0000e290: 2020 2020 226e 616d 6522 3a20 6e61 6d65      "name": name
+0000e2a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e2b0: 2020 2263 6f6e 7465 6e74 223a 2022 3a3a    "content": "::
+0000e2c0: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+0000e2d0: 2020 2020 2270 726f 7869 6162 6c65 223a      "proxiable":
+0000e2e0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+0000e2f0: 2020 2020 2020 2022 7072 6f78 6965 6422         "proxied"
+0000e300: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+0000e310: 2020 2020 2020 2020 2022 7474 6c22 3a20           "ttl": 
+0000e320: 3330 302c 0a20 2020 2020 2020 2020 2020  300,.           
+0000e330: 2020 2020 2022 6c6f 636b 6564 223a 2046       "locked": F
+0000e340: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+0000e350: 2020 2020 2020 227a 6f6e 655f 6964 223a        "zone_id":
+0000e360: 2022 6666 3132 6162 3334 6364 3536 3131   "ff12ab34cd5611
+0000e370: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+0000e380: 3530 222c 0a20 2020 2020 2020 2020 2020  50",.           
+0000e390: 2020 2020 2022 7a6f 6e65 5f6e 616d 6522       "zone_name"
+0000e3a0: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
+0000e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3c0: 226d 6f64 6966 6965 645f 6f6e 223a 2022  "modified_on": "
+0000e3d0: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
+0000e3e0: 3a34 332e 3432 3036 3839 5a22 2c0a 2020  :43.420689Z",.  
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+0000e400: 7265 6174 6564 5f6f 6e22 3a20 2232 3031  reated_on": "201
+0000e410: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
+0000e420: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
+0000e430: 2020 2020 2020 2020 2020 2022 6d65 7461             "meta
+0000e440: 223a 207b 2261 7574 6f5f 6164 6465 6422  ": {"auto_added"
+0000e450: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
+0000e460: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+0000e470: 5d0a 2020 2020 2020 2020 7072 6f76 6964  ].        provid
+0000e480: 6572 2e7a 6f6e 655f 7265 636f 7264 7320  er.zone_records 
+0000e490: 3d20 4d6f 636b 2872 6574 7572 6e5f 7661  = Mock(return_va
+0000e4a0: 6c75 653d 7a6f 6e65 5f72 6563 6f72 6473  lue=zone_records
+0000e4b0: 290a 2020 2020 2020 2020 7a6f 6e65 203d  ).        zone =
+0000e4c0: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+0000e4d0: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
+0000e4e0: 2070 726f 7669 6465 722e 706f 7075 6c61   provider.popula
+0000e4f0: 7465 287a 6f6e 6529 0a0a 2020 2020 2020  te(zone)..      
+0000e500: 2020 7265 636f 7264 203d 2070 726f 7669    record = provi
+0000e510: 6465 722e 5f72 6563 6f72 645f 666f 7228  der._record_for(
+0000e520: 7a6f 6e65 2c20 6e61 6d65 2c20 5f74 7970  zone, name, _typ
+0000e530: 652c 207a 6f6e 655f 7265 636f 7264 732c  e, zone_records,
+0000e540: 2046 616c 7365 290a 0a20 2020 2020 2020   False)..       
+0000e550: 2073 656c 662e 6173 7365 7274 4661 6c73   self.assertFals
+0000e560: 6528 0a20 2020 2020 2020 2020 2020 2072  e(.            r
+0000e570: 6563 6f72 642e 5f6f 6374 6f64 6e73 2e67  ecord._octodns.g
+0000e580: 6574 2827 636c 6f75 6466 6c61 7265 272c  et('cloudflare',
+0000e590: 207b 7d29 2e67 6574 2827 7072 6f78 6965   {}).get('proxie
+0000e5a0: 6427 2c20 4661 6c73 6529 0a20 2020 2020  d', False).     
+0000e5b0: 2020 2029 0a0a 2020 2020 6465 6620 7465     )..    def te
+0000e5c0: 7374 5f70 726f 7869 6162 6c65 7479 7065  st_proxiabletype
+0000e5d0: 5f72 6563 6f72 6466 6f72 5f72 6574 7572  _recordfor_retur
+0000e5e0: 6e73 7265 636f 7264 7769 7468 636c 6f75  nsrecordwithclou
+0000e5f0: 6466 6c61 7265 7072 6f78 6965 6428 7365  dflareproxied(se
+0000e600: 6c66 293a 0a20 2020 2020 2020 2070 726f  lf):.        pro
+0000e610: 7669 6465 7220 3d20 436c 6f75 6466 6c61  vider = Cloudfla
+0000e620: 7265 5072 6f76 6964 6572 2827 7465 7374  reProvider('test
+0000e630: 272c 2027 656d 6169 6c27 2c20 2774 6f6b  ', 'email', 'tok
+0000e640: 656e 2729 0a20 2020 2020 2020 206e 616d  en').        nam
+0000e650: 6520 3d20 226d 756c 7469 2e75 6e69 742e  e = "multi.unit.
+0000e660: 7465 7374 7322 0a20 2020 2020 2020 205f  tests".        _
+0000e670: 7479 7065 203d 2022 4141 4141 220a 2020  type = "AAAA".  
+0000e680: 2020 2020 2020 7a6f 6e65 5f72 6563 6f72        zone_recor
+0000e690: 6473 203d 205b 0a20 2020 2020 2020 2020  ds = [.         
+0000e6a0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+0000e6b0: 2020 2020 2022 6964 223a 2022 6663 3132       "id": "fc12
+0000e6c0: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
+0000e6d0: 6162 3333 3232 3939 3736 3432 222c 0a20  ab3322997642",. 
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000e6f0: 7479 7065 223a 205f 7479 7065 2c0a 2020  type": _type,.  
+0000e700: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+0000e710: 616d 6522 3a20 6e61 6d65 2c0a 2020 2020  ame": name,.    
+0000e720: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+0000e730: 7465 6e74 223a 2022 3a3a 3122 2c0a 2020  tent": "::1",.  
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+0000e750: 726f 7869 6162 6c65 223a 2054 7275 652c  roxiable": True,
+0000e760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e770: 2022 7072 6f78 6965 6422 3a20 5472 7565   "proxied": True
+0000e780: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e790: 2020 2274 746c 223a 2031 2c0a 2020 2020    "ttl": 1,.    
+0000e7a0: 2020 2020 2020 2020 2020 2020 226c 6f63              "loc
+0000e7b0: 6b65 6422 3a20 4661 6c73 652c 0a20 2020  ked": False,.   
+0000e7c0: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+0000e7d0: 6e65 5f69 6422 3a20 2266 6631 3261 6233  ne_id": "ff12ab3
+0000e7e0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+0000e7f0: 3332 3239 3937 3635 3022 2c0a 2020 2020  322997650",.    
+0000e800: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+0000e810: 655f 6e61 6d65 223a 2022 756e 6974 2e74  e_name": "unit.t
+0000e820: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+0000e830: 2020 2020 2020 2022 6d6f 6469 6669 6564         "modified
+0000e840: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
+0000e850: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
+0000e860: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
+0000e870: 2020 2020 2022 6372 6561 7465 645f 6f6e       "created_on
+0000e880: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
+0000e890: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
+0000e8a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e8b0: 2020 226d 6574 6122 3a20 7b22 6175 746f    "meta": {"auto
+0000e8c0: 5f61 6464 6564 223a 2046 616c 7365 7d2c  _added": False},
+0000e8d0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+0000e8e0: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+0000e8f0: 2070 726f 7669 6465 722e 7a6f 6e65 5f72   provider.zone_r
+0000e900: 6563 6f72 6473 203d 204d 6f63 6b28 7265  ecords = Mock(re
+0000e910: 7475 726e 5f76 616c 7565 3d7a 6f6e 655f  turn_value=zone_
+0000e920: 7265 636f 7264 7329 0a20 2020 2020 2020  records).       
+0000e930: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
+0000e940: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
+0000e950: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+0000e960: 2e70 6f70 756c 6174 6528 7a6f 6e65 290a  .populate(zone).
+0000e970: 0a20 2020 2020 2020 2072 6563 6f72 6420  .        record 
+0000e980: 3d20 7072 6f76 6964 6572 2e5f 7265 636f  = provider._reco
+0000e990: 7264 5f66 6f72 287a 6f6e 652c 206e 616d  rd_for(zone, nam
+0000e9a0: 652c 205f 7479 7065 2c20 7a6f 6e65 5f72  e, _type, zone_r
+0000e9b0: 6563 6f72 6473 2c20 4661 6c73 6529 0a0a  ecords, False)..
+0000e9c0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000e9d0: 6572 7454 7275 6528 7265 636f 7264 2e5f  ertTrue(record._
+0000e9e0: 6f63 746f 646e 735b 2763 6c6f 7564 666c  octodns['cloudfl
+0000e9f0: 6172 6527 5d5b 2761 7574 6f2d 7474 6c27  are']['auto-ttl'
+0000ea00: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
+0000ea10: 6173 7365 7274 5472 7565 2872 6563 6f72  assertTrue(recor
+0000ea20: 642e 5f6f 6374 6f64 6e73 5b27 636c 6f75  d._octodns['clou
+0000ea30: 6466 6c61 7265 275d 5b27 7072 6f78 6965  dflare']['proxie
+0000ea40: 6427 5d29 0a0a 2020 2020 6465 6620 7465  d'])..    def te
+0000ea50: 7374 5f72 6563 6f72 645f 666f 725f 6175  st_record_for_au
+0000ea60: 746f 5f74 746c 5f6e 6f5f 7072 6f78 6965  to_ttl_no_proxie
+0000ea70: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
+0000ea80: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
+0000ea90: 6466 6c61 7265 5072 6f76 6964 6572 2827  dflareProvider('
+0000eaa0: 7465 7374 272c 2027 656d 6169 6c27 2c20  test', 'email', 
+0000eab0: 2774 6f6b 656e 2729 0a20 2020 2020 2020  'token').       
+0000eac0: 206e 616d 6520 3d20 2270 726f 7869 6564   name = "proxied
+0000ead0: 2e75 6e69 742e 7465 7374 7322 0a20 2020  .unit.tests".   
+0000eae0: 2020 2020 205f 7479 7065 203d 2022 4122       _type = "A"
+0000eaf0: 0a20 2020 2020 2020 207a 6f6e 655f 7265  .        zone_re
+0000eb00: 636f 7264 7320 3d20 5b0a 2020 2020 2020  cords = [.      
+0000eb10: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+0000eb20: 2020 2020 2020 2020 2269 6422 3a20 2266          "id": "f
+0000eb30: 6331 3261 6233 3463 6435 3631 3133 3334  c12ab34cd5611334
+0000eb40: 3432 3261 6233 3332 3239 3937 3634 3222  422ab3322997642"
+0000eb50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000eb60: 2020 2274 7970 6522 3a20 5f74 7970 652c    "type": _type,
+0000eb70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb80: 2022 6e61 6d65 223a 206e 616d 652c 0a20   "name": name,. 
+0000eb90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000eba0: 636f 6e74 656e 7422 3a20 2234 2e33 2e32  content": "4.3.2
+0000ebb0: 2e31 222c 0a20 2020 2020 2020 2020 2020  .1",.           
+0000ebc0: 2020 2020 2022 7072 6f78 6961 626c 6522       "proxiable"
+0000ebd0: 3a20 5472 7565 2c0a 2020 2020 2020 2020  : True,.        
+0000ebe0: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
+0000ebf0: 223a 2046 616c 7365 2c0a 2020 2020 2020  ": False,.      
+0000ec00: 2020 2020 2020 2020 2020 2274 746c 223a            "ttl":
+0000ec10: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+0000ec20: 2020 2020 226c 6f63 6b65 6422 3a20 4661      "locked": Fa
+0000ec30: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+0000ec40: 2020 2020 2022 7a6f 6e65 5f69 6422 3a20       "zone_id": 
+0000ec50: 2266 6631 3261 6233 3463 6435 3631 3133  "ff12ab34cd56113
+0000ec60: 3334 3432 3261 6233 3332 3239 3937 3635  34422ab332299765
+0000ec70: 3022 2c0a 2020 2020 2020 2020 2020 2020  0",.            
+0000ec80: 2020 2020 227a 6f6e 655f 6e61 6d65 223a      "zone_name":
+0000ec90: 2022 756e 6974 2e74 6573 7473 222c 0a20   "unit.tests",. 
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ecb0: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
+0000ecc0: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
+0000ecd0: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
+0000ece0: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+0000ecf0: 6561 7465 645f 6f6e 223a 2022 3230 3137  eated_on": "2017
+0000ed00: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+0000ed10: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+0000ed20: 2020 2020 2020 2020 2020 226d 6574 6122            "meta"
+0000ed30: 3a20 7b22 6175 746f 5f61 6464 6564 223a  : {"auto_added":
+0000ed40: 2046 616c 7365 7d2c 0a20 2020 2020 2020   False},.       
+0000ed50: 2020 2020 207d 0a20 2020 2020 2020 205d       }.        ]
+0000ed60: 0a0a 2020 2020 2020 2020 7a6f 6e65 203d  ..        zone =
+0000ed70: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+0000ed80: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
+0000ed90: 2072 6563 6f72 6420 3d20 7072 6f76 6964   record = provid
+0000eda0: 6572 2e5f 7265 636f 7264 5f66 6f72 287a  er._record_for(z
+0000edb0: 6f6e 652c 206e 616d 652c 205f 7479 7065  one, name, _type
+0000edc0: 2c20 7a6f 6e65 5f72 6563 6f72 6473 2c20  , zone_records, 
+0000edd0: 4661 6c73 6529 0a0a 2020 2020 2020 2020  False)..        
+0000ede0: 7365 6c66 2e61 7373 6572 7454 7275 6528  self.assertTrue(
+0000edf0: 7265 636f 7264 2e5f 6f63 746f 646e 735b  record._octodns[
+0000ee00: 2763 6c6f 7564 666c 6172 6527 5d5b 2761  'cloudflare']['a
+0000ee10: 7574 6f2d 7474 6c27 5d29 0a20 2020 2020  uto-ttl']).     
+0000ee20: 2020 2073 656c 662e 6173 7365 7274 4661     self.assertFa
+0000ee30: 6c73 6528 7265 636f 7264 2e5f 6f63 746f  lse(record._octo
+0000ee40: 646e 735b 2763 6c6f 7564 666c 6172 6527  dns['cloudflare'
+0000ee50: 5d2e 6765 7428 2770 726f 7869 6564 272c  ].get('proxied',
+0000ee60: 2046 616c 7365 2929 0a0a 2020 2020 6465   False))..    de
+0000ee70: 6620 7465 7374 5f70 726f 7869 6564 7265  f test_proxiedre
+0000ee80: 636f 7264 616e 646e 6577 7474 6c5f 696e  cordandnewttl_in
+0000ee90: 636c 7564 6563 6861 6e67 655f 7265 7475  cludechange_retu
+0000eea0: 726e 7366 616c 7365 2873 656c 6629 3a0a  rnsfalse(self):.
+0000eeb0: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+0000eec0: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
+0000eed0: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
+0000eee0: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
+0000eef0: 2020 2020 2020 2020 7a6f 6e65 203d 205a          zone = Z
+0000ef00: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
+0000ef10: 272c 205b 5d29 0a20 2020 2020 2020 2065  ', []).        e
+0000ef20: 7869 7374 696e 6720 3d20 7365 745f 7265  xisting = set_re
+0000ef30: 636f 7264 5f70 726f 7869 6564 5f66 6c61  cord_proxied_fla
+0000ef40: 6728 0a20 2020 2020 2020 2020 2020 2052  g(.            R
+0000ef50: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
+0000ef60: 2020 2020 2020 2020 2020 207a 6f6e 652c             zone,
+0000ef70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef80: 2027 6127 2c0a 2020 2020 2020 2020 2020   'a',.          
+0000ef90: 2020 2020 2020 7b27 7474 6c27 3a20 312c        {'ttl': 1,
+0000efa0: 2027 7479 7065 273a 2027 4127 2c20 2776   'type': 'A', 'v
+0000efb0: 616c 7565 7327 3a20 5b27 312e 312e 312e  alues': ['1.1.1.
+0000efc0: 3127 2c20 2732 2e32 2e32 2e32 275d 7d2c  1', '2.2.2.2']},
+0000efd0: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+0000efe0: 2020 2020 2020 2020 2020 2020 5472 7565              True
+0000eff0: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+0000f000: 2020 2020 6e65 7720 3d20 7365 745f 7265      new = set_re
+0000f010: 636f 7264 5f70 726f 7869 6564 5f66 6c61  cord_proxied_fla
+0000f020: 6728 0a20 2020 2020 2020 2020 2020 2052  g(.            R
+0000f030: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
+0000f040: 2020 2020 2020 2020 2020 207a 6f6e 652c             zone,
+0000f050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f060: 2027 6127 2c0a 2020 2020 2020 2020 2020   'a',.          
+0000f070: 2020 2020 2020 7b27 7474 6c27 3a20 3330        {'ttl': 30
+0000f080: 302c 2027 7479 7065 273a 2027 4127 2c20  0, 'type': 'A', 
+0000f090: 2776 616c 7565 7327 3a20 5b27 312e 312e  'values': ['1.1.
+0000f0a0: 312e 3127 2c20 2732 2e32 2e32 2e32 275d  1.1', '2.2.2.2']
+0000f0b0: 7d2c 0a20 2020 2020 2020 2020 2020 2029  },.            )
+0000f0c0: 2c0a 2020 2020 2020 2020 2020 2020 5472  ,.            Tr
+0000f0d0: 7565 2c0a 2020 2020 2020 2020 290a 2020  ue,.        ).  
+0000f0e0: 2020 2020 2020 6368 616e 6765 203d 2055        change = U
+0000f0f0: 7064 6174 6528 6578 6973 7469 6e67 2c20  pdate(existing, 
+0000f100: 6e65 7729 0a0a 2020 2020 2020 2020 696e  new)..        in
+0000f110: 636c 7564 655f 6368 616e 6765 203d 2070  clude_change = p
+0000f120: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
+0000f130: 5f63 6861 6e67 6528 6368 616e 6765 290a  _change(change).
+0000f140: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+0000f150: 7365 7274 4661 6c73 6528 696e 636c 7564  sertFalse(includ
+0000f160: 655f 6368 616e 6765 290a 0a20 2020 2064  e_change)..    d
+0000f170: 6566 2074 6573 745f 6175 746f 5f74 746c  ef test_auto_ttl
+0000f180: 5f69 676e 6f72 6573 5f74 746c 5f63 6861  _ignores_ttl_cha
+0000f190: 6e67 6528 7365 6c66 293a 0a20 2020 2020  nge(self):.     
+0000f1a0: 2020 2070 726f 7669 6465 7220 3d20 436c     provider = Cl
+0000f1b0: 6f75 6466 6c61 7265 5072 6f76 6964 6572  oudflareProvider
+0000f1c0: 2827 7465 7374 272c 2027 656d 6169 6c27  ('test', 'email'
+0000f1d0: 2c20 2774 6f6b 656e 2729 0a20 2020 2020  , 'token').     
+0000f1e0: 2020 207a 6f6e 6520 3d20 5a6f 6e65 2827     zone = Zone('
+0000f1f0: 756e 6974 2e74 6573 7473 2e27 2c20 5b5d  unit.tests.', []
+0000f200: 290a 2020 2020 2020 2020 6578 6973 7469  ).        existi
+0000f210: 6e67 203d 2073 6574 5f72 6563 6f72 645f  ng = set_record_
+0000f220: 6175 746f 5f74 746c 5f66 6c61 6728 0a20  auto_ttl_flag(. 
+0000f230: 2020 2020 2020 2020 2020 2052 6563 6f72             Recor
+0000f240: 642e 6e65 7728 0a20 2020 2020 2020 2020  d.new(.         
+0000f250: 2020 2020 2020 207a 6f6e 652c 0a20 2020         zone,.   
+0000f260: 2020 2020 2020 2020 2020 2020 2027 6127               'a'
+0000f270: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f280: 2020 7b27 7474 6c27 3a20 312c 2027 7479    {'ttl': 1, 'ty
+0000f290: 7065 273a 2027 4127 2c20 2776 616c 7565  pe': 'A', 'value
+0000f2a0: 7327 3a20 5b27 312e 312e 312e 3127 2c20  s': ['1.1.1.1', 
+0000f2b0: 2732 2e32 2e32 2e32 275d 7d2c 0a20 2020  '2.2.2.2']},.   
+0000f2c0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+0000f2d0: 2020 2020 2020 2020 5472 7565 2c0a 2020          True,.  
+0000f2e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000f2f0: 6e65 7720 3d20 7365 745f 7265 636f 7264  new = set_record
+0000f300: 5f61 7574 6f5f 7474 6c5f 666c 6167 280a  _auto_ttl_flag(.
+0000f310: 2020 2020 2020 2020 2020 2020 5265 636f              Reco
+0000f320: 7264 2e6e 6577 280a 2020 2020 2020 2020  rd.new(.        
+0000f330: 2020 2020 2020 2020 7a6f 6e65 2c0a 2020          zone,.  
+0000f340: 2020 2020 2020 2020 2020 2020 2020 2761                'a
+0000f350: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0000f360: 2020 207b 2774 746c 273a 2033 3030 2c20     {'ttl': 300, 
+0000f370: 2774 7970 6527 3a20 2741 272c 2027 7661  'type': 'A', 'va
+0000f380: 6c75 6573 273a 205b 2731 2e31 2e31 2e31  lues': ['1.1.1.1
+0000f390: 272c 2027 322e 322e 322e 3227 5d7d 2c0a  ', '2.2.2.2']},.
+0000f3a0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+0000f3b0: 2020 2020 2020 2020 2020 2054 7275 652c             True,
+0000f3c0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000f3d0: 2020 2063 6861 6e67 6520 3d20 5570 6461     change = Upda
+0000f3e0: 7465 2865 7869 7374 696e 672c 206e 6577  te(existing, new
+0000f3f0: 290a 0a20 2020 2020 2020 2069 6e63 6c75  )..        inclu
+0000f400: 6465 5f63 6861 6e67 6520 3d20 7072 6f76  de_change = prov
+0000f410: 6964 6572 2e5f 696e 636c 7564 655f 6368  ider._include_ch
+0000f420: 616e 6765 2863 6861 6e67 6529 0a0a 2020  ange(change)..  
+0000f430: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000f440: 7446 616c 7365 2869 6e63 6c75 6465 5f63  tFalse(include_c
+0000f450: 6861 6e67 6529 0a0a 2020 2020 2020 2020  hange)..        
+0000f460: 2320 6966 2066 6c61 6720 6973 2066 616c  # if flag is fal
+0000f470: 7365 2c20 776f 756c 6420 7265 7475 726e  se, would return
+0000f480: 2074 6865 2063 6861 6e67 650a 2020 2020   the change.    
+0000f490: 2020 2020 6578 6973 7469 6e67 203d 2073      existing = s
+0000f4a0: 6574 5f72 6563 6f72 645f 6175 746f 5f74  et_record_auto_t
+0000f4b0: 746c 5f66 6c61 6728 6578 6973 7469 6e67  tl_flag(existing
+0000f4c0: 2c20 4661 6c73 6529 0a20 2020 2020 2020  , False).       
+0000f4d0: 2069 6e63 6c75 6465 5f63 6861 6e67 6520   include_change 
+0000f4e0: 3d20 7072 6f76 6964 6572 2e5f 696e 636c  = provider._incl
+0000f4f0: 7564 655f 6368 616e 6765 2863 6861 6e67  ude_change(chang
+0000f500: 6529 0a20 2020 2020 2020 2073 656c 662e  e).        self.
+0000f510: 6173 7365 7274 5472 7565 2869 6e63 6c75  assertTrue(inclu
+0000f520: 6465 5f63 6861 6e67 6529 0a0a 2020 2020  de_change)..    
+0000f530: 6465 6620 7465 7374 5f69 6e63 6c75 6465  def test_include
+0000f540: 5f63 6861 6e67 655f 7370 6563 6961 6c5f  _change_special_
+0000f550: 666c 6167 7328 7365 6c66 293a 0a20 2020  flags(self):.   
+0000f560: 2020 2020 2070 726f 7669 6465 7220 3d20       provider = 
+0000f570: 436c 6f75 6466 6c61 7265 5072 6f76 6964  CloudflareProvid
+0000f580: 6572 2827 7465 7374 272c 2027 656d 6169  er('test', 'emai
+0000f590: 6c27 2c20 2774 6f6b 656e 2729 0a0a 2020  l', 'token')..  
+0000f5a0: 2020 2020 2020 7a6f 6e65 203d 205a 6f6e        zone = Zon
+0000f5b0: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
+0000f5c0: 205b 5d29 0a20 2020 2020 2020 2061 315f   []).        a1_
+0000f5d0: 706c 6169 6e20 3d20 5265 636f 7264 2e6e  plain = Record.n
+0000f5e0: 6577 280a 2020 2020 2020 2020 2020 2020  ew(.            
+0000f5f0: 7a6f 6e65 2c20 2777 7777 272c 207b 2774  zone, 'www', {'t
+0000f600: 746c 273a 2033 3030 2c20 2774 7970 6527  tl': 300, 'type'
+0000f610: 3a20 2741 272c 2027 7661 6c75 6527 3a20  : 'A', 'value': 
+0000f620: 2731 2e32 2e33 2e34 277d 0a20 2020 2020  '1.2.3.4'}.     
+0000f630: 2020 2029 0a20 2020 2020 2020 2061 315f     ).        a1_
+0000f640: 7072 6f78 6965 6420 3d20 7365 745f 7265  proxied = set_re
+0000f650: 636f 7264 5f70 726f 7869 6564 5f66 6c61  cord_proxied_fla
+0000f660: 6728 0a20 2020 2020 2020 2020 2020 2052  g(.            R
+0000f670: 6563 6f72 642e 6e65 7728 0a20 2020 2020  ecord.new(.     
+0000f680: 2020 2020 2020 2020 2020 207a 6f6e 652c             zone,
+0000f690: 2027 7777 7727 2c20 7b27 7474 6c27 3a20   'www', {'ttl': 
+0000f6a0: 3330 302c 2027 7479 7065 273a 2027 4127  300, 'type': 'A'
+0000f6b0: 2c20 2776 616c 7565 273a 2027 312e 322e  , 'value': '1.2.
+0000f6c0: 332e 3427 7d0a 2020 2020 2020 2020 2020  3.4'}.          
+0000f6d0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0000f6e0: 2054 7275 652c 0a20 2020 2020 2020 2029   True,.        )
+0000f6f0: 0a20 2020 2020 2020 2061 315f 6175 746f  .        a1_auto
+0000f700: 5f74 746c 203d 2073 6574 5f72 6563 6f72  _ttl = set_recor
+0000f710: 645f 6175 746f 5f74 746c 5f66 6c61 6728  d_auto_ttl_flag(
+0000f720: 0a20 2020 2020 2020 2020 2020 2052 6563  .            Rec
+0000f730: 6f72 642e 6e65 7728 0a20 2020 2020 2020  ord.new(.       
+0000f740: 2020 2020 2020 2020 207a 6f6e 652c 2027           zone, '
+0000f750: 7777 7727 2c20 7b27 7474 6c27 3a20 3330  www', {'ttl': 30
+0000f760: 302c 2027 7479 7065 273a 2027 4127 2c20  0, 'type': 'A', 
+0000f770: 2776 616c 7565 273a 2027 312e 322e 332e  'value': '1.2.3.
+0000f780: 3427 7d0a 2020 2020 2020 2020 2020 2020  4'}.            
+0000f790: 292c 0a20 2020 2020 2020 2020 2020 2054  ),.            T
+0000f7a0: 7275 652c 0a20 2020 2020 2020 2029 0a0a  rue,.        )..
+0000f7b0: 2020 2020 2020 2020 2320 706c 6169 6e20          # plain 
+0000f7c0: 3c2d 3e20 7072 6f78 6965 640a 2020 2020  <-> proxied.    
+0000f7d0: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0000f7e0: 7275 6528 7072 6f76 6964 6572 2e5f 696e  rue(provider._in
+0000f7f0: 636c 7564 655f 6368 616e 6765 2855 7064  clude_change(Upd
+0000f800: 6174 6528 6131 5f70 6c61 696e 2c20 6131  ate(a1_plain, a1
+0000f810: 5f70 726f 7869 6564 2929 290a 2020 2020  _proxied))).    
+0000f820: 2020 2020 7365 6c66 2e61 7373 6572 7454      self.assertT
+0000f830: 7275 6528 7072 6f76 6964 6572 2e5f 696e  rue(provider._in
+0000f840: 636c 7564 655f 6368 616e 6765 2855 7064  clude_change(Upd
+0000f850: 6174 6528 6131 5f70 726f 7869 6564 2c20  ate(a1_proxied, 
+0000f860: 6131 5f70 6c61 696e 2929 290a 2020 2020  a1_plain))).    
+0000f870: 2020 2020 2320 706c 6169 6e20 3c2d 3e20      # plain <-> 
+0000f880: 6175 746f 2d74 746c 0a20 2020 2020 2020  auto-ttl.       
+0000f890: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+0000f8a0: 2870 726f 7669 6465 722e 5f69 6e63 6c75  (provider._inclu
+0000f8b0: 6465 5f63 6861 6e67 6528 5570 6461 7465  de_change(Update
+0000f8c0: 2861 315f 706c 6169 6e2c 2061 315f 6175  (a1_plain, a1_au
+0000f8d0: 746f 5f74 746c 2929 290a 2020 2020 2020  to_ttl))).      
+0000f8e0: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0000f8f0: 6528 7072 6f76 6964 6572 2e5f 696e 636c  e(provider._incl
+0000f900: 7564 655f 6368 616e 6765 2855 7064 6174  ude_change(Updat
+0000f910: 6528 6131 5f61 7574 6f5f 7474 6c2c 2061  e(a1_auto_ttl, a
+0000f920: 315f 706c 6169 6e29 2929 0a20 2020 2020  1_plain))).     
+0000f930: 2020 2023 2070 726f 7869 6564 203c 2d3e     # proxied <->
+0000f940: 2061 7574 6f2d 7474 6c0a 2020 2020 2020   auto-ttl.      
+0000f950: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+0000f960: 6528 0a20 2020 2020 2020 2020 2020 2070  e(.            p
+0000f970: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
+0000f980: 5f63 6861 6e67 6528 5570 6461 7465 2861  _change(Update(a
+0000f990: 315f 7072 6f78 6965 642c 2061 315f 6175  1_proxied, a1_au
+0000f9a0: 746f 5f74 746c 2929 0a20 2020 2020 2020  to_ttl)).       
+0000f9b0: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
+0000f9c0: 6173 7365 7274 5472 7565 280a 2020 2020  assertTrue(.    
+0000f9d0: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+0000f9e0: 2e5f 696e 636c 7564 655f 6368 616e 6765  ._include_change
+0000f9f0: 2855 7064 6174 6528 6131 5f61 7574 6f5f  (Update(a1_auto_
+0000fa00: 7474 6c2c 2061 315f 7072 6f78 6965 6429  ttl, a1_proxied)
+0000fa10: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+0000fa20: 2020 2020 2023 206e 6f20 7370 6563 6961       # no specia
+0000fa30: 6c20 666c 6167 2063 6861 6e67 6573 0a20  l flag changes. 
+0000fa40: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000fa50: 7274 4661 6c73 6528 7072 6f76 6964 6572  rtFalse(provider
+0000fa60: 2e5f 696e 636c 7564 655f 6368 616e 6765  ._include_change
+0000fa70: 2855 7064 6174 6528 6131 5f70 6c61 696e  (Update(a1_plain
+0000fa80: 2c20 6131 5f70 6c61 696e 2929 290a 2020  , a1_plain))).  
+0000fa90: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+0000faa0: 7446 616c 7365 280a 2020 2020 2020 2020  tFalse(.        
+0000fab0: 2020 2020 7072 6f76 6964 6572 2e5f 696e      provider._in
+0000fac0: 636c 7564 655f 6368 616e 6765 2855 7064  clude_change(Upd
+0000fad0: 6174 6528 6131 5f70 726f 7869 6564 2c20  ate(a1_proxied, 
+0000fae0: 6131 5f70 726f 7869 6564 2929 0a20 2020  a1_proxied)).   
+0000faf0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+0000fb00: 656c 662e 6173 7365 7274 4661 6c73 6528  elf.assertFalse(
+0000fb10: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
+0000fb20: 7669 6465 722e 5f69 6e63 6c75 6465 5f63  vider._include_c
+0000fb30: 6861 6e67 6528 5570 6461 7465 2861 315f  hange(Update(a1_
+0000fb40: 6175 746f 5f74 746c 2c20 6131 5f61 7574  auto_ttl, a1_aut
+0000fb50: 6f5f 7474 6c29 290a 2020 2020 2020 2020  o_ttl)).        
+0000fb60: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
+0000fb70: 696e 636c 7564 655f 6368 616e 6765 5f6d  include_change_m
+0000fb80: 696e 5f74 746c 2873 656c 6629 3a0a 2020  in_ttl(self):.  
+0000fb90: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
+0000fba0: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
+0000fbb0: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
+0000fbc0: 696c 272c 2027 746f 6b65 6e27 290a 0a20  il', 'token').. 
+0000fbd0: 2020 2020 2020 207a 6f6e 6520 3d20 5a6f         zone = Zo
+0000fbe0: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
+0000fbf0: 2c20 5b5d 290a 2020 2020 2020 2020 6265  , []).        be
+0000fc00: 6c6f 7731 203d 2052 6563 6f72 642e 6e65  low1 = Record.ne
+0000fc10: 7728 0a20 2020 2020 2020 2020 2020 207a  w(.            z
+0000fc20: 6f6e 652c 2027 7777 7727 2c20 7b27 7474  one, 'www', {'tt
+0000fc30: 6c27 3a20 3432 2c20 2774 7970 6527 3a20  l': 42, 'type': 
+0000fc40: 2741 272c 2027 7661 6c75 6527 3a20 2731  'A', 'value': '1
+0000fc50: 2e32 2e33 2e34 277d 0a20 2020 2020 2020  .2.3.4'}.       
+0000fc60: 2029 0a20 2020 2020 2020 2062 656c 6f77   ).        below
+0000fc70: 3220 3d20 5265 636f 7264 2e6e 6577 280a  2 = Record.new(.
+0000fc80: 2020 2020 2020 2020 2020 2020 7a6f 6e65              zone
+0000fc90: 2c20 2777 7777 272c 207b 2774 746c 273a  , 'www', {'ttl':
+0000fca0: 2031 3139 2c20 2774 7970 6527 3a20 2741   119, 'type': 'A
+0000fcb0: 272c 2027 7661 6c75 6527 3a20 2731 2e32  ', 'value': '1.2
+0000fcc0: 2e33 2e34 277d 0a20 2020 2020 2020 2029  .3.4'}.        )
+0000fcd0: 0a20 2020 2020 2020 2065 6467 6520 3d20  .        edge = 
+0000fce0: 5265 636f 7264 2e6e 6577 280a 2020 2020  Record.new(.    
+0000fcf0: 2020 2020 2020 2020 7a6f 6e65 2c20 2777          zone, 'w
+0000fd00: 7777 272c 207b 2774 746c 273a 2031 3230  ww', {'ttl': 120
+0000fd10: 2c20 2774 7970 6527 3a20 2741 272c 2027  , 'type': 'A', '
+0000fd20: 7661 6c75 6527 3a20 2731 2e32 2e33 2e34  value': '1.2.3.4
+0000fd30: 277d 0a20 2020 2020 2020 2029 0a20 2020  '}.        ).   
+0000fd40: 2020 2020 2061 626f 7665 3120 3d20 5265       above1 = Re
+0000fd50: 636f 7264 2e6e 6577 280a 2020 2020 2020  cord.new(.      
+0000fd60: 2020 2020 2020 7a6f 6e65 2c20 2777 7777        zone, 'www
+0000fd70: 272c 207b 2774 746c 273a 2031 3231 2c20  ', {'ttl': 121, 
+0000fd80: 2774 7970 6527 3a20 2741 272c 2027 7661  'type': 'A', 'va
+0000fd90: 6c75 6527 3a20 2731 2e32 2e33 2e34 277d  lue': '1.2.3.4'}
+0000fda0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+0000fdb0: 2020 2061 626f 7665 3220 3d20 5265 636f     above2 = Reco
+0000fdc0: 7264 2e6e 6577 280a 2020 2020 2020 2020  rd.new(.        
+0000fdd0: 2020 2020 7a6f 6e65 2c20 2777 7777 272c      zone, 'www',
+0000fde0: 207b 2774 746c 273a 2035 3030 2c20 2774   {'ttl': 500, 't
+0000fdf0: 7970 6527 3a20 2741 272c 2027 7661 6c75  ype': 'A', 'valu
+0000fe00: 6527 3a20 2731 2e32 2e33 2e34 277d 0a20  e': '1.2.3.4'}. 
+0000fe10: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+0000fe20: 2020 2320 626f 7468 2062 656c 6f77 0a20    # both below. 
+0000fe30: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+0000fe40: 7274 4661 6c73 6528 7072 6f76 6964 6572  rtFalse(provider
+0000fe50: 2e5f 696e 636c 7564 655f 6368 616e 6765  ._include_change
+0000fe60: 2855 7064 6174 6528 6265 6c6f 7731 2c20  (Update(below1, 
+0000fe70: 6265 6c6f 7731 2929 290a 2020 2020 2020  below1))).      
+0000fe80: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
+0000fe90: 7365 2870 726f 7669 6465 722e 5f69 6e63  se(provider._inc
+0000fea0: 6c75 6465 5f63 6861 6e67 6528 5570 6461  lude_change(Upda
+0000feb0: 7465 2862 656c 6f77 312c 2062 656c 6f77  te(below1, below
+0000fec0: 3229 2929 0a20 2020 2020 2020 2073 656c  2))).        sel
+0000fed0: 662e 6173 7365 7274 4661 6c73 6528 7072  f.assertFalse(pr
+0000fee0: 6f76 6964 6572 2e5f 696e 636c 7564 655f  ovider._include_
+0000fef0: 6368 616e 6765 2855 7064 6174 6528 6265  change(Update(be
+0000ff00: 6c6f 7732 2c20 6265 6c6f 7731 2929 290a  low2, below1))).
+0000ff10: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+0000ff20: 6572 7446 616c 7365 2870 726f 7669 6465  ertFalse(provide
+0000ff30: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
+0000ff40: 6528 5570 6461 7465 2862 656c 6f77 322c  e(Update(below2,
+0000ff50: 2062 656c 6f77 3229 2929 0a0a 2020 2020   below2)))..    
+0000ff60: 2020 2020 2320 6f6e 6520 6265 6c6f 772c      # one below,
+0000ff70: 206f 7468 6572 2061 740a 2020 2020 2020   other at.      
+0000ff80: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
+0000ff90: 7365 2870 726f 7669 6465 722e 5f69 6e63  se(provider._inc
+0000ffa0: 6c75 6465 5f63 6861 6e67 6528 5570 6461  lude_change(Upda
+0000ffb0: 7465 2862 656c 6f77 312c 2065 6467 6529  te(below1, edge)
+0000ffc0: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+0000ffd0: 6173 7365 7274 4661 6c73 6528 7072 6f76  assertFalse(prov
+0000ffe0: 6964 6572 2e5f 696e 636c 7564 655f 6368  ider._include_ch
+0000fff0: 616e 6765 2855 7064 6174 6528 6265 6c6f  ange(Update(belo
+00010000: 7732 2c20 6564 6765 2929 290a 2020 2020  w2, edge))).    
+00010010: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
+00010020: 616c 7365 2870 726f 7669 6465 722e 5f69  alse(provider._i
+00010030: 6e63 6c75 6465 5f63 6861 6e67 6528 5570  nclude_change(Up
+00010040: 6461 7465 2865 6467 652c 2062 656c 6f77  date(edge, below
+00010050: 3129 2929 0a20 2020 2020 2020 2073 656c  1))).        sel
+00010060: 662e 6173 7365 7274 4661 6c73 6528 7072  f.assertFalse(pr
+00010070: 6f76 6964 6572 2e5f 696e 636c 7564 655f  ovider._include_
+00010080: 6368 616e 6765 2855 7064 6174 6528 6564  change(Update(ed
+00010090: 6765 2c20 6265 6c6f 7732 2929 290a 0a20  ge, below2))).. 
+000100a0: 2020 2020 2020 2023 2062 6f74 6820 6174         # both at
+000100b0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000100c0: 7365 7274 4661 6c73 6528 7072 6f76 6964  sertFalse(provid
+000100d0: 6572 2e5f 696e 636c 7564 655f 6368 616e  er._include_chan
+000100e0: 6765 2855 7064 6174 6528 6564 6765 2c20  ge(Update(edge, 
+000100f0: 6564 6765 2929 290a 0a20 2020 2020 2020  edge)))..       
+00010100: 2023 206f 6e65 2061 742c 206f 7468 6572   # one at, other
+00010110: 2061 626f 7665 0a20 2020 2020 2020 2073   above.        s
+00010120: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
+00010130: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
+00010140: 5f63 6861 6e67 6528 5570 6461 7465 2865  _change(Update(e
+00010150: 6467 652c 2061 626f 7665 3129 2929 0a20  dge, above1))). 
+00010160: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010170: 7274 5472 7565 2870 726f 7669 6465 722e  rtTrue(provider.
+00010180: 5f69 6e63 6c75 6465 5f63 6861 6e67 6528  _include_change(
+00010190: 5570 6461 7465 2865 6467 652c 2061 626f  Update(edge, abo
+000101a0: 7665 3229 2929 0a20 2020 2020 2020 2073  ve2))).        s
+000101b0: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
+000101c0: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
+000101d0: 5f63 6861 6e67 6528 5570 6461 7465 2861  _change(Update(a
+000101e0: 626f 7665 312c 2065 6467 6529 2929 0a20  bove1, edge))). 
+000101f0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+00010200: 7274 5472 7565 2870 726f 7669 6465 722e  rtTrue(provider.
+00010210: 5f69 6e63 6c75 6465 5f63 6861 6e67 6528  _include_change(
+00010220: 5570 6461 7465 2861 626f 7665 322c 2065  Update(above2, e
+00010230: 6467 6529 2929 0a0a 2020 2020 2020 2020  dge)))..        
+00010240: 2320 626f 7468 2061 626f 7665 0a20 2020  # both above.   
+00010250: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00010260: 5472 7565 2870 726f 7669 6465 722e 5f69  True(provider._i
+00010270: 6e63 6c75 6465 5f63 6861 6e67 6528 5570  nclude_change(Up
+00010280: 6461 7465 2861 626f 7665 312c 2061 626f  date(above1, abo
+00010290: 7665 3229 2929 0a20 2020 2020 2020 2073  ve2))).        s
+000102a0: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
+000102b0: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
+000102c0: 5f63 6861 6e67 6528 5570 6461 7465 2861  _change(Update(a
+000102d0: 626f 7665 322c 2061 626f 7665 3129 2929  bove2, above1)))
+000102e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000102f0: 7365 7274 4661 6c73 6528 7072 6f76 6964  sertFalse(provid
+00010300: 6572 2e5f 696e 636c 7564 655f 6368 616e  er._include_chan
+00010310: 6765 2855 7064 6174 6528 6162 6f76 6531  ge(Update(above1
+00010320: 2c20 6162 6f76 6531 2929 290a 2020 2020  , above1))).    
+00010330: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
+00010340: 616c 7365 2870 726f 7669 6465 722e 5f69  alse(provider._i
+00010350: 6e63 6c75 6465 5f63 6861 6e67 6528 5570  nclude_change(Up
+00010360: 6461 7465 2861 626f 7665 322c 2061 626f  date(above2, abo
+00010370: 7665 3229 2929 0a0a 2020 2020 2020 2020  ve2)))..        
+00010380: 2320 6f6e 6520 6265 6c6f 772c 206f 6e65  # one below, one
+00010390: 2061 626f 7665 0a20 2020 2020 2020 2073   above.        s
+000103a0: 656c 662e 6173 7365 7274 5472 7565 2870  elf.assertTrue(p
+000103b0: 726f 7669 6465 722e 5f69 6e63 6c75 6465  rovider._include
+000103c0: 5f63 6861 6e67 6528 5570 6461 7465 2862  _change(Update(b
+000103d0: 656c 6f77 322c 2061 626f 7665 3129 2929  elow2, above1)))
+000103e0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+000103f0: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
+00010400: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
+00010410: 6528 5570 6461 7465 2861 626f 7665 312c  e(Update(above1,
+00010420: 2062 656c 6f77 3229 2929 0a0a 2020 2020   below2)))..    
+00010430: 6465 6620 7465 7374 5f75 6e70 726f 7869  def test_unproxi
+00010440: 6162 6c65 7479 7065 5f67 656e 6461 7461  abletype_gendata
+00010450: 5f72 6574 7572 6e73 6e6f 7072 6f78 6965  _returnsnoproxie
+00010460: 6428 7365 6c66 293a 0a20 2020 2020 2020  d(self):.       
+00010470: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
+00010480: 6466 6c61 7265 5072 6f76 6964 6572 2827  dflareProvider('
+00010490: 7465 7374 272c 2027 656d 6169 6c27 2c20  test', 'email', 
+000104a0: 2774 6f6b 656e 2729 0a20 2020 2020 2020  'token').       
+000104b0: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
+000104c0: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
+000104d0: 2020 2020 2020 2020 7265 636f 7264 203d          record =
+000104e0: 2052 6563 6f72 642e 6e65 7728 0a20 2020   Record.new(.   
+000104f0: 2020 2020 2020 2020 207a 6f6e 652c 2027           zone, '
+00010500: 6127 2c20 7b27 7474 6c27 3a20 3336 3030  a', {'ttl': 3600
+00010510: 2c20 2774 7970 6527 3a20 274e 5327 2c20  , 'type': 'NS', 
+00010520: 2776 616c 7565 273a 2027 6e73 312e 756e  'value': 'ns1.un
+00010530: 6974 2e74 6573 7473 2e27 7d0a 2020 2020  it.tests.'}.    
+00010540: 2020 2020 290a 0a20 2020 2020 2020 2064      )..        d
+00010550: 6174 6120 3d20 6e65 7874 2870 726f 7669  ata = next(provi
+00010560: 6465 722e 5f67 656e 5f64 6174 6128 7265  der._gen_data(re
+00010570: 636f 7264 2929 0a0a 2020 2020 2020 2020  cord))..        
+00010580: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+00010590: 2827 7072 6f78 6965 6427 2069 6e20 6461  ('proxied' in da
+000105a0: 7461 290a 0a20 2020 2064 6566 2074 6573  ta)..    def tes
+000105b0: 745f 7072 6f78 6961 626c 6574 7970 655f  t_proxiabletype_
+000105c0: 6765 6e64 6174 615f 7265 7475 726e 7375  gendata_returnsu
+000105d0: 6e70 726f 7869 6564 2873 656c 6629 3a0a  nproxied(self):.
+000105e0: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+000105f0: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
+00010600: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
+00010610: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
+00010620: 2020 2020 2020 2020 7a6f 6e65 203d 205a          zone = Z
+00010630: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
+00010640: 272c 205b 5d29 0a20 2020 2020 2020 2072  ', []).        r
+00010650: 6563 6f72 6420 3d20 7365 745f 7265 636f  ecord = set_reco
+00010660: 7264 5f70 726f 7869 6564 5f66 6c61 6728  rd_proxied_flag(
+00010670: 0a20 2020 2020 2020 2020 2020 2052 6563  .            Rec
+00010680: 6f72 642e 6e65 7728 0a20 2020 2020 2020  ord.new(.       
+00010690: 2020 2020 2020 2020 207a 6f6e 652c 2027           zone, '
+000106a0: 6127 2c20 7b27 7474 6c27 3a20 3330 302c  a', {'ttl': 300,
+000106b0: 2027 7479 7065 273a 2027 4127 2c20 2776   'type': 'A', 'v
+000106c0: 616c 7565 273a 2027 312e 322e 332e 3427  alue': '1.2.3.4'
+000106d0: 7d0a 2020 2020 2020 2020 2020 2020 292c  }.            ),
+000106e0: 0a20 2020 2020 2020 2020 2020 2046 616c  .            Fal
+000106f0: 7365 2c0a 2020 2020 2020 2020 290a 0a20  se,.        ).. 
+00010700: 2020 2020 2020 2064 6174 6120 3d20 6e65         data = ne
+00010710: 7874 2870 726f 7669 6465 722e 5f67 656e  xt(provider._gen
+00010720: 5f64 6174 6128 7265 636f 7264 2929 0a0a  _data(record))..
+00010730: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00010740: 6572 7446 616c 7365 2864 6174 615b 2770  ertFalse(data['p
+00010750: 726f 7869 6564 275d 290a 0a20 2020 2064  roxied'])..    d
+00010760: 6566 2074 6573 745f 7072 6f78 6961 626c  ef test_proxiabl
+00010770: 6574 7970 655f 6765 6e64 6174 615f 7265  etype_gendata_re
+00010780: 7475 726e 7370 726f 7869 6564 2873 656c  turnsproxied(sel
+00010790: 6629 3a0a 2020 2020 2020 2020 7072 6f76  f):.        prov
+000107a0: 6964 6572 203d 2043 6c6f 7564 666c 6172  ider = Cloudflar
+000107b0: 6550 726f 7669 6465 7228 2774 6573 7427  eProvider('test'
+000107c0: 2c20 2765 6d61 696c 272c 2027 746f 6b65  , 'email', 'toke
+000107d0: 6e27 290a 2020 2020 2020 2020 7a6f 6e65  n').        zone
+000107e0: 203d 205a 6f6e 6528 2775 6e69 742e 7465   = Zone('unit.te
+000107f0: 7374 732e 272c 205b 5d29 0a20 2020 2020  sts.', []).     
+00010800: 2020 2072 6563 6f72 6420 3d20 7365 745f     record = set_
+00010810: 7265 636f 7264 5f70 726f 7869 6564 5f66  record_proxied_f
+00010820: 6c61 6728 0a20 2020 2020 2020 2020 2020  lag(.           
+00010830: 2052 6563 6f72 642e 6e65 7728 0a20 2020   Record.new(.   
+00010840: 2020 2020 2020 2020 2020 2020 207a 6f6e               zon
+00010850: 652c 2027 6127 2c20 7b27 7474 6c27 3a20  e, 'a', {'ttl': 
+00010860: 3330 302c 2027 7479 7065 273a 2027 4127  300, 'type': 'A'
+00010870: 2c20 2776 616c 7565 273a 2027 312e 322e  , 'value': '1.2.
+00010880: 332e 3427 7d0a 2020 2020 2020 2020 2020  3.4'}.          
+00010890: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+000108a0: 2054 7275 652c 0a20 2020 2020 2020 2029   True,.        )
+000108b0: 0a0a 2020 2020 2020 2020 6461 7461 203d  ..        data =
+000108c0: 206e 6578 7428 7072 6f76 6964 6572 2e5f   next(provider._
+000108d0: 6765 6e5f 6461 7461 2872 6563 6f72 6429  gen_data(record)
+000108e0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+000108f0: 6173 7365 7274 5472 7565 2864 6174 615b  assertTrue(data[
+00010900: 2770 726f 7869 6564 275d 290a 0a20 2020  'proxied'])..   
+00010910: 2064 6566 2074 6573 745f 6372 6561 7465   def test_create
+00010920: 7265 636f 7264 5f65 7874 7261 6368 616e  record_extrachan
+00010930: 6765 735f 7265 7475 726e 7365 6d70 7479  ges_returnsempty
+00010940: 6c69 7374 2873 656c 6629 3a0a 2020 2020  list(self):.    
+00010950: 2020 2020 7072 6f76 6964 6572 203d 2043      provider = C
+00010960: 6c6f 7564 666c 6172 6550 726f 7669 6465  loudflareProvide
+00010970: 7228 2774 6573 7427 2c20 2765 6d61 696c  r('test', 'email
+00010980: 272c 2027 746f 6b65 6e27 290a 2020 2020  ', 'token').    
+00010990: 2020 2020 7072 6f76 6964 6572 2e7a 6f6e      provider.zon
+000109a0: 655f 7265 636f 7264 7320 3d20 4d6f 636b  e_records = Mock
+000109b0: 2872 6574 7572 6e5f 7661 6c75 653d 5b5d  (return_value=[]
+000109c0: 290a 2020 2020 2020 2020 6578 6973 7469  ).        existi
+000109d0: 6e67 203d 205a 6f6e 6528 2775 6e69 742e  ng = Zone('unit.
+000109e0: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
+000109f0: 2020 2020 2070 726f 7669 6465 722e 706f       provider.po
+00010a00: 7075 6c61 7465 2865 7869 7374 696e 6729  pulate(existing)
+00010a10: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+00010a20: 722e 7a6f 6e65 5f72 6563 6f72 6473 203d  r.zone_records =
+00010a30: 204d 6f63 6b28 0a20 2020 2020 2020 2020   Mock(.         
+00010a40: 2020 2072 6574 7572 6e5f 7661 6c75 653d     return_value=
+00010a50: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00010a60: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00010a70: 2020 2020 2020 2020 2269 6422 3a20 2266          "id": "f
+00010a80: 6331 3261 6233 3463 6435 3631 3133 3334  c12ab34cd5611334
+00010a90: 3432 3261 6233 3332 3239 3937 3634 3222  422ab3322997642"
+00010aa0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010ab0: 2020 2020 2020 2274 7970 6522 3a20 2243        "type": "C
+00010ac0: 4e41 4d45 222c 0a20 2020 2020 2020 2020  NAME",.         
+00010ad0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00010ae0: 223a 2022 612e 756e 6974 2e74 6573 7473  ": "a.unit.tests
+00010af0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00010b00: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
+00010b10: 3a20 2277 7777 2e75 6e69 742e 7465 7374  : "www.unit.test
+00010b20: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00010b30: 2020 2020 2020 2020 2270 726f 7869 6162          "proxiab
+00010b40: 6c65 223a 2054 7275 652c 0a20 2020 2020  le": True,.     
+00010b50: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00010b60: 7072 6f78 6965 6422 3a20 5472 7565 2c0a  proxied": True,.
+00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b80: 2020 2020 2274 746c 223a 2033 3030 2c0a      "ttl": 300,.
+00010b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ba0: 2020 2020 226c 6f63 6b65 6422 3a20 4661      "locked": Fa
+00010bb0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00010bc0: 2020 2020 2020 2020 2022 7a6f 6e65 5f69           "zone_i
+00010bd0: 6422 3a20 2266 6631 3261 6233 3463 6435  d": "ff12ab34cd5
+00010be0: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
+00010bf0: 3937 3635 3022 2c0a 2020 2020 2020 2020  97650",.        
+00010c00: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+00010c10: 655f 6e61 6d65 223a 2022 756e 6974 2e74  e_name": "unit.t
+00010c20: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+00010c30: 2020 2020 2020 2020 2020 2022 6d6f 6469             "modi
+00010c40: 6669 6564 5f6f 6e22 3a20 2232 3031 372d  fied_on": "2017-
+00010c50: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
+00010c60: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
+00010c70: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+00010c80: 6561 7465 645f 6f6e 223a 2022 3230 3137  eated_on": "2017
+00010c90: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+00010ca0: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+00010cb0: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00010cc0: 6574 6122 3a20 7b22 6175 746f 5f61 6464  eta": {"auto_add
+00010cd0: 6564 223a 2046 616c 7365 7d2c 0a20 2020  ed": False},.   
+00010ce0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00010cf0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+00010d00: 2020 2020 2029 0a20 2020 2020 2020 2064       ).        d
+00010d10: 6573 6972 6564 203d 205a 6f6e 6528 2775  esired = Zone('u
+00010d20: 6e69 742e 7465 7374 732e 272c 205b 5d29  nit.tests.', [])
+00010d30: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+00010d40: 722e 706f 7075 6c61 7465 2864 6573 6972  r.populate(desir
+00010d50: 6564 290a 2020 2020 2020 2020 6368 616e  ed).        chan
+00010d60: 6765 7320 3d20 6578 6973 7469 6e67 2e63  ges = existing.c
+00010d70: 6861 6e67 6573 2864 6573 6972 6564 2c20  hanges(desired, 
+00010d80: 7072 6f76 6964 6572 290a 0a20 2020 2020  provider)..     
+00010d90: 2020 2065 7874 7261 5f63 6861 6e67 6573     extra_changes
+00010da0: 203d 2070 726f 7669 6465 722e 5f65 7874   = provider._ext
+00010db0: 7261 5f63 6861 6e67 6573 2865 7869 7374  ra_changes(exist
+00010dc0: 696e 672c 2064 6573 6972 6564 2c20 6368  ing, desired, ch
+00010dd0: 616e 6765 7329 0a0a 2020 2020 2020 2020  anges)..        
+00010de0: 7365 6c66 2e61 7373 6572 7446 616c 7365  self.assertFalse
+00010df0: 2865 7874 7261 5f63 6861 6e67 6573 290a  (extra_changes).
+00010e00: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
+00010e10: 6461 7465 7265 636f 7264 5f65 7874 7261  daterecord_extra
+00010e20: 6368 616e 6765 735f 7265 7475 726e 7365  changes_returnse
+00010e30: 6d70 7479 6c69 7374 2873 656c 6629 3a0a  mptylist(self):.
+00010e40: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00010e50: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
+00010e60: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
+00010e70: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
+00010e80: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00010e90: 2e7a 6f6e 655f 7265 636f 7264 7320 3d20  .zone_records = 
+00010ea0: 4d6f 636b 280a 2020 2020 2020 2020 2020  Mock(.          
+00010eb0: 2020 7265 7475 726e 5f76 616c 7565 3d5b    return_value=[
+00010ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010ed0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00010ee0: 2020 2020 2020 2022 6964 223a 2022 6663         "id": "fc
+00010ef0: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
+00010f00: 3232 6162 3333 3232 3939 3736 3432 222c  22ab3322997642",
+00010f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f20: 2020 2020 2022 7479 7065 223a 2022 434e       "type": "CN
+00010f30: 414d 4522 2c0a 2020 2020 2020 2020 2020  AME",.          
+00010f40: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00010f50: 3a20 2261 2e75 6e69 742e 7465 7374 7322  : "a.unit.tests"
+00010f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010f70: 2020 2020 2020 2263 6f6e 7465 6e74 223a        "content":
+00010f80: 2022 7777 772e 756e 6974 2e74 6573 7473   "www.unit.tests
+00010f90: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00010fa0: 2020 2020 2020 2022 7072 6f78 6961 626c         "proxiabl
+00010fb0: 6522 3a20 5472 7565 2c0a 2020 2020 2020  e": True,.      
+00010fc0: 2020 2020 2020 2020 2020 2020 2020 2270                "p
+00010fd0: 726f 7869 6564 223a 2054 7275 652c 0a20  roxied": True,. 
+00010fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ff0: 2020 2022 7474 6c22 3a20 3132 302c 0a20     "ttl": 120,. 
+00011000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011010: 2020 2022 6c6f 636b 6564 223a 2046 616c     "locked": Fal
+00011020: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00011030: 2020 2020 2020 2020 227a 6f6e 655f 6964          "zone_id
+00011040: 223a 2022 6666 3132 6162 3334 6364 3536  ": "ff12ab34cd56
+00011050: 3131 3333 3434 3232 6162 3333 3232 3939  11334422ab332299
+00011060: 3736 3530 222c 0a20 2020 2020 2020 2020  7650",.         
+00011070: 2020 2020 2020 2020 2020 2022 7a6f 6e65             "zone
+00011080: 5f6e 616d 6522 3a20 2275 6e69 742e 7465  _name": "unit.te
+00011090: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+000110a0: 2020 2020 2020 2020 2020 226d 6f64 6966            "modif
+000110b0: 6965 645f 6f6e 223a 2022 3230 3137 2d30  ied_on": "2017-0
+000110c0: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
+000110d0: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
+000110e0: 2020 2020 2020 2020 2020 2020 2263 7265              "cre
+000110f0: 6174 6564 5f6f 6e22 3a20 2232 3031 372d  ated_on": "2017-
+00011100: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
+00011110: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
+00011120: 2020 2020 2020 2020 2020 2020 2022 6d65               "me
+00011130: 7461 223a 207b 2261 7574 6f5f 6164 6465  ta": {"auto_adde
+00011140: 6422 3a20 4661 6c73 657d 2c0a 2020 2020  d": False},.    
+00011150: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00011160: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
+00011170: 2020 2020 290a 2020 2020 2020 2020 6578      ).        ex
+00011180: 6973 7469 6e67 203d 205a 6f6e 6528 2775  isting = Zone('u
+00011190: 6e69 742e 7465 7374 732e 272c 205b 5d29  nit.tests.', [])
+000111a0: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+000111b0: 722e 706f 7075 6c61 7465 2865 7869 7374  r.populate(exist
+000111c0: 696e 6729 0a20 2020 2020 2020 2070 726f  ing).        pro
+000111d0: 7669 6465 722e 7a6f 6e65 5f72 6563 6f72  vider.zone_recor
+000111e0: 6473 203d 204d 6f63 6b28 0a20 2020 2020  ds = Mock(.     
+000111f0: 2020 2020 2020 2072 6574 7572 6e5f 7661         return_va
+00011200: 6c75 653d 5b0a 2020 2020 2020 2020 2020  lue=[.          
+00011210: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00011220: 2020 2020 2020 2020 2020 2020 2269 6422              "id"
+00011230: 3a20 2266 6331 3261 6233 3463 6435 3631  : "fc12ab34cd561
+00011240: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
+00011250: 3634 3222 2c0a 2020 2020 2020 2020 2020  642",.          
+00011260: 2020 2020 2020 2020 2020 2274 7970 6522            "type"
+00011270: 3a20 2243 4e41 4d45 222c 0a20 2020 2020  : "CNAME",.     
+00011280: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011290: 6e61 6d65 223a 2022 612e 756e 6974 2e74  name": "a.unit.t
+000112a0: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+000112b0: 2020 2020 2020 2020 2020 2022 636f 6e74             "cont
+000112c0: 656e 7422 3a20 2277 7777 2e75 6e69 742e  ent": "www.unit.
+000112d0: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
+000112e0: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
+000112f0: 7869 6162 6c65 223a 2054 7275 652c 0a20  xiable": True,. 
+00011300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011310: 2020 2022 7072 6f78 6965 6422 3a20 5472     "proxied": Tr
+00011320: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00011330: 2020 2020 2020 2020 2274 746c 223a 2033          "ttl": 3
+00011340: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+00011350: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
+00011360: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00011370: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+00011380: 6e65 5f69 6422 3a20 2266 6631 3261 6233  ne_id": "ff12ab3
+00011390: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+000113a0: 3332 3239 3937 3635 3022 2c0a 2020 2020  322997650",.    
+000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000113c0: 227a 6f6e 655f 6e61 6d65 223a 2022 756e  "zone_name": "un
+000113d0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
+000113e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000113f0: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
+00011400: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
+00011410: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
+00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011430: 2022 6372 6561 7465 645f 6f6e 223a 2022   "created_on": "
+00011440: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
+00011450: 3a34 332e 3432 3036 3839 5a22 2c0a 2020  :43.420689Z",.  
+00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011470: 2020 226d 6574 6122 3a20 7b22 6175 746f    "meta": {"auto
+00011480: 5f61 6464 6564 223a 2046 616c 7365 7d2c  _added": False},
+00011490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000114a0: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
+000114b0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000114c0: 2020 2064 6573 6972 6564 203d 205a 6f6e     desired = Zon
+000114d0: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
+000114e0: 205b 5d29 0a20 2020 2020 2020 2070 726f   []).        pro
+000114f0: 7669 6465 722e 706f 7075 6c61 7465 2864  vider.populate(d
+00011500: 6573 6972 6564 290a 2020 2020 2020 2020  esired).        
+00011510: 6368 616e 6765 7320 3d20 6578 6973 7469  changes = existi
+00011520: 6e67 2e63 6861 6e67 6573 2864 6573 6972  ng.changes(desir
+00011530: 6564 2c20 7072 6f76 6964 6572 290a 0a20  ed, provider).. 
+00011540: 2020 2020 2020 2065 7874 7261 5f63 6861         extra_cha
+00011550: 6e67 6573 203d 2070 726f 7669 6465 722e  nges = provider.
+00011560: 5f65 7874 7261 5f63 6861 6e67 6573 2865  _extra_changes(e
+00011570: 7869 7374 696e 672c 2064 6573 6972 6564  xisting, desired
+00011580: 2c20 6368 616e 6765 7329 0a0a 2020 2020  , changes)..    
+00011590: 2020 2020 7365 6c66 2e61 7373 6572 7446      self.assertF
+000115a0: 616c 7365 2865 7874 7261 5f63 6861 6e67  alse(extra_chang
+000115b0: 6573 290a 0a20 2020 2064 6566 2074 6573  es)..    def tes
+000115c0: 745f 6465 6c65 7465 7265 636f 7264 5f65  t_deleterecord_e
+000115d0: 7874 7261 6368 616e 6765 735f 7265 7475  xtrachanges_retu
+000115e0: 726e 7365 6d70 7479 6c69 7374 2873 656c  rnsemptylist(sel
+000115f0: 6629 3a0a 2020 2020 2020 2020 7072 6f76  f):.        prov
+00011600: 6964 6572 203d 2043 6c6f 7564 666c 6172  ider = Cloudflar
+00011610: 6550 726f 7669 6465 7228 2774 6573 7427  eProvider('test'
+00011620: 2c20 2765 6d61 696c 272c 2027 746f 6b65  , 'email', 'toke
+00011630: 6e27 290a 2020 2020 2020 2020 7072 6f76  n').        prov
+00011640: 6964 6572 2e7a 6f6e 655f 7265 636f 7264  ider.zone_record
+00011650: 7320 3d20 4d6f 636b 280a 2020 2020 2020  s = Mock(.      
+00011660: 2020 2020 2020 7265 7475 726e 5f76 616c        return_val
+00011670: 7565 3d5b 0a20 2020 2020 2020 2020 2020  ue=[.           
+00011680: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00011690: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+000116a0: 2022 6663 3132 6162 3334 6364 3536 3131   "fc12ab34cd5611
+000116b0: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+000116c0: 3432 222c 0a20 2020 2020 2020 2020 2020  42",.           
+000116d0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000116e0: 2022 434e 414d 4522 2c0a 2020 2020 2020   "CNAME",.      
+000116f0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00011700: 616d 6522 3a20 2261 2e75 6e69 742e 7465  ame": "a.unit.te
+00011710: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+00011720: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00011730: 6e74 223a 2022 7777 772e 756e 6974 2e74  nt": "www.unit.t
+00011740: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+00011750: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
+00011760: 6961 626c 6522 3a20 5472 7565 2c0a 2020  iable": True,.  
+00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011780: 2020 2270 726f 7869 6564 223a 2054 7275    "proxied": Tru
+00011790: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000117a0: 2020 2020 2020 2022 7474 6c22 3a20 3330         "ttl": 30
+000117b0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+000117c0: 2020 2020 2020 2022 6c6f 636b 6564 223a         "locked":
+000117d0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+000117e0: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+000117f0: 655f 6964 223a 2022 6666 3132 6162 3334  e_id": "ff12ab34
+00011800: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
+00011810: 3232 3939 3736 3530 222c 0a20 2020 2020  22997650",.     
+00011820: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011830: 7a6f 6e65 5f6e 616d 6522 3a20 2275 6e69  zone_name": "uni
+00011840: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+00011850: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00011860: 6f64 6966 6965 645f 6f6e 223a 2022 3230  odified_on": "20
+00011870: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
+00011880: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
+00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118a0: 2263 7265 6174 6564 5f6f 6e22 3a20 2232  "created_on": "2
+000118b0: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
+000118c0: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
+000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118e0: 2022 6d65 7461 223a 207b 2261 7574 6f5f   "meta": {"auto_
+000118f0: 6164 6465 6422 3a20 4661 6c73 657d 2c0a  added": False},.
+00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011910: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
+00011920: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00011930: 2020 6578 6973 7469 6e67 203d 205a 6f6e    existing = Zon
+00011940: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
+00011950: 205b 5d29 0a20 2020 2020 2020 2070 726f   []).        pro
+00011960: 7669 6465 722e 706f 7075 6c61 7465 2865  vider.populate(e
+00011970: 7869 7374 696e 6729 0a20 2020 2020 2020  xisting).       
+00011980: 2070 726f 7669 6465 722e 7a6f 6e65 5f72   provider.zone_r
+00011990: 6563 6f72 6473 203d 204d 6f63 6b28 7265  ecords = Mock(re
+000119a0: 7475 726e 5f76 616c 7565 3d5b 5d29 0a20  turn_value=[]). 
+000119b0: 2020 2020 2020 2064 6573 6972 6564 203d         desired =
+000119c0: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+000119d0: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
+000119e0: 2070 726f 7669 6465 722e 706f 7075 6c61   provider.popula
+000119f0: 7465 2864 6573 6972 6564 290a 2020 2020  te(desired).    
+00011a00: 2020 2020 6368 616e 6765 7320 3d20 6578      changes = ex
+00011a10: 6973 7469 6e67 2e63 6861 6e67 6573 2864  isting.changes(d
+00011a20: 6573 6972 6564 2c20 7072 6f76 6964 6572  esired, provider
+00011a30: 290a 0a20 2020 2020 2020 2065 7874 7261  )..        extra
+00011a40: 5f63 6861 6e67 6573 203d 2070 726f 7669  _changes = provi
+00011a50: 6465 722e 5f65 7874 7261 5f63 6861 6e67  der._extra_chang
+00011a60: 6573 2865 7869 7374 696e 672c 2064 6573  es(existing, des
+00011a70: 6972 6564 2c20 6368 616e 6765 7329 0a0a  ired, changes)..
+00011a80: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00011a90: 6572 7446 616c 7365 2865 7874 7261 5f63  ertFalse(extra_c
+00011aa0: 6861 6e67 6573 290a 0a20 2020 2064 6566  hanges)..    def
+00011ab0: 2074 6573 745f 7072 6f78 6966 795f 6578   test_proxify_ex
+00011ac0: 7472 6163 6861 6e67 6573 5f72 6574 7572  trachanges_retur
+00011ad0: 6e73 7570 6461 7465 6c69 7374 2873 656c  nsupdatelist(sel
+00011ae0: 6629 3a0a 2020 2020 2020 2020 7072 6f76  f):.        prov
+00011af0: 6964 6572 203d 2043 6c6f 7564 666c 6172  ider = Cloudflar
+00011b00: 6550 726f 7669 6465 7228 2774 6573 7427  eProvider('test'
+00011b10: 2c20 2765 6d61 696c 272c 2027 746f 6b65  , 'email', 'toke
+00011b20: 6e27 290a 2020 2020 2020 2020 7072 6f76  n').        prov
+00011b30: 6964 6572 2e7a 6f6e 655f 7265 636f 7264  ider.zone_record
+00011b40: 7320 3d20 4d6f 636b 280a 2020 2020 2020  s = Mock(.      
+00011b50: 2020 2020 2020 7265 7475 726e 5f76 616c        return_val
+00011b60: 7565 3d5b 0a20 2020 2020 2020 2020 2020  ue=[.           
+00011b70: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+00011b80: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+00011b90: 2022 6663 3132 6162 3334 6364 3536 3131   "fc12ab34cd5611
+00011ba0: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+00011bb0: 3432 222c 0a20 2020 2020 2020 2020 2020  42",.           
+00011bc0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00011bd0: 2022 434e 414d 4522 2c0a 2020 2020 2020   "CNAME",.      
+00011be0: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00011bf0: 616d 6522 3a20 2261 2e75 6e69 742e 7465  ame": "a.unit.te
+00011c00: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+00011c10: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00011c20: 6e74 223a 2022 7777 772e 756e 6974 2e74  nt": "www.unit.t
+00011c30: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+00011c40: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
+00011c50: 6961 626c 6522 3a20 5472 7565 2c0a 2020  iable": True,.  
+00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c70: 2020 2270 726f 7869 6564 223a 2046 616c    "proxied": Fal
+00011c80: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00011c90: 2020 2020 2020 2020 2274 746c 223a 2033          "ttl": 3
+00011ca0: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+00011cb0: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
+00011cc0: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00011cd0: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+00011ce0: 6e65 5f69 6422 3a20 2266 6631 3261 6233  ne_id": "ff12ab3
+00011cf0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+00011d00: 3332 3239 3937 3635 3022 2c0a 2020 2020  322997650",.    
+00011d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d20: 227a 6f6e 655f 6e61 6d65 223a 2022 756e  "zone_name": "un
+00011d30: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011d50: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
+00011d60: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
+00011d70: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
+00011d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d90: 2022 6372 6561 7465 645f 6f6e 223a 2022   "created_on": "
+00011da0: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
+00011db0: 3a34 332e 3432 3036 3839 5a22 2c0a 2020  :43.420689Z",.  
+00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011dd0: 2020 226d 6574 6122 3a20 7b22 6175 746f    "meta": {"auto
+00011de0: 5f61 6464 6564 223a 2046 616c 7365 7d2c  _added": False},
+00011df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011e00: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
+00011e10: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00011e20: 2020 2065 7869 7374 696e 6720 3d20 5a6f     existing = Zo
+00011e30: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
+00011e40: 2c20 5b5d 290a 2020 2020 2020 2020 7072  , []).        pr
+00011e50: 6f76 6964 6572 2e70 6f70 756c 6174 6528  ovider.populate(
+00011e60: 6578 6973 7469 6e67 290a 2020 2020 2020  existing).      
+00011e70: 2020 7072 6f76 6964 6572 2e7a 6f6e 655f    provider.zone_
+00011e80: 7265 636f 7264 7320 3d20 4d6f 636b 280a  records = Mock(.
+00011e90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00011ea0: 726e 5f76 616c 7565 3d5b 0a20 2020 2020  rn_value=[.     
+00011eb0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2022 6964 223a 2022 6663 3132 6162 3334   "id": "fc12ab34
+00011ee0: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
+00011ef0: 3232 3939 3736 3432 222c 0a20 2020 2020  22997642",.     
+00011f00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00011f10: 7479 7065 223a 2022 434e 414d 4522 2c0a  type": "CNAME",.
+00011f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f30: 2020 2020 226e 616d 6522 3a20 2261 2e75      "name": "a.u
+00011f40: 6e69 742e 7465 7374 7322 2c0a 2020 2020  nit.tests",.    
+00011f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f60: 2263 6f6e 7465 6e74 223a 2022 7777 772e  "content": "www.
+00011f70: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+00011f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011f90: 2022 7072 6f78 6961 626c 6522 3a20 5472   "proxiable": Tr
+00011fa0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00011fb0: 2020 2020 2020 2020 2270 726f 7869 6564          "proxied
+00011fc0: 223a 2054 7275 652c 0a20 2020 2020 2020  ": True,.       
+00011fd0: 2020 2020 2020 2020 2020 2020 2022 7474               "tt
+00011fe0: 6c22 3a20 3330 302c 0a20 2020 2020 2020  l": 300,.       
+00011ff0: 2020 2020 2020 2020 2020 2020 2022 6c6f               "lo
+00012000: 636b 6564 223a 2046 616c 7365 2c0a 2020  cked": False,.  
+00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012020: 2020 227a 6f6e 655f 6964 223a 2022 6666    "zone_id": "ff
+00012030: 3132 6162 3334 6364 3536 3131 3333 3434  12ab34cd56113344
+00012040: 3232 6162 3333 3232 3939 3736 3530 222c  22ab3322997650",
+00012050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012060: 2020 2020 2022 7a6f 6e65 5f6e 616d 6522       "zone_name"
+00012070: 3a20 2275 6e69 742e 7465 7374 7322 2c0a  : "unit.tests",.
+00012080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012090: 2020 2020 226d 6f64 6966 6965 645f 6f6e      "modified_on
+000120a0: 223a 2022 3230 3137 2d30 332d 3131 5431  ": "2017-03-11T1
+000120b0: 383a 3031 3a34 332e 3432 3036 3839 5a22  8:01:43.420689Z"
+000120c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000120d0: 2020 2020 2020 2263 7265 6174 6564 5f6f        "created_o
+000120e0: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
+000120f0: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
+00012100: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012110: 2020 2020 2020 2022 6d65 7461 223a 207b         "meta": {
+00012120: 2261 7574 6f5f 6164 6465 6422 3a20 4661  "auto_added": Fa
+00012130: 6c73 657d 2c0a 2020 2020 2020 2020 2020  lse},.          
+00012140: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00012150: 2020 2020 5d0a 2020 2020 2020 2020 290a      ].        ).
+00012160: 2020 2020 2020 2020 6465 7369 7265 6420          desired 
+00012170: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
+00012180: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
+00012190: 2020 7072 6f76 6964 6572 2e70 6f70 756c    provider.popul
+000121a0: 6174 6528 6465 7369 7265 6429 0a20 2020  ate(desired).   
+000121b0: 2020 2020 2063 6861 6e67 6573 203d 2065       changes = e
+000121c0: 7869 7374 696e 672e 6368 616e 6765 7328  xisting.changes(
+000121d0: 6465 7369 7265 642c 2070 726f 7669 6465  desired, provide
+000121e0: 7229 0a0a 2020 2020 2020 2020 6578 7472  r)..        extr
+000121f0: 615f 6368 616e 6765 7320 3d20 7072 6f76  a_changes = prov
+00012200: 6964 6572 2e5f 6578 7472 615f 6368 616e  ider._extra_chan
+00012210: 6765 7328 6578 6973 7469 6e67 2c20 6465  ges(existing, de
+00012220: 7369 7265 642c 2063 6861 6e67 6573 290a  sired, changes).
+00012230: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00012240: 7365 7274 4571 7561 6c28 312c 206c 656e  sertEqual(1, len
+00012250: 2865 7874 7261 5f63 6861 6e67 6573 2929  (extra_changes))
+00012260: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00012270: 7365 7274 4661 6c73 6528 0a20 2020 2020  sertFalse(.     
+00012280: 2020 2020 2020 2065 7874 7261 5f63 6861         extra_cha
+00012290: 6e67 6573 5b30 5d0a 2020 2020 2020 2020  nges[0].        
+000122a0: 2020 2020 2e65 7869 7374 696e 672e 5f6f      .existing._o
+000122b0: 6374 6f64 6e73 2e67 6574 2827 636c 6f75  ctodns.get('clou
+000122c0: 6466 6c61 7265 272c 207b 7d29 0a20 2020  dflare', {}).   
+000122d0: 2020 2020 2020 2020 202e 6765 7428 2770           .get('p
+000122e0: 726f 7869 6564 272c 2046 616c 7365 290a  roxied', False).
+000122f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00012300: 2020 7365 6c66 2e61 7373 6572 7454 7275    self.assertTru
+00012310: 6528 6578 7472 615f 6368 616e 6765 735b  e(extra_changes[
+00012320: 305d 2e6e 6577 2e5f 6f63 746f 646e 735b  0].new._octodns[
+00012330: 2763 6c6f 7564 666c 6172 6527 5d5b 2770  'cloudflare']['p
+00012340: 726f 7869 6564 275d 290a 0a20 2020 2064  roxied'])..    d
+00012350: 6566 2074 6573 745f 756e 7072 6f78 6966  ef test_unproxif
+00012360: 795f 6578 7472 6163 6861 6e67 6573 5f72  y_extrachanges_r
+00012370: 6574 7572 6e73 7570 6461 7465 6c69 7374  eturnsupdatelist
+00012380: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00012390: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
+000123a0: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
+000123b0: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
+000123c0: 746f 6b65 6e27 290a 2020 2020 2020 2020  token').        
+000123d0: 7072 6f76 6964 6572 2e7a 6f6e 655f 7265  provider.zone_re
+000123e0: 636f 7264 7320 3d20 4d6f 636b 280a 2020  cords = Mock(.  
+000123f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012400: 5f76 616c 7565 3d5b 0a20 2020 2020 2020  _value=[.       
+00012410: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00012420: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00012430: 6964 223a 2022 6663 3132 6162 3334 6364  id": "fc12ab34cd
+00012440: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
+00012450: 3939 3736 3432 222c 0a20 2020 2020 2020  997642",.       
+00012460: 2020 2020 2020 2020 2020 2020 2022 7479               "ty
+00012470: 7065 223a 2022 434e 414d 4522 2c0a 2020  pe": "CNAME",.  
+00012480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012490: 2020 226e 616d 6522 3a20 2261 2e75 6e69    "name": "a.uni
+000124a0: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+000124b0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+000124c0: 6f6e 7465 6e74 223a 2022 7777 772e 756e  ontent": "www.un
+000124d0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
+000124e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000124f0: 7072 6f78 6961 626c 6522 3a20 5472 7565  proxiable": True
+00012500: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012510: 2020 2020 2020 2270 726f 7869 6564 223a        "proxied":
+00012520: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00012530: 2020 2020 2020 2020 2020 2022 7474 6c22             "ttl"
+00012540: 3a20 3330 302c 0a20 2020 2020 2020 2020  : 300,.         
+00012550: 2020 2020 2020 2020 2020 2022 6c6f 636b             "lock
+00012560: 6564 223a 2046 616c 7365 2c0a 2020 2020  ed": False,.    
+00012570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012580: 227a 6f6e 655f 6964 223a 2022 6666 3132  "zone_id": "ff12
+00012590: 6162 3334 6364 3536 3131 3333 3434 3232  ab34cd5611334422
+000125a0: 6162 3333 3232 3939 3736 3530 222c 0a20  ab3322997650",. 
+000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125c0: 2020 2022 7a6f 6e65 5f6e 616d 6522 3a20     "zone_name": 
+000125d0: 2275 6e69 742e 7465 7374 7322 2c0a 2020  "unit.tests",.  
+000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125f0: 2020 226d 6f64 6966 6965 645f 6f6e 223a    "modified_on":
+00012600: 2022 3230 3137 2d30 332d 3131 5431 383a   "2017-03-11T18:
+00012610: 3031 3a34 332e 3432 3036 3839 5a22 2c0a  01:43.420689Z",.
+00012620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012630: 2020 2020 2263 7265 6174 6564 5f6f 6e22      "created_on"
+00012640: 3a20 2232 3031 372d 3033 2d31 3154 3138  : "2017-03-11T18
+00012650: 3a30 313a 3433 2e34 3230 3638 395a 222c  :01:43.420689Z",
+00012660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012670: 2020 2020 2022 6d65 7461 223a 207b 2261       "meta": {"a
+00012680: 7574 6f5f 6164 6465 6422 3a20 4661 6c73  uto_added": Fals
+00012690: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
+000126a0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+000126b0: 2020 5d0a 2020 2020 2020 2020 290a 2020    ].        ).  
+000126c0: 2020 2020 2020 6578 6973 7469 6e67 203d        existing =
+000126d0: 205a 6f6e 6528 2775 6e69 742e 7465 7374   Zone('unit.test
+000126e0: 732e 272c 205b 5d29 0a20 2020 2020 2020  s.', []).       
+000126f0: 2070 726f 7669 6465 722e 706f 7075 6c61   provider.popula
+00012700: 7465 2865 7869 7374 696e 6729 0a20 2020  te(existing).   
+00012710: 2020 2020 2070 726f 7669 6465 722e 7a6f       provider.zo
+00012720: 6e65 5f72 6563 6f72 6473 203d 204d 6f63  ne_records = Moc
+00012730: 6b28 0a20 2020 2020 2020 2020 2020 2072  k(.            r
+00012740: 6574 7572 6e5f 7661 6c75 653d 5b0a 2020  eturn_value=[.  
+00012750: 2020 2020 2020 2020 2020 2020 2020 7b0a                {.
 00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012770: 2020 2022 7a6f 6e65 5f6e 616d 6522 3a20     "zone_name": 
-00012780: 2275 6e69 742e 7465 7374 7322 2c0a 2020  "unit.tests",.  
-00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 226d 6f64 6966 6965 645f 6f6e 223a    "modified_on":
-000127b0: 2022 3230 3137 2d30 332d 3131 5431 383a   "2017-03-11T18:
-000127c0: 3031 3a34 332e 3432 3036 3839 5a22 2c0a  01:43.420689Z",.
-000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127e0: 2020 2020 2263 7265 6174 6564 5f6f 6e22      "created_on"
-000127f0: 3a20 2232 3031 372d 3033 2d31 3154 3138  : "2017-03-11T18
-00012800: 3a30 313a 3433 2e34 3230 3638 395a 222c  :01:43.420689Z",
-00012810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012820: 2020 2020 2022 6d65 7461 223a 207b 2261       "meta": {"a
-00012830: 7574 6f5f 6164 6465 6422 3a20 4661 6c73  uto_added": Fals
-00012840: 657d 2c0a 2020 2020 2020 2020 2020 2020  e},.            
-00012850: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00012860: 2020 5d0a 2020 2020 2020 2020 290a 2020    ].        ).  
-00012870: 2020 2020 2020 6465 7369 7265 6420 3d20        desired = 
-00012880: 5a6f 6e65 2827 756e 6974 2e74 6573 7473  Zone('unit.tests
-00012890: 2e27 2c20 5b5d 290a 2020 2020 2020 2020  .', []).        
-000128a0: 7072 6f76 6964 6572 2e70 6f70 756c 6174  provider.populat
-000128b0: 6528 6465 7369 7265 6429 0a20 2020 2020  e(desired).     
-000128c0: 2020 2063 6861 6e67 6573 203d 2065 7869     changes = exi
-000128d0: 7374 696e 672e 6368 616e 6765 7328 6465  sting.changes(de
-000128e0: 7369 7265 642c 2070 726f 7669 6465 7229  sired, provider)
-000128f0: 0a0a 2020 2020 2020 2020 6578 7472 615f  ..        extra_
-00012900: 6368 616e 6765 7320 3d20 7072 6f76 6964  changes = provid
-00012910: 6572 2e5f 6578 7472 615f 6368 616e 6765  er._extra_change
-00012920: 7328 6578 6973 7469 6e67 2c20 6465 7369  s(existing, desi
-00012930: 7265 642c 2063 6861 6e67 6573 290a 0a20  red, changes).. 
-00012940: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00012950: 7274 4571 7561 6c28 312c 206c 656e 2865  rtEqual(1, len(e
-00012960: 7874 7261 5f63 6861 6e67 6573 2929 0a20  xtra_changes)). 
-00012970: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00012980: 7274 5472 7565 280a 2020 2020 2020 2020  rtTrue(.        
-00012990: 2020 2020 6578 7472 615f 6368 616e 6765      extra_change
-000129a0: 735b 305d 2e65 7869 7374 696e 672e 5f6f  s[0].existing._o
-000129b0: 6374 6f64 6e73 5b27 636c 6f75 6466 6c61  ctodns['cloudfla
-000129c0: 7265 275d 5b27 7072 6f78 6965 6427 5d0a  re']['proxied'].
-000129d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000129e0: 2020 7365 6c66 2e61 7373 6572 7446 616c    self.assertFal
-000129f0: 7365 280a 2020 2020 2020 2020 2020 2020  se(.            
-00012a00: 6578 7472 615f 6368 616e 6765 735b 305d  extra_changes[0]
-00012a10: 0a20 2020 2020 2020 2020 2020 202e 6e65  .            .ne
-00012a20: 772e 5f6f 6374 6f64 6e73 2e67 6574 2827  w._octodns.get('
-00012a30: 636c 6f75 6466 6c61 7265 272c 207b 7d29  cloudflare', {})
-00012a40: 0a20 2020 2020 2020 2020 2020 202e 6765  .            .ge
-00012a50: 7428 2770 726f 7869 6564 272c 2046 616c  t('proxied', Fal
-00012a60: 7365 290a 2020 2020 2020 2020 290a 0a20  se).        ).. 
-00012a70: 2020 2064 6566 2074 6573 745f 656d 6169     def test_emai
-00012a80: 6c6c 6573 735f 6175 7468 2873 656c 6629  lless_auth(self)
-00012a90: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
-00012aa0: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
-00012ab0: 726f 7669 6465 7228 0a20 2020 2020 2020  rovider(.       
-00012ac0: 2020 2020 2027 7465 7374 272c 2074 6f6b       'test', tok
-00012ad0: 656e 3d27 746f 6b65 6e20 3132 3327 2c20  en='token 123', 
-00012ae0: 656d 6169 6c3d 2765 6d61 696c 2032 3334  email='email 234
-00012af0: 270a 2020 2020 2020 2020 290a 2020 2020  '.        ).    
-00012b00: 2020 2020 6865 6164 6572 7320 3d20 7072      headers = pr
-00012b10: 6f76 6964 6572 2e5f 7365 7373 2e68 6561  ovider._sess.hea
-00012b20: 6465 7273 0a20 2020 2020 2020 2073 656c  ders.        sel
-00012b30: 662e 6173 7365 7274 4571 7561 6c28 2765  f.assertEqual('e
-00012b40: 6d61 696c 2032 3334 272c 2068 6561 6465  mail 234', heade
-00012b50: 7273 5b27 582d 4175 7468 2d45 6d61 696c  rs['X-Auth-Email
-00012b60: 275d 290a 2020 2020 2020 2020 7365 6c66  ']).        self
-00012b70: 2e61 7373 6572 7445 7175 616c 2827 746f  .assertEqual('to
-00012b80: 6b65 6e20 3132 3327 2c20 6865 6164 6572  ken 123', header
-00012b90: 735b 2758 2d41 7574 682d 4b65 7927 5d29  s['X-Auth-Key'])
-00012ba0: 0a0a 2020 2020 2020 2020 7072 6f76 6964  ..        provid
-00012bb0: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
-00012bc0: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
-00012bd0: 746f 6b65 6e3d 2774 6f6b 656e 2031 3233  token='token 123
-00012be0: 2729 0a20 2020 2020 2020 2068 6561 6465  ').        heade
-00012bf0: 7273 203d 2070 726f 7669 6465 722e 5f73  rs = provider._s
-00012c00: 6573 732e 6865 6164 6572 730a 2020 2020  ess.headers.    
-00012c10: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
-00012c20: 7175 616c 2827 4265 6172 6572 2074 6f6b  qual('Bearer tok
-00012c30: 656e 2031 3233 272c 2068 6561 6465 7273  en 123', headers
-00012c40: 5b27 4175 7468 6f72 697a 6174 696f 6e27  ['Authorization'
-00012c50: 5d29 0a20 2020 2020 2020 2073 656c 662e  ]).        self.
-00012c60: 6173 7365 7274 5472 7565 2868 6561 6465  assertTrue(heade
-00012c70: 7273 5b27 7573 6572 2d61 6765 6e74 275d  rs['user-agent']
-00012c80: 290a 0a20 2020 2064 6566 2074 6573 745f  )..    def test_
-00012c90: 7265 7472 795f 6265 6861 7669 6f72 2873  retry_behavior(s
-00012ca0: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
-00012cb0: 6f76 6964 6572 203d 2043 6c6f 7564 666c  ovider = Cloudfl
-00012cc0: 6172 6550 726f 7669 6465 7228 0a20 2020  areProvider(.   
-00012cd0: 2020 2020 2020 2020 2027 7465 7374 272c           'test',
-00012ce0: 2074 6f6b 656e 3d27 746f 6b65 6e20 3132   token='token 12
-00012cf0: 3327 2c20 656d 6169 6c3d 2765 6d61 696c  3', email='email
-00012d00: 2032 3334 272c 2072 6574 7279 5f70 6572   234', retry_per
-00012d10: 696f 643d 300a 2020 2020 2020 2020 290a  iod=0.        ).
-00012d20: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00012d30: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00012d40: 7375 6363 6573 7322 3a20 5472 7565 2c0a  success": True,.
-00012d50: 2020 2020 2020 2020 2020 2020 2265 7272              "err
-00012d60: 6f72 7322 3a20 5b5d 2c0a 2020 2020 2020  ors": [],.      
-00012d70: 2020 2020 2020 226d 6573 7361 6765 7322        "messages"
-00012d80: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
-00012d90: 2020 2272 6573 756c 7422 3a20 5b5d 2c0a    "result": [],.
-00012da0: 2020 2020 2020 2020 2020 2020 2272 6573              "res
-00012db0: 756c 745f 696e 666f 223a 207b 2263 6f75  ult_info": {"cou
-00012dc0: 6e74 223a 2031 2c20 2270 6572 5f70 6167  nt": 1, "per_pag
-00012dd0: 6522 3a20 3530 7d2c 0a20 2020 2020 2020  e": 50},.       
-00012de0: 207d 0a20 2020 2020 2020 207a 6f6e 6520   }.        zone 
-00012df0: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
-00012e00: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
-00012e10: 2020 7072 6f76 6964 6572 2e5f 7265 7175    provider._requ
-00012e20: 6573 7420 3d20 4d6f 636b 2829 0a0a 2020  est = Mock()..  
-00012e30: 2020 2020 2020 2320 4e6f 2072 6574 7279        # No retry
-00012e40: 2072 6571 7569 7265 642c 206a 7573 7420   required, just 
-00012e50: 6361 6c6c 7320 616e 6420 6973 2072 6574  calls and is ret
-00012e60: 7572 6e65 640a 2020 2020 2020 2020 7072  urned.        pr
-00012e70: 6f76 6964 6572 2e5f 7a6f 6e65 7320 3d20  ovider._zones = 
-00012e80: 4e6f 6e65 0a20 2020 2020 2020 2070 726f  None.        pro
-00012e90: 7669 6465 722e 5f72 6571 7565 7374 2e72  vider._request.r
-00012ea0: 6573 6574 5f6d 6f63 6b28 290a 2020 2020  eset_mock().    
-00012eb0: 2020 2020 7072 6f76 6964 6572 2e5f 7265      provider._re
-00012ec0: 7175 6573 742e 7369 6465 5f65 6666 6563  quest.side_effec
-00012ed0: 7420 3d20 5b72 6573 756c 745d 0a20 2020  t = [result].   
-00012ee0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00012ef0: 4571 7561 6c28 5b5d 2c20 7072 6f76 6964  Equal([], provid
-00012f00: 6572 2e7a 6f6e 655f 7265 636f 7264 7328  er.zone_records(
-00012f10: 7a6f 6e65 2929 0a20 2020 2020 2020 2070  zone)).        p
-00012f20: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
-00012f30: 2e61 7373 6572 745f 6861 735f 6361 6c6c  .assert_has_call
-00012f40: 7328 0a20 2020 2020 2020 2020 2020 205b  s(.            [
-00012f50: 6361 6c6c 2827 4745 5427 2c20 272f 7a6f  call('GET', '/zo
-00012f60: 6e65 7327 2c20 7061 7261 6d73 3d7b 2770  nes', params={'p
-00012f70: 6167 6527 3a20 312c 2027 7065 725f 7061  age': 1, 'per_pa
-00012f80: 6765 273a 2035 307d 295d 0a20 2020 2020  ge': 50})].     
-00012f90: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-00012fa0: 4f6e 6520 7265 7472 7920 7265 7175 6972  One retry requir
-00012fb0: 6564 0a20 2020 2020 2020 2070 726f 7669  ed.        provi
-00012fc0: 6465 722e 5f7a 6f6e 6573 203d 204e 6f6e  der._zones = Non
-00012fd0: 650a 2020 2020 2020 2020 7072 6f76 6964  e.        provid
-00012fe0: 6572 2e5f 7265 7175 6573 742e 7265 7365  er._request.rese
-00012ff0: 745f 6d6f 636b 2829 0a20 2020 2020 2020  t_mock().       
-00013000: 2070 726f 7669 6465 722e 5f72 6571 7565   provider._reque
-00013010: 7374 2e73 6964 655f 6566 6665 6374 203d  st.side_effect =
-00013020: 205b 436c 6f75 6466 6c61 7265 5261 7465   [CloudflareRate
-00013030: 4c69 6d69 7445 7272 6f72 2827 7b7d 2729  LimitError('{}')
-00013040: 2c20 7265 7375 6c74 5d0a 2020 2020 2020  , result].      
-00013050: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-00013060: 616c 285b 5d2c 2070 726f 7669 6465 722e  al([], provider.
-00013070: 7a6f 6e65 5f72 6563 6f72 6473 287a 6f6e  zone_records(zon
-00013080: 6529 290a 2020 2020 2020 2020 7072 6f76  e)).        prov
-00013090: 6964 6572 2e5f 7265 7175 6573 742e 6173  ider._request.as
-000130a0: 7365 7274 5f68 6173 5f63 616c 6c73 280a  sert_has_calls(.
-000130b0: 2020 2020 2020 2020 2020 2020 5b63 616c              [cal
-000130c0: 6c28 2747 4554 272c 2027 2f7a 6f6e 6573  l('GET', '/zones
-000130d0: 272c 2070 6172 616d 733d 7b27 7061 6765  ', params={'page
-000130e0: 273a 2031 2c20 2770 6572 5f70 6167 6527  ': 1, 'per_page'
-000130f0: 3a20 3530 7d29 5d0a 2020 2020 2020 2020  : 50})].        
-00013100: 290a 0a20 2020 2020 2020 2023 2054 776f  )..        # Two
-00013110: 2072 6574 7269 6573 2072 6571 7569 7265   retries require
-00013120: 640a 2020 2020 2020 2020 7072 6f76 6964  d.        provid
-00013130: 6572 2e5f 7a6f 6e65 7320 3d20 4e6f 6e65  er._zones = None
-00013140: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
-00013150: 722e 5f72 6571 7565 7374 2e72 6573 6574  r._request.reset
-00013160: 5f6d 6f63 6b28 290a 2020 2020 2020 2020  _mock().        
+00012770: 2020 2020 2269 6422 3a20 2266 6331 3261      "id": "fc12a
+00012780: 6233 3463 6435 3631 3133 3334 3432 3261  b34cd5611334422a
+00012790: 6233 3332 3239 3937 3634 3222 2c0a 2020  b3322997642",.  
+000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127b0: 2020 2274 7970 6522 3a20 2243 4e41 4d45    "type": "CNAME
+000127c0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000127d0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000127e0: 612e 756e 6974 2e74 6573 7473 222c 0a20  a.unit.tests",. 
+000127f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012800: 2020 2022 636f 6e74 656e 7422 3a20 2277     "content": "w
+00012810: 7777 2e75 6e69 742e 7465 7374 7322 2c0a  ww.unit.tests",.
+00012820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012830: 2020 2020 2270 726f 7869 6162 6c65 223a      "proxiable":
+00012840: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00012850: 2020 2020 2020 2020 2020 2022 7072 6f78             "prox
+00012860: 6965 6422 3a20 4661 6c73 652c 0a20 2020  ied": False,.   
+00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012880: 2022 7474 6c22 3a20 3330 302c 0a20 2020   "ttl": 300,.   
+00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128a0: 2022 6c6f 636b 6564 223a 2046 616c 7365   "locked": False
+000128b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000128c0: 2020 2020 2020 227a 6f6e 655f 6964 223a        "zone_id":
+000128d0: 2022 6666 3132 6162 3334 6364 3536 3131   "ff12ab34cd5611
+000128e0: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
+000128f0: 3530 222c 0a20 2020 2020 2020 2020 2020  50",.           
+00012900: 2020 2020 2020 2020 2022 7a6f 6e65 5f6e           "zone_n
+00012910: 616d 6522 3a20 2275 6e69 742e 7465 7374  ame": "unit.test
+00012920: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00012930: 2020 2020 2020 2020 226d 6f64 6966 6965          "modifie
+00012940: 645f 6f6e 223a 2022 3230 3137 2d30 332d  d_on": "2017-03-
+00012950: 3131 5431 383a 3031 3a34 332e 3432 3036  11T18:01:43.4206
+00012960: 3839 5a22 2c0a 2020 2020 2020 2020 2020  89Z",.          
+00012970: 2020 2020 2020 2020 2020 2263 7265 6174            "creat
+00012980: 6564 5f6f 6e22 3a20 2232 3031 372d 3033  ed_on": "2017-03
+00012990: 2d31 3154 3138 3a30 313a 3433 2e34 3230  -11T18:01:43.420
+000129a0: 3638 395a 222c 0a20 2020 2020 2020 2020  689Z",.         
+000129b0: 2020 2020 2020 2020 2020 2022 6d65 7461             "meta
+000129c0: 223a 207b 2261 7574 6f5f 6164 6465 6422  ": {"auto_added"
+000129d0: 3a20 4661 6c73 657d 2c0a 2020 2020 2020  : False},.      
+000129e0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+000129f0: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00012a00: 2020 290a 2020 2020 2020 2020 6465 7369    ).        desi
+00012a10: 7265 6420 3d20 5a6f 6e65 2827 756e 6974  red = Zone('unit
+00012a20: 2e74 6573 7473 2e27 2c20 5b5d 290a 2020  .tests.', []).  
+00012a30: 2020 2020 2020 7072 6f76 6964 6572 2e70        provider.p
+00012a40: 6f70 756c 6174 6528 6465 7369 7265 6429  opulate(desired)
+00012a50: 0a20 2020 2020 2020 2063 6861 6e67 6573  .        changes
+00012a60: 203d 2065 7869 7374 696e 672e 6368 616e   = existing.chan
+00012a70: 6765 7328 6465 7369 7265 642c 2070 726f  ges(desired, pro
+00012a80: 7669 6465 7229 0a0a 2020 2020 2020 2020  vider)..        
+00012a90: 6578 7472 615f 6368 616e 6765 7320 3d20  extra_changes = 
+00012aa0: 7072 6f76 6964 6572 2e5f 6578 7472 615f  provider._extra_
+00012ab0: 6368 616e 6765 7328 6578 6973 7469 6e67  changes(existing
+00012ac0: 2c20 6465 7369 7265 642c 2063 6861 6e67  , desired, chang
+00012ad0: 6573 290a 0a20 2020 2020 2020 2073 656c  es)..        sel
+00012ae0: 662e 6173 7365 7274 4571 7561 6c28 312c  f.assertEqual(1,
+00012af0: 206c 656e 2865 7874 7261 5f63 6861 6e67   len(extra_chang
+00012b00: 6573 2929 0a20 2020 2020 2020 2073 656c  es)).        sel
+00012b10: 662e 6173 7365 7274 5472 7565 280a 2020  f.assertTrue(.  
+00012b20: 2020 2020 2020 2020 2020 6578 7472 615f            extra_
+00012b30: 6368 616e 6765 735b 305d 2e65 7869 7374  changes[0].exist
+00012b40: 696e 672e 5f6f 6374 6f64 6e73 5b27 636c  ing._octodns['cl
+00012b50: 6f75 6466 6c61 7265 275d 5b27 7072 6f78  oudflare']['prox
+00012b60: 6965 6427 5d0a 2020 2020 2020 2020 290a  ied'].        ).
+00012b70: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00012b80: 6572 7446 616c 7365 280a 2020 2020 2020  ertFalse(.      
+00012b90: 2020 2020 2020 6578 7472 615f 6368 616e        extra_chan
+00012ba0: 6765 735b 305d 0a20 2020 2020 2020 2020  ges[0].         
+00012bb0: 2020 202e 6e65 772e 5f6f 6374 6f64 6e73     .new._octodns
+00012bc0: 2e67 6574 2827 636c 6f75 6466 6c61 7265  .get('cloudflare
+00012bd0: 272c 207b 7d29 0a20 2020 2020 2020 2020  ', {}).         
+00012be0: 2020 202e 6765 7428 2770 726f 7869 6564     .get('proxied
+00012bf0: 272c 2046 616c 7365 290a 2020 2020 2020  ', False).      
+00012c00: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+00012c10: 745f 656d 6169 6c6c 6573 735f 6175 7468  t_emailless_auth
+00012c20: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00012c30: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
+00012c40: 666c 6172 6550 726f 7669 6465 7228 0a20  flareProvider(. 
+00012c50: 2020 2020 2020 2020 2020 2027 7465 7374             'test
+00012c60: 272c 2074 6f6b 656e 3d27 746f 6b65 6e20  ', token='token 
+00012c70: 3132 3327 2c20 656d 6169 6c3d 2765 6d61  123', email='ema
+00012c80: 696c 2032 3334 270a 2020 2020 2020 2020  il 234'.        
+00012c90: 290a 2020 2020 2020 2020 6865 6164 6572  ).        header
+00012ca0: 7320 3d20 7072 6f76 6964 6572 2e5f 7365  s = provider._se
+00012cb0: 7373 2e68 6561 6465 7273 0a20 2020 2020  ss.headers.     
+00012cc0: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00012cd0: 7561 6c28 2765 6d61 696c 2032 3334 272c  ual('email 234',
+00012ce0: 2068 6561 6465 7273 5b27 582d 4175 7468   headers['X-Auth
+00012cf0: 2d45 6d61 696c 275d 290a 2020 2020 2020  -Email']).      
+00012d00: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00012d10: 616c 2827 746f 6b65 6e20 3132 3327 2c20  al('token 123', 
+00012d20: 6865 6164 6572 735b 2758 2d41 7574 682d  headers['X-Auth-
+00012d30: 4b65 7927 5d29 0a0a 2020 2020 2020 2020  Key'])..        
+00012d40: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
+00012d50: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
+00012d60: 6573 7427 2c20 746f 6b65 6e3d 2774 6f6b  est', token='tok
+00012d70: 656e 2031 3233 2729 0a20 2020 2020 2020  en 123').       
+00012d80: 2068 6561 6465 7273 203d 2070 726f 7669   headers = provi
+00012d90: 6465 722e 5f73 6573 732e 6865 6164 6572  der._sess.header
+00012da0: 730a 2020 2020 2020 2020 7365 6c66 2e61  s.        self.a
+00012db0: 7373 6572 7445 7175 616c 2827 4265 6172  ssertEqual('Bear
+00012dc0: 6572 2074 6f6b 656e 2031 3233 272c 2068  er token 123', h
+00012dd0: 6561 6465 7273 5b27 4175 7468 6f72 697a  eaders['Authoriz
+00012de0: 6174 696f 6e27 5d29 0a20 2020 2020 2020  ation']).       
+00012df0: 2073 656c 662e 6173 7365 7274 5472 7565   self.assertTrue
+00012e00: 2868 6561 6465 7273 5b27 7573 6572 2d61  (headers['user-a
+00012e10: 6765 6e74 275d 290a 0a20 2020 2064 6566  gent'])..    def
+00012e20: 2074 6573 745f 7265 7472 795f 6265 6861   test_retry_beha
+00012e30: 7669 6f72 2873 656c 6629 3a0a 2020 2020  vior(self):.    
+00012e40: 2020 2020 7072 6f76 6964 6572 203d 2043      provider = C
+00012e50: 6c6f 7564 666c 6172 6550 726f 7669 6465  loudflareProvide
+00012e60: 7228 0a20 2020 2020 2020 2020 2020 2027  r(.            '
+00012e70: 7465 7374 272c 2074 6f6b 656e 3d27 746f  test', token='to
+00012e80: 6b65 6e20 3132 3327 2c20 656d 6169 6c3d  ken 123', email=
+00012e90: 2765 6d61 696c 2032 3334 272c 2072 6574  'email 234', ret
+00012ea0: 7279 5f70 6572 696f 643d 300a 2020 2020  ry_period=0.    
+00012eb0: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
+00012ec0: 7375 6c74 203d 207b 0a20 2020 2020 2020  sult = {.       
+00012ed0: 2020 2020 2022 7375 6363 6573 7322 3a20       "success": 
+00012ee0: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00012ef0: 2020 2265 7272 6f72 7322 3a20 5b5d 2c0a    "errors": [],.
+00012f00: 2020 2020 2020 2020 2020 2020 226d 6573              "mes
+00012f10: 7361 6765 7322 3a20 5b5d 2c0a 2020 2020  sages": [],.    
+00012f20: 2020 2020 2020 2020 2272 6573 756c 7422          "result"
+00012f30: 3a20 5b5d 2c0a 2020 2020 2020 2020 2020  : [],.          
+00012f40: 2020 2272 6573 756c 745f 696e 666f 223a    "result_info":
+00012f50: 207b 2263 6f75 6e74 223a 2031 2c20 2270   {"count": 1, "p
+00012f60: 6572 5f70 6167 6522 3a20 3530 7d2c 0a20  er_page": 50},. 
+00012f70: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00012f80: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
+00012f90: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
+00012fa0: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00012fb0: 2e5f 7265 7175 6573 7420 3d20 4d6f 636b  ._request = Mock
+00012fc0: 2829 0a0a 2020 2020 2020 2020 2320 4e6f  ()..        # No
+00012fd0: 2072 6574 7279 2072 6571 7569 7265 642c   retry required,
+00012fe0: 206a 7573 7420 6361 6c6c 7320 616e 6420   just calls and 
+00012ff0: 6973 2072 6574 7572 6e65 640a 2020 2020  is returned.    
+00013000: 2020 2020 7072 6f76 6964 6572 2e5f 7a6f      provider._zo
+00013010: 6e65 7320 3d20 4e6f 6e65 0a20 2020 2020  nes = None.     
+00013020: 2020 2070 726f 7669 6465 722e 5f72 6571     provider._req
+00013030: 7565 7374 2e72 6573 6574 5f6d 6f63 6b28  uest.reset_mock(
+00013040: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
+00013050: 6572 2e5f 7265 7175 6573 742e 7369 6465  er._request.side
+00013060: 5f65 6666 6563 7420 3d20 5b72 6573 756c  _effect = [resul
+00013070: 745d 0a20 2020 2020 2020 2073 656c 662e  t].        self.
+00013080: 6173 7365 7274 4571 7561 6c28 5b5d 2c20  assertEqual([], 
+00013090: 7072 6f76 6964 6572 2e7a 6f6e 655f 7265  provider.zone_re
+000130a0: 636f 7264 7328 7a6f 6e65 2929 0a20 2020  cords(zone)).   
+000130b0: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
+000130c0: 6571 7565 7374 2e61 7373 6572 745f 6861  equest.assert_ha
+000130d0: 735f 6361 6c6c 7328 0a20 2020 2020 2020  s_calls(.       
+000130e0: 2020 2020 205b 6361 6c6c 2827 4745 5427       [call('GET'
+000130f0: 2c20 272f 7a6f 6e65 7327 2c20 7061 7261  , '/zones', para
+00013100: 6d73 3d7b 2770 6167 6527 3a20 312c 2027  ms={'page': 1, '
+00013110: 7065 725f 7061 6765 273a 2035 307d 295d  per_page': 50})]
+00013120: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00013130: 2020 2020 2320 4f6e 6520 7265 7472 7920      # One retry 
+00013140: 7265 7175 6972 6564 0a20 2020 2020 2020  required.       
+00013150: 2070 726f 7669 6465 722e 5f7a 6f6e 6573   provider._zones
+00013160: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
 00013170: 7072 6f76 6964 6572 2e5f 7265 7175 6573  provider._reques
-00013180: 742e 7369 6465 5f65 6666 6563 7420 3d20  t.side_effect = 
-00013190: 5b0a 2020 2020 2020 2020 2020 2020 436c  [.            Cl
-000131a0: 6f75 6466 6c61 7265 5261 7465 4c69 6d69  oudflareRateLimi
-000131b0: 7445 7272 6f72 2827 7b7d 2729 2c0a 2020  tError('{}'),.  
-000131c0: 2020 2020 2020 2020 2020 436c 6f75 6466            Cloudf
-000131d0: 6c61 7265 5261 7465 4c69 6d69 7445 7272  lareRateLimitErr
-000131e0: 6f72 2827 7b7d 2729 2c0a 2020 2020 2020  or('{}'),.      
-000131f0: 2020 2020 2020 7265 7375 6c74 2c0a 2020        result,.  
-00013200: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00013210: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00013220: 285b 5d2c 2070 726f 7669 6465 722e 7a6f  ([], provider.zo
-00013230: 6e65 5f72 6563 6f72 6473 287a 6f6e 6529  ne_records(zone)
-00013240: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
-00013250: 6572 2e5f 7265 7175 6573 742e 6173 7365  er._request.asse
-00013260: 7274 5f68 6173 5f63 616c 6c73 280a 2020  rt_has_calls(.  
-00013270: 2020 2020 2020 2020 2020 5b63 616c 6c28            [call(
-00013280: 2747 4554 272c 2027 2f7a 6f6e 6573 272c  'GET', '/zones',
-00013290: 2070 6172 616d 733d 7b27 7061 6765 273a   params={'page':
-000132a0: 2031 2c20 2770 6572 5f70 6167 6527 3a20   1, 'per_page': 
-000132b0: 3530 7d29 5d0a 2020 2020 2020 2020 290a  50})].        ).
-000132c0: 0a20 2020 2020 2020 2023 2023 2045 7868  .        # # Exh
-000132d0: 6175 7374 206f 7572 2072 6574 7269 6573  aust our retries
-000132e0: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
-000132f0: 722e 5f7a 6f6e 6573 203d 204e 6f6e 650a  r._zones = None.
-00013300: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
-00013310: 2e5f 7265 7175 6573 742e 7265 7365 745f  ._request.reset_
-00013320: 6d6f 636b 2829 0a20 2020 2020 2020 2070  mock().        p
-00013330: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
-00013340: 2e73 6964 655f 6566 6665 6374 203d 205b  .side_effect = [
-00013350: 0a20 2020 2020 2020 2020 2020 2043 6c6f  .            Clo
-00013360: 7564 666c 6172 6552 6174 654c 696d 6974  udflareRateLimit
-00013370: 4572 726f 7228 7b22 6572 726f 7273 223a  Error({"errors":
-00013380: 205b 7b22 6d65 7373 6167 6522 3a20 2266   [{"message": "f
-00013390: 6972 7374 227d 5d7d 292c 0a20 2020 2020  irst"}]}),.     
-000133a0: 2020 2020 2020 2043 6c6f 7564 666c 6172         Cloudflar
-000133b0: 6552 6174 654c 696d 6974 4572 726f 7228  eRateLimitError(
-000133c0: 7b22 6572 726f 7273 223a 205b 7b22 6d65  {"errors": [{"me
-000133d0: 7373 6167 6522 3a20 2262 6f6f 227d 5d7d  ssage": "boo"}]}
-000133e0: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-000133f0: 6c6f 7564 666c 6172 6552 6174 654c 696d  loudflareRateLim
-00013400: 6974 4572 726f 7228 7b22 6572 726f 7273  itError({"errors
-00013410: 223a 205b 7b22 6d65 7373 6167 6522 3a20  ": [{"message": 
-00013420: 2262 6f6f 227d 5d7d 292c 0a20 2020 2020  "boo"}]}),.     
-00013430: 2020 2020 2020 2043 6c6f 7564 666c 6172         Cloudflar
-00013440: 6552 6174 654c 696d 6974 4572 726f 7228  eRateLimitError(
-00013450: 7b22 6572 726f 7273 223a 205b 7b22 6d65  {"errors": [{"me
-00013460: 7373 6167 6522 3a20 2262 6f6f 227d 5d7d  ssage": "boo"}]}
-00013470: 292c 0a20 2020 2020 2020 2020 2020 2043  ),.            C
-00013480: 6c6f 7564 666c 6172 6552 6174 654c 696d  loudflareRateLim
-00013490: 6974 4572 726f 7228 7b22 6572 726f 7273  itError({"errors
-000134a0: 223a 205b 7b22 6d65 7373 6167 6522 3a20  ": [{"message": 
-000134b0: 226c 6173 7422 7d5d 7d29 2c0a 2020 2020  "last"}]}),.    
-000134c0: 2020 2020 5d0a 2020 2020 2020 2020 7769      ].        wi
-000134d0: 7468 2073 656c 662e 6173 7365 7274 5261  th self.assertRa
-000134e0: 6973 6573 2843 6c6f 7564 666c 6172 6552  ises(CloudflareR
-000134f0: 6174 654c 696d 6974 4572 726f 7229 2061  ateLimitError) a
-00013500: 7320 6374 783a 0a20 2020 2020 2020 2020  s ctx:.         
-00013510: 2020 2070 726f 7669 6465 722e 7a6f 6e65     provider.zone
-00013520: 5f72 6563 6f72 6473 287a 6f6e 6529 0a20  _records(zone). 
-00013530: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00013540: 6173 7365 7274 4571 7561 6c28 276c 6173  assertEqual('las
-00013550: 7427 2c20 7374 7228 6374 782e 6578 6365  t', str(ctx.exce
-00013560: 7074 696f 6e29 290a 0a20 2020 2064 6566  ption))..    def
-00013570: 2074 6573 745f 7474 6c5f 6d61 7070 696e   test_ttl_mappin
-00013580: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-00013590: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
-000135a0: 6466 6c61 7265 5072 6f76 6964 6572 2827  dflareProvider('
-000135b0: 7465 7374 272c 2027 656d 6169 6c27 2c20  test', 'email', 
-000135c0: 2774 6f6b 656e 2729 0a0a 2020 2020 2020  'token')..      
-000135d0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000135e0: 616c 2831 3230 2c20 7072 6f76 6964 6572  al(120, provider
-000135f0: 2e5f 7474 6c5f 6461 7461 2831 3230 2929  ._ttl_data(120))
-00013600: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00013610: 7365 7274 4571 7561 6c28 3132 302c 2070  sertEqual(120, p
-00013620: 726f 7669 6465 722e 5f74 746c 5f64 6174  rovider._ttl_dat
-00013630: 6128 3132 3029 290a 2020 2020 2020 2020  a(120)).        
-00013640: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00013650: 2833 3630 302c 2070 726f 7669 6465 722e  (3600, provider.
-00013660: 5f74 746c 5f64 6174 6128 3336 3030 2929  _ttl_data(3600))
-00013670: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
-00013680: 7365 7274 4571 7561 6c28 3330 302c 2070  sertEqual(300, p
-00013690: 726f 7669 6465 722e 5f74 746c 5f64 6174  rovider._ttl_dat
-000136a0: 6128 3129 290a 0a20 2020 2064 6566 2074  a(1))..    def t
-000136b0: 6573 745f 746c 7361 2873 656c 6629 3a0a  est_tlsa(self):.
-000136c0: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
-000136d0: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
-000136e0: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
-000136f0: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
-00013700: 0a20 2020 2020 2020 2063 665f 6461 7461  .        cf_data
-00013710: 203d 207b 0a20 2020 2020 2020 2020 2020   = {.           
-00013720: 2027 636f 6d6d 656e 7427 3a20 4e6f 6e65   'comment': None
-00013730: 2c0a 2020 2020 2020 2020 2020 2020 2763  ,.            'c
-00013740: 6f6e 7465 6e74 273a 2027 3120 3120 3120  ontent': '1 1 1 
-00013750: 6161 3432 3432 3432 3432 3432 3432 3432  aa42424242424242
-00013760: 3432 3432 3432 3432 3432 3432 3432 3432  4242424242424242
-00013770: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
-00013780: 6372 6561 7465 645f 6f6e 273a 2027 3230  created_on': '20
-00013790: 3232 2d31 322d 3233 5430 313a 3537 3a31  22-12-23T01:57:1
-000137a0: 342e 3536 3739 3835 5a27 2c0a 2020 2020  4.567985Z',.    
-000137b0: 2020 2020 2020 2020 2764 6174 6127 3a20          'data': 
-000137c0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000137d0: 2020 2763 6572 7469 6669 6361 7465 273a    'certificate':
-000137e0: 2027 6161 3432 3432 3432 3432 3432 3432   'aa424242424242
-000137f0: 3432 3432 3432 3432 3432 3432 3432 3432  4242424242424242
-00013800: 3432 272c 0a20 2020 2020 2020 2020 2020  42',.           
-00013810: 2020 2020 2027 6d61 7463 6869 6e67 5f74       'matching_t
-00013820: 7970 6527 3a20 312c 0a20 2020 2020 2020  ype': 1,.       
-00013830: 2020 2020 2020 2020 2027 7365 6c65 6374           'select
-00013840: 6f72 273a 2031 2c0a 2020 2020 2020 2020  or': 1,.        
-00013850: 2020 2020 2020 2020 2775 7361 6765 273a          'usage':
-00013860: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
-00013870: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
-00013880: 6964 273a 2027 3432 3939 3861 6336 3966  id': '42998ac69f
-00013890: 6334 6139 3563 6335 6338 3562 6539 6265  c4a95cc5c85be9be
-000138a0: 6632 6466 6265 272c 0a20 2020 2020 2020  f2dfbe',.       
-000138b0: 2020 2020 2027 6c6f 636b 6564 273a 2046       'locked': F
-000138c0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
-000138d0: 2020 276d 6574 6127 3a20 7b0a 2020 2020    'meta': {.    
-000138e0: 2020 2020 2020 2020 2020 2020 2761 7574              'aut
-000138f0: 6f5f 6164 6465 6427 3a20 4661 6c73 652c  o_added': False,
-00013900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013910: 2027 6d61 6e61 6765 645f 6279 5f61 7070   'managed_by_app
-00013920: 7327 3a20 4661 6c73 652c 0a20 2020 2020  s': False,.     
-00013930: 2020 2020 2020 2020 2020 2027 6d61 6e61             'mana
-00013940: 6765 645f 6279 5f61 7267 6f5f 7475 6e6e  ged_by_argo_tunn
-00013950: 656c 273a 2046 616c 7365 2c0a 2020 2020  el': False,.    
-00013960: 2020 2020 2020 2020 2020 2020 2773 6f75              'sou
-00013970: 7263 6527 3a20 2770 7269 6d61 7279 272c  rce': 'primary',
-00013980: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00013990: 2020 2020 2020 2020 2020 2020 276d 6f64              'mod
-000139a0: 6966 6965 645f 6f6e 273a 2027 3230 3232  ified_on': '2022
-000139b0: 2d31 322d 3233 5430 313a 3537 3a31 342e  -12-23T01:57:14.
-000139c0: 3536 3739 3835 5a27 2c0a 2020 2020 2020  567985Z',.      
-000139d0: 2020 2020 2020 276e 616d 6527 3a20 2774        'name': 't
-000139e0: 6c73 612e 756e 6974 2e74 6573 7473 272c  lsa.unit.tests',
-000139f0: 0a20 2020 2020 2020 2020 2020 2027 7072  .            'pr
-00013a00: 6f78 6961 626c 6527 3a20 4661 6c73 652c  oxiable': False,
-00013a10: 0a20 2020 2020 2020 2020 2020 2027 7072  .            'pr
-00013a20: 6f78 6965 6427 3a20 4661 6c73 652c 0a20  oxied': False,. 
-00013a30: 2020 2020 2020 2020 2020 2027 7461 6773             'tags
-00013a40: 273a 205b 5d2c 0a20 2020 2020 2020 2020  ': [],.         
-00013a50: 2020 2027 7474 6c27 3a20 312c 0a20 2020     'ttl': 1,.   
-00013a60: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
-00013a70: 2027 544c 5341 272c 0a20 2020 2020 2020   'TLSA',.       
-00013a80: 2020 2020 2027 7a6f 6e65 5f69 6427 3a20       'zone_id': 
-00013a90: 2763 6166 3931 3139 3763 6337 3933 3063  'caf91197cc7930c
-00013aa0: 3333 6237 3431 6563 3330 6432 3964 3930  33b741ec30d29d90
-00013ab0: 3927 2c0a 2020 2020 2020 2020 2020 2020  9',.            
-00013ac0: 277a 6f6e 655f 6e61 6d65 273a 2027 756e  'zone_name': 'un
-00013ad0: 6974 2e74 6573 7473 272c 0a20 2020 2020  it.tests',.     
-00013ae0: 2020 207d 0a20 2020 2020 2020 2064 6174     }.        dat
-00013af0: 6120 3d20 7072 6f76 6964 6572 2e5f 6461  a = provider._da
-00013b00: 7461 5f66 6f72 5f54 4c53 4128 2754 4c53  ta_for_TLSA('TLS
-00013b10: 4127 2c20 5b63 665f 6461 7461 5d29 0a20  A', [cf_data]). 
-00013b20: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
-00013b30: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
-00013b40: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
-00013b50: 2020 2020 2020 2027 7474 6c27 3a20 3330         'ttl': 30
-00013b60: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-00013b70: 2020 2027 7479 7065 273a 2027 544c 5341     'type': 'TLSA
-00013b80: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00013b90: 2020 2027 7661 6c75 6573 273a 205b 0a20     'values': [. 
-00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013bb0: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
-00013bc0: 2020 2020 2020 2020 2020 2020 2027 6365               'ce
-00013bd0: 7274 6966 6963 6174 655f 6173 736f 6369  rtificate_associ
-00013be0: 6174 696f 6e5f 6461 7461 273a 2027 6161  ation_data': 'aa
-00013bf0: 3432 3432 3432 3432 3432 3432 3432 3432  4242424242424242
-00013c00: 3432 3432 3432 3432 3432 3432 3432 272c  42424242424242',
-00013c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c20: 2020 2020 2020 2020 2027 6365 7274 6966           'certif
-00013c30: 6963 6174 655f 7573 6167 6527 3a20 312c  icate_usage': 1,
-00013c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013c50: 2020 2020 2020 2020 2027 6d61 7463 6869           'matchi
-00013c60: 6e67 5f74 7970 6527 3a20 312c 0a20 2020  ng_type': 1,.   
-00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c80: 2020 2020 2027 7365 6c65 6374 6f72 273a       'selector':
-00013c90: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
-00013ca0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00013cb0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00013cc0: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
-00013cd0: 2020 2020 2020 2020 6461 7461 2c0a 2020          data,.  
-00013ce0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00013cf0: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
-00013d00: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
-00013d10: 2020 2020 2020 2020 7265 636f 7264 203d          record =
-00013d20: 2052 6563 6f72 642e 6e65 7728 7a6f 6e65   Record.new(zone
-00013d30: 2c20 2774 6c73 6127 2c20 6461 7461 290a  , 'tlsa', data).
-00013d40: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-00013d50: 203d 206c 6973 7428 7072 6f76 6964 6572   = list(provider
-00013d60: 2e5f 636f 6e74 656e 7473 5f66 6f72 5f54  ._contents_for_T
-00013d70: 4c53 4128 7265 636f 7264 2929 0a20 2020  LSA(record)).   
-00013d80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00013d90: 4571 7561 6c28 5b7b 2764 6174 6127 3a20  Equal([{'data': 
-00013da0: 6366 5f64 6174 615b 2764 6174 6127 5d7d  cf_data['data']}
-00013db0: 5d2c 2063 6f6e 7465 6e74 7329 0a0a 2020  ], contents)..  
-00013dc0: 2020 2020 2020 6b65 7920 3d20 7072 6f76        key = prov
-00013dd0: 6964 6572 2e5f 6765 6e5f 6b65 7928 6366  ider._gen_key(cf
-00013de0: 5f64 6174 6129 0a20 2020 2020 2020 2073  _data).        s
-00013df0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00013e00: 2731 2031 2031 2061 6134 3234 3234 3234  '1 1 1 aa4242424
-00013e10: 3234 3234 3234 3234 3234 3234 3234 3234  2424242424242424
-00013e20: 3234 3234 3234 3227 2c20 6b65 7929 0a0a  2424242', key)..
-00013e30: 2020 2020 6465 6620 7465 7374 5f6e 6f5f      def test_no_
-00013e40: 7370 665f 6372 6561 7465 2873 656c 6629  spf_create(self)
-00013e50: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
-00013e60: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
-00013e70: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
-00013e80: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
-00013e90: 2c20 7265 7472 795f 7065 7269 6f64 3d30  , retry_period=0
-00013ea0: 290a 0a20 2020 2020 2020 207a 6f6e 6520  )..        zone 
-00013eb0: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
-00013ec0: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
-00013ed0: 2020 6131 203d 2052 6563 6f72 642e 6e65    a1 = Record.ne
-00013ee0: 7728 0a20 2020 2020 2020 2020 2020 207a  w(.            z
-00013ef0: 6f6e 652c 2027 6127 2c20 7b27 7479 7065  one, 'a', {'type
-00013f00: 273a 2027 4127 2c20 2774 746c 273a 2034  ': 'A', 'ttl': 4
-00013f10: 3230 2c20 2776 616c 7565 273a 2027 312e  20, 'value': '1.
-00013f20: 322e 332e 3427 7d0a 2020 2020 2020 2020  2.3.4'}.        
-00013f30: 290a 2020 2020 2020 2020 6132 203d 2061  ).        a2 = a
-00013f40: 312e 636f 7079 2829 0a20 2020 2020 2020  1.copy().       
-00013f50: 2061 322e 7474 6c20 2b3d 2031 0a20 2020   a2.ttl += 1.   
-00013f60: 2020 2020 2073 7066 3120 3d20 5265 636f       spf1 = Reco
-00013f70: 7264 2e6e 6577 280a 2020 2020 2020 2020  rd.new(.        
-00013f80: 2020 2020 7a6f 6e65 2c20 2773 7066 272c      zone, 'spf',
-00013f90: 207b 2774 7970 6527 3a20 2753 5046 272c   {'type': 'SPF',
-00013fa0: 2027 7474 6c27 3a20 3433 302c 2027 7661   'ttl': 430, 'va
-00013fb0: 6c75 6527 3a20 2762 6c61 6862 6c61 6827  lue': 'blahblah'
-00013fc0: 7d0a 2020 2020 2020 2020 290a 2020 2020  }.        ).    
-00013fd0: 2020 2020 7370 6632 203d 2073 7066 312e      spf2 = spf1.
-00013fe0: 636f 7079 2829 0a20 2020 2020 2020 2073  copy().        s
-00013ff0: 7066 322e 7474 6c20 2b3d 2031 0a0a 2020  pf2.ttl += 1..  
-00014000: 2020 2020 2020 2320 4120 6973 2061 6c77        # A is alw
-00014010: 6179 7320 696e 636c 7564 6564 0a20 2020  ays included.   
-00014020: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-00014030: 5472 7565 2870 726f 7669 6465 722e 5f69  True(provider._i
-00014040: 6e63 6c75 6465 5f63 6861 6e67 6528 4372  nclude_change(Cr
-00014050: 6561 7465 2861 3129 2929 0a20 2020 2020  eate(a1))).     
-00014060: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00014070: 7565 2870 726f 7669 6465 722e 5f69 6e63  ue(provider._inc
-00014080: 6c75 6465 5f63 6861 6e67 6528 5570 6461  lude_change(Upda
-00014090: 7465 2861 312c 2061 3229 2929 0a20 2020  te(a1, a2))).   
-000140a0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
-000140b0: 5472 7565 2870 726f 7669 6465 722e 5f69  True(provider._i
-000140c0: 6e63 6c75 6465 5f63 6861 6e67 6528 4465  nclude_change(De
-000140d0: 6c65 7465 2861 3129 2929 0a0a 2020 2020  lete(a1)))..    
-000140e0: 2020 2020 2320 5350 4620 6361 6e27 7420      # SPF can't 
-000140f0: 6265 2063 7265 6174 6564 2c20 7570 6461  be created, upda
-00014100: 7465 7320 616e 6420 6465 6c65 7465 7320  tes and deletes 
-00014110: 6172 6520 4f4b 0a20 2020 2020 2020 2077  are OK.        w
-00014120: 6974 6820 7365 6c66 2e61 7373 6572 7452  ith self.assertR
-00014130: 6169 7365 7328 5375 7070 6f72 7473 4578  aises(SupportsEx
-00014140: 6365 7074 696f 6e29 2061 7320 6374 783a  ception) as ctx:
-00014150: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00014160: 7669 6465 722e 5f69 6e63 6c75 6465 5f63  vider._include_c
-00014170: 6861 6e67 6528 4372 6561 7465 2873 7066  hange(Create(spf
-00014180: 3129 290a 2020 2020 2020 2020 7365 6c66  1)).        self
-00014190: 2e61 7373 6572 7445 7175 616c 280a 2020  .assertEqual(.  
-000141a0: 2020 2020 2020 2020 2020 2774 6573 743a            'test:
-000141b0: 2063 7265 6174 696e 6720 6e65 7720 5350   creating new SP
-000141c0: 4620 7265 636f 7264 7320 6e6f 7420 7375  F records not su
-000141d0: 7070 6f72 7465 642c 2075 7365 2054 5854  pported, use TXT
-000141e0: 2069 6e73 7465 6164 272c 0a20 2020 2020   instead',.     
-000141f0: 2020 2020 2020 2073 7472 2863 7478 2e65         str(ctx.e
-00014200: 7863 6570 7469 6f6e 292c 0a20 2020 2020  xception),.     
-00014210: 2020 2029 0a20 2020 2020 2020 2073 656c     ).        sel
-00014220: 662e 6173 7365 7274 5472 7565 2870 726f  f.assertTrue(pro
-00014230: 7669 6465 722e 5f69 6e63 6c75 6465 5f63  vider._include_c
-00014240: 6861 6e67 6528 5570 6461 7465 2873 7066  hange(Update(spf
-00014250: 312c 2073 7066 3229 2929 0a20 2020 2020  1, spf2))).     
-00014260: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
-00014270: 7565 2870 726f 7669 6465 722e 5f69 6e63  ue(provider._inc
-00014280: 6c75 6465 5f63 6861 6e67 6528 4465 6c65  lude_change(Dele
-00014290: 7465 2873 7066 3129 2929 0a0a 2020 2020  te(spf1)))..    
-000142a0: 6465 6620 7465 7374 5f73 7368 6670 2873  def test_sshfp(s
-000142b0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
-000142c0: 6c66 2e6d 6178 4469 6666 203d 204e 6f6e  lf.maxDiff = Non
-000142d0: 650a 2020 2020 2020 2020 7072 6f76 6964  e.        provid
-000142e0: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
-000142f0: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
-00014300: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
-00014310: 290a 0a20 2020 2020 2020 2063 665f 6461  )..        cf_da
-00014320: 7461 203d 207b 0a20 2020 2020 2020 2020  ta = {.         
-00014330: 2020 2027 636f 6d6d 656e 7427 3a20 4e6f     'comment': No
-00014340: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-00014350: 2763 6f6e 7465 6e74 273a 2027 3120 3220  'content': '1 2 
-00014360: 3835 3962 6536 6564 3034 3634 3364 6234  859be6ed04643db4
-00014370: 3131 6630 3637 6236 6331 6461 3164 3735  11f067b6c1da1d75
-00014380: 6665 3038 6236 3732 272c 0a20 2020 2020  fe08b672',.     
-00014390: 2020 2020 2020 2027 6372 6561 7465 645f         'created_
-000143a0: 6f6e 273a 2027 3230 3233 2d30 332d 3032  on': '2023-03-02
-000143b0: 5430 313a 3032 3a34 342e 3536 3739 3835  T01:02:44.567985
-000143c0: 5a27 2c0a 2020 2020 2020 2020 2020 2020  Z',.            
-000143d0: 2764 6174 6127 3a20 7b0a 2020 2020 2020  'data': {.      
-000143e0: 2020 2020 2020 2020 2020 2761 6c67 6f72            'algor
-000143f0: 6974 686d 273a 2031 2c0a 2020 2020 2020  ithm': 1,.      
-00014400: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
-00014410: 3a20 322c 0a20 2020 2020 2020 2020 2020  : 2,.           
-00014420: 2020 2020 2027 6669 6e67 6572 7072 696e       'fingerprin
-00014430: 7427 3a20 2738 3539 6265 3665 6430 3436  t': '859be6ed046
-00014440: 3433 6462 3431 3166 3036 3762 3663 3164  43db411f067b6c1d
-00014450: 6131 6437 3566 6530 3862 3637 3227 2c0a  a1d75fe08b672',.
-00014460: 2020 2020 2020 2020 2020 2020 7d2c 0a20              },. 
-00014470: 2020 2020 2020 2020 2020 2027 6964 273a             'id':
-00014480: 2027 6767 6f7a 7274 6e7a 6231 316e 7272   'ggozrtnzb11nrr
-00014490: 3971 7334 6b6f 3679 336a 3139 716b 6568  9qs4ko6y3j19qkeh
-000144a0: 7578 3927 2c0a 2020 2020 2020 2020 2020  ux9',.          
-000144b0: 2020 276c 6f63 6b65 6427 3a20 4661 6c73    'locked': Fals
-000144c0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
-000144d0: 6d65 7461 273a 207b 0a20 2020 2020 2020  meta': {.       
-000144e0: 2020 2020 2020 2020 2027 6175 746f 5f61           'auto_a
-000144f0: 6464 6564 273a 2046 616c 7365 2c0a 2020  dded': False,.  
-00014500: 2020 2020 2020 2020 2020 2020 2020 276d                'm
-00014510: 616e 6167 6564 5f62 795f 6170 7073 273a  anaged_by_apps':
-00014520: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
-00014530: 2020 2020 2020 2020 276d 616e 6167 6564          'managed
-00014540: 5f62 795f 6172 676f 5f74 756e 6e65 6c27  _by_argo_tunnel'
-00014550: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
-00014560: 2020 2020 2020 2020 2027 736f 7572 6365           'source
-00014570: 273a 2027 7072 696d 6172 7927 2c0a 2020  ': 'primary',.  
-00014580: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
-00014590: 2020 2020 2020 2020 2027 6d6f 6469 6669           'modifi
-000145a0: 6564 5f6f 6e27 3a20 2732 3032 332d 3033  ed_on': '2023-03
-000145b0: 2d30 3254 3031 3a30 323a 3434 2e35 3637  -02T01:02:44.567
-000145c0: 3938 355a 272c 0a20 2020 2020 2020 2020  985Z',.         
-000145d0: 2020 2027 6e61 6d65 273a 2027 6e61 7074     'name': 'napt
-000145e0: 722e 756e 6974 2e74 6573 7473 272c 0a20  r.unit.tests',. 
-000145f0: 2020 2020 2020 2020 2020 2027 7072 6f78             'prox
-00014600: 6961 626c 6527 3a20 4661 6c73 652c 0a20  iable': False,. 
-00014610: 2020 2020 2020 2020 2020 2027 7072 6f78             'prox
-00014620: 6965 6427 3a20 4661 6c73 652c 0a20 2020  ied': False,.   
-00014630: 2020 2020 2020 2020 2027 7461 6773 273a           'tags':
-00014640: 205b 5d2c 0a20 2020 2020 2020 2020 2020   [],.           
-00014650: 2027 7474 6c27 3a20 3330 302c 0a20 2020   'ttl': 300,.   
-00014660: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
-00014670: 2027 5353 4846 5027 2c0a 2020 2020 2020   'SSHFP',.      
-00014680: 2020 2020 2020 277a 6f6e 655f 6964 273a        'zone_id':
-00014690: 2027 6666 3132 6162 3334 6364 3536 3131   'ff12ab34cd5611
-000146a0: 3333 3434 3232 6162 3333 3232 3939 3736  334422ab33229976
-000146b0: 3530 272c 0a20 2020 2020 2020 2020 2020  50',.           
-000146c0: 2027 7a6f 6e65 5f6e 616d 6527 3a20 2775   'zone_name': 'u
-000146d0: 6e69 742e 7465 7374 7327 2c0a 2020 2020  nit.tests',.    
-000146e0: 2020 2020 7d0a 2020 2020 2020 2020 6461      }.        da
-000146f0: 7461 203d 2070 726f 7669 6465 722e 5f64  ta = provider._d
-00014700: 6174 615f 666f 725f 5353 4846 5028 2753  ata_for_SSHFP('S
-00014710: 5348 4650 272c 205b 6366 5f64 6174 615d  SHFP', [cf_data]
-00014720: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
-00014730: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
-00014740: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-00014750: 2020 2020 2020 2020 2020 2774 746c 273a            'ttl':
-00014760: 2033 3030 2c0a 2020 2020 2020 2020 2020   300,.          
-00014770: 2020 2020 2020 2774 7970 6527 3a20 2753        'type': 'S
-00014780: 5348 4650 272c 0a20 2020 2020 2020 2020  SHFP',.         
-00014790: 2020 2020 2020 2027 7661 6c75 6573 273a         'values':
-000147a0: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
-000147b0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2027 616c 676f 7269 7468 6d27 3a20 312c   'algorithm': 1,
-000147e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000147f0: 2020 2020 2020 2020 2027 6669 6e67 6572           'finger
-00014800: 7072 696e 745f 7479 7065 273a 2032 2c0a  print_type': 2,.
-00014810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014820: 2020 2020 2020 2020 2766 696e 6765 7270          'fingerp
-00014830: 7269 6e74 273a 2027 3835 3962 6536 6564  rint': '859be6ed
-00014840: 3034 3634 3364 6234 3131 6630 3637 6236  04643db411f067b6
-00014850: 6331 6461 3164 3735 6665 3038 6236 3732  c1da1d75fe08b672
-00014860: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00014870: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00014880: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
-00014890: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-000148a0: 2020 2020 2020 2064 6174 612c 0a20 2020         data,.   
-000148b0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000148c0: 7a6f 6e65 203d 205a 6f6e 6528 2775 6e69  zone = Zone('uni
-000148d0: 742e 7465 7374 732e 272c 205b 5d29 0a20  t.tests.', []). 
-000148e0: 2020 2020 2020 2072 6563 6f72 6420 3d20         record = 
-000148f0: 5265 636f 7264 2e6e 6577 287a 6f6e 652c  Record.new(zone,
-00014900: 2027 7373 6866 7027 2c20 6461 7461 290a   'sshfp', data).
-00014910: 2020 2020 2020 2020 636f 6e74 656e 7473          contents
-00014920: 203d 206c 6973 7428 7072 6f76 6964 6572   = list(provider
-00014930: 2e5f 636f 6e74 656e 7473 5f66 6f72 5f53  ._contents_for_S
-00014940: 5348 4650 2872 6563 6f72 6429 290a 2020  SHFP(record)).  
-00014950: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
-00014960: 7445 7175 616c 285b 7b27 6461 7461 273a  tEqual([{'data':
-00014970: 2063 665f 6461 7461 5b27 6461 7461 275d   cf_data['data']
-00014980: 7d5d 2c20 636f 6e74 656e 7473 290a 0a20  }], contents).. 
-00014990: 2020 2020 2020 206b 6579 203d 2070 726f         key = pro
-000149a0: 7669 6465 722e 5f67 656e 5f6b 6579 2863  vider._gen_key(c
-000149b0: 665f 6461 7461 290a 2020 2020 2020 2020  f_data).        
-000149c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-000149d0: 2827 3120 3220 3835 3962 6536 6564 3034  ('1 2 859be6ed04
-000149e0: 3634 3364 6234 3131 6630 3637 6236 6331  643db411f067b6c1
-000149f0: 6461 3164 3735 6665 3038 6236 3732 272c  da1d75fe08b672',
-00014a00: 206b 6579 290a 0a20 2020 2064 6566 2074   key)..    def t
-00014a10: 6573 745f 6964 6e61 5f64 6f6d 6169 6e28  est_idna_domain(
-00014a20: 7365 6c66 293a 0a20 2020 2020 2020 2073  self):.        s
-00014a30: 656c 662e 6d61 7844 6966 6620 3d20 4e6f  elf.maxDiff = No
-00014a40: 6e65 0a20 2020 2020 2020 2070 726f 7669  ne.        provi
-00014a50: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
-00014a60: 5072 6f76 6964 6572 2827 7465 7374 272c  Provider('test',
-00014a70: 2027 656d 6169 6c27 2c20 2774 6f6b 656e   'email', 'token
-00014a80: 2729 0a20 2020 2020 2020 2023 2065 7869  ').        # exi
-00014a90: 7374 696e 6720 7a6f 6e65 2077 6974 6820  sting zone with 
-00014aa0: 6461 7461 0a20 2020 2020 2020 2077 6974  data.        wit
-00014ab0: 6820 7265 7175 6573 7473 5f6d 6f63 6b28  h requests_mock(
-00014ac0: 2920 6173 206d 6f63 6b3a 0a20 2020 2020  ) as mock:.     
-00014ad0: 2020 2020 2020 2062 6173 6520 3d20 2768         base = 'h
-00014ae0: 7474 7073 3a2f 2f61 7069 2e63 6c6f 7564  ttps://api.cloud
-00014af0: 666c 6172 652e 636f 6d2f 636c 6965 6e74  flare.com/client
-00014b00: 2f76 342f 7a6f 6e65 7327 0a20 2020 2020  /v4/zones'.     
-00014b10: 2020 2020 2020 2069 646e 615f 7a6f 6e65         idna_zone
-00014b20: 5f69 6420 3d20 2732 3334 3233 3432 3433  _id = '234234243
-00014b30: 3432 3361 6161 6262 3333 3433 3432 6262  423aaabb334342bb
-00014b40: 6233 3433 3433 3327 0a20 2020 2020 2020  b343433'.       
-00014b50: 2020 2020 2023 207a 6f6e 6520 666f 7220       # zone for 
-00014b60: 6964 6e61 207a 6f6e 6520 6973 2069 6e20  idna zone is in 
-00014b70: 7061 6765 2033 0a20 2020 2020 2020 2020  page 3.         
-00014b80: 2020 2077 6974 6820 6f70 656e 2827 7465     with open('te
-00014b90: 7374 732f 6669 7874 7572 6573 2f63 6c6f  sts/fixtures/clo
-00014ba0: 7564 666c 6172 652d 7a6f 6e65 732d 7061  udflare-zones-pa
-00014bb0: 6765 2d33 2e6a 736f 6e27 2920 6173 2066  ge-3.json') as f
-00014bc0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00014bd0: 2020 206d 6f63 6b2e 6765 7428 6627 7b62     mock.get(f'{b
-00014be0: 6173 657d 3f70 6167 653d 3127 2c20 7374  ase}?page=1', st
-00014bf0: 6174 7573 5f63 6f64 653d 3230 302c 2074  atus_code=200, t
-00014c00: 6578 743d 6668 2e72 6561 6428 2929 0a20  ext=fh.read()). 
-00014c10: 2020 2020 2020 2020 2020 2023 2072 6563             # rec
-00014c20: 6f72 6473 2066 6f72 2069 646e 6120 7a6f  ords for idna zo
-00014c30: 6e65 2069 7320 696e 2070 6167 6520 330a  ne is in page 3.
-00014c40: 2020 2020 2020 2020 2020 2020 6261 7365              base
-00014c50: 203d 2066 277b 6261 7365 7d2f 7b69 646e   = f'{base}/{idn
-00014c60: 615f 7a6f 6e65 5f69 647d 270a 2020 2020  a_zone_id}'.    
-00014c70: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-00014c80: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00014c90: 2020 2027 7465 7374 732f 6669 7874 7572     'tests/fixtur
-00014ca0: 6573 2f63 6c6f 7564 666c 6172 652d 646e  es/cloudflare-dn
-00014cb0: 735f 7265 636f 7264 732d 7061 6765 2d33  s_records-page-3
-00014cc0: 2e6a 736f 6e27 0a20 2020 2020 2020 2020  .json'.         
-00014cd0: 2020 2029 2061 7320 6668 3a0a 2020 2020     ) as fh:.    
-00014ce0: 2020 2020 2020 2020 2020 2020 6d6f 636b              mock
-00014cf0: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-00014d00: 2020 2020 2020 2020 2020 6627 7b62 6173            f'{bas
-00014d10: 657d 2f64 6e73 5f72 6563 6f72 6473 3f70  e}/dns_records?p
-00014d20: 6167 653d 3127 2c0a 2020 2020 2020 2020  age=1',.        
-00014d30: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-00014d40: 7573 5f63 6f64 653d 3230 302c 0a20 2020  us_code=200,.   
-00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d60: 2074 6578 743d 6668 2e72 6561 6428 292c   text=fh.read(),
-00014d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014d80: 2029 0a20 2020 2020 2020 2020 2020 2023   ).            #
-00014d90: 206c 6f61 6420 7061 6765 2072 756c 6573   load page rules
-00014da0: 2066 6f72 2069 646e 6120 7a6f 6e65 0a20   for idna zone. 
-00014db0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00014dc0: 6f70 656e 2827 7465 7374 732f 6669 7874  open('tests/fixt
-00014dd0: 7572 6573 2f63 6c6f 7564 666c 6172 652d  ures/cloudflare-
-00014de0: 7061 6765 7275 6c65 732e 6a73 6f6e 2729  pagerules.json')
-00014df0: 2061 7320 6668 3a0a 2020 2020 2020 2020   as fh:.        
-00014e00: 2020 2020 2020 2020 6d6f 636b 2e67 6574          mock.get
-00014e10: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00014e20: 2020 2020 2020 6627 7b62 6173 657d 2f70        f'{base}/p
-00014e30: 6167 6572 756c 6573 3f73 7461 7475 733d  agerules?status=
-00014e40: 6163 7469 7665 272c 0a20 2020 2020 2020  active',.       
-00014e50: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-00014e60: 7475 735f 636f 6465 3d32 3030 2c0a 2020  tus_code=200,.  
-00014e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e80: 2020 7465 7874 3d66 682e 7265 6164 2829    text=fh.read()
-00014e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014ea0: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00014eb0: 2023 206e 6f74 6963 6520 7468 6520 6920   # notice the i 
-00014ec0: 6973 2061 2075 7466 2d38 2063 6861 7261  is a utf-8 chara
-00014ed0: 6374 6572 2077 6869 6368 2062 6563 6f6d  cter which becom
-00014ee0: 6573 2060 786e 2d2d 6774 6875 622d 7a73  es `xn--gthub-zs
-00014ef0: 612e 636f 6d2e 600a 2020 2020 2020 2020  a.com.`.        
-00014f00: 2020 2020 7a6f 6e65 203d 205a 6f6e 6528      zone = Zone(
-00014f10: 2767 c3ad 7468 7562 2e63 6f6d 2e27 2c20  'g..thub.com.', 
-00014f20: 5b5d 290a 2020 2020 2020 2020 2020 2020  []).            
-00014f30: 7072 6f76 6964 6572 2e70 6f70 756c 6174  provider.populat
-00014f40: 6528 7a6f 6e65 290a 2020 2020 2020 2020  e(zone).        
-00014f50: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
-00014f60: 2838 2c20 6c65 6e28 7a6f 6e65 2e72 6563  (8, len(zone.rec
-00014f70: 6f72 6473 2929 0a20 2020 2020 2020 2073  ords)).        s
-00014f80: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
-00014f90: 7a6f 6e65 2e6e 616d 652c 2069 646e 615f  zone.name, idna_
-00014fa0: 656e 636f 6465 2827 67c3 ad74 6875 622e  encode('g..thub.
-00014fb0: 636f 6d2e 2729 290a 0a20 2020 2064 6566  com.'))..    def
-00014fc0: 2074 6573 745f 6163 636f 756e 745f 6964   test_account_id
-00014fd0: 5f66 696c 7465 7228 7365 6c66 293a 0a20  _filter(self):. 
-00014fe0: 2020 2020 2020 2070 726f 7669 6465 7220         provider 
-00014ff0: 3d20 436c 6f75 6466 6c61 7265 5072 6f76  = CloudflareProv
-00015000: 6964 6572 280a 2020 2020 2020 2020 2020  ider(.          
-00015010: 2020 2774 6573 7427 2c0a 2020 2020 2020    'test',.      
-00015020: 2020 2020 2020 2765 6d61 696c 272c 0a20        'email',. 
-00015030: 2020 2020 2020 2020 2020 2027 746f 6b65             'toke
-00015040: 6e27 2c0a 2020 2020 2020 2020 2020 2020  n',.            
-00015050: 6163 636f 756e 745f 6964 3d27 3333 3432  account_id='3342
-00015060: 3334 3234 3334 3233 6161 6162 6233 3334  34243423aaabb334
-00015070: 3334 3261 6161 3334 3334 3333 272c 0a20  342aaa343433',. 
-00015080: 2020 2020 2020 2020 2020 2073 7472 6963             stric
-00015090: 745f 7375 7070 6f72 7473 3d46 616c 7365  t_supports=False
-000150a0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-000150b0: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
-000150c0: 6571 7565 7374 203d 204d 6f63 6b28 7374  equest = Mock(st
-000150d0: 6174 7573 5f63 6f64 653d 3230 3029 0a20  atus_code=200). 
-000150e0: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
-000150f0: 5f72 6571 7565 7374 2e73 6964 655f 6566  _request.side_ef
-00015100: 6665 6374 203d 205b 0a20 2020 2020 2020  fect = [.       
-00015110: 2020 2020 2073 656c 662e 656d 7074 792c       self.empty,
-00015120: 0a20 2020 2020 2020 2020 2020 204e 6f6e  .            Non
-00015130: 652c 0a20 2020 2020 2020 2020 2020 204e  e,.            N
-00015140: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00015150: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
-00015160: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
-00015170: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
-00015180: 2020 205d 0a0a 2020 2020 2020 2020 7072     ]..        pr
-00015190: 6f76 6964 6572 2e70 6c61 6e28 7365 6c66  ovider.plan(self
-000151a0: 2e65 7870 6563 7465 6429 0a20 2020 2020  .expected).     
-000151b0: 2020 2070 726f 7669 6465 722e 5f72 6571     provider._req
-000151c0: 7565 7374 2e61 7373 6572 745f 6361 6c6c  uest.assert_call
-000151d0: 6564 5f77 6974 6828 0a20 2020 2020 2020  ed_with(.       
-000151e0: 2020 2020 2027 4745 5427 2c0a 2020 2020       'GET',.    
-000151f0: 2020 2020 2020 2020 272f 7a6f 6e65 7327          '/zones'
-00015200: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-00015210: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
-00015220: 2020 2020 2020 2027 7061 6765 273a 2031         'page': 1
-00015230: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015240: 2020 2770 6572 5f70 6167 6527 3a20 3530    'per_page': 50
-00015250: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015260: 2020 2761 6363 6f75 6e74 2e69 6427 3a20    'account.id': 
-00015270: 2733 3334 3233 3432 3433 3432 3361 6161  '334234243423aaa
-00015280: 6262 3333 3433 3432 6161 6133 3433 3433  bb334342aaa34343
-00015290: 3327 2c0a 2020 2020 2020 2020 2020 2020  3',.            
-000152a0: 7d2c 0a20 2020 2020 2020 2029 0a0a 2020  },.        )..  
-000152b0: 2020 6465 6620 7465 7374 5f6c 6973 745f    def test_list_
-000152c0: 7a6f 6e65 7328 7365 6c66 293a 0a20 2020  zones(self):.   
-000152d0: 2020 2020 2070 726f 7669 6465 7220 3d20       provider = 
-000152e0: 436c 6f75 6466 6c61 7265 5072 6f76 6964  CloudflareProvid
-000152f0: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00015300: 2774 6573 7427 2c0a 2020 2020 2020 2020  'test',.        
-00015310: 2020 2020 2765 6d61 696c 272c 0a20 2020      'email',.   
-00015320: 2020 2020 2020 2020 2027 746f 6b65 6e27           'token'
-00015330: 2c0a 2020 2020 2020 2020 2020 2020 6163  ,.            ac
-00015340: 636f 756e 745f 6964 3d27 3333 3432 3334  count_id='334234
-00015350: 3234 3334 3233 6161 6162 6233 3334 3334  243423aaabb33434
-00015360: 3261 6161 3334 3334 3333 272c 0a20 2020  2aaa343433',.   
-00015370: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00015380: 2320 6578 6973 7469 6e67 207a 6f6e 6520  # existing zone 
-00015390: 7769 7468 2064 6174 610a 2020 2020 2020  with data.      
-000153a0: 2020 7769 7468 2072 6571 7565 7374 735f    with requests_
-000153b0: 6d6f 636b 2829 2061 7320 6d6f 636b 3a0a  mock() as mock:.
-000153c0: 2020 2020 2020 2020 2020 2020 6261 7365              base
-000153d0: 203d 2027 6874 7470 733a 2f2f 6170 692e   = 'https://api.
-000153e0: 636c 6f75 6466 6c61 7265 2e63 6f6d 2f63  cloudflare.com/c
-000153f0: 6c69 656e 742f 7634 2f7a 6f6e 6573 270a  lient/v4/zones'.
-00015400: 0a20 2020 2020 2020 2020 2020 2023 207a  .            # z
-00015410: 6f6e 6573 0a20 2020 2020 2020 2020 2020  ones.           
-00015420: 2077 6974 6820 6f70 656e 2827 7465 7374   with open('test
-00015430: 732f 6669 7874 7572 6573 2f63 6c6f 7564  s/fixtures/cloud
-00015440: 666c 6172 652d 7a6f 6e65 732d 7061 6765  flare-zones-page
-00015450: 2d31 2e6a 736f 6e27 2920 6173 2066 683a  -1.json') as fh:
-00015460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015470: 206d 6f63 6b2e 6765 7428 6627 7b62 6173   mock.get(f'{bas
-00015480: 657d 3f70 6167 653d 3127 2c20 7374 6174  e}?page=1', stat
-00015490: 7573 5f63 6f64 653d 3230 302c 2074 6578  us_code=200, tex
-000154a0: 743d 6668 2e72 6561 6428 2929 0a20 2020  t=fh.read()).   
-000154b0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
-000154c0: 656e 2827 7465 7374 732f 6669 7874 7572  en('tests/fixtur
-000154d0: 6573 2f63 6c6f 7564 666c 6172 652d 7a6f  es/cloudflare-zo
-000154e0: 6e65 732d 7061 6765 2d32 2e6a 736f 6e27  nes-page-2.json'
-000154f0: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
-00015500: 2020 2020 2020 2020 206d 6f63 6b2e 6765           mock.ge
-00015510: 7428 6627 7b62 6173 657d 3f70 6167 653d  t(f'{base}?page=
-00015520: 3227 2c20 7374 6174 7573 5f63 6f64 653d  2', status_code=
-00015530: 3230 302c 2074 6578 743d 6668 2e72 6561  200, text=fh.rea
-00015540: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
-00015550: 2077 6974 6820 6f70 656e 2827 7465 7374   with open('test
-00015560: 732f 6669 7874 7572 6573 2f63 6c6f 7564  s/fixtures/cloud
-00015570: 666c 6172 652d 7a6f 6e65 732d 7061 6765  flare-zones-page
-00015580: 2d33 2e6a 736f 6e27 2920 6173 2066 683a  -3.json') as fh:
-00015590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000155a0: 206d 6f63 6b2e 6765 7428 6627 7b62 6173   mock.get(f'{bas
-000155b0: 657d 3f70 6167 653d 3327 2c20 7374 6174  e}?page=3', stat
-000155c0: 7573 5f63 6f64 653d 3230 302c 2074 6578  us_code=200, tex
-000155d0: 743d 6668 2e72 6561 6428 2929 0a20 2020  t=fh.read()).   
-000155e0: 2020 2020 2020 2020 206d 6f63 6b2e 6765           mock.ge
-000155f0: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00015600: 2020 2066 277b 6261 7365 7d3f 7061 6765     f'{base}?page
-00015610: 3d34 272c 0a20 2020 2020 2020 2020 2020  =4',.           
-00015620: 2020 2020 2073 7461 7475 735f 636f 6465       status_code
-00015630: 3d32 3030 2c0a 2020 2020 2020 2020 2020  =200,.          
-00015640: 2020 2020 2020 6a73 6f6e 3d7b 2772 6573        json={'res
-00015650: 756c 7427 3a20 5b5d 2c20 2772 6573 756c  ult': [], 'resul
-00015660: 745f 696e 666f 273a 207b 2763 6f75 6e74  t_info': {'count
-00015670: 273a 2030 2c20 2770 6572 5f70 6167 6527  ': 0, 'per_page'
-00015680: 3a20 307d 7d2c 0a20 2020 2020 2020 2020  : 0}},.         
-00015690: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-000156a0: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
-000156b0: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
-000156c0: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-000156d0: 2020 2020 2020 2020 2020 2767 6974 6875            'githu
-000156e0: 622e 636f 6d2e 272c 0a20 2020 2020 2020  b.com.',.       
-000156f0: 2020 2020 2020 2020 2020 2020 2027 6769               'gi
-00015700: 7468 7562 2e69 6f2e 272c 0a20 2020 2020  thub.io.',.     
-00015710: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00015720: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
-00015730: 742e 636f 6d2e 272c 0a20 2020 2020 2020  t.com.',.       
-00015740: 2020 2020 2020 2020 2020 2020 2027 756e               'un
-00015750: 6974 2e74 6573 7473 2e27 2c0a 2020 2020  it.tests.',.    
-00015760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015770: 2778 6e2d 2d67 7468 7562 2d7a 7361 2e63  'xn--gthub-zsa.c
-00015780: 6f6d 2e27 2c0a 2020 2020 2020 2020 2020  om.',.          
-00015790: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-000157a0: 2020 2020 2020 2020 2070 726f 7669 6465           provide
-000157b0: 722e 6c69 7374 5f7a 6f6e 6573 2829 2c0a  r.list_zones(),.
-000157c0: 2020 2020 2020 2020 2020 2020 290a                   ).
+00013180: 742e 7265 7365 745f 6d6f 636b 2829 0a20  t.reset_mock(). 
+00013190: 2020 2020 2020 2070 726f 7669 6465 722e         provider.
+000131a0: 5f72 6571 7565 7374 2e73 6964 655f 6566  _request.side_ef
+000131b0: 6665 6374 203d 205b 436c 6f75 6466 6c61  fect = [Cloudfla
+000131c0: 7265 5261 7465 4c69 6d69 7445 7272 6f72  reRateLimitError
+000131d0: 2827 7b7d 2729 2c20 7265 7375 6c74 5d0a  ('{}'), result].
+000131e0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000131f0: 6572 7445 7175 616c 285b 5d2c 2070 726f  ertEqual([], pro
+00013200: 7669 6465 722e 7a6f 6e65 5f72 6563 6f72  vider.zone_recor
+00013210: 6473 287a 6f6e 6529 290a 2020 2020 2020  ds(zone)).      
+00013220: 2020 7072 6f76 6964 6572 2e5f 7265 7175    provider._requ
+00013230: 6573 742e 6173 7365 7274 5f68 6173 5f63  est.assert_has_c
+00013240: 616c 6c73 280a 2020 2020 2020 2020 2020  alls(.          
+00013250: 2020 5b63 616c 6c28 2747 4554 272c 2027    [call('GET', '
+00013260: 2f7a 6f6e 6573 272c 2070 6172 616d 733d  /zones', params=
+00013270: 7b27 7061 6765 273a 2031 2c20 2770 6572  {'page': 1, 'per
+00013280: 5f70 6167 6527 3a20 3530 7d29 5d0a 2020  _page': 50})].  
+00013290: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+000132a0: 2023 2054 776f 2072 6574 7269 6573 2072   # Two retries r
+000132b0: 6571 7569 7265 640a 2020 2020 2020 2020  equired.        
+000132c0: 7072 6f76 6964 6572 2e5f 7a6f 6e65 7320  provider._zones 
+000132d0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2070  = None.        p
+000132e0: 726f 7669 6465 722e 5f72 6571 7565 7374  rovider._request
+000132f0: 2e72 6573 6574 5f6d 6f63 6b28 290a 2020  .reset_mock().  
+00013300: 2020 2020 2020 7072 6f76 6964 6572 2e5f        provider._
+00013310: 7265 7175 6573 742e 7369 6465 5f65 6666  request.side_eff
+00013320: 6563 7420 3d20 5b0a 2020 2020 2020 2020  ect = [.        
+00013330: 2020 2020 436c 6f75 6466 6c61 7265 5261      CloudflareRa
+00013340: 7465 4c69 6d69 7445 7272 6f72 2827 7b7d  teLimitError('{}
+00013350: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00013360: 436c 6f75 6466 6c61 7265 5261 7465 4c69  CloudflareRateLi
+00013370: 6d69 7445 7272 6f72 2827 7b7d 2729 2c0a  mitError('{}'),.
+00013380: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00013390: 6c74 2c0a 2020 2020 2020 2020 5d0a 2020  lt,.        ].  
+000133a0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000133b0: 7445 7175 616c 285b 5d2c 2070 726f 7669  tEqual([], provi
+000133c0: 6465 722e 7a6f 6e65 5f72 6563 6f72 6473  der.zone_records
+000133d0: 287a 6f6e 6529 290a 2020 2020 2020 2020  (zone)).        
+000133e0: 7072 6f76 6964 6572 2e5f 7265 7175 6573  provider._reques
+000133f0: 742e 6173 7365 7274 5f68 6173 5f63 616c  t.assert_has_cal
+00013400: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
+00013410: 5b63 616c 6c28 2747 4554 272c 2027 2f7a  [call('GET', '/z
+00013420: 6f6e 6573 272c 2070 6172 616d 733d 7b27  ones', params={'
+00013430: 7061 6765 273a 2031 2c20 2770 6572 5f70  page': 1, 'per_p
+00013440: 6167 6527 3a20 3530 7d29 5d0a 2020 2020  age': 50})].    
+00013450: 2020 2020 290a 0a20 2020 2020 2020 2023      )..        #
+00013460: 2023 2045 7868 6175 7374 206f 7572 2072   # Exhaust our r
+00013470: 6574 7269 6573 0a20 2020 2020 2020 2070  etries.        p
+00013480: 726f 7669 6465 722e 5f7a 6f6e 6573 203d  rovider._zones =
+00013490: 204e 6f6e 650a 2020 2020 2020 2020 7072   None.        pr
+000134a0: 6f76 6964 6572 2e5f 7265 7175 6573 742e  ovider._request.
+000134b0: 7265 7365 745f 6d6f 636b 2829 0a20 2020  reset_mock().   
+000134c0: 2020 2020 2070 726f 7669 6465 722e 5f72       provider._r
+000134d0: 6571 7565 7374 2e73 6964 655f 6566 6665  equest.side_effe
+000134e0: 6374 203d 205b 0a20 2020 2020 2020 2020  ct = [.         
+000134f0: 2020 2043 6c6f 7564 666c 6172 6552 6174     CloudflareRat
+00013500: 654c 696d 6974 4572 726f 7228 7b22 6572  eLimitError({"er
+00013510: 726f 7273 223a 205b 7b22 6d65 7373 6167  rors": [{"messag
+00013520: 6522 3a20 2266 6972 7374 227d 5d7d 292c  e": "first"}]}),
+00013530: 0a20 2020 2020 2020 2020 2020 2043 6c6f  .            Clo
+00013540: 7564 666c 6172 6552 6174 654c 696d 6974  udflareRateLimit
+00013550: 4572 726f 7228 7b22 6572 726f 7273 223a  Error({"errors":
+00013560: 205b 7b22 6d65 7373 6167 6522 3a20 2262   [{"message": "b
+00013570: 6f6f 227d 5d7d 292c 0a20 2020 2020 2020  oo"}]}),.       
+00013580: 2020 2020 2043 6c6f 7564 666c 6172 6552       CloudflareR
+00013590: 6174 654c 696d 6974 4572 726f 7228 7b22  ateLimitError({"
+000135a0: 6572 726f 7273 223a 205b 7b22 6d65 7373  errors": [{"mess
+000135b0: 6167 6522 3a20 2262 6f6f 227d 5d7d 292c  age": "boo"}]}),
+000135c0: 0a20 2020 2020 2020 2020 2020 2043 6c6f  .            Clo
+000135d0: 7564 666c 6172 6552 6174 654c 696d 6974  udflareRateLimit
+000135e0: 4572 726f 7228 7b22 6572 726f 7273 223a  Error({"errors":
+000135f0: 205b 7b22 6d65 7373 6167 6522 3a20 2262   [{"message": "b
+00013600: 6f6f 227d 5d7d 292c 0a20 2020 2020 2020  oo"}]}),.       
+00013610: 2020 2020 2043 6c6f 7564 666c 6172 6552       CloudflareR
+00013620: 6174 654c 696d 6974 4572 726f 7228 7b22  ateLimitError({"
+00013630: 6572 726f 7273 223a 205b 7b22 6d65 7373  errors": [{"mess
+00013640: 6167 6522 3a20 226c 6173 7422 7d5d 7d29  age": "last"}]})
+00013650: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00013660: 2020 2020 7769 7468 2073 656c 662e 6173      with self.as
+00013670: 7365 7274 5261 6973 6573 2843 6c6f 7564  sertRaises(Cloud
+00013680: 666c 6172 6552 6174 654c 696d 6974 4572  flareRateLimitEr
+00013690: 726f 7229 2061 7320 6374 783a 0a20 2020  ror) as ctx:.   
+000136a0: 2020 2020 2020 2020 2070 726f 7669 6465           provide
+000136b0: 722e 7a6f 6e65 5f72 6563 6f72 6473 287a  r.zone_records(z
+000136c0: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+000136d0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+000136e0: 6c28 276c 6173 7427 2c20 7374 7228 6374  l('last', str(ct
+000136f0: 782e 6578 6365 7074 696f 6e29 290a 0a20  x.exception)).. 
+00013700: 2020 2064 6566 2074 6573 745f 7474 6c5f     def test_ttl_
+00013710: 6d61 7070 696e 6728 7365 6c66 293a 0a20  mapping(self):. 
+00013720: 2020 2020 2020 2070 726f 7669 6465 7220         provider 
+00013730: 3d20 436c 6f75 6466 6c61 7265 5072 6f76  = CloudflareProv
+00013740: 6964 6572 2827 7465 7374 272c 2027 656d  ider('test', 'em
+00013750: 6169 6c27 2c20 2774 6f6b 656e 2729 0a0a  ail', 'token')..
+00013760: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00013770: 6572 7445 7175 616c 2831 3230 2c20 7072  ertEqual(120, pr
+00013780: 6f76 6964 6572 2e5f 7474 6c5f 6461 7461  ovider._ttl_data
+00013790: 2831 3230 2929 0a20 2020 2020 2020 2073  (120)).        s
+000137a0: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+000137b0: 3132 302c 2070 726f 7669 6465 722e 5f74  120, provider._t
+000137c0: 746c 5f64 6174 6128 3132 3029 290a 2020  tl_data(120)).  
+000137d0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000137e0: 7445 7175 616c 2833 3630 302c 2070 726f  tEqual(3600, pro
+000137f0: 7669 6465 722e 5f74 746c 5f64 6174 6128  vider._ttl_data(
+00013800: 3336 3030 2929 0a20 2020 2020 2020 2073  3600)).        s
+00013810: 656c 662e 6173 7365 7274 4571 7561 6c28  elf.assertEqual(
+00013820: 3330 302c 2070 726f 7669 6465 722e 5f74  300, provider._t
+00013830: 746c 5f64 6174 6128 3129 290a 0a20 2020  tl_data(1))..   
+00013840: 2064 6566 2074 6573 745f 746c 7361 2873   def test_tlsa(s
+00013850: 656c 6629 3a0a 2020 2020 2020 2020 7072  elf):.        pr
+00013860: 6f76 6964 6572 203d 2043 6c6f 7564 666c  ovider = Cloudfl
+00013870: 6172 6550 726f 7669 6465 7228 2774 6573  areProvider('tes
+00013880: 7427 2c20 2765 6d61 696c 272c 2027 746f  t', 'email', 'to
+00013890: 6b65 6e27 290a 0a20 2020 2020 2020 2063  ken')..        c
+000138a0: 665f 6461 7461 203d 207b 0a20 2020 2020  f_data = {.     
+000138b0: 2020 2020 2020 2027 636f 6d6d 656e 7427         'comment'
+000138c0: 3a20 4e6f 6e65 2c0a 2020 2020 2020 2020  : None,.        
+000138d0: 2020 2020 2763 6f6e 7465 6e74 273a 2027      'content': '
+000138e0: 3120 3120 3120 6161 3432 3432 3432 3432  1 1 1 aa42424242
+000138f0: 3432 3432 3432 3432 3432 3432 3432 3432  4242424242424242
+00013900: 3432 3432 3432 272c 0a20 2020 2020 2020  424242',.       
+00013910: 2020 2020 2027 6372 6561 7465 645f 6f6e       'created_on
+00013920: 273a 2027 3230 3232 2d31 322d 3233 5430  ': '2022-12-23T0
+00013930: 313a 3537 3a31 342e 3536 3739 3835 5a27  1:57:14.567985Z'
+00013940: 2c0a 2020 2020 2020 2020 2020 2020 2764  ,.            'd
+00013950: 6174 6127 3a20 7b0a 2020 2020 2020 2020  ata': {.        
+00013960: 2020 2020 2020 2020 2763 6572 7469 6669          'certifi
+00013970: 6361 7465 273a 2027 6161 3432 3432 3432  cate': 'aa424242
+00013980: 3432 3432 3432 3432 3432 3432 3432 3432  4242424242424242
+00013990: 3432 3432 3432 3432 272c 0a20 2020 2020  42424242',.     
+000139a0: 2020 2020 2020 2020 2020 2027 6d61 7463             'matc
+000139b0: 6869 6e67 5f74 7970 6527 3a20 312c 0a20  hing_type': 1,. 
+000139c0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000139d0: 7365 6c65 6374 6f72 273a 2031 2c0a 2020  selector': 1,.  
+000139e0: 2020 2020 2020 2020 2020 2020 2020 2775                'u
+000139f0: 7361 6765 273a 2031 2c0a 2020 2020 2020  sage': 1,.      
+00013a00: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00013a10: 2020 2020 2027 6964 273a 2027 3432 3939       'id': '4299
+00013a20: 3861 6336 3966 6334 6139 3563 6335 6338  8ac69fc4a95cc5c8
+00013a30: 3562 6539 6265 6632 6466 6265 272c 0a20  5be9bef2dfbe',. 
+00013a40: 2020 2020 2020 2020 2020 2027 6c6f 636b             'lock
+00013a50: 6564 273a 2046 616c 7365 2c0a 2020 2020  ed': False,.    
+00013a60: 2020 2020 2020 2020 276d 6574 6127 3a20          'meta': 
+00013a70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00013a80: 2020 2761 7574 6f5f 6164 6465 6427 3a20    'auto_added': 
+00013a90: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00013aa0: 2020 2020 2020 2027 6d61 6e61 6765 645f         'managed_
+00013ab0: 6279 5f61 7070 7327 3a20 4661 6c73 652c  by_apps': False,
+00013ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ad0: 2027 6d61 6e61 6765 645f 6279 5f61 7267   'managed_by_arg
+00013ae0: 6f5f 7475 6e6e 656c 273a 2046 616c 7365  o_tunnel': False
+00013af0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00013b00: 2020 2773 6f75 7263 6527 3a20 2770 7269    'source': 'pri
+00013b10: 6d61 7279 272c 0a20 2020 2020 2020 2020  mary',.         
+00013b20: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00013b30: 2020 276d 6f64 6966 6965 645f 6f6e 273a    'modified_on':
+00013b40: 2027 3230 3232 2d31 322d 3233 5430 313a   '2022-12-23T01:
+00013b50: 3537 3a31 342e 3536 3739 3835 5a27 2c0a  57:14.567985Z',.
+00013b60: 2020 2020 2020 2020 2020 2020 276e 616d              'nam
+00013b70: 6527 3a20 2774 6c73 612e 756e 6974 2e74  e': 'tlsa.unit.t
+00013b80: 6573 7473 272c 0a20 2020 2020 2020 2020  ests',.         
+00013b90: 2020 2027 7072 6f78 6961 626c 6527 3a20     'proxiable': 
+00013ba0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
+00013bb0: 2020 2027 7072 6f78 6965 6427 3a20 4661     'proxied': Fa
+00013bc0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00013bd0: 2027 7461 6773 273a 205b 5d2c 0a20 2020   'tags': [],.   
+00013be0: 2020 2020 2020 2020 2027 7474 6c27 3a20           'ttl': 
+00013bf0: 312c 0a20 2020 2020 2020 2020 2020 2027  1,.            '
+00013c00: 7479 7065 273a 2027 544c 5341 272c 0a20  type': 'TLSA',. 
+00013c10: 2020 2020 2020 2020 2020 2027 7a6f 6e65             'zone
+00013c20: 5f69 6427 3a20 2763 6166 3931 3139 3763  _id': 'caf91197c
+00013c30: 6337 3933 3063 3333 6237 3431 6563 3330  c7930c33b741ec30
+00013c40: 6432 3964 3930 3927 2c0a 2020 2020 2020  d29d909',.      
+00013c50: 2020 2020 2020 277a 6f6e 655f 6e61 6d65        'zone_name
+00013c60: 273a 2027 756e 6974 2e74 6573 7473 272c  ': 'unit.tests',
+00013c70: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00013c80: 2020 2064 6174 6120 3d20 7072 6f76 6964     data = provid
+00013c90: 6572 2e5f 6461 7461 5f66 6f72 5f54 4c53  er._data_for_TLS
+00013ca0: 4128 2754 4c53 4127 2c20 5b63 665f 6461  A('TLSA', [cf_da
+00013cb0: 7461 5d29 0a20 2020 2020 2020 2073 656c  ta]).        sel
+00013cc0: 662e 6173 7365 7274 4571 7561 6c28 0a20  f.assertEqual(. 
+00013cd0: 2020 2020 2020 2020 2020 207b 0a20 2020             {.   
+00013ce0: 2020 2020 2020 2020 2020 2020 2027 7474               'tt
+00013cf0: 6c27 3a20 3330 302c 0a20 2020 2020 2020  l': 300,.       
+00013d00: 2020 2020 2020 2020 2027 7479 7065 273a           'type':
+00013d10: 2027 544c 5341 272c 0a20 2020 2020 2020   'TLSA',.       
+00013d20: 2020 2020 2020 2020 2027 7661 6c75 6573           'values
+00013d30: 273a 205b 0a20 2020 2020 2020 2020 2020  ': [.           
+00013d40: 2020 2020 2020 2020 207b 0a20 2020 2020           {.     
+00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d60: 2020 2027 6365 7274 6966 6963 6174 655f     'certificate_
+00013d70: 6173 736f 6369 6174 696f 6e5f 6461 7461  association_data
+00013d80: 273a 2027 6161 3432 3432 3432 3432 3432  ': 'aa4242424242
+00013d90: 3432 3432 3432 3432 3432 3432 3432 3432  4242424242424242
+00013da0: 3432 3432 272c 0a20 2020 2020 2020 2020  4242',.         
+00013db0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00013dc0: 6365 7274 6966 6963 6174 655f 7573 6167  certificate_usag
+00013dd0: 6527 3a20 312c 0a20 2020 2020 2020 2020  e': 1,.         
+00013de0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00013df0: 6d61 7463 6869 6e67 5f74 7970 6527 3a20  matching_type': 
+00013e00: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+00013e10: 2020 2020 2020 2020 2020 2027 7365 6c65             'sele
+00013e20: 6374 6f72 273a 2031 2c0a 2020 2020 2020  ctor': 1,.      
+00013e30: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e50: 5d2c 0a20 2020 2020 2020 2020 2020 207d  ],.            }
+00013e60: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
+00013e70: 7461 2c0a 2020 2020 2020 2020 290a 0a20  ta,.        ).. 
+00013e80: 2020 2020 2020 207a 6f6e 6520 3d20 5a6f         zone = Zo
+00013e90: 6e65 2827 756e 6974 2e74 6573 7473 2e27  ne('unit.tests.'
+00013ea0: 2c20 5b5d 290a 2020 2020 2020 2020 7265  , []).        re
+00013eb0: 636f 7264 203d 2052 6563 6f72 642e 6e65  cord = Record.ne
+00013ec0: 7728 7a6f 6e65 2c20 2774 6c73 6127 2c20  w(zone, 'tlsa', 
+00013ed0: 6461 7461 290a 2020 2020 2020 2020 636f  data).        co
+00013ee0: 6e74 656e 7473 203d 206c 6973 7428 7072  ntents = list(pr
+00013ef0: 6f76 6964 6572 2e5f 636f 6e74 656e 7473  ovider._contents
+00013f00: 5f66 6f72 5f54 4c53 4128 7265 636f 7264  _for_TLSA(record
+00013f10: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00013f20: 6173 7365 7274 4571 7561 6c28 5b7b 2764  assertEqual([{'d
+00013f30: 6174 6127 3a20 6366 5f64 6174 615b 2764  ata': cf_data['d
+00013f40: 6174 6127 5d7d 5d2c 2063 6f6e 7465 6e74  ata']}], content
+00013f50: 7329 0a0a 2020 2020 2020 2020 6b65 7920  s)..        key 
+00013f60: 3d20 7072 6f76 6964 6572 2e5f 6765 6e5f  = provider._gen_
+00013f70: 6b65 7928 6366 5f64 6174 6129 0a20 2020  key(cf_data).   
+00013f80: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00013f90: 4571 7561 6c28 2731 2031 2031 2061 6134  Equal('1 1 1 aa4
+00013fa0: 3234 3234 3234 3234 3234 3234 3234 3234  2424242424242424
+00013fb0: 3234 3234 3234 3234 3234 3234 3227 2c20  2424242424242', 
+00013fc0: 6b65 7929 0a0a 2020 2020 6465 6620 7465  key)..    def te
+00013fd0: 7374 5f6e 6f5f 7370 665f 6372 6561 7465  st_no_spf_create
+00013fe0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00013ff0: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
+00014000: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
+00014010: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
+00014020: 746f 6b65 6e27 2c20 7265 7472 795f 7065  token', retry_pe
+00014030: 7269 6f64 3d30 290a 0a20 2020 2020 2020  riod=0)..       
+00014040: 207a 6f6e 6520 3d20 5a6f 6e65 2827 756e   zone = Zone('un
+00014050: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
+00014060: 2020 2020 2020 2020 6131 203d 2052 6563          a1 = Rec
+00014070: 6f72 642e 6e65 7728 0a20 2020 2020 2020  ord.new(.       
+00014080: 2020 2020 207a 6f6e 652c 2027 6127 2c20       zone, 'a', 
+00014090: 7b27 7479 7065 273a 2027 4127 2c20 2774  {'type': 'A', 't
+000140a0: 746c 273a 2034 3230 2c20 2776 616c 7565  tl': 420, 'value
+000140b0: 273a 2027 312e 322e 332e 3427 7d0a 2020  ': '1.2.3.4'}.  
+000140c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000140d0: 6132 203d 2061 312e 636f 7079 2829 0a20  a2 = a1.copy(). 
+000140e0: 2020 2020 2020 2061 322e 7474 6c20 2b3d         a2.ttl +=
+000140f0: 2031 0a20 2020 2020 2020 2073 7066 3120   1.        spf1 
+00014100: 3d20 5265 636f 7264 2e6e 6577 280a 2020  = Record.new(.  
+00014110: 2020 2020 2020 2020 2020 7a6f 6e65 2c20            zone, 
+00014120: 2773 7066 272c 207b 2774 7970 6527 3a20  'spf', {'type': 
+00014130: 2753 5046 272c 2027 7474 6c27 3a20 3433  'SPF', 'ttl': 43
+00014140: 302c 2027 7661 6c75 6527 3a20 2762 6c61  0, 'value': 'bla
+00014150: 6862 6c61 6827 7d0a 2020 2020 2020 2020  hblah'}.        
+00014160: 290a 2020 2020 2020 2020 7370 6632 203d  ).        spf2 =
+00014170: 2073 7066 312e 636f 7079 2829 0a20 2020   spf1.copy().   
+00014180: 2020 2020 2073 7066 322e 7474 6c20 2b3d       spf2.ttl +=
+00014190: 2031 0a0a 2020 2020 2020 2020 2320 4120   1..        # A 
+000141a0: 6973 2061 6c77 6179 7320 696e 636c 7564  is always includ
+000141b0: 6564 0a20 2020 2020 2020 2073 656c 662e  ed.        self.
+000141c0: 6173 7365 7274 5472 7565 2870 726f 7669  assertTrue(provi
+000141d0: 6465 722e 5f69 6e63 6c75 6465 5f63 6861  der._include_cha
+000141e0: 6e67 6528 4372 6561 7465 2861 3129 2929  nge(Create(a1)))
+000141f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00014200: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
+00014210: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
+00014220: 6528 5570 6461 7465 2861 312c 2061 3229  e(Update(a1, a2)
+00014230: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00014240: 6173 7365 7274 5472 7565 2870 726f 7669  assertTrue(provi
+00014250: 6465 722e 5f69 6e63 6c75 6465 5f63 6861  der._include_cha
+00014260: 6e67 6528 4465 6c65 7465 2861 3129 2929  nge(Delete(a1)))
+00014270: 0a0a 2020 2020 2020 2020 2320 5350 4620  ..        # SPF 
+00014280: 6361 6e27 7420 6265 2063 7265 6174 6564  can't be created
+00014290: 2c20 7570 6461 7465 7320 616e 6420 6465  , updates and de
+000142a0: 6c65 7465 7320 6172 6520 4f4b 0a20 2020  letes are OK.   
+000142b0: 2020 2020 2077 6974 6820 7365 6c66 2e61       with self.a
+000142c0: 7373 6572 7452 6169 7365 7328 5375 7070  ssertRaises(Supp
+000142d0: 6f72 7473 4578 6365 7074 696f 6e29 2061  ortsException) a
+000142e0: 7320 6374 783a 0a20 2020 2020 2020 2020  s ctx:.         
+000142f0: 2020 2070 726f 7669 6465 722e 5f69 6e63     provider._inc
+00014300: 6c75 6465 5f63 6861 6e67 6528 4372 6561  lude_change(Crea
+00014310: 7465 2873 7066 3129 290a 2020 2020 2020  te(spf1)).      
+00014320: 2020 7365 6c66 2e61 7373 6572 7445 7175    self.assertEqu
+00014330: 616c 280a 2020 2020 2020 2020 2020 2020  al(.            
+00014340: 2774 6573 743a 2063 7265 6174 696e 6720  'test: creating 
+00014350: 6e65 7720 5350 4620 7265 636f 7264 7320  new SPF records 
+00014360: 6e6f 7420 7375 7070 6f72 7465 642c 2075  not supported, u
+00014370: 7365 2054 5854 2069 6e73 7465 6164 272c  se TXT instead',
+00014380: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00014390: 2863 7478 2e65 7863 6570 7469 6f6e 292c  (ctx.exception),
+000143a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000143b0: 2020 2073 656c 662e 6173 7365 7274 5472     self.assertTr
+000143c0: 7565 2870 726f 7669 6465 722e 5f69 6e63  ue(provider._inc
+000143d0: 6c75 6465 5f63 6861 6e67 6528 5570 6461  lude_change(Upda
+000143e0: 7465 2873 7066 312c 2073 7066 3229 2929  te(spf1, spf2)))
+000143f0: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00014400: 7365 7274 5472 7565 2870 726f 7669 6465  sertTrue(provide
+00014410: 722e 5f69 6e63 6c75 6465 5f63 6861 6e67  r._include_chang
+00014420: 6528 4465 6c65 7465 2873 7066 3129 2929  e(Delete(spf1)))
+00014430: 0a0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
+00014440: 7368 6670 2873 656c 6629 3a0a 2020 2020  shfp(self):.    
+00014450: 2020 2020 7365 6c66 2e6d 6178 4469 6666      self.maxDiff
+00014460: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00014470: 7072 6f76 6964 6572 203d 2043 6c6f 7564  provider = Cloud
+00014480: 666c 6172 6550 726f 7669 6465 7228 2774  flareProvider('t
+00014490: 6573 7427 2c20 2765 6d61 696c 272c 2027  est', 'email', '
+000144a0: 746f 6b65 6e27 290a 0a20 2020 2020 2020  token')..       
+000144b0: 2063 665f 6461 7461 203d 207b 0a20 2020   cf_data = {.   
+000144c0: 2020 2020 2020 2020 2027 636f 6d6d 656e           'commen
+000144d0: 7427 3a20 4e6f 6e65 2c0a 2020 2020 2020  t': None,.      
+000144e0: 2020 2020 2020 2763 6f6e 7465 6e74 273a        'content':
+000144f0: 2027 3120 3220 3835 3962 6536 6564 3034   '1 2 859be6ed04
+00014500: 3634 3364 6234 3131 6630 3637 6236 6331  643db411f067b6c1
+00014510: 6461 3164 3735 6665 3038 6236 3732 272c  da1d75fe08b672',
+00014520: 0a20 2020 2020 2020 2020 2020 2027 6372  .            'cr
+00014530: 6561 7465 645f 6f6e 273a 2027 3230 3233  eated_on': '2023
+00014540: 2d30 332d 3032 5430 313a 3032 3a34 342e  -03-02T01:02:44.
+00014550: 3536 3739 3835 5a27 2c0a 2020 2020 2020  567985Z',.      
+00014560: 2020 2020 2020 2764 6174 6127 3a20 7b0a        'data': {.
+00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014580: 2761 6c67 6f72 6974 686d 273a 2031 2c0a  'algorithm': 1,.
+00014590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145a0: 2774 7970 6527 3a20 322c 0a20 2020 2020  'type': 2,.     
+000145b0: 2020 2020 2020 2020 2020 2027 6669 6e67             'fing
+000145c0: 6572 7072 696e 7427 3a20 2738 3539 6265  erprint': '859be
+000145d0: 3665 6430 3436 3433 6462 3431 3166 3036  6ed04643db411f06
+000145e0: 3762 3663 3164 6131 6437 3566 6530 3862  7b6c1da1d75fe08b
+000145f0: 3637 3227 2c0a 2020 2020 2020 2020 2020  672',.          
+00014600: 2020 7d2c 0a20 2020 2020 2020 2020 2020    },.           
+00014610: 2027 6964 273a 2027 6767 6f7a 7274 6e7a   'id': 'ggozrtnz
+00014620: 6231 316e 7272 3971 7334 6b6f 3679 336a  b11nrr9qs4ko6y3j
+00014630: 3139 716b 6568 7578 3927 2c0a 2020 2020  19qkehux9',.    
+00014640: 2020 2020 2020 2020 276c 6f63 6b65 6427          'locked'
+00014650: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00014660: 2020 2020 2027 6d65 7461 273a 207b 0a20       'meta': {. 
+00014670: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014680: 6175 746f 5f61 6464 6564 273a 2046 616c  auto_added': Fal
+00014690: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+000146a0: 2020 2020 276d 616e 6167 6564 5f62 795f      'managed_by_
+000146b0: 6170 7073 273a 2046 616c 7365 2c0a 2020  apps': False,.  
+000146c0: 2020 2020 2020 2020 2020 2020 2020 276d                'm
+000146d0: 616e 6167 6564 5f62 795f 6172 676f 5f74  anaged_by_argo_t
+000146e0: 756e 6e65 6c27 3a20 4661 6c73 652c 0a20  unnel': False,. 
+000146f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014700: 736f 7572 6365 273a 2027 7072 696d 6172  source': 'primar
+00014710: 7927 2c0a 2020 2020 2020 2020 2020 2020  y',.            
+00014720: 7d2c 0a20 2020 2020 2020 2020 2020 2027  },.            '
+00014730: 6d6f 6469 6669 6564 5f6f 6e27 3a20 2732  modified_on': '2
+00014740: 3032 332d 3033 2d30 3254 3031 3a30 323a  023-03-02T01:02:
+00014750: 3434 2e35 3637 3938 355a 272c 0a20 2020  44.567985Z',.   
+00014760: 2020 2020 2020 2020 2027 6e61 6d65 273a           'name':
+00014770: 2027 6e61 7074 722e 756e 6974 2e74 6573   'naptr.unit.tes
+00014780: 7473 272c 0a20 2020 2020 2020 2020 2020  ts',.           
+00014790: 2027 7072 6f78 6961 626c 6527 3a20 4661   'proxiable': Fa
+000147a0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+000147b0: 2027 7072 6f78 6965 6427 3a20 4661 6c73   'proxied': Fals
+000147c0: 652c 0a20 2020 2020 2020 2020 2020 2027  e,.            '
+000147d0: 7461 6773 273a 205b 5d2c 0a20 2020 2020  tags': [],.     
+000147e0: 2020 2020 2020 2027 7474 6c27 3a20 3330         'ttl': 30
+000147f0: 302c 0a20 2020 2020 2020 2020 2020 2027  0,.            '
+00014800: 7479 7065 273a 2027 5353 4846 5027 2c0a  type': 'SSHFP',.
+00014810: 2020 2020 2020 2020 2020 2020 277a 6f6e              'zon
+00014820: 655f 6964 273a 2027 6666 3132 6162 3334  e_id': 'ff12ab34
+00014830: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
+00014840: 3232 3939 3736 3530 272c 0a20 2020 2020  22997650',.     
+00014850: 2020 2020 2020 2027 7a6f 6e65 5f6e 616d         'zone_nam
+00014860: 6527 3a20 2775 6e69 742e 7465 7374 7327  e': 'unit.tests'
+00014870: 2c0a 2020 2020 2020 2020 7d0a 2020 2020  ,.        }.    
+00014880: 2020 2020 6461 7461 203d 2070 726f 7669      data = provi
+00014890: 6465 722e 5f64 6174 615f 666f 725f 5353  der._data_for_SS
+000148a0: 4846 5028 2753 5348 4650 272c 205b 6366  HFP('SSHFP', [cf
+000148b0: 5f64 6174 615d 290a 2020 2020 2020 2020  _data]).        
+000148c0: 7365 6c66 2e61 7373 6572 7445 7175 616c  self.assertEqual
+000148d0: 280a 2020 2020 2020 2020 2020 2020 7b0a  (.            {.
+000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148f0: 2774 746c 273a 2033 3030 2c0a 2020 2020  'ttl': 300,.    
+00014900: 2020 2020 2020 2020 2020 2020 2774 7970              'typ
+00014910: 6527 3a20 2753 5348 4650 272c 0a20 2020  e': 'SSHFP',.   
+00014920: 2020 2020 2020 2020 2020 2020 2027 7661               'va
+00014930: 6c75 6573 273a 205b 0a20 2020 2020 2020  lues': [.       
+00014940: 2020 2020 2020 2020 2020 2020 207b 0a20               {. 
+00014950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014960: 2020 2020 2020 2027 616c 676f 7269 7468         'algorith
+00014970: 6d27 3a20 312c 0a20 2020 2020 2020 2020  m': 1,.         
+00014980: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014990: 6669 6e67 6572 7072 696e 745f 7479 7065  fingerprint_type
+000149a0: 273a 2032 2c0a 2020 2020 2020 2020 2020  ': 2,.          
+000149b0: 2020 2020 2020 2020 2020 2020 2020 2766                'f
+000149c0: 696e 6765 7270 7269 6e74 273a 2027 3835  ingerprint': '85
+000149d0: 3962 6536 6564 3034 3634 3364 6234 3131  9be6ed04643db411
+000149e0: 6630 3637 6236 6331 6461 3164 3735 6665  f067b6c1da1d75fe
+000149f0: 3038 6236 3732 272c 0a20 2020 2020 2020  08b672',.       
+00014a00: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00014a10: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00014a20: 2c0a 2020 2020 2020 2020 2020 2020 7d2c  ,.            },
+00014a30: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00014a40: 612c 0a20 2020 2020 2020 2029 0a0a 2020  a,.        )..  
+00014a50: 2020 2020 2020 7a6f 6e65 203d 205a 6f6e        zone = Zon
+00014a60: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
+00014a70: 205b 5d29 0a20 2020 2020 2020 2072 6563   []).        rec
+00014a80: 6f72 6420 3d20 5265 636f 7264 2e6e 6577  ord = Record.new
+00014a90: 287a 6f6e 652c 2027 7373 6866 7027 2c20  (zone, 'sshfp', 
+00014aa0: 6461 7461 290a 2020 2020 2020 2020 636f  data).        co
+00014ab0: 6e74 656e 7473 203d 206c 6973 7428 7072  ntents = list(pr
+00014ac0: 6f76 6964 6572 2e5f 636f 6e74 656e 7473  ovider._contents
+00014ad0: 5f66 6f72 5f53 5348 4650 2872 6563 6f72  _for_SSHFP(recor
+00014ae0: 6429 290a 2020 2020 2020 2020 7365 6c66  d)).        self
+00014af0: 2e61 7373 6572 7445 7175 616c 285b 7b27  .assertEqual([{'
+00014b00: 6461 7461 273a 2063 665f 6461 7461 5b27  data': cf_data['
+00014b10: 6461 7461 275d 7d5d 2c20 636f 6e74 656e  data']}], conten
+00014b20: 7473 290a 0a20 2020 2020 2020 206b 6579  ts)..        key
+00014b30: 203d 2070 726f 7669 6465 722e 5f67 656e   = provider._gen
+00014b40: 5f6b 6579 2863 665f 6461 7461 290a 2020  _key(cf_data).  
+00014b50: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+00014b60: 7445 7175 616c 2827 3120 3220 3835 3962  tEqual('1 2 859b
+00014b70: 6536 6564 3034 3634 3364 6234 3131 6630  e6ed04643db411f0
+00014b80: 3637 6236 6331 6461 3164 3735 6665 3038  67b6c1da1d75fe08
+00014b90: 6236 3732 272c 206b 6579 290a 0a20 2020  b672', key)..   
+00014ba0: 2064 6566 2074 6573 745f 6964 6e61 5f64   def test_idna_d
+00014bb0: 6f6d 6169 6e28 7365 6c66 293a 0a20 2020  omain(self):.   
+00014bc0: 2020 2020 2073 656c 662e 6d61 7844 6966       self.maxDif
+00014bd0: 6620 3d20 4e6f 6e65 0a20 2020 2020 2020  f = None.       
+00014be0: 2070 726f 7669 6465 7220 3d20 436c 6f75   provider = Clou
+00014bf0: 6466 6c61 7265 5072 6f76 6964 6572 2827  dflareProvider('
+00014c00: 7465 7374 272c 2027 656d 6169 6c27 2c20  test', 'email', 
+00014c10: 2774 6f6b 656e 2729 0a20 2020 2020 2020  'token').       
+00014c20: 2023 2065 7869 7374 696e 6720 7a6f 6e65   # existing zone
+00014c30: 2077 6974 6820 6461 7461 0a20 2020 2020   with data.     
+00014c40: 2020 2077 6974 6820 7265 7175 6573 7473     with requests
+00014c50: 5f6d 6f63 6b28 2920 6173 206d 6f63 6b3a  _mock() as mock:
+00014c60: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+00014c70: 6520 3d20 2768 7474 7073 3a2f 2f61 7069  e = 'https://api
+00014c80: 2e63 6c6f 7564 666c 6172 652e 636f 6d2f  .cloudflare.com/
+00014c90: 636c 6965 6e74 2f76 342f 7a6f 6e65 7327  client/v4/zones'
+00014ca0: 0a20 2020 2020 2020 2020 2020 2069 646e  .            idn
+00014cb0: 615f 7a6f 6e65 5f69 6420 3d20 2732 3334  a_zone_id = '234
+00014cc0: 3233 3432 3433 3432 3361 6161 6262 3333  234243423aaabb33
+00014cd0: 3433 3432 6262 6233 3433 3433 3327 0a20  4342bbb343433'. 
+00014ce0: 2020 2020 2020 2020 2020 2023 207a 6f6e             # zon
+00014cf0: 6520 666f 7220 6964 6e61 207a 6f6e 6520  e for idna zone 
+00014d00: 6973 2069 6e20 7061 6765 2033 0a20 2020  is in page 3.   
+00014d10: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+00014d20: 656e 2827 7465 7374 732f 6669 7874 7572  en('tests/fixtur
+00014d30: 6573 2f63 6c6f 7564 666c 6172 652d 7a6f  es/cloudflare-zo
+00014d40: 6e65 732d 7061 6765 2d33 2e6a 736f 6e27  nes-page-3.json'
+00014d50: 2920 6173 2066 683a 0a20 2020 2020 2020  ) as fh:.       
+00014d60: 2020 2020 2020 2020 206d 6f63 6b2e 6765           mock.ge
+00014d70: 7428 6627 7b62 6173 657d 3f70 6167 653d  t(f'{base}?page=
+00014d80: 3127 2c20 7374 6174 7573 5f63 6f64 653d  1', status_code=
+00014d90: 3230 302c 2074 6578 743d 6668 2e72 6561  200, text=fh.rea
+00014da0: 6428 2929 0a20 2020 2020 2020 2020 2020  d()).           
+00014db0: 2023 2072 6563 6f72 6473 2066 6f72 2069   # records for i
+00014dc0: 646e 6120 7a6f 6e65 2069 7320 696e 2070  dna zone is in p
+00014dd0: 6167 6520 330a 2020 2020 2020 2020 2020  age 3.          
+00014de0: 2020 6261 7365 203d 2066 277b 6261 7365    base = f'{base
+00014df0: 7d2f 7b69 646e 615f 7a6f 6e65 5f69 647d  }/{idna_zone_id}
+00014e00: 270a 2020 2020 2020 2020 2020 2020 7769  '.            wi
+00014e10: 7468 206f 7065 6e28 0a20 2020 2020 2020  th open(.       
+00014e20: 2020 2020 2020 2020 2027 7465 7374 732f           'tests/
+00014e30: 6669 7874 7572 6573 2f63 6c6f 7564 666c  fixtures/cloudfl
+00014e40: 6172 652d 646e 735f 7265 636f 7264 732d  are-dns_records-
+00014e50: 7061 6765 2d33 2e6a 736f 6e27 0a20 2020  page-3.json'.   
+00014e60: 2020 2020 2020 2020 2029 2061 7320 6668           ) as fh
+00014e70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014e80: 2020 6d6f 636b 2e67 6574 280a 2020 2020    mock.get(.    
+00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ea0: 6627 7b62 6173 657d 2f64 6e73 5f72 6563  f'{base}/dns_rec
+00014eb0: 6f72 6473 3f70 6167 653d 3127 2c0a 2020  ords?page=1',.  
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ed0: 2020 7374 6174 7573 5f63 6f64 653d 3230    status_code=20
+00014ee0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+00014ef0: 2020 2020 2020 2074 6578 743d 6668 2e72         text=fh.r
+00014f00: 6561 6428 292c 0a20 2020 2020 2020 2020  ead(),.         
+00014f10: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00014f20: 2020 2020 2023 206c 6f61 6420 7061 6765       # load page
+00014f30: 2072 756c 6573 2066 6f72 2069 646e 6120   rules for idna 
+00014f40: 7a6f 6e65 0a20 2020 2020 2020 2020 2020  zone.           
+00014f50: 2077 6974 6820 6f70 656e 2827 7465 7374   with open('test
+00014f60: 732f 6669 7874 7572 6573 2f63 6c6f 7564  s/fixtures/cloud
+00014f70: 666c 6172 652d 7061 6765 7275 6c65 732e  flare-pagerules.
+00014f80: 6a73 6f6e 2729 2061 7320 6668 3a0a 2020  json') as fh:.  
+00014f90: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00014fa0: 636b 2e67 6574 280a 2020 2020 2020 2020  ck.get(.        
+00014fb0: 2020 2020 2020 2020 2020 2020 6627 7b62              f'{b
+00014fc0: 6173 657d 2f70 6167 6572 756c 6573 3f73  ase}/pagerules?s
+00014fd0: 7461 7475 733d 6163 7469 7665 272c 0a20  tatus=active',. 
+00014fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014ff0: 2020 2073 7461 7475 735f 636f 6465 3d32     status_code=2
+00015000: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+00015010: 2020 2020 2020 2020 7465 7874 3d66 682e          text=fh.
+00015020: 7265 6164 2829 2c0a 2020 2020 2020 2020  read(),.        
+00015030: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00015040: 2020 2020 2020 2023 206e 6f74 6963 6520         # notice 
+00015050: 7468 6520 6920 6973 2061 2075 7466 2d38  the i is a utf-8
+00015060: 2063 6861 7261 6374 6572 2077 6869 6368   character which
+00015070: 2062 6563 6f6d 6573 2060 786e 2d2d 6774   becomes `xn--gt
+00015080: 6875 622d 7a73 612e 636f 6d2e 600a 2020  hub-zsa.com.`.  
+00015090: 2020 2020 2020 2020 2020 7a6f 6e65 203d            zone =
+000150a0: 205a 6f6e 6528 2767 c3ad 7468 7562 2e63   Zone('g..thub.c
+000150b0: 6f6d 2e27 2c20 5b5d 290a 2020 2020 2020  om.', []).      
+000150c0: 2020 2020 2020 7072 6f76 6964 6572 2e70        provider.p
+000150d0: 6f70 756c 6174 6528 7a6f 6e65 290a 2020  opulate(zone).  
+000150e0: 2020 2020 2020 7365 6c66 2e61 7373 6572        self.asser
+000150f0: 7445 7175 616c 2838 2c20 6c65 6e28 7a6f  tEqual(8, len(zo
+00015100: 6e65 2e72 6563 6f72 6473 2929 0a20 2020  ne.records)).   
+00015110: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00015120: 4571 7561 6c28 7a6f 6e65 2e6e 616d 652c  Equal(zone.name,
+00015130: 2069 646e 615f 656e 636f 6465 2827 67c3   idna_encode('g.
+00015140: ad74 6875 622e 636f 6d2e 2729 290a 0a20  .thub.com.')).. 
+00015150: 2020 2064 6566 2074 6573 745f 6163 636f     def test_acco
+00015160: 756e 745f 6964 5f66 696c 7465 7228 7365  unt_id_filter(se
+00015170: 6c66 293a 0a20 2020 2020 2020 2070 726f  lf):.        pro
+00015180: 7669 6465 7220 3d20 436c 6f75 6466 6c61  vider = Cloudfla
+00015190: 7265 5072 6f76 6964 6572 280a 2020 2020  reProvider(.    
+000151a0: 2020 2020 2020 2020 2774 6573 7427 2c0a          'test',.
+000151b0: 2020 2020 2020 2020 2020 2020 2765 6d61              'ema
+000151c0: 696c 272c 0a20 2020 2020 2020 2020 2020  il',.           
+000151d0: 2027 746f 6b65 6e27 2c0a 2020 2020 2020   'token',.      
+000151e0: 2020 2020 2020 6163 636f 756e 745f 6964        account_id
+000151f0: 3d27 3333 3432 3334 3234 3334 3233 6161  ='334234243423aa
+00015200: 6162 6233 3334 3334 3261 6161 3334 3334  abb334342aaa3434
+00015210: 3333 272c 0a20 2020 2020 2020 2020 2020  33',.           
+00015220: 2073 7472 6963 745f 7375 7070 6f72 7473   strict_supports
+00015230: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
+00015240: 290a 0a20 2020 2020 2020 2070 726f 7669  )..        provi
+00015250: 6465 722e 5f72 6571 7565 7374 203d 204d  der._request = M
+00015260: 6f63 6b28 7374 6174 7573 5f63 6f64 653d  ock(status_code=
+00015270: 3230 3029 0a20 2020 2020 2020 2070 726f  200).        pro
+00015280: 7669 6465 722e 5f72 6571 7565 7374 2e73  vider._request.s
+00015290: 6964 655f 6566 6665 6374 203d 205b 0a20  ide_effect = [. 
+000152a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000152b0: 656d 7074 792c 0a20 2020 2020 2020 2020  empty,.         
+000152c0: 2020 204e 6f6e 652c 0a20 2020 2020 2020     None,.       
+000152d0: 2020 2020 204e 6f6e 652c 0a20 2020 2020       None,.     
+000152e0: 2020 2020 2020 204e 6f6e 652c 0a20 2020         None,.   
+000152f0: 2020 2020 2020 2020 204e 6f6e 652c 0a20           None,. 
+00015300: 2020 2020 2020 2020 2020 204e 6f6e 652c             None,
+00015310: 0a20 2020 2020 2020 205d 0a0a 2020 2020  .        ]..    
+00015320: 2020 2020 7072 6f76 6964 6572 2e70 6c61      provider.pla
+00015330: 6e28 7365 6c66 2e65 7870 6563 7465 6429  n(self.expected)
+00015340: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+00015350: 722e 5f72 6571 7565 7374 2e61 7373 6572  r._request.asser
+00015360: 745f 6361 6c6c 6564 5f77 6974 6828 0a20  t_called_with(. 
+00015370: 2020 2020 2020 2020 2020 2027 4745 5427             'GET'
+00015380: 2c0a 2020 2020 2020 2020 2020 2020 272f  ,.            '/
+00015390: 7a6f 6e65 7327 2c0a 2020 2020 2020 2020  zones',.        
+000153a0: 2020 2020 7061 7261 6d73 3d7b 0a20 2020      params={.   
+000153b0: 2020 2020 2020 2020 2020 2020 2027 7061               'pa
+000153c0: 6765 273a 2031 2c0a 2020 2020 2020 2020  ge': 1,.        
+000153d0: 2020 2020 2020 2020 2770 6572 5f70 6167          'per_pag
+000153e0: 6527 3a20 3530 2c0a 2020 2020 2020 2020  e': 50,.        
+000153f0: 2020 2020 2020 2020 2761 6363 6f75 6e74          'account
+00015400: 2e69 6427 3a20 2733 3334 3233 3432 3433  .id': '334234243
+00015410: 3432 3361 6161 6262 3333 3433 3432 6161  423aaabb334342aa
+00015420: 6133 3433 3433 3327 2c0a 2020 2020 2020  a343433',.      
+00015430: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00015440: 2029 0a0a 2020 2020 6465 6620 7465 7374   )..    def test
+00015450: 5f6c 6973 745f 7a6f 6e65 7328 7365 6c66  _list_zones(self
+00015460: 293a 0a20 2020 2020 2020 2070 726f 7669  ):.        provi
+00015470: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
+00015480: 5072 6f76 6964 6572 280a 2020 2020 2020  Provider(.      
+00015490: 2020 2020 2020 2774 6573 7427 2c0a 2020        'test',.  
+000154a0: 2020 2020 2020 2020 2020 2765 6d61 696c            'email
+000154b0: 272c 0a20 2020 2020 2020 2020 2020 2027  ',.            '
+000154c0: 746f 6b65 6e27 2c0a 2020 2020 2020 2020  token',.        
+000154d0: 2020 2020 6163 636f 756e 745f 6964 3d27      account_id='
+000154e0: 3333 3432 3334 3234 3334 3233 6161 6162  334234243423aaab
+000154f0: 6233 3334 3334 3261 6161 3334 3334 3333  b334342aaa343433
+00015500: 272c 0a20 2020 2020 2020 2029 0a0a 2020  ',.        )..  
+00015510: 2020 2020 2020 2320 6578 6973 7469 6e67        # existing
+00015520: 207a 6f6e 6520 7769 7468 2064 6174 610a   zone with data.
+00015530: 2020 2020 2020 2020 7769 7468 2072 6571          with req
+00015540: 7565 7374 735f 6d6f 636b 2829 2061 7320  uests_mock() as 
+00015550: 6d6f 636b 3a0a 2020 2020 2020 2020 2020  mock:.          
+00015560: 2020 6261 7365 203d 2027 6874 7470 733a    base = 'https:
+00015570: 2f2f 6170 692e 636c 6f75 6466 6c61 7265  //api.cloudflare
+00015580: 2e63 6f6d 2f63 6c69 656e 742f 7634 2f7a  .com/client/v4/z
+00015590: 6f6e 6573 270a 0a20 2020 2020 2020 2020  ones'..         
+000155a0: 2020 2023 207a 6f6e 6573 0a20 2020 2020     # zones.     
+000155b0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+000155c0: 2827 7465 7374 732f 6669 7874 7572 6573  ('tests/fixtures
+000155d0: 2f63 6c6f 7564 666c 6172 652d 7a6f 6e65  /cloudflare-zone
+000155e0: 732d 7061 6765 2d31 2e6a 736f 6e27 2920  s-page-1.json') 
+000155f0: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
+00015600: 2020 2020 2020 206d 6f63 6b2e 6765 7428         mock.get(
+00015610: 6627 7b62 6173 657d 3f70 6167 653d 3127  f'{base}?page=1'
+00015620: 2c20 7374 6174 7573 5f63 6f64 653d 3230  , status_code=20
+00015630: 302c 2074 6578 743d 6668 2e72 6561 6428  0, text=fh.read(
+00015640: 2929 0a20 2020 2020 2020 2020 2020 2077  )).            w
+00015650: 6974 6820 6f70 656e 2827 7465 7374 732f  ith open('tests/
+00015660: 6669 7874 7572 6573 2f63 6c6f 7564 666c  fixtures/cloudfl
+00015670: 6172 652d 7a6f 6e65 732d 7061 6765 2d32  are-zones-page-2
+00015680: 2e6a 736f 6e27 2920 6173 2066 683a 0a20  .json') as fh:. 
+00015690: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000156a0: 6f63 6b2e 6765 7428 6627 7b62 6173 657d  ock.get(f'{base}
+000156b0: 3f70 6167 653d 3227 2c20 7374 6174 7573  ?page=2', status
+000156c0: 5f63 6f64 653d 3230 302c 2074 6578 743d  _code=200, text=
+000156d0: 6668 2e72 6561 6428 2929 0a20 2020 2020  fh.read()).     
+000156e0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+000156f0: 2827 7465 7374 732f 6669 7874 7572 6573  ('tests/fixtures
+00015700: 2f63 6c6f 7564 666c 6172 652d 7a6f 6e65  /cloudflare-zone
+00015710: 732d 7061 6765 2d33 2e6a 736f 6e27 2920  s-page-3.json') 
+00015720: 6173 2066 683a 0a20 2020 2020 2020 2020  as fh:.         
+00015730: 2020 2020 2020 206d 6f63 6b2e 6765 7428         mock.get(
+00015740: 6627 7b62 6173 657d 3f70 6167 653d 3327  f'{base}?page=3'
+00015750: 2c20 7374 6174 7573 5f63 6f64 653d 3230  , status_code=20
+00015760: 302c 2074 6578 743d 6668 2e72 6561 6428  0, text=fh.read(
+00015770: 2929 0a20 2020 2020 2020 2020 2020 206d  )).            m
+00015780: 6f63 6b2e 6765 7428 0a20 2020 2020 2020  ock.get(.       
+00015790: 2020 2020 2020 2020 2066 277b 6261 7365           f'{base
+000157a0: 7d3f 7061 6765 3d34 272c 0a20 2020 2020  }?page=4',.     
+000157b0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+000157c0: 735f 636f 6465 3d32 3030 2c0a 2020 2020  s_code=200,.    
+000157d0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
+000157e0: 3d7b 2772 6573 756c 7427 3a20 5b5d 2c20  ={'result': [], 
+000157f0: 2772 6573 756c 745f 696e 666f 273a 207b  'result_info': {
+00015800: 2763 6f75 6e74 273a 2030 2c20 2770 6572  'count': 0, 'per
+00015810: 5f70 6167 6527 3a20 307d 7d2c 0a20 2020  _page': 0}},.   
+00015820: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00015830: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+00015840: 6572 7445 7175 616c 280a 2020 2020 2020  ertEqual(.      
+00015850: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00015860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015870: 2767 6974 6875 622e 636f 6d2e 272c 0a20  'github.com.',. 
+00015880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015890: 2020 2027 6769 7468 7562 2e69 6f2e 272c     'github.io.',
+000158a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000158b0: 2020 2020 2027 6769 7468 7562 7573 6572       'githubuser
+000158c0: 636f 6e74 656e 742e 636f 6d2e 272c 0a20  content.com.',. 
+000158d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000158e0: 2020 2027 756e 6974 2e74 6573 7473 2e27     'unit.tests.'
+000158f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00015900: 2020 2020 2020 2778 6e2d 2d67 7468 7562        'xn--gthub
+00015910: 2d7a 7361 2e63 6f6d 2e27 2c0a 2020 2020  -zsa.com.',.    
+00015920: 2020 2020 2020 2020 2020 2020 5d2c 0a20              ],. 
+00015930: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00015940: 726f 7669 6465 722e 6c69 7374 5f7a 6f6e  rovider.list_zon
+00015950: 6573 2829 2c0a 2020 2020 2020 2020 2020  es(),.          
+00015960: 2020 290a 0a20 2020 2064 6566 2074 6573    )..    def tes
+00015970: 745f 7265 636f 7264 5f63 6f6e 7461 696e  t_record_contain
+00015980: 735f 6e6f 5f74 6167 7328 7365 6c66 293a  s_no_tags(self):
+00015990: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+000159a0: 7220 3d20 436c 6f75 6466 6c61 7265 5072  r = CloudflarePr
+000159b0: 6f76 6964 6572 2827 7465 7374 272c 2027  ovider('test', '
+000159c0: 656d 6169 6c27 2c20 2774 6f6b 656e 2729  email', 'token')
+000159d0: 0a20 2020 2020 2020 207a 6f6e 6520 3d20  .        zone = 
+000159e0: 5a6f 6e65 2827 756e 6974 2e74 6573 7473  Zone('unit.tests
+000159f0: 2e27 2c20 5b5d 290a 2020 2020 2020 2020  .', []).        
+00015a00: 7265 636f 7264 203d 2073 6574 5f72 6563  record = set_rec
+00015a10: 6f72 645f 7461 6773 280a 2020 2020 2020  ord_tags(.      
+00015a20: 2020 2020 2020 5265 636f 7264 2e6e 6577        Record.new
+00015a30: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00015a40: 2020 7a6f 6e65 2c20 2761 272c 207b 2774    zone, 'a', {'t
+00015a50: 746c 273a 2033 3030 2c20 2774 7970 6527  tl': 300, 'type'
+00015a60: 3a20 2741 272c 2027 7661 6c75 6527 3a20  : 'A', 'value': 
+00015a70: 2731 2e32 2e33 2e34 277d 0a20 2020 2020  '1.2.3.4'}.     
+00015a80: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00015a90: 2020 2020 2020 5b5d 2c0a 2020 2020 2020        [],.      
+00015aa0: 2020 290a 0a20 2020 2020 2020 2064 6174    )..        dat
+00015ab0: 6120 3d20 6e65 7874 2870 726f 7669 6465  a = next(provide
+00015ac0: 722e 5f67 656e 5f64 6174 6128 7265 636f  r._gen_data(reco
+00015ad0: 7264 2929 0a0a 2020 2020 2020 2020 7365  rd))..        se
+00015ae0: 6c66 2e61 7373 6572 7445 7175 616c 2827  lf.assertEqual('
+00015af0: 7461 6773 2720 696e 2064 6174 612c 2046  tags' in data, F
+00015b00: 616c 7365 290a 0a20 2020 2064 6566 2074  alse)..    def t
+00015b10: 6573 745f 7265 636f 7264 5f63 6f6e 7461  est_record_conta
+00015b20: 696e 735f 7461 6773 2873 656c 6629 3a0a  ins_tags(self):.
+00015b30: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00015b40: 203d 2043 6c6f 7564 666c 6172 6550 726f   = CloudflarePro
+00015b50: 7669 6465 7228 2774 6573 7427 2c20 2765  vider('test', 'e
+00015b60: 6d61 696c 272c 2027 746f 6b65 6e27 290a  mail', 'token').
+00015b70: 2020 2020 2020 2020 7a6f 6e65 203d 205a          zone = Z
+00015b80: 6f6e 6528 2775 6e69 742e 7465 7374 732e  one('unit.tests.
+00015b90: 272c 205b 5d29 0a20 2020 2020 2020 2072  ', []).        r
+00015ba0: 6563 6f72 6420 3d20 7365 745f 7265 636f  ecord = set_reco
+00015bb0: 7264 5f74 6167 7328 0a20 2020 2020 2020  rd_tags(.       
+00015bc0: 2020 2020 2052 6563 6f72 642e 6e65 7728       Record.new(
+00015bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015be0: 207a 6f6e 652c 2027 6127 2c20 7b27 7474   zone, 'a', {'tt
+00015bf0: 6c27 3a20 3330 302c 2027 7479 7065 273a  l': 300, 'type':
+00015c00: 2027 4127 2c20 2776 616c 7565 273a 2027   'A', 'value': '
+00015c10: 312e 322e 332e 3427 7d0a 2020 2020 2020  1.2.3.4'}.      
+00015c20: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00015c30: 2020 2020 205b 2774 6573 7469 6e67 3a61       ['testing:a
+00015c40: 6263 272c 2027 6162 633a 7465 7374 696e  bc', 'abc:testin
+00015c50: 6727 5d2c 0a20 2020 2020 2020 2029 0a0a  g'],.        )..
+00015c60: 2020 2020 2020 2020 6461 7461 203d 206e          data = n
+00015c70: 6578 7428 7072 6f76 6964 6572 2e5f 6765  ext(provider._ge
+00015c80: 6e5f 6461 7461 2872 6563 6f72 6429 290a  n_data(record)).
+00015c90: 0a20 2020 2020 2020 2073 656c 662e 6173  .        self.as
+00015ca0: 7365 7274 436f 756e 7445 7175 616c 2864  sertCountEqual(d
+00015cb0: 6174 615b 2774 6167 7327 5d2c 205b 2774  ata['tags'], ['t
+00015cc0: 6573 7469 6e67 3a61 6263 272c 2027 6162  esting:abc', 'ab
+00015cd0: 633a 7465 7374 696e 6727 5d29 0a0a 2020  c:testing'])..  
+00015ce0: 2020 6465 6620 7465 7374 5f61 6464 5f74    def test_add_t
+00015cf0: 6167 7328 7365 6c66 293a 0a20 2020 2020  ags(self):.     
+00015d00: 2020 2070 726f 7669 6465 7220 3d20 436c     provider = Cl
+00015d10: 6f75 6466 6c61 7265 5072 6f76 6964 6572  oudflareProvider
+00015d20: 2827 7465 7374 272c 2027 656d 6169 6c27  ('test', 'email'
+00015d30: 2c20 2774 6f6b 656e 2729 0a20 2020 2020  , 'token').     
+00015d40: 2020 2070 726f 7669 6465 722e 7a6f 6e65     provider.zone
+00015d50: 5f72 6563 6f72 6473 203d 204d 6f63 6b28  _records = Mock(
+00015d60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00015d70: 7572 6e5f 7661 6c75 653d 5b0a 2020 2020  urn_value=[.    
+00015d80: 2020 2020 2020 2020 2020 2020 7b0a 2020              {.  
+00015d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015da0: 2020 2269 6422 3a20 2264 6435 3330 6131    "id": "dd530a1
+00015db0: 6338 3339 6436 3734 6334 3337 3134 3464  c839d674c437144d
+00015dc0: 3263 3265 6132 3836 3122 2c0a 2020 2020  2c2ea2861",.    
+00015dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015de0: 2274 7970 6522 3a20 2243 4e41 4d45 222c  "type": "CNAME",
+00015df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e00: 2020 2020 2022 6e61 6d65 223a 2022 612e       "name": "a.
+00015e10: 756e 6974 2e74 6573 7473 222c 0a20 2020  unit.tests",.   
+00015e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e30: 2022 636f 6e74 656e 7422 3a20 2277 7777   "content": "www
+00015e40: 2e75 6e69 742e 7465 7374 7322 2c0a 2020  .unit.tests",.  
+00015e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e60: 2020 2274 6167 7322 3a20 5b5d 2c0a 2020    "tags": [],.  
+00015e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e80: 2020 2274 746c 223a 2033 3030 2c0a 2020    "ttl": 300,.  
+00015e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ea0: 2020 226c 6f63 6b65 6422 3a20 4661 6c73    "locked": Fals
+00015eb0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00015ec0: 2020 2020 2020 2022 7a6f 6e65 5f69 6422         "zone_id"
+00015ed0: 3a20 2266 6631 3261 6233 3463 6435 3631  : "ff12ab34cd561
+00015ee0: 3133 3334 3432 3261 6233 3332 3239 3937  1334422ab3322997
+00015ef0: 3635 3022 2c0a 2020 2020 2020 2020 2020  650",.          
+00015f00: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
+00015f10: 6e61 6d65 223a 2022 756e 6974 2e74 6573  name": "unit.tes
+00015f20: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
+00015f30: 2020 2020 2020 2020 2022 6d6f 6469 6669           "modifi
+00015f40: 6564 5f6f 6e22 3a20 2232 3031 372d 3033  ed_on": "2017-03
+00015f50: 2d31 3154 3138 3a30 313a 3433 2e34 3230  -11T18:01:43.420
+00015f60: 3638 395a 222c 0a20 2020 2020 2020 2020  689Z",.         
+00015f70: 2020 2020 2020 2020 2020 2022 6372 6561             "crea
+00015f80: 7465 645f 6f6e 223a 2022 3230 3137 2d30  ted_on": "2017-0
+00015f90: 332d 3131 5431 383a 3031 3a34 332e 3432  3-11T18:01:43.42
+00015fa0: 3036 3839 5a22 2c0a 2020 2020 2020 2020  0689Z",.        
+00015fb0: 2020 2020 2020 2020 2020 2020 226d 6574              "met
+00015fc0: 6122 3a20 7b22 6175 746f 5f61 6464 6564  a": {"auto_added
+00015fd0: 223a 2046 616c 7365 7d2c 0a20 2020 2020  ": False},.     
+00015fe0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00015ff0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+00016000: 2020 2029 0a20 2020 2020 2020 2065 7869     ).        exi
+00016010: 7374 696e 6720 3d20 5a6f 6e65 2827 756e  sting = Zone('un
+00016020: 6974 2e74 6573 7473 2e27 2c20 5b5d 290a  it.tests.', []).
+00016030: 2020 2020 2020 2020 7072 6f76 6964 6572          provider
+00016040: 2e70 6f70 756c 6174 6528 6578 6973 7469  .populate(existi
+00016050: 6e67 290a 2020 2020 2020 2020 7072 6f76  ng).        prov
+00016060: 6964 6572 2e7a 6f6e 655f 7265 636f 7264  ider.zone_record
+00016070: 7320 3d20 4d6f 636b 280a 2020 2020 2020  s = Mock(.      
+00016080: 2020 2020 2020 7265 7475 726e 5f76 616c        return_val
+00016090: 7565 3d5b 0a20 2020 2020 2020 2020 2020  ue=[.           
+000160a0: 2020 2020 207b 0a20 2020 2020 2020 2020       {.         
+000160b0: 2020 2020 2020 2020 2020 2022 6964 223a             "id":
+000160c0: 2022 6464 3533 3061 3163 3833 3964 3637   "dd530a1c839d67
+000160d0: 3463 3433 3731 3434 6432 6332 6561 3238  4c437144d2c2ea28
+000160e0: 3631 222c 0a20 2020 2020 2020 2020 2020  61",.           
+000160f0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00016100: 2022 434e 414d 4522 2c0a 2020 2020 2020   "CNAME",.      
+00016110: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00016120: 616d 6522 3a20 2261 2e75 6e69 742e 7465  ame": "a.unit.te
+00016130: 7374 7322 2c0a 2020 2020 2020 2020 2020  sts",.          
+00016140: 2020 2020 2020 2020 2020 2263 6f6e 7465            "conte
+00016150: 6e74 223a 2022 7777 772e 756e 6974 2e74  nt": "www.unit.t
+00016160: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+00016170: 2020 2020 2020 2020 2020 2022 7461 6773             "tags
+00016180: 223a 205b 2274 6573 7469 6e67 3a61 6263  ": ["testing:abc
+00016190: 222c 2022 6162 633a 7465 7374 696e 6722  ", "abc:testing"
+000161a0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000161b0: 2020 2020 2020 2022 7474 6c22 3a20 3330         "ttl": 30
+000161c0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+000161d0: 2020 2020 2020 2022 6c6f 636b 6564 223a         "locked":
+000161e0: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+000161f0: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+00016200: 655f 6964 223a 2022 6666 3132 6162 3334  e_id": "ff12ab34
+00016210: 6364 3536 3131 3333 3434 3232 6162 3333  cd5611334422ab33
+00016220: 3232 3939 3736 3530 222c 0a20 2020 2020  22997650",.     
+00016230: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00016240: 7a6f 6e65 5f6e 616d 6522 3a20 2275 6e69  zone_name": "uni
+00016250: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+00016260: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00016270: 6f64 6966 6965 645f 6f6e 223a 2022 3230  odified_on": "20
+00016280: 3137 2d30 332d 3131 5431 383a 3031 3a34  17-03-11T18:01:4
+00016290: 332e 3432 3036 3839 5a22 2c0a 2020 2020  3.420689Z",.    
+000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162b0: 2263 7265 6174 6564 5f6f 6e22 3a20 2232  "created_on": "2
+000162c0: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
+000162d0: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
+000162e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162f0: 2022 6d65 7461 223a 207b 2261 7574 6f5f   "meta": {"auto_
+00016300: 6164 6465 6422 3a20 4661 6c73 657d 2c0a  added": False},.
+00016310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016320: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
+00016330: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00016340: 2020 6465 7369 7265 6420 3d20 5a6f 6e65    desired = Zone
+00016350: 2827 756e 6974 2e74 6573 7473 2e27 2c20  ('unit.tests.', 
+00016360: 5b5d 290a 2020 2020 2020 2020 7072 6f76  []).        prov
+00016370: 6964 6572 2e70 6f70 756c 6174 6528 6465  ider.populate(de
+00016380: 7369 7265 6429 0a20 2020 2020 2020 2063  sired).        c
+00016390: 6861 6e67 6573 203d 2065 7869 7374 696e  hanges = existin
+000163a0: 672e 6368 616e 6765 7328 6465 7369 7265  g.changes(desire
+000163b0: 642c 2070 726f 7669 6465 7229 0a0a 2020  d, provider)..  
+000163c0: 2020 2020 2020 6578 7472 615f 6368 616e        extra_chan
+000163d0: 6765 7320 3d20 7072 6f76 6964 6572 2e5f  ges = provider._
+000163e0: 6578 7472 615f 6368 616e 6765 7328 6578  extra_changes(ex
+000163f0: 6973 7469 6e67 2c20 6465 7369 7265 642c  isting, desired,
+00016400: 2063 6861 6e67 6573 290a 0a20 2020 2020   changes)..     
+00016410: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00016420: 7561 6c28 312c 206c 656e 2865 7874 7261  ual(1, len(extra
+00016430: 5f63 6861 6e67 6573 2929 0a20 2020 2020  _changes)).     
+00016440: 2020 2073 656c 662e 6173 7365 7274 4571     self.assertEq
+00016450: 7561 6c28 0a20 2020 2020 2020 2020 2020  ual(.           
+00016460: 2065 7874 7261 5f63 6861 6e67 6573 5b30   extra_changes[0
+00016470: 5d0a 2020 2020 2020 2020 2020 2020 2e65  ].            .e
+00016480: 7869 7374 696e 672e 5f6f 6374 6f64 6e73  xisting._octodns
+00016490: 2e67 6574 2827 636c 6f75 6466 6c61 7265  .get('cloudflare
+000164a0: 272c 207b 7d29 0a20 2020 2020 2020 2020  ', {}).         
+000164b0: 2020 202e 6765 7428 2774 6167 7327 2c20     .get('tags', 
+000164c0: 5b5d 292c 0a20 2020 2020 2020 2020 2020  []),.           
+000164d0: 205b 5d2c 0a20 2020 2020 2020 2029 0a20   [],.        ). 
+000164e0: 2020 2020 2020 2073 656c 662e 6173 7365         self.asse
+000164f0: 7274 4571 7561 6c28 0a20 2020 2020 2020  rtEqual(.       
+00016500: 2020 2020 2065 7874 7261 5f63 6861 6e67       extra_chang
+00016510: 6573 5b30 5d2e 6e65 772e 5f6f 6374 6f64  es[0].new._octod
+00016520: 6e73 5b27 636c 6f75 6466 6c61 7265 275d  ns['cloudflare']
+00016530: 5b27 7461 6773 275d 2c0a 2020 2020 2020  ['tags'],.      
+00016540: 2020 2020 2020 5b27 7465 7374 696e 673a        ['testing:
+00016550: 6162 6327 2c20 2761 6263 3a74 6573 7469  abc', 'abc:testi
+00016560: 6e67 275d 2c0a 2020 2020 2020 2020 290a  ng'],.        ).
+00016570: 0a20 2020 2064 6566 2074 6573 745f 7570  .    def test_up
+00016580: 6461 7465 5f74 6167 7328 7365 6c66 293a  date_tags(self):
+00016590: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+000165a0: 7220 3d20 436c 6f75 6466 6c61 7265 5072  r = CloudflarePr
+000165b0: 6f76 6964 6572 2827 7465 7374 272c 2027  ovider('test', '
+000165c0: 656d 6169 6c27 2c20 2774 6f6b 656e 2729  email', 'token')
+000165d0: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+000165e0: 722e 7a6f 6e65 5f72 6563 6f72 6473 203d  r.zone_records =
+000165f0: 204d 6f63 6b28 0a20 2020 2020 2020 2020   Mock(.         
+00016600: 2020 2072 6574 7572 6e5f 7661 6c75 653d     return_value=
+00016610: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00016620: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00016630: 2020 2020 2020 2020 2269 6422 3a20 2232          "id": "2
+00016640: 6233 3135 3634 6534 3266 6430 3935 6439  b31564e42fd095d9
+00016650: 6664 6437 6162 6166 3266 6338 3666 3822  fdd7abaf2fc86f8"
+00016660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00016670: 2020 2020 2020 2274 7970 6522 3a20 2243        "type": "C
+00016680: 4e41 4d45 222c 0a20 2020 2020 2020 2020  NAME",.         
+00016690: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+000166a0: 223a 2022 612e 756e 6974 2e74 6573 7473  ": "a.unit.tests
+000166b0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000166c0: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
+000166d0: 3a20 2277 7777 2e75 6e69 742e 7465 7374  : "www.unit.test
+000166e0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+000166f0: 2020 2020 2020 2020 2274 6167 7322 3a20          "tags": 
+00016700: 5b22 7465 7374 696e 673a 6162 6322 2c20  ["testing:abc", 
+00016710: 2261 6263 3a74 6573 7469 6e67 225d 2c0a  "abc:testing"],.
+00016720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016730: 2020 2020 2274 746c 223a 2033 3030 2c0a      "ttl": 300,.
+00016740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016750: 2020 2020 226c 6f63 6b65 6422 3a20 4661      "locked": Fa
+00016760: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00016770: 2020 2020 2020 2020 2022 7a6f 6e65 5f69           "zone_i
+00016780: 6422 3a20 2266 6631 3261 6233 3463 6435  d": "ff12ab34cd5
+00016790: 3631 3133 3334 3432 3261 6233 3332 3239  611334422ab33229
+000167a0: 3937 3635 3022 2c0a 2020 2020 2020 2020  97650",.        
+000167b0: 2020 2020 2020 2020 2020 2020 227a 6f6e              "zon
+000167c0: 655f 6e61 6d65 223a 2022 756e 6974 2e74  e_name": "unit.t
+000167d0: 6573 7473 222c 0a20 2020 2020 2020 2020  ests",.         
+000167e0: 2020 2020 2020 2020 2020 2022 6d6f 6469             "modi
+000167f0: 6669 6564 5f6f 6e22 3a20 2232 3031 372d  fied_on": "2017-
+00016800: 3033 2d31 3154 3138 3a30 313a 3433 2e34  03-11T18:01:43.4
+00016810: 3230 3638 395a 222c 0a20 2020 2020 2020  20689Z",.       
+00016820: 2020 2020 2020 2020 2020 2020 2022 6372               "cr
+00016830: 6561 7465 645f 6f6e 223a 2022 3230 3137  eated_on": "2017
+00016840: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+00016850: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+00016860: 2020 2020 2020 2020 2020 2020 2020 226d                "m
+00016870: 6574 6122 3a20 7b22 6175 746f 5f61 6464  eta": {"auto_add
+00016880: 6564 223a 2046 616c 7365 7d2c 0a20 2020  ed": False},.   
+00016890: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+000168a0: 2020 2020 2020 2020 2020 205d 0a20 2020             ].   
+000168b0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+000168c0: 7869 7374 696e 6720 3d20 5a6f 6e65 2827  xisting = Zone('
+000168d0: 756e 6974 2e74 6573 7473 2e27 2c20 5b5d  unit.tests.', []
+000168e0: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
+000168f0: 6572 2e70 6f70 756c 6174 6528 6578 6973  er.populate(exis
+00016900: 7469 6e67 290a 2020 2020 2020 2020 7072  ting).        pr
+00016910: 6f76 6964 6572 2e7a 6f6e 655f 7265 636f  ovider.zone_reco
+00016920: 7264 7320 3d20 4d6f 636b 280a 2020 2020  rds = Mock(.    
+00016930: 2020 2020 2020 2020 7265 7475 726e 5f76          return_v
+00016940: 616c 7565 3d5b 0a20 2020 2020 2020 2020  alue=[.         
+00016950: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00016960: 2020 2020 2020 2020 2020 2020 2022 6964               "id
+00016970: 223a 2022 3262 3331 3536 3465 3432 6664  ": "2b31564e42fd
+00016980: 3039 3564 3966 6464 3761 6261 6632 6663  095d9fdd7abaf2fc
+00016990: 3836 6638 222c 0a20 2020 2020 2020 2020  86f8",.         
+000169a0: 2020 2020 2020 2020 2020 2022 7479 7065             "type
+000169b0: 223a 2022 434e 414d 4522 2c0a 2020 2020  ": "CNAME",.    
+000169c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169d0: 226e 616d 6522 3a20 2261 2e75 6e69 742e  "name": "a.unit.
+000169e0: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
+000169f0: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00016a00: 7465 6e74 223a 2022 7777 772e 756e 6974  tent": "www.unit
+00016a10: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
+00016a20: 2020 2020 2020 2020 2020 2020 2022 7461               "ta
+00016a30: 6773 223a 205b 226f 6e65 3a61 6263 222c  gs": ["one:abc",
+00016a40: 2022 6162 633a 7465 7374 696e 6722 5d2c   "abc:testing"],
+00016a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a60: 2020 2020 2022 7474 6c22 3a20 3330 302c       "ttl": 300,
+00016a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a80: 2020 2020 2022 6c6f 636b 6564 223a 2046       "locked": F
+00016a90: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+00016aa0: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
+00016ab0: 6964 223a 2022 6666 3132 6162 3334 6364  id": "ff12ab34cd
+00016ac0: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
+00016ad0: 3939 3736 3530 222c 0a20 2020 2020 2020  997650",.       
+00016ae0: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+00016af0: 6e65 5f6e 616d 6522 3a20 2275 6e69 742e  ne_name": "unit.
+00016b00: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
+00016b10: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
+00016b20: 6966 6965 645f 6f6e 223a 2022 3230 3137  ified_on": "2017
+00016b30: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+00016b40: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+00016b50: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00016b60: 7265 6174 6564 5f6f 6e22 3a20 2232 3031  reated_on": "201
+00016b70: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
+00016b80: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
+00016b90: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00016ba0: 6d65 7461 223a 207b 2261 7574 6f5f 6164  meta": {"auto_ad
+00016bb0: 6465 6422 3a20 4661 6c73 657d 2c0a 2020  ded": False},.  
+00016bc0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00016bd0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00016be0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00016bf0: 6465 7369 7265 6420 3d20 5a6f 6e65 2827  desired = Zone('
+00016c00: 756e 6974 2e74 6573 7473 2e27 2c20 5b5d  unit.tests.', []
+00016c10: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
+00016c20: 6572 2e70 6f70 756c 6174 6528 6465 7369  er.populate(desi
+00016c30: 7265 6429 0a20 2020 2020 2020 2063 6861  red).        cha
+00016c40: 6e67 6573 203d 2065 7869 7374 696e 672e  nges = existing.
+00016c50: 6368 616e 6765 7328 6465 7369 7265 642c  changes(desired,
+00016c60: 2070 726f 7669 6465 7229 0a0a 2020 2020   provider)..    
+00016c70: 2020 2020 6578 7472 615f 6368 616e 6765      extra_change
+00016c80: 7320 3d20 7072 6f76 6964 6572 2e5f 6578  s = provider._ex
+00016c90: 7472 615f 6368 616e 6765 7328 6578 6973  tra_changes(exis
+00016ca0: 7469 6e67 2c20 6465 7369 7265 642c 2063  ting, desired, c
+00016cb0: 6861 6e67 6573 290a 0a20 2020 2020 2020  hanges)..       
+00016cc0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00016cd0: 6c28 312c 206c 656e 2865 7874 7261 5f63  l(1, len(extra_c
+00016ce0: 6861 6e67 6573 2929 0a20 2020 2020 2020  hanges)).       
+00016cf0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00016d00: 6c28 0a20 2020 2020 2020 2020 2020 2065  l(.            e
+00016d10: 7874 7261 5f63 6861 6e67 6573 5b30 5d0a  xtra_changes[0].
+00016d20: 2020 2020 2020 2020 2020 2020 2e65 7869              .exi
+00016d30: 7374 696e 672e 5f6f 6374 6f64 6e73 2e67  sting._octodns.g
+00016d40: 6574 2827 636c 6f75 6466 6c61 7265 272c  et('cloudflare',
+00016d50: 207b 7d29 0a20 2020 2020 2020 2020 2020   {}).           
+00016d60: 202e 6765 7428 2774 6167 7327 2c20 5b5d   .get('tags', []
+00016d70: 292c 0a20 2020 2020 2020 2020 2020 205b  ),.            [
+00016d80: 2274 6573 7469 6e67 3a61 6263 222c 2022  "testing:abc", "
+00016d90: 6162 633a 7465 7374 696e 6722 5d2c 0a20  abc:testing"],. 
+00016da0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00016db0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00016dc0: 6c28 0a20 2020 2020 2020 2020 2020 2073  l(.            s
+00016dd0: 6f72 7465 6428 6578 7472 615f 6368 616e  orted(extra_chan
+00016de0: 6765 735b 305d 2e6e 6577 2e5f 6f63 746f  ges[0].new._octo
+00016df0: 646e 735b 2763 6c6f 7564 666c 6172 6527  dns['cloudflare'
+00016e00: 5d5b 2774 6167 7327 5d29 2c0a 2020 2020  ]['tags']),.    
+00016e10: 2020 2020 2020 2020 736f 7274 6564 285b          sorted([
+00016e20: 226f 6e65 3a61 6263 222c 2022 6162 633a  "one:abc", "abc:
+00016e30: 7465 7374 696e 6722 5d29 2c0a 2020 2020  testing"]),.    
+00016e40: 2020 2020 290a 0a20 2020 2064 6566 2074      )..    def t
+00016e50: 6573 745f 7265 636f 7264 5f63 6f6e 7461  est_record_conta
+00016e60: 696e 735f 636f 6d6d 656e 7428 7365 6c66  ins_comment(self
+00016e70: 293a 0a20 2020 2020 2020 2070 726f 7669  ):.        provi
+00016e80: 6465 7220 3d20 436c 6f75 6466 6c61 7265  der = Cloudflare
+00016e90: 5072 6f76 6964 6572 2827 7465 7374 272c  Provider('test',
+00016ea0: 2027 656d 6169 6c27 2c20 2774 6f6b 656e   'email', 'token
+00016eb0: 2729 0a20 2020 2020 2020 207a 6f6e 6520  ').        zone 
+00016ec0: 3d20 5a6f 6e65 2827 756e 6974 2e74 6573  = Zone('unit.tes
+00016ed0: 7473 2e27 2c20 5b5d 290a 2020 2020 2020  ts.', []).      
+00016ee0: 2020 7265 636f 7264 203d 2073 6574 5f72    record = set_r
+00016ef0: 6563 6f72 645f 636f 6d6d 656e 7428 0a20  ecord_comment(. 
+00016f00: 2020 2020 2020 2020 2020 2052 6563 6f72             Recor
+00016f10: 642e 6e65 7728 0a20 2020 2020 2020 2020  d.new(.         
+00016f20: 2020 2020 2020 207a 6f6e 652c 2027 6127         zone, 'a'
+00016f30: 2c20 7b27 7474 6c27 3a20 3330 302c 2027  , {'ttl': 300, '
+00016f40: 7479 7065 273a 2027 4127 2c20 2776 616c  type': 'A', 'val
+00016f50: 7565 273a 2027 312e 322e 332e 3427 7d0a  ue': '1.2.3.4'}.
+00016f60: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00016f70: 2020 2020 2020 2020 2020 2027 616e 2065             'an e
+00016f80: 7861 6d70 6c65 2063 6f6d 6d65 6e74 272c  xample comment',
+00016f90: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00016fa0: 2020 2020 6461 7461 203d 206e 6578 7428      data = next(
+00016fb0: 7072 6f76 6964 6572 2e5f 6765 6e5f 6461  provider._gen_da
+00016fc0: 7461 2872 6563 6f72 6429 290a 0a20 2020  ta(record))..   
+00016fd0: 2020 2020 2073 656c 662e 6173 7365 7274       self.assert
+00016fe0: 4571 7561 6c28 6461 7461 5b27 636f 6d6d  Equal(data['comm
+00016ff0: 656e 7427 5d2c 2027 616e 2065 7861 6d70  ent'], 'an examp
+00017000: 6c65 2063 6f6d 6d65 6e74 2729 0a0a 2020  le comment')..  
+00017010: 2020 6465 6620 7465 7374 5f61 6464 5f63    def test_add_c
+00017020: 6f6d 6d65 6e74 2873 656c 6629 3a0a 2020  omment(self):.  
+00017030: 2020 2020 2020 7072 6f76 6964 6572 203d        provider =
+00017040: 2043 6c6f 7564 666c 6172 6550 726f 7669   CloudflareProvi
+00017050: 6465 7228 2774 6573 7427 2c20 2765 6d61  der('test', 'ema
+00017060: 696c 272c 2027 746f 6b65 6e27 290a 2020  il', 'token').  
+00017070: 2020 2020 2020 7072 6f76 6964 6572 2e7a        provider.z
+00017080: 6f6e 655f 7265 636f 7264 7320 3d20 4d6f  one_records = Mo
+00017090: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
+000170a0: 7265 7475 726e 5f76 616c 7565 3d5b 0a20  return_value=[. 
+000170b0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+000170c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000170d0: 2020 2020 2022 6964 223a 2022 6464 3533       "id": "dd53
+000170e0: 3061 3163 3833 3964 3637 3463 3433 3731  0a1c839d674c4371
+000170f0: 3434 6432 6332 6561 3238 3631 222c 0a20  44d2c2ea2861",. 
+00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017110: 2020 2022 7479 7065 223a 2022 434e 414d     "type": "CNAM
+00017120: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
+00017130: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00017140: 2261 2e75 6e69 742e 7465 7374 7322 2c0a  "a.unit.tests",.
+00017150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017160: 2020 2020 2263 6f6e 7465 6e74 223a 2022      "content": "
+00017170: 7777 772e 756e 6974 2e74 6573 7473 222c  www.unit.tests",
+00017180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017190: 2020 2020 2022 7474 6c22 3a20 3330 302c       "ttl": 300,
+000171a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000171b0: 2020 2020 2022 6c6f 636b 6564 223a 2046       "locked": F
+000171c0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+000171d0: 2020 2020 2020 2020 2020 227a 6f6e 655f            "zone_
+000171e0: 6964 223a 2022 6666 3132 6162 3334 6364  id": "ff12ab34cd
+000171f0: 3536 3131 3333 3434 3232 6162 3333 3232  5611334422ab3322
+00017200: 3939 3736 3530 222c 0a20 2020 2020 2020  997650",.       
+00017210: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+00017220: 6e65 5f6e 616d 6522 3a20 2275 6e69 742e  ne_name": "unit.
+00017230: 7465 7374 7322 2c0a 2020 2020 2020 2020  tests",.        
+00017240: 2020 2020 2020 2020 2020 2020 226d 6f64              "mod
+00017250: 6966 6965 645f 6f6e 223a 2022 3230 3137  ified_on": "2017
+00017260: 2d30 332d 3131 5431 383a 3031 3a34 332e  -03-11T18:01:43.
+00017270: 3432 3036 3839 5a22 2c0a 2020 2020 2020  420689Z",.      
+00017280: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00017290: 7265 6174 6564 5f6f 6e22 3a20 2232 3031  reated_on": "201
+000172a0: 372d 3033 2d31 3154 3138 3a30 313a 3433  7-03-11T18:01:43
+000172b0: 2e34 3230 3638 395a 222c 0a20 2020 2020  .420689Z",.     
+000172c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000172d0: 6d65 7461 223a 207b 2261 7574 6f5f 6164  meta": {"auto_ad
+000172e0: 6465 6422 3a20 4661 6c73 657d 2c0a 2020  ded": False},.  
+000172f0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00017300: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+00017310: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00017320: 6578 6973 7469 6e67 203d 205a 6f6e 6528  existing = Zone(
+00017330: 2775 6e69 742e 7465 7374 732e 272c 205b  'unit.tests.', [
+00017340: 5d29 0a20 2020 2020 2020 2070 726f 7669  ]).        provi
+00017350: 6465 722e 706f 7075 6c61 7465 2865 7869  der.populate(exi
+00017360: 7374 696e 6729 0a20 2020 2020 2020 2070  sting).        p
+00017370: 726f 7669 6465 722e 7a6f 6e65 5f72 6563  rovider.zone_rec
+00017380: 6f72 6473 203d 204d 6f63 6b28 0a20 2020  ords = Mock(.   
+00017390: 2020 2020 2020 2020 2072 6574 7572 6e5f           return_
+000173a0: 7661 6c75 653d 5b0a 2020 2020 2020 2020  value=[.        
+000173b0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+000173c0: 2020 2020 2020 2020 2020 2020 2020 2269                "i
+000173d0: 6422 3a20 2264 6435 3330 6131 6338 3339  d": "dd530a1c839
+000173e0: 6436 3734 6334 3337 3134 3464 3263 3265  d674c437144d2c2e
+000173f0: 6132 3836 3122 2c0a 2020 2020 2020 2020  a2861",.        
+00017400: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
+00017410: 6522 3a20 2243 4e41 4d45 222c 0a20 2020  e": "CNAME",.   
+00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017430: 2022 6e61 6d65 223a 2022 612e 756e 6974   "name": "a.unit
+00017440: 2e74 6573 7473 222c 0a20 2020 2020 2020  .tests",.       
+00017450: 2020 2020 2020 2020 2020 2020 2022 636f               "co
+00017460: 6e74 656e 7422 3a20 2277 7777 2e75 6e69  ntent": "www.uni
+00017470: 742e 7465 7374 7322 2c0a 2020 2020 2020  t.tests",.      
+00017480: 2020 2020 2020 2020 2020 2020 2020 2263                "c
+00017490: 6f6d 6d65 6e74 223a 2022 6120 6e65 7720  omment": "a new 
+000174a0: 636f 6d6d 656e 7422 2c0a 2020 2020 2020  comment",.      
+000174b0: 2020 2020 2020 2020 2020 2020 2020 2274                "t
+000174c0: 746c 223a 2033 3030 2c0a 2020 2020 2020  tl": 300,.      
+000174d0: 2020 2020 2020 2020 2020 2020 2020 226c                "l
+000174e0: 6f63 6b65 6422 3a20 4661 6c73 652c 0a20  ocked": False,. 
+000174f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017500: 2020 2022 7a6f 6e65 5f69 6422 3a20 2266     "zone_id": "f
+00017510: 6631 3261 6233 3463 6435 3631 3133 3334  f12ab34cd5611334
+00017520: 3432 3261 6233 3332 3239 3937 3635 3022  422ab3322997650"
+00017530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017540: 2020 2020 2020 227a 6f6e 655f 6e61 6d65        "zone_name
+00017550: 223a 2022 756e 6974 2e74 6573 7473 222c  ": "unit.tests",
+00017560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017570: 2020 2020 2022 6d6f 6469 6669 6564 5f6f       "modified_o
+00017580: 6e22 3a20 2232 3031 372d 3033 2d31 3154  n": "2017-03-11T
+00017590: 3138 3a30 313a 3433 2e34 3230 3638 395a  18:01:43.420689Z
+000175a0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000175b0: 2020 2020 2020 2022 6372 6561 7465 645f         "created_
+000175c0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
+000175d0: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
+000175e0: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
+000175f0: 2020 2020 2020 2020 226d 6574 6122 3a20          "meta": 
+00017600: 7b22 6175 746f 5f61 6464 6564 223a 2046  {"auto_added": F
+00017610: 616c 7365 7d2c 0a20 2020 2020 2020 2020  alse},.         
+00017620: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00017630: 2020 2020 205d 0a20 2020 2020 2020 2029       ].        )
+00017640: 0a20 2020 2020 2020 2064 6573 6972 6564  .        desired
+00017650: 203d 205a 6f6e 6528 2775 6e69 742e 7465   = Zone('unit.te
+00017660: 7374 732e 272c 205b 5d29 0a20 2020 2020  sts.', []).     
+00017670: 2020 2070 726f 7669 6465 722e 706f 7075     provider.popu
+00017680: 6c61 7465 2864 6573 6972 6564 290a 2020  late(desired).  
+00017690: 2020 2020 2020 6368 616e 6765 7320 3d20        changes = 
+000176a0: 6578 6973 7469 6e67 2e63 6861 6e67 6573  existing.changes
+000176b0: 2864 6573 6972 6564 2c20 7072 6f76 6964  (desired, provid
+000176c0: 6572 290a 0a20 2020 2020 2020 2065 7874  er)..        ext
+000176d0: 7261 5f63 6861 6e67 6573 203d 2070 726f  ra_changes = pro
+000176e0: 7669 6465 722e 5f65 7874 7261 5f63 6861  vider._extra_cha
+000176f0: 6e67 6573 2865 7869 7374 696e 672c 2064  nges(existing, d
+00017700: 6573 6972 6564 2c20 6368 616e 6765 7329  esired, changes)
+00017710: 0a0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00017720: 7373 6572 7445 7175 616c 2831 2c20 6c65  ssertEqual(1, le
+00017730: 6e28 6578 7472 615f 6368 616e 6765 7329  n(extra_changes)
+00017740: 290a 2020 2020 2020 2020 7365 6c66 2e61  ).        self.a
+00017750: 7373 6572 7445 7175 616c 280a 2020 2020  ssertEqual(.    
+00017760: 2020 2020 2020 2020 6578 7472 615f 6368          extra_ch
+00017770: 616e 6765 735b 305d 0a20 2020 2020 2020  anges[0].       
+00017780: 2020 2020 202e 6578 6973 7469 6e67 2e5f       .existing._
+00017790: 6f63 746f 646e 732e 6765 7428 2763 6c6f  octodns.get('clo
+000177a0: 7564 666c 6172 6527 2c20 7b7d 290a 2020  udflare', {}).  
+000177b0: 2020 2020 2020 2020 2020 2e67 6574 2827            .get('
+000177c0: 636f 6d6d 656e 7427 2c20 2727 292c 0a20  comment', ''),. 
+000177d0: 2020 2020 2020 2020 2020 2027 272c 0a20             '',. 
+000177e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000177f0: 2073 656c 662e 6173 7365 7274 4571 7561   self.assertEqua
+00017800: 6c28 0a20 2020 2020 2020 2020 2020 2065  l(.            e
+00017810: 7874 7261 5f63 6861 6e67 6573 5b30 5d2e  xtra_changes[0].
+00017820: 6e65 772e 5f6f 6374 6f64 6e73 5b27 636c  new._octodns['cl
+00017830: 6f75 6466 6c61 7265 275d 5b27 636f 6d6d  oudflare']['comm
+00017840: 656e 7427 5d2c 0a20 2020 2020 2020 2020  ent'],.         
+00017850: 2020 2027 6120 6e65 7720 636f 6d6d 656e     'a new commen
+00017860: 7427 2c0a 2020 2020 2020 2020 290a 0a20  t',.        ).. 
+00017870: 2020 2064 6566 2074 6573 745f 7570 6461     def test_upda
+00017880: 7465 5f63 6f6d 6d65 6e74 2873 656c 6629  te_comment(self)
+00017890: 3a0a 2020 2020 2020 2020 7072 6f76 6964  :.        provid
+000178a0: 6572 203d 2043 6c6f 7564 666c 6172 6550  er = CloudflareP
+000178b0: 726f 7669 6465 7228 2774 6573 7427 2c20  rovider('test', 
+000178c0: 2765 6d61 696c 272c 2027 746f 6b65 6e27  'email', 'token'
+000178d0: 290a 2020 2020 2020 2020 7072 6f76 6964  ).        provid
+000178e0: 6572 2e7a 6f6e 655f 7265 636f 7264 7320  er.zone_records 
+000178f0: 3d20 4d6f 636b 280a 2020 2020 2020 2020  = Mock(.        
+00017900: 2020 2020 7265 7475 726e 5f76 616c 7565      return_value
+00017910: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
+00017920: 2020 207b 0a20 2020 2020 2020 2020 2020     {.           
+00017930: 2020 2020 2020 2020 2022 6964 223a 2022           "id": "
+00017940: 3262 3331 3536 3465 3432 6664 3039 3564  2b31564e42fd095d
+00017950: 3966 6464 3761 6261 6632 6663 3836 6638  9fdd7abaf2fc86f8
+00017960: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017970: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00017980: 434e 414d 4522 2c0a 2020 2020 2020 2020  CNAME",.        
+00017990: 2020 2020 2020 2020 2020 2020 226e 616d              "nam
+000179a0: 6522 3a20 2261 2e75 6e69 742e 7465 7374  e": "a.unit.test
+000179b0: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+000179c0: 2020 2020 2020 2020 2263 6f6e 7465 6e74          "content
+000179d0: 223a 2022 7777 772e 756e 6974 2e74 6573  ": "www.unit.tes
+000179e0: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
+000179f0: 2020 2020 2020 2020 2022 636f 6d6d 656e           "commen
+00017a00: 7422 3a20 2261 6e20 6578 6973 7469 6e67  t": "an existing
+00017a10: 2063 6f6d 6d65 6e74 222c 0a20 2020 2020   comment",.     
+00017a20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00017a30: 7474 6c22 3a20 3330 302c 0a20 2020 2020  ttl": 300,.     
+00017a40: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00017a50: 6c6f 636b 6564 223a 2046 616c 7365 2c0a  locked": False,.
+00017a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017a70: 2020 2020 227a 6f6e 655f 6964 223a 2022      "zone_id": "
+00017a80: 6666 3132 6162 3334 6364 3536 3131 3333  ff12ab34cd561133
+00017a90: 3434 3232 6162 3333 3232 3939 3736 3530  4422ab3322997650
+00017aa0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017ab0: 2020 2020 2020 2022 7a6f 6e65 5f6e 616d         "zone_nam
+00017ac0: 6522 3a20 2275 6e69 742e 7465 7374 7322  e": "unit.tests"
+00017ad0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017ae0: 2020 2020 2020 226d 6f64 6966 6965 645f        "modified_
+00017af0: 6f6e 223a 2022 3230 3137 2d30 332d 3131  on": "2017-03-11
+00017b00: 5431 383a 3031 3a34 332e 3432 3036 3839  T18:01:43.420689
+00017b10: 5a22 2c0a 2020 2020 2020 2020 2020 2020  Z",.            
+00017b20: 2020 2020 2020 2020 2263 7265 6174 6564          "created
+00017b30: 5f6f 6e22 3a20 2232 3031 372d 3033 2d31  _on": "2017-03-1
+00017b40: 3154 3138 3a30 313a 3433 2e34 3230 3638  1T18:01:43.42068
+00017b50: 395a 222c 0a20 2020 2020 2020 2020 2020  9Z",.           
+00017b60: 2020 2020 2020 2020 2022 6d65 7461 223a           "meta":
+00017b70: 207b 2261 7574 6f5f 6164 6465 6422 3a20   {"auto_added": 
+00017b80: 4661 6c73 657d 2c0a 2020 2020 2020 2020  False},.        
+00017b90: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00017ba0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+00017bb0: 290a 2020 2020 2020 2020 6578 6973 7469  ).        existi
+00017bc0: 6e67 203d 205a 6f6e 6528 2775 6e69 742e  ng = Zone('unit.
+00017bd0: 7465 7374 732e 272c 205b 5d29 0a20 2020  tests.', []).   
+00017be0: 2020 2020 2070 726f 7669 6465 722e 706f       provider.po
+00017bf0: 7075 6c61 7465 2865 7869 7374 696e 6729  pulate(existing)
+00017c00: 0a20 2020 2020 2020 2070 726f 7669 6465  .        provide
+00017c10: 722e 7a6f 6e65 5f72 6563 6f72 6473 203d  r.zone_records =
+00017c20: 204d 6f63 6b28 0a20 2020 2020 2020 2020   Mock(.         
+00017c30: 2020 2072 6574 7572 6e5f 7661 6c75 653d     return_value=
+00017c40: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+00017c50: 2020 7b0a 2020 2020 2020 2020 2020 2020    {.            
+00017c60: 2020 2020 2020 2020 2269 6422 3a20 2232          "id": "2
+00017c70: 6233 3135 3634 6534 3266 6430 3935 6439  b31564e42fd095d9
+00017c80: 6664 6437 6162 6166 3266 6338 3666 3822  fdd7abaf2fc86f8"
+00017c90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00017ca0: 2020 2020 2020 2274 7970 6522 3a20 2243        "type": "C
+00017cb0: 4e41 4d45 222c 0a20 2020 2020 2020 2020  NAME",.         
+00017cc0: 2020 2020 2020 2020 2020 2022 6e61 6d65             "name
+00017cd0: 223a 2022 612e 756e 6974 2e74 6573 7473  ": "a.unit.tests
+00017ce0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00017cf0: 2020 2020 2020 2022 636f 6e74 656e 7422         "content"
+00017d00: 3a20 2277 7777 2e75 6e69 742e 7465 7374  : "www.unit.test
+00017d10: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00017d20: 2020 2020 2020 2020 2263 6f6d 6d65 6e74          "comment
+00017d30: 223a 2022 6120 6e65 7720 636f 6d6d 656e  ": "a new commen
+00017d40: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00017d50: 2020 2020 2020 2020 2274 746c 223a 2033          "ttl": 3
+00017d60: 3030 2c0a 2020 2020 2020 2020 2020 2020  00,.            
+00017d70: 2020 2020 2020 2020 226c 6f63 6b65 6422          "locked"
+00017d80: 3a20 4661 6c73 652c 0a20 2020 2020 2020  : False,.       
+00017d90: 2020 2020 2020 2020 2020 2020 2022 7a6f               "zo
+00017da0: 6e65 5f69 6422 3a20 2266 6631 3261 6233  ne_id": "ff12ab3
+00017db0: 3463 6435 3631 3133 3334 3432 3261 6233  4cd5611334422ab3
+00017dc0: 3332 3239 3937 3635 3022 2c0a 2020 2020  322997650",.    
+00017dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017de0: 227a 6f6e 655f 6e61 6d65 223a 2022 756e  "zone_name": "un
+00017df0: 6974 2e74 6573 7473 222c 0a20 2020 2020  it.tests",.     
+00017e00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00017e10: 6d6f 6469 6669 6564 5f6f 6e22 3a20 2232  modified_on": "2
+00017e20: 3031 372d 3033 2d31 3154 3138 3a30 313a  017-03-11T18:01:
+00017e30: 3433 2e34 3230 3638 395a 222c 0a20 2020  43.420689Z",.   
+00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e50: 2022 6372 6561 7465 645f 6f6e 223a 2022   "created_on": "
+00017e60: 3230 3137 2d30 332d 3131 5431 383a 3031  2017-03-11T18:01
+00017e70: 3a34 332e 3432 3036 3839 5a22 2c0a 2020  :43.420689Z",.  
+00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e90: 2020 226d 6574 6122 3a20 7b22 6175 746f    "meta": {"auto
+00017ea0: 5f61 6464 6564 223a 2046 616c 7365 7d2c  _added": False},
+00017eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017ec0: 207d 0a20 2020 2020 2020 2020 2020 205d   }.            ]
+00017ed0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00017ee0: 2020 2064 6573 6972 6564 203d 205a 6f6e     desired = Zon
+00017ef0: 6528 2775 6e69 742e 7465 7374 732e 272c  e('unit.tests.',
+00017f00: 205b 5d29 0a20 2020 2020 2020 2070 726f   []).        pro
+00017f10: 7669 6465 722e 706f 7075 6c61 7465 2864  vider.populate(d
+00017f20: 6573 6972 6564 290a 2020 2020 2020 2020  esired).        
+00017f30: 6368 616e 6765 7320 3d20 6578 6973 7469  changes = existi
+00017f40: 6e67 2e63 6861 6e67 6573 2864 6573 6972  ng.changes(desir
+00017f50: 6564 2c20 7072 6f76 6964 6572 290a 0a20  ed, provider).. 
+00017f60: 2020 2020 2020 2065 7874 7261 5f63 6861         extra_cha
+00017f70: 6e67 6573 203d 2070 726f 7669 6465 722e  nges = provider.
+00017f80: 5f65 7874 7261 5f63 6861 6e67 6573 2865  _extra_changes(e
+00017f90: 7869 7374 696e 672c 2064 6573 6972 6564  xisting, desired
+00017fa0: 2c20 6368 616e 6765 7329 0a0a 2020 2020  , changes)..    
+00017fb0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00017fc0: 7175 616c 2831 2c20 6c65 6e28 6578 7472  qual(1, len(extr
+00017fd0: 615f 6368 616e 6765 7329 290a 2020 2020  a_changes)).    
+00017fe0: 2020 2020 7365 6c66 2e61 7373 6572 7445      self.assertE
+00017ff0: 7175 616c 280a 2020 2020 2020 2020 2020  qual(.          
+00018000: 2020 6578 7472 615f 6368 616e 6765 735b    extra_changes[
+00018010: 305d 0a20 2020 2020 2020 2020 2020 202e  0].            .
+00018020: 6578 6973 7469 6e67 2e5f 6f63 746f 646e  existing._octodn
+00018030: 732e 6765 7428 2763 6c6f 7564 666c 6172  s.get('cloudflar
+00018040: 6527 2c20 7b7d 290a 2020 2020 2020 2020  e', {}).        
+00018050: 2020 2020 2e67 6574 2827 636f 6d6d 656e      .get('commen
+00018060: 7427 2c20 2727 292c 0a20 2020 2020 2020  t', ''),.       
+00018070: 2020 2020 2027 616e 2065 7869 7374 696e       'an existin
+00018080: 6720 636f 6d6d 656e 7427 2c0a 2020 2020  g comment',.    
+00018090: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+000180a0: 6c66 2e61 7373 6572 7445 7175 616c 280a  lf.assertEqual(.
+000180b0: 2020 2020 2020 2020 2020 2020 6578 7472              extr
+000180c0: 615f 6368 616e 6765 735b 305d 2e6e 6577  a_changes[0].new
+000180d0: 2e5f 6f63 746f 646e 735b 2763 6c6f 7564  ._octodns['cloud
+000180e0: 666c 6172 6527 5d5b 2763 6f6d 6d65 6e74  flare']['comment
+000180f0: 275d 2c0a 2020 2020 2020 2020 2020 2020  '],.            
+00018100: 2761 206e 6577 2063 6f6d 6d65 6e74 272c  'a new comment',
+00018110: 0a20 2020 2020 2020 2029 0a              .        ).
```

