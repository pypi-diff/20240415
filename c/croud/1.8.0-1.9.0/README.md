# Comparing `tmp/croud-1.8.0.tar.gz` & `tmp/croud-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "croud-1.8.0.tar", last modified: Tue Nov  7 14:30:43 2023, max compression
+gzip compressed data, was "croud-1.9.0.tar", last modified: Tue Dec  5 16:08:38 2023, max compression
```

## Comparing `croud-1.8.0.tar` & `croud-1.9.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.350773 croud-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2023-11-07 14:30:39.000000 croud-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-11-07 14:30:43.350773 croud-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-11-07 14:30:39.000000 croud-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.338773 croud-1.8.0/croud/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-11-07 14:30:39.000000 croud-1.8.0/croud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    60960 2023-11-07 14:30:39.000000 croud-1.8.0/croud/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7616 2023-11-07 14:30:39.000000 croud-1.8.0/croud/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.338773 croud-1.8.0/croud/apikeys/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/apikeys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-11-07 14:30:39.000000 croud-1.8.0/croud/apikeys/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.338773 croud-1.8.0/croud/clusters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30184 2023-11-07 14:30:39.000000 croud-1.8.0/croud/clusters/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-07 14:30:39.000000 croud-1.8.0/croud/clusters/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/config/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-11-07 14:30:39.000000 croud-1.8.0/croud/config/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/consumers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/consumers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-11-07 14:30:39.000000 croud-1.8.0/croud/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-11-07 14:30:39.000000 croud-1.8.0/croud/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-11-07 14:30:39.000000 croud-1.8.0/croud/me.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/organizations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/organizations/auditlogs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/organizations/auditlogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-11-07 14:30:39.000000 croud-1.8.0/croud/organizations/auditlogs/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2023-11-07 14:30:39.000000 croud-1.8.0/croud/organizations/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/organizations/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/organizations/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-11-07 14:30:39.000000 croud-1.8.0/croud/organizations/users/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-11-07 14:30:39.000000 croud-1.8.0/croud/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2023-11-07 14:30:39.000000 croud-1.8.0/croud/printer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/products/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-07 14:30:39.000000 croud-1.8.0/croud/products/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/projects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-07 14:30:39.000000 croud-1.8.0/croud/projects/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/projects/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/projects/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-11-07 14:30:39.000000 croud-1.8.0/croud/projects/users/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.342773 croud-1.8.0/croud/regions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5334 2023-11-07 14:30:39.000000 croud-1.8.0/croud/regions/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-11-07 14:30:39.000000 croud-1.8.0/croud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.346773 croud-1.8.0/croud/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-11-07 14:30:39.000000 croud-1.8.0/croud/subscriptions/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.346773 croud-1.8.0/croud/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-11-07 14:30:39.000000 croud-1.8.0/croud/tools/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-11-07 14:30:39.000000 croud-1.8.0/croud/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.346773 croud-1.8.0/croud/users/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-11-07 14:30:39.000000 croud-1.8.0/croud/users/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.346773 croud-1.8.0/croud/users/roles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/croud/users/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-11-07 14:30:39.000000 croud-1.8.0/croud/users/roles/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2023-11-07 14:30:39.000000 croud-1.8.0/croud/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.338773 croud-1.8.0/croud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-11-07 14:30:43.000000 croud-1.8.0/croud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-11-07 14:30:43.000000 croud-1.8.0/croud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-07 14:30:43.000000 croud-1.8.0/croud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-07 14:30:43.000000 croud-1.8.0/croud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-11-07 14:30:43.000000 croud-1.8.0/croud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-07 14:30:43.000000 croud-1.8.0/croud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-11-07 14:30:43.350773 croud-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2023-11-07 14:30:39.000000 croud-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.346773 croud-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.350773 croud-1.8.0/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_api_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)    56252 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_me.py
--rw-r--r--   0 runner    (1001) docker     (127)    15275 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_products.py
--rw-r--r--   0 runner    (1001) docker     (127)     8935 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2023-11-07 14:30:39.000000 croud-1.8.0/tests/commands/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-11-07 14:30:39.000000 croud-1.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_config_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6888 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7322 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8140 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2023-11-07 14:30:39.000000 croud-1.8.0/tests/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-07 14:30:43.350773 croud-1.8.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-11-07 14:30:39.000000 croud-1.8.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2023-11-07 14:30:39.000000 croud-1.8.0/tests/util/fake_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.646308 croud-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2023-12-05 16:08:34.000000 croud-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-12-05 16:08:38.646308 croud-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2023-12-05 16:08:34.000000 croud-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.630308 croud-1.9.0/croud/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-05 16:08:34.000000 croud-1.9.0/croud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65371 2023-12-05 16:08:34.000000 croud-1.9.0/croud/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7616 2023-12-05 16:08:34.000000 croud-1.9.0/croud/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.634308 croud-1.9.0/croud/apikeys/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/apikeys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-12-05 16:08:34.000000 croud-1.9.0/croud/apikeys/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.634308 croud-1.9.0/croud/clusters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30184 2023-12-05 16:08:34.000000 croud-1.9.0/croud/clusters/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-12-05 16:08:34.000000 croud-1.9.0/croud/clusters/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.634308 croud-1.9.0/croud/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2023-12-05 16:08:34.000000 croud-1.9.0/croud/config/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.634308 croud-1.9.0/croud/consumers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/consumers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-12-05 16:08:34.000000 croud-1.9.0/croud/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2023-12-05 16:08:34.000000 croud-1.9.0/croud/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2023-12-05 16:08:34.000000 croud-1.9.0/croud/me.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/organizations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/organizations/auditlogs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/organizations/auditlogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2023-12-05 16:08:34.000000 croud-1.9.0/croud/organizations/auditlogs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11624 2023-12-05 16:08:34.000000 croud-1.9.0/croud/organizations/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/organizations/users/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/organizations/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2023-12-05 16:08:34.000000 croud-1.9.0/croud/organizations/users/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-05 16:08:34.000000 croud-1.9.0/croud/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2023-12-05 16:08:34.000000 croud-1.9.0/croud/printer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/products/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-12-05 16:08:34.000000 croud-1.9.0/croud/products/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/projects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-12-05 16:08:34.000000 croud-1.9.0/croud/projects/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/projects/users/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/projects/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-12-05 16:08:34.000000 croud-1.9.0/croud/projects/users/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/regions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5334 2023-12-05 16:08:34.000000 croud-1.9.0/croud/regions/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-12-05 16:08:34.000000 croud-1.9.0/croud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-12-05 16:08:34.000000 croud-1.9.0/croud/subscriptions/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2023-12-05 16:08:34.000000 croud-1.9.0/croud/tools/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-12-05 16:08:34.000000 croud-1.9.0/croud/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/users/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-05 16:08:34.000000 croud-1.9.0/croud/users/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.638308 croud-1.9.0/croud/users/roles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/croud/users/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-12-05 16:08:34.000000 croud-1.9.0/croud/users/roles/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2023-12-05 16:08:34.000000 croud-1.9.0/croud/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.646308 croud-1.9.0/croud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-12-05 16:08:38.000000 croud-1.9.0/croud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-12-05 16:08:38.000000 croud-1.9.0/croud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 16:08:38.000000 croud-1.9.0/croud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-05 16:08:38.000000 croud-1.9.0/croud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-05 16:08:38.000000 croud-1.9.0/croud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-05 16:08:38.000000 croud-1.9.0/croud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-05 16:08:38.646308 croud-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2023-12-05 16:08:34.000000 croud-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.642308 croud-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.646308 croud-1.9.0/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56252 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20021 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_products.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8935 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2023-12-05 16:08:34.000000 croud-1.9.0/tests/commands/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-05 16:08:34.000000 croud-1.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_config_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7322 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2023-12-05 16:08:34.000000 croud-1.9.0/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:08:38.646308 croud-1.9.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-12-05 16:08:34.000000 croud-1.9.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2023-12-05 16:08:34.000000 croud-1.9.0/tests/util/fake_cloud.py
```

### Comparing `croud-1.8.0/LICENSE` & `croud-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/PKG-INFO` & `croud-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croud
-Version: 1.8.0
+Version: 1.9.0
 Summary: A command line interface for CrateDB Cloud
 Home-page: https://github.com/crate/croud
 Author: Crate.io
 Author-email: office@crate.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Requires-Dist: bitmath==1.3.3.1
 Requires-Dist: certifi
 Requires-Dist: colorama==0.4.6
 Requires-Dist: marshmallow==3.20.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: tabulate<1.0,>=0.8
-Requires-Dist: yarl==1.9.2
+Requires-Dist: yarl==1.9.3
 Requires-Dist: halo==0.0.31
 Requires-Dist: shtab==1.6.4
 Requires-Dist: tqdm==4.66.1
 Provides-Extra: testing
 Requires-Dist: tox==3.14.2; extra == "testing"
 Requires-Dist: pytest-freezegun==0.4.2; extra == "testing"
 Provides-Extra: development
```

### Comparing `croud-1.8.0/README.rst` & `croud-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/__init__.py` & `croud-1.9.0/croud/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/__main__.py` & `croud-1.9.0/croud/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,18 @@
     config_show,
 )
 from croud.login import login
 from croud.logout import logout
 from croud.me import me, me_edit
 from croud.organizations.auditlogs.commands import auditlogs_list
 from croud.organizations.commands import (
+    org_credits_create,
+    org_credits_edit,
+    org_credits_expire,
+    org_credits_list,
     org_files_create,
     org_files_delete,
     org_files_get,
     org_files_list,
     org_secrets_create,
     org_secrets_delete,
     org_secrets_list,
@@ -1202,14 +1206,100 @@
                                 "--file-id", type=str, required=True,
                                 help="The ID of the file.",
                             ),
                         ],
                         "resolver": org_files_delete,
                     },
                 }
+            },
+            "credits": {
+                "help": "Manage organization's credits.",
+                "commands" : {
+                    "list": {
+                        "help": "Lists all credits of an organization.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--status", type=str, required=False,
+                                help="Filter credits by status, comma separated. Valid "
+                                     "values are ``ACTIVE`` and ``EXPIRED``. By "
+                                     "default only ``ACTIVE`` credits are listed.",
+                            ),
+                        ],
+                        "resolver": org_credits_list,
+                    },
+                    "create": {
+                        "help": "Creates a new credit for the specified organization.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--amount", type=float, required=True,
+                                help="The amount to be credited in USD.",
+                            ),
+                            Argument(
+                                "--expiration-date", type=str, required=True,
+                                help="The expiration date of the credit in ISO 8601 "
+                                     "format (i.e. ``2024-01-01T10:00:00Z``).",
+                            ),
+                            Argument(
+                                "--comment", type=str, required=True,
+                                help="The reason for creating this credit.",
+                            ),
+                        ],
+                        "resolver": org_credits_create,
+                    },
+                    "edit": {
+                        "help": "Edits the specified credit.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--credit-id", type=str, required=True,
+                                help="The credit ID to use.",
+                            ),
+                            Argument(
+                                "--amount", type=float, required=False,
+                                help="The amount to be credited in USD. It can only be "
+                                     "increased.",
+                            ),
+                            Argument(
+                                "--expiration-date", type=str, required=False,
+                                help="The expiration date of the credit in ISO 8601 "
+                                     "format (i.e. ``2024-01-01T10:00:00Z``).",
+                            ),
+                            Argument(
+                                "--comment", type=str, required=False,
+                                help="The reason for creating this credit.",
+                            ),
+                        ],
+                        "resolver": org_credits_edit,
+                    },
+                    "expire": {
+                        "help": "Expires the specified credit.",
+                        "extra_args": [
+                            Argument(
+                                "--org-id", type=str, required=True,
+                                help="The organization ID to use.",
+                            ),
+                            Argument(
+                                "--credit-id", type=str, required=True,
+                                help="The credit ID to use.",
+                            ),
+                        ],
+                        "resolver": org_credits_expire,
+                    },
+                }
             }
         },
     },
     "users": {
         "help": "Manage users.",
         "commands": {
             "list": {
```

### Comparing `croud-1.8.0/croud/api.py` & `croud-1.9.0/croud/api.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/apikeys/commands.py` & `croud-1.9.0/croud/apikeys/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/clusters/commands.py` & `croud-1.9.0/croud/clusters/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/clusters/exceptions.py` & `croud-1.9.0/croud/clusters/exceptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/__init__.py` & `croud-1.9.0/croud/config/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/commands.py` & `croud-1.9.0/croud/config/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/configuration.py` & `croud-1.9.0/croud/config/configuration.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/exceptions.py` & `croud-1.9.0/croud/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/schemas.py` & `croud-1.9.0/croud/config/schemas.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/types.py` & `croud-1.9.0/croud/config/types.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/config/util.py` & `croud-1.9.0/croud/config/util.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/login.py` & `croud-1.9.0/croud/login.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/logout.py` & `croud-1.9.0/croud/logout.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/me.py` & `croud-1.9.0/croud/me.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/organizations/auditlogs/commands.py` & `croud-1.9.0/croud/organizations/auditlogs/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/organizations/commands.py` & `croud-1.9.0/croud/organizations/commands.py`

 * *Files 19% similar despite different names*

```diff
@@ -259,7 +259,115 @@
     )
 
 
 def _transform_file_size(size_bytes):
     if not size_bytes:
         return None
     return bitmath.Byte(size_bytes).best_prefix().format("{value:.2f} {unit}")
+
+
+def org_credits_create(args: Namespace) -> None:
+    client = Client.from_args(args)
+    payload = {
+        "amount": int(args.amount * 100),
+        "expiration_date": args.expiration_date,
+        "comment": args.comment,
+    }
+    data, errors = client.post(
+        f"/api/v2/organizations/{args.org_id}/credits/", body=payload
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        keys=[
+            "id",
+            "original_amount",
+            "expiration_date",
+            "comment",
+            "status",
+        ],
+        success_message="Credit created.",
+        output_fmt=get_output_format(args),
+        transforms={
+            "original_amount": _transform_credits_amount_to_usd,
+        },
+    )
+
+
+def org_credits_edit(args: Namespace) -> None:
+    client = Client.from_args(args)
+    payload = {}
+    if getattr(args, "amount") is not None:
+        payload["amount"] = int(args.amount * 100)
+    if args.expiration_date:
+        payload["expiration_date"] = args.expiration_date
+    if args.comment:
+        payload["comment"] = args.comment
+    if not payload:
+        print_error("No input arguments found.")
+        exit(1)
+
+    data, errors = client.patch(
+        f"/api/v2/organizations/{args.org_id}/credits/{args.credit_id}/", body=payload
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        keys=[
+            "id",
+            "original_amount",
+            "expiration_date",
+            "comment",
+            "status",
+        ],
+        output_fmt=get_output_format(args),
+        success_message="Credit edited.",
+        transforms={
+            "original_amount": _transform_credits_amount_to_usd,
+        },
+    )
+
+
+def org_credits_list(args: Namespace) -> None:
+    client = Client.from_args(args)
+    options = {}
+    if args.status:
+        options["status"] = args.status
+    data, errors = client.get(
+        f"/api/v2/organizations/{args.org_id}/credits/", params=options
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        keys=[
+            "id",
+            "original_amount",
+            "remaining_amount",
+            "expiration_date",
+            "comment",
+            "status",
+        ],
+        output_fmt=get_output_format(args),
+        transforms={
+            "original_amount": _transform_credits_amount_to_usd,
+            "remaining_amount": _transform_credits_amount_to_usd,
+        },
+    )
+
+
+def _transform_credits_amount_to_usd(amount_cents):
+    if not amount_cents:
+        return 0
+    return f"${round(amount_cents / 100, 2)}"
+
+
+def org_credits_expire(args: Namespace) -> None:
+    client = Client.from_args(args)
+    data, errors = client.delete(
+        f"/api/v2/organizations/{args.org_id}/credits/{args.credit_id}/"
+    )
+    print_response(
+        data=data,
+        errors=errors,
+        success_message="Credit expired.",
+        output_fmt=get_output_format(args),
+    )
```

### Comparing `croud-1.8.0/croud/organizations/users/commands.py` & `croud-1.9.0/croud/organizations/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/parser.py` & `croud-1.9.0/croud/parser.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/printer.py` & `croud-1.9.0/croud/printer.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/products/commands.py` & `croud-1.9.0/croud/products/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/projects/commands.py` & `croud-1.9.0/croud/projects/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/projects/users/commands.py` & `croud-1.9.0/croud/projects/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/regions/commands.py` & `croud-1.9.0/croud/regions/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/server.py` & `croud-1.9.0/croud/server.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/subscriptions/commands.py` & `croud-1.9.0/croud/subscriptions/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/typing.py` & `croud-1.9.0/croud/typing.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/users/commands.py` & `croud-1.9.0/croud/users/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/users/roles/commands.py` & `croud-1.9.0/croud/users/roles/commands.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud/util.py` & `croud-1.9.0/croud/util.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/croud.egg-info/PKG-INFO` & `croud-1.9.0/croud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: croud
-Version: 1.8.0
+Version: 1.9.0
 Summary: A command line interface for CrateDB Cloud
 Home-page: https://github.com/crate/croud
 Author: Crate.io
 Author-email: office@crate.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Requires-Dist: bitmath==1.3.3.1
 Requires-Dist: certifi
 Requires-Dist: colorama==0.4.6
 Requires-Dist: marshmallow==3.20.1
 Requires-Dist: pyyaml==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: tabulate<1.0,>=0.8
-Requires-Dist: yarl==1.9.2
+Requires-Dist: yarl==1.9.3
 Requires-Dist: halo==0.0.31
 Requires-Dist: shtab==1.6.4
 Requires-Dist: tqdm==4.66.1
 Provides-Extra: testing
 Requires-Dist: tox==3.14.2; extra == "testing"
 Requires-Dist: pytest-freezegun==0.4.2; extra == "testing"
 Provides-Extra: development
```

### Comparing `croud-1.8.0/croud.egg-info/SOURCES.txt` & `croud-1.9.0/croud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/setup.py` & `croud-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 from pkg_resources.extern.packaging.version import Version
 from setuptools import find_packages, setup
 
-__version__ = Version("1.8.0")
+__version__ = Version("1.9.0")
 
 try:
     with open("README.rst", "r", encoding="utf-8") as f:
         readme = f.read()
 except IOError:
     readme = ""
 
@@ -46,15 +46,15 @@
         "bitmath==1.3.3.1",
         "certifi",
         "colorama==0.4.6",
         "marshmallow==3.20.1",
         "pyyaml==6.0.1",
         "requests==2.31.0",
         "tabulate>=0.8,<1.0",
-        "yarl==1.9.2",
+        "yarl==1.9.3",
         "halo==0.0.31",
         "shtab==1.6.4",
         "tqdm==4.66.1",
     ],
     extras_require={
         "testing": [
             "tox==3.14.2",
```

### Comparing `croud-1.8.0/tests/commands/test_api_keys.py` & `croud-1.9.0/tests/commands/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_clusters.py` & `croud-1.9.0/tests/commands/test_clusters.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_config.py` & `croud-1.9.0/tests/commands/test_config.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_login.py` & `croud-1.9.0/tests/commands/test_login.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_logout.py` & `croud-1.9.0/tests/commands/test_logout.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_me.py` & `croud-1.9.0/tests/commands/test_me.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_organizations.py` & `croud-1.9.0/tests/commands/test_organizations.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # under the License.
 #
 # However, if you have executed another commercial license agreement
 # with Crate these terms will supersede the license and you may use the
 # software solely pursuant to the terms of the relevant commercial agreement.
 
 import uuid
+from datetime import datetime, timedelta
 from unittest import mock
 
 import pytest
 
 from croud.api import Client, RequestMethod
 from croud.organizations.users.commands import (
     role_fqn_transform as organization_role_fqn_transform,
@@ -513,7 +514,194 @@
         "my_secret_id",
     )
     assert_rest(
         mock_request,
         RequestMethod.DELETE,
         f"/api/v2/organizations/{org_id}/secrets/my_secret_id/",
     )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_list(mock_request):
+    org_id = gen_uuid()
+
+    call_command("croud", "organizations", "credits", "list", "--org-id", org_id)
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        f"/api/v2/organizations/{org_id}/credits/",
+        params={},
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_list_filter_status(mock_request):
+    org_id = gen_uuid()
+
+    call_command(
+        "croud",
+        "organizations",
+        "credits",
+        "list",
+        "--org-id",
+        org_id,
+        "--status",
+        "ACTIVE,EXPIRED",
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.GET,
+        f"/api/v2/organizations/{org_id}/credits/",
+        params={"status": "ACTIVE,EXPIRED"},
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_create(mock_request):
+    org_id = gen_uuid()
+    amount = 123.45
+    expiration_date = datetime.utcnow() + timedelta(days=30)
+    comment = "Free Trial"
+
+    call_command(
+        "croud",
+        "organizations",
+        "credits",
+        "create",
+        "--org-id",
+        org_id,
+        "--amount",
+        str(amount),
+        "--expiration-date",
+        expiration_date.isoformat(),
+        "--comment",
+        comment,
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.POST,
+        f"/api/v2/organizations/{org_id}/credits/",
+        body={
+            "amount": amount * 100,
+            "expiration_date": expiration_date.isoformat(),
+            "comment": comment,
+        },
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_expire(mock_request):
+    org_id = gen_uuid()
+
+    call_command(
+        "croud",
+        "organizations",
+        "credits",
+        "expire",
+        "--org-id",
+        org_id,
+        "--credit-id",
+        "my_credit_id",
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.DELETE,
+        f"/api/v2/organizations/{org_id}/credits/my_credit_id/",
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_edit(mock_request):
+    org_id = gen_uuid()
+    expiration_date = datetime.utcnow() + timedelta(days=60)
+    call_command(
+        "croud",
+        "organizations",
+        "credits",
+        "edit",
+        "--org-id",
+        org_id,
+        "--credit-id",
+        "my_credit_id",
+        "--amount",
+        str(234.56),
+        "--expiration-date",
+        expiration_date.isoformat(),
+        "--comment",
+        "Starter Package",
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.PATCH,
+        f"/api/v2/organizations/{org_id}/credits/my_credit_id/",
+        body={
+            "amount": 23456,
+            "expiration_date": expiration_date.isoformat(),
+            "comment": "Starter Package",
+        },
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_edit_amount(mock_request):
+    org_id = gen_uuid()
+    call_command(
+        "croud",
+        "organizations",
+        "credits",
+        "edit",
+        "--org-id",
+        org_id,
+        "--credit-id",
+        "my_credit_id",
+        "--amount",
+        str(234.56),
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.PATCH,
+        f"/api/v2/organizations/{org_id}/credits/my_credit_id/",
+        body={"amount": 23456},
+    )
+
+
+@mock.patch.object(Client, "request", return_value=({}, None))
+def test_organizations_credits_edit_expiration_date(mock_request):
+    org_id = gen_uuid()
+    expiration_date = datetime.utcnow() + timedelta(days=60)
+    call_command(
+        "croud",
+        "organizations",
+        "credits",
+        "edit",
+        "--org-id",
+        org_id,
+        "--credit-id",
+        "my_credit_id",
+        "--expiration-date",
+        expiration_date.isoformat(),
+    )
+    assert_rest(
+        mock_request,
+        RequestMethod.PATCH,
+        f"/api/v2/organizations/{org_id}/credits/my_credit_id/",
+        body={"expiration_date": expiration_date.isoformat()},
+    )
+
+
+@mock.patch.object(Client, "request", return_value=(None, {}))
+def test_organizations_credits_edit_no_arguments(mock_request, capsys):
+    org_id = gen_uuid()
+    with pytest.raises(SystemExit):
+        call_command(
+            "croud",
+            "organizations",
+            "credits",
+            "edit",
+            "--org-id",
+            org_id,
+            "--credit-id",
+            "my_credit_id",
+        )
+
+    _, err = capsys.readouterr()
+    assert "No input arguments found." in err
```

### Comparing `croud-1.8.0/tests/commands/test_products.py` & `croud-1.9.0/tests/commands/test_products.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_projects.py` & `croud-1.9.0/tests/commands/test_projects.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_regions.py` & `croud-1.9.0/tests/commands/test_regions.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_subscriptions.py` & `croud-1.9.0/tests/commands/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/commands/test_users.py` & `croud-1.9.0/tests/commands/test_users.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/conftest.py` & `croud-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_api.py` & `croud-1.9.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_config_schemas.py` & `croud-1.9.0/tests/test_config_schemas.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_configuration.py` & `croud-1.9.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_parser.py` & `croud-1.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_printer.py` & `croud-1.9.0/tests/test_printer.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_server.py` & `croud-1.9.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/test_util.py` & `croud-1.9.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/util/__init__.py` & `croud-1.9.0/tests/util/__init__.py`

 * *Files identical despite different names*

### Comparing `croud-1.8.0/tests/util/fake_cloud.py` & `croud-1.9.0/tests/util/fake_cloud.py`

 * *Files identical despite different names*

