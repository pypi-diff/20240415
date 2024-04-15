# Comparing `tmp/pragma_sdk-1.2.9.tar.gz` & `tmp/pragma_sdk-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pragma_sdk-1.2.9.tar", max compression
+gzip compressed data, was "pragma_sdk-1.3.0.tar", max compression
```

## Comparing `pragma_sdk-1.2.9.tar` & `pragma_sdk-1.3.0.tar`

### file list

```diff
@@ -1,63 +1,65 @@
--rw-r--r--   0        0        0      943 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/README.md
--rw-r--r--   0        0        0        0 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/__init__.py
--rw-r--r--   0        0        0      195 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/__init__.py
--rw-r--r--   0        0        0       55 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/abis/__init__.py
--rw-r--r--   0        0        0     1773 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/abis/abi.py
--rw-r--r--   0        0        0      375 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/abis/pragma_Admin.sierra.json
--rw-r--r--   0        0        0     6050 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/abis/pragma_ERC20.json
--rw-r--r--   0        0        0   140867 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/abis/pragma_ExampleRandomness.sierra.json
--rw-r--r--   0        0        0    34149 2024-03-08 15:07:18.719249 pragma_sdk-1.2.9/pragma/core/abis/pragma_MockOracle.sierra.json
--rw-r--r--   0        0        0  1704091 2024-03-08 15:07:18.727249 pragma_sdk-1.2.9/pragma/core/abis/pragma_Oracle.sierra.json
--rw-r--r--   0        0        0    42794 2024-03-08 15:07:18.727249 pragma_sdk-1.2.9/pragma/core/abis/pragma_Ownable.sierra.json
--rw-r--r--   0        0        0   275940 2024-03-08 15:07:18.727249 pragma_sdk-1.2.9/pragma/core/abis/pragma_PublisherRegistry.sierra.json
--rw-r--r--   0        0        0   544514 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/abis/pragma_Randomness.sierra.json
--rw-r--r--   0        0        0   323399 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/abis/pragma_SummaryStats.sierra.json
--rw-r--r--   0        0        0      686 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/abis/pragma_Upgradeable.sierra.json
--rw-r--r--   0        0        0   491352 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/abis/pragma_YieldCurve.sierra.json
--rw-r--r--   0        0        0     4009 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/assets.py
--rw-r--r--   0        0        0     6046 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/client.py
--rw-r--r--   0        0        0     1903 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/contract.py
--rw-r--r--   0        0        0    12551 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/entry.py
--rw-r--r--   0        0        0      393 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/logger.py
--rw-r--r--   0        0        0      344 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/__init__.py
--rw-r--r--   0        0        0     2992 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/nonce.py
--rw-r--r--   0        0        0     7303 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/offchain.py
--rw-r--r--   0        0        0    15773 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/oracle.py
--rw-r--r--   0        0        0     2505 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/publisher_registry.py
--rw-r--r--   0        0        0    13845 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/randomness.py
--rw-r--r--   0        0        0      669 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/mixins/transactions.py
--rw-r--r--   0        0        0        0 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/randomness/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/randomness/actions.py
--rw-r--r--   0        0        0    16307 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/randomness/randomness_utils.py
--rw-r--r--   0        0        0     1845 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/randomness/utils.py
--rw-r--r--   0        0        0    10170 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/types.py
--rw-r--r--   0        0        0     2598 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/core/utils.py
--rw-r--r--   0        0        0       59 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/publisher/__init__.py
--rw-r--r--   0        0        0    10305 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/publisher/client.py
--rw-r--r--   0        0        0      612 2024-03-08 15:07:18.731249 pragma_sdk-1.2.9/pragma/publisher/fetchers/__init__.py
--rw-r--r--   0        0        0     2751 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/ascendex.py
--rw-r--r--   0        0        0     4156 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/binance.py
--rw-r--r--   0        0        0     2345 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/bitstamp.py
--rw-r--r--   0        0        0     4385 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/bybit.py
--rw-r--r--   0        0        0     2843 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/cex.py
--rw-r--r--   0        0        0     2581 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/coinbase.py
--rw-r--r--   0        0        0     3115 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/coingecko.py
--rw-r--r--   0        0        0     5149 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/defillama.py
--rw-r--r--   0        0        0     6035 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/gecko.py
--rw-r--r--   0        0        0     2739 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/gemini.py
--rw-r--r--   0        0        0     4267 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/huobi.py
--rw-r--r--   0        0        0     3489 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/kaiko.py
--rw-r--r--   0        0        0     3970 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/kucoin.py
--rw-r--r--   0        0        0     2975 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/okx.py
--rw-r--r--   0        0        0     5648 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/propeller.py
--rw-r--r--   0        0        0     6164 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/starknetamm.py
--rw-r--r--   0        0        0     3952 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/thegraph.py
--rw-r--r--   0        0        0     2530 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/fetchers/upbit.py
--rw-r--r--   0        0        0      114 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/future_fetchers/__init__.py
--rw-r--r--   0        0        0     4872 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/future_fetchers/binance.py
--rw-r--r--   0        0        0     3177 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/future_fetchers/bybit.py
--rw-r--r--   0        0        0     4527 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/future_fetchers/okx.py
--rw-r--r--   0        0        0      892 2024-03-08 15:07:18.735249 pragma_sdk-1.2.9/pragma/publisher/types.py
--rw-r--r--   0        0        0     3926 2024-03-08 15:07:18.739249 pragma_sdk-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 pragma_sdk-1.2.9/setup.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pragma_sdk-1.2.9/PKG-INFO
+-rw-r--r--   0        0        0      943 2024-04-15 09:55:05.520861 pragma_sdk-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/__init__.py
+-rw-r--r--   0        0        0      195 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/abis/__init__.py
+-rw-r--r--   0        0        0     1773 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/abis/abi.py
+-rw-r--r--   0        0        0      375 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/abis/pragma_Admin.sierra.json
+-rw-r--r--   0        0        0     6050 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/abis/pragma_ERC20.json
+-rw-r--r--   0        0        0   140867 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/abis/pragma_ExampleRandomness.sierra.json
+-rw-r--r--   0        0        0    34149 2024-04-15 09:55:05.524861 pragma_sdk-1.3.0/pragma/core/abis/pragma_MockOracle.sierra.json
+-rw-r--r--   0        0        0  1704091 2024-04-15 09:55:05.532861 pragma_sdk-1.3.0/pragma/core/abis/pragma_Oracle.sierra.json
+-rw-r--r--   0        0        0    42794 2024-04-15 09:55:05.532861 pragma_sdk-1.3.0/pragma/core/abis/pragma_Ownable.sierra.json
+-rw-r--r--   0        0        0   275940 2024-04-15 09:55:05.532861 pragma_sdk-1.3.0/pragma/core/abis/pragma_PublisherRegistry.sierra.json
+-rw-r--r--   0        0        0   544514 2024-04-15 09:55:05.532861 pragma_sdk-1.3.0/pragma/core/abis/pragma_Randomness.sierra.json
+-rw-r--r--   0        0        0   323399 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/abis/pragma_SummaryStats.sierra.json
+-rw-r--r--   0        0        0      686 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/abis/pragma_Upgradeable.sierra.json
+-rw-r--r--   0        0        0   491352 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/abis/pragma_YieldCurve.sierra.json
+-rw-r--r--   0        0        0     5669 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/assets.py
+-rw-r--r--   0        0        0     6046 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/client.py
+-rw-r--r--   0        0        0     1904 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/contract.py
+-rw-r--r--   0        0        0    12550 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/entry.py
+-rw-r--r--   0        0        0      393 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/logger.py
+-rw-r--r--   0        0        0      344 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/__init__.py
+-rw-r--r--   0        0        0     4013 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/nonce.py
+-rw-r--r--   0        0        0     7303 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/offchain.py
+-rw-r--r--   0        0        0    15904 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/oracle.py
+-rw-r--r--   0        0        0     2505 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/publisher_registry.py
+-rw-r--r--   0        0        0    13949 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/randomness.py
+-rw-r--r--   0        0        0      669 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/mixins/transactions.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/randomness/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/randomness/actions.py
+-rw-r--r--   0        0        0    16307 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/randomness/randomness_utils.py
+-rw-r--r--   0        0        0     1845 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/randomness/utils.py
+-rw-r--r--   0        0        0    11222 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/types.py
+-rw-r--r--   0        0        0     2598 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/core/utils.py
+-rw-r--r--   0        0        0       59 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/__init__.py
+-rw-r--r--   0        0        0    10464 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/client.py
+-rw-r--r--   0        0        0      684 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/ascendex.py
+-rw-r--r--   0        0        0     4600 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/binance.py
+-rw-r--r--   0        0        0     2346 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/bitstamp.py
+-rw-r--r--   0        0        0     4827 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/bybit.py
+-rw-r--r--   0        0        0     2843 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/cex.py
+-rw-r--r--   0        0        0     2581 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/coinbase.py
+-rw-r--r--   0        0        0     3259 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/coingecko.py
+-rw-r--r--   0        0        0     5158 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/defillama.py
+-rw-r--r--   0        0        0     7706 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/gecko.py
+-rw-r--r--   0        0        0     2739 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/gemini.py
+-rw-r--r--   0        0        0     4645 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/huobi.py
+-rw-r--r--   0        0        0     3219 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/index.py
+-rw-r--r--   0        0        0     3836 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/indexcoop.py
+-rw-r--r--   0        0        0     3489 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/kaiko.py
+-rw-r--r--   0        0        0     4226 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/kucoin.py
+-rw-r--r--   0        0        0     3366 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/okx.py
+-rw-r--r--   0        0        0     6580 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/propeller.py
+-rw-r--r--   0        0        0     6225 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/starknetamm.py
+-rw-r--r--   0        0        0     5100 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/thegraph.py
+-rw-r--r--   0        0        0     2530 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/fetchers/upbit.py
+-rw-r--r--   0        0        0      114 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/future_fetchers/__init__.py
+-rw-r--r--   0        0        0     4871 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/future_fetchers/binance.py
+-rw-r--r--   0        0        0     3177 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/future_fetchers/bybit.py
+-rw-r--r--   0        0        0     4527 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/future_fetchers/okx.py
+-rw-r--r--   0        0        0     1199 2024-04-15 09:55:05.536861 pragma_sdk-1.3.0/pragma/publisher/types.py
+-rw-r--r--   0        0        0     4102 2024-04-15 09:55:05.544861 pragma_sdk-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 pragma_sdk-1.3.0/setup.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 pragma_sdk-1.3.0/PKG-INFO
```

### Comparing `pragma_sdk-1.2.9/README.md` & `pragma_sdk-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/abi.py` & `pragma_sdk-1.3.0/pragma/core/abis/abi.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_ERC20.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_ERC20.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_ExampleRandomness.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_ExampleRandomness.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_MockOracle.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_MockOracle.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_Oracle.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_Oracle.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_Ownable.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_Ownable.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_PublisherRegistry.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_PublisherRegistry.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_Randomness.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_Randomness.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_SummaryStats.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_SummaryStats.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_Upgradeable.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_Upgradeable.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/abis/pragma_YieldCurve.sierra.json` & `pragma_sdk-1.3.0/pragma/core/abis/pragma_YieldCurve.sierra.json`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/client.py` & `pragma_sdk-1.3.0/pragma/core/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,35 +40,35 @@
     is_user_client: bool = False
     account_contract_address: Optional[int] = None
     account: Account = None
     full_node_client: FullNodeClient = None
 
     def __init__(
         self,
-        network: str = "testnet",
+        network: str = "sepolia",
         account_private_key: Optional[int] = None,
         account_contract_address: Optional[int] = None,
         contract_addresses_config: Optional[ContractAddresses] = None,
         port: Optional[int] = None,
         chain_name: Optional[str] = None,
         api_url: Optional[str] = PRAGMA_API_URL,
         api_key: Optional[str] = None,
     ):
         """
         Client for interacting with Pragma on Starknet.
         :param network: Target network for the client.
             Can be a URL string, or one of
-            ``"mainnet"``, ``"testnet"``, ``"pragma_testnet"``, ``"sharingan"`` or ``"devnet"``
+            ``"mainnet"``, ``"sepolia"``, ``"pragma_testnet"``, ``"sharingan"`` or ``"devnet"``
         :param account_private_key: Optional private key for requests.  Not necessary if not making network updates
         :param account_contract_address: Optional account contract address.  Not necessary if not making network updates
         :param contract_addresses_config: Optional Contract Addresses for Pragma.
             Will default to the provided network but must be set if using non standard contracts.
         :param port: Optional port to interact with local node. Will default to 5050.
         :param chain_name: A str-representation of the chain if a URL string is given for `network`.
-            Must be one of ``"mainnet"``, ``"testnet"``, ``"pragma_testnet"``, ``"sharingan"`` or ``"devnet"``.
+            Must be one of ``"mainnet"``, ``"sepolia"``, ``"pragma_testnet"``, ``"sharingan"`` or ``"devnet"``.
         :param api_url: Optional URL for the Pragma API.  Defaults to http://localhost:8080
         :param api_key: Optional API key for the Pragma API.
         """
         self.ssl_context = None
         self.api_url = api_url
 
         if api_key is not None:
```

### Comparing `pragma_sdk-1.2.9/pragma/core/contract.py` & `pragma_sdk-1.3.0/pragma/core/contract.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,26 +43,25 @@
 
     transaction = await self.get_account.sign_invoke_v1(
         calls=self,
         max_fee=self.max_fee,
         auto_estimate=auto_estimate,
     )
     response = await self._client.send_transaction(transaction)
-
     if callback:
         await callback(transaction.nonce, response.transaction_hash)
 
     invoke_result = InvokeResult(
         hash=response.transaction_hash,
         _client=self._client,
         contract=self._contract_data,
         invoke_transaction=transaction,
     )
 
     # don't return invoke result until it is received or errors
-    await invoke_result.wait_for_acceptance()
+    # await invoke_result.wait_for_acceptance()
 
     return invoke_result
 
 
 # patch contract function to use new invoke function
 ContractFunction.invoke_v1 = invoke_
```

### Comparing `pragma_sdk-1.2.9/pragma/core/entry.py` & `pragma_sdk-1.3.0/pragma/core/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 from pragma.core.assets import get_asset_spec_for_pair_id_by_type
 from pragma.core.utils import felt_to_str, str_to_felt
 
 
 class Entry(abc.ABC):
     @abc.abstractmethod
-    def serialize(self) -> Dict[str, str]:
-        ...
+    def serialize(self) -> Dict[str, str]: ...
 
     @abc.abstractmethod
-    def to_tuple(self) -> Tuple:
-        ...
+    def to_tuple(self) -> Tuple: ...
 
     @staticmethod
     def serialize_entries(entries: List[Entry]) -> List[Dict[str, int]]:
         serialized_entries = [
             entry.serialize() for entry in entries if issubclass(entry, Entry)
         ]
         return list(filter(lambda item: item is not None, serialized_entries))
@@ -82,15 +80,15 @@
         if isinstance(source, str):
             source = str_to_felt(source)
 
         self.base = BaseEntry(timestamp, source, publisher)
         self.pair_id = pair_id
         self.price = price
 
-        if autoscale_volume:
+        if volume > 0 and autoscale_volume:
             asset = get_asset_spec_for_pair_id_by_type(felt_to_str(pair_id), "SPOT")
             decimals = asset["decimals"] or 0
             volume = volume or 0
 
             self.volume = int(volume * price * 10**decimals)
         else:
             self.volume = volume
```

### Comparing `pragma_sdk-1.2.9/pragma/core/mixins/offchain.py` & `pragma_sdk-1.3.0/pragma/core/mixins/offchain.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/mixins/oracle.py` & `pragma_sdk-1.3.0/pragma/core/mixins/oracle.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,15 @@
                     len(entries_subset),
                     hex(invocation.hash),
                 )
         elif len(serialized_spot_entries) > 0:
             invocation = await self.oracle.functions["publish_data_entries"].invoke_v1(
                 new_entries=[{"Spot": entry} for entry in serialized_spot_entries],
                 max_fee=max_fee,
+                callback=self.track_nonce,
             )
             invocations.append(invocation)
             logger.debug(str(invocation))
             logger.info(
                 "Sent %d updated spot entries with transaction %s",
                 len(serialized_spot_entries),
                 hex(invocation.hash),
@@ -119,27 +120,29 @@
             while index < len(serialized_future_entries):
                 entries_subset = serialized_future_entries[index : index + pagination]
                 invocation = await self.oracle.functions[
                     "publish_data_entries"
                 ].invoke_v1(
                     new_entries=[{"Future": entry} for entry in entries_subset],
                     max_fee=max_fee,
+                    callback=self.track_nonce,
                 )
                 index += pagination
                 invocations.append(invocation)
                 logger.debug(str(invocation))
                 logger.info(
                     "Sent %d updated future entries with transaction %s",
                     len(entries_subset),
                     hex(invocation.hash),
                 )
         elif len(serialized_future_entries) > 0:
             invocation = await self.oracle.functions["publish_data_entries"].invoke_v1(
                 new_entries=[{"Future": entry} for entry in serialized_future_entries],
                 max_fee=max_fee,
+                callback=self.track_nonce,
             )
             invocations.append(invocation)
             logger.debug(str(invocation))
             logger.info(
                 "Sent %d updated future entries with transaction %s",
                 len(serialized_future_entries),
                 hex(invocation.hash),
@@ -410,22 +413,24 @@
             implementation_hash,
             max_fee=max_fee,
         )
         return invocation
 
     async def get_time_since_last_published(self, pair_id, publisher) -> int:
         all_entries = await self.get_spot_entries(pair_id)
-        if len(all_entries) == 0:
-            return 1000000000  # arbitrary large number
 
         entries = [
             entry
             for entry in all_entries
             if entry.base.publisher == str_to_felt(publisher)
         ]
+
+        if len(entries) == 0:
+            return 1000000000  # arbitrary large number
+
         max_timestamp = max([entry.base.timestamp for entry in entries])
 
         diff = int(time.time()) - max_timestamp
 
         return diff
 
     async def get_current_price_deviation(self, pair_id) -> float:
```

### Comparing `pragma_sdk-1.2.9/pragma/core/mixins/publisher_registry.py` & `pragma_sdk-1.3.0/pragma/core/mixins/publisher_registry.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/mixins/randomness.py` & `pragma_sdk-1.3.0/pragma/core/mixins/randomness.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         calldata: List[int] = [],
         max_fee=int(1e16),
     ):
         if not self.is_user_client:
             raise AttributeError(
                 "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
             )
-        prepared_call = self.randomness.functions["request_random"].prepare(
+        prepared_call = self.randomness.functions["request_random"].prepare_invoke_v1(
             seed,
             callback_address,
             callback_fee_limit,
             publish_delay,
             num_words,
             calldata,
             max_fee=max_fee,
@@ -86,15 +86,17 @@
         return estimate_fee
 
     async def estimate_gas_call(self, caller_address: int, method: str):
         if not self.is_user_client:
             raise AttributeError(
                 "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
             )
-        prepared_call = self.randomness.functions[method].prepare(caller_address)
+        prepared_call = self.randomness.functions[method].prepare_invoke_v1(
+            caller_address
+        )
         estimate_fee = await prepared_call.estimate_fee()
         return estimate_fee
 
     async def submit_random(
         self,
         request_id: int,
         requestor_address: int,
@@ -107,15 +109,15 @@
         calldata: List[int],
         max_fee=int(1e16),
     ) -> InvokeResult:
         if not self.is_user_client:
             raise AttributeError(
                 "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
             )
-        prepared_call = self.randomness.functions["submit_random"].prepare(
+        prepared_call = self.randomness.functions["submit_random"].prepare_invoke_v1(
             request_id,
             requestor_address,
             seed,
             minimum_block_number,
             callback_address,
             callback_fee_limit,
             callback_fee_limit,
@@ -175,15 +177,15 @@
         calldata: List[int],
         max_fee=int(1e16),
     ):
         if not self.is_user_client:
             raise AttributeError(
                 "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
             )
-        prepared_call = self.randomness.functions["submit_random"].prepare(
+        prepared_call = self.randomness.functions["submit_random"].prepare_invoke_v1(
             request_id,
             requestor_address,
             seed,
             minimum_block_number,
             callback_address,
             callback_fee_limit,
             callback_fee_limit,
@@ -200,15 +202,15 @@
         requestor_address,
         request_id,
     ):
         if not self.is_user_client:
             raise AttributeError(
                 "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
             )
-        prepared_call = self.randomness.functions["update_status"].prepare(
+        prepared_call = self.randomness.functions["update_status"].prepare_invoke_v1(
             requestor_address,
             request_id,
             RequestStatus.RECEIVED.serialize(),
         )
         estimate_fee = await prepared_call.estimate_fee()
         return estimate_fee
 
@@ -297,15 +299,17 @@
         num_words: int,
         max_fee=int(1e16),
     ):
         if not self.is_user_client:
             raise AttributeError(
                 "Must set account.  You may do this by invoking self._setup_account_client(private_key, account_contract_address)"
             )
-        prepared_call = self.randomness.functions["cancel_random_request"].prepare(
+        prepared_call = self.randomness.functions[
+            "cancel_random_request"
+        ].prepare_invoke_v1(
             request_id,
             requestor_address,
             seed,
             minimum_block_number,
             callback_address,
             callback_fee_limit,
             num_words,
```

### Comparing `pragma_sdk-1.2.9/pragma/core/mixins/transactions.py` & `pragma_sdk-1.3.0/pragma/core/mixins/transactions.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/randomness/randomness_utils.py` & `pragma_sdk-1.3.0/pragma/core/randomness/randomness_utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/randomness/utils.py` & `pragma_sdk-1.3.0/pragma/core/randomness/utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/core/types.py` & `pragma_sdk-1.3.0/pragma/core/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,43 +14,41 @@
 
 
 ADDRESS = int
 HEX_STR = str  # pylint: disable=invalid-name
 
 # Network Types
 DEVNET = "devnet"
-TESTNET = "testnet"
 SEPOLIA = "sepolia"
 MAINNET = "mainnet"
 SHARINGAN = "sharingan"
 FORK_DEVNET = "fork_devnet"
 PRAGMA_TESTNET = "pragma_testnet"
 
 Network = Literal[
     "devnet",
-    "testnet",
     "mainnet",
     "sharingan",
     "pragma_testnet",
     "fork_devnet",
     "sepolia",
 ]
 
 CHAIN_IDS = {
     DEVNET: 1536727068981429685321,
     SHARINGAN: 1536727068981429685321,
-    TESTNET: 1536727068981429685321,
     MAINNET: 23448594291968334,
     PRAGMA_TESTNET: 8908953246943201047421899664489,
     FORK_DEVNET: 1536727068981429685321,
     SEPOLIA: 393402133025997798000961,
 }
 
 ASSET_MAPPING: Dict[str, str] = {
     "ETH": "ethereum",
+    "WETH": "weth",
     "BTC": "bitcoin",
     "WBTC": "wrapped-bitcoin",
     "SOL": "solana",
     "AVAX": "avalanche-2",
     "DOGE": "dogecoin",
     "SHIB": "shiba-inu",
     "TEMP": "tempus",
@@ -66,49 +64,79 @@
     "AAVE": "aave",
     "R": "r",
     "LORDS": "lords",
     "WSTETH": "wrapped-steth",
     "UNI": "uniswap",
     "LUSD": "liquity-usd",
     "STRK": "starknet",
+    "MKR": "maker",
+    "BAL": "balancer",
+    "ZEND": "zklend-2",
+    "LDO": "lido-dao",
+    "SNX": "havven",
+    "RPL": "rocket-pool",
+    "YFI": "yearn-finance",
+    "COMP": "compound-governance-token",
+    "DPI": "defipulse-index",
+    "MVI": "metaverse-index",
 }
 
+DPI_ASSETS = [
+    {"type": "SPOT", "pair": ("YFI", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("COMP", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("SNX", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("MKR", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("BAL", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("UNI", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("AAVE", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("LDO", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("ETH", "USD"), "decimals": 8},
+]
+
+MVI_ASSETS = [
+    {"type": "SPOT", "pair": ("MC", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("RNDR", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("FET", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("IMX", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("GALA", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("ILV", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("APE", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("SAND", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("AXS", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("MANA", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("ENS", "USD"), "decimals": 8},
+    {"type": "SPOT", "pair": ("BLUR", "USD"), "decimals": 8},
+]
+
 CHAIN_ID_TO_NETWORK = {v: k for k, v in CHAIN_IDS.items()}
 
 STARKSCAN_URLS = {
     MAINNET: "https://starkscan.co",
-    TESTNET: "https://testnet.starkscan.co",
     SEPOLIA: "https://sepolia.starkscan.co",
     DEVNET: "https://devnet.starkscan.co",
     SHARINGAN: "https://sharingan-explorer.madara.zone",
     PRAGMA_TESTNET: "https://testnet.pragmaoracle.com/explorer",
     FORK_DEVNET: "https://devnet.starkscan.co",
 }
 
 PRAGMA_API_URL = "https://api.dev.pragma.build/node"
 
 RPC_URLS = {
     MAINNET: [
         "https://starknet-mainnet.public.blastapi.io/rpc/v0_6",
     ],
-    TESTNET: [
-        "https://starknet-testnet.public.blastapi.io/rpc/v0_6",
-    ],
     SEPOLIA: [
         "https://starknet-sepolia.public.blastapi.io/rpc/v0_6",
     ],
 }
 
 
-def get_rpc_url(network=TESTNET, port=5050):
+def get_rpc_url(network=SEPOLIA, port=5050):
     if network.startswith("http"):
         return network
-    if network == TESTNET:
-        random_index = random.randint(0, len(RPC_URLS[TESTNET]) - 1)
-        return RPC_URLS[TESTNET][random_index]
     if network == SEPOLIA:
         random_index = random.randint(0, len(RPC_URLS[SEPOLIA]) - 1)
         return RPC_URLS[SEPOLIA][random_index]
     if network == MAINNET:
         random_index = random.randint(0, len(RPC_URLS[MAINNET]) - 1)
         return RPC_URLS[MAINNET][random_index]
     if network == SHARINGAN:
@@ -131,18 +159,14 @@
 class ContractAddresses:
     publisher_registry_address: int
     oracle_proxy_addresss: int
 
 
 CONTRACT_ADDRESSES = {
     DEVNET: ContractAddresses(0, 0),
-    TESTNET: ContractAddresses(
-        2408056700008799988274832007944460979526684291270693941276336026156441738630,
-        3108238389225984732543655444430831893780207443780498125530192910262931411303,
-    ),
     MAINNET: ContractAddresses(
         1035964020232444284030697086969999610062982650901949616270651804992179237909,
         1202089834814778579992154020333959781277480478747022471664051891421849487195,
     ),
     SEPOLIA: ContractAddresses(
         764259049439565269590387705502051444787910047543242149334355727309682685773,
         1526899943909931281366530977873767661043021921869578496106478460498705257242,
```

### Comparing `pragma_sdk-1.2.9/pragma/core/utils.py` & `pragma_sdk-1.3.0/pragma/core/utils.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/publisher/client.py` & `pragma_sdk-1.3.0/pragma/publisher/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 import asyncio
-import http.client
-import json
-import os
 import time
 from typing import Dict, List
 
 import aiohttp
-import requests
 from dotenv import load_dotenv
 
 from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import get_cur_from_pair
 from pragma.publisher.types import PublisherInterfaceT
 
@@ -133,24 +129,30 @@
         for fetcher in self.fetchers:
             data = fetcher._fetch_sync()
             results.extend(data)
         return results
 
 
 class PragmaAPIClient(PragmaClient):
-    api_base_ur: str
+    api_base_url: str
     api_key: str
 
     def __init__(
         self,
+        account_private_key,
+        account_contract_address,
         api_base_url,
         api_key,
     ):
         self.api_base_url = api_base_url
         self.api_key = api_key
+        super().__init__(
+            account_private_key=account_private_key,
+            account_contract_address=account_contract_address,
+        )
 
     @staticmethod
     def convert_to_publisher(client: PragmaClient):
         client.__class__ = PragmaAPIClient
         return client
 
     async def api_get_ohlc(
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/__init__.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,13 +5,15 @@
 from .cex import CexFetcher
 from .coinbase import CoinbaseFetcher
 from .coingecko import CoingeckoFetcher
 from .defillama import DefillamaFetcher
 from .gecko import GeckoTerminalFetcher
 from .gemini import GeminiFetcher
 from .huobi import HuobiFetcher
+from .index import IndexFetcher
+from .indexcoop import IndexCoopFetcher
 from .kaiko import KaikoFetcher
 from .kucoin import KucoinFetcher
 from .okx import OkxFetcher
 from .propeller import PropellerFetcher
 from .starknetamm import StarknetAMMFetcher
 from .thegraph import TheGraphFetcher
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/ascendex.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/upbit.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,70 +9,66 @@
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
+SUPPORTED_ASSETS = [("BTC", "ETH")]
 
-class AscendexFetcher(PublisherInterfaceT):
-    BASE_URL: str = "https://ascendex.com/api/pro/v1/spot/ticker"
-    SOURCE: str = "ASCENDEX"
+
+class UpbitFetcher(PublisherInterfaceT):
+    BASE_URL: str = "https://sg-api.upbit.com/v1/ticker"
+    SOURCE: str = "UPBIT"
 
     publisher: str
 
     def __init__(self, assets: List[PragmaAsset], publisher):
         self.assets = assets
         self.publisher = publisher
 
     async def _fetch_pair(
         self, asset: PragmaSpotAsset, session: ClientSession
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
-        url = f"{self.BASE_URL}?symbol={pair[0]}/{pair[1]}"
+        url = self.format_url(pair[0], pair[1])
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from Ascendex"
+                    f"No data found for {'/'.join(pair)} from Upbit"
                 )
             result = await resp.json()
-            if result["code"] == 100002 and result["reason"] == "DATA_NOT_AVAILABLE":
-                return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from Ascendex"
-                )
-
             return self._construct(asset, result)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
         for asset in self.assets:
-            if asset["type"] != "SPOT":
-                logger.debug("Skipping Ascendex for non-spot asset %s", asset)
+            if asset["type"] == "SPOT" and asset["pair"] in SUPPORTED_ASSETS:
+                entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
+            else:
+                logger.debug("Skipping Upbit for non-spot asset %s", asset)
                 continue
-            entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
-        url = f"{self.BASE_URL}?symbol={quote_asset}/{base_asset}"
+        url = f"{self.BASE_URL}?markets={quote_asset}-{base_asset}"
         return url
 
     def _construct(self, asset, result) -> SpotEntry:
         pair = asset["pair"]
-        data = result["data"]
+        data = result[0]
         timestamp = int(time.time())
-        ask = float(data["ask"][0])
-        bid = float(data["bid"][0])
-        price = (ask + bid) / 2.0
+        price = float(data["trade_price"])
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
-        volume = float(data["volume"])
+        volume = float(data["trade_volume"])
 
-        logger.info("Fetched price %d for %s from Ascendex", price, "/".join(pair))
+        logger.info("Fetched price %d for %s from Upbit", price, "/".join(pair))
 
         return SpotEntry(
             pair_id=pair_id,
             price=price_int,
             volume=volume,
             timestamp=timestamp,
             source=self.SOURCE,
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/binance.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/binance.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,57 +3,65 @@
 import time
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
 class BinanceFetcher(PublisherInterfaceT):
     BASE_URL: str = "https://api.binance.com/api/v3/ticker/24hr"
     SOURCE: str = "BINANCE"
-
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher):
+    def __init__(self, assets: List[PragmaAsset], publisher, client=None):
         self.assets = assets
         self.publisher = publisher
+        self.client = client or PragmaClient(network="mainnet")
 
     async def _fetch_pair(
-        self, asset: PragmaSpotAsset, session: ClientSession
+        self, asset: PragmaSpotAsset, session: ClientSession, usdt_price=1
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
 
         # For now still leaving this line,
-        if pair == ("STRK", "USD"):
-            pair = ("STRK", "USDT")
+        if pair[1] == "USD":
+            pair = (pair[0], "USDT")
+        if pair[0] == "WETH":
+            pair = ("ETH", pair[1])
+        else:
+            usdt_price = 1
         url = self.format_url(pair[0], pair[1])
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Binance"
                 )
             result = await resp.json()
             if "code" in result:
                 return await self.operate_usdt_hop(asset, session)
-            return self._construct(asset, result)
+            return self._construct(asset=asset, result=result, usdt_price=usdt_price)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
+        usdt_price = await self.get_stable_price(self.client, "USDT")
         for asset in self.assets:
             if asset["type"] == "SPOT":
-                entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
+                entries.append(
+                    asyncio.ensure_future(self._fetch_pair(asset, session, usdt_price))
+                )
             else:
                 logger.debug("Skipping Binance for non-spot asset %s", asset)
                 continue
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
         url = f"{self.BASE_URL}?symbol={quote_asset}{base_asset}"
@@ -79,21 +87,21 @@
                     f"No data found for {'/'.join(pair)} from Binance - hop failed for {pair[1]}"
                 )
             pair2_usdt = await resp.json()
             if "code" in pair2_usdt:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Binance - hop failed for {pair[1]}"
                 )
-        return self._construct(asset, pair2_usdt, pair1_usdt)
+        return self._construct(asset=asset, result=pair2_usdt, hop_result=pair1_usdt)
 
-    def _construct(self, asset, result, hop_result=None) -> SpotEntry:
+    def _construct(self, asset, result, hop_result=None, usdt_price=1) -> SpotEntry:
         pair = asset["pair"]
         bid = float(result["bidPrice"])
         ask = float(result["askPrice"])
-        price = (bid + ask) / 2
+        price = (bid + ask) / (2 * usdt_price)
         if hop_result is not None:
             hop_bid = float(hop_result["bidPrice"])
             hop_ask = float(hop_result["askPrice"])
             hop_price = (hop_bid + hop_ask) / 2
             price = hop_price / price
         timestamp = int(time.time())
         price_int = int(price * (10 ** asset["decimals"]))
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/bitstamp.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/bitstamp.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
                 )
             return self._construct(asset, await resp.json())
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
+
         for asset in self.assets:
             if asset["type"] != "SPOT":
                 logger.debug("Skipping Bitstamp for non-spot asset %s", asset)
                 continue
             entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
         return await asyncio.gather(*entries, return_exceptions=True)
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/bybit.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/bybit.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,64 +3,70 @@
 import time
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
 class BybitFetcher(PublisherInterfaceT):
     BASE_URL: str = "https://api.bybit.com/v5/market/tickers?category=spot&"
     SOURCE: str = "BYBIT"
-
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher):
+    def __init__(self, assets: List[PragmaAsset], publisher, client=None):
         self.assets = assets
         self.publisher = publisher
+        self.client = client or PragmaClient(network="mainnet")
 
     async def _fetch_pair(
-        self, asset: PragmaSpotAsset, session: ClientSession
+        self, asset: PragmaSpotAsset, session: ClientSession, usdt_price=1
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
-        if pair == ("STRK", "USD"):
-            pair = ("STRK", "USDT")
+        if pair[1] == "USD":
+            pair = (pair[0], "USDT")
+        else:
+            usdt_price = 1
         url = self.format_url(pair[0], pair[1])
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Bybit"
                 )
             result = await resp.json()
             if result["retCode"] == 10001:
                 return await self.operate_usdt_hop(asset, session)
-            return self._construct(asset, result)
+            return self._construct(asset=asset, result=result, usdt_price=usdt_price)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
+        usdt_price = await self.get_stable_price(self.client, "USDT")
         for asset in self.assets:
             if asset["type"] != "SPOT":
                 logger.debug("Skipping Bybit for non-spot asset %s", asset)
                 continue
-            entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
+            entries.append(
+                asyncio.ensure_future(self._fetch_pair(asset, session, usdt_price))
+            )
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
         url = f"{self.BASE_URL}symbol={quote_asset}{base_asset}"
         return url
 
-    async def operate_usdt_hop(self, asset, session) -> SpotEntry:
+    async def operate_usdt_hop(self, asset, session, usdt_price=None) -> SpotEntry:
         pair = asset["pair"]
         url_pair1 = self.format_url(asset["pair"][0], "USDT")
         async with session.get(url_pair1) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Bybit - hop failed for {pair[0]}"
                 )
@@ -76,21 +82,23 @@
                     f"No data found for {'/'.join(pair)} from Bybit - hop failed for {pair[1]}"
                 )
             pair2_usdt = await resp.json()
             if pair2_usdt["retCode"] == 10001:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Bybit - hop failed for {pair[1]}"
                 )
-        return self._construct(asset, pair2_usdt, pair1_usdt)
+        return self._construct(asset=asset, result=pair2_usdt, hop_result=pair1_usdt)
 
-    def _construct(self, asset, result, hop_result=None) -> SpotEntry:
+    def _construct(self, asset, result, hop_result=None, usdt_price=1) -> SpotEntry:
         pair = asset["pair"]
+        if pair[0] == "BAL":
+            print(result)
         bid = float(result["result"]["list"][0]["bid1Price"])
         ask = float(result["result"]["list"][0]["ask1Price"])
-        price = (bid + ask) / 2
+        price = (bid + ask) / (2 * usdt_price)
         if hop_result is not None:
             hop_bid = float(hop_result["result"]["list"][0]["bid1Price"])
             hop_ask = float(hop_result["result"]["list"][0]["ask1Price"])
             hop_price = (hop_bid + hop_ask) / 2
             price = hop_price / price
         timestamp = int(time.time())
         price_int = int(price * (10 ** asset["decimals"]))
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/cex.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/cex.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/coinbase.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/coinbase.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/coingecko.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/coingecko.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
     "TUSD": "true-usd",
     "BUSD": "binance-usd",
     "BNB": "binancecoin",
     "ADA": "cardano",
     "XRP": "ripple",
     "MATIC": "matic-network",
     "AAVE": "aave",
+    "MKR": "maker",
+    "BAL": "balancer",
 }
 
 
 class CoingeckoFetcher(PublisherInterfaceT):
     BASE_URL: str = (
         "https://api.coingecko.com/api/v3/coins/{pair_id}"
         "?localization=false&market_data=true&community_data=false"
@@ -58,16 +60,15 @@
     ) -> SpotEntry:
         pair = asset["pair"]
         pair_id = ASSET_MAPPING.get(pair[0])
         if pair_id is None:
             return PublisherFetchError(
                 f"Unknown price pair, do not know how to query Coingecko for {pair[0]}"
             )
-        url = self.BASE_URL.format(pair_id=pair_id)
-
+        url = self.format_url(pair_id=pair_id)
         async with session.get(
             url, headers=self.headers, raise_for_status=True
         ) as resp:
             result = await resp.json()
             return self._construct(asset, result)
 
     async def fetch(self, session: ClientSession) -> List[SpotEntry]:
@@ -75,14 +76,18 @@
         for asset in self.assets:
             if asset["type"] != "SPOT":
                 logger.debug("Skipping %s for non-spot asset %s", self.SOURCE, asset)
                 continue
             entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
         return await asyncio.gather(*entries, return_exceptions=True)
 
+    def format_url(self, pair_id):
+        url = self.BASE_URL.format(pair_id=pair_id)
+        return url
+
     def _construct(self, asset, result) -> SpotEntry:
         pair = asset["pair"]
         pair_id = currency_pair_to_pair_id(*pair)
         price = result["market_data"]["current_price"][pair[1].lower()]
         price_int = int(price * (10 ** asset["decimals"]))
         timestamp = int(
             datetime.datetime.strptime(
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/defillama.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/defillama.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
 class DefillamaFetcher(PublisherInterfaceT):
     BASE_URL: str = (
-        "https://coins.llama.fi/prices/current/coingecko:{pair_id}" "?searchWidth=5m"
+        "https://coins.llama.fi/prices/current/coingecko:{pair_id}" "?searchWidth=15m"
     )
 
     SOURCE: str = "DEFILLAMA"
     api_key: str
 
     headers: dict
 
@@ -52,16 +52,15 @@
                     f"No data found for {'/'.join(pair)} from Defillama"
                 )
             result = await resp.json()
             if not result["coins"]:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Defillama"
                 )
-
-        return self._construct(asset=asset, result=result)
+        return self._construct(asset, result)
 
     async def fetch(self, session: ClientSession) -> List[SpotEntry]:
         entries = []
         for asset in self.assets:
             if asset["type"] != "SPOT":
                 logger.debug("Skipping %s for non-spot asset %s", self.SOURCE, asset)
                 continue
@@ -117,14 +116,15 @@
             price_int = int((price / hop_price) * (10 ** asset["decimals"]))
         else:
             price = result["coins"][f"coingecko:{base_id}"]["price"]
             price_int = int(price * (10 ** asset["decimals"]))
 
         logger.info("Fetched price %d for %s from Coingecko", price, pair_id)
 
-        return SpotEntry(
+        entry = SpotEntry(
             pair_id=pair_id,
             price=price_int,
             timestamp=timestamp,
             source=self.SOURCE,
             publisher=self.publisher,
         )
+        return entry
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/gecko.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/gecko.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,14 +26,44 @@
     "ETH": ("eth", "0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2"),
     "UNI": ("eth", "0x1f9840a85d5af5bf1d1762f925bdaddc4201f984"),
     "LUSD": ("eth", "0x5f98805a4e8be255a32880fdec7f6728c6568ba0"),
     "STRK": (
         "starknet-alpha",
         "0x4718f5a0fc34cc1af16a1cdee98ffb20c31f5cd61d6ab07201858f4287c938d",
     ),
+    "ZEND": (
+        "starknet-alpha",
+        "0x00585c32b625999e6e5e78645ff8df7a9001cf5cf3eb6b80ccdd16cb64bd3a34",
+    ),
+    "YFI": (
+        "eth",
+        "0x0bc529c00C6401aEF6D220BE8C6Ea1667F6Ad93e",
+    ),
+    "COMP": ("eth", "0xc00e94Cb662C3520282E6f5717214004A7f26888"),
+    "SNX": ("eth", "0xC011a73ee8576Fb46F5E1c5751cA3B9Fe0af2a6F"),
+    "MKR": ("eth", "0x9f8F72aA9304c8B593d555F12eF6589cC3A579A2"),
+    "BAL": ("eth", "0xba100000625a3754423978a60c9317c58a424e3D"),
+    "UNI": ("eth", "0x1f9840a85d5aF5bf1D1762F925BDADdC4201F984"),
+    "AAVE": ("eth", "0x7Fc66500c84A76Ad7e9c93437bFc5Ac33E2DDaE9"),
+    "LDO": ("eth", "0x5A98FcBEA516Cf06857215779Fd812CA3beF1B32"),
+    "RPL": ("eth", "0xD33526068D116cE69F19A9ee46F0bd304F21A51f"),
+    "WETH": ("eth", "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"),
+    "MC": ("eth", "0x949d48eca67b17269629c7194f4b727d4ef9e5d6"),
+    "RNDR": ("eth", "0x6de037ef9ad2725eb40118bb1702ebb27e4aeb24"),
+    "FET": ("eth", "0xaea46A60368A7bD060eec7DF8CBa43b7EF41Ad85"),
+    "IMX": ("eth", "0xf57e7e7c23978c3caec3c3548e3d615c346e79ff"),
+    "GALA": ("eth", "0xd1d2Eb1B1e90B638588728b4130137D262C87cae"),
+    "ILV": ("eth", "0x767fe9edc9e0df98e07454847909b5e959d7ca0e"),
+    "SAND": ("eth", "0x3845badAde8e6dFF049820680d1F14bD3903a5d0"),
+    "AXS": ("eth", "0xbb0e17ef65f82ab018d8edd776e8dd940327b28b"),
+    "MANA": ("eth", "0x0f5d2fb29fb7d3cfee444a200298f468908cc942"),
+    "ENS": ("eth", "0xC18360217D8F7Ab5e7c516566761Ea12Ce7F9D72"),
+    "BLUR": ("eth", "0x5283d291dbcf85356a21ba090e6db59121208b44"),
+    "DPI": ("eth", "0x1494ca1f11d487c2bbe4543e90080aeba4ba3c2b"),
+    "MVI": ("eth", "0x72e364f2abdc788b7e918bc238b21f109cd634d7"),
 }
 
 
 class GeckoTerminalFetcher(PublisherInterfaceT):
     BASE_URL: str = (
         "https://api.geckoterminal.com/api/v2/networks/{network}/tokens/{token_address}"
     )
@@ -56,15 +86,14 @@
         if pair[1] != "USD":
             return await self.operate_usd_hop(asset, session)
         pool = ASSET_MAPPING.get(pair[0])
         if pool is None:
             return PublisherFetchError(
                 f"Unknown price pair, do not know how to query GeckoTerminal for {pair[0]}"
             )
-
         url = self.BASE_URL.format(network=pool[0], token_address=pool[1])
         async with session.get(url, headers=self.headers) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from GeckoTerminal"
                 )
             result = await resp.json()
@@ -139,23 +168,23 @@
         price = float(data["price_usd"])
         if hop_result is not None:
             hop_price = float(hop_result["data"]["attributes"]["price_usd"])
             price_int = int(hop_price / price * 10 ** asset["decimals"])
         else:
             price_int = int(price * (10 ** asset["decimals"]))
 
-        volume = float(data["volume_usd"]["h24"] * 10 ** asset["decimals"])
+        volume = float(data["volume_usd"]["h24"]) / 10 ** asset["decimals"]
 
         timestamp = int(time.time())
 
         pair_id = currency_pair_to_pair_id(*pair)
         logger.info("Fetched price %d for %s from GeckoTerminal", price, pair_id)
 
         return SpotEntry(
             pair_id=pair_id,
             price=price_int,
             timestamp=timestamp,
             source=self.SOURCE,
             publisher=self.publisher,
             volume=int(volume),
-            autoscale_volume=False,
+            autoscale_volume=True,
         )
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/gemini.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/gemini.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/huobi.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/huobi.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,55 +3,61 @@
 import time
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
 class HuobiFetcher(PublisherInterfaceT):
     BASE_URL: str = "https://api.huobi.pro/market/detail/merged"
     SOURCE: str = "HUOBI"
-
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher):
+    def __init__(self, assets: List[PragmaAsset], publisher, client=None):
         self.assets = assets
         self.publisher = publisher
+        self.client = client or PragmaClient(network="mainnet")
 
     async def _fetch_pair(
-        self, asset: PragmaSpotAsset, session: ClientSession
+        self, asset: PragmaSpotAsset, session: ClientSession, usdt_price=1
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
-        if pair == ("STRK", "USD"):
-            pair = ("STRK", "USDT")
+        if pair[1] == "USD":
+            pair = (pair[0], "USDT")
+        else:
+            usdt_price = 1
         url = self.format_url(pair[0], pair[1])
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Huobi"
                 )
             result = await resp.json()
             if result["status"] != "ok":
                 return await self.operate_usdt_hop(asset, session)
-            return self._construct(asset, result)
+            return self._construct(asset=asset, result=result, usdt_price=usdt_price)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
+        usdt_price = await self.get_stable_price(self.client, "USDT")
         for asset in self.assets:
             if asset["type"] == "SPOT":
-                entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
+                entries.append(
+                    asyncio.ensure_future(self._fetch_pair(asset, session, usdt_price))
+                )
             else:
                 logger.debug("Skipping Huobi for non-spot asset %s", asset)
                 continue
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
         url = f"{self.BASE_URL}?symbol={quote_asset.lower()}{base_asset.lower()}"
@@ -77,21 +83,21 @@
                     f"No data found for {'/'.join(pair)} from Huobi - hop failed for {pair[1]}"
                 )
             pair2_usdt = await resp.json()
             if pair2_usdt["status"] != "ok":
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Huobi - hop failed for {pair[1]}"
                 )
-        return self._construct(asset, pair2_usdt, pair1_usdt)
+        return self._construct(asset=asset, result=pair2_usdt, hop_result=pair1_usdt)
 
-    def _construct(self, asset, result, hop_result=None) -> SpotEntry:
+    def _construct(self, asset, result, hop_result=None, usdt_price=1) -> SpotEntry:
         pair = asset["pair"]
         bid = float(result["tick"]["bid"][0])
         ask = float(result["tick"]["ask"][0])
-        price = (bid + ask) / 2
+        price = (bid + ask) / (2 * usdt_price)
         if hop_result is not None:
             hop_bid = float(hop_result["tick"]["bid"][0])
             hop_ask = float(hop_result["tick"]["ask"][0])
             hop_price = (hop_bid + hop_ask) / 2
             price = hop_price / price
         timestamp = int(result["ts"] / 1000)
         price_int = int(price * (10 ** asset["decimals"]))
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/kaiko.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/kaiko.py`

 * *Files identical despite different names*

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/kucoin.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/kucoin.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,47 +3,50 @@
 import time
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
 class KucoinFetcher(PublisherInterfaceT):
     BASE_URL: str = "https://api.kucoin.com/api/v1/market/orderbook/level1"
     SOURCE: str = "KUCOIN"
-
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher):
+    def __init__(self, assets: List[PragmaAsset], publisher, client=None):
         self.assets = assets
         self.publisher = publisher
+        self.client = client or PragmaClient(network="mainnet")
 
     async def _fetch_pair(
-        self, asset: PragmaSpotAsset, session: ClientSession
+        self, asset: PragmaSpotAsset, session: ClientSession, usdt_price=1
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
-        if pair == ("STRK", "USD"):
-            pair = ("STRK", "USDT")
+        if pair[1] == "USD":
+            pair = (pair[0], "USDT")
+        else:
+            usdt_price = 1
         url = self.format_url(pair[0], pair[1])
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Kucoin"
                 )
             result = await resp.json()
             if result["data"] == None:
                 return await self.operate_usdt_hop(asset, session)
-            return self._construct(asset, result)
+            return self._construct(asset=asset, result=result, usdt_price=usdt_price)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
         for asset in self.assets:
             if asset["type"] != "SPOT":
@@ -76,19 +79,19 @@
                     f"No data found for {'/'.join(pair)} from Kucoin - hop failed for {pair[1]}"
                 )
             pair2_usdt = await resp.json()
             if pair2_usdt["data"] == None:
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Kucoin - hop failed for {pair[1]}"
                 )
-        return self._construct(asset, pair2_usdt, pair1_usdt)
+        return self._construct(asset=asset, result=pair2_usdt, hop_result=pair1_usdt)
 
-    def _construct(self, asset, result, hop_result=None) -> SpotEntry:
+    def _construct(self, asset, result, hop_result=None, usdt_price=1) -> SpotEntry:
         pair = asset["pair"]
-        price = float(result["data"]["price"])
+        price = float(result["data"]["price"]) / usdt_price
         if hop_result is not None:
             hop_price = float(hop_result["data"]["price"])
             price = hop_price / price
         timestamp = int(result["data"]["time"] / 1000)
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
         logger.info("Fetched price %d for %s from Kucoin", price, "/".join(pair))
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/okx.py` & `pragma_sdk-1.3.0/pragma/publisher/future_fetchers/bybit.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,89 +2,91 @@
 import json
 import logging
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
-from pragma.core.assets import PragmaAsset, PragmaSpotAsset
-from pragma.core.entry import SpotEntry
+from pragma.core.assets import PragmaAsset, PragmaFutureAsset
+from pragma.core.entry import FutureEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
-class OkxFetcher(PublisherInterfaceT):
-    BASE_URL: str = "https://okx.com/api/v5/market/ticker"
-    SOURCE: str = "OKX"
+class ByBitFutureFetcher(PublisherInterfaceT):
+    BASE_URL: str = (
+        "https://api.bybit.com/derivatives/v3/public/tickers?category=linear&symbol="
+    )
+    SOURCE: str = "BYBIT"
 
     publisher: str
 
     def __init__(self, assets: List[PragmaAsset], publisher):
         self.assets = assets
         self.publisher = publisher
 
     async def _fetch_pair(
-        self, asset: PragmaSpotAsset, session: ClientSession
-    ) -> Union[SpotEntry, PublisherFetchError]:
+        self, asset: PragmaFutureAsset, session: ClientSession
+    ) -> Union[FutureEntry, PublisherFetchError]:
         pair = asset["pair"]
-        url = f"{self.BASE_URL}?instId={pair[0]}-{pair[1]}-SWAP"
+        url = self.format_url(pair[0], pair[1])
 
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from OKX"
+                    f"No data found for {'/'.join(pair)} from BYBIT"
                 )
 
             content_type = resp.content_type
             if content_type and "json" in content_type:
                 text = await resp.text()
                 result = json.loads(text)
             else:
-                raise ValueError(f"OKX: Unexpected content type: {content_type}")
+                raise ValueError(f"BYBIT: Unexpected content type: {content_type}")
 
             if (
-                result["code"] == "51001"
-                or result["msg"] == "Instrument ID does not exist"
+                result["retCode"] == "51001"
+                or result["retMsg"] == "Instrument ID does not exist"
             ):
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from OKX"
+                    f"No data found for {'/'.join(pair)} from BYBIT"
                 )
 
             return self._construct(asset, result)
 
     async def fetch(
         self, session: ClientSession
-    ) -> List[Union[SpotEntry, PublisherFetchError]]:
+    ) -> List[Union[FutureEntry, PublisherFetchError]]:
         entries = []
         for asset in self.assets:
-            if asset["type"] != "SPOT":
-                logger.debug("Skipping OKX for non-spot asset %s", asset)
+            if asset["type"] != "FUTURE":
+                logger.debug("Skipping BYBIT for non-spot asset %s", asset)
                 continue
             entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
-        url = f"{self.BASE_URL}?instId={quote_asset}-{base_asset}-SWAP"
+        url = f"{self.BASE_URL}{quote_asset}{base_asset}"
         return url
 
-    def _construct(self, asset, result) -> SpotEntry:
+    def _construct(self, asset, result) -> FutureEntry:
         pair = asset["pair"]
-        data = result["data"][0]
-
-        timestamp = int(int(data["ts"]) / 1000)
-        price = float(data["last"])
+        data = result["result"]["list"][0]
+        timestamp = int(int(result["time"]) / 1000)
+        price = float(data["lastPrice"])
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
-        volume = float(data["volCcy24h"])
-
-        logger.info("Fetched price %d for %s from OKX", price, "/".join(pair))
+        volume = float(data["volume24h"]) / 10 ** asset["decimals"]
+        expiry_timestamp = int(data["deliveryTime"])
+        logger.info("Fetched future for %s from BYBIT", ("/".join(pair)))
 
-        return SpotEntry(
+        return FutureEntry(
             pair_id=pair_id,
             price=price_int,
             volume=volume,
             timestamp=timestamp,
             source=self.SOURCE,
             publisher=self.publisher,
+            expiry_timestamp=expiry_timestamp,
         )
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/propeller.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/propeller.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from typing import Dict, List, Union
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PRAGMA_ALL_ASSETS, PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 SELL_AMOUNTS = [1, 10, 100, 1000]
@@ -21,42 +22,56 @@
     "USDC": "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48",
     "USD": "0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48",  # FIXME: Unsafe
     "USDT": "0xdAC17F958D2ee523a2206206994597C13D831ec7",
     "DAI": "0x6B175474E89094C44Da98b954EedeAC495271d0F",
     "WBTC": "0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599",
     "BTC": "0x2260FAC5E5542a773Aa44fBCfeDf7C193bc2C599",  # FIXME: Unsafe
     "WSTETH": "0x7f39c581f595b53c5cb19bd0b3f8da6c935e2ca0",
+    "ZEND": "0xb2606492712d311be8f41d940afe8ce742a52d442",
+    "DPI": "0x1494CA1F11D487c2bBe4543E90080AeBa4BA3C2b",
+    "WETH": "0xc02aaa39b223fe8d0a0e5c4f27ead9083c756cc2",
+    "MVI": "0x72e364f2abdc788b7e918bc238b21f109cd634d7",
 }
 
+
 DECIMALS_MAPPING: Dict[str, int] = {
     "ETH": 18,
     "USDC": 6,
     "USD": 6,
     "USDT": 6,
     "DAI": 18,
     "WBTC": 8,
     "BTC": 8,
     "WSTETH": 18,
     "STRK": 18,
     "LUSD": 18,
     "UNI": 18,
     "LORDS": 18,
+    "ZEND": 18,
+    "DPI": 8,
+    "MVI": 8,
+    "WETH": 8,
 }
 
 
 class PropellerFetcher(PublisherInterfaceT):
-    BASE_URL: str = "https://api.propellerheads.xyz/v2/solver/quote?blockchain=ethereum"
+    BASE_URL: str = (
+        "https://api.propellerheads.xyz/partner/v2/solver/quote?blockchain=ethereum"
+    )
     SOURCE: str = "PROPELLER"
 
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher, api_key: str = ""):
+    def __init__(
+        self, assets: List[PragmaAsset], publisher, api_key: str = "", client=None
+    ):
         self.assets = assets
         self.publisher = publisher
         self.headers = {"X-Api-Key": api_key}
+        self.client = client or PragmaClient(network="mainnet")
 
     # Propeller requires a payload to be sent with the request
     # The payload is a list of orders, each with a sell_token, buy_token, and sell_amount
     # The sell_amount is the amount of the sell_token to be sold
     # The buy_token is the token to be bought
     # The sell_token is the token to be sold
     def build_payload(self, sell_token, buy_token):
@@ -77,24 +92,31 @@
             ],
         }
 
     async def _fetch_pair(
         self, asset: PragmaSpotAsset, session: ClientSession
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
+        if pair == ("DPI", "USD") or pair == ("MVI", "USD"):
+            substitute_pair = (pair[0], "WETH")
+            eth_price = await self.get_stable_price(self.client, "ETH")
+        else:
+            substitute_pair = pair
+            eth_price = 1
+
         url = f"{self.BASE_URL}"
         try:
-            payload = self.build_payload(pair[0], pair[1])
+            payload = self.build_payload(substitute_pair[0], substitute_pair[1])
         except PublisherFetchError as e:
             return e
 
         async with session.post(url, headers=self.headers, json=payload) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from Propeller"
+                    f"No data found for {'/'.join(substitute_pair)} from Propeller"
                 )
 
             if resp.status == 403:
                 return PublisherFetchError(
                     "Unauthorized: Please provide an API Key to use PropellerFetcher"
                 )
 
@@ -106,15 +128,15 @@
                 raise ValueError(f"PROPELLER: Unexpected content type: {content_type}")
 
             if "error" in result and result["error"] == "Invalid Symbols Pair":
                 return PublisherFetchError(
                     f"No data found for {'/'.join(pair)} from Propeller"
                 )
 
-            return self._construct(asset, result)
+            return self._construct(asset, result, eth_price)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
         for asset in self.assets:
             if asset["type"] != "SPOT":
@@ -123,33 +145,35 @@
             entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
         url = self.BASE_URL
         return url
 
-    def _construct(self, asset, result) -> SpotEntry:
+    def _construct(self, asset, result, eth_price=None) -> SpotEntry:
         pair = asset["pair"]
-
         mid_prices = []
+
+        print(result)
         for quotes, buy_tokens, sell_tokens in zip(
             result["quotes"], result["buy_tokens"], result["sell_tokens"]
         ):
             sell_amount = float(quotes["sell_amount"])
             buy_amount = float(quotes["buy_amount"])
             sell_decimals = int(sell_tokens["decimals"])
             buy_decimals = int(buy_tokens["decimals"])
-
             # Take the mid price
             mid_price = (buy_amount / sell_amount) * 10 ** (
                 sell_decimals - buy_decimals
             )
             mid_prices.append(mid_price)
-
-        price = sum(mid_prices) / len(mid_prices)
+        if pair == ("DPI", "USD") or pair == ("MVI", "USD"):
+            price = sum(mid_prices) * eth_price / len(mid_prices)
+        else:
+            price = sum(mid_prices) / len(mid_prices)
         price_int = int(price * (10 ** asset["decimals"]))
 
         timestamp = int(time.time())
 
         pair_id = currency_pair_to_pair_id(*pair)
 
         logger.info("Fetched price %d for %s from Propeller", price, "/".join(pair))
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/starknetamm.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/starknetamm.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,22 @@
 
 SUPPORTED_ASSETS = [
     ("ETH", "STRK"),
     ("STRK", "USD"),
     ("STRK", "USDT"),
     ("LORDS", "USD"),
     ("ETH", "LORDS"),
+    ("ZEND", "USD"),
+    ("ZEND", "USDC"),
+    ("ZEND", "USDT"),
+    ("ETH", "ZEND"),
 ]
 
 
 class StarknetAMMFetcher(PublisherInterfaceT):
-    client: PragmaClient
     EKUBO_PUBLIC_API: str = "https://mainnet-api.ekubo.org"
     EKUBO_MAINNET_CORE_CONTRACT: str = (
         "0x00000005dd3d2f4429af886cd1a3b08289dbcea99a294197e9eb43b0e0325b4b"
     )
     PRAGMA_ORACLE_CONTRACT: str = (
         "0x2a85bd616f912537c50a49a4076db02c00b29b2cdc8a197ce92ed1837fa875b"
     )
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/thegraph.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/thegraph.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import time
 from typing import Dict, List
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
-from pragma.core.utils import currency_pair_to_pair_id
+from pragma.core.utils import currency_pair_to_pair_id, str_to_felt
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 ASSET_MAPPING: Dict[str, str] = {
     "ETH": "0x88e6a0c2ddd26feeb64f039a2c41296fcb3f5640",  # WETH/USDC 500bps pool
     "BTC": "0x99ac8ca7087fa4a2a1fb6357269965a2014abc35",  # WBTC/USDC 30bps pool
@@ -21,93 +22,108 @@
     "USDC": "0x3416cf6c708da44db2624d63ea0aaef7113527c6",  # USDC/USDT 100bps pool
 }
 
 
 class TheGraphFetcher(PublisherInterfaceT):
     BASE_URL: str = "https://api.thegraph.com/subgraphs/name/"
     SOURCE: str = "THEGRAPH"
-
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher):
+    def __init__(self, assets: List[PragmaAsset], publisher, client=None):
         self.assets = assets
         self.publisher = publisher
+        self.client = client or PragmaClient(network="mainnet")
 
     async def _fetch_pair(
         self, asset: PragmaSpotAsset, session: ClientSession
     ) -> SpotEntry:
         pair = asset["pair"]
-        pool = ASSET_MAPPING.get(pair[0])
-        if pool is None:
+        base_pool = ASSET_MAPPING.get(pair[0])
+        if base_pool is None:
             return PublisherFetchError(
                 f"Unknown price pair, do not know how to query TheGraph for {pair[0]}"
             )
-        if pair[1] != "USD":
-            return PublisherFetchError(f"Base asset not supported : {pair[1]}")
-
-        url_slug = "uniswap/uniswap-v3"
-        query = (
-            f"query "
-            f'{{pool(where: {{id: "{pool}"}}) '
-            f"{{volumeUSD token0Price token1Price liquidity sqrtPrice feeTier tick token0 {{symbol}} token1 {{symbol}}}}}}"
-        )
-
-        async with session.post(
-            self.BASE_URL + url_slug, json={"query": query}
-        ) as resp:
-            if resp.status == 404:
-                return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from TheGraph"
+        quote_result = await self.pool_query(session, self.query_body(pair[0]), pair)
+        if pair[1] != "USDC":
+            if pair[1] == "USD":
+                usdc_str = str_to_felt("USDC/USD")
+                usdc_entry = await self.client.get_spot(usdc_str)
+                usdc_price = int(usdc_entry.price) / (10 ** int(usdc_entry.decimals))
+                print(usdc_price)
+                return self._construct(asset, quote_result, usd_price=usdc_price)
+            elif pair[1] in ASSET_MAPPING.keys():
+                base_result = await self.pool_query(
+                    session, self.query_body(pair[1]), pair
                 )
-            result_json = await resp.json()
-            result = result_json["data"]["pool"]
-
-            return self._construct(asset, result)
+                return self._construct(
+                    asset=asset, quote_result=quote_result, base_result=base_result
+                )
+            else:
+                return PublisherFetchError(f"Base asset not supported : {pair[1]}")
+        return self._construct(asset, quote_result)
 
     async def fetch(self, session: ClientSession) -> List[SpotEntry]:
         entries = []
         for asset in self.assets:
             if asset["type"] != "SPOT":
                 logger.debug("Skipping The Graph for non-spot asset %s", asset)
                 continue
             entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
         return await asyncio.gather(*entries, return_exceptions=True)
 
-    def format_url(self, quote_asset, base_asset):
-        pool = ASSET_MAPPING[quote_asset]
+    def format_url(self, base_asset=None, quote_asset=None):
         url_slug = "uniswap/uniswap-v3"
         url = self.BASE_URL + url_slug
         return url
 
     def query_body(self, quote_asset):
         pool = ASSET_MAPPING[quote_asset]
         query = (
-            f"query "
-            f'{{pool(where: {{id: "{pool}"}}) '
-            f"{{volumeUSD token0Price token1Price liquidity sqrtPrice feeTier tick token0 {{symbol}} token1 {{symbol}}}}}}"
+            f'{{pool(id: "{pool}")'
+            f"{{ tick token0 {{ symbol }} token1 {{ symbol }} "
+            f"feeTier sqrtPrice liquidity token0Price token1Price volumeUSD}}}}"
         )
         return query
 
-    def _construct(self, asset, result) -> SpotEntry:
+    async def pool_query(self, session: ClientSession, query: str, pair: List[str]):
+        async with session.post(self.format_url(), json={"query": query}) as resp:
+            if resp.status == 404:
+                return PublisherFetchError(
+                    f"No data found for {'/'.join(pair)} from TheGraph"
+                )
+            result_json = await resp.json()
+            result = result_json["data"]["pool"]
+            return result
+
+    def _construct(
+        self, asset, quote_result, base_result=None, usd_price=1
+    ) -> SpotEntry:
         pair = asset["pair"]
 
-        if pair[0] in result["token0"]["symbol"]:
-            price = float(result["token1Price"])
+        if pair[0] in quote_result["token0"]["symbol"]:
+            price = float(quote_result["token1Price"]) / usd_price
         else:
-            price = float(result["token0Price"])
+            price = float(quote_result["token0Price"]) / usd_price
 
+        if base_result is not None:
+            if pair[1] in base_result["token0"]["symbol"]:
+                base_price = float(base_result["token1Price"])
+            else:
+                base_price = float(base_result["token0Price"])
+            price = price / base_price
         price_int = int(price * (10 ** asset["decimals"]))
-        volume = float(result["volumeUSD"])
+        volume = float(quote_result["volumeUSD"]) * (10 ** asset["decimals"])
 
         timestamp = int(time.time())
 
         pair_id = currency_pair_to_pair_id(*pair)
         logger.info("Fetched data %s for %s from The Graph", price, pair_id)
 
         return SpotEntry(
             pair_id=pair_id,
             price=price_int,
             timestamp=timestamp,
             source=self.SOURCE,
             publisher=self.publisher,
-            volume=volume,
+            volume=int(volume),
+            autoscale_volume=False,
         )
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/fetchers/upbit.py` & `pragma_sdk-1.3.0/pragma/publisher/fetchers/okx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,74 +1,95 @@
 import asyncio
+import json
 import logging
-import time
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
 from pragma.core.assets import PragmaAsset, PragmaSpotAsset
+from pragma.core.client import PragmaClient
 from pragma.core.entry import SpotEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
-SUPPORTED_ASSETS = [("BTC", "ETH")]
-
-
-class UpbitFetcher(PublisherInterfaceT):
-    BASE_URL: str = "https://sg-api.upbit.com/v1/ticker"
-    SOURCE: str = "UPBIT"
 
+class OkxFetcher(PublisherInterfaceT):
+    BASE_URL: str = "https://okx.com/api/v5/market/ticker"
+    SOURCE: str = "OKX"
     publisher: str
 
-    def __init__(self, assets: List[PragmaAsset], publisher):
+    def __init__(self, assets: List[PragmaAsset], publisher, client=None):
         self.assets = assets
         self.publisher = publisher
+        self.client = client or PragmaClient(network="mainnet")
 
     async def _fetch_pair(
-        self, asset: PragmaSpotAsset, session: ClientSession
+        self, asset: PragmaSpotAsset, session: ClientSession, usdt_price=1
     ) -> Union[SpotEntry, PublisherFetchError]:
         pair = asset["pair"]
-        url = self.format_url(pair[0], pair[1])
+        if pair[1] == "USD":
+            pair = (pair[0], "USDT")
+        else:
+            usdt_price = 1
+        url = f"{self.BASE_URL}?instId={pair[0]}-{pair[1]}-SWAP"
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from Upbit"
+                    f"No data found for {'/'.join(pair)} from OKX"
+                )
+
+            content_type = resp.content_type
+            if content_type and "json" in content_type:
+                text = await resp.text()
+                result = json.loads(text)
+            else:
+                raise ValueError(f"OKX: Unexpected content type: {content_type}")
+
+            if (
+                result["code"] == "51001"
+                or result["msg"] == "Instrument ID does not exist"
+            ):
+                return PublisherFetchError(
+                    f"No data found for {'/'.join(pair)} from OKX"
                 )
-            result = await resp.json()
-            return self._construct(asset, result)
+
+            return self._construct(asset, result, usdt_price)
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[SpotEntry, PublisherFetchError]]:
         entries = []
+        usdt_price = await self.get_stable_price(self.client, "USDT")
         for asset in self.assets:
-            if asset["type"] == "SPOT" and asset["pair"] in SUPPORTED_ASSETS:
-                entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
-            else:
-                logger.debug("Skipping Upbit for non-spot asset %s", asset)
+            if asset["type"] != "SPOT":
+                logger.debug("Skipping OKX for non-spot asset %s", asset)
                 continue
+            entries.append(
+                asyncio.ensure_future(self._fetch_pair(asset, session, usdt_price))
+            )
         return await asyncio.gather(*entries, return_exceptions=True)
 
     def format_url(self, quote_asset, base_asset):
-        url = f"{self.BASE_URL}?markets={quote_asset}-{base_asset}"
+        url = f"{self.BASE_URL}?instId={quote_asset}-{base_asset}-SWAP"
         return url
 
-    def _construct(self, asset, result) -> SpotEntry:
+    def _construct(self, asset, result, usdt_price=1) -> SpotEntry:
         pair = asset["pair"]
-        data = result[0]
-        timestamp = int(time.time())
-        price = float(data["trade_price"])
+        data = result["data"][0]
+
+        timestamp = int(int(data["ts"]) / 1000)
+        price = float(data["last"]) / usdt_price
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
-        volume = float(data["trade_volume"])
+        volume = float(data["volCcy24h"])
 
-        logger.info("Fetched price %d for %s from Upbit", price, "/".join(pair))
+        logger.info("Fetched price %d for %s from OKX", price, "/".join(pair))
 
         return SpotEntry(
             pair_id=pair_id,
             price=price_int,
             volume=volume,
             timestamp=timestamp,
             source=self.SOURCE,
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/future_fetchers/binance.py` & `pragma_sdk-1.3.0/pragma/publisher/future_fetchers/binance.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         pair = asset["pair"]
         result_arr = []
         for data in result:
             timestamp = int(data["time"])
             price = float(data["markPrice"])
             price_int = int(price * (10 ** asset["decimals"]))
             pair_id = currency_pair_to_pair_id(*pair)
-            volume = float(self.retrieve_volume(data["symbol"], volume_arr)) * (
+            volume = float(self.retrieve_volume(data["symbol"], volume_arr)) / (
                 10 ** asset["decimals"]
             )
             if data["symbol"] == f"{pair[0]}{pair[1]}":
                 expiry_timestamp = 0
             else:
                 date_arr = data["symbol"].split("_")
                 if len(date_arr) > 1:
@@ -118,11 +118,11 @@
                     pair_id=pair_id,
                     price=price_int,
                     volume=int(volume),
                     timestamp=int(timestamp / 1000),
                     source=self.SOURCE,
                     publisher=self.publisher,
                     expiry_timestamp=expiry_timestamp * 1000,
-                    autoscale_volume=False,
+                    autoscale_volume=True,
                 )
             )
         return result_arr
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/future_fetchers/bybit.py` & `pragma_sdk-1.3.0/pragma/publisher/future_fetchers/okx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import json
 import logging
 from typing import List, Union
 
 import requests
 from aiohttp import ClientSession
 
@@ -10,83 +9,110 @@
 from pragma.core.entry import FutureEntry
 from pragma.core.utils import currency_pair_to_pair_id
 from pragma.publisher.types import PublisherFetchError, PublisherInterfaceT
 
 logger = logging.getLogger(__name__)
 
 
-class ByBitFutureFetcher(PublisherInterfaceT):
-    BASE_URL: str = (
-        "https://api.bybit.com/derivatives/v3/public/tickers?category=linear&symbol="
-    )
-    SOURCE: str = "BYBIT"
-
+class OkxFutureFetcher(PublisherInterfaceT):
+    BASE_URL: str = "https://okx.com/api/v5/market/tickers"
+    SOURCE: str = "OKX"
+    TIMESTAMP_URL: str = "https://www.okx.com/api/v5/public/instruments"
     publisher: str
 
     def __init__(self, assets: List[PragmaAsset], publisher):
         self.assets = assets
         self.publisher = publisher
 
-    async def _fetch_pair(
-        self, asset: PragmaFutureAsset, session: ClientSession
-    ) -> Union[FutureEntry, PublisherFetchError]:
+    async def fetch_expiry_timestamp(self, asset, instrument_id, session):
         pair = asset["pair"]
-        url = self.format_url(pair[0], pair[1])
+        url = self.format_expiry_timestamp_url(instrument_id)
+        async with session.get(url) as resp:
+            if resp.status == 404:
+                return PublisherFetchError(
+                    f"No data found for {'/'.join(pair)} from OKX"
+                )
+            result = await resp.json(content_type="application/json")
+            if (
+                result["code"] == "51001"
+                or result["msg"] == "Instrument ID does not exist"
+            ):
+                return PublisherFetchError(
+                    f"No data found for {'/'.join(pair)} from OKX"
+                )
+            return result["data"][0]["expTime"]
+
+    def format_expiry_timestamp_url(self, instrument_id):
+        return f"{self.TIMESTAMP_URL}?instType=FUTURES&instId={instrument_id}"
 
+    async def _fetch_pair(self, asset: PragmaFutureAsset, session: ClientSession):
+        pair = asset["pair"]
+        url = f"{self.BASE_URL}?instType=FUTURES&uly={pair[0]}-{pair[1]}"
+        future_entries = []
         async with session.get(url) as resp:
             if resp.status == 404:
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from BYBIT"
+                    f"No data found for {'/'.join(pair)} from OKX"
                 )
 
             content_type = resp.content_type
             if content_type and "json" in content_type:
                 text = await resp.text()
                 result = json.loads(text)
             else:
-                raise ValueError(f"BYBIT: Unexpected content type: {content_type}")
+                raise ValueError(f"OKX: Unexpected content type: {content_type}")
 
             if (
-                result["retCode"] == "51001"
-                or result["retMsg"] == "Instrument ID does not exist"
+                result["code"] == "51001"
+                or result["msg"] == "Instrument ID does not exist"
             ):
                 return PublisherFetchError(
-                    f"No data found for {'/'.join(pair)} from BYBIT"
+                    f"No data found for {'/'.join(pair)} from OKX"
                 )
-
-            return self._construct(asset, result)
+            result_len = len(result["data"])
+            if result_len > 1:
+                for i in range(0, result_len):
+                    expiry_timestamp = await self.fetch_expiry_timestamp(
+                        asset, result["data"][i]["instId"], session
+                    )
+                    future_entries.append(
+                        self._construct(asset, result["data"][i], expiry_timestamp)
+                    )
+            return future_entries
 
     async def fetch(
         self, session: ClientSession
     ) -> List[Union[FutureEntry, PublisherFetchError]]:
         entries = []
         for asset in self.assets:
             if asset["type"] != "FUTURE":
-                logger.debug("Skipping BYBIT for non-spot asset %s", asset)
+                logger.debug("Skipping OKX for non-future asset %s", asset)
                 continue
-            entries.append(asyncio.ensure_future(self._fetch_pair(asset, session)))
-        return await asyncio.gather(*entries, return_exceptions=True)
+            future_entries = await self._fetch_pair(asset, session)
+            if isinstance(future_entries, list):
+                entries.extend(future_entries)
+            else:
+                entries.append(future_entries)
+        return entries
 
-    def format_url(self, quote_asset, base_asset):
-        url = f"{self.BASE_URL}{quote_asset}{base_asset}"
+    def format_url(self, quote_asset, base_asset) -> str:
+        url = f"{self.BASE_URL}?instType=FUTURES&uly={quote_asset}-{base_asset}"
         return url
 
-    def _construct(self, asset, result) -> FutureEntry:
+    def _construct(self, asset, data, expiry_timestamp) -> List[FutureEntry]:
         pair = asset["pair"]
-        data = result["result"]["list"][0]
-        timestamp = int(int(result["time"]) / 1000)
-        price = float(data["lastPrice"])
+        timestamp = int(int(data["ts"]) / 1000)
+        price = float(data["last"])
         price_int = int(price * (10 ** asset["decimals"]))
         pair_id = currency_pair_to_pair_id(*pair)
-        volume = float(data["volume24h"]) / 10 ** asset["decimals"]
-        expiry_timestamp = int(data["deliveryTime"])
-        logger.info("Fetched future for %s from BYBIT", ("/".join(pair)))
+        volume = float(data["volCcy24h"]) / 10 ** asset["decimals"]
+        logger.info("Fetched future for %s from OKX", "/".join(pair))
 
         return FutureEntry(
             pair_id=pair_id,
             price=price_int,
             volume=volume,
             timestamp=timestamp,
             source=self.SOURCE,
             publisher=self.publisher,
-            expiry_timestamp=expiry_timestamp,
+            expiry_timestamp=int(expiry_timestamp),
         )
```

### Comparing `pragma_sdk-1.2.9/pragma/publisher/types.py` & `pragma_sdk-1.3.0/pragma/publisher/types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import abc
 from typing import Any, List
 
 import aiohttp
 from aiohttp import ClientSession
 
-from pragma.core.utils import add_sync_methods
+from pragma.core.client import PragmaClient
+from pragma.core.utils import add_sync_methods, str_to_felt
 
 
 # Abstract base class for all publishers
 @add_sync_methods
 class PublisherInterfaceT(abc.ABC):
+    client: PragmaClient
+
     @abc.abstractmethod
-    async def fetch(self, session: ClientSession) -> List[Any]:
-        ...
+    async def fetch(self, session: ClientSession) -> List[Any]: ...
 
     @abc.abstractmethod
-    def format_url(self, quote_asset, base_asset) -> str:
-        ...
+    def format_url(self, quote_asset, base_asset) -> str: ...
 
     async def _fetch(self):
         async with aiohttp.ClientSession() as session:
             data = await self.fetch(session)
             return data
 
+    async def get_stable_price(self, client, stable_asset):
+        usdt_str = str_to_felt(stable_asset + "/USD")
+        usdt_entry = await client.get_spot(usdt_str)
+        return int(usdt_entry.price) / (10 ** int(usdt_entry.decimals))
+
 
 class PublisherFetchError(Exception):
     message: str
 
     def __init__(self, message: str):
         self.message = message
```

### Comparing `pragma_sdk-1.2.9/pyproject.toml` & `pragma_sdk-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pragma-sdk"
-version = "1.2.9"
+version = "1.3.0"
 authors = ["0xevolve <matthias@pragma.build>"]
 description = "Core package for rollup-native Pragma Oracle"
 readme = "README.md"
 homepage = "https://pragma.build"
 repository = "https://github.com/Astraly-Labs/pragma-sdk"
 documentation = "https://docs.pragma.build"
 classifiers = [
@@ -56,15 +56,15 @@
 test_ci_client = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/client_test.py -s"
 test_ci_update_client = "coverage run -m pytest --net=fork_devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/update_client_test.py -s"
 test_ci_publisher = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/publisher_test.py -s"
 test_ci_fetchers = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/fetchers_test.py -s"
 test_ci_vrf = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 1 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/vrf_test.py -s"
 test_stagecoach = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError stagecoach/ -s"
 test_ci_api_client = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/api_client_test.py -s"
-
+test_ci_utils = "coverage run -m pytest --net=devnet --client=full_node -v --reruns 5 --only-rerun aiohttp.client_exceptions.ClientConnectorError pragma/tests/utils_test.py -s"
 
 circular_imports_check.shell = "poetry run pytest circular.py"
 update_abis = "find ./pragma-oracle -name '*.sierra.json' -exec cp -prv '{}' './pragma/core/abis' ';'"
 
 [tool.poetry.build]
 generate-setup-file = true
```

### Comparing `pragma_sdk-1.2.9/setup.py` & `pragma_sdk-1.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'python-dotenv>=1.0.0,<2.0.0',
  'requests-mock>=1.11.0,<2.0.0',
  'starknet.py==0.20.0',
  'typer==0.6.1']
 
 setup_kwargs = {
     'name': 'pragma-sdk',
-    'version': '1.2.9',
+    'version': '1.3.0',
     'description': 'Core package for rollup-native Pragma Oracle',
     'long_description': "# Pragma SDK\n\n[![codecov](https://codecov.io/gh/Astraly-Labs/pragma-sdk/graph/badge.svg?token=98pUFYGHIK)](https://codecov.io/gh/Astraly-Labs/pragma-sdk)\n\n[![Checks](https://github.com/Astraly-Labs/pragma-sdk/actions/workflows/checks.yml/badge.svg)](https://github.com/Astraly-Labs/pragma-sdk/actions/workflows/checks.yml)\n\n[![Package](https://img.shields.io/pypi/v/pragma-sdk)](https://pypi.org/project/pragma-sdk/)\n\n---\n\n**Pragma SDK, written in Python.**\n\nOne can leverage this SDK to interact with Pragma on Starknet.\nThis SDK should also be used by Data Providers willing to push data on Pragma contracts.\n\n## About\n\nFor more information, see the [project's repository](https://github.com/Astraly-Labs/Pragma), [documentation overview](https://docs.pragmaoracle.com/) and [documentation on how to publish data](https://docs.pragmaoracle.com/using-pragma/publishing-data).\n\n## Contributing\n\nSee the [CONTRIBUTING](./CONTRIBUTING.md) guide.",
     'author': '0xevolve',
     'author_email': 'matthias@pragma.build',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pragma.build',
```

### Comparing `pragma_sdk-1.2.9/PKG-INFO` & `pragma_sdk-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pragma-sdk
-Version: 1.2.9
+Version: 1.3.0
 Summary: Core package for rollup-native Pragma Oracle
 Home-page: https://pragma.build
 Author: 0xevolve
 Author-email: matthias@pragma.build
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

