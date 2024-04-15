# Comparing `tmp/scrapy-util-1.0.2.tar.gz` & `tmp/scrapy-util-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapy-util-1.0.2.tar", last modified: Thu Apr 11 07:31:53 2024, max compression
+gzip compressed data, was "dist/scrapy-util-1.0.3.tar", last modified: Mon Apr 15 03:14:31 2024, max compression
```

## Comparing `scrapy-util-1.0.2.tar` & `scrapy-util-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/
--rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/localtime_core_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/show_duration_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/extensions/stats_collector_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/items/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/items/mongo_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/items/trick_item.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/middlewares/dont_request_downloader_middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/pipelines/mongo_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util/spiders/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/list_next_request_spider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/list_spider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/spiders/script_spider.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/scrapy_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5023 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/scrapy_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:31:52.000000 scrapy-util-1.0.2/scrapy_util.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1911 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:31:53.000000 scrapy-util-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 07:31:44.000000 scrapy-util-1.0.2/tests/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       45 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/extensions/localtime_core_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/extensions/show_duration_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/extensions/stats_collector_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util/items/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/items/mongo_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/items/trick_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/middlewares/dont_request_downloader_middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/pipelines/mongo_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/spider_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util/spiders/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/spiders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/spiders/list_next_request_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/spiders/list_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/spiders/script_spider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/scrapy_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-15 03:14:30.000000 scrapy-util-1.0.3/scrapy_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/scrapy_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:14:30.000000 scrapy-util-1.0.3/scrapy_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 03:14:30.000000 scrapy-util-1.0.3/scrapy_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 03:14:30.000000 scrapy-util-1.0.3/scrapy_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:14:30.000000 scrapy-util-1.0.3/scrapy_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1911 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:14:31.000000 scrapy-util-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 03:14:18.000000 scrapy-util-1.0.3/tests/test_hello.py
```

### Comparing `scrapy-util-1.0.2/PKG-INFO` & `scrapy-util-1.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: scrapy-util
-Version: 1.0.2
+Version: 1.0.3
 Summary: scrapy util
 Home-page: https://github.com/mouday/scrapy-util
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Scrapy util
         
         基于scrapy 的一些扩展
         
         pypi: [https://pypi.org/project/scrapy-util](https://pypi.org/project/scrapy-util)
         
         github: [https://github.com/mouday/scrapy-util](https://github.com/mouday/scrapy-util)
         
         
-        ```
-        pip install scrapy-util
+        ```bash
+        pip install six scrapy-util
         ```
         
         ## 启用数据收集功能
         
         此功能配合 [spider-admin-pro](https://github.com/mouday/spider-admin-pro) 使用
         
         ```python
@@ -152,15 +152,34 @@
                 return MongoItem(item)
         
         
         if __name__ == '__main__':
             cmdline.execute('scrapy crawl baidu_mongo'.split())
         
         ```
-        
+         
         如果需要做微调，可以继承`MongoPipeline` 重写函数
         
+        
+        ## 工具方法
+        
+        运行爬虫工具方法
+        
+        ```python
+        import scrapy
+        from scrapy_util import spider_util
+        
+        class BaiduSpider(scrapy.Spider):
+            name = 'baidu_spider'
+        
+        
+        if __name__ == '__main__':
+            # cmdline.execute('scrapy crawl baidu_spider'.split()
+            spider_util.run_spider(BaiduSpider)
+        ```
+        
+        
 Keywords: spider,admin
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrapy-util-1.0.2/README.md` & `scrapy-util-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 基于scrapy 的一些扩展
 
 pypi: [https://pypi.org/project/scrapy-util](https://pypi.org/project/scrapy-util)
 
 github: [https://github.com/mouday/scrapy-util](https://github.com/mouday/scrapy-util)
 
 
-```
-pip install scrapy-util
+```bash
+pip install six scrapy-util
 ```
 
 ## 启用数据收集功能
 
 此功能配合 [spider-admin-pro](https://github.com/mouday/spider-admin-pro) 使用
 
 ```python
@@ -144,9 +144,28 @@
         return MongoItem(item)
 
 
 if __name__ == '__main__':
     cmdline.execute('scrapy crawl baidu_mongo'.split())
 
 ```
-
+ 
 如果需要做微调，可以继承`MongoPipeline` 重写函数
+
+
+## 工具方法
+
+运行爬虫工具方法
+
+```python
+import scrapy
+from scrapy_util import spider_util
+
+class BaiduSpider(scrapy.Spider):
+    name = 'baidu_spider'
+
+
+if __name__ == '__main__':
+    # cmdline.execute('scrapy crawl baidu_spider'.split()
+    spider_util.run_spider(BaiduSpider)
+```
+
```

### Comparing `scrapy-util-1.0.2/scrapy_util/extensions/show_duration_extension.py` & `scrapy-util-1.0.3/scrapy_util/extensions/show_duration_extension.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/extensions/stats_collector_extension.py` & `scrapy-util-1.0.3/scrapy_util/extensions/stats_collector_extension.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/middlewares/dont_request_downloader_middleware.py` & `scrapy-util-1.0.3/scrapy_util/middlewares/dont_request_downloader_middleware.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/pipelines/mongo_pipeline.py` & `scrapy-util-1.0.3/scrapy_util/pipelines/mongo_pipeline.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/spiders/list_next_request_spider.py` & `scrapy-util-1.0.3/scrapy_util/spiders/list_next_request_spider.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/spiders/list_spider.py` & `scrapy-util-1.0.3/scrapy_util/spiders/list_spider.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/spiders/script_spider.py` & `scrapy-util-1.0.3/scrapy_util/spiders/script_spider.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util/utils.py` & `scrapy-util-1.0.3/scrapy_util/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy-util-1.0.2/scrapy_util.egg-info/PKG-INFO` & `scrapy-util-1.0.3/scrapy_util.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: scrapy-util
-Version: 1.0.2
+Version: 1.0.3
 Summary: scrapy util
 Home-page: https://github.com/mouday/scrapy-util
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Scrapy util
         
         基于scrapy 的一些扩展
         
         pypi: [https://pypi.org/project/scrapy-util](https://pypi.org/project/scrapy-util)
         
         github: [https://github.com/mouday/scrapy-util](https://github.com/mouday/scrapy-util)
         
         
-        ```
-        pip install scrapy-util
+        ```bash
+        pip install six scrapy-util
         ```
         
         ## 启用数据收集功能
         
         此功能配合 [spider-admin-pro](https://github.com/mouday/spider-admin-pro) 使用
         
         ```python
@@ -152,15 +152,34 @@
                 return MongoItem(item)
         
         
         if __name__ == '__main__':
             cmdline.execute('scrapy crawl baidu_mongo'.split())
         
         ```
-        
+         
         如果需要做微调，可以继承`MongoPipeline` 重写函数
         
+        
+        ## 工具方法
+        
+        运行爬虫工具方法
+        
+        ```python
+        import scrapy
+        from scrapy_util import spider_util
+        
+        class BaiduSpider(scrapy.Spider):
+            name = 'baidu_spider'
+        
+        
+        if __name__ == '__main__':
+            # cmdline.execute('scrapy crawl baidu_spider'.split()
+            spider_util.run_spider(BaiduSpider)
+        ```
+        
+        
 Keywords: spider,admin
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
```

### Comparing `scrapy-util-1.0.2/scrapy_util.egg-info/SOURCES.txt` & `scrapy-util-1.0.3/scrapy_util.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 scrapy_util/__init__.py
 scrapy_util/logger.py
+scrapy_util/spider_util.py
 scrapy_util/utils.py
 scrapy_util/version.py
 scrapy_util.egg-info/PKG-INFO
 scrapy_util.egg-info/SOURCES.txt
 scrapy_util.egg-info/dependency_links.txt
 scrapy_util.egg-info/requires.txt
 scrapy_util.egg-info/top_level.txt
```

### Comparing `scrapy-util-1.0.2/setup.py` & `scrapy-util-1.0.3/setup.py`

 * *Files identical despite different names*

