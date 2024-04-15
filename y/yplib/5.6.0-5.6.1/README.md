# Comparing `tmp/yplib-5.6.0.tar.gz` & `tmp/yplib-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-5.6.0.tar", last modified: Fri Apr 12 03:56:59 2024, max compression
+gzip compressed data, was "dist\yplib-5.6.1.tar", last modified: Mon Apr 15 04:15:08 2024, max compression
```

## Comparing `yplib-5.6.0.tar` & `yplib-5.6.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 03:56:59.880433 yplib-5.6.0/
--rw-rw-rw-   0        0        0      400 2024-04-12 03:56:59.879437 yplib-5.6.0/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 03:56:59.880433 yplib-5.6.0/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-12 03:56:22.000000 yplib-5.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:56:59.872437 yplib-5.6.0/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.0/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.0/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.0/yplib/chart_html.py
--rw-rw-rw-   0        0        0    10190 2024-04-12 03:50:53.000000 yplib-5.6.0/yplib/db.py
--rw-rw-rw-   0        0        0     5292 2023-07-17 06:31:43.000000 yplib-5.6.0/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.0/yplib/http_util.py
--rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.0/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.0/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.0/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.0/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.0/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-04-12 03:56:59.877433 yplib-5.6.0/yplib.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-12 03:56:59.000000 yplib-5.6.0/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 04:15:08.699082 yplib-5.6.1/
+-rw-rw-rw-   0        0        0      400 2024-04-15 04:15:08.699082 yplib-5.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 04:15:08.700086 yplib-5.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-15 04:14:06.000000 yplib-5.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 04:15:08.694119 yplib-5.6.1/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.1/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.1/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.1/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    10190 2024-04-12 03:50:53.000000 yplib-5.6.1/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.1/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.1/yplib/http_util.py
+-rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.1/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.1/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.1/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.1/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.1/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-04-15 04:15:08.698097 yplib-5.6.1/yplib.egg-info/
+-rw-rw-rw-   0        0        0      400 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-15 04:15:08.000000 yplib-5.6.1/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.6.0/setup.py` & `yplib-5.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.6.0",
+    version="5.6.1",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.6.0/yplib/__init__.py` & `yplib-5.6.1/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/chart.py` & `yplib-5.6.1/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/chart_html.py` & `yplib-5.6.1/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/db.py` & `yplib-5.6.1/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/file.py` & `yplib-5.6.1/yplib/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 from yplib.index import *
 
 
 # 有关文件的操作
 # 查询指定文件夹下面的所有的文件信息, 也可以是指定的文件
-# param list
+# file_path     : 文件路径
+# path_prefix   : 文件路径,以 prefix 开头
+# prefix        : 文件名称,以 prefix 开头
+# path_contain  : 文件路径,含有
+# contain       : 文件名称,含有
+# path_suffix   : 文件路径,以 suffix 结尾
+# suffix        : 文件名称,以 suffix 结尾
 # return list
-def get_file(file_path=None, prefix=None, contain=None, suffix=None):
+def get_file(file_path=None,
+             path_prefix=None,
+             prefix=None,
+             path_contain=None,
+             contain=None,
+             path_suffix=None,
+             suffix=None):
     if file_path is None:
         file_path = os.path.dirname(os.path.abspath('.'))
     list_data = []
-    get_file_all(file_path, list_data, prefix, contain, suffix)
+    get_file_all(file_path, list_data, path_prefix, prefix, path_contain, contain, path_suffix, suffix)
     # 去一下重复的数据
     return list(set(list_data))
 
 
 # 有关文件的操作, 只查询文件夹
 # 查询指定文件夹下面的所有的文件信息, 也可以是指定的文件
 # param list
@@ -51,23 +63,32 @@
                 index += 1
             if one_line.find(find_str) > -1:
                 return one_line
     return None
 
 
 # 查询指定文件夹下面的所有的文件信息, 也可以是指定的文件
-def get_file_all(file_path, list_data, prefix=None, contain=None, suffix=None):
+def get_file_all(file_path,
+                 list_data,
+                 path_prefix=None,
+                 prefix=None,
+                 path_contain=None,
+                 contain=None,
+                 path_suffix=None,
+                 suffix=None):
     if os.path.isdir(file_path):
         for root, dir_names, file_names in os.walk(file_path):
             for file_name in file_names:
-                if get_file_check(file_name, prefix, contain, suffix):
+                if (get_file_check(os.path.join(root, file_name), path_prefix, path_contain, path_suffix)
+                        and get_file_check(file_name, prefix, contain, suffix)):
                     list_data.append(os.path.join(root, file_name))
             for dir_name in dir_names:
-                get_file_all(os.path.join(root, dir_name), list_data)
-    elif get_file_check(file_path, prefix, contain, suffix):
+                get_file_all(os.path.join(root, dir_name), list_data, path_prefix, prefix, path_contain, contain, path_suffix, suffix)
+    elif (get_file_check(file_path, prefix, contain, suffix)
+          and get_file_check(file_path, path_prefix, path_contain, path_suffix)):
         list_data.append(file_path)
 
 
 # 查询指定文件夹下面的所有的文件信息, 也可以是指定的文件
 def get_folder_all(file_path, list_data, prefix=None, contain=None, suffix=None):
     if os.path.isdir(file_path):
         for root, dir_names, file_names in os.walk(file_path):
@@ -79,35 +100,30 @@
                     get_folder_all(dir_name_path, list_data, prefix, contain, suffix)
 
 
 # 检查文件是否符合要求
 # prefix : 前缀
 # contain : 包含这个字符
 # suffix : 后缀
-def get_file_check(file_name='', prefix=None, contain=None, suffix=None):
-    if file_name is None or file_name == '':
+def get_file_check(
+        name=None,
+        prefix=None,
+        contain=None,
+        suffix=None):
+    if name is None or name == '':
         return False
     p = True
     c = True
     s = True
     if prefix is not None:
-        if file_name.startswith(prefix):
-            p = True
-        else:
-            p = False
+        p = name.startswith(prefix)
     if contain is not None:
-        if file_name.find(contain) > -1:
-            c = True
-        else:
-            c = False
+        c = name.find(contain) > -1
     if suffix is not None:
-        if file_name.endswith(suffix):
-            s = True
-        else:
-            s = False
+        s = name.endswith(suffix)
     return p and c and s
 
 
 # 检查文件内容是否包含指定的字符串
 # 慎用,否则, 执行时间可能比较长
 def find_file_by_content(file_path='', contain_txt=None, prefix=None, contain=None, suffix=None):
     list_file = get_file(file_path, prefix, contain, suffix)
@@ -125,16 +141,22 @@
                     if line.endswith('\n'):
                         line = line[0:-1]
                     to_log(one_file, line)
         except Exception as e:
             to_log(one_file, e)
             continue
 
+
 # print(get_file_data_line(r'D:\notepad_file\202306\fasdfsadfaf.txt', 'payout', from_last=False))
 
+# file_all = get_file(r'C:\Users\yang\Desktop\ticket\no.use', path_contain='03')
+#
+# for one_file in file_all:
+#     print(one_file)
+
 # get_file_data_line(r'D:\notepad_file\202306', 'a')
 # get_file_by_content(r'D:\notepad_file\202306', 'a')
 # print(get_file(r'D:\notepad_file\202306', 'a'))
 # print(get_file(r'D:\notepad_file\202306'))
 # print(get_file())
 # print(os.path.abspath('.'))
```

### Comparing `yplib-5.6.0/yplib/http_util.py` & `yplib-5.6.1/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/index.py` & `yplib-5.6.1/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/mail.py` & `yplib-5.6.1/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/mail_html.py` & `yplib-5.6.1/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.0/yplib/markdown.py` & `yplib-5.6.1/yplib/markdown.py`

 * *Files identical despite different names*

