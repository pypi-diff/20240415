# Comparing `tmp/migoapiclient-1.1.5.tar.gz` & `tmp/migoapiclient-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.1.5.tar", last modified: Mon Apr 15 03:50:56 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.6.tar", last modified: Mon Apr 15 08:49:50 2024, max compression
```

## Comparing `migoapiclient-1.1.5.tar` & `migoapiclient-1.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.081393 migoapiclient-1.1.5/
--rw-rw-rw-   0        0        0     3900 2024-04-15 03:50:56.079390 migoapiclient-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.073390 migoapiclient-1.1.5/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.5/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    11651 2024-04-15 03:49:13.000000 migoapiclient-1.1.5/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.5/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.078390 migoapiclient-1.1.5/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 03:50:56.081393 migoapiclient-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-15 03:50:53.000000 migoapiclient-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.078390 migoapiclient-1.1.5/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.5/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:49:50.566955 migoapiclient-1.1.6/
+-rw-rw-rw-   0        0        0     3900 2024-04-15 08:49:50.565956 migoapiclient-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 08:49:50.562955 migoapiclient-1.1.6/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.6/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    12135 2024-04-15 08:48:47.000000 migoapiclient-1.1.6/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.6/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:49:50.565956 migoapiclient-1.1.6/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-15 08:49:50.000000 migoapiclient-1.1.6/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-15 08:49:50.000000 migoapiclient-1.1.6/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 08:49:50.000000 migoapiclient-1.1.6/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 08:49:50.000000 migoapiclient-1.1.6/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 08:49:50.566955 migoapiclient-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-15 08:48:47.000000 migoapiclient-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 08:49:50.564957 migoapiclient-1.1.6/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.6/src/__init__.py
```

### Comparing `migoapiclient-1.1.5/PKG-INFO` & `migoapiclient-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.5
+Version: 1.1.6
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.5/README.md` & `migoapiclient-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.5/migoapiclient/api_client.py` & `migoapiclient-1.1.6/migoapiclient/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from dateutil.tz import tz
 from requests import Response
 
 from .file_manager import LogFileManager
 import time
 import requests
 
+TZ_NAME = 'Asia/Shanghai'
 ERROR_MSG = """
 ---------------------------------- {0} begin ----------------------------------
 请求URL是：{1}
 请求headers是：{2}
 请求params是：{3}
 请求post是：{4}
 错误信息是：{5}
@@ -50,15 +51,15 @@
                 res_data = self.get(url, timeout=self.timeout, **kwargs)
                 return self.res_callback(res_data)
             except Exception as e:
                 print(e)
                 time.sleep(error_count)
                 error_count += 1
                 return self.try_get(url, error_count, **kwargs)
-        raise Exception('已经尝试请求：{}次，服务器依然没有响应'.format(self.retry_count))
+        raise Exception('已经尝试请求：{}次，服务器依然没有响应，错误信息是：{}'.format(self.retry_count, str(e)))
 
     def try_post(self, url: str, error_count: int = 0, **kwargs):
         """
         尝试重发post请求
         """
         while error_count <= self.retry_count:
             try:
@@ -66,15 +67,23 @@
                 return self.res_callback(res_data)
             except Exception as e:
                 print(e)
                 time.sleep(error_count)
                 error_count += 1
                 time.sleep(error_count)
                 return self.try_post(url, error_count, **kwargs)
-        raise Exception('已经尝试请求：{}次，服务器依然没有响应'.format(self.retry_count))
+        raise Exception('已经尝试请求：{}次，服务器依然没有响应，错误信息是：{}'.format(self.retry_count, str(e)))
+
+    @staticmethod
+    def get_log_time():
+        """
+        生成日志时间
+        """
+        now_datetime_obj = datetime.fromtimestamp(int(time.time()), tz.gettz(TZ_NAME))
+        return str(now_datetime_obj).replace(' ', 'T', 1)
 
 
 class MigoApiClient(ApiClient):
     def __init__(self, node_id: str, retry_count: int, timeout: int, host: str, auth_key: str, log_path: str):
         """
         初始化米果API客户端
         :param node_id 节点ID
@@ -207,19 +216,19 @@
         :param log_params 请求的get参数
         :param log_stack 日志其他信息
         """
         uri = '/data-collection-service/node/logsave'
         post_data = {
             "data": [
                 {
-                    "id": str(time.time()).replace('.', ''),
+                    "id": str(time.time()).replace('.', ''),  # 日志数据能容忍缺失，所以暂时用时间戳作为ID
                     "shopId": shop_id,
                     "nodeId": self.node_id,
                     "dataType": data_type,
-                    "logTime": str(datetime.fromtimestamp(int(time.time()), tz.gettz('Asia/Shanghai'))),
+                    "logTime": self.get_log_time(),
                     "logData": json.dumps(log_data),
                     "logParams": json.dumps(log_params),
                     "logStack": log_stack,
                     "logMsg": error_msg
                 }
             ],
             "primaryKey": "id",
@@ -227,15 +236,15 @@
             "tableName": "node_spider_log_error"
         }
         try:
             res_data = self.try_post(self.host + uri, 0, json=post_data)
             return res_data
         except Exception as e:
             msg = ERROR_MSG.format(
-                datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+                self.get_log_time(),
                 self.host + uri,
                 self.headers,
                 '',
                 post_data,
                 str(e),
             )
             self.log_manager.write_request_error_log(msg)
@@ -252,19 +261,19 @@
         :param log_params 请求的get参数
         :param log_stack 日志其他信息
         """
         uri = '/data-collection-service/node/logsave'
         post_data = {
             "data": [
                 {
-                    "id": str(time.time()).replace('.', ''),
+                    "id": str(time.time()).replace('.', ''),  # 日志数据能容忍缺失，所以暂时用时间戳作为ID
                     "shopId": shop_id,
                     "nodeId": self.node_id,
                     "dataType": data_type,
-                    "logTime": str(datetime.fromtimestamp(int(time.time()), tz.gettz('Asia/Shanghai'))),
+                    "logTime": self.get_log_time(),
                     "logData": json.dumps(log_data),
                     "logParams": json.dumps(log_params),
                     "logStack": log_stack,
                     "logMsg": msg
                 }
             ],
             "primaryKey": "id",
@@ -284,26 +293,28 @@
         post_data = {
             'sourceStrings': column_list,
             'queryString': json.dumps(es_query),
             'indexName': table_name
         }
         return self.migo_try_post(self.host + uri, 0, '获取节点信息', 0, json=post_data)
 
-    def post_schedule_log(self, msg: str, shop_id: str, definition_info: dict = None):
+    def post_schedule_log(self, msg: str, shop_id: str, definition_info: dict, log_params: dict = None):
         """
         上传日志
         :param msg 信息
         :param shop_id 店铺ID
         :param definition_info 策略信息
+        :param log_params 其他信息
         """
         data_type = '更新调度策略'
-        return self.post_info_log(msg, data_type, shop_id, definition_info)
+        return self.post_info_log(msg, data_type, shop_id, definition_info, log_params)
 
-    def post_error_schedule_log(self, msg: str, shop_id: str, definition_info: dict = None):
+    def post_error_schedule_log(self, msg: str, shop_id: str, definition_info: dict = None, log_params: dict = None):
         """
         上传错误日志
         :param msg 信息
         :param shop_id 店铺ID
         :param definition_info 策略信息
+        :param log_params 其他信息
         """
         data_type = '更新调度策略失败'
-        return self.post_error_log(msg, data_type, shop_id, definition_info)
+        return self.post_error_log(msg, data_type, shop_id, definition_info, log_params)
```

### Comparing `migoapiclient-1.1.5/migoapiclient/file_manager.py` & `migoapiclient-1.1.6/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.5/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.6/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.5
+Version: 1.1.6
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.5/setup.py` & `migoapiclient-1.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.1.5'
+VERSION = '1.1.6'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

