# Comparing `tmp/migoapiclient-1.1.4.tar.gz` & `tmp/migoapiclient-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.1.4.tar", last modified: Sat Apr 13 04:27:00 2024, max compression
+gzip compressed data, was "migoapiclient-1.1.5.tar", last modified: Mon Apr 15 03:50:56 2024, max compression
```

## Comparing `migoapiclient-1.1.4.tar` & `migoapiclient-1.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.078589 migoapiclient-1.1.4/
--rw-rw-rw-   0        0        0     3900 2024-04-13 04:27:00.078589 migoapiclient-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.074589 migoapiclient-1.1.4/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.4/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0    11272 2024-04-13 04:25:08.000000 migoapiclient-1.1.4/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.4/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.077588 migoapiclient-1.1.4/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-13 04:26:59.000000 migoapiclient-1.1.4/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-13 04:27:00.000000 migoapiclient-1.1.4/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 04:26:59.000000 migoapiclient-1.1.4/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 04:26:59.000000 migoapiclient-1.1.4/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 04:27:00.078589 migoapiclient-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-13 04:25:39.000000 migoapiclient-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 04:27:00.076588 migoapiclient-1.1.4/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.4/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.081393 migoapiclient-1.1.5/
+-rw-rw-rw-   0        0        0     3900 2024-04-15 03:50:56.079390 migoapiclient-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.073390 migoapiclient-1.1.5/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:53:54.000000 migoapiclient-1.1.5/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0    11651 2024-04-15 03:49:13.000000 migoapiclient-1.1.5/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 08:53:54.000000 migoapiclient-1.1.5/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.078390 migoapiclient-1.1.5/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-15 03:50:55.000000 migoapiclient-1.1.5/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 03:50:56.081393 migoapiclient-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3898 2024-04-15 03:50:53.000000 migoapiclient-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 03:50:56.078390 migoapiclient-1.1.5/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.1.5/src/__init__.py
```

### Comparing `migoapiclient-1.1.4/PKG-INFO` & `migoapiclient-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.4
+Version: 1.1.5
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.4/README.md` & `migoapiclient-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.4/migoapiclient/api_client.py` & `migoapiclient-1.1.5/migoapiclient/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -220,15 +220,15 @@
                     "logParams": json.dumps(log_params),
                     "logStack": log_stack,
                     "logMsg": error_msg
                 }
             ],
             "primaryKey": "id",
             "refreshNow": 0,
-            "tableName": "log_node_spider_error"
+            "tableName": "node_spider_log_error"
         }
         try:
             res_data = self.try_post(self.host + uri, 0, json=post_data)
             return res_data
         except Exception as e:
             msg = ERROR_MSG.format(
                 datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
@@ -265,15 +265,15 @@
                     "logParams": json.dumps(log_params),
                     "logStack": log_stack,
                     "logMsg": msg
                 }
             ],
             "primaryKey": "id",
             "refreshNow": 0,
-            "tableName": "log_node_spider"
+            "tableName": "node_spider_log"
         }
         return self.migo_try_post(self.host + uri, shop_id, '上传日志', 0, json=post_data)
 
     def post_node_es_query(self, column_list: list, table_name: str, es_query: dict):
         """
         根据es语法获取节点信息
         :param column_list 字段名
@@ -291,10 +291,19 @@
     def post_schedule_log(self, msg: str, shop_id: str, definition_info: dict = None):
         """
         上传日志
         :param msg 信息
         :param shop_id 店铺ID
         :param definition_info 策略信息
         """
-        data_type = '调度任务失败'
+        data_type = '更新调度策略'
         return self.post_info_log(msg, data_type, shop_id, definition_info)
 
+    def post_error_schedule_log(self, msg: str, shop_id: str, definition_info: dict = None):
+        """
+        上传错误日志
+        :param msg 信息
+        :param shop_id 店铺ID
+        :param definition_info 策略信息
+        """
+        data_type = '更新调度策略失败'
+        return self.post_error_log(msg, data_type, shop_id, definition_info)
```

### Comparing `migoapiclient-1.1.4/migoapiclient/file_manager.py` & `migoapiclient-1.1.5/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.1.4/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.1.5/migoapiclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.1.4
+Version: 1.1.5
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.1.4/setup.py` & `migoapiclient-1.1.5/setup.py`

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
-VERSION = '1.1.4'
+VERSION = '1.1.5'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

