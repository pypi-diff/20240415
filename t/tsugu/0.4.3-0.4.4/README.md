# Comparing `tmp/tsugu-0.4.3.tar.gz` & `tmp/tsugu-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.3.tar", last modified: Mon Apr 15 02:22:53 2024, max compression
+gzip compressed data, was "tsugu-0.4.4.tar", last modified: Mon Apr 15 02:34:56 2024, max compression
```

## Comparing `tsugu-0.4.3.tar` & `tsugu-0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:22:43.000000 tsugu-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:22:53.022044 tsugu-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:22:43.000000 tsugu-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:22:53.022044 tsugu-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:22:43.000000 tsugu-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:22:43.000000 tsugu-0.4.3/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:34:47.000000 tsugu-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:34:56.510357 tsugu-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:34:47.000000 tsugu-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:34:56.510357 tsugu-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:34:47.000000 tsugu-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:34:47.000000 tsugu-0.4.4/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21049 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.3/LICENSE` & `tsugu-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.3/PKG-INFO` & `tsugu-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.3
+Version: 0.4.4
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.3 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.4 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.3/README.md` & `tsugu-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.3/setup.py` & `tsugu-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.3',
+    version='0.4.4',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.3/test/test_main.py` & `tsugu-0.4.4/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.3/tsugu/bot.py` & `tsugu-0.4.4/tsugu/bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         if command_matched:
             return v2_api_command(message, command_matched, api, platform, user_id, channel_id)
         if config.user_database_path:
             return bot_extra_local_database(message, user_id, platform)
         return bot_extra_remote_server(message, user_id, platform)
     except Exception as e:
         print(e)
+        raise e
         return []
 
 
 def bot_extra_local_database(message, user_id, platform):
     # 玩家状态
     if config.features.get('player_status', True):
         if message.endswith('服玩家状态'):
```

### Comparing `tsugu-0.4.3/tsugu/config.py` & `tsugu-0.4.4/tsugu/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,24 @@
         self.server_index_to_s_name = {
             "0": "jp",
             "1": "en",
             "2": "tw",
             "3": "cn",
             "4": "kr",
         }
-        self.features = (
-            {
+
+        self.features = {
                 "change_main_server": True,
                 "switch_car_forwarding": True,
                 "bind_player": True,
                 "change_server_list": True,
                 "player_status": True,
                 "help": True,
-            },
-        )
+            }
+
         self.commands = [
             {"api": "cardIllustration", "command_name": ["查插画", "查卡面"]},
             {"api": "player", "command_name": ["查玩家", "查询玩家"]},
             {"api": "gachaSimulate", "command_name": ["抽卡模拟", "卡池模拟"]},
             {"api": "gacha", "command_name": ["查卡池"]},
             {"api": "event", "command_name": ["查活动"]},
             {"api": "song", "command_name": ["查歌曲", "查曲"]},
@@ -193,15 +193,15 @@
 查询指定ID玩家的信息。省略服务器名时，默认从你当前的主服务器查询
 使用示例：
     查玩家 10000000 : 查询你当前默认服务器中，玩家ID为10000000的玩家信息
     查玩家 40474621 jp : 查询日服玩家ID为40474621的玩家信息
 """,
             "卡池模拟": """
 模拟抽卡，如果没有卡池ID的话，卡池为当前活动的卡池
-使用示例：å
+使用示例：
     抽卡模拟:模拟抽卡10次
     抽卡模拟 300 922 :模拟抽卡300次，卡池为922号卡池
 """,
             "查卡池": """
 根据卡池ID查询卡池信息
 """,
             "查活动": """
```

### Comparing `tsugu-0.4.3/tsugu/router.py` & `tsugu-0.4.4/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.3/tsugu/utils.py` & `tsugu-0.4.4/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.3/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.4/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.3
+Version: 0.4.4
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.3 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.4 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

