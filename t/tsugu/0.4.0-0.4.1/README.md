# Comparing `tmp/tsugu-0.4.0.tar.gz` & `tmp/tsugu-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.0.tar", last modified: Mon Apr 15 02:01:14 2024, max compression
+gzip compressed data, was "tsugu-0.4.1.tar", last modified: Mon Apr 15 02:08:07 2024, max compression
```

## Comparing `tsugu-0.4.0.tar` & `tsugu-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:01:14.571529 tsugu-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:01:03.000000 tsugu-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:01:14.571529 tsugu-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:01:03.000000 tsugu-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:01:14.571529 tsugu-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:01:03.000000 tsugu-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:01:14.571529 tsugu-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:01:03.000000 tsugu-0.4.0/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:01:14.571529 tsugu-0.4.0/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:01:03.000000 tsugu-0.4.0/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:01:03.000000 tsugu-0.4.0/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:01:03.000000 tsugu-0.4.0/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-15 02:01:03.000000 tsugu-0.4.0/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19010 2024-04-15 02:01:03.000000 tsugu-0.4.0/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:01:14.571529 tsugu-0.4.0/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:01:14.000000 tsugu-0.4.0/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:01:14.000000 tsugu-0.4.0/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:01:14.000000 tsugu-0.4.0/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:01:14.000000 tsugu-0.4.0/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:01:14.000000 tsugu-0.4.0/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:07:57.000000 tsugu-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:08:07.942648 tsugu-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:07:57.000000 tsugu-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:08:07.942648 tsugu-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:07:57.000000 tsugu-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:07:57.000000 tsugu-0.4.1/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11115 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21074 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19010 2024-04-15 02:07:57.000000 tsugu-0.4.1/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:08:07.942648 tsugu-0.4.1/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:08:07.000000 tsugu-0.4.1/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.0/LICENSE` & `tsugu-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.0/PKG-INFO` & `tsugu-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.0 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.1 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.0/README.md` & `tsugu-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.0/setup.py` & `tsugu-0.4.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.0',
+    version='0.4.1',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.0/test/test_main.py` & `tsugu-0.4.1/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.0/tsugu/bot.py` & `tsugu-0.4.1/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.0/tsugu/config.py` & `tsugu-0.4.1/tsugu/config.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.0/tsugu/router.py` & `tsugu-0.4.1/tsugu/router.py`

 * *Files 11% similar despite different names*

```diff
@@ -114,14 +114,18 @@
     def set_server_mode(platform: str, user_id: str, text: str):
         return set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         return get_user_data(platform, user_id)
 
+    @staticmethod
+    def submit_car_number_msg(platform: str, user_id: str, car_number: str):
+        return submit_car_number_msg(platform, user_id, car_number)
+
 
 interior_local_method = InteriorLocal()
 
 
 class InteriorRemote:
     def __init__(self):
         pass
@@ -146,9 +150,13 @@
     def set_server_mode(platform: str, user_id: str, text: str):
         return Remote.set_server_mode(platform, user_id, text)
 
     @staticmethod
     def get_user_data(platform: str, user_id: str):
         return Remote.get_user_data(platform, user_id)
 
+    @staticmethod
+    def submit_car_number_msg(platform: str, user_id: str, car_number: str):
+        return submit_car_number_msg(platform, user_id, car_number)
+
 
 interior_remote_method = InteriorRemote()
```

### Comparing `tsugu-0.4.0/tsugu/utils.py` & `tsugu-0.4.1/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.0/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.1/tsugu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.0 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.1 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

