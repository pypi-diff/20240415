# Comparing `tmp/protoplasm-5.0.0b1.tar.gz` & `tmp/protoplasm-5.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protoplasm-5.0.0b1.tar", last modified: Mon Apr 15 14:58:01 2024, max compression
+gzip compressed data, was "protoplasm-5.0.0b2.tar", last modified: Mon Apr 15 15:26:39 2024, max compression
```

## Comparing `protoplasm-5.0.0b1.tar` & `protoplasm-5.0.0b2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.832949 protoplasm-5.0.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-15 14:58:01.832949 protoplasm-5.0.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.820949 protoplasm-5.0.0b1/protoplasm/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.824949 protoplasm-5.0.0b1/protoplasm/bases/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/_exwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/_methwrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/_remotewrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/_servicer.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/dataclass_bases.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/bases/grpc_bases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.824949 protoplasm-5.0.0b1/protoplasm/casting/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/casting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/casting/casters.py
--rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/casting/castutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/casting/dictator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.824949 protoplasm-5.0.0b1/protoplasm/casting/dictators/
--rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/casting/dictators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/casting/objectifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.828949 protoplasm-5.0.0b1/protoplasm/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/decorators/apihelpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.828949 protoplasm-5.0.0b1/protoplasm/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/errors/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/errors/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/grpcserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.828949 protoplasm-5.0.0b1/protoplasm/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/loader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.828949 protoplasm-5.0.0b1/protoplasm/plasm/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/plasm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.828949 protoplasm-5.0.0b1/protoplasm/structs/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.832949 protoplasm-5.0.0b1/protoplasm/structs/_ctx/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_ctx/_basectx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_ctx/_grpcctx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_methodtype.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_reqestsiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/_responseiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/protoplasm/structs/dataclassbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.832949 protoplasm-5.0.0b1/protoplasm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-15 14:58:01.000000 protoplasm-5.0.0b1/protoplasm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-15 14:58:01.000000 protoplasm-5.0.0b1/protoplasm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:58:01.000000 protoplasm-5.0.0b1/protoplasm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 14:58:01.000000 protoplasm-5.0.0b1/protoplasm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:58:01.832949 protoplasm-5.0.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:01.832949 protoplasm-5.0.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    24968 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_casting.py
--rw-r--r--   0 runner    (1001) docker     (127)    47379 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_castutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_dictator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14734 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_dictators.py
--rw-r--r--   0 runner    (1001) docker     (127)    33341 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_objectifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    13502 2024-04-15 14:57:52.000000 protoplasm-5.0.0b1/tests/test_services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.974471 protoplasm-5.0.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-15 15:26:39.974471 protoplasm-5.0.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.962471 protoplasm-5.0.0b2/protoplasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.966471 protoplasm-5.0.0b2/protoplasm/bases/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/_exwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/_methwrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9854 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/_remotewrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/_servicer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/dataclass_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/bases/grpc_bases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.966471 protoplasm-5.0.0b2/protoplasm/casting/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/casting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/casting/casters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15536 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/casting/castutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/casting/dictator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.966471 protoplasm-5.0.0b2/protoplasm/casting/dictators/
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/casting/dictators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/casting/objectifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.966471 protoplasm-5.0.0b2/protoplasm/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/decorators/apihelpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.966471 protoplasm-5.0.0b2/protoplasm/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/errors/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/errors/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/grpcserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.970471 protoplasm-5.0.0b2/protoplasm/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/loader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.970471 protoplasm-5.0.0b2/protoplasm/plasm/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/plasm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.970471 protoplasm-5.0.0b2/protoplasm/structs/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.970471 protoplasm-5.0.0b2/protoplasm/structs/_ctx/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_ctx/_basectx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_ctx/_grpcctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_methodtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_reqestsiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6651 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/_responseiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/protoplasm/structs/dataclassbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.974471 protoplasm-5.0.0b2/protoplasm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-15 15:26:39.000000 protoplasm-5.0.0b2/protoplasm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-15 15:26:39.000000 protoplasm-5.0.0b2/protoplasm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:26:39.000000 protoplasm-5.0.0b2/protoplasm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 15:26:39.000000 protoplasm-5.0.0b2/protoplasm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 15:26:39.000000 protoplasm-5.0.0b2/protoplasm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:26:39.974471 protoplasm-5.0.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:26:39.974471 protoplasm-5.0.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24968 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47379 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_castutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6037 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_dictator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14734 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_dictators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33341 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_objectifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13502 2024-04-15 15:26:28.000000 protoplasm-5.0.0b2/tests/test_services.py
```

### Comparing `protoplasm-5.0.0b1/LICENSE` & `protoplasm-5.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/PKG-INFO` & `protoplasm-5.0.0b2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoplasm
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: Utilities for working with Protobuf & gRPC in Python.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Daniel Maxson <dmaxson@ccpgames.com>, John Aldis <johnaldis@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ccptools<2,>=1.1
+Requires-Dist: protobuf<5,>=4.25.3
+Requires-Dist: grpcio<2,>=1.62.1
+Requires-Dist: grpcio-tools<2,>=1.62.1
+Requires-Dist: googleapis-common-protos<2,>=1.63.0
 
 # Protoplasm
 
 Utilities for working with Protobuf & gRPC in Python, e.g; compiling Python 3 
 Dataclasses from compiled proto-message-python code and casting between the two,
 quickly initializing large/nested Protobuf object, simplifying gRPC service 
 interfaces etc.
```

### Comparing `protoplasm-5.0.0b1/README.md` & `protoplasm-5.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/bases/_client.py` & `protoplasm-5.0.0b2/protoplasm/bases/_client.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/bases/_exwrap.py` & `protoplasm-5.0.0b2/protoplasm/bases/_exwrap.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/bases/_methwrap.py` & `protoplasm-5.0.0b2/protoplasm/bases/_methwrap.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/bases/_remotewrap.py` & `protoplasm-5.0.0b2/protoplasm/bases/_remotewrap.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/bases/_servicer.py` & `protoplasm-5.0.0b2/protoplasm/bases/_servicer.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/casting/casters.py` & `protoplasm-5.0.0b2/protoplasm/casting/casters.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/casting/castutils.py` & `protoplasm-5.0.0b2/protoplasm/casting/castutils.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/casting/dictator.py` & `protoplasm-5.0.0b2/protoplasm/casting/dictator.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/casting/dictators/__init__.py` & `protoplasm-5.0.0b2/protoplasm/casting/dictators/__init__.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/casting/objectifier.py` & `protoplasm-5.0.0b2/protoplasm/casting/objectifier.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/decorators/apihelpers.py` & `protoplasm-5.0.0b2/protoplasm/decorators/apihelpers.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/errors/_api.py` & `protoplasm-5.0.0b2/protoplasm/errors/_api.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/errors/_base.py` & `protoplasm-5.0.0b2/protoplasm/errors/_base.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/grpcserver.py` & `protoplasm-5.0.0b2/protoplasm/grpcserver.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/loader/__init__.py` & `protoplasm-5.0.0b2/protoplasm/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/structs/_ctx/_basectx.py` & `protoplasm-5.0.0b2/protoplasm/structs/_ctx/_basectx.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/structs/_ctx/_grpcctx.py` & `protoplasm-5.0.0b2/protoplasm/structs/_ctx/_grpcctx.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/structs/_methodtype.py` & `protoplasm-5.0.0b2/protoplasm/structs/_methodtype.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/structs/_reqestsiter.py` & `protoplasm-5.0.0b2/protoplasm/structs/_reqestsiter.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/structs/_responseiter.py` & `protoplasm-5.0.0b2/protoplasm/structs/_responseiter.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm/structs/dataclassbase.py` & `protoplasm-5.0.0b2/protoplasm/structs/dataclassbase.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/protoplasm.egg-info/PKG-INFO` & `protoplasm-5.0.0b2/protoplasm.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protoplasm
-Version: 5.0.0b1
+Version: 5.0.0b2
 Summary: Utilities for working with Protobuf & gRPC in Python.
 Author-email: Thordur Matthiasson <thordurm@ccpgames.com>, Daniel Maxson <dmaxson@ccpgames.com>, John Aldis <johnaldis@ccpgames.com>
 License: MIT License
         
         Copyright (c) 2019-2024 CCP Games
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,14 +43,19 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ccptools<2,>=1.1
+Requires-Dist: protobuf<5,>=4.25.3
+Requires-Dist: grpcio<2,>=1.62.1
+Requires-Dist: grpcio-tools<2,>=1.62.1
+Requires-Dist: googleapis-common-protos<2,>=1.63.0
 
 # Protoplasm
 
 Utilities for working with Protobuf & gRPC in Python, e.g; compiling Python 3 
 Dataclasses from compiled proto-message-python code and casting between the two,
 quickly initializing large/nested Protobuf object, simplifying gRPC service 
 interfaces etc.
```

### Comparing `protoplasm-5.0.0b1/protoplasm.egg-info/SOURCES.txt` & `protoplasm-5.0.0b2/protoplasm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 protoplasm/__init__.py
 protoplasm/grpcserver.py
 protoplasm.egg-info/PKG-INFO
 protoplasm.egg-info/SOURCES.txt
 protoplasm.egg-info/dependency_links.txt
+protoplasm.egg-info/requires.txt
 protoplasm.egg-info/top_level.txt
 protoplasm/bases/__init__.py
 protoplasm/bases/_client.py
 protoplasm/bases/_exwrap.py
 protoplasm/bases/_methwrap.py
 protoplasm/bases/_remotewrap.py
 protoplasm/bases/_servicer.py
```

### Comparing `protoplasm-5.0.0b1/pyproject.toml` & `protoplasm-5.0.0b2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -31,14 +31,22 @@
 
     "Topic :: Software Development",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities"
 ]
 
+dependencies = [
+    "ccptools >= 1.1, <2",
+    "protobuf >=4.25.3, <5",
+    "grpcio >=1.62.1, <2",
+    "grpcio-tools >=1.62.1, <2",
+    "googleapis-common-protos >=1.63.0, <2"
+]
+
 [project.urls]
 Homepage = "https://github.com/ccpgames/protoplasm"
 Documentation = "https://github.com/ccpgames/protoplasm/blob/main/README.md"
 Repository = "https://github.com/ccpgames/protoplasm.git"
 Issues = "https://github.com/ccpgames/protoplasm/issues"
 Changelog = "https://github.com/ccpgames/protoplasm/blob/main/CHANGELOG.md"
```

### Comparing `protoplasm-5.0.0b1/tests/test_casting.py` & `protoplasm-5.0.0b2/tests/test_casting.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/tests/test_castutils.py` & `protoplasm-5.0.0b2/tests/test_castutils.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/tests/test_dataclasses.py` & `protoplasm-5.0.0b2/tests/test_dataclasses.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/tests/test_dictator.py` & `protoplasm-5.0.0b2/tests/test_dictator.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/tests/test_dictators.py` & `protoplasm-5.0.0b2/tests/test_dictators.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/tests/test_objectifier.py` & `protoplasm-5.0.0b2/tests/test_objectifier.py`

 * *Files identical despite different names*

### Comparing `protoplasm-5.0.0b1/tests/test_services.py` & `protoplasm-5.0.0b2/tests/test_services.py`

 * *Files identical despite different names*

