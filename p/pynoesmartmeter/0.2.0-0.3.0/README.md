# Comparing `tmp/pynoesmartmeter-0.2.0.tar.gz` & `tmp/pynoesmartmeter-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynoesmartmeter-0.2.0.tar", max compression
+gzip compressed data, was "pynoesmartmeter-0.3.0.tar", max compression
```

## Comparing `pynoesmartmeter-0.2.0.tar` & `pynoesmartmeter-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.2.0/LICENSE
--rw-r--r--   0        0        0     1773 2024-04-09 19:49:23.005538 pynoesmartmeter-0.2.0/README.md
--rw-r--r--   0        0        0      468 2024-04-09 19:56:59.836345 pynoesmartmeter-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.2.0/src/pynoesmartmeter/__init__.py
--rw-r--r--   0        0        0     9369 2024-04-09 19:55:51.026498 pynoesmartmeter-0.2.0/src/pynoesmartmeter/client.py
--rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.2.0/src/pynoesmartmeter/errors.py
--rw-r--r--   0        0        0     2292 1970-01-01 00:00:00.000000 pynoesmartmeter-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-03-23 18:14:39.956539 pynoesmartmeter-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1716 2024-04-15 15:15:57.546593 pynoesmartmeter-0.3.0/README.md
+-rw-r--r--   0        0        0      507 2024-04-15 15:16:42.628054 pynoesmartmeter-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      241 2024-03-29 16:58:07.196697 pynoesmartmeter-0.3.0/src/pynoesmartmeter/__init__.py
+-rw-r--r--   0        0        0     9886 2024-04-15 15:11:39.403601 pynoesmartmeter-0.3.0/src/pynoesmartmeter/client.py
+-rw-r--r--   0        0        0      679 2024-03-29 14:27:30.372086 pynoesmartmeter-0.3.0/src/pynoesmartmeter/errors.py
+-rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 pynoesmartmeter-0.3.0/PKG-INFO
```

### Comparing `pynoesmartmeter-0.2.0/LICENSE` & `pynoesmartmeter-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.2.0/README.md` & `pynoesmartmeter-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 <h1 align="center">
   NÖ Smart Meter
 </h1>
 <h4 align="center">An unofficial python wrapper for the <a href="https://smartmeter.netz-noe.at/#/" target="_blank">EVN - Netz Niederösterreich</a> private API.
 </h4>
 
------
 <h2>
   WARNING: This library is still work in progress and might change a lot!
   This project will be used in a home assistant integration. 
 </h2>
 
 
 ## Features
@@ -25,25 +24,24 @@
 `pip install pynoesmartmeter`
 
 ## How To Use
 
 Import the Smartmeter client, provide login information and access available api functions:
 
 ```python
+import asyncio
 from pynoesmartmeter import Smartmeter
 
 username = 'YOUR_LOGIN_USER_NAME'
 password = 'YOUR_PASSWORD'
 
 offset = 0
 
 api = Smartmeter(USERNAME, PASSWORD)
-loop = asyncio.get_event_loop()
-coroutine = api.get_consumption_since_date("24.03.2024 10:03", offset)
-loop.run_until_complete(coroutine)
+asyncio.run(api.get_consumption_since_date("24.03.2024 10:03", offset))
 
 ```
 
 
 ## Awesome projects
 - **EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/mobilfunk/evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/) \
 I used his code as the base for this project.
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
                          ************ NN?Ã? SSmmaarrtt MMeetteerr ************
  ****** AAnn uunnooffffiicciiaall ppyytthhoonn wwrraappppeerr ffoorr tthhee _EE_VV_NN_ _--_ _NN_ee_tt_zz_ _NN_ii_ee_dd_ee_rr_?Ã_?¶_ss_tt_ee_rr_rr_ee_ii_cc_hh pprriivvaattee
                                    AAPPII.. ******
------
 ********** WWAARRNNIINNGG:: TThhiiss lliibbrraarryy iiss ssttiillll wwoorrkk iinn pprrooggrreessss aanndd mmiigghhtt cchhaannggee aa lloott!!
 TThhiiss pprroojjeecctt wwiillll bbee uusseedd iinn aa hhoommee aassssiissttaanntt iinntteeggrraattiioonn.. **********
 ## Features - Access energy usage - Get user & meter information This library
 is currently written for asynchronous use. There might be a synchronous version
 in the future. ## Installation Install with pip: `pip install pynoesmartmeter`
 ## How To Use Import the Smartmeter client, provide login information and
-access available api functions: ```python from pynoesmartmeter import
-Smartmeter username = 'YOUR_LOGIN_USER_NAME' password = 'YOUR_PASSWORD' offset
-= 0 api = Smartmeter(USERNAME, PASSWORD) loop = asyncio.get_event_loop()
-coroutine = api.get_consumption_since_date("24.03.2024 10:03", offset)
-loop.run_until_complete(coroutine) ``` ## Awesome projects -
-**EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/mobilfunk/
-evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/) \ I used
-his code as the base for this project. - **vienna-smartmeter** from platysma
-(https://github.com/platysma/vienna-smartmeter) \ I used this project as a
-starting point. (I even stole the readme) ## License > You can check out the
-full license [here](https://github.com/xilinx64/vienna-smartmeter/blob/main/
-LICENSE) This project is licensed under the terms of the **MIT** license. ##
-Legal Disclaimer: This is not affliated, endorsed or certified by Netz
+access available api functions: ```python import asyncio from pynoesmartmeter
+import Smartmeter username = 'YOUR_LOGIN_USER_NAME' password = 'YOUR_PASSWORD'
+offset = 0 api = Smartmeter(USERNAME, PASSWORD) asyncio.run
+(api.get_consumption_since_date("24.03.2024 10:03", offset)) ``` ## Awesome
+projects - **EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/
+mobilfunk/evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/
+) \ I used his code as the base for this project. - **vienna-smartmeter** from
+platysma (https://github.com/platysma/vienna-smartmeter) \ I used this project
+as a starting point. (I even stole the readme) ## License > You can check out
+the full license [here](https://github.com/xilinx64/vienna-smartmeter/blob/
+main/LICENSE) This project is licensed under the terms of the **MIT** license.
+## Legal Disclaimer: This is not affliated, endorsed or certified by Netz
 NiederÃ¶sterreich GmbH. This is an independent and unofficial API. Strictly not
 for spam. Use at your own risk.
```

### Comparing `pynoesmartmeter-0.2.0/src/pynoesmartmeter/client.py` & `pynoesmartmeter-0.3.0/src/pynoesmartmeter/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Contains the Smartmeter API Client."""
 
 import logging
 
 import datetime
 import os
 import pickle
-import requests
+import httpx
+import aiofiles
 
 
 from .errors import SmartmeterLoginError, SmartmeterConnectionError
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,70 +22,90 @@
 
     API_USER_DETAILS_URL = API_BASE_URL + "/User/GetBasicInfo"
     API_ACCOUNTING_DETAILS_URL = API_BASE_URL + "/User/GetAccountIdByBussinespartnerId"
     API_METER_DETAILS_URL = API_BASE_URL + "/User/GetMeteringPointByAccountId"
 
     API_CONSUMPTION_URL = API_BASE_URL + "/ConsumptionRecord"
 
+    SESSION_FILE = "noe_smartmeter_session_httpx.pkl"
+
     def __init__(self, username, password):
         """Access the Smartmeter API."""
         self.supports_api = False
         self._metering_point_id = None
         self._account_id = None
         self._session = None
         self._username = username
         self._password = password
 
-    async def authenticate(self, username, password):
+    async def authenticate(self, username = None, password = None):
         """Load session file or authenticate user."""
-        session = None
-        session_file = "noe_smartmeter_session.pkl"
+        if username is not None:
+            self._username = username
+        if password is not None:
+            self._password = password
+
+        if await self._load_check_session():
+           return True
+
+        print("Starting new session and authenticate")
+        session = httpx.AsyncClient(timeout=30.0)
+        auth_data = {"user": self._username, "pwd": self._password}
+        response = await session.post(self.AUTH_URL, data=auth_data)
+
+        if response.status_code == 200:
+            print("Authentication sucessful")
+        elif response.status_code == 401:
+            raise SmartmeterLoginError("Login failed. Check username/password.")
+        else:
+            raise SmartmeterConnectionError(
+                f"Authentication failed with status {response.status_code}"
+            )
+        await self._save_session(session)
+        
+        self._session = session
+        return True
 
+    async def _check_session(self, session):
+        try:
+            response = await session.get(self.API_USER_DETAILS_URL)
+            return response.status_code == 200
+        except (TypeError) as error:
+            print(error)
+            return False
+
+    async def _save_session(self, session):
+        serialized_data = pickle.dumps(dict(session.cookies))
+        async with aiofiles.open(self.SESSION_FILE, "wb") as f:
+            await f.write(serialized_data)
+    
+    async def _load_check_session(self):
         # Check if a cached session exists
-        if os.path.exists(session_file):
-            with open(session_file, "rb") as f:
-                session = pickle.load(f)
-                # Check if the cached session is still valid
-                print("Check if stored Session is valid...")
-                response = session.get(self.API_USER_DETAILS_URL)
-                if response.status_code != 200:
-                    session = None
-                    print("Stored session is not valid")
-                    print("Reauthenticating...")
-                else:
-                    print("Stored session is valid")
-
-        # If a valid session doesn't exist, authenticate the user
-        if session is None:
-            session = requests.Session()
-            auth_data = {"user": username, "pwd": password}
-            response = session.post(self.AUTH_URL, json=auth_data)
-            if response.status_code == 200:
-                print("Authentication sucessful")
-            elif response.status_code == 401:
-                raise SmartmeterLoginError("Login failed. Check username/password.")
-            else:
-                raise SmartmeterConnectionError(
-                    f"Authentication failed with status {response.status_code}"
-                )
-            # Save the session to disk
-            with open(session_file, "wb") as f:
-                pickle.dump(session, f)
+        print("Checking stored session")
+        if os.path.exists(self.SESSION_FILE):
+            async with aiofiles.open(self.SESSION_FILE, "rb") as f:
+                data = await f.read()
+                cookies = pickle.loads(data)
+                session = httpx.AsyncClient(timeout=30.0, cookies=cookies)
+                if await self._check_session(session):
+                    print("Stored Session is valid")
+                    self._session = session
+                    return True           
+        print("Session is not stored or invalid!")                
+        return False
 
-        self._session = session
-        return True
 
     async def _call_api(self, url, params=None):
         if self._session is None:
-            await self.authenticate(self._username, self._password)
+            await self.authenticate()
         retry_count = 0
         while retry_count < 1:
-            response = self._session.get(url, params=params)
+            response = await self._session.get(url, params=params)
             if response.status_code == 401:
-                await self.authenticate(self._username, self._password)
+                await self.authenticate()
                 retry_count += 1
             elif response.status_code == 200:
                 return response
 
     async def get_user_details(self):
         """Load user details"""
         response = await self._call_api(self.API_USER_DETAILS_URL + "?context=2")
@@ -132,15 +153,15 @@
                 params={"meterId": self._metering_point_id, "day": day},
             )
             data = response.json()[0]
             consumption_per_day = list(
                 zip(data["peakDemandTimes"], data["meteredValues"])
             )
             return consumption_per_day
-        except (requests.exceptions.RequestException, ValueError) as error:
+        except (httpx.RequestError, ValueError) as error:
             print(f"An error occurred: {error}")
             return []
 
     async def get_consumption_for_month(self, year, month):
         """Load consumption for one month"""
         print(f"Load consumption for month {month}/{year}")
         if self._metering_point_id is None:
@@ -155,15 +176,15 @@
                 },
             )
             data = response.json()[0]
             consumption_for_month = list(
                 zip(data["peakDemandTimes"], data["meteredValues"])
             )
             return consumption_for_month
-        except (requests.exceptions.RequestException, ValueError) as error:
+        except (httpx.RequestError, ValueError) as error:
             print(f"An error occurred: {error}")
             return []
 
     async def get_consumption_for_year(self, year):
         """Load consumption for one year"""
         print("Load consumption for year:", year)
         if self._metering_point_id is None:
@@ -173,15 +194,15 @@
                 self.API_CONSUMPTION_URL + "/Year",
                 params={"meterId": self._metering_point_id, "year": year},
             )
             response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
             data = response.json()[0]
             consumption_for_year = list(zip(data["peakDemandTimes"], data["values"]))
             return consumption_for_year
-        except (requests.exceptions.RequestException, ValueError) as error:
+        except (httpx.RequestError, ValueError) as error:
             print(f"An error occurred: {error}")
             return []
 
     async def get_consumption_since_date(self, input_date_string, offset):
         """Load consumption since a specific datetime and adds the offset"""
         current_date = datetime.date.today()
         input_date = datetime.datetime.strptime(input_date_string, "%d.%m.%Y %H:%M")
@@ -228,9 +249,9 @@
             for year in range(start_year, current_date.year + 1):
                 year_values = await self.get_consumption_for_year(year)
                 energy_sum += sum(
                     value[1] for value in year_values if value[1] is not None
                 )
 
         # It is assumed that the last datapoint is from the current date at 00:00 since the smartmeter only transmits data once a day
-        print(f"COnsumption until {current_date.strftime("%d.%m.%Y %H:%M")}: {energy_sum + offset}")
+        print(f"Consumption until {current_date.strftime("%d.%m.%Y %H:%M")}: {energy_sum + offset}")
         return (current_date.strftime("%d.%m.%Y %H:%M"), energy_sum + offset)
```

### Comparing `pynoesmartmeter-0.2.0/src/pynoesmartmeter/errors.py` & `pynoesmartmeter-0.3.0/src/pynoesmartmeter/errors.py`

 * *Files identical despite different names*

### Comparing `pynoesmartmeter-0.2.0/PKG-INFO` & `pynoesmartmeter-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pynoesmartmeter
-Version: 0.2.0
+Version: 0.3.0
 Summary: Python library to access the Netz Nö (EVN) Smart Meter private API
 License: MIT
 Author: David Illichmann
 Author-email: david.illichmann@ebcont.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   NÖ Smart Meter
 </h1>
 <h4 align="center">An unofficial python wrapper for the <a href="https://smartmeter.netz-noe.at/#/" target="_blank">EVN - Netz Niederösterreich</a> private API.
 </h4>
 
------
 <h2>
   WARNING: This library is still work in progress and might change a lot!
   This project will be used in a home assistant integration. 
 </h2>
 
 
 ## Features
@@ -40,25 +41,24 @@
 `pip install pynoesmartmeter`
 
 ## How To Use
 
 Import the Smartmeter client, provide login information and access available api functions:
 
 ```python
+import asyncio
 from pynoesmartmeter import Smartmeter
 
 username = 'YOUR_LOGIN_USER_NAME'
 password = 'YOUR_PASSWORD'
 
 offset = 0
 
 api = Smartmeter(USERNAME, PASSWORD)
-loop = asyncio.get_event_loop()
-coroutine = api.get_consumption_since_date("24.03.2024 10:03", offset)
-loop.run_until_complete(coroutine)
+asyncio.run(api.get_consumption_since_date("24.03.2024 10:03", offset))
 
 ```
 
 
 ## Awesome projects
 - **EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/mobilfunk/evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/) \
 I used his code as the base for this project.
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
-Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.2.0 Summary: Python
+Metadata-Version: 2.1 Name: pynoesmartmeter Version: 0.3.0 Summary: Python
 library to access the Netz NÃ¶ (EVN) Smart Meter private API License: MIT
 Author: David Illichmann Author-email: david.illichmann@ebcont.com Requires-
 Python: >=3.12,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: asyncio (>=3.4.3,<4.0.0) Requires-
-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/markdown
+Language :: Python :: 3.12 Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-
+Dist: asyncio (>=3.4.3,<4.0.0) Requires-Dist: httpx (>=0.27.0,<0.28.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0) Description-Content-Type: text/
+markdown
                          ************ NN?Ã? SSmmaarrtt MMeetteerr ************
  ****** AAnn uunnooffffiicciiaall ppyytthhoonn wwrraappppeerr ffoorr tthhee _EE_VV_NN_ _--_ _NN_ee_tt_zz_ _NN_ii_ee_dd_ee_rr_?Ã_?¶_ss_tt_ee_rr_rr_ee_ii_cc_hh pprriivvaattee
                                    AAPPII.. ******
------
 ********** WWAARRNNIINNGG:: TThhiiss lliibbrraarryy iiss ssttiillll wwoorrkk iinn pprrooggrreessss aanndd mmiigghhtt cchhaannggee aa lloott!!
 TThhiiss pprroojjeecctt wwiillll bbee uusseedd iinn aa hhoommee aassssiissttaanntt iinntteeggrraattiioonn.. **********
 ## Features - Access energy usage - Get user & meter information This library
 is currently written for asynchronous use. There might be a synchronous version
 in the future. ## Installation Install with pip: `pip install pynoesmartmeter`
 ## How To Use Import the Smartmeter client, provide login information and
-access available api functions: ```python from pynoesmartmeter import
-Smartmeter username = 'YOUR_LOGIN_USER_NAME' password = 'YOUR_PASSWORD' offset
-= 0 api = Smartmeter(USERNAME, PASSWORD) loop = asyncio.get_event_loop()
-coroutine = api.get_consumption_since_date("24.03.2024 10:03", offset)
-loop.run_until_complete(coroutine) ``` ## Awesome projects -
-**EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/mobilfunk/
-evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/) \ I used
-his code as the base for this project. - **vienna-smartmeter** from platysma
-(https://github.com/platysma/vienna-smartmeter) \ I used this project as a
-starting point. (I even stole the readme) ## License > You can check out the
-full license [here](https://github.com/xilinx64/vienna-smartmeter/blob/main/
-LICENSE) This project is licensed under the terms of the **MIT** license. ##
-Legal Disclaimer: This is not affliated, endorsed or certified by Netz
+access available api functions: ```python import asyncio from pynoesmartmeter
+import Smartmeter username = 'YOUR_LOGIN_USER_NAME' password = 'YOUR_PASSWORD'
+offset = 0 api = Smartmeter(USERNAME, PASSWORD) asyncio.run
+(api.get_consumption_since_date("24.03.2024 10:03", offset)) ``` ## Awesome
+projects - **EVN_Smartmeter_Wrapper** from A.E.I.O.U. (https://www.lteforum.at/
+mobilfunk/evn-smartmeter-api-wrapper-influx-importer-grafana-dashboard.21319/
+) \ I used his code as the base for this project. - **vienna-smartmeter** from
+platysma (https://github.com/platysma/vienna-smartmeter) \ I used this project
+as a starting point. (I even stole the readme) ## License > You can check out
+the full license [here](https://github.com/xilinx64/vienna-smartmeter/blob/
+main/LICENSE) This project is licensed under the terms of the **MIT** license.
+## Legal Disclaimer: This is not affliated, endorsed or certified by Netz
 NiederÃ¶sterreich GmbH. This is an independent and unofficial API. Strictly not
 for spam. Use at your own risk.
```

