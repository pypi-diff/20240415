# Comparing `tmp/hyper_sdk-0.1.0.tar.gz` & `tmp/hyper_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper_sdk-0.1.0.tar", last modified: Tue Apr  9 18:06:12 2024, max compression
+gzip compressed data, was "hyper_sdk-0.1.1.tar", last modified: Mon Apr 15 13:33:54 2024, max compression
```

## Comparing `hyper_sdk-0.1.0.tar` & `hyper_sdk-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 18:06:12.141070 hyper_sdk-0.1.0/
--rw-rw-rw-   0        0        0     1093 2024-04-07 08:49:14.000000 hyper_sdk-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     6002 2024-04-09 18:06:12.139557 hyper_sdk-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5370 2024-04-09 17:59:05.000000 hyper_sdk-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 18:06:12.128027 hyper_sdk-0.1.0/hyper_sdk/
--rw-rw-rw-   0        0        0      186 2024-04-09 13:40:00.000000 hyper_sdk-0.1.0/hyper_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:06:12.137427 hyper_sdk-0.1.0/hyper_sdk/akamai/
--rw-rw-rw-   0        0        0      102 2024-04-09 14:00:05.000000 hyper_sdk-0.1.0/hyper_sdk/akamai/__init__.py
--rw-rw-rw-   0        0        0     2774 2023-12-24 14:34:58.000000 hyper_sdk-0.1.0/hyper_sdk/akamai/pixel.py
--rw-rw-rw-   0        0        0      929 2023-12-24 14:34:58.000000 hyper_sdk-0.1.0/hyper_sdk/akamai/script_path.py
--rw-rw-rw-   0        0        0     3912 2024-04-09 14:10:29.000000 hyper_sdk-0.1.0/hyper_sdk/akamai/sec_cpt.py
--rw-rw-rw-   0        0        0     1898 2023-12-25 13:39:54.000000 hyper_sdk-0.1.0/hyper_sdk/akamai/stop_signal.py
--rw-rw-rw-   0        0        0      532 2024-04-07 08:09:37.000000 hyper_sdk-0.1.0/hyper_sdk/akamai_input.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:06:12.139021 hyper_sdk-0.1.0/hyper_sdk/incapsula/
--rw-rw-rw-   0        0        0       22 2024-04-09 14:00:05.000000 hyper_sdk-0.1.0/hyper_sdk/incapsula/__init__.py
--rw-rw-rw-   0        0        0     1481 2023-12-24 14:38:17.000000 hyper_sdk-0.1.0/hyper_sdk/incapsula/utmvc.py
--rw-rw-rw-   0        0        0      185 2024-04-07 08:14:08.000000 hyper_sdk-0.1.0/hyper_sdk/incapsula_input.py
--rw-rw-rw-   0        0        0     5436 2024-04-09 13:54:31.000000 hyper_sdk-0.1.0/hyper_sdk/session.py
-drwxrwxrwx   0        0        0        0 2024-04-09 18:06:12.139557 hyper_sdk-0.1.0/hyper_sdk.egg-info/
--rw-rw-rw-   0        0        0     6002 2024-04-09 18:06:12.000000 hyper_sdk-0.1.0/hyper_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-04-09 18:06:12.000000 hyper_sdk-0.1.0/hyper_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 18:06:12.000000 hyper_sdk-0.1.0/hyper_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      117 2024-04-09 18:06:12.000000 hyper_sdk-0.1.0/hyper_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-09 18:06:12.000000 hyper_sdk-0.1.0/hyper_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      755 2024-04-09 13:31:48.000000 hyper_sdk-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 18:06:12.141070 hyper_sdk-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-15 13:33:54.201965 hyper_sdk-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2024-04-07 08:49:14.000000 hyper_sdk-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     5920 2024-04-15 13:33:54.200966 hyper_sdk-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5288 2024-04-15 13:32:58.000000 hyper_sdk-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 13:33:54.190076 hyper_sdk-0.1.1/hyper_sdk/
+-rw-rw-rw-   0        0        0      186 2024-04-09 13:40:00.000000 hyper_sdk-0.1.1/hyper_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 13:33:54.197919 hyper_sdk-0.1.1/hyper_sdk/akamai/
+-rw-rw-rw-   0        0        0      102 2024-04-09 14:00:05.000000 hyper_sdk-0.1.1/hyper_sdk/akamai/__init__.py
+-rw-rw-rw-   0        0        0     2774 2023-12-24 14:34:58.000000 hyper_sdk-0.1.1/hyper_sdk/akamai/pixel.py
+-rw-rw-rw-   0        0        0      929 2023-12-24 14:34:58.000000 hyper_sdk-0.1.1/hyper_sdk/akamai/script_path.py
+-rw-rw-rw-   0        0        0     3715 2024-04-15 13:32:11.000000 hyper_sdk-0.1.1/hyper_sdk/akamai/sec_cpt.py
+-rw-rw-rw-   0        0        0     1898 2023-12-25 13:39:54.000000 hyper_sdk-0.1.1/hyper_sdk/akamai/stop_signal.py
+-rw-rw-rw-   0        0        0      532 2024-04-07 08:09:37.000000 hyper_sdk-0.1.1/hyper_sdk/akamai_input.py
+drwxrwxrwx   0        0        0        0 2024-04-15 13:33:54.199984 hyper_sdk-0.1.1/hyper_sdk/incapsula/
+-rw-rw-rw-   0        0        0       22 2024-04-09 14:00:05.000000 hyper_sdk-0.1.1/hyper_sdk/incapsula/__init__.py
+-rw-rw-rw-   0        0        0     1481 2023-12-24 14:38:17.000000 hyper_sdk-0.1.1/hyper_sdk/incapsula/utmvc.py
+-rw-rw-rw-   0        0        0      185 2024-04-07 08:14:08.000000 hyper_sdk-0.1.1/hyper_sdk/incapsula_input.py
+-rw-rw-rw-   0        0        0     5436 2024-04-09 13:54:31.000000 hyper_sdk-0.1.1/hyper_sdk/session.py
+drwxrwxrwx   0        0        0        0 2024-04-15 13:33:54.200966 hyper_sdk-0.1.1/hyper_sdk.egg-info/
+-rw-rw-rw-   0        0        0     5920 2024-04-15 13:33:54.000000 hyper_sdk-0.1.1/hyper_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-04-15 13:33:54.000000 hyper_sdk-0.1.1/hyper_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 13:33:54.000000 hyper_sdk-0.1.1/hyper_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2024-04-15 13:33:54.000000 hyper_sdk-0.1.1/hyper_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-15 13:33:54.000000 hyper_sdk-0.1.1/hyper_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      755 2024-04-15 13:33:32.000000 hyper_sdk-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 13:33:54.201965 hyper_sdk-0.1.1/setup.cfg
```

### Comparing `hyper_sdk-0.1.0/LICENSE` & `hyper_sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/PKG-INFO` & `hyper_sdk-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hyper Solutions Python SDK
 Project-URL: homepage, https://github.com/Hyper-Solutions/hyper-sdk-py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -80,24 +80,24 @@
 
 ### Handling Sec-Cpt Challenges
 
 The Akamai package provides functions for handling sec-cpt challenges:
 
 - `SecCptChallenge.parse`: Parses a sec-cpt challenge from an HTML source.
 - `generate_sec_cpt_payload`: Generates a sec-cpt payload using the provided sec-cpt cookie.
-- `update_sec_cpt_challenge_data`: Updates the challenge data of a `SecCptChallenge` instance from a response body.
+- `sleep`: Sleeps for the duration specified in the sec-cpt challenge.
 
 Example usage:
 
 ```python
 from hyper_sdk.akamai.sec_cpt import SecCptChallenge
 
 challenge = SecCptChallenge.parse(html_source)
 payload = challenge.generate_sec_cpt_payload(sec_cpt_cookie)
-challenge.update_sec_cpt_challenge_data(response_body)
+challenge.sleep()
 ```
 
 ### Validating Cookies
 
 The Akamai package provides functions for validating cookies:
 
 - `is_cookie_valid`: Determines if the provided `_abck` cookie value is valid based on the given request count.
```

### Comparing `hyper_sdk-0.1.0/README.md` & `hyper_sdk-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -61,24 +61,24 @@
 
 ### Handling Sec-Cpt Challenges
 
 The Akamai package provides functions for handling sec-cpt challenges:
 
 - `SecCptChallenge.parse`: Parses a sec-cpt challenge from an HTML source.
 - `generate_sec_cpt_payload`: Generates a sec-cpt payload using the provided sec-cpt cookie.
-- `update_sec_cpt_challenge_data`: Updates the challenge data of a `SecCptChallenge` instance from a response body.
+- `sleep`: Sleeps for the duration specified in the sec-cpt challenge.
 
 Example usage:
 
 ```python
 from hyper_sdk.akamai.sec_cpt import SecCptChallenge
 
 challenge = SecCptChallenge.parse(html_source)
 payload = challenge.generate_sec_cpt_payload(sec_cpt_cookie)
-challenge.update_sec_cpt_challenge_data(response_body)
+challenge.sleep()
 ```
 
 ### Validating Cookies
 
 The Akamai package provides functions for validating cookies:
 
 - `is_cookie_valid`: Determines if the provided `_abck` cookie value is valid based on the given request count.
```

### Comparing `hyper_sdk-0.1.0/hyper_sdk/akamai/pixel.py` & `hyper_sdk-0.1.1/hyper_sdk/akamai/pixel.py`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/hyper_sdk/akamai/script_path.py` & `hyper_sdk-0.1.1/hyper_sdk/akamai/script_path.py`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/hyper_sdk/akamai/sec_cpt.py` & `hyper_sdk-0.1.1/hyper_sdk/akamai/sec_cpt.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import hashlib
 import json
 import os
 import re
+import time
 from collections import OrderedDict
 from typing import List
 
 sec_duration_expr = re.compile(r'data-duration=(\d+)')
 sec_challenge_expr = re.compile(r'challenge="(.*?)"')
 sec_page_expr = re.compile(r'src="(/_sec/cp_challenge/ak-challenge-\d+-\d+.htm)"')
 
@@ -68,32 +69,28 @@
         if not page_match:
             raise Exception("hyper-sdk: Challenge path not found.")
 
         return page_match.group(1)
 
     def generate_sec_cpt_payload(self, sec_cpt_cookie: str) -> str:
         sec, _, _ = sec_cpt_cookie.partition("~")
+        if sec == sec_cpt_cookie:
+            raise Exception("hyper-sdk: Malformed sec_cpt cookie.")
 
         answers = self._generate_sec_cpt_answers(sec)
 
         payload = OrderedDict([
             ("token", self.challenge_data.token),
             ("answers", answers)
         ])
 
         return json.dumps(payload)
 
-    def update_sec_cpt_challenge_data(self, response_body: str):
-        challenge_data = json.loads(response_body)
-        self.challenge_data = SecCptChallengeData(
-            challenge_data.get('token', ''),
-            challenge_data.get('timestamp', 0),
-            challenge_data.get('nonce', ''),
-            challenge_data.get('difficulty', 0)
-        )
+    def sleep(self):
+        time.sleep(self.duration)
 
     def _generate_sec_cpt_answers(self, sec: str) -> List[str]:
         answers = []
         difficulty = self.challenge_data.difficulty
 
         while True:
             answer = f"0.{os.urandom(8).hex()}"
```

### Comparing `hyper_sdk-0.1.0/hyper_sdk/akamai/stop_signal.py` & `hyper_sdk-0.1.1/hyper_sdk/akamai/stop_signal.py`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/hyper_sdk/akamai_input.py` & `hyper_sdk-0.1.1/hyper_sdk/akamai_input.py`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/hyper_sdk/incapsula/utmvc.py` & `hyper_sdk-0.1.1/hyper_sdk/incapsula/utmvc.py`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/hyper_sdk/session.py` & `hyper_sdk-0.1.1/hyper_sdk/session.py`

 * *Files identical despite different names*

### Comparing `hyper_sdk-0.1.0/hyper_sdk.egg-info/PKG-INFO` & `hyper_sdk-0.1.1/hyper_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: Hyper Solutions Python SDK
 Project-URL: homepage, https://github.com/Hyper-Solutions/hyper-sdk-py
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -80,24 +80,24 @@
 
 ### Handling Sec-Cpt Challenges
 
 The Akamai package provides functions for handling sec-cpt challenges:
 
 - `SecCptChallenge.parse`: Parses a sec-cpt challenge from an HTML source.
 - `generate_sec_cpt_payload`: Generates a sec-cpt payload using the provided sec-cpt cookie.
-- `update_sec_cpt_challenge_data`: Updates the challenge data of a `SecCptChallenge` instance from a response body.
+- `sleep`: Sleeps for the duration specified in the sec-cpt challenge.
 
 Example usage:
 
 ```python
 from hyper_sdk.akamai.sec_cpt import SecCptChallenge
 
 challenge = SecCptChallenge.parse(html_source)
 payload = challenge.generate_sec_cpt_payload(sec_cpt_cookie)
-challenge.update_sec_cpt_challenge_data(response_body)
+challenge.sleep()
 ```
 
 ### Validating Cookies
 
 The Akamai package provides functions for validating cookies:
 
 - `is_cookie_valid`: Determines if the provided `_abck` cookie value is valid based on the given request count.
```

### Comparing `hyper_sdk-0.1.0/pyproject.toml` & `hyper_sdk-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyper_sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = "Hyper Solutions Python SDK"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
```

