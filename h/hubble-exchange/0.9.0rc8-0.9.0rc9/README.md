# Comparing `tmp/hubble_exchange-0.9.0rc8.tar.gz` & `tmp/hubble_exchange-0.9.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubble_exchange-0.9.0rc8.tar", last modified: Mon Mar 11 07:08:42 2024, max compression
+gzip compressed data, was "hubble_exchange-0.9.0rc9.tar", last modified: Thu Mar 14 05:04:33 2024, max compression
```

## Comparing `hubble_exchange-0.9.0rc8.tar` & `hubble_exchange-0.9.0rc9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-11 07:08:42.040327 hubble_exchange-0.9.0rc8/
--rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.9.0rc8/LICENSE
--rw-r--r--   0 shubham    (501) staff       (20)      134 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/MANIFEST.in
--rw-r--r--   0 shubham    (501) staff       (20)    20960 2024-03-11 07:08:42.040073 hubble_exchange-0.9.0rc8/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)    19078 2024-02-03 16:04:30.000000 hubble_exchange-0.9.0rc8/README.md
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-11 07:08:42.034298 hubble_exchange-0.9.0rc8/hubble_exchange/
--rw-r--r--   0 shubham    (501) staff       (20)      643 2024-01-22 15:57:19.000000 hubble_exchange-0.9.0rc8/hubble_exchange/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)    25889 2024-03-01 07:57:57.000000 hubble_exchange-0.9.0rc8/hubble_exchange/client.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-11 07:08:42.035996 hubble_exchange-0.9.0rc8/hubble_exchange/config/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2023-09-07 05:27:24.000000 hubble_exchange-0.9.0rc8/hubble_exchange/config/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     1160 2024-01-18 15:44:33.000000 hubble_exchange-0.9.0rc8/hubble_exchange/config/aylin.py
--rw-r--r--   0 shubham    (501) staff       (20)      899 2023-10-05 10:42:27.000000 hubble_exchange-0.9.0rc8/hubble_exchange/config/hubblenext.py
--rw-r--r--   0 shubham    (501) staff       (20)     1121 2024-02-25 09:51:44.000000 hubble_exchange-0.9.0rc8/hubble_exchange/config/local.py
--rw-r--r--   0 shubham    (501) staff       (20)     1162 2024-03-01 09:20:49.000000 hubble_exchange-0.9.0rc8/hubble_exchange/config/mainnet.py
--rw-r--r--   0 shubham    (501) staff       (20)      739 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/constants.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-11 07:08:42.039209 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/
--rw-r--r--   0 shubham    (501) staff       (20)    22218 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/AMM.json
--rw-r--r--   0 shubham    (501) staff       (20)    25060 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/ClearingHouse.json
--rw-r--r--   0 shubham    (501) staff       (20)    24834 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/HGT.json
--rw-r--r--   0 shubham    (501) staff       (20)    27957 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/HGTRemote.json
--rw-r--r--   0 shubham    (501) staff       (20)     4460 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/IERC20.json
--rw-r--r--   0 shubham    (501) staff       (20)     7583 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/ImmediateOrCancelOrders.json
--rw-r--r--   0 shubham    (501) staff       (20)    10987 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/LimitOrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     7118 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/MarginAccountHelper.json
--rw-r--r--   0 shubham    (501) staff       (20)     4973 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/OrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)    10456 2024-01-16 14:11:20.000000 hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/SignedOrderBook.json
--rw-r--r--   0 shubham    (501) staff       (20)     4057 2024-02-27 16:29:32.000000 hubble_exchange-0.9.0rc8/hubble_exchange/eip712.py
--rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.9.0rc8/hubble_exchange/errors.py
--rw-r--r--   0 shubham    (501) staff       (20)     8227 2024-03-11 07:01:02.000000 hubble_exchange-0.9.0rc8/hubble_exchange/eth.py
--rw-r--r--   0 shubham    (501) staff       (20)     1536 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc8/hubble_exchange/indexer_client.py
--rw-r--r--   0 shubham    (501) staff       (20)     9444 2024-01-22 15:50:54.000000 hubble_exchange-0.9.0rc8/hubble_exchange/models.py
--rw-r--r--   0 shubham    (501) staff       (20)    11852 2024-03-01 07:57:57.000000 hubble_exchange-0.9.0rc8/hubble_exchange/order_book.py
--rw-r--r--   0 shubham    (501) staff       (20)     3916 2024-01-31 08:10:44.000000 hubble_exchange-0.9.0rc8/hubble_exchange/utils.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-11 07:08:42.039803 hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)    20960 2024-03-11 07:08:42.000000 hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)     1164 2024-03-11 07:08:42.000000 hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2024-03-11 07:08:42.000000 hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)      117 2024-03-11 07:08:42.000000 hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       16 2024-03-11 07:08:42.000000 hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/top_level.txt
--rw-r--r--   0 shubham    (501) staff       (20)     1074 2024-03-11 07:08:00.000000 hubble_exchange-0.9.0rc8/pyproject.toml
--rw-r--r--   0 shubham    (501) staff       (20)       38 2024-03-11 07:08:42.040375 hubble_exchange-0.9.0rc8/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.9.0rc8/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-14 05:04:33.568610 hubble_exchange-0.9.0rc9/
+-rw-r--r--   0 shubham    (501) staff       (20)     1072 2023-06-28 09:55:40.000000 hubble_exchange-0.9.0rc9/LICENSE
+-rw-r--r--   0 shubham    (501) staff       (20)      134 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/MANIFEST.in
+-rw-r--r--   0 shubham    (501) staff       (20)    20960 2024-03-14 05:04:33.568294 hubble_exchange-0.9.0rc9/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)    19078 2024-02-03 16:04:30.000000 hubble_exchange-0.9.0rc9/README.md
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-14 05:04:33.550686 hubble_exchange-0.9.0rc9/hubble_exchange/
+-rw-r--r--   0 shubham    (501) staff       (20)      643 2024-01-22 15:57:19.000000 hubble_exchange-0.9.0rc9/hubble_exchange/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)    25889 2024-03-01 07:57:57.000000 hubble_exchange-0.9.0rc9/hubble_exchange/client.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-14 05:04:33.553428 hubble_exchange-0.9.0rc9/hubble_exchange/config/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2023-09-07 05:27:24.000000 hubble_exchange-0.9.0rc9/hubble_exchange/config/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1160 2024-01-18 15:44:33.000000 hubble_exchange-0.9.0rc9/hubble_exchange/config/aylin.py
+-rw-r--r--   0 shubham    (501) staff       (20)      899 2023-10-05 10:42:27.000000 hubble_exchange-0.9.0rc9/hubble_exchange/config/hubblenext.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1121 2024-02-25 09:51:44.000000 hubble_exchange-0.9.0rc9/hubble_exchange/config/local.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1162 2024-03-01 09:20:49.000000 hubble_exchange-0.9.0rc9/hubble_exchange/config/mainnet.py
+-rw-r--r--   0 shubham    (501) staff       (20)      739 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/constants.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-14 05:04:33.567348 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/
+-rw-r--r--   0 shubham    (501) staff       (20)    22218 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/AMM.json
+-rw-r--r--   0 shubham    (501) staff       (20)    25060 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/ClearingHouse.json
+-rw-r--r--   0 shubham    (501) staff       (20)    24834 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/HGT.json
+-rw-r--r--   0 shubham    (501) staff       (20)    27957 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/HGTRemote.json
+-rw-r--r--   0 shubham    (501) staff       (20)     4460 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/IERC20.json
+-rw-r--r--   0 shubham    (501) staff       (20)     7583 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/ImmediateOrCancelOrders.json
+-rw-r--r--   0 shubham    (501) staff       (20)    10987 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/LimitOrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     7118 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/MarginAccountHelper.json
+-rw-r--r--   0 shubham    (501) staff       (20)     4973 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/OrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)    10456 2024-01-16 14:11:20.000000 hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/SignedOrderBook.json
+-rw-r--r--   0 shubham    (501) staff       (20)     4057 2024-02-27 16:29:32.000000 hubble_exchange-0.9.0rc9/hubble_exchange/eip712.py
+-rw-r--r--   0 shubham    (501) staff       (20)       84 2023-07-14 06:05:29.000000 hubble_exchange-0.9.0rc9/hubble_exchange/errors.py
+-rw-r--r--   0 shubham    (501) staff       (20)     8232 2024-03-14 05:03:00.000000 hubble_exchange-0.9.0rc9/hubble_exchange/eth.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1536 2024-01-09 11:00:14.000000 hubble_exchange-0.9.0rc9/hubble_exchange/indexer_client.py
+-rw-r--r--   0 shubham    (501) staff       (20)     9444 2024-01-22 15:50:54.000000 hubble_exchange-0.9.0rc9/hubble_exchange/models.py
+-rw-r--r--   0 shubham    (501) staff       (20)    11852 2024-03-12 06:34:49.000000 hubble_exchange-0.9.0rc9/hubble_exchange/order_book.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3916 2024-01-31 08:10:44.000000 hubble_exchange-0.9.0rc9/hubble_exchange/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-03-14 05:04:33.567925 hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)    20960 2024-03-14 05:04:33.000000 hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)     1164 2024-03-14 05:04:33.000000 hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2024-03-14 05:04:33.000000 hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)      117 2024-03-14 05:04:33.000000 hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       16 2024-03-14 05:04:33.000000 hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/top_level.txt
+-rw-r--r--   0 shubham    (501) staff       (20)     1074 2024-03-14 05:03:05.000000 hubble_exchange-0.9.0rc9/pyproject.toml
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2024-03-14 05:04:33.568670 hubble_exchange-0.9.0rc9/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)       69 2023-06-29 07:08:06.000000 hubble_exchange-0.9.0rc9/setup.py
```

### Comparing `hubble_exchange-0.9.0rc8/LICENSE` & `hubble_exchange-0.9.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/PKG-INFO` & `hubble_exchange-0.9.0rc9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.9.0rc8
+Version: 0.9.0rc9
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hubble_exchange-0.9.0rc8/README.md` & `hubble_exchange-0.9.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/__init__.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/client.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/client.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/config/aylin.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/config/aylin.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/config/hubblenext.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/config/hubblenext.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/config/local.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/config/local.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/config/mainnet.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/config/mainnet.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/constants.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/constants.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/AMM.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/AMM.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/ClearingHouse.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/ClearingHouse.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/HGT.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/HGT.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/HGTRemote.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/HGTRemote.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/IERC20.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/ImmediateOrCancelOrders.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/ImmediateOrCancelOrders.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/LimitOrderBook.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/LimitOrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/MarginAccountHelper.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/MarginAccountHelper.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/OrderBook.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/OrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/contract_abis/SignedOrderBook.json` & `hubble_exchange-0.9.0rc9/hubble_exchange/contract_abis/SignedOrderBook.json`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/eip712.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/eip712.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/eth.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/eth.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             positions = [dict(position) for position in margin_response['positions']]
             for position in positions:
                 index_price = clearing_house_vars.underlying_prices[position['market']]
                 index_price = int_to_scaled_float(index_price, 6)
                 open_notional = float(position['openNotional'])
                 size = float(position['size'])
                 margin = float(margin_response['margin'])
-                notional_position = size * index_price
+                notional_position = abs(size * index_price)
                 uPnL = notional_position - open_notional if size > 0 else open_notional - notional_position
 
                 position['notionalPosition'] = round(notional_position, 6)
                 position['unrealisedProfit'] = round(uPnL, 6)
 
             margin_response['positions'] = [AttributeDict(position) for position in positions]
             margin_response = AttributeDict(margin_response)
```

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/indexer_client.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/indexer_client.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/models.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/models.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/order_book.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/order_book.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange/utils.py` & `hubble_exchange-0.9.0rc9/hubble_exchange/utils.py`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/PKG-INFO` & `hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubble_exchange
-Version: 0.9.0rc8
+Version: 0.9.0rc9
 Summary: Official python SDK for Hubble Exchange
 Author-email: Lumos <lumos@hubble.exchange>
 License: MIT License
         
         Copyright (c) 2023 Hubble Exchange
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hubble_exchange-0.9.0rc8/hubble_exchange.egg-info/SOURCES.txt` & `hubble_exchange-0.9.0rc9/hubble_exchange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hubble_exchange-0.9.0rc8/pyproject.toml` & `hubble_exchange-0.9.0rc9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 author_email = "lumos@hubble.exchange"
 long_description = {file = "README.md"}
 long_description_content_type = "text/markdown"
 url = "https://github.com/hubble-exchange/python-sdk"
 
 [project]
 name = "hubble_exchange"
-version = "0.9.0-rc8"
+version = "0.9.0-rc9"
 description = "Official python SDK for Hubble Exchange"
 authors = [{name = "Lumos", email = "lumos@hubble.exchange"}]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies = [
     "web3 >= 6.5.0",
     "eth_typing >= 3.4.0",
```

