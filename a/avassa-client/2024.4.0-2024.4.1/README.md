# Comparing `tmp/avassa-client-2024.4.0.tar.gz` & `tmp/avassa_client-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avassa-client-2024.4.0.tar", last modified: Fri Apr  5 12:39:54 2024, max compression
+gzip compressed data, was "avassa_client-2024.4.1.tar", last modified: Mon Apr 15 12:23:06 2024, max compression
```

## Comparing `avassa-client-2024.4.0.tar` & `avassa_client-2024.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-05 12:39:54.110092 avassa-client-2024.4.0/
--rw-r--r--   0 frja       (501) staff       (20)    11343 2023-04-25 10:38:10.000000 avassa-client-2024.4.0/LICENSE
--rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-05 12:39:54.109761 avassa-client-2024.4.0/PKG-INFO
--rw-r--r--   0 frja       (501) staff       (20)      758 2024-01-15 13:20:32.000000 avassa-client-2024.4.0/README.md
-drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-05 12:39:54.108776 avassa-client-2024.4.0/avassa_client/
--rw-r--r--   0 frja       (501) staff       (20)    10414 2024-04-05 12:14:05.000000 avassa-client-2024.4.0/avassa_client/__init__.py
--rw-r--r--   0 frja       (501) staff       (20)    17620 2024-01-15 13:06:43.000000 avassa-client-2024.4.0/avassa_client/volga.py
-drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-05 12:39:54.109559 avassa-client-2024.4.0/avassa_client.egg-info/
--rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/PKG-INFO
--rw-r--r--   0 frja       (501) staff       (20)      265 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/SOURCES.txt
--rw-r--r--   0 frja       (501) staff       (20)        1 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/dependency_links.txt
--rw-r--r--   0 frja       (501) staff       (20)       15 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/requires.txt
--rw-r--r--   0 frja       (501) staff       (20)       14 2024-04-05 12:39:54.000000 avassa-client-2024.4.0/avassa_client.egg-info/top_level.txt
--rw-r--r--   0 frja       (501) staff       (20)      654 2024-04-05 12:15:21.000000 avassa-client-2024.4.0/pyproject.toml
--rw-r--r--   0 frja       (501) staff       (20)       38 2024-04-05 12:39:54.110146 avassa-client-2024.4.0/setup.cfg
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-15 12:23:06.048917 avassa_client-2024.4.1/
+-rw-r--r--   0 frja       (501) staff       (20)    11343 2023-04-25 10:38:10.000000 avassa_client-2024.4.1/LICENSE
+-rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-15 12:23:06.048590 avassa_client-2024.4.1/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      758 2024-01-15 13:20:32.000000 avassa_client-2024.4.1/README.md
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-15 12:23:06.046927 avassa_client-2024.4.1/avassa_client/
+-rw-r--r--   0 frja       (501) staff       (20)    10471 2024-04-15 12:20:50.000000 avassa_client-2024.4.1/avassa_client/__init__.py
+-rw-r--r--   0 frja       (501) staff       (20)    17620 2024-01-15 13:06:43.000000 avassa_client-2024.4.1/avassa_client/volga.py
+drwxr-xr-x   0 frja       (501) staff       (20)        0 2024-04-15 12:23:06.048310 avassa_client-2024.4.1/avassa_client.egg-info/
+-rw-r--r--   0 frja       (501) staff       (20)    14236 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/PKG-INFO
+-rw-r--r--   0 frja       (501) staff       (20)      265 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 frja       (501) staff       (20)        1 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 frja       (501) staff       (20)       15 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/requires.txt
+-rw-r--r--   0 frja       (501) staff       (20)       14 2024-04-15 12:23:06.000000 avassa_client-2024.4.1/avassa_client.egg-info/top_level.txt
+-rw-r--r--   0 frja       (501) staff       (20)      654 2024-04-15 12:22:36.000000 avassa_client-2024.4.1/pyproject.toml
+-rw-r--r--   0 frja       (501) staff       (20)       38 2024-04-15 12:23:06.048967 avassa_client-2024.4.1/setup.cfg
```

### Comparing `avassa-client-2024.4.0/LICENSE` & `avassa_client-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avassa-client-2024.4.0/PKG-INFO` & `avassa_client-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avassa-client
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Library for integrating with the Avassa APIs
 Author-email: Avassa <info@avassa.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `avassa-client-2024.4.0/README.md` & `avassa_client-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `avassa-client-2024.4.0/avassa_client/__init__.py` & `avassa_client-2024.4.1/avassa_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,14 +156,16 @@
                   secret_id: str,
                   user_agent: Optional[str] = None,
                   server_hostname: Optional[str] = None):
     try:
         payload = {'secret-id': secret_id}
         if role_id is not None:
             payload['role-id'] = role_id
+        else:
+            payload['role-id'] = secret_id
         base_url = urlparse(host)
         url = base_url.geturl() + '/v1/approle-login'
         sslc = create_ssl_context(server_hostname)
         (_code, msg, _headers, body) = post_request(
             None, url, payload, user_agent, sslc)
         del payload['secret-id']
         if msg != 'OK':
```

### Comparing `avassa-client-2024.4.0/avassa_client/volga.py` & `avassa_client-2024.4.1/avassa_client/volga.py`

 * *Files identical despite different names*

### Comparing `avassa-client-2024.4.0/avassa_client.egg-info/PKG-INFO` & `avassa_client-2024.4.1/avassa_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avassa-client
-Version: 2024.4.0
+Version: 2024.4.1
 Summary: Library for integrating with the Avassa APIs
 Author-email: Avassa <info@avassa.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `avassa-client-2024.4.0/pyproject.toml` & `avassa_client-2024.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avassa-client"
-version = "2024.4.0"
+version = "2024.4.1"
 description = "Library for integrating with the Avassa APIs"
 readme = "README.md"
 authors = [{ name = "Avassa", email = "info@avassa.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

