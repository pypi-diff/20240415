# Comparing `tmp/kitetrader-2.0.0.tar.gz` & `tmp/kitetrader-2.1.0.tar.gz`

## Comparing `kitetrader-2.0.0.tar` & `kitetrader-2.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 kitetrader-2.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kitetrader-2.0.0/src/__init__.py
--rw-r--r--   0        0        0    13574 2020-02-02 00:00:00.000000 kitetrader-2.0.0/src/kitetrader/Kite.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kitetrader-2.0.0/src/kitetrader/__init__.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kitetrader-2.0.0/tests/Dockerfile
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 kitetrader-2.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kitetrader-2.0.0/LICENSE
--rw-r--r--   0        0        0    10816 2020-02-02 00:00:00.000000 kitetrader-2.0.0/README.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 kitetrader-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    11528 2020-02-02 00:00:00.000000 kitetrader-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 kitetrader-2.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 kitetrader-2.1.0/src/__init__.py
+-rw-r--r--   0        0        0    12615 2020-02-02 00:00:00.000000 kitetrader-2.1.0/src/kitetrader/Kite.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 kitetrader-2.1.0/src/kitetrader/__init__.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 kitetrader-2.1.0/tests/Dockerfile
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 kitetrader-2.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 kitetrader-2.1.0/LICENSE
+-rw-r--r--   0        0        0    11172 2020-02-02 00:00:00.000000 kitetrader-2.1.0/README.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 kitetrader-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11884 2020-02-02 00:00:00.000000 kitetrader-2.1.0/PKG-INFO
```

### Comparing `kitetrader-2.0.0/.github/workflows/python-publish.yml` & `kitetrader-2.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `kitetrader-2.0.0/src/kitetrader/Kite.py` & `kitetrader-2.1.0/src/kitetrader/Kite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Collection
-from typing import Union
+from typing import Optional, Union, Any
 from requests import Session
 from requests.exceptions import ReadTimeout
 from urllib3.util import Retry
 from requests.adapters import HTTPAdapter
 from pathlib import Path
-from pickle import loads as pickle_loads, dumps as pickle_dumps
+import pickle
 from mthrottle import Throttle
 from datetime import datetime
 
 throttle_config = {
     "quote": {
         "rps": 1,
     },
@@ -81,90 +81,80 @@
     GTT_TYPE_SINGLE = "single"
 
     base_dir = Path(__file__).parent
     base_url = "https://api.kite.trade"
     cookies = None
     config = None
 
-    def __init__(self, enctoken: Union[str, None] = None):
+    def __init__(
+        self,
+        user_id: Optional[str] = None,
+        password: Optional[str] = None,
+        twofa: Optional[str] = None,
+        enctoken: Optional[str] = None,
+    ):
 
         self.cookie_path = self.base_dir / "kite_cookies"
-        self.enctoken = enctoken
+
         self.session = Session()
+        self.session.headers.update({"X-Kite-version": "3"})
+
+        self.enctoken = enctoken
 
         retries = Retry(
             total=None,
             connect=3,
             read=3,
             redirect=0,
             status=3,
             other=0,
             backoff_factor=0.1,
-            status_forcelist=["502", "503", "504"],
+            status_forcelist=[502, 503, 504],
             raise_on_status=False,
         )
 
         self.session.mount("https://", HTTPAdapter(max_retries=retries))
 
-        ua = (
-            "Mozilla/5.0 (Windows NT 10.0; rv:91.0) Gecko/20100101 Firefox/91.0"
-        )
-
-        self.session.headers.update(
-            {
-                "User-Agent": ua,
-            }
-        )
-
         if self.cookie_path.exists():
             self.cookies = self._get_cookie()
 
             # get enctoken from cookies
-            cookie_token = self.cookies.get("enctoken")
-
-            # only save cookies to file if enctoken has changed
-            if enctoken and cookie_token != enctoken:
-                self._set_cookie(self.session.cookies)
-            else:
-                # else set cookie enctoken
-                self.enctoken = cookie_token
+            self.enctoken = self.cookies.get("enctoken")
 
         if self.enctoken:
-            # Finally set Authorization headers and cookies on session
             self.session.headers.update(
                 {"Authorization": f"enctoken {self.enctoken}"}
             )
         else:
             # initiate login
-            self._check_auth()
+            self._authorize(user_id, password, twofa)
 
     def __enter__(self):
         return self
 
     def __exit__(self, *_):
         self.session.close()
-
         return False
 
     def close(self):
         """Close the Requests session"""
 
         self.session.close()
 
     def _get_cookie(self):
         """Load the pickle format cookie file"""
 
-        return pickle_loads(self.cookie_path.read_bytes())
+        return pickle.loads(self.cookie_path.read_bytes())
 
     def _set_cookie(self, cookies):
         """Save the cookies to pickle formatted file"""
 
-        self.cookie_path.write_bytes(pickle_dumps(cookies))
+        self.cookie_path.write_bytes(pickle.dumps(cookies))
 
-    def _req(self, url, method, payload=None, timeout=15, hint=None):
+    def _req(self, url, method, payload=None, timeout=15, hint=None) -> Any:
         """Make an HTTP request"""
 
         try:
             if method == "PUT":
                 r = self.session.put(url, data=payload, timeout=timeout)
             elif method == "DELETE":
                 r = self.session.delete(url)
@@ -194,79 +184,73 @@
 
         if code == 400:
             reason = "Missing or bad request parameters or values"
             raise ConnectionError(f"{hint} | {code}: {reason}")
 
         raise ConnectionError(f"{hint} | {code}: {r.reason}")
 
-    def _authorize(self, user_id: str, pwd: str):
+    def _authorize(
+        self,
+        user_id: Optional[str] = None,
+        password: Optional[str] = None,
+        twofa: Optional[str] = None,
+    ):
         """Authenthicate the user"""
 
-        base_url = "https://kite.zerodha.com"
+        if not user_id:
+            user_id = input("Enter User id\n> ")
 
-        payload = {"user_id": user_id, "password": pwd}
+        if not password:
+            password = input("Enter Password\n> ")
 
-        r = self._req(
-            f"{base_url}/api/login", "POST", payload=payload, hint="Login"
-        )
+        base_url = "https://kite.zerodha.com"
 
-        if r is None:
-            return
+        response = self._req(
+            f"{base_url}/api/login",
+            "POST",
+            payload=dict(user_id=user_id, password=password),
+            hint="Login",
+        ).json()
 
-        res = r.json()
+        request_id = response["data"]["request_id"]
+        twofa_type = response["data"]["twofa_type"]
 
-        request_id = res["data"]["request_id"]
-        twofa_type = res["data"]["twofa_type"]
-        twofa_value = input(f"Please enter {twofa_type} code\n> ")
+        if not twofa:
+            twofa = input(f"Please enter {twofa_type} code\n> ")
 
-        res = self._req(
+        response = self._req(
             f"{base_url}/api/twofa",
             "POST",
-            payload={
-                "user_id": user_id,
-                "request_id": request_id,
-                "twofa_value": twofa_value,
-                "twofa_type": twofa_type,
-                "skip_session": "",
-            },
+            payload=dict(
+                user_id=user_id,
+                request_id=request_id,
+                twofa_value=twofa,
+                twofa_type=twofa_type,
+                skip_session="",
+            ),
             hint="TwoFA",
         )
 
-        if res:
-            enctoken = res.cookies["enctoken"]
-
-            self._set_cookie(res.cookies)
+        enctoken = response.cookies["enctoken"]
+        self._set_cookie(response.cookies)
 
-            self.session.headers.update(
-                {"authorization": f"enctoken {enctoken}"}
-            )
-
-            print("Authorization Succces")
-
-    def _check_auth(self):
-        print("Authorization required")
+        self.session.headers.update({"Authorization": f"enctoken {enctoken}"})
 
-        user_id = input("Enter User id\n> ")
-        pwd = input("Enter Password\n> ")
+        print("Authorization Succces")
 
-        self._authorize(user_id, pwd)
-
-    def instruments(self, exchange: Union[str, None] = None):
+    def instruments(self, exchange: Optional[str] = None):
         """return a CSV dump of all tradable instruments"""
 
         th.check()
         url = f"{self.base_url}/instruments"
 
         if exchange:
             url += f"/{exchange}"
 
-        res = self._req(url, "GET", hint="Instruments")
-
-        if res:
-            return res.content
+        return self._req(url, "GET", hint="Instruments")
 
     def quote(self, instruments: Union[str, Collection]):
         """Return the full market quotes - ohlc, OI, bid/ask etc"""
 
         if not isinstance(instruments, str) and len(instruments) > 500:
             raise ValueError("Instruments length cannot exceed 500")
 
@@ -275,15 +259,15 @@
         res = self._req(
             f"{self.base_url}/quote",
             "GET",
             payload={"i": instruments},
             hint="Quote",
         )
 
-        return res.json()["data"] if res else None
+        return res.json()["data"]
 
     def ohlc(self, instruments: Union[str, Collection]):
         """Returns ohlc and last traded price"""
 
         if not isinstance(instruments, str) and len(instruments) > 1000:
             raise ValueError("Instruments length cannot exceed 1000")
 
@@ -292,95 +276,85 @@
         res = self._req(
             f"{self.base_url}/quote/ohlc",
             method="GET",
             payload={"i": instruments},
             hint="Quote/OHLC",
         )
 
-        return res.json()["data"] if res else None
+        return res.json()["data"]
 
     def ltp(self, instruments: Union[str, Collection]):
         """Returns the last traded price"""
 
         if not isinstance(instruments, str) and len(instruments) > 1000:
             raise ValueError("Instruments length cannot exceed 1000")
 
         th.check("quote")
 
-        res = self._req(
+        return self._req(
             f"{self.base_url}/quote/ltp",
             method="GET",
             payload={"i": instruments},
             hint="LTP",
-        )
-
-        return res.json()["data"] if res else None
+        ).json()["data"]
 
     def holdings(self):
         """Return the list of long term equity holdings"""
 
         th.check()
 
-        res = self._req(
+        return self._req(
             f"{self.base_url}/portfolio/holdings",
             method="GET",
             hint="Portfolio/holdings",
-        )
-
-        return res.json()["data"] if res else None
+        ).json()["data"]
 
     def positions(self):
         """Retrieve the list of short term positions"""
 
         th.check()
 
-        res = self._req(
+        return self._req(
             f"{self.base_url}/portfolio/positions",
             method="GET",
             hint="Portfolio/positions",
-        )
-
-        return res.json()["data"] if res else None
+        ).json()["data"]
 
     def auctions(self):
         """Retrieve the list of auctions that are currently being held"""
 
         th.check()
 
-        res = self._req(
+        return self._req(
             f"{self.base_url}/portfolio/auctions",
             method="GET",
             hint="Portfolio/auctions",
-        )
-
-        return res.json()["data"] if res else None
+        ).json()["data"]
 
-    def margins(self, segment: Union[str, None] = None):
+    def margins(self, segment: Optional[str] = None):
         """Returns funds, cash, and margin information for the user
         for equity and commodity segments"""
 
         url = f"{self.base_url}/user/margins"
 
         if segment:
             url += f"/{segment}"
 
         th.check()
 
-        res = self._req(url, method="GET", hint="Margins")
-
-        return res.json()["data"] if res else None
+        return self._req(url, method="GET", hint="Margins").json()["data"]
 
     def profile(self):
         """Retrieve the user profile"""
 
         th.check()
 
-        res = self._req(f"{self.base_url}/user/profile", "GET", hint="Profile")
-
-        return res.json()["data"] if res else None
+        return self._req(
+            f"{self.base_url}/user/profile", "GET", hint="Profile"
+        ).json()["data"]
 
     def historical_data(
         self,
         instrument_token: str,
         from_dt: Union[datetime, str],
         to_dt: Union[datetime, str],
         interval: str,
@@ -402,17 +376,17 @@
             "to": to_dt,
             "continuous": int(continuous),
             "oi": int(oi),
         }
 
         th.check("historical")
 
-        res = self._req(url, method="GET", payload=payload, hint="Historical")
-
-        return res.json()["data"]["candles"] if res else None
+        return self._req(
+            url, method="GET", payload=payload, hint="Historical"
+        ).json()["data"]["candles"]
 
     def place_order(
         self,
         variety,
         exchange,
         tradingsymbol,
         transaction_type,
@@ -427,104 +401,90 @@
         iceberg_legs=None,
         iceberg_quantity=None,
         auction_number=None,
         tag=None,
     ):
         """Place an order of a particular variety"""
 
-        url = f"{self.base_url}/orders/{variety}"
+        params = {k: v for k, v in locals().items() if v is not None}
 
-        params = locals()
-
-        del params["self"]
-
-        for k in params.keys():
-            if params[k] is None:
-                del params[k]
+        params.pop("self")
 
         th.check("order")
 
-        res = self._req(url, "POST", payload=params, hint="Place Order")
-
-        return res.json()["data"]["order_id"] if res else None
+        return self._req(
+            f"{self.base_url}/orders/{variety}",
+            "POST",
+            payload=params,
+            hint="Place Order",
+        ).json()["data"]["order_id"]
 
     def modify_order(
         self,
         variety,
         order_id,
         quantity=None,
         price=None,
         order_type=None,
         trigger_price=None,
         validity=None,
         disclosed_quantity=None,
     ):
         """Modify an open order."""
 
-        url = f"{self.base_url}/orders/{variety}/{order_id}"
-
-        params = locals()
-
-        del params["self"]
+        params = {k: v for k, v in locals().items() if v is not None}
 
-        for k in list(params.keys()):
-            if params[k] is None:
-                del params[k]
+        params.pop("self")
 
         th.check("order")
 
-        res = self._req(url, "PUT", payload=params, hint="Modify order")
-
-        return res.json()["data"]["order_id"] if res else None
+        return self._req(
+            f"{self.base_url}/orders/{variety}/{order_id}",
+            "PUT",
+            payload=params,
+            hint="Modify order",
+        ).json()["data"]["order_id"]
 
     def cancel_order(self, variety, order_id):
         """Cancel an order."""
 
         url = f"{self.base_url}/orders/{variety}/{order_id}"
 
         th.check("order")
 
-        res = self._req(url, "DELETE", hint="Cancel order")
-
-        return res.json()["data"]["order_id"] if res else None
+        return self._req(url, "DELETE", hint="Cancel order").json()["data"]
 
     def orders(self):
         """Get list of all orders for the day"""
 
         th.check("order")
 
-        res = self._req(f"{self.base_url}/orders", "GET", hint="Orders")
-
-        return res.json()["data"] if res else None
+        return self._req(
+            f"{self.base_url}/orders", "GET", hint="Orders"
+        ).json()["data"]
 
     def order_history(self, order_id):
         """Get history of individual orders"""
 
         url = f"{self.base_url}/orders/{order_id}"
 
         th.check("order")
 
-        res = self._req(url, "GET", hint="Order history")
-
-        return res.json()["data"] if res else None
+        return self._req(url, "GET", hint="Order history").json()["data"]
 
     def trades(self):
         """Get the list of all executed trades for the day"""
 
         url = f"{self.base_url}/trades"
 
         th.check()
 
-        res = self._req(url, "GET", hint="Trades")
-
-        return res.json()["data"] if res else None
+        return self._req(url, "GET", hint="Trades").json()["data"]
 
     def order_trades(self, order_id):
         """Get the the trades generated by an order"""
 
         url = f"{self.base_url}/orders/{order_id}/trades"
 
         th.check("orders")
 
-        res = self._req(url, "GET", hint="Order Trades")
-
-        return res.json()["data"] if res else None
+        return self._req(url, "GET", hint="Order Trades").json()["data"]
```

### Comparing `kitetrader-2.0.0/.gitignore` & `kitetrader-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `kitetrader-2.0.0/LICENSE` & `kitetrader-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kitetrader-2.0.0/README.md` & `kitetrader-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,33 +27,36 @@
 
 # close the requests session
 kite.close()
 ```
 
 ## Login
 
+**Update v2.1.0**
+
+- You can pass the user_id, password and OTP during class initialization. This allows full automation of script for those requiring it. See #notes below for details.
+
 On first initialization, Kite will check for user authentication. If no arguments are provided, the script prompts for username, password, and OTP.
 
 On successful login, an `enctoken` is generated and stored in a cookie file.
 
 If the cookie file exists on subsequent initialization, the `enctoken` is reused, eliminating the need to log in again.
 
 This method will logout all Kite web (browser) sessions. (You can continue to use the Kite Mobile App).
 
 You can reuse the browser `enctoken`, passing it to Kite. This way, you can use Kite without getting logged out.
 
 `kite = Kite(enctoken='<token string>')`
 
 To access the browser `enctoken`, login to kite.zerodha.com and press `SHIFT + F9` to open the Storage inspector (On Firefox). You will find the info under cookies.
 
-**Passing credentials file path**
-Credentials file is no longer supported. Storing plain text passwords in a file, could be unsafe.
-
 ## NOTES
 
+- Hard coding password and credentials can be risky. Take appropriate measure to safeguard your credentials from accidental uploads or exposure on shared computers. Stick to defaults or use enctoken if unsure.
+
 - Starting `v1.1.0`, kitetrader no longer exits on error. You must handle the error appropriately.
 
 - Methods may raise the following errors:
   - A `RuntimeError` is raised if too many (>15) 429 reponse codes are returned.
   - A `TimeoutError` is raised if server takes too long to respond.
   - A `ConnectionError` is raised if:
     - Session expired
@@ -276,15 +279,15 @@
 class Kite(builtins.object)
  |  Kite(enctoken: Optional[str] = None)
  |  
  |  Unofficial implementation of Zerodha Kite api
  |  
  |  Methods defined here:
  |  
- |  __init__(self, enctoken: Optional[str] = None)
+ |  __init__(self, user_id: Optional[str] = None, password: Optional[str] = None, twofa: Optional[str] = None, enctoken: Optional[str] = None)
  |      Initialize self.  See help(type(self)) for accurate signature.
  |  
  |  auctions(self)
  |      Retrieve the list of auctions that are currently being held
  |  
  |  cancel_order(self, variety, order_id)
  |      Cancel an order.
```

### Comparing `kitetrader-2.0.0/pyproject.toml` & `kitetrader-2.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kitetrader"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Benny Thadikaran" },
 ]
 description = "Unofficial Python Client for Zerodha Kite"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `kitetrader-2.0.0/PKG-INFO` & `kitetrader-2.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: kitetrader
-Version: 2.0.0
+Version: 2.1.0
 Summary: Unofficial Python Client for Zerodha Kite
 Project-URL: Homepage, https://github.com/BennyThadikaran/Kite-Trader
 Project-URL: Bug Tracker, https://github.com/BennyThadikaran/Kite-Trader/issues
 Author: Benny Thadikaran
 License-File: LICENSE
 Keywords: algo-trading,historical-data,intraday-data,kiteconnect,stock-data,stock-market,zerodha,zerodha-kite
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -44,33 +44,36 @@
 
 # close the requests session
 kite.close()
 ```
 
 ## Login
 
+**Update v2.1.0**
+
+- You can pass the user_id, password and OTP during class initialization. This allows full automation of script for those requiring it. See #notes below for details.
+
 On first initialization, Kite will check for user authentication. If no arguments are provided, the script prompts for username, password, and OTP.
 
 On successful login, an `enctoken` is generated and stored in a cookie file.
 
 If the cookie file exists on subsequent initialization, the `enctoken` is reused, eliminating the need to log in again.
 
 This method will logout all Kite web (browser) sessions. (You can continue to use the Kite Mobile App).
 
 You can reuse the browser `enctoken`, passing it to Kite. This way, you can use Kite without getting logged out.
 
 `kite = Kite(enctoken='<token string>')`
 
 To access the browser `enctoken`, login to kite.zerodha.com and press `SHIFT + F9` to open the Storage inspector (On Firefox). You will find the info under cookies.
 
-**Passing credentials file path**
-Credentials file is no longer supported. Storing plain text passwords in a file, could be unsafe.
-
 ## NOTES
 
+- Hard coding password and credentials can be risky. Take appropriate measure to safeguard your credentials from accidental uploads or exposure on shared computers. Stick to defaults or use enctoken if unsure.
+
 - Starting `v1.1.0`, kitetrader no longer exits on error. You must handle the error appropriately.
 
 - Methods may raise the following errors:
   - A `RuntimeError` is raised if too many (>15) 429 reponse codes are returned.
   - A `TimeoutError` is raised if server takes too long to respond.
   - A `ConnectionError` is raised if:
     - Session expired
@@ -293,15 +296,15 @@
 class Kite(builtins.object)
  |  Kite(enctoken: Optional[str] = None)
  |  
  |  Unofficial implementation of Zerodha Kite api
  |  
  |  Methods defined here:
  |  
- |  __init__(self, enctoken: Optional[str] = None)
+ |  __init__(self, user_id: Optional[str] = None, password: Optional[str] = None, twofa: Optional[str] = None, enctoken: Optional[str] = None)
  |      Initialize self.  See help(type(self)) for accurate signature.
  |  
  |  auctions(self)
  |      Retrieve the list of auctions that are currently being held
  |  
  |  cancel_order(self, variety, order_id)
  |      Cancel an order.
```

