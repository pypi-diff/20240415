# Comparing `tmp/apitoolkit-pyramid-0.1.3.tar.gz` & `tmp/apitoolkit-pyramid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apitoolkit-pyramid-0.1.3.tar", last modified: Tue Apr  2 22:11:06 2024, max compression
+gzip compressed data, was "apitoolkit-pyramid-0.1.4.tar", last modified: Mon Apr 15 10:53:27 2024, max compression
```

## Comparing `apitoolkit-pyramid-0.1.3.tar` & `apitoolkit-pyramid-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 22:11:06.296457 apitoolkit-pyramid-0.1.3/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     1067 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.3/LICENSE
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      275 2024-04-02 22:11:06.296457 apitoolkit-pyramid-0.1.3/PKG-INFO
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       40 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.3/README.md
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 22:11:06.292457 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6446 2024-04-02 22:10:27.000000 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid/__init__.py
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 22:11:06.296457 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid.egg-info/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      275 2024-04-02 22:11:06.000000 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      266 2024-04-02 22:11:06.000000 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)        1 2024-04-02 22:11:06.000000 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       84 2024-04-02 22:11:06.000000 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid.egg-info/requires.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       19 2024-04-02 22:11:06.000000 apitoolkit-pyramid-0.1.3/apitoolkit_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       38 2024-04-02 22:11:06.296457 apitoolkit-pyramid-0.1.3/setup.cfg
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      634 2024-04-02 22:10:18.000000 apitoolkit-pyramid-0.1.3/setup.py
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     1067 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.4/LICENSE
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     5739 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/PKG-INFO
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     5504 2024-04-03 08:44:57.000000 apitoolkit-pyramid-0.1.4/README.md
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-15 10:53:27.704083 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6419 2024-04-15 10:52:15.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid/__init__.py
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     5739 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      266 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)        1 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       84 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       19 2024-04-15 10:53:27.000000 apitoolkit-pyramid-0.1.4/apitoolkit_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       38 2024-04-15 10:53:27.708083 apitoolkit-pyramid-0.1.4/setup.cfg
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      634 2024-04-15 10:52:35.000000 apitoolkit-pyramid-0.1.4/setup.py
```

### Comparing `apitoolkit-pyramid-0.1.3/LICENSE` & `apitoolkit-pyramid-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `apitoolkit-pyramid-0.1.3/apitoolkit_pyramid/__init__.py` & `apitoolkit-pyramid-0.1.4/apitoolkit_pyramid/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,30 +92,30 @@
 
         request_body = None
         query_params =  {key: value for key, value in request.params.items()}
         request_headers = self.redact_headers_func(request.headers)
         content_type = request.headers.get('Content-Type', '')
 
         if content_type == 'application/json':
-            request_body = json.loads(request.body.decode('utf-8'))
+            request_body = request.json_body
         if content_type == 'text/plain':
             request_body = request.body.decode('utf-8')
         if content_type == 'application/x-www-form-urlencoded' or 'multipart/form-data' in content_type:
             request_body = dict(request.POST.copy())
         request.apitoolkit_message_id = str(uuid.uuid4())
         request.apitoolkit_errors = []
         request.apitoolkit_client = self
 
         response = self.get_response(request)
 
         if self.debug:
             print("APIToolkit: after request")
         end_time = time.perf_counter_ns()
         url_path = request.matched_route.pattern if request.matched_route is not None else request.path
-        path_params = request.matchdict     
+        path_params = request.matchdict
         duration = (end_time - start_time)
         status_code = response.status_code
         request_body = json.dumps(request_body)
         response_headers = self.redact_headers_func(response.headers)
         request_body = self.redact_fields(
             request_body, self.redact_request_body)
         response_body = self.redact_fields(
@@ -148,8 +148,8 @@
                 "service_version": self.service_version,
                 "tags": self.tags,
                 "timestamp": timestamp
             }
             self.publish_message(payload)
         except Exception as e:
             return response
-        return response
+        return response
```

### Comparing `apitoolkit-pyramid-0.1.3/setup.py` & `apitoolkit-pyramid-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apitoolkit-pyramid",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     description='A Python Pyramid SDK for Apitoolkit integration',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='hello@apitoolkit.io',
     author='APIToolkit',
     install_requires=[
```

