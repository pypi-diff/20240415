# Comparing `tmp/eirStru-0.2.92.tar.gz` & `tmp/eirStru-0.2.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eirStru-0.2.92.tar", last modified: Sun Apr 14 20:18:37 2024, max compression
+gzip compressed data, was "eirStru-0.2.93.tar", last modified: Sun Apr 14 22:54:24 2024, max compression
```

## Comparing `eirStru-0.2.92.tar` & `eirStru-0.2.93.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 20:18:37.853994 eirStru-0.2.92/
--rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.92/LICENSE
--rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.92/MANIFEST.in
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-14 20:18:37.853716 eirStru-0.2.92/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.92/README.md
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 20:18:37.852779 eirStru-0.2.92/eirStru/
--rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.92/eirStru/__init__.py
--rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.92/eirStru/__version__.py
--rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.92/eirStru/aiomysql_helper.py
--rwxr--r--   0 wangwh     (501) staff       (20)    17687 2024-04-14 20:18:24.000000 eirStru-0.2.92/eirStru/common.py
--rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.92/eirStru/eirjob_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     5271 2024-03-14 03:14:41.000000 eirStru-0.2.92/eirStru/eirlogin_intf.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.92/eirStru/redis_utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.92/eirStru/test.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.92/eirStru/utils.py
--rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.92/eirStru/wx_push.py
-drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 20:18:37.853466 eirStru-0.2.92/eirStru.egg-info/
--rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-14 20:18:37.000000 eirStru-0.2.92/eirStru.egg-info/PKG-INFO
--rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-14 20:18:37.000000 eirStru-0.2.92/eirStru.egg-info/SOURCES.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-14 20:18:37.000000 eirStru-0.2.92/eirStru.egg-info/dependency_links.txt
--rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-14 20:18:37.000000 eirStru-0.2.92/eirStru.egg-info/top_level.txt
--rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-14 20:18:37.854077 eirStru-0.2.92/setup.cfg
--rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-14 20:18:36.000000 eirStru-0.2.92/setup.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 22:54:24.469102 eirStru-0.2.93/
+-rw-r--r--   0 wangwh     (501) staff       (20)     1060 2024-01-25 06:27:18.000000 eirStru-0.2.93/LICENSE
+-rw-r--r--   0 wangwh     (501) staff       (20)       26 2024-01-25 06:27:18.000000 eirStru-0.2.93/MANIFEST.in
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-14 22:54:24.468809 eirStru-0.2.93/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)     2338 2024-01-25 06:27:18.000000 eirStru-0.2.93/README.md
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 22:54:24.467881 eirStru-0.2.93/eirStru/
+-rw-r--r--   0 wangwh     (501) staff       (20)       43 2024-03-14 03:14:41.000000 eirStru-0.2.93/eirStru/__init__.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      352 2024-01-25 06:27:18.000000 eirStru-0.2.93/eirStru/__version__.py
+-rwxr--r--   0 wangwh     (501) staff       (20)     5220 2024-03-14 03:14:41.000000 eirStru-0.2.93/eirStru/aiomysql_helper.py
+-rwxr--r--   0 wangwh     (501) staff       (20)    17673 2024-04-14 22:54:05.000000 eirStru-0.2.93/eirStru/common.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     3584 2024-02-29 12:42:57.000000 eirStru-0.2.93/eirStru/eirjob_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     5271 2024-03-14 03:14:41.000000 eirStru-0.2.93/eirStru/eirlogin_intf.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1190 2024-02-29 02:15:20.000000 eirStru-0.2.93/eirStru/redis_utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)      421 2024-03-15 21:24:26.000000 eirStru-0.2.93/eirStru/test.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1428 2024-03-14 03:14:41.000000 eirStru-0.2.93/eirStru/utils.py
+-rw-r--r--   0 wangwh     (501) staff       (20)     1670 2024-03-15 21:25:26.000000 eirStru-0.2.93/eirStru/wx_push.py
+drwxr-xr-x   0 wangwh     (501) staff       (20)        0 2024-04-14 22:54:24.468601 eirStru-0.2.93/eirStru.egg-info/
+-rw-r--r--   0 wangwh     (501) staff       (20)     2964 2024-04-14 22:54:24.000000 eirStru-0.2.93/eirStru.egg-info/PKG-INFO
+-rw-r--r--   0 wangwh     (501) staff       (20)      373 2024-04-14 22:54:24.000000 eirStru-0.2.93/eirStru.egg-info/SOURCES.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        1 2024-04-14 22:54:24.000000 eirStru-0.2.93/eirStru.egg-info/dependency_links.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)        8 2024-04-14 22:54:24.000000 eirStru-0.2.93/eirStru.egg-info/top_level.txt
+-rw-r--r--   0 wangwh     (501) staff       (20)       38 2024-04-14 22:54:24.469152 eirStru-0.2.93/setup.cfg
+-rw-r--r--   0 wangwh     (501) staff       (20)     3777 2024-04-14 22:54:23.000000 eirStru-0.2.93/setup.py
```

### Comparing `eirStru-0.2.92/LICENSE` & `eirStru-0.2.93/LICENSE`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/PKG-INFO` & `eirStru-0.2.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.92
+Version: 0.2.93
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.92/README.md` & `eirStru-0.2.93/README.md`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru/aiomysql_helper.py` & `eirStru-0.2.93/eirStru/aiomysql_helper.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru/common.py` & `eirStru-0.2.93/eirStru/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
 
     @property
     def need_apply(self):
         """
         判断本单是否需要申请
         @return:
         """
-        return self.ctns and self.ctns_for_apply()
+        return self.ctns_for_apply()
         # if self.ctntypedigit_list:
         #     for item in self.ctntypedigit_list:
         #         if item.ctn_digit_for_apply > 0:
         #             return True
         #     return False
         # else:
         #     return bool(list(filter(lambda x: not x.is_applied, self.ctns)))
```

### Comparing `eirStru-0.2.92/eirStru/eirjob_intf.py` & `eirStru-0.2.93/eirStru/eirjob_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru/eirlogin_intf.py` & `eirStru-0.2.93/eirStru/eirlogin_intf.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru/redis_utils.py` & `eirStru-0.2.93/eirStru/redis_utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru/utils.py` & `eirStru-0.2.93/eirStru/utils.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru/wx_push.py` & `eirStru-0.2.93/eirStru/wx_push.py`

 * *Files identical despite different names*

### Comparing `eirStru-0.2.92/eirStru.egg-info/PKG-INFO` & `eirStru-0.2.93/eirStru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eirStru
-Version: 0.2.92
+Version: 0.2.93
 Summary: My short description for my project.
 Home-page: https://github.com/me/myproject
 Author: Awesome Soul
 Author-email: me@example.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `eirStru-0.2.92/setup.py` & `eirStru-0.2.93/setup.py`

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
-VERSION = '0.2.92'
+VERSION = '0.2.93'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

