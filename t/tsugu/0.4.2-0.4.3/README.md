# Comparing `tmp/tsugu-0.4.2.tar.gz` & `tmp/tsugu-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.2.tar", last modified: Mon Apr 15 02:16:35 2024, max compression
+gzip compressed data, was "tsugu-0.4.3.tar", last modified: Mon Apr 15 02:22:53 2024, max compression
```

## Comparing `tsugu-0.4.2.tar` & `tsugu-0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:16:26.000000 tsugu-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:16:35.796039 tsugu-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:16:26.000000 tsugu-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:16:35.796039 tsugu-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:16:26.000000 tsugu-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:16:26.000000 tsugu-0.4.2/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:16:26.000000 tsugu-0.4.2/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:16:35.796039 tsugu-0.4.2/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:16:35.000000 tsugu-0.4.2/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:22:43.000000 tsugu-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:22:53.022044 tsugu-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:22:43.000000 tsugu-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:22:53.022044 tsugu-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:22:43.000000 tsugu-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:22:43.000000 tsugu-0.4.3/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:22:43.000000 tsugu-0.4.3/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:22:53.022044 tsugu-0.4.3/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:22:52.000000 tsugu-0.4.3/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.2/LICENSE` & `tsugu-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.2/PKG-INFO` & `tsugu-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.2
+Version: 0.4.3
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.2 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.3 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.2/README.md` & `tsugu-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.2/setup.py` & `tsugu-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.2',
+    version='0.4.3',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.2/test/test_main.py` & `tsugu-0.4.3/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.2/tsugu/bot.py` & `tsugu-0.4.3/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.2/tsugu/config.py` & `tsugu-0.4.3/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.2/tsugu/router.py` & `tsugu-0.4.3/tsugu/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         return set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         return get_user_data(platform, user_id)
 
     @staticmethod
-    def submit_car_number_msg(message: str, user_id: str, platform: str):
+    def submit_car_number_msg(message: str, user_id: str, platform: str | None = None):
         return submit_car_number_msg(message, user_id, platform)
 
 
 interior_local_method = InteriorLocal()
 
 
 class InteriorRemote:
@@ -151,12 +151,12 @@
         return Remote.set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         return Remote.get_user_data(platform, user_id)
 
     @staticmethod
-    def submit_car_number_msg(message: str, user_id: str, platform: str):
+    def submit_car_number_msg(message: str, user_id: str, platform: str | None = None):
         return submit_car_number_msg(message, user_id, platform)
 
 
 interior_remote_method = InteriorRemote()
```

### Comparing `tsugu-0.4.2/tsugu/utils.py` & `tsugu-0.4.3/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.2/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.3/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.2
+Version: 0.4.3
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.2 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.3 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

