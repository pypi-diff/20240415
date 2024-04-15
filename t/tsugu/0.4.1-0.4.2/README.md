# Comparing `tmp/tsugu-0.4.1.tar.gz` & `tmp/tsugu-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.1.tar", last modified: Mon Apr 15 02:08:07 2024, max compression
+gzip compressed data, was "tsugu-0.4.2.tar", last modified: Mon Apr 15 02:16:35 2024, max compression
```

## Comparing `tsugu-0.4.1.tar` & `tsugu-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:07:57.000000 tsugu-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:08:07.942648 tsugu-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:07:57.000000 tsugu-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:08:07.942648 tsugu-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:07:57.000000 tsugu-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:07:57.000000 tsugu-0.4.1/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19010 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:16:26.000000 tsugu-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:16:35.796039 tsugu-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:16:26.000000 tsugu-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:16:35.796039 tsugu-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:16:26.000000 tsugu-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:16:26.000000 tsugu-0.4.2/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.1/LICENSE` & `tsugu-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.1/PKG-INFO` & `tsugu-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.1
+Version: 0.4.2
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.1/README.md` & `tsugu-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.1/setup.py` & `tsugu-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.1',
+    version='0.4.2',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.1/test/test_main.py` & `tsugu-0.4.2/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.1/tsugu/bot.py` & `tsugu-0.4.2/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.1/tsugu/config.py` & `tsugu-0.4.2/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.1/tsugu/router.py` & `tsugu-0.4.2/tsugu/router.py`

 * *Files 10% similar despite different names*

```diff
@@ -115,16 +115,16 @@
         return set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         return get_user_data(platform, user_id)
 
     @staticmethod
-    def submit_car_number_msg(platform: str, user_id: str, car_number: str):
-        return submit_car_number_msg(platform, user_id, car_number)
+    def submit_car_number_msg(message: str, user_id: str, platform: str):
+        return submit_car_number_msg(message, user_id, platform)
 
 
 interior_local_method = InteriorLocal()
 
 
 class InteriorRemote:
     def __init__(self):
@@ -151,12 +151,12 @@
         return Remote.set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         return Remote.get_user_data(platform, user_id)
 
     @staticmethod
-    def submit_car_number_msg(platform: str, user_id: str, car_number: str):
-        return submit_car_number_msg(platform, user_id, car_number)
+    def submit_car_number_msg(message: str, user_id: str, platform: str):
+        return submit_car_number_msg(message, user_id, platform)
 
 
 interior_remote_method = InteriorRemote()
```

### Comparing `tsugu-0.4.1/tsugu/utils.py` & `tsugu-0.4.2/tsugu/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,32 +134,40 @@
     try:
         if user_data['status'] != 'success':
             return text_response('获取用户数据失败')
         return v2api_from_backend(api, text, user_data['data']['default_server'], user_data['data']['server_mode'])
     except Exception as e:
         return text_response('前端错误: ' + str(e))
 
-def submit_car_number_msg(message, user_id, platform):
+def submit_car_number_msg(message, user_id, platform=None):
     # 检查car_config['car']中的关键字
     for keyword in config.car_config["car"]:
         if str(keyword) in message:
             break
     else:
         return False
     # 检查car_config['fake']中的关键字
     for keyword in config.car_config["fake"]:
         if str(keyword) in message:
             return False
     pattern = r"^\d{5}(\D|$)|^\d{6}(\D|$)"
     if not re.match(pattern, message):
         return False
+
     # 获取用户数据
-    user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
-    if not user_data['data']['car']:
-        return True
+    try:
+        if platform:
+            user_data = get_user_data(platform, user_id) if config.user_database_path else Remote.get_user_data(platform, user_id)
+            if not user_data['data']['car']:
+                return True
+    except Exception as e:
+        print('unknown user')
+        # 默认不开启关闭车牌，继续提交
+        pass
+
     try:
         car_id = message[:6]
         if not car_id.isdigit() and car_id[:5].isdigit():
             car_id = car_id[:5]
         # 构建URL
         url = f"https://api.bandoristation.com/index.php?function=submit_room_number&number={car_id}&user_id={user_id}&raw_message={message}&source={config.token_name}&token={config.bandori_station_token}"
         # 发送请求
@@ -168,15 +176,14 @@
             print(f"[Tsugu] 提交车牌失败，HTTP响应码: {response.status_code}")
             return True  # 虽然提交失败，但是确定了是车牌消息
         return True
     except Exception as e:
         print(f"[Tsugu] 发生异常: {e}")
         return True  # 虽然提交失败，但是确定了是车牌消息
 
-
 def match_command(message, cmd_dict):
     for command, api_value in cmd_dict.items():
         if message.startswith(command):
             return command, api_value
     return None, None
```

### Comparing `tsugu-0.4.1/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.2/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.1
+Version: 0.4.2
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.1 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.2 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

