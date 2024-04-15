# Comparing `tmp/telegram_wallet_pay-0.3.0.tar.gz` & `tmp/telegram_wallet_pay-0.3.1.tar.gz`

## Comparing `telegram_wallet_pay-0.3.0.tar` & `telegram_wallet_pay-0.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/.editorconfig
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/Makefile
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/codecov.yaml
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/examples/00_create_order.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/examples/01_get_order_preview.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/__init__.py
--rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/client.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/errors.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/tools.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/_default.py
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/create_order_request.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/create_order_response.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/get_order_preview_response.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/money_amount.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_amount.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_amount_response.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_preview.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_reconciliation_item.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_reconciliation_list.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/payment_option.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/webhook_message.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/webhook_payload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/tests/test_client.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/tests/test_schemas.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/tests/test_signature.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/.gitignore
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/README.md
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/.editorconfig
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/Makefile
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/codecov.yaml
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/examples/00_create_order.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/examples/01_get_order_preview.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/__init__.py
+-rw-r--r--   0        0        0     7062 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/client.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/errors.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/tools.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/__init__.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/_default.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/create_order_request.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/create_order_response.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/get_order_preview_response.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/get_order_reconciliation_list_response.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/money_amount.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_amount.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_amount_response.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_preview.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_reconciliation_item.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_reconciliation_list.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/payment_option.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_message.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_payload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     6608 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/test_client.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/test_schemas.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/tests/test_signature.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/.gitignore
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/README.md
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4139 2020-02-02 00:00:00.000000 telegram_wallet_pay-0.3.1/PKG-INFO
```

### Comparing `telegram_wallet_pay-0.3.0/examples/00_create_order.py` & `telegram_wallet_pay-0.3.1/examples/00_create_order.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/client.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/tools.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/tools.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/__init__.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/create_order_request.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/create_order_request.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_preview.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_preview.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/order_reconciliation_item.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/order_reconciliation_item.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/webhook_message.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_message.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/telegram_wallet_pay/schemas/webhook_payload.py` & `telegram_wallet_pay-0.3.1/telegram_wallet_pay/schemas/webhook_payload.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/tests/test_client.py` & `telegram_wallet_pay-0.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/tests/test_schemas.py` & `telegram_wallet_pay-0.3.1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/tests/test_signature.py` & `telegram_wallet_pay-0.3.1/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/.gitignore` & `telegram_wallet_pay-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `telegram_wallet_pay-0.3.0/README.md` & `telegram_wallet_pay-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -58,54 +58,14 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 
-### Create order
-
-```python
-import asyncio
-import os
-from uuid import uuid4
-
-from telegram_wallet_pay import TelegramWalletPay
-
-# use your token from https://pay.wallet.tg/
-TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
-
-
-async def main():
-    # create API-client instance
-    wallet = TelegramWalletPay(TOKEN)
-
-    # create your first order
-    response = await wallet.create_order(
-        amount=40,
-        currency_code="RUB",
-        description="Test Payment",
-        external_id=str(uuid4()),
-        timeout_seconds=5 * 60,
-        customer_telegram_user_id=66812456,
-    )
-
-    # let's print creation response
-    print("Response:", response)
-    print("Order:", response.data)
-
-    # don't forget close API-client instance on your app shutdown
-    await wallet.close()
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
-
-```
-
 ### Get order preview
 
 ```python
 import asyncio
 import os
 
 from telegram_wallet_pay import TelegramWalletPay
```

### Comparing `telegram_wallet_pay-0.3.0/pyproject.toml` & `telegram_wallet_pay-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Typing :: Typed",
 ]
 
 dependencies = [
-    "aiohttp>=3.8.5,<3.10",
+    "aiohttp>=3.8,<4",
     "pydantic>=2.4,<3",
     "certifi>=2023",
 ]
 
 [project.optional-dependencies]
 dev = [
     "ruff>=0",
@@ -57,15 +57,15 @@
     "pre-commit>=3",
 ]
 test = [
     "coverage>=7",
     "pytest>=8",
     "pytest-asyncio>=0",
     "pytest-cov>=5",
-    "aresponses==3.0.0",
+    "aresponses>=3",
 ]
 
 
 [project.urls]
 Repository = "https://github.com/Olegt0rr/TelegramWalletPay"
 
 [tool.hatch.version]
```

### Comparing `telegram_wallet_pay-0.3.0/PKG-INFO` & `telegram_wallet_pay-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: telegram-wallet-pay
-Version: 0.3.0
+Version: 0.3.1
 Summary: Async client for Telegram Wallet Pay API
 Project-URL: Repository, https://github.com/Olegt0rr/TelegramWalletPay
 Author-email: Oleg Abramov <oleg@trueweb.app>
 Maintainer-email: Oleg Abramov <oleg@trueweb.app>
 License-Expression: MIT
 Keywords: API,Pay,Telegram,Wallet,async
 Classifier: Development Status :: 4 - Beta
@@ -23,23 +23,23 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: aiohttp<3.10,>=3.8.5
+Requires-Dist: aiohttp<4,>=3.8
 Requires-Dist: certifi>=2023
 Requires-Dist: pydantic<3,>=2.4
 Provides-Extra: dev
 Requires-Dist: mypy>=1; extra == 'dev'
 Requires-Dist: pre-commit>=3; extra == 'dev'
 Requires-Dist: ruff>=0; extra == 'dev'
 Provides-Extra: test
-Requires-Dist: aresponses==3.0.0; extra == 'test'
+Requires-Dist: aresponses>=3; extra == 'test'
 Requires-Dist: coverage>=7; extra == 'test'
 Requires-Dist: pytest-asyncio>=0; extra == 'test'
 Requires-Dist: pytest-cov>=5; extra == 'test'
 Requires-Dist: pytest>=8; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Telegram Wallet Pay
@@ -102,54 +102,14 @@
 
 if __name__ == "__main__":
     asyncio.run(main())
 
 ```
 
 
-### Create order
-
-```python
-import asyncio
-import os
-from uuid import uuid4
-
-from telegram_wallet_pay import TelegramWalletPay
-
-# use your token from https://pay.wallet.tg/
-TOKEN = os.getenv("TELEGRAM_WALLET_PAY_TOKEN")
-
-
-async def main():
-    # create API-client instance
-    wallet = TelegramWalletPay(TOKEN)
-
-    # create your first order
-    response = await wallet.create_order(
-        amount=40,
-        currency_code="RUB",
-        description="Test Payment",
-        external_id=str(uuid4()),
-        timeout_seconds=5 * 60,
-        customer_telegram_user_id=66812456,
-    )
-
-    # let's print creation response
-    print("Response:", response)
-    print("Order:", response.data)
-
-    # don't forget close API-client instance on your app shutdown
-    await wallet.close()
-
-
-if __name__ == "__main__":
-    asyncio.run(main())
-
-```
-
 ### Get order preview
 
 ```python
 import asyncio
 import os
 
 from telegram_wallet_pay import TelegramWalletPay
```

