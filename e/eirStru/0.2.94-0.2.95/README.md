# Comparing `tmp/eirStru-0.2.94.tar.gz` & `tmp/eirStru-0.2.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.2.94.tar", last modified: Mon Apr 15 07:34:03 2024, max compression
+gzip compressed data, was "eirStru-0.2.95.tar", last modified: Mon Apr 15 08:36:09 2024, max compression
```

## Comparing `eirStru-0.2.94.tar` & `eirStru-0.2.95.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 07:34:03.841995 eirStru-0.2.94/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.94/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.94/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 07:34:03.841716 eirStru-0.2.94/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.94/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 07:34:03.841024 eirStru-0.2.94/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.94/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.94/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.94/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    17605 2024-04-15 07:33:47.000000 eirStru-0.2.94/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.94/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     5271 2024-03-14 03:14:41.000000 eirStru-0.2.94/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.94/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.94/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.94/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.94/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 07:34:03.841518 eirStru-0.2.94/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 07:34:03.000000 eirStru-0.2.94/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 07:34:03.000000 eirStru-0.2.94/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 07:34:03.000000 eirStru-0.2.94/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 07:34:03.000000 eirStru-0.2.94/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 07:34:03.842045 eirStru-0.2.94/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 07:33:55.000000 eirStru-0.2.94/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 08:36:09.214943 eirStru-0.2.95/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.95/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.95/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 08:36:09.214684 eirStru-0.2.95/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.95/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 08:36:09.213536 eirStru-0.2.95/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.95/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.95/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.95/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    17775 2024-04-15 08:35:42.000000 eirStru-0.2.95/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.95/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     5927 2024-04-15 08:35:42.000000 eirStru-0.2.95/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.95/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.95/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.95/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.95/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 08:36:09.214415 eirStru-0.2.95/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 08:36:09.000000 eirStru-0.2.95/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 08:36:09.000000 eirStru-0.2.95/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 08:36:09.000000 eirStru-0.2.95/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 08:36:09.000000 eirStru-0.2.95/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 08:36:09.214998 eirStru-0.2.95/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 08:36:07.000000 eirStru-0.2.95/setup.py
```

### Comparing `eirStru-0.2.94/LICENSE` & `eirStru-0.2.95/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/PKG-INFO` & `eirStru-0.2.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.94
+Version: 0.2.95
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.94/README.md` & `eirStru-0.2.95/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/eirStru/aiomysql_helper.py` & `eirStru-0.2.95/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/eirStru/common.py` & `eirStru-0.2.95/eirStru/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,7 +491,14 @@
     session_guid: Optional[str] = None
 
 
 class ParamsCheckAccount(BaseModel):
     carrier_id: str = ''  # 船公司
     account: str = ''  # 账号
     password: str = ''  # 密码
+
+
+class LoginParams(BaseModel):
+    carrier_id: str = ''  # 船公司
+    account: str = ''  # 账号
+    password: str = ''  # 密码
+    proxy_id: Optional[str] = None
```

### Comparing `eirStru-0.2.94/eirStru/eirjob_intf.py` & `eirStru-0.2.95/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/eirStru/eirlogin_intf.py` & `eirStru-0.2.95/eirStru/eirlogin_intf.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,34 @@
             async with ClientSession() as cs:
                 async with cs.post(url, headers=headers, data=data, verify_ssl=False) as resp:
                     r_json = await resp.json()
                     return ResponseData(**r_json)
         except Exception as e:
             return ResponseData(code=RespType.task_failed, message=f'{e}')
 
+    async def login(self, params: Pa) -> ResponseData:
+        """
+        检查账号
+        """
+        url = f'{self.host}/login/'
+        headers = {
+            'accept': 'application/json',
+            'Content-Type': 'application/json',
+        }
+
+        data = params.model_dump_json()
+
+        try:
+            async with ClientSession() as cs:
+                async with cs.post(url, headers=headers, data=data, verify_ssl=False) as resp:
+                    r_json = await resp.json()
+                    return ResponseData(**r_json)
+        except Exception as e:
+            return ResponseData(code=RespType.task_failed, message=f'{e}')
+
     async def get_session(self, carrier_id, action: ActionType, account: str = None, bookingagent_id: str = None,
                           sub_code: str = None) -> ResponseData:
         url = f'{self.host}/get_session/'
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
         }
```

### Comparing `eirStru-0.2.94/eirStru/redis_utils.py` & `eirStru-0.2.95/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/eirStru/utils.py` & `eirStru-0.2.95/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/eirStru/wx_push.py` & `eirStru-0.2.95/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.94/eirStru.egg-info/PKG-INFO` & `eirStru-0.2.95/eirStru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.94
+Version: 0.2.95
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.94/setup.py` & `eirStru-0.2.95/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'eirStru'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'me@example.com'
 AUTHOR = 'Awesome Soul'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.94'
+VERSION = '0.2.95'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

