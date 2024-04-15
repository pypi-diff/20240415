# Comparing `tmp/porkbun_ddns-0.6.1-py3-none-any.whl.zip` & `tmp/porkbun_ddns-0.6.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9164 bytes, number of entries: 10
--rw-r--r--  2.0 unx       82 b- defN 24-Mar-03 14:45 porkbun_ddns/__init__.py
--rw-r--r--  2.0 unx     3254 b- defN 24-Mar-03 14:45 porkbun_ddns/cli.py
--rw-r--r--  2.0 unx     1475 b- defN 24-Mar-03 14:45 porkbun_ddns/helpers.py
--rw-r--r--  2.0 unx    10175 b- defN 24-Mar-03 14:45 porkbun_ddns/porkbun_ddns.py
--rw-r--r--  2.0 unx     1061 b- defN 24-Mar-03 14:46 porkbun_ddns-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5415 b- defN 24-Mar-03 14:46 porkbun_ddns-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-03 14:46 porkbun_ddns-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       55 b- defN 24-Mar-03 14:46 porkbun_ddns-0.6.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-03 14:46 porkbun_ddns-0.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      832 b- defN 24-Mar-03 14:46 porkbun_ddns-0.6.1.dist-info/RECORD
-10 files, 22454 bytes uncompressed, 7736 bytes compressed:  65.5%
+Zip file size: 9190 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       82 b- defN 24-Apr-15 06:10 porkbun_ddns/__init__.py
+-rw-r--r--  2.0 unx     3254 b- defN 24-Apr-15 06:10 porkbun_ddns/cli.py
+-rw-r--r--  2.0 unx     1475 b- defN 24-Apr-15 06:10 porkbun_ddns/helpers.py
+-rw-r--r--  2.0 unx    10256 b- defN 24-Apr-15 06:10 porkbun_ddns/porkbun_ddns.py
+-rw-r--r--  2.0 unx     1061 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5532 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      832 b- defN 24-Apr-15 06:10 porkbun_ddns-0.6.2.dist-info/RECORD
+10 files, 22652 bytes uncompressed, 7762 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: porkbun_ddns/helpers.py
 Comment: 
 
 Filename: porkbun_ddns/porkbun_ddns.py
 Comment: 
 
-Filename: porkbun_ddns-0.6.1.dist-info/LICENSE
+Filename: porkbun_ddns-0.6.2.dist-info/LICENSE
 Comment: 
 
-Filename: porkbun_ddns-0.6.1.dist-info/METADATA
+Filename: porkbun_ddns-0.6.2.dist-info/METADATA
 Comment: 
 
-Filename: porkbun_ddns-0.6.1.dist-info/WHEEL
+Filename: porkbun_ddns-0.6.2.dist-info/WHEEL
 Comment: 
 
-Filename: porkbun_ddns-0.6.1.dist-info/entry_points.txt
+Filename: porkbun_ddns-0.6.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: porkbun_ddns-0.6.1.dist-info/top_level.txt
+Filename: porkbun_ddns-0.6.2.dist-info/top_level.txt
 Comment: 
 
-Filename: porkbun_ddns-0.6.1.dist-info/RECORD
+Filename: porkbun_ddns-0.6.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## porkbun_ddns/porkbun_ddns.py

```diff
@@ -64,15 +64,17 @@
             raise PorkbunDDNS_Error("Missing keys! All of the following are required: '{}'\nYour config:\n{}".format(
                 required_keys, self.config))
         if 'endpoint' not in self.config.keys():
             self.config["endpoint"] = "https://porkbun.com/api/json/v3"
 
     def set_subdomain(self, subdomain: str) -> None:
         self.subdomain = subdomain.lower()
-        if self.subdomain != '@':
+        if self.subdomain == '@':
+            self.fqdn = self.domain
+        else:
             self.fqdn = '.'.join([self.subdomain, self.domain])
 
     def get_public_ips(self) -> list:
         """Retrieve the public IP addresses of the network.
         """
         if self.static_ips:
             public_ips = self.static_ips
@@ -193,15 +195,15 @@
         """Delete A and AAAA DNS record for set record.
         """
         self.records = self.get_records()
         domain_names = [x['name'] for x in self.records if x['type']
                         in ["A", "AAAA"]]
         if self.fqdn in domain_names:
             for i in self.records:
-                if i["name"] == self.fqdn:
+                if i["name"] == self.fqdn and i['type'] in ["A", "AAAA"]:
                     logger.debug('Deleting existing entry:\n{}'.format(json.dumps(
                         {"name": self.fqdn, "type": i['type'], "content": str(i['content'])})))
                     self._delete_record(i['id'])
         else:
             logger.debug('Record not found:\n{}'.format(json.dumps(
                 {"name": self.fqdn, "type": i['type'], "content": str(i['content'])})))
```

## Comparing `porkbun_ddns-0.6.1.dist-info/LICENSE` & `porkbun_ddns-0.6.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `porkbun_ddns-0.6.1.dist-info/METADATA` & `porkbun_ddns-0.6.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: porkbun-ddns
-Version: 0.6.1
+Version: 0.6.2
 Summary: A unofficial DDNS-Client for Porkbun domains
 Home-page: https://github.com/mietzen/porkbun-ddns
 Author: Nils Stein
 Author-email: github.nstein@mailbox.org
 License: MIT
 Keywords: porkbun ddns
 Classifier: Development Status :: 4 - Beta
@@ -73,14 +73,17 @@
 
 ```shell
 $ porkbun-ddns "./config.json" domain.com my_subdomain
 
 # Multiple subdomains:
 $ porkbun-ddns "./config.json" domain.com my_subdomain_1 my_subdomain_2 my_subdomain_3
 
+# Set root and subdomains:
+$ porkbun-ddns "./config.json" domain.com @ my_subdomain_1 my_subdomain_2 my_subdomain_3
+
 # Get config from environment variable:
 # PORKBUN_APIKEY
 # PORKBUN_SECRETAPIKEY
 # PORKBUN_DDNS_ENDPOINT (Optional)
 $ porkbun-ddns - domain.com my_subdomain
 
 # Set IP's explicit
```

## Comparing `porkbun_ddns-0.6.1.dist-info/RECORD` & `porkbun_ddns-0.6.2.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 porkbun_ddns/__init__.py,sha256=4E9knps0KH0NhbKGNNEeixpexHTNnxHbfUvhJD7rOUU,82
 porkbun_ddns/cli.py,sha256=WQJEcM4qsmpODHd83X_gA9fDJ-OTNbjzceZlO4EpL24,3254
 porkbun_ddns/helpers.py,sha256=i3OPqrDzMJTuhuGC18V2qerYI_i77dSF-nFIQMBcSEM,1475
-porkbun_ddns/porkbun_ddns.py,sha256=B1PtxrNFHbSYtNbRCrr69sy4d_2GTXbZ6H82N6VlhlA,10175
-porkbun_ddns-0.6.1.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
-porkbun_ddns-0.6.1.dist-info/METADATA,sha256=MShIIduJWD5UmDrUxpo8M_shOOwDJJKyZ9ntXCmk70c,5415
-porkbun_ddns-0.6.1.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-porkbun_ddns-0.6.1.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
-porkbun_ddns-0.6.1.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
-porkbun_ddns-0.6.1.dist-info/RECORD,,
+porkbun_ddns/porkbun_ddns.py,sha256=B6P0kSVEG_E6AsyQXOWIctd1sFznWCs8WIVZr8r4dZU,10256
+porkbun_ddns-0.6.2.dist-info/LICENSE,sha256=WbmjIVUkxwQ1vDNiEe2eMKL3-6nYRBN1qUv7rdvvSvY,1061
+porkbun_ddns-0.6.2.dist-info/METADATA,sha256=kF_KNairMrlu-UJbMeu8xD9yCTu2u4gH5DP0K7LYe0Y,5532
+porkbun_ddns-0.6.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+porkbun_ddns-0.6.2.dist-info/entry_points.txt,sha256=Ux4_6ekA_PZiOxw-7MbJOvQVo_7IJQzaYS24EzSjwbg,55
+porkbun_ddns-0.6.2.dist-info/top_level.txt,sha256=8hi5L7CGOlYLIOlnnPPToRxZqnZ1UkpUmCYbgYZO2JA,13
+porkbun_ddns-0.6.2.dist-info/RECORD,,
```

