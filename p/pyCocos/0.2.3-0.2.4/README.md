# Comparing `tmp/pyCocos-0.2.3.tar.gz` & `tmp/pycocos-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyCocos-0.2.3.tar", last modified: Mon Feb  5 04:17:04 2024, max compression
+gzip compressed data, was "pycocos-0.2.4.tar", last modified: Mon Apr 15 00:10:11 2024, max compression
```

## Comparing `pyCocos-0.2.3.tar` & `pycocos-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:17:04.759858 pyCocos-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-02-05 04:16:52.000000 pyCocos-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-02-05 04:17:04.759858 pyCocos-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-02-05 04:16:52.000000 pyCocos-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 04:17:04.759858 pyCocos-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-05 04:16:52.000000 pyCocos-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:17:04.755858 pyCocos-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:17:04.759858 pyCocos-0.2.3/src/pyCocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-02-05 04:17:04.000000 pyCocos-0.2.3/src/pyCocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-02-05 04:17:04.000000 pyCocos-0.2.3/src/pyCocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 04:17:04.000000 pyCocos-0.2.3/src/pyCocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-05 04:17:04.000000 pyCocos-0.2.3/src/pyCocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-05 04:17:04.000000 pyCocos-0.2.3/src/pyCocos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:17:04.759858 pyCocos-0.2.3/src/pycocos/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 04:17:04.759858 pyCocos-0.2.3/src/pycocos/components/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15378 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/components/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/components/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/components/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/components/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    50794 2024-02-05 04:16:52.000000 pyCocos-0.2.3/src/pycocos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 00:10:07.000000 pycocos-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-15 00:10:11.684365 pycocos-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-15 00:10:07.000000 pycocos-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:10:11.684365 pycocos-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 00:10:07.000000 pycocos-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.680365 pycocos-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/src/pyCocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/src/pycocos/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/src/pycocos/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52337 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/main.py
```

### Comparing `pyCocos-0.2.3/LICENSE` & `pycocos-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyCocos-0.2.3/PKG-INFO` & `pycocos-0.2.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: pyCocos
-Version: 0.2.3
-Summary: Python connector for Cocos Capital's Rest APIs.
-Home-page: https://github.com/nacho-herrera/pyCocos
-Author: Nacho Herrera
-Author-email: github@nachoherrera.com.ar
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Office/Business :: Financial :: Investment
-Classifier: Topic :: Software Development
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: simplejson>=3.19.1
-
 # Welcome to pyCocos' Documentation
 
 ## Overview
 
 *pyCocos* is a Python library that enables interaction with Cocos Capital REST APIs. It is designed to save developers hours of research and coding required to connect to Cocos Capital REST APIs.
 
 ## Disclaimer
@@ -44,24 +23,30 @@
 ## Dependencies
 
 The library has the following dependency:
 
 ```
 requests>=2.31.0
 simplejson>=3.19.1
+pyotp>=2.9.0
 ```
 ## Features
 
 This section describes the functionality and components of the library.
 
 #### Available Methods
 
 #### Initialization
 
-Before using the library, you need to initialize it with a valid email and password. You can find the token using the browser dev-yTools.
+Before using the library, you need to initialize it with a valid email and password. The library includes the working webpage api_key token, but if that token is updated, you can find it using the browser dev-tools and pass it on initialization with the *api_key* parameter.
+
+#### 2nd Factor Authentication
+
+On 4/13/2024 Cocos Capital implemented a 2nd factor authentication for all users. Different users may have SMS, Mail or TOTP app authentication. The library implements pyotp library for automatic code generation. To use that feature, topt secret key must be passed as parameters *topt_secret_key* parameter on initialization. If parameter is not passed, library will request code interactively. 
+If you have TOTP app activated, you can get your secret key using this [method](https://shieldplanet.com/extract-secret-keys-from-google-authenticator-qr-code/). Pyotp implementation was kindly developed by @El_Raulo on Telegram. 
 
 #### REST
 
 The library provides functions to make requests to the REST API and retrieve the corresponding responses.
 
 ###### Functions
 
@@ -111,17 +96,20 @@
 ## Usage
 
 Once the library has been installed, you can import and initialize it. The initialization sets the email, password, and reCAPTCHA token. It then attempts to authenticate with the provided credentials. If the authentication fails, an `ApiException` is thrown.
 
 ```python
 from pycocos import Cocos
 
-app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd")
+app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd", api_key="OPTIONAL", topt_secret_key="OPTIONAL")
+
 ```
 
+*api_key* and *topt_secret_key* are optional parameters, default values are None.
+
 #### REST
 
 ```python
 # Get the available portfolio with the current market valuation
 app.my_portfolio()
 
 # Get the available funds
@@ -156,8 +144,9 @@
 
 ## Official API Documentation
 
 There is no official API documentation for this library. The library was created by webscraping the app.
 
 ## Acknowledgements
 
-This library was created with the support of the Scrappers Argentinos and Inversiones y Algoritmos Telegram Groups.
+This library was created with the support of the Scrappers Argentinos and Inversiones y Algoritmos Telegram Groups. 
+Updated version that includes OTP validation is based on the development and testing of @El_Raulo, @mjcolom and @sebivaq. Special thanks to them.
```

### Comparing `pyCocos-0.2.3/setup.py` & `pycocos-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyCocos",
-    version="0.2.3",
+    version="0.2.4",
     author="Nacho Herrera",
     author_email="github@nachoherrera.com.ar",
     description="Python connector for Cocos Capital's Rest APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nacho-herrera/pyCocos",
     packages=setuptools.find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'requests>=2.31.0',
         'simplejson>=3.19.1',
+        'pyotp>=2.9.0'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

### Comparing `pyCocos-0.2.3/src/pyCocos.egg-info/PKG-INFO` & `pycocos-0.2.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,14 +14,15 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: simplejson>=3.19.1
+Requires-Dist: pyotp>=2.9.0
 
 # Welcome to pyCocos' Documentation
 
 ## Overview
 
 *pyCocos* is a Python library that enables interaction with Cocos Capital REST APIs. It is designed to save developers hours of research and coding required to connect to Cocos Capital REST APIs.
 
@@ -44,24 +45,30 @@
 ## Dependencies
 
 The library has the following dependency:
 
 ```
 requests>=2.31.0
 simplejson>=3.19.1
+pyotp>=2.9.0
 ```
 ## Features
 
 This section describes the functionality and components of the library.
 
 #### Available Methods
 
 #### Initialization
 
-Before using the library, you need to initialize it with a valid email and password. You can find the token using the browser dev-yTools.
+Before using the library, you need to initialize it with a valid email and password. The library includes the working webpage api_key token, but if that token is updated, you can find it using the browser dev-tools and pass it on initialization with the *api_key* parameter.
+
+#### 2nd Factor Authentication
+
+On 4/13/2024 Cocos Capital implemented a 2nd factor authentication for all users. Different users may have SMS, Mail or TOTP app authentication. The library implements pyotp library for automatic code generation. To use that feature, topt secret key must be passed as parameters *topt_secret_key* parameter on initialization. If parameter is not passed, library will request code interactively. 
+If you have TOTP app activated, you can get your secret key using this [method](https://shieldplanet.com/extract-secret-keys-from-google-authenticator-qr-code/). Pyotp implementation was kindly developed by @El_Raulo on Telegram. 
 
 #### REST
 
 The library provides functions to make requests to the REST API and retrieve the corresponding responses.
 
 ###### Functions
 
@@ -111,17 +118,20 @@
 ## Usage
 
 Once the library has been installed, you can import and initialize it. The initialization sets the email, password, and reCAPTCHA token. It then attempts to authenticate with the provided credentials. If the authentication fails, an `ApiException` is thrown.
 
 ```python
 from pycocos import Cocos
 
-app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd")
+app = Cocos(email="sample@email.com", password="S4mp13.p4ssW0rd", api_key="OPTIONAL", topt_secret_key="OPTIONAL")
+
 ```
 
+*api_key* and *topt_secret_key* are optional parameters, default values are None.
+
 #### REST
 
 ```python
 # Get the available portfolio with the current market valuation
 app.my_portfolio()
 
 # Get the available funds
@@ -156,8 +166,9 @@
 
 ## Official API Documentation
 
 There is no official API documentation for this library. The library was created by webscraping the app.
 
 ## Acknowledgements
 
-This library was created with the support of the Scrappers Argentinos and Inversiones y Algoritmos Telegram Groups.
+This library was created with the support of the Scrappers Argentinos and Inversiones y Algoritmos Telegram Groups. 
+Updated version that includes OTP validation is based on the development and testing of @El_Raulo, @mjcolom and @sebivaq. Special thanks to them.
```

### Comparing `pyCocos-0.2.3/src/pycocos/components/client.py` & `pycocos-0.2.4/src/pycocos/components/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,27 @@
         Returns:
             dict: Dict with token and user data
         """
         return self.api_request(
             urls.endpoints["token"], method="post", params=params, data=data
         )
 
+    def get_2factors(self):
+        return self.api_request(urls.endpoints["2factors"])
+
+    def submit_challenge_request(self, challenge_id: str):
+        return self.api_request(
+            urls.endpoints["challenge"].format(challenge_id), method="post"
+        )
+
+    def submit_challenge_verification(self, challenge_id: str, json: str):
+        return self.api_request(
+            urls.endpoints["verify"].format(challenge_id), method="post", json_data=json
+        )
+
     def logout(self) -> None:
         """Makes a request to the api to logout current session
 
         Returns:
             dict: empty dict
         """
         return self.api_request(urls.endpoints["logout"], method="post")
@@ -445,22 +458,21 @@
                 self._api_url(path),
                 params=params,
                 data=data,
                 json=json_data,
             )
 
         if method == "delete":
-            response = self.session.delete(
-                self._api_url(path), json=json_data
-            )
+            response = self.session.delete(self._api_url(path), json=json_data)
+
         if not response:
             raise ApiException("Bad HTTP API Response")
 
         json_response = simplejson.loads(response.text)
-        
+
         if response.status_code == 401:
             if retry:
                 self.api_request(path, retry=False)
             else:
                 raise ApiException("Authentication Fails.")
 
         if response.status_code == 500:
```

### Comparing `pyCocos-0.2.3/src/pycocos/components/enums.py` & `pycocos-0.2.4/src/pycocos/components/enums.py`

 * *Files identical despite different names*

### Comparing `pyCocos-0.2.3/src/pycocos/components/urls.py` & `pycocos-0.2.4/src/pycocos/components/urls.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 """
 
 api_url = "https://api.cocos.capital/"
 
 endpoints = {
     "token": "auth/v1/token",
     "logout": "auth/v1/logout",
+    "2factors": "auth/v1/factors/default",
+    "challenge": "auth/v1/factors/{}/challenge",
+    "verify": "auth/v1/factors/{}/verify",
     "open_market": "api/v1/calendar/open-market",
     "carrousel": "api/v1/home/carrousel",
     "news": "api/v1/home/news",
     "university": "api/v1/home/university",
     "dolar_mep": "api/v1/markets/dolar-mep",
     "home_list": "api/v1/markets/lists/home",
     "my_list": "api/v1/markets/lists/me",
```

### Comparing `pyCocos-0.2.3/src/pycocos/main.py` & `pycocos-0.2.4/src/pycocos/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """
     pyCocos.main
     Main client.
 """
 from __future__ import annotations
 from typing import Any, Dict, List, Optional, Tuple
+import pyotp
 import json
 
 from .components import (
     ApiException,
     Currency,
     InstrumentSubType,
     InstrumentType,
@@ -23,15 +24,15 @@
 
 class Cocos:
     headers: dict[str, str] = {
         "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:91.0) Gecko/20100101 Firefox/91.0",
         "Content-Type": "application/json",
     }
 
-    def __init__(self, email: str, password: str, gotrue_meta_security: Optional[Dict[str, Any]] = {}, api_key: Optional[str] = None) -> None:
+    def __init__(self, email: str, password: str, gotrue_meta_security: Optional[Dict[str, Any]] = {}, api_key: Optional[str] = None, topt_secret_key: Optional[str] = None) -> None:
         ## Parameters validation
         required_fields: list[tuple[str, Any, Any]]  = [
             ("email", email, str),
             ("password", password, str),
             ("gotrue_meta_security", gotrue_meta_security, dict),
         ]
         self._check_fields(required_fields)
@@ -51,14 +52,20 @@
 
         ## Login Information
         self.email: str = email
         self.password: str = password
         self.gotrue_meta_security: Dict[str, Any] = gotrue_meta_security
         #self.recaptcha_token: str = recaptcha_token
         self.account_number: str = ""
+
+        if topt_secret_key:
+            self.topt = pyotp.TOTP(topt_secret_key)
+        else:
+            self.topt = None
+
         if not api_key: 
             self.api_key = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.ewogICJyb2xlIjogImFub24iLAogICJpc3MiOiAic3VwYWJhc2UiLAogICJpYXQiOiAxNzA0NjgyODAwLAogICJleHAiOiAxODYyNTM1NjAwCn0.f0w62k0q0eyyGBDkAP7vUUEg_Ingb9YbOlhsGCC4R3c"  # Working apikey from main JS File - 2024-02-05.
         else:
             self.api_key = api_key
                 
         ## Current session variables # ! NEEDS TO BE DEVELOPED
         self.orders: List[str] = []
@@ -91,15 +98,51 @@
         if "success" in response.keys() and response["success"] == False:
             raise Exception(f'Error: {response["message"]}')
 
         if "access_token" not in response.keys():
             raise Exception("Error: Access token not found in the API response")
 
         self.access_token = response["access_token"]
-        self._auth_phase_2()
+        self._2fa_challenge()
+
+    def _2fa_challenge(self) -> None:
+        headers_update: dict[str, str] = {
+            "apikey": self.api_key,
+            "authorization": f"Bearer {self.access_token}",
+        }
+        
+        self.client.update_session_headers(headers_update)
+        second_factor_response = self.client.get_2factors()
+        if "requireChallenge" in second_factor_response.keys() and second_factor_response["requireChallenge"]:
+            challenge_id = second_factor_response["id"]
+        
+        payload = json.dumps({
+            "expires_at": 123, 
+            "id": challenge_id,
+        })
+
+        challenge = self.client.submit_challenge_request(challenge_id=challenge_id)
+        
+        if challenge_id not in ["mail", "sms"] and self.topt is not None:
+            code = self.topt.now()
+        else:
+            code = input("Insert 2FA Code: ")
+        payload = {
+            "challenge_id": "_",
+            "code": code,
+        }
+        
+        #self.client.update_session_headers(headers_update)        
+        response = self.client.submit_challenge_verification(challenge_id=challenge_id, json=payload)
+
+        if "access_token" not in response.keys():
+            raise Exception("Error: Access token not found in the API response")
+        else:
+            self.access_token = response["access_token"]
+            self._auth_phase_2()
 
     def _auth_phase_2(self) -> None:
         """Updates the session headers and performs additional steps after login.
 
         After successful login and obtaining the access token, this method is responsible for updating the session headers
         with the necessary authentication information. It replicates the workflow of the web app.
```

