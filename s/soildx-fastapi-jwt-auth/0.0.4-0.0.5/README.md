# Comparing `tmp/soildx_fastapi_jwt_auth-0.0.4.tar.gz` & `tmp/soildx_fastapi_jwt_auth-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soildx_fastapi_jwt_auth-0.0.4.tar", last modified: Mon Apr 15 10:27:41 2024, max compression
+gzip compressed data, was "soildx_fastapi_jwt_auth-0.0.5.tar", last modified: Mon Apr 15 11:26:31 2024, max compression
```

## Comparing `soildx_fastapi_jwt_auth-0.0.4.tar` & `soildx_fastapi_jwt_auth-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 10:27:41.811144 soildx_fastapi_jwt_auth-0.0.4/
--rw-rw-r--   0 akash     (1000) akash     (1000)      341 2024-04-15 10:27:41.811144 soildx_fastapi_jwt_auth-0.0.4/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)        0 2024-04-14 15:56:40.000000 soildx_fastapi_jwt_auth-0.0.4/README.md
--rw-rw-r--   0 akash     (1000) akash     (1000)       38 2024-04-15 10:27:41.811144 soildx_fastapi_jwt_auth-0.0.4/setup.cfg
--rw-rw-r--   0 akash     (1000) akash     (1000)      639 2024-04-15 10:27:14.000000 soildx_fastapi_jwt_auth-0.0.4/setup.py
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 10:27:41.811144 soildx_fastapi_jwt_auth-0.0.4/soildx_fastapi_jwt_auth.egg-info/
--rw-rw-r--   0 akash     (1000) akash     (1000)      341 2024-04-15 10:27:41.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_fastapi_jwt_auth.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      308 2024-04-15 10:27:41.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_fastapi_jwt_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        1 2024-04-15 10:27:41.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_fastapi_jwt_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       59 2024-04-15 10:27:41.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_fastapi_jwt_auth.egg-info/requires.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       16 2024-04-15 10:27:41.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_fastapi_jwt_auth.egg-info/top_level.txt
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 10:27:41.811144 soildx_fastapi_jwt_auth-0.0.4/soildx_jwt_auth/
--rw-rw-r--   0 akash     (1000) akash     (1000)       24 2024-04-15 10:26:51.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_jwt_auth/__init__.py
--rw-rw-r--   0 akash     (1000) akash     (1000)     1705 2024-04-15 05:47:39.000000 soildx_fastapi_jwt_auth-0.0.4/soildx_jwt_auth/jwt_auth.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 11:26:31.253482 soildx_fastapi_jwt_auth-0.0.5/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      341 2024-04-15 11:26:31.253482 soildx_fastapi_jwt_auth-0.0.5/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)        0 2024-04-14 15:56:40.000000 soildx_fastapi_jwt_auth-0.0.5/README.md
+-rw-rw-r--   0 akash     (1000) akash     (1000)       38 2024-04-15 11:26:31.253482 soildx_fastapi_jwt_auth-0.0.5/setup.cfg
+-rw-rw-r--   0 akash     (1000) akash     (1000)      649 2024-04-15 11:26:28.000000 soildx_fastapi_jwt_auth-0.0.5/setup.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 11:26:31.253482 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth/
+-rw-rw-r--   0 akash     (1000) akash     (1000)       24 2024-04-15 10:26:51.000000 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth/__init__.py
+-rw-rw-r--   0 akash     (1000) akash     (1000)     1705 2024-04-15 05:47:39.000000 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth/jwt_auth.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 11:26:31.253482 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth.egg-info/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      341 2024-04-15 11:26:31.000000 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      278 2024-04-15 11:26:31.000000 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        1 2024-04-15 11:26:31.000000 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)       24 2024-04-15 11:26:31.000000 soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth.egg-info/top_level.txt
```

### Comparing `soildx_fastapi_jwt_auth-0.0.4/setup.py` & `soildx_fastapi_jwt_auth-0.0.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name='soildx_fastapi_jwt_auth',
-    version="0.0.4",
+    version="0.0.5",
     author="Akash",
     description="fastapi-jwt-auth simple jwt token authentication",
     packages=find_packages(),
-    install_requires=[
-        'fastapi>=0.110.1',
-        'python-jose[cryptography]',
-        'passlib[bcrypt]'
-    ],
+    # install_requires=[
+    #     'fastapi>=0.110.1',
+    #     'python-jose[cryptography]',
+    #     'passlib[bcrypt]'
+    # ],
     long_description=description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.10"
     ],
```

### Comparing `soildx_fastapi_jwt_auth-0.0.4/soildx_jwt_auth/jwt_auth.py` & `soildx_fastapi_jwt_auth-0.0.5/soildx_fastapi_jwt_auth/jwt_auth.py`

 * *Files identical despite different names*

