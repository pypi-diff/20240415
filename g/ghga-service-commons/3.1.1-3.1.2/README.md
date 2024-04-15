# Comparing `tmp/ghga_service_commons-3.1.1.tar.gz` & `tmp/ghga_service_commons-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghga_service_commons-3.1.1.tar", last modified: Thu Mar 14 08:11:13 2024, max compression
+gzip compressed data, was "ghga_service_commons-3.1.2.tar", last modified: Mon Apr 15 14:09:36 2024, max compression
```

## Comparing `ghga_service_commons-3.1.1.tar` & `ghga_service_commons-3.1.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.655211 ghga_service_commons-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-03-14 08:11:13.651211 ghga_service_commons-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 08:11:13.655211 ghga_service_commons-3.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.643211 ghga_service_commons-3.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.643211 ghga_service_commons-3.1.1/src/ghga_service_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.647211 ghga_service_commons-3.1.1/src/ghga_service_commons/api/
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/api/di.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/api/mock_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/api/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.647211 ghga_service_commons-3.1.1/src/ghga_service_commons/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/auth/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/auth/ghga.py
--rw-r--r--   0 runner    (1001) docker     (127)     5811 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/auth/jwt_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/auth/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.647211 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.647211 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9429 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.647211 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.651211 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.651211 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/crypt4gh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/jwt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/multinode_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/simple_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/temp_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-03-14 08:11:06.000000 ghga_service_commons-3.1.1/src/ghga_service_commons/utils/utc_dates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 08:11:13.651211 ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-03-14 08:11:13.000000 ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-14 08:11:13.000000 ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 08:11:13.000000 ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-14 08:11:13.000000 ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-14 08:11:13.000000 ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.115130 ghga_service_commons-3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-15 14:09:36.115130 ghga_service_commons-3.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:09:36.115130 ghga_service_commons-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.103130 ghga_service_commons-3.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.107130 ghga_service_commons-3.1.2/src/ghga_service_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.107130 ghga_service_commons-3.1.2/src/ghga_service_commons/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/di.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/mock_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/api/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.107130 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/ghga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/jwt_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/auth/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5859 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt4gh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/jwt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/multinode_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/simple_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/temp_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-15 14:09:32.000000 ghga_service_commons-3.1.2/src/ghga_service_commons/utils/utc_dates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:09:36.111130 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 14:09:36.000000 ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/top_level.txt
```

### Comparing `ghga_service_commons-3.1.1/LICENSE` & `ghga_service_commons-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/PKG-INFO` & `ghga_service_commons-3.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_service_commons
-Version: 3.1.1
+Version: 3.1.2
 Summary: A library that contains common functionality used in services of GHGA
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-service-commons
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -16,26 +16,26 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: api
 Requires-Dist: fastapi<0.111,>=0.110; extra == "api"
-Requires-Dist: uvicorn[standard]<0.28,>=0.27.1; extra == "api"
+Requires-Dist: uvicorn[standard]<0.30,>=0.29; extra == "api"
 Requires-Dist: ghga-service-commons[objectstorage]; extra == "api"
 Provides-Extra: auth
-Requires-Dist: jwcrypto<2,>=1.5.4; extra == "auth"
+Requires-Dist: jwcrypto<2,>=1.5.6; extra == "auth"
 Requires-Dist: pydantic[email]<3,>=2; extra == "auth"
 Provides-Extra: crypt
-Requires-Dist: pynacl<2,>=1.5.0; extra == "crypt"
-Requires-Dist: crypt4gh<2,>=1.6.0; extra == "crypt"
+Requires-Dist: pynacl<2,>=1.5; extra == "crypt"
+Requires-Dist: crypt4gh<2,>=1.6; extra == "crypt"
 Provides-Extra: dev
-Requires-Dist: requests<3,>=2.31.0; extra == "dev"
+Requires-Dist: requests<3,>=2.31; extra == "dev"
 Provides-Extra: objectstorage
-Requires-Dist: hexkit<3,>=2; extra == "objectstorage"
+Requires-Dist: hexkit<4,>=2; extra == "objectstorage"
 Provides-Extra: all
 Requires-Dist: ghga-service-commons[api,auth,crypt,dev,objectstorage]; extra == "all"
 
 ![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/unit_and_int_tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga_service_commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga_service_commons?branch=main)
```

### Comparing `ghga_service_commons-3.1.1/README.md` & `ghga_service_commons-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/pyproject.toml` & `ghga_service_commons-3.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,42 +18,42 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: Apache Software License",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Software Development :: Libraries",
     "Intended Audience :: Developers",
 ]
 name = "ghga_service_commons"
-version = "3.1.1"
+version = "3.1.2"
 description = "A library that contains common functionality used in services of GHGA"
 dependencies = [
     "pydantic >=2, <3",
 ]
 
 [project.license]
 text = "Apache 2.0"
 
 [project.optional-dependencies]
 api = [
     "fastapi>=0.110, <0.111",
-    "uvicorn[standard]>=0.27.1, <0.28",
+    "uvicorn[standard]>=0.29, <0.30",
     "ghga-service-commons[objectstorage]",
 ]
 auth = [
-    "jwcrypto>=1.5.4, <2",
+    "jwcrypto>=1.5.6, <2",
     "pydantic[email]>=2, <3",
 ]
 crypt = [
-    "pynacl>=1.5.0, <2",
-    "crypt4gh>=1.6.0, <2",
+    "pynacl>=1.5, <2",
+    "crypt4gh>=1.6, <2",
 ]
 dev = [
-    "requests>=2.31.0, <3",
+    "requests>=2.31, <3",
 ]
 objectstorage = [
-    "hexkit>=2, <3",
+    "hexkit>=2, <4",
 ]
 all = [
     "ghga-service-commons[api,auth,crypt,dev,objectstorage]",
 ]
 
 [project.urls]
 Repository = "https://github.com/ghga-de/ghga-service-commons"
@@ -83,16 +83,17 @@
 [tool.ruff.lint]
 fixable = [
     "UP",
     "I",
     "D",
 ]
 ignore = [
-    "E",
-    "W",
+    "E111",
+    "E114",
+    "E116",
     "PLW",
     "RUF001",
     "RUF010",
     "RUF012",
     "N818",
     "B008",
     "PLR2004",
@@ -157,9 +158,9 @@
 ]
 warn_redundant_casts = true
 warn_unused_ignores = true
 check_untyped_defs = true
 no_site_packages = false
 
 [tool.pytest.ini_options]
-minversion = "7.4"
+minversion = "8.0"
 asyncio_mode = "strict"
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/__main__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/__main__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/api/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/api/api.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/api/api.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/api/di.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/api/di.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/api/mock_router.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/api/mock_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """A class for mocking API endpoints when testing with the httpx_mock fixture."""
 
+from __future__ import annotations
+
 import re
 from functools import partial
 from inspect import signature
-from typing import Any, Callable, Generic, Optional, TypeVar, cast, get_type_hints
+from typing import Any, Callable, Generic, TypeVar, cast, get_type_hints
 
 import httpx
 import pytest
 from pydantic import BaseModel
 
 from ghga_service_commons.httpyexpect.server.exceptions import HttpException
 
@@ -100,18 +102,17 @@
     The only parameter types allowed in the endpoint functions are primitives
     that can be stored in the url string: int, float, str, bool, None, and complex.
     The one exception is "request", which will be passed in automatically if specified.
     """
 
     def __init__(
         self,
-        exception_handler: Optional[
-            Callable[[httpx.Request, ExpectedExceptionTypes], Any]
-        ] = None,
-        exceptions_to_handle: Optional[tuple[type[Exception], ...]] = None,
+        exception_handler: Callable[[httpx.Request, ExpectedExceptionTypes], Any]
+        | None = None,
+        exceptions_to_handle: tuple[type[Exception], ...] | None = None,
         handle_exception_subclasses: bool = False,
     ):
         """Initialize the MockRouter with an optional exception handler.
 
         Args:
             `exception_handler`:
                 custom exception handler function that takes the request and exception
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/api/testing.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/api/testing.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/auth/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/auth/context.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Protocol for retrieving a context for authentication and authorization."""
 
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
-from typing import Generic, Optional, TypeVar
+from typing import Generic, TypeVar
 
 from pydantic import BaseModel
 
 __all__ = ["AuthContext", "AuthContextProtocol"]
 
 
 # type variable for handling different kinds of auth contexts
@@ -31,15 +33,15 @@
 class AuthContextProtocol(ABC, Generic[AuthContext]):
     """A protocol for retrieving an authentication and authorization context."""
 
     class AuthContextValidationError(RuntimeError):
         """Error that is raised when the underlying token is invalid."""
 
     @abstractmethod
-    async def get_context(self, token: str) -> Optional[AuthContext]:
+    async def get_context(self, token: str) -> AuthContext | None:
         """Derive an authentication and authorization context from a token.
 
         The protocol is independent of the underlying serialization format.
 
         Raises an AuthContextValidationError if the provided token cannot establish
         a valid authentication and authorization context.
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/auth/ghga.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/ghga.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/auth/jwt_auth.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/jwt_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,19 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """JSON web token based provider implementing the AuthContextProtocol."""
 
+from __future__ import annotations
+
 import json
 from contextlib import asynccontextmanager
-from typing import Any, Optional
+from typing import Any
 
 from jwcrypto import jwk, jwt
 from jwcrypto.common import JWException
 from pydantic import Field, ValidationError
 from pydantic_settings import BaseSettings
 
 from ghga_service_commons.auth.context import AuthContext, AuthContextProtocol
@@ -87,15 +89,15 @@
             ) from error
         self._key = key
         self._algs = config.auth_algs
         self._check_claims = config.auth_check_claims
         self._map_claims = config.auth_map_claims
         self._context_class = context_class
 
-    async def get_context(self, token: str) -> Optional[AuthContext]:
+    async def get_context(self, token: str) -> AuthContext | None:
         """Get an authentication and authorization context from a token.
 
         The token must be a serialized and signed JSON web token.
 
         Raises an AuthContextValidationError if the provided token cannot
         establish a valid authentication and authorization context.
         """
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/auth/policies.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/auth/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 #
 
 """Authentication and authorization policies that can be used with FastAPI.
 
 See the auth_demo and ghga_auth examples for how to use these policies.
 """
 
-from typing import Callable, Optional
+from __future__ import annotations
+
+from typing import Callable
 
 from fastapi.exceptions import HTTPException
 from fastapi.security import HTTPAuthorizationCredentials
 from starlette.status import HTTP_401_UNAUTHORIZED, HTTP_403_FORBIDDEN
 
 from ghga_service_commons.auth.context import AuthContext, AuthContextProtocol
 
@@ -32,15 +34,15 @@
     "require_auth_context_using_credentials",
 ]
 
 
 async def get_auth_context_using_credentials(
     credentials: HTTPAuthorizationCredentials,
     auth_provider: AuthContextProtocol[AuthContext],
-) -> Optional[AuthContext]:
+) -> AuthContext | None:
     """Get an authentication and authorization context using FastAPI.
 
     Unauthenticated access is allowed and will return None as auth context.
     """
     token = credentials.credentials if credentials else None
     if not token:
         return None
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/base_exception.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/base_exception.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/custom_types.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/custom_types.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/exceptions.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/mapping.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/mapping.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 
 """This module provides functionality for working with exception mappings.
 
 A exception mapping is a datastructure that maps an HTTP error response (4xx or 5xx)
 to a python exception.
 """
 
+from __future__ import annotations
+
 import inspect
 from collections.abc import Mapping, Sequence
-from typing import Any, NamedTuple, Optional, cast
+from typing import Any, NamedTuple, cast
 
 from ghga_service_commons.httpyexpect.client.custom_types import (
     ExceptionFactory,
     ExceptionFactoryParam,
     ExceptionId,
     ExceptionMappingSpec,
 )
@@ -101,15 +103,15 @@
             raise ValidationError(
                 f"The mapping provided for the {status_code} status code was not a"
                 + " dict (or python Mapping-compatible datastructure)."
             )
 
     @staticmethod
     def _get_error_intro(
-        status_code: Optional[int] = None, exception_id: Optional[str] = None
+        status_code: int | None = None, exception_id: str | None = None
     ):
         """Return an intro for a ValidationError.
 
         To be used only by the `inspect_factory_params` and the `check_exception_factory`
         functions.
         """
         return (
@@ -122,16 +124,16 @@
         )
 
     @classmethod
     def _inspect_factory_params(
         cls,
         factory: ExceptionFactory,
         *,
-        exception_id: Optional[str] = None,
-        status_code: Optional[int] = None,
+        exception_id: str | None = None,
+        status_code: int | None = None,
     ) -> Sequence[ExceptionFactoryParam]:
         """Inspect the parameters of the given factory.
 
         Raises:
             ValidationError: if parameters are invalid.
 
         Returns:
@@ -184,16 +186,16 @@
         )
 
     @classmethod
     def _check_exception_factory(
         cls,
         factory: object,
         *,
-        exception_id: Optional[str] = None,
-        status_code: Optional[int] = None,
+        exception_id: str | None = None,
+        status_code: int | None = None,
     ) -> None:
         """Check the signature of an exception factory."""
         if not callable(factory):
             raise ValidationError(
                 f"{cls._get_error_intro(status_code, exception_id)} was not callable."
             )
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/client/translator.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/client/translator.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Logic to translate responses to HTTP calls to python exceptions."""
 
-from typing import Optional
+from __future__ import annotations
 
 import pydantic
 
 from ghga_service_commons.httpyexpect.client.custom_types import Response
 from ghga_service_commons.httpyexpect.client.exceptions import UnstructuredError
 from ghga_service_commons.httpyexpect.client.mapping import ExceptionMapping
 from ghga_service_commons.httpyexpect.models import HttpExceptionBody
@@ -87,15 +87,15 @@
             for key, value in param_values.items()
             if key in factory_kit.required_params
         }
 
         # call the factory with the param values to get the exception:
         return factory_kit.factory(**required_param_values)
 
-    def get_error(self) -> Optional[Exception]:
+    def get_error(self) -> Exception | None:
         """Translate the response into a python exception.
 
         In case the provided response corresponds to an error, it will translate the
         response into a python exception and return it.
         Please note, this function will only return exceptions but not raise them.
 
         Returns:
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/models.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/models.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/exceptions.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/server/handlers/fastapi_.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/httpyexpect/validation.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/httpyexpect/validation.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """General purpose validation logic used by both the client and server side."""
 
+from __future__ import annotations
+
 import re
-from typing import Optional
 
 from ghga_service_commons.httpyexpect.base_exception import HttpyExpectError
 from ghga_service_commons.httpyexpect.models import EXCEPTION_ID_PATTERN
 
 
 class ValidationError(HttpyExpectError):
     """Thrown when a exception mapping spec failed validation."""
@@ -35,15 +36,15 @@
             + f" obtained: {status_code}"
         )
 
 
 def validate_exception_id(
     exception_id: object,
     *,
-    status_code: Optional[int] = None,
+    status_code: int | None = None,
 ) -> None:
     """Check the format of an exception id."""
     if not isinstance(exception_id, str) or not re.match(
         EXCEPTION_ID_PATTERN, exception_id
     ):
         raise ValidationError(
             "The exception ID must be a string formatted according to the regex"
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/__init__.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/context.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/context.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/crypt.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 """Helper functions for Crypt4GH compliant encryption."""
 
+from __future__ import annotations
+
 import base64
-from typing import NamedTuple, Union
+from typing import NamedTuple
 
 from nacl.public import PrivateKey, PublicKey, SealedBox
 
 __all__ = [
     "generate_key_pair",
     "encode_key",
     "decode_key",
@@ -71,15 +73,15 @@
         raise ValueError(str(error)) from error
     if len(decoded_key) != PublicKey.SIZE:
         raise ValueError("Invalid key")
     return decoded_key
 
 
 def decrypt(
-    data: Union[bytes, str], key: Union[bytes, str, PrivateKey], encoding: str = "utf-8"
+    data: bytes | str, key: bytes | str | PrivateKey, encoding: str = "utf-8"
 ) -> str:
     """Decrypt a base64 encoded or bytes string using a private Crypt4GH key.
 
     The result will be decoded as a native string using the given encoding.
 
     Raises a ValueError if the given key cannot be used for decryption.
     """
@@ -93,15 +95,15 @@
     if isinstance(data, str):
         data = base64.b64decode(data)
     decrypted_data = sealed_box.decrypt(data)
     return decrypted_data.decode(encoding)
 
 
 def encrypt(
-    data: str, key: Union[bytes, str, PrivateKey, PublicKey], encoding: str = "utf-8"
+    data: str, key: bytes | str | PrivateKey | PublicKey, encoding: str = "utf-8"
 ) -> str:
     """Encrypt a str with given encoding using a public Crypt4GH key.
 
     The result will be returned as a base64 encoded string.
 
     Raises a ValueError if the given key cannot be used for encryption.
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/crypt4gh.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/crypt4gh.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 """Contains utility functions to deal with Crypt4GH on a slightly higher level."""
 
+from __future__ import annotations
+
 import base64
 import io
 import os
 from functools import wraps
 from pathlib import Path
 from tempfile import mkstemp
-from typing import Callable, NamedTuple, Union
+from typing import Callable, NamedTuple, cast
 
 import crypt4gh.header
 import crypt4gh.lib
 from crypt4gh.keys import c4gh, get_private_key, get_public_key
 
 from ghga_service_commons.utils.temp_files import big_temp_file
 
@@ -83,18 +85,15 @@
         return function(**kwargs)
 
     return wrapper
 
 
 @key_secret_decoder
 def create_envelope(
-    *,
-    file_secret: Union[str, bytes],
-    private_key: Union[str, bytes],
-    public_key: Union[str, bytes],
+    *, file_secret: str | bytes, private_key: str | bytes, public_key: str | bytes
 ) -> bytes:
     """Create a new Crypt4GH header/envelope.
 
     Arguments should be passed as base64 encoded string or raw bytes.
 
     Returns:
         bytes: Crypt4GH envelope containing encrypted symmetric file secret
@@ -103,47 +102,42 @@
     header_content = crypt4gh.header.make_packet_data_enc(0, file_secret)
     header_packets = crypt4gh.header.encrypt(header_content, keys)
     return crypt4gh.header.serialize(header_packets)
 
 
 @key_secret_decoder
 def decrypt_file(
-    *,
-    input_path: Union[str, Path],
-    output_path: Union[str, Path],
-    private_key: Union[str, bytes],
+    *, input_path: str | Path, output_path: str | Path, private_key: str | bytes
 ) -> None:
     """Decrypt a Crypt4GH encrypted file.
 
     Private key should be passed as base64 encoded string or raw bytes.
     """
     keys = [(0, private_key, None)]
-    with input_path.open("rb") as infile, output_path.open("wb") as outfile:  # type: ignore[union-attr]
+    input_path, output_path = cast(tuple[Path, Path], (input_path, output_path))
+    with input_path.open("rb") as infile, output_path.open("wb") as outfile:
         crypt4gh.lib.decrypt(keys=keys, infile=infile, outfile=outfile)
 
 
 @key_secret_decoder
 def extract_file_secret(
-    *,
-    encrypted_header: Union[str, bytes],
-    private_key: Union[str, bytes],
-    public_key: Union[str, bytes],
+    *, encrypted_header: str | bytes, private_key: str | bytes, public_key: str | bytes
 ) -> bytes:
     """Extract symmetric secret from Crypt4GH header/envelope.
 
     Arguments should be passed as base64 encoded string or raw bytes.
 
     Returns:
         bytes: symmetric files secret from header.
             Only one secret is supported for now.
     """
     # (method - only 0 supported for now, private_key, public_key)
     keys = [(0, private_key, None)]
-
-    infile = io.BytesIO(encrypted_header)  # type: ignore[arg-type]
+    encrypted_header = cast(bytes, encrypted_header)
+    infile = io.BytesIO(encrypted_header)
     session_keys, _ = crypt4gh.header.deconstruct(
         infile=infile, keys=keys, sender_pubkey=public_key
     )
 
     return session_keys[0]
 
 
@@ -164,15 +158,15 @@
     Path(sk_path).unlink()
 
     return Crypt4GHKeyPair(private=private_key, public=public_key)
 
 
 @key_secret_decoder
 def random_encrypted_content(
-    file_size: int, private_key: Union[str, bytes], public_key: Union[str, bytes]
+    file_size: int, private_key: str | bytes, public_key: str | bytes
 ) -> RandomEncryptedData:
     """Create an in-memory file with random content that is Crypt4GH encrypted."""
     encrypted_file = io.BytesIO()
 
     with big_temp_file(file_size) as raw_file:
         # rewind input file for reading
         true_size = raw_file.tell()
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/files.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/files.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/jwt_helpers.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/jwt_helpers.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/multinode_storage.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/multinode_storage.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/simple_token.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/simple_token.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/temp_files.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/temp_files.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons/utils/utc_dates.py` & `ghga_service_commons-3.1.2/src/ghga_service_commons/utils/utc_dates.py`

 * *Files identical despite different names*

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/PKG-INFO` & `ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghga_service_commons
-Version: 3.1.1
+Version: 3.1.2
 Summary: A library that contains common functionality used in services of GHGA
 Author-email: "German Human Genome Phenome Archive (GHGA)" <contact@ghga.de>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/ghga-de/ghga-service-commons
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
@@ -16,26 +16,26 @@
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: api
 Requires-Dist: fastapi<0.111,>=0.110; extra == "api"
-Requires-Dist: uvicorn[standard]<0.28,>=0.27.1; extra == "api"
+Requires-Dist: uvicorn[standard]<0.30,>=0.29; extra == "api"
 Requires-Dist: ghga-service-commons[objectstorage]; extra == "api"
 Provides-Extra: auth
-Requires-Dist: jwcrypto<2,>=1.5.4; extra == "auth"
+Requires-Dist: jwcrypto<2,>=1.5.6; extra == "auth"
 Requires-Dist: pydantic[email]<3,>=2; extra == "auth"
 Provides-Extra: crypt
-Requires-Dist: pynacl<2,>=1.5.0; extra == "crypt"
-Requires-Dist: crypt4gh<2,>=1.6.0; extra == "crypt"
+Requires-Dist: pynacl<2,>=1.5; extra == "crypt"
+Requires-Dist: crypt4gh<2,>=1.6; extra == "crypt"
 Provides-Extra: dev
-Requires-Dist: requests<3,>=2.31.0; extra == "dev"
+Requires-Dist: requests<3,>=2.31; extra == "dev"
 Provides-Extra: objectstorage
-Requires-Dist: hexkit<3,>=2; extra == "objectstorage"
+Requires-Dist: hexkit<4,>=2; extra == "objectstorage"
 Provides-Extra: all
 Requires-Dist: ghga-service-commons[api,auth,crypt,dev,objectstorage]; extra == "all"
 
 ![tests](https://github.com/ghga-de/ghga-service-commons/actions/workflows/unit_and_int_tests.yaml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/ghga_service_commons.svg)](https://pypi.python.org/pypi/ghga_service_commons/)
 [![Coverage Status](https://coveralls.io/repos/github/ghga-de/ghga_service_commons/badge.svg?branch=main)](https://coveralls.io/github/ghga-de/ghga_service_commons?branch=main)
```

### Comparing `ghga_service_commons-3.1.1/src/ghga_service_commons.egg-info/SOURCES.txt` & `ghga_service_commons-3.1.2/src/ghga_service_commons.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 src/ghga_service_commons/__init__.py
 src/ghga_service_commons/__main__.py
+src/ghga_service_commons/py.typed
 src/ghga_service_commons.egg-info/PKG-INFO
 src/ghga_service_commons.egg-info/SOURCES.txt
 src/ghga_service_commons.egg-info/dependency_links.txt
 src/ghga_service_commons.egg-info/requires.txt
 src/ghga_service_commons.egg-info/top_level.txt
 src/ghga_service_commons/api/__init__.py
 src/ghga_service_commons/api/api.py
```

