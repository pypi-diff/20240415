# Comparing `tmp/tsugu-0.4.4.tar.gz` & `tmp/tsugu-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsugu-0.4.4.tar", last modified: Mon Apr 15 02:34:56 2024, max compression
+gzip compressed data, was "tsugu-0.4.5.tar", last modified: Mon Apr 15 02:40:21 2024, max compression
```

## Comparing `tsugu-0.4.4.tar` & `tsugu-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:34:47.000000 tsugu-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:34:56.510357 tsugu-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:34:47.000000 tsugu-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:34:56.510357 tsugu-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:34:47.000000 tsugu-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:34:47.000000 tsugu-0.4.4/test/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/tsugu/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/bot.py
--rw-r--r--   0 runner    (1001) docker     (127)    21049 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:34:47.000000 tsugu-0.4.4/tsugu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:34:56.510357 tsugu-0.4.4/tsugu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:34:56.000000 tsugu-0.4.4/tsugu.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.301198 tsugu-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 02:40:11.000000 tsugu-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:40:21.301198 tsugu-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-15 02:40:11.000000 tsugu-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 02:40:21.301198 tsugu-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 02:40:11.000000 tsugu-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.297198 tsugu-0.4.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-15 02:40:11.000000 tsugu-0.4.5/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.297198 tsugu-0.4.5/tsugu/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21143 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19193 2024-04-15 02:40:11.000000 tsugu-0.4.5/tsugu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 02:40:21.301198 tsugu-0.4.5/tsugu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 02:40:21.000000 tsugu-0.4.5/tsugu.egg-info/top_level.txt
```

### Comparing `tsugu-0.4.4/LICENSE` & `tsugu-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.4/PKG-INFO` & `tsugu-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.4
+Version: 0.4.5
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.4 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.5 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

### Comparing `tsugu-0.4.4/README.md` & `tsugu-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.4/setup.py` & `tsugu-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as readme:
     long_description = readme.read()
 
 setup(
     name='tsugu',
-    version='0.4.4',
+    version='0.4.5',
     author='kumoSleeping',
     author_email='zjr2992@outlook.com',
     license="MIT",
     description='Tsugu Python Frontend',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py',
```

### Comparing `tsugu-0.4.4/test/test_main.py` & `tsugu-0.4.5/test/test_main.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.4/tsugu/bot.py` & `tsugu-0.4.5/tsugu/bot.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.4/tsugu/config.py` & `tsugu-0.4.5/tsugu/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             "1": "en",
             "2": "tw",
             "3": "cn",
             "4": "kr",
         }
 
         self.features = {
+                "car_number_forwarding": True,
                 "change_main_server": True,
                 "switch_car_forwarding": True,
                 "bind_player": True,
                 "change_server_list": True,
                 "player_status": True,
                 "help": True,
             }
@@ -327,14 +328,15 @@
                 "0": "jp",
                 "1": "en",
                 "2": "tw",
                 "3": "cn",
                 "4": "kr",
             },
             "features": {
+                "car_number_forwarding": True,
                 "change_main_server": True,
                 "switch_car_forwarding": True,
                 "bind_player": True,
                 "change_server_list": True,
                 "player_status": True,
                 "help": True,
             },
```

### Comparing `tsugu-0.4.4/tsugu/router.py` & `tsugu-0.4.5/tsugu/router.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.4/tsugu/utils.py` & `tsugu-0.4.5/tsugu/utils.py`

 * *Files identical despite different names*

### Comparing `tsugu-0.4.4/tsugu.egg-info/PKG-INFO` & `tsugu-0.4.5/tsugu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsugu
-Version: 0.4.4
+Version: 0.4.5
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
-Metadata-Version: 2.1 Name: tsugu Version: 0.4.4 Summary: Tsugu Python Frontend
+Metadata-Version: 2.1 Name: tsugu Version: 0.4.5 Summary: Tsugu Python Frontend
 Home-page: https://github.com/kumoSleeping/tsugu-bangdream-bot-lite-py Author:
 kumoSleeping Author-email: zjr2992@outlook.com License: MIT Description:
                    ************ TTssuugguu PPyytthhoonn FFrroonntteenndd[[ttmmrrnn]] ************
                           _[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]_[_l_i_c_e_n_s_e_]
 
                     Python ç¼åç Tsugu åç«¯æ¨¡å ***
                               ********** ?å?®??ç??° **********
```

