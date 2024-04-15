# Comparing `tmp/sleekify-0.0.8.tar.gz` & `tmp/sleekify-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleekify-0.0.8.tar", last modified: Thu Feb 15 16:06:37 2024, max compression
+gzip compressed data, was "sleekify-0.0.9.tar", last modified: Thu Feb 15 17:26:39 2024, max compression
```

## Comparing `sleekify-0.0.8.tar` & `sleekify-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 16:06:37.092488 sleekify-0.0.8/
--rw-r--r--   0 matt       (501) staff       (20)      902 2024-02-15 16:06:37.092227 sleekify-0.0.8/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      378 2024-02-15 04:22:24.000000 sleekify-0.0.8/README.md
--rw-r--r--   0 matt       (501) staff       (20)       38 2024-02-15 16:06:37.092534 sleekify-0.0.8/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)      719 2024-02-15 16:06:17.000000 sleekify-0.0.8/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 16:06:37.090717 sleekify-0.0.8/sleekify/
--rw-r--r--   0 matt       (501) staff       (20)     4350 2024-02-15 16:06:12.000000 sleekify-0.0.8/sleekify/__init__.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 16:06:37.091633 sleekify-0.0.8/sleekify/guard/
--rw-r--r--   0 matt       (501) staff       (20)      474 2024-02-15 03:32:56.000000 sleekify-0.0.8/sleekify/guard/__init__.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 16:06:37.091768 sleekify-0.0.8/sleekify/types/
--rw-r--r--   0 matt       (501) staff       (20)      302 2024-02-15 03:34:26.000000 sleekify-0.0.8/sleekify/types/__init__.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 16:06:37.091988 sleekify-0.0.8/sleekify.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)      902 2024-02-15 16:06:37.000000 sleekify-0.0.8/sleekify.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      252 2024-02-15 16:06:37.000000 sleekify-0.0.8/sleekify.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2024-02-15 16:06:37.000000 sleekify-0.0.8/sleekify.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       33 2024-02-15 16:06:37.000000 sleekify-0.0.8/sleekify.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)        9 2024-02-15 16:06:37.000000 sleekify-0.0.8/sleekify.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 17:26:39.133862 sleekify-0.0.9/
+-rw-r--r--   0 matt       (501) staff       (20)      902 2024-02-15 17:26:39.133609 sleekify-0.0.9/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      378 2024-02-15 04:22:24.000000 sleekify-0.0.9/README.md
+-rw-r--r--   0 matt       (501) staff       (20)       38 2024-02-15 17:26:39.133909 sleekify-0.0.9/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)      719 2024-02-15 17:15:47.000000 sleekify-0.0.9/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 17:26:39.131649 sleekify-0.0.9/sleekify/
+-rw-r--r--   0 matt       (501) staff       (20)     4339 2024-02-15 17:14:58.000000 sleekify-0.0.9/sleekify/__init__.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 17:26:39.132707 sleekify-0.0.9/sleekify/guard/
+-rw-r--r--   0 matt       (501) staff       (20)      474 2024-02-15 03:32:56.000000 sleekify-0.0.9/sleekify/guard/__init__.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 17:26:39.133030 sleekify-0.0.9/sleekify/types/
+-rw-r--r--   0 matt       (501) staff       (20)      302 2024-02-15 03:34:26.000000 sleekify-0.0.9/sleekify/types/__init__.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2024-02-15 17:26:39.133362 sleekify-0.0.9/sleekify.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)      902 2024-02-15 17:26:39.000000 sleekify-0.0.9/sleekify.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      252 2024-02-15 17:26:39.000000 sleekify-0.0.9/sleekify.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2024-02-15 17:26:39.000000 sleekify-0.0.9/sleekify.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)       33 2024-02-15 17:26:39.000000 sleekify-0.0.9/sleekify.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)        9 2024-02-15 17:26:39.000000 sleekify-0.0.9/sleekify.egg-info/top_level.txt
```

### Comparing `sleekify-0.0.8/PKG-INFO` & `sleekify-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleekify
-Version: 0.0.8
+Version: 0.0.9
 Summary: A minimalistic, ASGI, Python framework for building REST API's.
 Home-page: https://github.com/0mjs/sleek
 Author: Matt J. Stevenson
 Author-email: dev@mattjs.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sleekify-0.0.8/setup.py` & `sleekify-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="sleekify",
-    version="0.0.8",
+    version="0.0.9",
     author="Matt J. Stevenson",
     author_email="dev@mattjs.me",
     description="A minimalistic, ASGI, Python framework for building REST API's.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/0mjs/sleek",
     packages=find_packages(),
```

### Comparing `sleekify-0.0.8/sleekify/__init__.py` & `sleekify-0.0.9/sleekify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,24 @@
 
     async def resolve_parameters(
         self, request: Request, router: Router
     ) -> Dict[str, Any]:
         sig = signature(router)
         kwargs = {}
 
-        if "_request" in sig.parameters:
-            kwargs["_request"] = request
-
-        if request.method in ["POST", "PUT", "PATCH"]:
-            try:
-                json_body = await request.json()
-            except JSONDecodeError:
-                json_body = {}
-
-            for name, param in sig.parameters.items():
-                if name == "_request":
-                    continue
+        for name, param in sig.parameters.items():
+            if param.annotation is Request:
+                kwargs[name] = request
+                continue
+
+            if request.method in ["POST", "PUT", "PATCH"]:
+                try:
+                    json_body = await request.json()
+                except JSONDecodeError:
+                    json_body = {}
 
                 if isinstance(param.default, Guard):
                     resolved_value = await param.default.resolve()
                     kwargs[name] = resolved_value
                 elif isclass(param.annotation) and issubclass(
                     param.annotation, BaseModel
                 ):
@@ -51,18 +49,18 @@
                     except ValidationError as e:
                         return JSONResponse({"detail": e.errors()}, status_code=422)
                 else:
                     value = json_body.get(
                         name, param.default if param.default is not _empty else None
                     )
                     kwargs[name] = value
-        else:
-            for name, param in sig.parameters.items():
-                if name == "_request":
-                    continue
+            else:
+                for name, param in sig.parameters.items():
+                    if name == "_request":
+                        continue
 
         return kwargs
 
     async def common_handler(self, request: Request, router: Router):
         kwargs = await self.resolve_parameters(request, router)
         response = await router(**kwargs)
```

### Comparing `sleekify-0.0.8/sleekify.egg-info/PKG-INFO` & `sleekify-0.0.9/sleekify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleekify
-Version: 0.0.8
+Version: 0.0.9
 Summary: A minimalistic, ASGI, Python framework for building REST API's.
 Home-page: https://github.com/0mjs/sleek
 Author: Matt J. Stevenson
 Author-email: dev@mattjs.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

