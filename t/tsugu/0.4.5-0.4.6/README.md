# Comparing `tmp/tsugu-0.4.5.tar.gz` & `tmp/tsugu-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.5.tar", last modified: Mon Apr 15 02:40:21 2024, max compression
+gzip compressed data, was "tsugu-0.4.6.tar", last modified: Mon Apr 15 03:05:22 2024, max compression
```

## Comparing `tsugu-0.4.5.tar` & `tsugu-0.4.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.301198 tsugu-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:40:11.000000 tsugu-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:40:21.301198 tsugu-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:40:11.000000 tsugu-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:40:21.301198 tsugu-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:40:11.000000 tsugu-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.297198 tsugu-0.4.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:40:11.000000 tsugu-0.4.5/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.297198 tsugu-0.4.5/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.301198 tsugu-0.4.5/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.057525 tsugu-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 03:05:10.000000 tsugu-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 03:05:22.057525 tsugu-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 03:05:10.000000 tsugu-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:05:22.057525 tsugu-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 03:05:10.000000 tsugu-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.053525 tsugu-0.4.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 03:05:10.000000 tsugu-0.4.6/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.053525 tsugu-0.4.6/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19110 2024-04-15 03:05:10.000000 tsugu-0.4.6/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:05:22.057525 tsugu-0.4.6/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 03:05:22.000000 tsugu-0.4.6/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 03:05:21.000000 tsugu-0.4.6/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.5/LICENSE` & `tsugu-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.5/PKG-INFO` & `tsugu-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.5
+Version: 0.4.6
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.5 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.6 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.5/README.md` & `tsugu-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.5/setup.py` & `tsugu-0.4.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.5',
+    version='0.4.6',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.5/test/test_main.py` & `tsugu-0.4.6/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.5/tsugu/bot.py` & `tsugu-0.4.6/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.5/tsugu/config.py` & `tsugu-0.4.6/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.5/tsugu/router.py` & `tsugu-0.4.6/tsugu/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 
 
 class Router:
     def __init__(self):
         pass
 
     @staticmethod
+    def help(text: str, default_servers: List[int], server: int):
+        return help_command(text)
+
+    @staticmethod
     def player(text: str, default_servers: List[int], server: int):
         return v2api_from_backend('player', text, default_servers, server)
 
     @staticmethod
     def card(text: str, default_servers: List[int], server: int):
         return v2api_from_backend('card', text, default_servers, server)
```

### Comparing `tsugu-0.4.5/tsugu/utils.py` & `tsugu-0.4.6/tsugu/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,15 +431,15 @@
     if not command_name:
         # 读取 config.help_doc_dict 中的所有键
         command_list = list(config.help_doc_dict.keys())
         command_list.sort()
         return text_response(f'当前支持的命令有：\n{", ".join(command_list)}\n 请使用"help 命令名"来查看命令的详细帮助')
     else:
         # 读取 config.help_doc_dict 中的指定键
-        return text_response(config.help_doc_dict.get(command_name, '未找到对应的帮助文档'))
+        return None
 
 
 class Remote:
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         data = {
             'platform': platform,
```

### Comparing `tsugu-0.4.5/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.6/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.5
+Version: 0.4.6
 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py
 Author: kumoSleeping
 Author-email: zjr2992@outlook.com
 License: MIT
 Description: 
         <h1 align="center"> Tsugu Python Frontend <img src="./logo.jpg" width="30" width="30" height="30" alt="tmrn"/> </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.5 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.6 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

