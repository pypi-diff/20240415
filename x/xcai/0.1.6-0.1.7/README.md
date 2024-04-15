# Comparing `tmp/xcai-0.1.6.tar.gz` & `tmp/xcai-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcai-0.1.6.tar", last modified: Tue Apr  9 12:11:30 2024, max compression
+gzip compressed data, was "xcai-0.1.7.tar", last modified: Mon Apr 15 14:42:12 2024, max compression
```

## Comparing `xcai-0.1.6.tar` & `xcai-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-09 12:11:30.569963 xcai-0.1.6/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1091 2024-03-28 06:50:58.000000 xcai-0.1.6/LICENSE
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      654 2024-04-09 12:11:30.569720 xcai-0.1.6/PKG-INFO
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       15 2024-03-28 06:37:32.000000 xcai-0.1.6/README.md
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       91 2024-03-29 05:52:10.000000 xcai-0.1.6/pyproject.toml
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       38 2024-04-09 12:11:30.570028 xcai-0.1.6/setup.cfg
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1680 2024-04-09 12:09:44.000000 xcai-0.1.6/setup.py
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-09 12:11:30.568554 xcai-0.1.6/xcai/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       19 2024-03-29 06:04:42.000000 xcai-0.1.6/xcai/__init__.py
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     5600 2024-04-09 12:11:11.000000 xcai-0.1.6/xcai/xcai.py
-drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-09 12:11:30.569419 xcai-0.1.6/xcai.egg-info/
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      654 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/PKG-INFO
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      210 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/SOURCES.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        1 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/dependency_links.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        9 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/requires.txt
--rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        5 2024-04-09 12:11:30.000000 xcai-0.1.6/xcai.egg-info/top_level.txt
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-15 14:42:12.061608 xcai-0.1.7/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1091 2024-03-28 06:50:58.000000 xcai-0.1.7/LICENSE
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      654 2024-04-15 14:42:12.061395 xcai-0.1.7/PKG-INFO
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       15 2024-03-28 06:37:32.000000 xcai-0.1.7/README.md
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       91 2024-03-29 05:52:10.000000 xcai-0.1.7/pyproject.toml
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       38 2024-04-15 14:42:12.061655 xcai-0.1.7/setup.cfg
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     1680 2024-04-15 14:41:50.000000 xcai-0.1.7/setup.py
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-15 14:42:12.060210 xcai-0.1.7/xcai/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)       19 2024-03-29 06:04:42.000000 xcai-0.1.7/xcai/__init__.py
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)     5732 2024-04-15 14:41:42.000000 xcai-0.1.7/xcai/xcai.py
+drwxr-xr-x   0 xiaochuang.ai   (501) staff       (20)        0 2024-04-15 14:42:12.060980 xcai-0.1.7/xcai.egg-info/
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      654 2024-04-15 14:42:12.000000 xcai-0.1.7/xcai.egg-info/PKG-INFO
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)      210 2024-04-15 14:42:12.000000 xcai-0.1.7/xcai.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        1 2024-04-15 14:42:12.000000 xcai-0.1.7/xcai.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        9 2024-04-15 14:42:12.000000 xcai-0.1.7/xcai.egg-info/requires.txt
+-rw-r--r--   0 xiaochuang.ai   (501) staff       (20)        5 2024-04-15 14:42:12.000000 xcai-0.1.7/xcai.egg-info/top_level.txt
```

### Comparing `xcai-0.1.6/LICENSE` & `xcai-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xcai-0.1.6/PKG-INFO` & `xcai-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcai
-Version: 0.1.6
+Version: 0.1.7
 Summary: We make AI simple for you
 Author: XiaoChuang.ai
 Author-email: sup@XiaoChuangai.com
 License: MIT
 Keywords: ai AI simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xcai-0.1.6/setup.py` & `xcai-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xcai',  # 包名称，在PyPI中必须唯一
-    version='0.1.6',           # 当前包的版本
+    version='0.1.7',           # 当前包的版本
     author='XiaoChuang.ai',        # 作者名字
     author_email='sup@XiaoChuangai.com',  # 作者邮箱
     #maintainer='Maintainer Name',          # 维护者名字，可选
     #maintainer_email='maintainer.email@example.com',  # 维护者邮箱，可选
     #url='https://github.com/yourusername/your_package',  # 项目的URL，通常是代码仓库的地址
     description='We make AI simple for you',  # 简短的项目描述
     long_description=open('README.md').read(),  # 从README文件中读取的长描述
```

### Comparing `xcai-0.1.6/xcai/xcai.py` & `xcai-0.1.7/xcai/xcai.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 class maas:
     def __init__(self, url):
         self.__split_mark = "\r\n" 
         self.url = url
         self.headers = {
             'Content-Type': 'application/json'
             }
-        self.messages = [
-            {"role": "user", "content": "你好"},
-            {"role": "assistant", "content":"你好,有什么可以帮到你"}
-            ]
+        self.messages = self.init_message()
         self.answer = ""
         self.model_choice = ""
         self.content_code = 200
 
+    def init_message(self):
+        m = [{"role": "user", "content": "你好"},
+             {"role": "assistant", "content":"你好,有什么可以帮到你"}]
+        return m
+
     def add_account(self,appid,appkey):
         self.appid=appid
         self.appkey=appkey
         self.update_headers()
 
     def update_headers(self):
         self.headers["appid"] = self.appid
@@ -143,8 +145,11 @@
             return False
         
     def reset_messages(self, history):
         self.messages = []
         for human, assistant in history:
             self.messages.append({"role": "user", "content": human })
             self.messages.append({"role": "assistant", "content":assistant})
+    
+    def clear_messages(self):
+        self.messages = self.init_message()
```

### Comparing `xcai-0.1.6/xcai.egg-info/PKG-INFO` & `xcai-0.1.7/xcai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcai
-Version: 0.1.6
+Version: 0.1.7
 Summary: We make AI simple for you
 Author: XiaoChuang.ai
 Author-email: sup@XiaoChuangai.com
 License: MIT
 Keywords: ai AI simple
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

