# Comparing `tmp/eurovat-0.9.4.tar.gz` & `tmp/eurovat-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurovat-0.9.4.tar", last modified: Sun Dec 12 17:48:39 2021, max compression
+gzip compressed data, was "eurovat-0.9.5.tar", last modified: Sun Dec 12 18:37:54 2021, max compression
```

## Comparing `eurovat-0.9.4.tar` & `eurovat-0.9.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 17:48:39.795998 eurovat-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2021-12-12 17:48:39.795998 eurovat-0.9.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 17:48:39.795998 eurovat-0.9.4/eurovat/
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 17:48:39.795998 eurovat-0.9.4/eurovat/cache/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      795 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/cache/django.py
--rw-r--r--   0 runner    (1001) docker     (121)      804 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/cache/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/cn_code.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 17:48:39.795998 eurovat-0.9.4/eurovat/data/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3733 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/rate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1740 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/states.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/tedb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3017 2021-12-12 17:48:28.000000 eurovat-0.9.4/eurovat/vat_number.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 17:48:39.795998 eurovat-0.9.4/eurovat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2975 2021-12-12 17:48:39.000000 eurovat-0.9.4/eurovat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-12-12 17:48:39.000000 eurovat-0.9.4/eurovat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-12 17:48:39.000000 eurovat-0.9.4/eurovat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-12 17:48:35.000000 eurovat-0.9.4/eurovat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-12 17:48:39.000000 eurovat-0.9.4/eurovat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-12-12 17:48:39.000000 eurovat-0.9.4/eurovat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      693 2021-12-12 17:48:39.795998 eurovat-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       73 2021-12-12 17:48:28.000000 eurovat-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 18:37:54.602076 eurovat-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)     2975 2021-12-12 18:37:54.602076 eurovat-0.9.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 18:37:54.602076 eurovat-0.9.5/eurovat/
+-rw-r--r--   0 runner    (1001) docker     (121)      304 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 18:37:54.602076 eurovat-0.9.5/eurovat/cache/
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      795 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/cache/django.py
+-rw-r--r--   0 runner    (1001) docker     (121)      804 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/cache/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1195 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/cn_code.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 18:37:54.602076 eurovat-0.9.5/eurovat/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      213 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      400 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3733 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/rate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1740 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/states.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2656 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/tedb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3017 2021-12-12 18:37:38.000000 eurovat-0.9.5/eurovat/vat_number.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-12 18:37:54.602076 eurovat-0.9.5/eurovat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2975 2021-12-12 18:37:54.000000 eurovat-0.9.5/eurovat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-12-12 18:37:54.000000 eurovat-0.9.5/eurovat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-12 18:37:54.000000 eurovat-0.9.5/eurovat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-12 18:37:50.000000 eurovat-0.9.5/eurovat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2021-12-12 18:37:54.000000 eurovat-0.9.5/eurovat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2021-12-12 18:37:54.000000 eurovat-0.9.5/eurovat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      693 2021-12-12 18:37:54.606076 eurovat-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2021-12-12 18:37:38.000000 eurovat-0.9.5/setup.py
```

### Comparing `eurovat-0.9.4/PKG-INFO` & `eurovat-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurovat
-Version: 0.9.4
+Version: 0.9.5
 Summary: A python library to get the vat right in the EU.
 Home-page: https://github.com/airgproducts/eurovat
 Author: airG products
 Author-email: hello@airgproducts.com
 License: MIT License
 Keywords: vat,eu,tax
 Platform: UNKNOWN
```

### Comparing `eurovat-0.9.4/eurovat/cache/django.py` & `eurovat-0.9.5/eurovat/cache/django.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat/cache/filesystem.py` & `eurovat-0.9.5/eurovat/cache/filesystem.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat/cn_code.py` & `eurovat-0.9.5/eurovat/cn_code.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat/rate.py` & `eurovat-0.9.5/eurovat/rate.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat/registry.py` & `eurovat-0.9.5/eurovat/registry.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat/states.py` & `eurovat-0.9.5/eurovat/states.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat/tedb.py` & `eurovat-0.9.5/eurovat/tedb.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,13 +75,19 @@
     rates["DE"].append(VatRate(
         reduced=False,
         rate=decimal.Decimal("16"),
         cn_codes=[],
         cpa_codes=[],
         situation_on=datetime.datetime(2020, 7, 1).timestamp()
     ))
+
+    # canary-islands-reduced rate
+    spanish_standard_rates = filter(lambda el: el.reduced==False, rates["ES"])
+    for rate_es in spanish_standard_rates:
+        if rate_es.description:
+            rate_es.reduced = True
     
     return [
         VatRules(EUState.get(country_name), rate_lst)
         
         for country_name, rate_lst in rates.items()
     ]
```

### Comparing `eurovat-0.9.4/eurovat/vat_number.py` & `eurovat-0.9.5/eurovat/vat_number.py`

 * *Files identical despite different names*

### Comparing `eurovat-0.9.4/eurovat.egg-info/PKG-INFO` & `eurovat-0.9.5/eurovat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eurovat
-Version: 0.9.4
+Version: 0.9.5
 Summary: A python library to get the vat right in the EU.
 Home-page: https://github.com/airgproducts/eurovat
 Author: airG products
 Author-email: hello@airgproducts.com
 License: MIT License
 Keywords: vat,eu,tax
 Platform: UNKNOWN
```

### Comparing `eurovat-0.9.4/setup.cfg` & `eurovat-0.9.5/setup.cfg`

 * *Files identical despite different names*

