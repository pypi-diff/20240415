# Comparing `tmp/xcsc_dataapi-1.0.3.tar.gz` & `tmp/xcsc_dataapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsc_dataapi-1.0.3.tar", last modified: Thu Apr 11 01:58:32 2024, max compression
+gzip compressed data, was "xcsc_dataapi-1.0.4.tar", last modified: Mon Apr 15 01:59:04 2024, max compression
```

## Comparing `xcsc_dataapi-1.0.3.tar` & `xcsc_dataapi-1.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.807881 xcsc_dataapi-1.0.3/
--rw-r--r--   0 root         (0) staff       (20)      885 2024-04-11 01:58:32.807586 xcsc_dataapi-1.0.3/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     6217 2024-03-26 07:35:58.000000 xcsc_dataapi-1.0.3/README.md
--rw-r--r--   0 root         (0) staff       (20)       38 2024-04-11 01:58:32.807981 xcsc_dataapi-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1497 2024-03-29 08:07:07.000000 xcsc_dataapi-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.800601 xcsc_dataapi-1.0.3/test/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/test/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      264 2024-04-02 02:28:41.000000 xcsc_dataapi-1.0.3/test/dataapi_test.py
--rw-r--r--   0 root         (0) staff       (20)      171 2024-03-29 09:05:28.000000 xcsc_dataapi-1.0.3/test/token_test.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.802234 xcsc_dataapi-1.0.3/xcsc_dataapi/
--rw-r--r--   0 root         (0) staff       (20)        5 2024-04-11 01:57:29.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/VERSION.txt
--rw-r--r--   0 root         (0) staff       (20)      222 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.806480 xcsc_dataapi-1.0.3/xcsc_dataapi/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1952 2024-04-02 02:28:54.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/data/client.py
--rw-r--r--   0 root         (0) staff       (20)     2889 2024-04-11 01:48:58.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/data/token.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.806867 xcsc_dataapi-1.0.3/xcsc_dataapi/util/
--rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/util/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1229 2024-03-29 05:36:22.000000 xcsc_dataapi-1.0.3/xcsc_dataapi/util/sm4_cbc_util.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-11 01:58:32.807283 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      885 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      453 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       42 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       18 2024-04-11 01:58:32.000000 xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 01:59:04.622517 xcsc_dataapi-1.0.4/
+-rw-r--r--   0 root         (0) staff       (20)      885 2024-04-15 01:59:04.622291 xcsc_dataapi-1.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6217 2024-03-26 07:35:58.000000 xcsc_dataapi-1.0.4/README.md
+-rw-r--r--   0 root         (0) staff       (20)       38 2024-04-15 01:59:04.622556 xcsc_dataapi-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1497 2024-03-29 08:07:07.000000 xcsc_dataapi-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 01:59:04.619843 xcsc_dataapi-1.0.4/test/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.4/test/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      264 2024-04-02 02:28:41.000000 xcsc_dataapi-1.0.4/test/dataapi_test.py
+-rw-r--r--   0 root         (0) staff       (20)      171 2024-03-29 09:05:28.000000 xcsc_dataapi-1.0.4/test/token_test.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 01:59:04.620219 xcsc_dataapi-1.0.4/xcsc_dataapi/
+-rw-r--r--   0 root         (0) staff       (20)        5 2024-04-15 01:58:24.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/VERSION.txt
+-rw-r--r--   0 root         (0) staff       (20)      222 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 01:59:04.621438 xcsc_dataapi-1.0.4/xcsc_dataapi/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1895 2024-04-11 05:44:47.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/data/client.py
+-rw-r--r--   0 root         (0) staff       (20)     2889 2024-04-11 01:48:58.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/data/token.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 01:59:04.621769 xcsc_dataapi-1.0.4/xcsc_dataapi/util/
+-rw-r--r--   0 root         (0) staff       (20)        0 2024-03-29 03:30:43.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/util/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1229 2024-03-29 05:36:22.000000 xcsc_dataapi-1.0.4/xcsc_dataapi/util/sm4_cbc_util.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2024-04-15 01:59:04.622065 xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      885 2024-04-15 01:59:04.000000 xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      453 2024-04-15 01:59:04.000000 xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2024-04-15 01:59:04.000000 xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       42 2024-04-15 01:59:04.000000 xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       18 2024-04-15 01:59:04.000000 xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/top_level.txt
```

### Comparing `xcsc_dataapi-1.0.3/PKG-INFO` & `xcsc_dataapi-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsc_dataapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: xcsc_data data api
 Home-page: https://www.xcsc.com
 Author: Xiangcai Security
 Author-email: itsupport@xcsc.com
 License: MIT
 Keywords: Financial Data
 Classifier: Development Status :: 4 - Beta
```

### Comparing `xcsc_dataapi-1.0.3/README.md` & `xcsc_dataapi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.3/setup.py` & `xcsc_dataapi-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.3/xcsc_dataapi/data/client.py` & `xcsc_dataapi-1.0.4/xcsc_dataapi/data/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,16 +37,15 @@
             current_page = 1
         data_dict["currentPage"] = current_page  # 当前页数，1 代表第一页，2 代表第二页
         data_dict["fieldList"] = fields  # 自定义返回相应参数，不传或者为空默认都是返回全部，传参内容以逗号【,】分割
         api_data = {
             'requestId': time.time_ns(),
             'data': data_dict
         }
-        response = requests.post(self.__http_url + api_url, json=api_data, headers=api_headers, verify=False,
-                                 timeout=self.__timeout)
+        response = requests.post(self.__http_url + api_url, json=api_data, headers=api_headers, verify=False)
         if response.status_code == 200:
             print('api数据查询成功')
         else:
             raise Exception('api数据请求失败,' + response.text)
 
         return response.text
```

### Comparing `xcsc_dataapi-1.0.3/xcsc_dataapi/data/token.py` & `xcsc_dataapi-1.0.4/xcsc_dataapi/data/token.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.3/xcsc_dataapi/util/sm4_cbc_util.py` & `xcsc_dataapi-1.0.4/xcsc_dataapi/util/sm4_cbc_util.py`

 * *Files identical despite different names*

### Comparing `xcsc_dataapi-1.0.3/xcsc_dataapi.egg-info/PKG-INFO` & `xcsc_dataapi-1.0.4/xcsc_dataapi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsc_dataapi
-Version: 1.0.3
+Version: 1.0.4
 Summary: xcsc_data data api
 Home-page: https://www.xcsc.com
 Author: Xiangcai Security
 Author-email: itsupport@xcsc.com
 License: MIT
 Keywords: Financial Data
 Classifier: Development Status :: 4 - Beta
```

