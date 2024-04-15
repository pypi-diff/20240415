# Comparing `tmp/google-shopping-merchant-inventories-0.1.5.tar.gz` & `tmp/google-shopping-merchant-inventories-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-shopping-merchant-inventories-0.1.5.tar", last modified: Tue Mar  5 19:01:48 2024, max compression
+gzip compressed data, was "google-shopping-merchant-inventories-0.1.6.tar", last modified: Mon Apr 15 13:58:58 2024, max compression
```

## Comparing `google-shopping-merchant-inventories-0.1.5.tar` & `google-shopping-merchant-inventories-0.1.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5391 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3926 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.600989 google-shopping-merchant-inventories-0.1.5/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.600989 google-shopping-merchant-inventories-0.1.5/google/shopping/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.600989 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories/
--rw-rw-r--   0 root         (0)     1003     2291 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.604990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/
--rw-rw-r--   0 root         (0)     1003     1897 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     3685 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       97 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.604990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.604990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/
--rw-rw-r--   0 root         (0)     1003      797 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25264 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42185 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py
--rw-rw-r--   0 root         (0)     1003     6203 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.604990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/
--rw-rw-r--   0 root         (0)     1003     1519 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7245 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15447 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15726 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    22430 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.608990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/
--rw-rw-r--   0 root         (0)     1003      809 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25770 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42812 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py
--rw-rw-r--   0 root         (0)     1003     6375 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.608990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7361 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15724 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15997 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    23034 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.608990 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     1344 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     9888 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/localinventory.py
--rw-rw-r--   0 root         (0)     1003     8256 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.608990 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/
--rw-r--r--   0 root         (0)     1003     5391 2024-03-05 19:01:48.000000 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3053 2024-03-05 19:01:48.000000 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:48.000000 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 19:01:48.000000 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      343 2024-03-05 19:01:48.000000 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 19:01:48.000000 google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3281 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 19:01:48.612990 google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   138760 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py
--rw-rw-r--   0 root         (0)     1003   139740 2024-03-05 18:46:03.000000 google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5391 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3926 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.076362 google-shopping-merchant-inventories-0.1.6/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.076362 google-shopping-merchant-inventories-0.1.6/google/shopping/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/
+-rw-rw-r--   0 root         (0)     1003     2291 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/
+-rw-rw-r--   0 root         (0)     1003     1897 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3685 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       97 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/
+-rw-rw-r--   0 root         (0)     1003      797 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25264 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42185 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6203 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.080362 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1519 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7245 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15447 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15726 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    22430 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.084363 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/
+-rw-rw-r--   0 root         (0)     1003      809 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25770 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42812 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6375 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.084363 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7361 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15724 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15997 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    23034 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.084363 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     1344 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9899 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/localinventory.py
+-rw-rw-r--   0 root         (0)     1003     8279 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/
+-rw-r--r--   0 root         (0)     1003     5391 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3053 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      343 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-15 13:58:58.000000 google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3281 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-15 13:58:58.088363 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   145402 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py
+-rw-rw-r--   0 root         (0)     1003   146307 2024-04-15 13:54:45.000000 google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py
```

### Comparing `google-shopping-merchant-inventories-0.1.5/LICENSE` & `google-shopping-merchant-inventories-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.5/MANIFEST.in` & `google-shopping-merchant-inventories-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.5/PKG-INFO` & `google-shopping-merchant-inventories-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-inventories
-Version: 0.1.5
+Version: 0.1.6
 Summary: Google Shopping Merchant Inventories API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-inventories
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-inventories-0.1.5/README.rst` & `google-shopping-merchant-inventories-0.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories/gapic_version.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.5"  # {x-release-please-version}
+__version__ = "0.1.6"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/gapic_metadata.json` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/gapic_version.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.5"  # {x-release-please-version}
+__version__ = "0.1.6"  # {x-release-please-version}
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/local_inventory_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/services/regional_inventory_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/__init__.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/localinventory.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/localinventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -50,17 +50,17 @@
             Format:
             ``accounts/{account}/products/{product}/localInventories/{store_code}``
         account (int):
             Output only. The account that owns the
             product. This field will be ignored if set by
             the client.
         store_code (str):
-            Required. Store code (the store ID from your Business
-            Profile) of the physical store the product is sold in. See
-            the `Local product inventory feed
+            Required. Immutable. Store code (the store ID from your
+            Business Profile) of the physical store the product is sold
+            in. See the `Local product inventory feed
             specification <https://support.google.com/merchants/answer/3061342>`__
             for more information.
         price (google.shopping.type.types.Price):
             Price of the product at this store.
         sale_price (google.shopping.type.types.Price):
             Sale price of the product at this store. Mandatory if
             [``salePriceEffectiveDate``][google.shopping.merchant.inventories.v1beta.LocalInventory.sale_price_effective_date]
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py` & `google-shopping-merchant-inventories-0.1.6/google/shopping/merchant_inventories_v1beta/types/regionalinventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -51,16 +51,17 @@
             Format:
             ``{regional_inventory.name=accounts/{account}/products/{product}/regionalInventories/{region}``
         account (int):
             Output only. The account that owns the
             product. This field will be ignored if set by
             the client.
         region (str):
-            Required. ID of the region for this ``RegionalInventory``
-            resource. See the `Regional availability and
+            Required. Immutable. ID of the region for this
+            ``RegionalInventory`` resource. See the `Regional
+            availability and
             pricing <https://support.google.com/merchants/answer/9698880>`__
             for more details.
         price (google.shopping.type.types.Price):
             Price of the product in this region.
         sale_price (google.shopping.type.types.Price):
             Sale price of the product in this region. Mandatory if
             [``salePriceEffectiveDate``][google.shopping.merchant.inventories.v1beta.RegionalInventory.sale_price_effective_date]
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/PKG-INFO` & `google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-shopping-merchant-inventories
-Version: 0.1.5
+Version: 0.1.6
 Summary: Google Shopping Merchant Inventories API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-shopping-merchant-inventories
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-shopping-merchant-inventories-0.1.5/google_shopping_merchant_inventories.egg-info/SOURCES.txt` & `google-shopping-merchant-inventories-0.1.6/google_shopping_merchant_inventories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-shopping-merchant-inventories-0.1.5/setup.py` & `google-shopping-merchant-inventories-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/tests/__init__.py` & `google-shopping-merchant-inventories-0.1.6/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/tests/unit/__init__.py` & `google-shopping-merchant-inventories-0.1.6/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/__init__.py` & `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/__init__.py` & `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py` & `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_local_inventory_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1215,15 +1215,16 @@
             next_page_token="next_page_token_value",
         )
         response = client.list_local_inventories(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == localinventory.ListLocalInventoriesRequest()
+        request = localinventory.ListLocalInventoriesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListLocalInventoriesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_local_inventories_empty_call():
@@ -1240,14 +1241,68 @@
     ) as call:
         client.list_local_inventories()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.ListLocalInventoriesRequest()
 
 
+def test_list_local_inventories_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = LocalInventoryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = localinventory.ListLocalInventoriesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_local_inventories), "__call__"
+    ) as call:
+        client.list_local_inventories(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == localinventory.ListLocalInventoriesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_local_inventories_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = LocalInventoryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_local_inventories), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            localinventory.ListLocalInventoriesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_local_inventories()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == localinventory.ListLocalInventoriesRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_local_inventories_async(
     transport: str = "grpc_asyncio",
     request_type=localinventory.ListLocalInventoriesRequest,
 ):
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1269,15 +1324,16 @@
             )
         )
         response = await client.list_local_inventories(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == localinventory.ListLocalInventoriesRequest()
+        request = localinventory.ListLocalInventoriesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListLocalInventoriesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
@@ -1667,15 +1723,16 @@
             instore_product_location="instore_product_location_value",
         )
         response = client.insert_local_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == localinventory.InsertLocalInventoryRequest()
+        request = localinventory.InsertLocalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, localinventory.LocalInventory)
     assert response.name == "name_value"
     assert response.account == 749
     assert response.store_code == "store_code_value"
     assert response.availability == "availability_value"
@@ -1699,14 +1756,73 @@
     ) as call:
         client.insert_local_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.InsertLocalInventoryRequest()
 
 
+def test_insert_local_inventory_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = LocalInventoryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = localinventory.InsertLocalInventoryRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.insert_local_inventory), "__call__"
+    ) as call:
+        client.insert_local_inventory(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == localinventory.InsertLocalInventoryRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_insert_local_inventory_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = LocalInventoryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.insert_local_inventory), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            localinventory.LocalInventory(
+                name="name_value",
+                account=749,
+                store_code="store_code_value",
+                availability="availability_value",
+                quantity=895,
+                pickup_method="pickup_method_value",
+                pickup_sla="pickup_sla_value",
+                instore_product_location="instore_product_location_value",
+            )
+        )
+        response = await client.insert_local_inventory()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == localinventory.InsertLocalInventoryRequest()
+
+
 @pytest.mark.asyncio
 async def test_insert_local_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=localinventory.InsertLocalInventoryRequest,
 ):
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1735,15 +1851,16 @@
             )
         )
         response = await client.insert_local_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == localinventory.InsertLocalInventoryRequest()
+        request = localinventory.InsertLocalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, localinventory.LocalInventory)
     assert response.name == "name_value"
     assert response.account == 749
     assert response.store_code == "store_code_value"
     assert response.availability == "availability_value"
@@ -1847,15 +1964,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.delete_local_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == localinventory.DeleteLocalInventoryRequest()
+        request = localinventory.DeleteLocalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_delete_local_inventory_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1871,14 +1989,62 @@
     ) as call:
         client.delete_local_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == localinventory.DeleteLocalInventoryRequest()
 
 
+def test_delete_local_inventory_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = LocalInventoryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = localinventory.DeleteLocalInventoryRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_local_inventory), "__call__"
+    ) as call:
+        client.delete_local_inventory(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == localinventory.DeleteLocalInventoryRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_local_inventory_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = LocalInventoryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_local_inventory), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_local_inventory()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == localinventory.DeleteLocalInventoryRequest()
+
+
 @pytest.mark.asyncio
 async def test_delete_local_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=localinventory.DeleteLocalInventoryRequest,
 ):
     client = LocalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1896,15 +2062,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.delete_local_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == localinventory.DeleteLocalInventoryRequest()
+        request = localinventory.DeleteLocalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_delete_local_inventory_async_from_dict():
```

### Comparing `google-shopping-merchant-inventories-0.1.5/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py` & `google-shopping-merchant-inventories-0.1.6/tests/unit/gapic/merchant_inventories_v1beta/test_regional_inventory_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -1223,15 +1223,16 @@
             next_page_token="next_page_token_value",
         )
         response = client.list_regional_inventories(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == regionalinventory.ListRegionalInventoriesRequest()
+        request = regionalinventory.ListRegionalInventoriesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRegionalInventoriesPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 def test_list_regional_inventories_empty_call():
@@ -1248,14 +1249,68 @@
     ) as call:
         client.list_regional_inventories()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.ListRegionalInventoriesRequest()
 
 
+def test_list_regional_inventories_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = RegionalInventoryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = regionalinventory.ListRegionalInventoriesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_regional_inventories), "__call__"
+    ) as call:
+        client.list_regional_inventories(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == regionalinventory.ListRegionalInventoriesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_regional_inventories_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = RegionalInventoryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_regional_inventories), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            regionalinventory.ListRegionalInventoriesResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_regional_inventories()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == regionalinventory.ListRegionalInventoriesRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_regional_inventories_async(
     transport: str = "grpc_asyncio",
     request_type=regionalinventory.ListRegionalInventoriesRequest,
 ):
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1277,15 +1332,16 @@
             )
         )
         response = await client.list_regional_inventories(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == regionalinventory.ListRegionalInventoriesRequest()
+        request = regionalinventory.ListRegionalInventoriesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRegionalInventoriesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
 
 
 @pytest.mark.asyncio
@@ -1673,15 +1729,16 @@
             availability="availability_value",
         )
         response = client.insert_regional_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == regionalinventory.InsertRegionalInventoryRequest()
+        request = regionalinventory.InsertRegionalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, regionalinventory.RegionalInventory)
     assert response.name == "name_value"
     assert response.account == 749
     assert response.region == "region_value"
     assert response.availability == "availability_value"
@@ -1701,14 +1758,69 @@
     ) as call:
         client.insert_regional_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.InsertRegionalInventoryRequest()
 
 
+def test_insert_regional_inventory_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = RegionalInventoryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = regionalinventory.InsertRegionalInventoryRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.insert_regional_inventory), "__call__"
+    ) as call:
+        client.insert_regional_inventory(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == regionalinventory.InsertRegionalInventoryRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_insert_regional_inventory_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = RegionalInventoryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.insert_regional_inventory), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            regionalinventory.RegionalInventory(
+                name="name_value",
+                account=749,
+                region="region_value",
+                availability="availability_value",
+            )
+        )
+        response = await client.insert_regional_inventory()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == regionalinventory.InsertRegionalInventoryRequest()
+
+
 @pytest.mark.asyncio
 async def test_insert_regional_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=regionalinventory.InsertRegionalInventoryRequest,
 ):
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1733,15 +1845,16 @@
             )
         )
         response = await client.insert_regional_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == regionalinventory.InsertRegionalInventoryRequest()
+        request = regionalinventory.InsertRegionalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, regionalinventory.RegionalInventory)
     assert response.name == "name_value"
     assert response.account == 749
     assert response.region == "region_value"
     assert response.availability == "availability_value"
@@ -1841,15 +1954,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.delete_regional_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == regionalinventory.DeleteRegionalInventoryRequest()
+        request = regionalinventory.DeleteRegionalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_delete_regional_inventory_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1865,14 +1979,62 @@
     ) as call:
         client.delete_regional_inventory()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == regionalinventory.DeleteRegionalInventoryRequest()
 
 
+def test_delete_regional_inventory_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = RegionalInventoryServiceClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = regionalinventory.DeleteRegionalInventoryRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_regional_inventory), "__call__"
+    ) as call:
+        client.delete_regional_inventory(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == regionalinventory.DeleteRegionalInventoryRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_regional_inventory_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = RegionalInventoryServiceAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_regional_inventory), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_regional_inventory()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == regionalinventory.DeleteRegionalInventoryRequest()
+
+
 @pytest.mark.asyncio
 async def test_delete_regional_inventory_async(
     transport: str = "grpc_asyncio",
     request_type=regionalinventory.DeleteRegionalInventoryRequest,
 ):
     client = RegionalInventoryServiceAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -1890,15 +2052,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.delete_regional_inventory(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == regionalinventory.DeleteRegionalInventoryRequest()
+        request = regionalinventory.DeleteRegionalInventoryRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_delete_regional_inventory_async_from_dict():
```

