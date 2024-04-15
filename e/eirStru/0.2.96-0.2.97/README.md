# Comparing `tmp/eirStru-0.2.96.tar.gz` & `tmp/eirStru-0.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.2.96.tar", last modified: Mon Apr 15 08:48:09 2024, max compression
+gzip compressed data, was "eirStru-0.2.97.tar", last modified: Mon Apr 15 09:02:16 2024, max compression
```

## Comparing `eirStru-0.2.96.tar` & `eirStru-0.2.97.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 08:48:09.053787 eirStru-0.2.96/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.96/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.96/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 08:48:09.053537 eirStru-0.2.96/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.96/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 08:48:09.052634 eirStru-0.2.96/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.96/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.96/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.96/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    17775 2024-04-15 08:35:42.000000 eirStru-0.2.96/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.96/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     5936 2024-04-15 08:37:49.000000 eirStru-0.2.96/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.96/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.96/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.96/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.96/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 08:48:09.053291 eirStru-0.2.96/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 08:48:09.000000 eirStru-0.2.96/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 08:48:09.000000 eirStru-0.2.96/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 08:48:09.000000 eirStru-0.2.96/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 08:48:09.000000 eirStru-0.2.96/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 08:48:09.053840 eirStru-0.2.96/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 08:48:07.000000 eirStru-0.2.96/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:02:16.108662 eirStru-0.2.97/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.97/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.97/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:02:16.108402 eirStru-0.2.97/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.97/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:02:16.107299 eirStru-0.2.97/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.97/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.97/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.97/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    18022 2024-04-15 09:02:03.000000 eirStru-0.2.97/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.97/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     5936 2024-04-15 08:37:49.000000 eirStru-0.2.97/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.97/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.97/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.97/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.97/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-15 09:02:16.108163 eirStru-0.2.97/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-15 09:02:16.000000 eirStru-0.2.97/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-15 09:02:16.000000 eirStru-0.2.97/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-15 09:02:16.000000 eirStru-0.2.97/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-15 09:02:16.000000 eirStru-0.2.97/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-15 09:02:16.108719 eirStru-0.2.97/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-15 09:02:15.000000 eirStru-0.2.97/setup.py
```

### Comparing `eirStru-0.2.96/LICENSE` & `eirStru-0.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/PKG-INFO` & `eirStru-0.2.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.96
+Version: 0.2.97
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.96/README.md` & `eirStru-0.2.97/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru/aiomysql_helper.py` & `eirStru-0.2.97/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru/common.py` & `eirStru-0.2.97/eirStru/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -498,7 +498,17 @@
 
 
 class LoginParams(BaseModel):
     carrier_id: str = ''  # 船公司
     account: str = ''  # 账号
     password: str = ''  # 密码
     proxy_id: Optional[str] = None
+
+
+class RespException(Exception):
+    def __init__(self, code, msg, detail=None):
+        self.code = code
+        self.msg = msg
+        self.detail = detail
+
+    def __str__(self):
+        return f'\n{str(self.code)}\n{self.detail or self.msg}'
```

### Comparing `eirStru-0.2.96/eirStru/eirjob_intf.py` & `eirStru-0.2.97/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru/eirlogin_intf.py` & `eirStru-0.2.97/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru/redis_utils.py` & `eirStru-0.2.97/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru/utils.py` & `eirStru-0.2.97/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru/wx_push.py` & `eirStru-0.2.97/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.96/eirStru.egg-info/PKG-INFO` & `eirStru-0.2.97/eirStru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.96
+Version: 0.2.97
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.96/setup.py` & `eirStru-0.2.97/setup.py`

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
-VERSION = '0.2.96'
+VERSION = '0.2.97'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

