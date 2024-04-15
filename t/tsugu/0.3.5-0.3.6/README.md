# Comparing `tmp/tsugu-0.3.5.tar.gz` & `tmp/tsugu-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.3.5.tar", last modified: Sun Apr 14 08:26:24 2024, max compression
+gzip compressed data, was "tsugu-0.3.6.tar", last modified: Sun Apr 14 14:01:20 2024, max compression
```

## Comparing `tsugu-0.3.5.tar` & `tsugu-0.3.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.142280 tsugu-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-14 08:26:10.000000 tsugu-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 08:26:24.142280 tsugu-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-14 08:26:10.000000 tsugu-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 08:26:24.142280 tsugu-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-14 08:26:10.000000 tsugu-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.138280 tsugu-0.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-14 08:26:10.000000 tsugu-0.3.5/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.138280 tsugu-0.3.5/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9271 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-04-14 08:26:10.000000 tsugu-0.3.5/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 08:26:24.138280 tsugu-0.3.5/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 08:26:24.000000 tsugu-0.3.5/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 08:26:23.000000 tsugu-0.3.5/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:01:20.713989 tsugu-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-14 14:01:12.000000 tsugu-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 14:01:20.713989 tsugu-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-14 14:01:12.000000 tsugu-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:01:20.713989 tsugu-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-14 14:01:12.000000 tsugu-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:01:20.709989 tsugu-0.3.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-14 14:01:12.000000 tsugu-0.3.6/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:01:20.713989 tsugu-0.3.6/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-14 14:01:12.000000 tsugu-0.3.6/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9390 2024-04-14 14:01:12.000000 tsugu-0.3.6/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-14 14:01:12.000000 tsugu-0.3.6/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-14 14:01:12.000000 tsugu-0.3.6/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18493 2024-04-14 14:01:12.000000 tsugu-0.3.6/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:01:20.713989 tsugu-0.3.6/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 14:01:20.000000 tsugu-0.3.6/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 14:01:20.000000 tsugu-0.3.6/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:01:20.000000 tsugu-0.3.6/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 14:01:20.000000 tsugu-0.3.6/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 14:01:20.000000 tsugu-0.3.6/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.3.5/LICENSE` & `tsugu-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.5/PKG-INFO` & `tsugu-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.5
+Version: 0.3.6
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.5 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.6 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.3.5/README.md` & `tsugu-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.5/setup.py` & `tsugu-0.3.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.3.5',
+    version='0.3.6',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.3.5/test/test_main.py` & `tsugu-0.3.6/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.5/tsugu/bot.py` & `tsugu-0.3.6/tsugu/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from .utils import *
 
 
 def bot(message, user_id, platform, channel_id):
-    message = message.strip()
+    try:
+        message = message.strip()
 
-    # 进行车牌匹配
-    status = submit_car_number_msg(message, user_id, platform)
-    if status:
-        return None  # 已经匹配了车牌，就不需要再匹配其他指令了
-
-    # 进行 v2 api 命令匹配
-    command_matched, api = match_command(message, load_commands_from_config(config.commands))
-    if command_matched:
-        return v2_api_command(message, command_matched, api, platform, user_id, channel_id)
-    if config.user_database_path:
-        return bot_extra_local_database(message, user_id, platform)
-    return bot_extra_remote_server(message, user_id, platform)
+        # 进行车牌匹配
+        status = submit_car_number_msg(message, user_id, platform)
+        if status:
+            return None  # 已经匹配了车牌，就不需要再匹配其他指令了
+
+        # 进行 v2 api 命令匹配
+        command_matched, api = match_command(message, load_commands_from_config(config.commands))
+        if command_matched:
+            return v2_api_command(message, command_matched, api, platform, user_id, channel_id)
+        if config.user_database_path:
+            return bot_extra_local_database(message, user_id, platform)
+        return bot_extra_remote_server(message, user_id, platform)
+    except Exception as e:
+        print(e)
+        return []
 
 
 def bot_extra_local_database(message, user_id, platform):
     if message.endswith('服玩家状态'):
         return player_status(user_id, platform, message[:-4]) if server_exists(r_ := query_server_info(message[:-4])) else text_response('未找到被指定的服务器') if len(message) <= 7 else None
 
     if message.startswith('玩家状态'):
```

### Comparing `tsugu-0.3.5/tsugu/config.py` & `tsugu-0.3.6/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.5/tsugu/router.py` & `tsugu-0.3.6/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.5/tsugu/utils.py` & `tsugu-0.3.6/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.3.5/tsugu.egg-info/PKG-INFO` & `tsugu-0.3.6/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.3.5
+Version: 0.3.6
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.3.5 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.3.6 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

