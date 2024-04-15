# Comparing `tmp/apexpro-1.1.9.tar.gz` & `tmp/apexpro-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apexpro-1.1.9.tar", last modified: Tue Nov 21 04:01:49 2023, max compression
+gzip compressed data, was "apexpro-1.2.0.tar", last modified: Mon Apr 15 03:45:31 2024, max compression
```

## Comparing `apexpro-1.1.9.tar` & `apexpro-1.2.0.tar`

### file list

```diff
@@ -1,74 +1,75 @@
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.530067 apexpro-1.1.9/
--rw-r--r--   0 dl00015ml   (502) staff       (20)      363 2022-07-15 03:54:05.000000 apexpro-1.1.9/CHANGELOG.md
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1218 2022-11-25 01:02:08.000000 apexpro-1.1.9/LICENSE
--rw-r--r--   0 dl00015ml   (502) staff       (20)       83 2022-07-15 03:54:05.000000 apexpro-1.1.9/MANIFEST.in
--rw-r--r--   0 dl00015ml   (502) staff       (20)     9572 2023-11-21 04:01:49.529942 apexpro-1.1.9/PKG-INFO
--rw-r--r--   0 dl00015ml   (502) staff       (20)     8358 2023-08-07 14:04:01.000000 apexpro-1.1.9/README.md
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.517070 apexpro-1.1.9/apexpro/
--rw-r--r--   0 dl00015ml   (502) staff       (20)    15341 2023-10-13 04:15:21.000000 apexpro-1.1.9/apexpro/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     9992 2023-10-13 04:15:21.000000 apexpro-1.1.9/apexpro/_websocket_stream.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1591 2022-09-29 09:49:57.000000 apexpro-1.1.9/apexpro/constants.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      874 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/errors.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    16581 2022-12-22 07:57:17.000000 apexpro-1.1.9/apexpro/eth.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.519841 apexpro-1.1.9/apexpro/eth_signing/
--rw-r--r--   0 dl00015ml   (502) staff       (20)      246 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/eth_signing/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1812 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/eth_signing/eth_prive_action.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2617 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/eth_signing/onboarding_action.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3896 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/eth_signing/sign_off_chain_action.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3334 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/eth_signing/signers.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2749 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/eth_signing/util.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1318 2022-11-25 01:02:08.000000 apexpro-1.1.9/apexpro/exceptions.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.520974 apexpro-1.1.9/apexpro/helpers/
--rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/helpers/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      348 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/helpers/db.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2570 2022-09-16 09:30:41.000000 apexpro-1.1.9/apexpro/helpers/request_helpers.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1077 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/helpers/requests.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      840 2023-07-05 05:49:58.000000 apexpro-1.1.9/apexpro/helpers/util.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    30558 2023-11-21 03:58:37.000000 apexpro-1.1.9/apexpro/http_private.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    32560 2023-10-13 04:15:21.000000 apexpro-1.1.9/apexpro/http_private_stark_key_sign.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3821 2023-11-21 03:58:37.000000 apexpro-1.1.9/apexpro/http_public.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      127 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/models.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.522751 apexpro-1.1.9/apexpro/starkex/
--rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     4238 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/conditional_transfer.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1558 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/constants.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     5844 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/helpers.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     6588 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/order.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1124 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/signable.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.524269 apexpro-1.1.9/apexpro/starkex/starkex_resources/
--rw-r--r--   0 dl00015ml   (502) staff       (20)      285 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/starkex_resources/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3089 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/starkex_resources/cpp_signature.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3627 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/starkex_resources/math_utils.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)   102708 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/starkex_resources/pedersen_params.json
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1346 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/starkex_resources/proxy.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)    10414 2022-07-15 03:54:05.000000 apexpro-1.1.9/apexpro/starkex/starkex_resources/python_signature.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3812 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/transfer.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2631 2022-08-25 03:55:08.000000 apexpro-1.1.9/apexpro/starkex/withdrawal.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     4578 2023-05-24 06:10:59.000000 apexpro-1.1.9/apexpro/websocket_api.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.529614 apexpro-1.1.9/apexpro.egg-info/
--rw-r--r--   0 dl00015ml   (502) staff       (20)     9572 2023-11-21 04:01:49.000000 apexpro-1.1.9/apexpro.egg-info/PKG-INFO
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1792 2023-11-21 04:01:49.000000 apexpro-1.1.9/apexpro.egg-info/SOURCES.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2023-11-21 04:01:49.000000 apexpro-1.1.9/apexpro.egg-info/dependency_links.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2022-07-15 06:12:12.000000 apexpro-1.1.9/apexpro.egg-info/not-zip-safe
--rw-r--r--   0 dl00015ml   (502) staff       (20)      245 2023-11-21 04:01:49.000000 apexpro-1.1.9/apexpro.egg-info/requires.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)       14 2023-11-21 04:01:49.000000 apexpro-1.1.9/apexpro.egg-info/top_level.txt
--rw-r--r--   0 dl00015ml   (502) staff       (20)      131 2023-11-21 04:01:49.530303 apexpro-1.1.9/setup.cfg
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1656 2023-11-21 03:59:36.000000 apexpro-1.1.9/setup.py
-drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2023-11-21 04:01:49.529257 apexpro-1.1.9/tests/
--rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2022-07-15 03:54:05.000000 apexpro-1.1.9/tests/__init__.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     5583 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/account_value.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      147 2022-07-15 03:54:05.000000 apexpro-1.1.9/tests/constants.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1962 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_deposit.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2817 2023-02-09 06:01:49.000000 apexpro-1.1.9/tests/demo_private.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3099 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_private_v2.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1001 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_public.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1010 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_public_v2.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1433 2022-12-22 07:57:17.000000 apexpro-1.1.9/tests/demo_register.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1503 2022-11-23 00:41:45.000000 apexpro-1.1.9/tests/demo_register_mul_address.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     1454 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_register_v2.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      583 2022-09-29 09:49:57.000000 apexpro-1.1.9/tests/demo_sign.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     4704 2023-08-07 14:04:01.000000 apexpro-1.1.9/tests/demo_stark_key_sign.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     3098 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_stark_key_sign_v2.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)      962 2022-12-09 13:23:37.000000 apexpro-1.1.9/tests/demo_ws.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     2744 2023-11-21 03:58:37.000000 apexpro-1.1.9/tests/demo_ws_depthdata.py
--rw-r--r--   0 dl00015ml   (502) staff       (20)     5573 2022-08-25 03:55:08.000000 apexpro-1.1.9/tests/test_onboarding.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.256104 apexpro-1.2.0/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      363 2023-09-06 03:29:33.000000 apexpro-1.2.0/CHANGELOG.md
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1218 2023-09-06 03:29:33.000000 apexpro-1.2.0/LICENSE
+-rw-r--r--   0 dl00015ml   (502) staff       (20)       83 2023-09-06 03:29:33.000000 apexpro-1.2.0/MANIFEST.in
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    20418 2024-04-15 03:45:31.255950 apexpro-1.2.0/PKG-INFO
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    19204 2024-01-30 12:43:21.000000 apexpro-1.2.0/README.md
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.244756 apexpro-1.2.0/apexpro/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    15341 2023-10-13 03:57:54.000000 apexpro-1.2.0/apexpro/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    10010 2024-01-30 12:43:21.000000 apexpro-1.2.0/apexpro/_websocket_stream.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1598 2024-01-30 12:43:21.000000 apexpro-1.2.0/apexpro/constants.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      874 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/errors.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    16581 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.247327 apexpro-1.2.0/apexpro/eth_signing/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      246 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth_signing/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1812 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth_signing/eth_prive_action.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2617 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth_signing/onboarding_action.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3896 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth_signing/sign_off_chain_action.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3334 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth_signing/signers.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2749 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/eth_signing/util.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1318 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/exceptions.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.248296 apexpro-1.2.0/apexpro/helpers/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/helpers/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      348 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/helpers/db.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2570 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/helpers/request_helpers.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1077 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/helpers/requests.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      840 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/helpers/util.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    30558 2024-01-30 12:43:21.000000 apexpro-1.2.0/apexpro/http_private.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    32698 2024-01-30 12:43:21.000000 apexpro-1.2.0/apexpro/http_private_stark_key_sign.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3821 2024-01-30 12:43:21.000000 apexpro-1.2.0/apexpro/http_public.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      127 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/models.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.250096 apexpro-1.2.0/apexpro/starkex/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     4238 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/conditional_transfer.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1558 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/constants.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     5844 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/helpers.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     6588 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/order.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1124 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/signable.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.251410 apexpro-1.2.0/apexpro/starkex/starkex_resources/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      285 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/starkex_resources/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3089 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/starkex_resources/cpp_signature.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3627 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/starkex_resources/math_utils.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)   102708 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/starkex_resources/pedersen_params.json
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1346 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/starkex_resources/proxy.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    10414 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/starkex_resources/python_signature.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3812 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/transfer.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2631 2023-09-06 03:29:33.000000 apexpro-1.2.0/apexpro/starkex/withdrawal.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     4813 2024-01-30 12:43:21.000000 apexpro-1.2.0/apexpro/websocket_api.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.255535 apexpro-1.2.0/apexpro.egg-info/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)    20418 2024-04-15 03:45:31.000000 apexpro-1.2.0/apexpro.egg-info/PKG-INFO
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1818 2024-04-15 03:45:31.000000 apexpro-1.2.0/apexpro.egg-info/SOURCES.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2024-04-15 03:45:31.000000 apexpro-1.2.0/apexpro.egg-info/dependency_links.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        1 2024-04-15 03:42:19.000000 apexpro-1.2.0/apexpro.egg-info/not-zip-safe
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      245 2024-04-15 03:45:31.000000 apexpro-1.2.0/apexpro.egg-info/requires.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)       14 2024-04-15 03:45:31.000000 apexpro-1.2.0/apexpro.egg-info/top_level.txt
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      131 2024-04-15 03:45:31.256497 apexpro-1.2.0/setup.cfg
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1656 2024-04-15 03:44:54.000000 apexpro-1.2.0/setup.py
+drwxr-xr-x   0 dl00015ml   (502) staff       (20)        0 2024-04-15 03:45:31.255215 apexpro-1.2.0/tests/
+-rw-r--r--   0 dl00015ml   (502) staff       (20)        0 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/__init__.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     5583 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/account_value.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1237 2024-01-30 12:43:21.000000 apexpro-1.2.0/tests/account_value_ws.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      147 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/constants.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1961 2024-01-30 12:43:21.000000 apexpro-1.2.0/tests/demo_deposit.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2818 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_private.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     3099 2024-01-30 12:43:21.000000 apexpro-1.2.0/tests/demo_private_v2.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1001 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_public.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1010 2024-01-30 12:43:21.000000 apexpro-1.2.0/tests/demo_public_v2.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1432 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_register.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1503 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_register_mul_address.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     1454 2024-01-30 12:43:21.000000 apexpro-1.2.0/tests/demo_register_v2.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      583 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_sign.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     4801 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_stark_key_sign.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2938 2024-01-30 12:43:21.000000 apexpro-1.2.0/tests/demo_stark_key_sign_v2.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)      961 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_ws.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     2730 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/demo_ws_depthdata.py
+-rw-r--r--   0 dl00015ml   (502) staff       (20)     5573 2023-09-06 03:29:33.000000 apexpro-1.2.0/tests/test_onboarding.py
```

### Comparing `apexpro-1.1.9/LICENSE` & `apexpro-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/__init__.py` & `apexpro-1.2.0/apexpro/__init__.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/_websocket_stream.py` & `apexpro-1.2.0/apexpro/_websocket_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             method='GET',
             iso_timestamp=str(time_stamp),
         )
 
 
         req = {
             'type': 'login',
-            'topics': ['ws_notify_v1', 'ws_accounts_v1'],
+            'topics': ['ws_notify_v1', 'ws_accounts_v2', 'ws_accounts_v1'],
             'httpMethod': 'GET',
             'requestPath': PRIVATE_REQUEST_PATH,
             'apiKey': self.api_key_credentials['key'],
             'passphrase': self.api_key_credentials['passphrase'],
             'timestamp': time_stamp,
             'signature': signature,
         }
```

### Comparing `apexpro-1.1.9/apexpro/constants.py` & `apexpro-1.2.0/apexpro/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # ------------ register_env_id ------------
 REGISTER_ENVID_MAIN = 1
 REGISTER_ENVID_TEST = 5
 
 # ------------ network_id ------------
 NETWORKID_MAIN = 1
-NETWORKID_TEST = 5
+NETWORKID_TEST = 11155111
 
 # ------------ Signature Types ------------
 SIGNATURE_TYPE_NO_PREPEND = 0
 SIGNATURE_TYPE_DECIMAL = 1
 SIGNATURE_TYPE_HEXADECIMAL = 2
 SIGNATURE_TYPE_PERSONAL = 3
```

### Comparing `apexpro-1.1.9/apexpro/errors.py` & `apexpro-1.2.0/apexpro/errors.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/eth.py` & `apexpro-1.2.0/apexpro/eth.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/eth_signing/eth_prive_action.py` & `apexpro-1.2.0/apexpro/eth_signing/eth_prive_action.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/eth_signing/onboarding_action.py` & `apexpro-1.2.0/apexpro/eth_signing/onboarding_action.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/eth_signing/sign_off_chain_action.py` & `apexpro-1.2.0/apexpro/eth_signing/sign_off_chain_action.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/eth_signing/signers.py` & `apexpro-1.2.0/apexpro/eth_signing/signers.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/eth_signing/util.py` & `apexpro-1.2.0/apexpro/eth_signing/util.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/exceptions.py` & `apexpro-1.2.0/apexpro/exceptions.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/helpers/request_helpers.py` & `apexpro-1.2.0/apexpro/helpers/request_helpers.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/helpers/requests.py` & `apexpro-1.2.0/apexpro/helpers/requests.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/helpers/util.py` & `apexpro-1.2.0/apexpro/helpers/util.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/http_private.py` & `apexpro-1.2.0/apexpro/http_private.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/http_private_stark_key_sign.py` & `apexpro-1.2.0/apexpro/http_private_stark_key_sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,16 @@
                      triggerPriceType=None,
                      trailingPercent=None,
                      clientId=None,
                      expiration=None,
                      expirationEpochSeconds=None,
                      isPositionTpsl = False,
                      signature=None,
-                     sourceFlag=None,):
+                     sourceFlag=None,
+                     brokerId=None,):
         """"
         POST  create_order.
         client.create_order(symbol="BTC-USDC", side="SELL",
                                            type="LIMIT", size="0.01",
                                            price="20000", limitFeeRate="1",
                                             accountId="325881046451093849",reduceOnly=False,
                                            expiration=now_iso + SEVEN_DAYS_S + 60*1000, timeInForce="GOOD_TIL_CANCEL")
@@ -141,14 +142,15 @@
             'triggerPriceType': triggerPriceType,
             'trailingPercent': trailingPercent,
             'clientId': clientId,
             'signature': signature,
             'reduceOnly': reduceOnly,
             'isPositionTpsl': isPositionTpsl,
             'sourceFlag': sourceFlag,
+            'brokerId':brokerId,
         }
 
         path = URL_SUFFIX + "/v1/create-order"
         return self._post(
             endpoint=path,
             data=order
         )
@@ -168,15 +170,16 @@
                      triggerPriceType=None,
                      trailingPercent=None,
                      clientId=None,
                      expiration=None,
                      expirationEpochSeconds=None,
                      isPositionTpsl = False,
                      signature=None,
-                     sourceFlag=None,):
+                     sourceFlag=None,
+                     brokerId=None,):
         """"
         POST  create_order.
         client.create_order(symbol="BTC-USDC", side="SELL",
                                            type="LIMIT", size="0.01",
                                            price="20000", limitFeeRate="1",
                                             accountId="325881046451093849",reduceOnly=False,
                                            expiration=now_iso + SEVEN_DAYS_S + 60*1000, timeInForce="GOOD_TIL_CANCEL")
@@ -285,14 +288,15 @@
             'triggerPriceType': triggerPriceType,
             'trailingPercent': trailingPercent,
             'clientId': clientId,
             'signature': signature,
             'reduceOnly': reduceOnly,
             'isPositionTpsl': isPositionTpsl,
             'sourceFlag': sourceFlag,
+            'brokerId':brokerId,
         }
 
         path = URL_SUFFIX + "/v2/create-order"
         return self._post(
             endpoint=path,
             data=order
         )
```

### Comparing `apexpro-1.1.9/apexpro/http_public.py` & `apexpro-1.2.0/apexpro/http_public.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/conditional_transfer.py` & `apexpro-1.2.0/apexpro/starkex/conditional_transfer.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/constants.py` & `apexpro-1.2.0/apexpro/starkex/constants.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/helpers.py` & `apexpro-1.2.0/apexpro/starkex/helpers.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/order.py` & `apexpro-1.2.0/apexpro/starkex/order.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/signable.py` & `apexpro-1.2.0/apexpro/starkex/signable.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/starkex_resources/cpp_signature.py` & `apexpro-1.2.0/apexpro/starkex/starkex_resources/cpp_signature.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/starkex_resources/math_utils.py` & `apexpro-1.2.0/apexpro/starkex/starkex_resources/math_utils.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/starkex_resources/pedersen_params.json` & `apexpro-1.2.0/apexpro/starkex/starkex_resources/pedersen_params.json`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/starkex_resources/proxy.py` & `apexpro-1.2.0/apexpro/starkex/starkex_resources/proxy.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/starkex_resources/python_signature.py` & `apexpro-1.2.0/apexpro/starkex/starkex_resources/python_signature.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/transfer.py` & `apexpro-1.2.0/apexpro/starkex/transfer.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/starkex/withdrawal.py` & `apexpro-1.2.0/apexpro/starkex/withdrawal.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/apexpro/websocket_api.py` & `apexpro-1.2.0/apexpro/websocket_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -128,7 +128,14 @@
 
     def account_info_stream(self, callback):
         """
         https://api-docs.pro.apex.exchange/#private-websocket
         """
         topic = "ws_accounts_v1"
         self._ws_private_subscribe(topic=topic, callback=callback)
+
+    def account_info_stream_v2(self, callback):
+        """
+        https://api-docs.pro.apex.exchange/#private-websocket
+        """
+        topic = "ws_accounts_v2"
+        self._ws_private_subscribe(topic=topic, callback=callback)
```

### Comparing `apexpro-1.1.9/apexpro.egg-info/SOURCES.txt` & `apexpro-1.2.0/apexpro.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 apexpro/starkex/starkex_resources/cpp_signature.py
 apexpro/starkex/starkex_resources/math_utils.py
 apexpro/starkex/starkex_resources/pedersen_params.json
 apexpro/starkex/starkex_resources/proxy.py
 apexpro/starkex/starkex_resources/python_signature.py
 tests/__init__.py
 tests/account_value.py
+tests/account_value_ws.py
 tests/constants.py
 tests/demo_deposit.py
 tests/demo_private.py
 tests/demo_private_v2.py
 tests/demo_public.py
 tests/demo_public_v2.py
 tests/demo_register.py
```

### Comparing `apexpro-1.1.9/setup.py` & `apexpro-1.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='apexpro',
-    version='1.1.9',
+    version='1.2.0',
     packages=find_packages(),
     description='Python3 Apexpro HTTP/WebSocket API Connector',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/xxx',
     license='MIT License',
     author='Dexter Dickinson',
```

### Comparing `apexpro-1.1.9/tests/account_value.py` & `apexpro-1.2.0/tests/account_value.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_deposit.py` & `apexpro-1.2.0/tests/demo_deposit.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 root_path = os.path.abspath(__file__)
 root_path = '/'.join(root_path.split('/')[:-2])
 sys.path.append(root_path)
 
 from apexpro.http_private import HttpPrivate
 from apexpro.constants import APEX_HTTP_TEST, NETWORKID_TEST, APEX_HTTP_MAIN, NETWORKID_MAIN
 
-
 print("Hello, Apexpro")
 priKey = "your eth private key"
 
 key = 'your apiKey-key from register'
 secret = 'your apiKey-secret from register'
 passphrase = 'your apiKey-passphrase from register'
```

### Comparing `apexpro-1.1.9/tests/demo_private.py` & `apexpro-1.2.0/tests/demo_private.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 modifyUserRes = client.modify_user(username="pythonTest",email="11@aa.com",emailNotifyGeneralEnable="false")
 print(modifyUserRes)
 
 accountRes = client.get_account()
 print(accountRes)
 
+
 transfersRes = client.transfers(limit=100,page=0,currencyId="USDC",chainIds="1,5,13")
 print(transfersRes)
 
 withdrawListRes = client.withdraw_list(limit=100,page=0,beginTimeInclusive=1651406864000,endTimeExclusive=1657105971171)
 print(withdrawListRes)
 
 uncommon_withdraw_feeRes = client.uncommon_withdraw_fee(amount="101000.1",chainId=5)
```

### Comparing `apexpro-1.1.9/tests/demo_private_v2.py` & `apexpro-1.2.0/tests/demo_private_v2.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_public.py` & `apexpro-1.2.0/tests/demo_public.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_public_v2.py` & `apexpro-1.2.0/tests/demo_public_v2.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_register.py` & `apexpro-1.2.0/tests/demo_register.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 stark_key_pair_with_y_coordinate = client.derive_stark_key(client.default_address)
 
 nonceRes = client.generate_nonce(starkKey=stark_key_pair_with_y_coordinate['public_key'],ethAddress=client.default_address,chainId=NETWORKID_MAIN)
 
 #api_key = client.recover_api_key_credentials(nonce=nonceRes['data']['nonce'], ethereum_address=client.default_address)
 #print(api_key)
-
 regRes = client.register_user(nonce=nonceRes['data']['nonce'],starkKey=stark_key_pair_with_y_coordinate['public_key'],stark_public_key_y_coordinate=stark_key_pair_with_y_coordinate['public_key_y_coordinate'],ethereum_address=client.default_address)
 key = regRes['data']['apiKey']['key']
 secret = regRes['data']['apiKey']['secret']
 passphrase = regRes['data']['apiKey']['passphrase']
 
 #back stark_key_pair, apiKey,and accountId for private Api or create-oreder or withdraw
 print(stark_key_pair_with_y_coordinate)
```

### Comparing `apexpro-1.1.9/tests/demo_register_mul_address.py` & `apexpro-1.2.0/tests/demo_register_mul_address.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_register_v2.py` & `apexpro-1.2.0/tests/demo_register_v2.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_sign.py` & `apexpro-1.2.0/tests/demo_sign.py`

 * *Files identical despite different names*

### Comparing `apexpro-1.1.9/tests/demo_stark_key_sign.py` & `apexpro-1.2.0/tests/demo_stark_key_sign.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 root_path = '/'.join(root_path.split('/')[:-2])
 sys.path.append(root_path)
 
 from apexpro.constants import APEX_HTTP_TEST, NETWORKID_TEST, APEX_HTTP_MAIN, NETWORKID_MAIN
 
 print("Hello, Apexpro")
 
+
 # need api_key_credentials={'key': key,'secret': secret, 'passphrase': passphrase} for private api
 # need starkey for withdraw and createOrder
 
 key = 'your apiKey-key from register'
 secret = 'your apiKey-secret from register'
 passphrase = 'your apiKey-passphrase from register'
 
@@ -79,14 +80,15 @@
 print(createOrderRes)
 
 # sample5
 # Create a TP/SL order
 # first, Set a slippage to get an acceptable price
 # if timeInForce="GOOD_TIL_CANCEL" or "POST_ONLY", slippage is recommended to be greater than 0.1
 # if timeInForce="FILL_OR_KILL" or "IMMEDIATE_OR_CANCEL", slippage is recommended to be greater than 0.2
+# when buying, the price = price*(1 + slippage). when selling, the price = price*(1 - slippage)
 
 slippage = decimal.Decimal("0.1")
 price =  round_size(decimal.Decimal("28888") * (decimal.Decimal("1") + slippage), symbolData.get('tickSize'))
 
 createOrderRes = client.create_order(symbol="BTC-USDC", side="BUY", isPositionTpsl = True, reduceOnly= True,
                                      type="TAKE_PROFIT_MARKET", size="0.1", price=price, limitFeeRate=limitFeeRate,
                                      expirationEpochSeconds= currentTime, triggerPriceType="INDEX", triggerPrice="28888" )
```

### Comparing `apexpro-1.1.9/tests/demo_stark_key_sign_v2.py` & `apexpro-1.2.0/tests/demo_stark_key_sign_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 passphrase = 'your apiKey-passphrase from register'
 
 public_key = 'your stark_public_key from register'
 public_key_y_coordinate = 'your stark_public_key_y_coordinate from register'
 private_key = 'your stark_private_key from register'
 
 
-
 client = HttpPrivateStark(APEX_HTTP_TEST, network_id=NETWORKID_TEST,
                           stark_public_key=public_key,
                           stark_private_key=private_key,
                           stark_public_key_y_coordinate=public_key_y_coordinate,
                           api_key_credentials={'key': key, 'secret': secret, 'passphrase': passphrase})
 configs = client.configs_v2()
 client.get_user()
@@ -52,23 +51,18 @@
 orderFills = client.order_fills_v2(orderId='498441108374684453')
 print(orderFills)
 
 limitFeeRate = '0.0005'
 
 deleteOrdersRes = client.delete_open_orders_v2(token="USDT")
 print(deleteOrdersRes)
-
-for i in range(0,300):
-    createOrderRes = client.create_order_v2(symbol="BTC-USDT", side="SELL",
+createOrderRes = client.create_order_v2(symbol="BTC-USDT", side="SELL",
                                            type="LIMIT", size="0.01",expirationEpochSeconds= currentTime,
-                                           price="36890", limitFeeRate=limitFeeRate, timeInForce="POST_ONLY")
-    if len(createOrderRes.get('data')) < 5:
-        print(createOrderRes)
-    time.sleep(0.1)
-    print(i)
+                                           price="36890", limitFeeRate=limitFeeRate)
+
 
 #print(createOrderRes)
 
 fillsRes = client.fills_v2(limit=100,page=0,symbol="BTC-USDT",token="USDT")
 print(fillsRes)
```

### Comparing `apexpro-1.1.9/tests/demo_ws.py` & `apexpro-1.2.0/tests/demo_ws.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 from apexpro.constants import APEX_WS_TEST
 from apexpro.websocket_api import WebSocket
 
 key = 'your apiKey-key from register'
 secret = 'your apiKey-secret from register'
 passphrase = 'your apiKey-passphrase from register'
 
-
 # Connect with authentication!
 ws_client = WebSocket(
     endpoint=APEX_WS_TEST,
     api_key_credentials={'key': key, 'secret': secret, 'passphrase': passphrase},
 )
 
 def handle_account(message):
@@ -27,15 +26,14 @@
     print(3, message)
 def h4(message):
     print(4, message)
 
 #ws_client.depth_stream(h1,'BTCUSDC',25)
 #ws_client.ticker_stream(h2,'BTCUSDC')
 #ws_client.trade_stream(h3,'BTCUSDC')
-ws_client.klines_stream(h4,'BTCUSDC',1)
+#ws_client.klines_stream(h4,'BTCUSDC',1)
 ws_client.account_info_stream(handle_account)
 
 
 while True:
     # Run your main trading logic here.
     sleep(1)
-
```

### Comparing `apexpro-1.1.9/tests/demo_ws_depthdata.py` & `apexpro-1.2.0/tests/demo_ws_depthdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from time import sleep
 
-from apexpro.constants import APEX_WS_TEST, APEX_WS_MAIN
+from apexpro.constants import APEX_WS_TEST
 from apexpro.websocket_api import WebSocket
 
 
 # Connect with authentication!
 ws_client = WebSocket(
-    endpoint=APEX_WS_MAIN,
+    endpoint=APEX_WS_TEST,
 )
 
 def depth_data(message):
     showDepthdata(message)
 
 
 lastDepthData = {}
```

### Comparing `apexpro-1.1.9/tests/test_onboarding.py` & `apexpro-1.2.0/tests/test_onboarding.py`

 * *Files identical despite different names*

