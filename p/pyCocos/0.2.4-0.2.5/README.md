# Comparing `tmp/pycocos-0.2.4.tar.gz` & `tmp/pycocos-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycocos-0.2.4.tar", last modified: Mon Apr 15 00:10:11 2024, max compression
+gzip compressed data, was "pycocos-0.2.5.tar", last modified: Mon Apr 15 01:11:14 2024, max compression
```

## Comparing `pycocos-0.2.4.tar` & `pycocos-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 00:10:07.000000 pycocos-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-15 00:10:11.684365 pycocos-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-15 00:10:07.000000 pycocos-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 00:10:11.684365 pycocos-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 00:10:07.000000 pycocos-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.680365 pycocos-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/src/pyCocos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 00:10:11.000000 pycocos-0.2.4/src/pyCocos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/src/pycocos/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 00:10:11.684365 pycocos-0.2.4/src/pycocos/components/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/components/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    52337 2024-04-15 00:10:07.000000 pycocos-0.2.4/src/pycocos/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:14.653402 pycocos-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-15 01:11:11.000000 pycocos-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-15 01:11:14.653402 pycocos-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-15 01:11:11.000000 pycocos-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 01:11:14.653402 pycocos-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-15 01:11:11.000000 pycocos-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:14.649402 pycocos-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:14.653402 pycocos-0.2.5/src/pyCocos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-15 01:11:14.000000 pycocos-0.2.5/src/pyCocos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-15 01:11:14.000000 pycocos-0.2.5/src/pyCocos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 01:11:14.000000 pycocos-0.2.5/src/pyCocos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 01:11:14.000000 pycocos-0.2.5/src/pyCocos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 01:11:14.000000 pycocos-0.2.5/src/pyCocos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:14.649402 pycocos-0.2.5/src/pycocos/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 01:11:14.653402 pycocos-0.2.5/src/pycocos/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15817 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/components/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/components/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/components/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/components/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52554 2024-04-15 01:11:11.000000 pycocos-0.2.5/src/pycocos/main.py
```

### Comparing `pycocos-0.2.4/LICENSE` & `pycocos-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.4/PKG-INFO` & `pycocos-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycocos-0.2.4/README.md` & `pycocos-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.4/setup.py` & `pycocos-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyCocos",
-    version="0.2.4",
+    version="0.2.5",
     author="Nacho Herrera",
     author_email="github@nachoherrera.com.ar",
     description="Python connector for Cocos Capital's Rest APIs.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nacho-herrera/pyCocos",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `pycocos-0.2.4/src/pyCocos.egg-info/PKG-INFO` & `pycocos-0.2.5/src/pyCocos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyCocos
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python connector for Cocos Capital's Rest APIs.
 Home-page: https://github.com/nacho-herrera/pyCocos
 Author: Nacho Herrera
 Author-email: github@nachoherrera.com.ar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pycocos-0.2.4/src/pycocos/components/client.py` & `pycocos-0.2.5/src/pycocos/components/client.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.4/src/pycocos/components/enums.py` & `pycocos-0.2.5/src/pycocos/components/enums.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.4/src/pycocos/components/urls.py` & `pycocos-0.2.5/src/pycocos/components/urls.py`

 * *Files identical despite different names*

### Comparing `pycocos-0.2.4/src/pycocos/main.py` & `pycocos-0.2.5/src/pycocos/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,19 @@
         headers_update: dict[str, str] = {
             "apikey": self.api_key,
             "authorization": f"Bearer {self.access_token}",
         }
         
         self.client.update_session_headers(headers_update)
         second_factor_response = self.client.get_2factors()
-        if "requireChallenge" in second_factor_response.keys() and second_factor_response["requireChallenge"]:
+        #if "requireChallenge" in second_factor_response.keys() and second_factor_response["requireChallenge"]:
+        if "id" in second_factor_response.keys():
             challenge_id = second_factor_response["id"]
+        else:
+            raise Exception("Error: 2FA challenge not found in the API response, please share the broswer response on GitHub so i can implement this.")
         
         payload = json.dumps({
             "expires_at": 123, 
             "id": challenge_id,
         })
 
         challenge = self.client.submit_challenge_request(challenge_id=challenge_id)
```

