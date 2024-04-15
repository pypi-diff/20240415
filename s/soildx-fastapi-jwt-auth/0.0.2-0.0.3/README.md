# Comparing `tmp/soildx_fastapi_jwt_auth-0.0.2.tar.gz` & `tmp/soildx_fastapi_jwt_auth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soildx_fastapi_jwt_auth-0.0.2.tar", last modified: Mon Apr 15 09:30:00 2024, max compression
+gzip compressed data, was "soildx_fastapi_jwt_auth-0.0.3.tar", last modified: Mon Apr 15 09:37:22 2024, max compression
```

## Comparing `soildx_fastapi_jwt_auth-0.0.2.tar` & `soildx_fastapi_jwt_auth-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 09:30:00.108944 soildx_fastapi_jwt_auth-0.0.2/
--rw-rw-r--   0 akash     (1000) akash     (1000)      243 2024-04-15 09:30:00.108944 soildx_fastapi_jwt_auth-0.0.2/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)        0 2024-04-14 15:56:40.000000 soildx_fastapi_jwt_auth-0.0.2/README.md
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 09:30:00.108944 soildx_fastapi_jwt_auth-0.0.2/authentication/
--rw-rw-r--   0 akash     (1000) akash     (1000)       24 2024-04-15 05:47:13.000000 soildx_fastapi_jwt_auth-0.0.2/authentication/__init__.py
--rw-rw-r--   0 akash     (1000) akash     (1000)     1705 2024-04-15 05:47:39.000000 soildx_fastapi_jwt_auth-0.0.2/authentication/jwt_auth.py
--rw-rw-r--   0 akash     (1000) akash     (1000)       38 2024-04-15 09:30:00.108944 soildx_fastapi_jwt_auth-0.0.2/setup.cfg
--rw-rw-r--   0 akash     (1000) akash     (1000)      496 2024-04-15 09:29:53.000000 soildx_fastapi_jwt_auth-0.0.2/setup.py
-drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 09:30:00.108944 soildx_fastapi_jwt_auth-0.0.2/soildx_fastapi_jwt_auth.egg-info/
--rw-rw-r--   0 akash     (1000) akash     (1000)      243 2024-04-15 09:30:00.000000 soildx_fastapi_jwt_auth-0.0.2/soildx_fastapi_jwt_auth.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1000) akash     (1000)      306 2024-04-15 09:30:00.000000 soildx_fastapi_jwt_auth-0.0.2/soildx_fastapi_jwt_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)        1 2024-04-15 09:30:00.000000 soildx_fastapi_jwt_auth-0.0.2/soildx_fastapi_jwt_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       59 2024-04-15 09:30:00.000000 soildx_fastapi_jwt_auth-0.0.2/soildx_fastapi_jwt_auth.egg-info/requires.txt
--rw-rw-r--   0 akash     (1000) akash     (1000)       15 2024-04-15 09:30:00.000000 soildx_fastapi_jwt_auth-0.0.2/soildx_fastapi_jwt_auth.egg-info/top_level.txt
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 09:37:22.558700 soildx_fastapi_jwt_auth-0.0.3/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      243 2024-04-15 09:37:22.558700 soildx_fastapi_jwt_auth-0.0.3/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)        0 2024-04-14 15:56:40.000000 soildx_fastapi_jwt_auth-0.0.3/README.md
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 09:37:22.558700 soildx_fastapi_jwt_auth-0.0.3/authentication/
+-rw-rw-r--   0 akash     (1000) akash     (1000)       24 2024-04-15 05:47:13.000000 soildx_fastapi_jwt_auth-0.0.3/authentication/__init__.py
+-rw-rw-r--   0 akash     (1000) akash     (1000)     1705 2024-04-15 05:47:39.000000 soildx_fastapi_jwt_auth-0.0.3/authentication/jwt_auth.py
+-rw-rw-r--   0 akash     (1000) akash     (1000)       38 2024-04-15 09:37:22.558700 soildx_fastapi_jwt_auth-0.0.3/setup.cfg
+-rw-rw-r--   0 akash     (1000) akash     (1000)      496 2024-04-15 09:30:27.000000 soildx_fastapi_jwt_auth-0.0.3/setup.py
+drwxrwxr-x   0 akash     (1000) akash     (1000)        0 2024-04-15 09:37:22.558700 soildx_fastapi_jwt_auth-0.0.3/soildx_fastapi_jwt_auth.egg-info/
+-rw-rw-r--   0 akash     (1000) akash     (1000)      243 2024-04-15 09:37:22.000000 soildx_fastapi_jwt_auth-0.0.3/soildx_fastapi_jwt_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1000) akash     (1000)      306 2024-04-15 09:37:22.000000 soildx_fastapi_jwt_auth-0.0.3/soildx_fastapi_jwt_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)        1 2024-04-15 09:37:22.000000 soildx_fastapi_jwt_auth-0.0.3/soildx_fastapi_jwt_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)       59 2024-04-15 09:37:22.000000 soildx_fastapi_jwt_auth-0.0.3/soildx_fastapi_jwt_auth.egg-info/requires.txt
+-rw-rw-r--   0 akash     (1000) akash     (1000)       15 2024-04-15 09:37:22.000000 soildx_fastapi_jwt_auth-0.0.3/soildx_fastapi_jwt_auth.egg-info/top_level.txt
```

### Comparing `soildx_fastapi_jwt_auth-0.0.2/authentication/jwt_auth.py` & `soildx_fastapi_jwt_auth-0.0.3/authentication/jwt_auth.py`

 * *Files identical despite different names*

