# Comparing `tmp/wawona-1.1.0.tar.gz` & `tmp/wawona-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wawona-1.1.0.tar", last modified: Wed Apr 10 12:10:10 2024, max compression
+gzip compressed data, was "wawona-1.1.1.tar", last modified: Mon Apr 15 12:38:44 2024, max compression
```

## Comparing `wawona-1.1.0.tar` & `wawona-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.335307 wawona-1.1.0/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.1.0/LICENSE
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-10 12:10:10.334512 wawona-1.1.0/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     4048 2024-04-03 23:20:59.000000 wawona-1.1.0/README.md
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-04-10 12:09:00.000000 wawona-1.1.0/pyproject.toml
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-04-10 12:10:10.335673 wawona-1.1.0/setup.cfg
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.326083 wawona-1.1.0/src/
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.329921 wawona-1.1.0/src/wawona/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.1.0/src/wawona/__init__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.1.0/src/wawona/__main__.py
--rw-r--r--   0 jtyuzawa   (501) staff       (20)    19224 2024-04-03 23:29:59.000000 wawona-1.1.0/src/wawona/wawona.py
-drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-10 12:10:10.333827 wawona-1.1.0/src/wawona.egg-info/
--rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/PKG-INFO
--rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/SOURCES.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/dependency_links.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/entry_points.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/requires.txt
--rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-04-10 12:10:10.000000 wawona-1.1.0/src/wawona.egg-info/top_level.txt
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.340938 wawona-1.1.1/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1082 2024-03-20 00:07:08.000000 wawona-1.1.1/LICENSE
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-15 12:38:44.339630 wawona-1.1.1/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     4048 2024-04-03 23:20:59.000000 wawona-1.1.1/README.md
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     1075 2024-04-15 12:38:02.000000 wawona-1.1.1/pyproject.toml
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       38 2024-04-15 12:38:44.341123 wawona-1.1.1/setup.cfg
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.329340 wawona-1.1.1/src/
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.333655 wawona-1.1.1/src/wawona/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       92 2024-03-23 13:31:34.000000 wawona-1.1.1/src/wawona/__init__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       61 2024-03-20 00:07:08.000000 wawona-1.1.1/src/wawona/__main__.py
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)    19567 2024-04-12 12:10:20.000000 wawona-1.1.1/src/wawona/wawona.py
+drwxr-xr-x   0 jtyuzawa   (501) staff       (20)        0 2024-04-15 12:38:44.338262 wawona-1.1.1/src/wawona.egg-info/
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)     5087 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/PKG-INFO
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)      305 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/SOURCES.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        1 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/dependency_links.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       45 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/entry_points.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)       79 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/requires.txt
+-rw-r--r--   0 jtyuzawa   (501) staff       (20)        7 2024-04-15 12:38:44.000000 wawona-1.1.1/src/wawona.egg-info/top_level.txt
```

### Comparing `wawona-1.1.0/LICENSE` & `wawona-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wawona-1.1.0/PKG-INFO` & `wawona-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.1.0
+Version: 1.1.1
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
```

### Comparing `wawona-1.1.0/README.md` & `wawona-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `wawona-1.1.0/pyproject.toml` & `wawona-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wawona"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="yuzawa-san", email="jtyuzawa@gmail.com" },
 ]
 license = {text = "MIT License"}
 description = "Easily make office reservations in sequoia from the command line."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `wawona-1.1.0/src/wawona/wawona.py` & `wawona-1.1.1/src/wawona/wawona.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     pass
 
 
 def api_call(method, url, **kwargs):
     if VERBOSE:
         print("API REQUEST: %s %s %s %s" % (method, url, kwargs.get("headers"), kwargs.get("json")))
     response = requests.request(method, url, **kwargs)
+    response_json = response.json()
+    if response.status_code == 400 and not response_json.get("success"):
+        raise ApiException(response_json.get("message"))
     if response.status_code != 200:
         raise ApiException("%s %s %s %s %s" % (method, url, kwargs.get("headers"), response, response.json()))
     if VERBOSE:
         print("API RESPONSE: %s %s" % (response, response.json()))
     return response
 
 
@@ -78,19 +81,24 @@
     okta_status = user_details["oktaStatus"]
     if okta_status == "MFA_CHALLENGE":
         factors = login_data.get("factors")
         if factors:
             factor = factors[0]
             print(
                 "Using MFA %s %s" % (factor.get("factorType", "unknown"), factor.get("profile", {}).get("phoneNumber")))
-        mfa_code = inquirer.text(message="MFA Code")
-        headers = {"apitoken": token}
-        headers.update(HEADERS)
-        api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login/verify-mfa", headers=headers,
-                 json={"passCode": mfa_code, "browserHash": BROWSER_HASH})
+        while True:
+            mfa_code = inquirer.text(message="MFA Code")
+            headers = {"apitoken": token}
+            headers.update(HEADERS)
+            try:
+                api_call(method='POST', url="https://hrx-backend.sequoia.com/idm/users/login/verify-mfa",
+                         headers=headers, json={"passCode": mfa_code, "browserHash": BROWSER_HASH})
+                break
+            except ApiException as e:
+                print("MFA Verification Failed", e)
     elif okta_status != "SUCCESS":
         # https://developer.okta.com/docs/reference/api/authn/#transaction-state
         raise ApiException("Invalid okta status %s: "
                            "Please authenticate via https://px.sequoia.com/workplace before retrying." % okta_status)
     keyring.set_password(KEYRING_EMAIL, email, password)
     keyring.set_password(KEYRING_TOKEN, email, token)
     return token
```

### Comparing `wawona-1.1.0/src/wawona.egg-info/PKG-INFO` & `wawona-1.1.1/src/wawona.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wawona
-Version: 1.1.0
+Version: 1.1.1
 Summary: Easily make office reservations in sequoia from the command line.
 Author-email: yuzawa-san <jtyuzawa@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/yuzawa-san/wawona
 Project-URL: Changelog, https://github.com/yuzawa-san/wawona/releases
 Project-URL: Issues, https://github.com/yuzawa-san/wawona/issues
 Project-URL: CI, https://github.com/yuzawa-san/wawona/actions
```

