# Comparing `tmp/webchatgpt-0.2.9.tar.gz` & `tmp/webchatgpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webchatgpt-0.2.9.tar", last modified: Wed Feb 21 10:56:49 2024, max compression
+gzip compressed data, was "webchatgpt-0.3.0.tar", last modified: Mon Apr 15 15:31:58 2024, max compression
```

## Comparing `webchatgpt-0.2.9.tar` & `webchatgpt-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:56:49.036887 webchatgpt-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17586 2024-02-21 10:56:49.036887 webchatgpt-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2024-02-21 10:56:48.000000 webchatgpt-0.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:56:49.032887 webchatgpt-0.2.9/WebChatGPT/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/WebChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/WebChatGPT/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28547 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/WebChatGPT/console.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/WebChatGPT/errors.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    33982 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/WebChatGPT/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8764 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/WebChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 10:56:49.036887 webchatgpt-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:56:49.032887 webchatgpt-0.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-21 10:56:35.000000 webchatgpt-0.2.9/tests/test_webchatgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 10:56:49.036887 webchatgpt-0.2.9/webchatgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17586 2024-02-21 10:56:49.000000 webchatgpt-0.2.9/webchatgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-21 10:56:49.000000 webchatgpt-0.2.9/webchatgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 10:56:49.000000 webchatgpt-0.2.9/webchatgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-21 10:56:49.000000 webchatgpt-0.2.9/webchatgpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-21 10:56:49.000000 webchatgpt-0.2.9/webchatgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-21 10:56:49.000000 webchatgpt-0.2.9/webchatgpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:31:58.618192 webchatgpt-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-15 15:31:58.614192 webchatgpt-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15761 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:31:58.614192 webchatgpt-0.3.0/WebChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/WebChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/WebChatGPT/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28547 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/WebChatGPT/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/WebChatGPT/errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32492 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/WebChatGPT/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/WebChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:31:58.618192 webchatgpt-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:31:58.614192 webchatgpt-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-15 15:31:54.000000 webchatgpt-0.3.0/tests/test_webchatgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:31:58.614192 webchatgpt-0.3.0/webchatgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17472 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/webchatgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/webchatgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/webchatgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/webchatgpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/webchatgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 15:31:58.000000 webchatgpt-0.3.0/webchatgpt.egg-info/top_level.txt
```

### Comparing `webchatgpt-0.2.9/LICENSE` & `webchatgpt-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `webchatgpt-0.2.9/PKG-INFO` & `webchatgpt-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webchatgpt
-Version: 0.2.9
+Version: 0.3.0
 Summary: Reverse Engineering of ChatGPT Web-Version
 Home-page: https://github.com/Simatwa/WebChatGPT
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: GNU v3
 Project-URL: Bug Report, https://github.com/Simatwa/WebChatGPT/issues/new
@@ -32,22 +32,21 @@
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3
 Requires-Dist: rich==13.3.4
 Requires-Dist: clipman==3.1.0
 Requires-Dist: pyperclip==1.8.2
-Requires-Dist: websocket-client==1.7.0
 
 <h1 align="center"> WebChatGPT </h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/WebChatGPT/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/WebChatGPT/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GNUv3&label=License"/></a>
-<a href="https://pypi.org/project/webchatgpt"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.2.7&color=green"/></a>
+<a href="https://pypi.org/project/webchatgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/webchatgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/webchatgpt"><img src="https://static.pepy.tech/personalized-badge/webchatgpt?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <!--<a href="https://github.com/Simatwa/WebChatGPT/releases"><img src="https://img.shields.io/github/downloads/Simatwa/WebChatGPT/total?label=Downloads&color=success" alt="Downloads"></img></a> -->
 <a href="https://github.com/Simatwa/WebChatGPT/releases"><img src="https://img.shields.io/github/v/release/Simatwa/WebChatGPT?color=success&label=Release&logo=github" alt="Latest release"></img></a>
@@ -62,17 +61,14 @@
 
 <p align="center">
 <a href="https://en.wikipedia.org/wiki/Reverse_engineering">Reverse Engineering</a> of ChatGPT in Python.
 </p> 
 
 Unlike the [official Openai library](https://github.com/openai/openai-python), this library makes REST-API calls to [ChatGPT](https://chat.openai.com) via the **browser** endpoints. *No API-KEY required*
 
-> [!CAUTION]
-> **Currently** very unreliable!
-
 ```python
 from WebChatGPT import ChatGPT
 bot = ChatGPT(
     "<path-to-openai-cookies.json>"
 )
 response = bot.chat('<Your prompt>')
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webchatgpt Version: 0.2.9 Summary: Reverse
+Metadata-Version: 2.1 Name: webchatgpt Version: 0.3.0 Summary: Reverse
 Engineering of ChatGPT Web-Version Home-page: https://github.com/Simatwa/
 WebChatGPT Author: Smartwa Author-email: simatwacaleb@proton.me Maintainer:
 Smartwa License: GNU v3 Project-URL: Bug Report, https://github.com/Simatwa/
 WebChatGPT/issues/new Project-URL: Homepage, https://github.com/Simatwa/
 WebChatGPT Project-URL: Source Code, https://github.com/Simatwa/WebChatGPT
 Project-URL: Issue Tracker, https://github.com/Simatwa/WebChatGPT/issues
 Project-URL: Download, https://github.com/Simatwa/WebChatGPT/releases Project-
@@ -16,42 +16,40 @@
 Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests==2.31.0 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3 Requires-Dist: rich==13.3.4 Requires-Dist:
-clipman==3.1.0 Requires-Dist: pyperclip==1.8.2 Requires-Dist: websocket-
-client==1.7.0
+clipman==3.1.0 Requires-Dist: pyperclip==1.8.2
                            ************ WWeebbCChhaattGGPPTT ************
   _[_P_y_t_h_o_n_ _T_e_s_t_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
      _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_W_e_b_C_h_a_t_G_P_T_]_[_w_a_k_a_t_i_m_e_]
   [https://github.com/Simatwa/WebChatGPT/blob/main/assets/demo.gif?raw=true]
                    _R_e_v_e_r_s_e_ _E_n_g_i_n_e_e_r_i_n_g of ChatGPT in Python.
 Unlike the [official Openai library](https://github.com/openai/openai-python),
 this library makes REST-API calls to [ChatGPT](https://chat.openai.com) via the
-**browser** endpoints. *No API-KEY required* > [!CAUTION] > **Currently** very
-unreliable! ```python from WebChatGPT import ChatGPT bot = ChatGPT( "" )
-response = bot.chat('') print(response) #Ouput : What can I do for you today?
-``` ## Prerequisites - [x] Python>=3.10 Installed - [x] Chrome or Firefox
-browser - [x] [export-cookie-for-puppeteer](https://github.com/ktty1220/export-
-cookie-for-puppeteer) extension installed. ## Installation & usage ###
-Installation Either of the following ways will get you ready : 1. From pypi:
-``` pip install --upgrade webchatgpt ``` 2. From source ``` pip install
-git+https://github.com/Simatwa/WebChatGPT.git ``` ## Usage The script utilizes
-[HTTP Cookies](https://en.wikipedia.org/wiki/HTTP_cookie) and [OAuth](https://
-en.wikipedia.org/wiki/OAuth) to justify the REST-API requests at [Openai]
-(https://openai.com). In order to do that, we will use the [export-cookie-for-
-puppeteer](https://github.com/ktty1220/export-cookie-for-puppeteer) extension
-to extract the cookies which will later on used to retrieve the OAuth. ###
-Procedure 1. Login to https://chat.openai.com 2. Upon successfull login, use
-**Export cookie JSON File Puppeteer** to export cookies. If you haven't
-installed the extension, here are the quick installation links for you. -
-[Google Chrome](https://chrome.google.com/webstore/detail/
+**browser** endpoints. *No API-KEY required* ```python from WebChatGPT import
+ChatGPT bot = ChatGPT( "" ) response = bot.chat('') print(response) #Ouput :
+What can I do for you today? ``` ## Prerequisites - [x] Python>=3.10 Installed
+- [x] Chrome or Firefox browser - [x] [export-cookie-for-puppeteer](https://
+github.com/ktty1220/export-cookie-for-puppeteer) extension installed. ##
+Installation & usage ### Installation Either of the following ways will get you
+ready : 1. From pypi: ``` pip install --upgrade webchatgpt ``` 2. From source
+``` pip install git+https://github.com/Simatwa/WebChatGPT.git ``` ## Usage The
+script utilizes [HTTP Cookies](https://en.wikipedia.org/wiki/HTTP_cookie) and
+[OAuth](https://en.wikipedia.org/wiki/OAuth) to justify the REST-API requests
+at [Openai](https://openai.com). In order to do that, we will use the [export-
+cookie-for-puppeteer](https://github.com/ktty1220/export-cookie-for-puppeteer)
+extension to extract the cookies which will later on used to retrieve the
+OAuth. ### Procedure 1. Login to https://chat.openai.com 2. Upon successfull
+login, use **Export cookie JSON File Puppeteer** to export cookies. If you
+haven't installed the extension, here are the quick installation links for you.
+- [Google Chrome](https://chrome.google.com/webstore/detail/
 nmckokihipjgplolmcmjakknndddifde) - [Firefox](https://addons.mozilla.org/ja/
 firefox/addon/
 %E3%82%AF%E3%83%83%E3%82%AD%E3%83%BCjson%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E5%87%BA%E5%8A%9B-
 for-puppeteer/) By doing that you are good to go. - Converse Interactively: ```
 $ webchatgpt interactive -C "" ``` - Have a quick response ``` $ webchatgpt
 generate -C "" ``` - Since `generate` is the default option so something like
 this will this workout. `$ webchatgpt -C ""` Alternatives to `-C ` : On the
```

### Comparing `webchatgpt-0.2.9/README.md` & `webchatgpt-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <h1 align="center"> WebChatGPT </h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/WebChatGPT/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/WebChatGPT/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GNUv3&label=License"/></a>
-<a href="https://pypi.org/project/webchatgpt"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.2.7&color=green"/></a>
+<a href="https://pypi.org/project/webchatgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/webchatgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/webchatgpt"><img src="https://static.pepy.tech/personalized-badge/webchatgpt?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <!--<a href="https://github.com/Simatwa/WebChatGPT/releases"><img src="https://img.shields.io/github/downloads/Simatwa/WebChatGPT/total?label=Downloads&color=success" alt="Downloads"></img></a> -->
 <a href="https://github.com/Simatwa/WebChatGPT/releases"><img src="https://img.shields.io/github/v/release/Simatwa/WebChatGPT?color=success&label=Release&logo=github" alt="Latest release"></img></a>
@@ -22,17 +22,14 @@
 
 <p align="center">
 <a href="https://en.wikipedia.org/wiki/Reverse_engineering">Reverse Engineering</a> of ChatGPT in Python.
 </p> 
 
 Unlike the [official Openai library](https://github.com/openai/openai-python), this library makes REST-API calls to [ChatGPT](https://chat.openai.com) via the **browser** endpoints. *No API-KEY required*
 
-> [!CAUTION]
-> **Currently** very unreliable!
-
 ```python
 from WebChatGPT import ChatGPT
 bot = ChatGPT(
     "<path-to-openai-cookies.json>"
 )
 response = bot.chat('<Your prompt>')
```

#### html2text {}

```diff
@@ -2,32 +2,31 @@
   _[_P_y_t_h_o_n_ _T_e_s_t_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
      _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_W_e_b_C_h_a_t_G_P_T_]_[_w_a_k_a_t_i_m_e_]
   [https://github.com/Simatwa/WebChatGPT/blob/main/assets/demo.gif?raw=true]
                    _R_e_v_e_r_s_e_ _E_n_g_i_n_e_e_r_i_n_g of ChatGPT in Python.
 Unlike the [official Openai library](https://github.com/openai/openai-python),
 this library makes REST-API calls to [ChatGPT](https://chat.openai.com) via the
-**browser** endpoints. *No API-KEY required* > [!CAUTION] > **Currently** very
-unreliable! ```python from WebChatGPT import ChatGPT bot = ChatGPT( "" )
-response = bot.chat('') print(response) #Ouput : What can I do for you today?
-``` ## Prerequisites - [x] Python>=3.10 Installed - [x] Chrome or Firefox
-browser - [x] [export-cookie-for-puppeteer](https://github.com/ktty1220/export-
-cookie-for-puppeteer) extension installed. ## Installation & usage ###
-Installation Either of the following ways will get you ready : 1. From pypi:
-``` pip install --upgrade webchatgpt ``` 2. From source ``` pip install
-git+https://github.com/Simatwa/WebChatGPT.git ``` ## Usage The script utilizes
-[HTTP Cookies](https://en.wikipedia.org/wiki/HTTP_cookie) and [OAuth](https://
-en.wikipedia.org/wiki/OAuth) to justify the REST-API requests at [Openai]
-(https://openai.com). In order to do that, we will use the [export-cookie-for-
-puppeteer](https://github.com/ktty1220/export-cookie-for-puppeteer) extension
-to extract the cookies which will later on used to retrieve the OAuth. ###
-Procedure 1. Login to https://chat.openai.com 2. Upon successfull login, use
-**Export cookie JSON File Puppeteer** to export cookies. If you haven't
-installed the extension, here are the quick installation links for you. -
-[Google Chrome](https://chrome.google.com/webstore/detail/
+**browser** endpoints. *No API-KEY required* ```python from WebChatGPT import
+ChatGPT bot = ChatGPT( "" ) response = bot.chat('') print(response) #Ouput :
+What can I do for you today? ``` ## Prerequisites - [x] Python>=3.10 Installed
+- [x] Chrome or Firefox browser - [x] [export-cookie-for-puppeteer](https://
+github.com/ktty1220/export-cookie-for-puppeteer) extension installed. ##
+Installation & usage ### Installation Either of the following ways will get you
+ready : 1. From pypi: ``` pip install --upgrade webchatgpt ``` 2. From source
+``` pip install git+https://github.com/Simatwa/WebChatGPT.git ``` ## Usage The
+script utilizes [HTTP Cookies](https://en.wikipedia.org/wiki/HTTP_cookie) and
+[OAuth](https://en.wikipedia.org/wiki/OAuth) to justify the REST-API requests
+at [Openai](https://openai.com). In order to do that, we will use the [export-
+cookie-for-puppeteer](https://github.com/ktty1220/export-cookie-for-puppeteer)
+extension to extract the cookies which will later on used to retrieve the
+OAuth. ### Procedure 1. Login to https://chat.openai.com 2. Upon successfull
+login, use **Export cookie JSON File Puppeteer** to export cookies. If you
+haven't installed the extension, here are the quick installation links for you.
+- [Google Chrome](https://chrome.google.com/webstore/detail/
 nmckokihipjgplolmcmjakknndddifde) - [Firefox](https://addons.mozilla.org/ja/
 firefox/addon/
 %E3%82%AF%E3%83%83%E3%82%AD%E3%83%BCjson%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E5%87%BA%E5%8A%9B-
 for-puppeteer/) By doing that you are good to go. - Converse Interactively: ```
 $ webchatgpt interactive -C "" ``` - Have a quick response ``` $ webchatgpt
 generate -C "" ``` - Since `generate` is the default option so something like
 this will this workout. `$ webchatgpt -C ""` Alternatives to `-C ` : On the
```

### Comparing `webchatgpt-0.2.9/WebChatGPT/console.py` & `webchatgpt-0.3.0/WebChatGPT/console.py`

 * *Files identical despite different names*

### Comparing `webchatgpt-0.2.9/WebChatGPT/main.py` & `webchatgpt-0.3.0/WebChatGPT/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,73 +1,14 @@
 #!/usr/bin/python
 import requests
 from WebChatGPT import utils
-import logging
 import json
 import re
 from functools import lru_cache
-import websocket
-from base64 import b64decode
-from WebChatGPT.errors import WebSocketError
-from threading import Thread as thr
 from typing import Iterator
-from .errors import MaximumRetrialError
-
-
-class Websocket:
-
-    def __init__(
-        self,
-        data: dict,
-        chatgpt: object,
-        trace: bool = False,
-    ):
-        chatgpt.socket_closed = False
-        chatgpt.loading_chunk = ""
-        self.payload = data.copy()
-        self.url = data.get("wss_url")
-        self.payload.pop("wss_url")
-        self.chatgpt = chatgpt
-        self.last_response_chunk: dict = {}
-        self.last_response_undecoded_chunk: dict = {}
-        websocket.enableTrace(trace)
-
-    def on_message(self, ws, message):
-        response = json.loads(message)
-        self.chatgpt.last_response_undecoded_chunk = response
-        decoded_body = b64decode(response["body"]).decode("utf-8")
-        response["body"] = decoded_body
-        self.chatgpt.last_response_chunk = response
-        self.chatgpt.loading_chunk = decoded_body
-
-    def on_error(self, ws, error):
-        self.on_close("ws")
-        raise WebSocketError(error)
-
-    def on_close(self, ws, *args, **kwargs):
-        self.chatgpt.socket_closed = True
-
-    def on_open(
-        self,
-        ws,
-    ):
-        json_data = json.dumps(self.payload, indent=4)
-        ws.send(json_data)
-
-    def run(
-        self,
-    ):
-        ws = websocket.WebSocketApp(
-            self.url,
-            on_message=self.on_message,
-            on_error=self.on_error,
-            on_close=self.on_close,
-            on_open=self.on_open,
-        )
-        ws.run_forever(origin="https://chat.openai.com")
 
 
 class ChatGPT:
     def __init__(
         self,
         cookie_path: str,
         model: str = "text-davinci-002-render-sha",
@@ -123,32 +64,30 @@
         )
         self.shared_conversation_view_endpoint = (
             "https://chat.openai.com/share/%(share_id)s"
         )
         self.stop_sharing_conversation_endpoint = (
             "https://chat.openai.com/backend-api/%(share_id)s"
         )
+        self.sentinel_chat_requirements_endpoint: str = (
+            "https://chat.openai.com/backend-api/sentinel/chat-requirements"
+        )
         self.session.headers["User-Agent"] = user_agent
         self.locale = locale
         self.model = model
         self.disable_history_and_training = disable_history_and_training
         self.last_response = {}
         self.last_response_metadata = {
             1: {},
             2: {},
         }
         self.__already_init = False
         self.__index = conversation_index
         self.__title_cache = {}
-        self.last_response_undecoded_chunk: str = ""
-        self.last_response_chunk: dict = {}
-        self.loading_chunk: str = ""
-        self.socket_closed: bool = True
-        self.trace = trace
-        self.request_more_times: int = 2
+        self.stream_chunk_size = 64
         # self.register_ws =self.session.post("https://chat.openai.com/backend-api/register-websocket")
         # Websocket(self.register_ws.json(),self).run()
 
     def __generate_payload(self, prompt: str) -> dict:
         return utils.generate_payload(self, prompt)
 
     @property
@@ -167,14 +106,21 @@
             )  # When index is 0 create new conversation else resume conversation
             self.last_response_metadata[2]["conversation_id"] = id
             return id
 
     def get_current_message_id(self):
         return self.last_response_metadata.get(2).get("message_id")
 
+    def update_sentinel_tokens(self):
+        resp = self.session.post(self.sentinel_chat_requirements_endpoint, json={})
+        resp.raise_for_status()
+        self.session.headers.update(
+            {"OpenAI-Sentinel-Chat-Requirements-Token": resp.json()["token"]}
+        )
+
     def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw_response: bool = False,
     ) -> dict | Iterator:
         """Chat with ChatGPT
@@ -224,40 +170,36 @@
                 "recipient": "all"
             },
             "conversation_id": "affdda8c-588c-4342-9869-26c5bd7xxxxx",
             "error": null
         }
         ```
         """
+        self.update_sentinel_tokens()
         response = self.session.post(
             url=self.conversation_endpoint,
             json=self.__generate_payload(prompt),
             timeout=self.timeout,
-            stream=False,
+            stream=True,
         )
-        response.raise_for_status()
-        ws_payload = dict(response.json())
-        self.__request_more_count: int = 0
-
-        # out = lambda v:print(json.dumps(dict(v), indent=4))
-        # out(response.headers)
-        def for_stream():
-
-            ws = Websocket(ws_payload, self, self.trace)
-            t1 = thr(target=ws.run)
-            t1.start()
-            cached_loading_chunk = self.loading_chunk
-            cached_last_response = self.last_response.copy()
-            while True:
-                if self.loading_chunk != cached_loading_chunk:
-                    # New chunk loaded
+        # response.raise_for_status()
+        if (
+            response.ok
+            and response.headers.get("content-type")
+            == "text/event-stream; charset=utf-8"
+        ):
+
+            def for_stream():
+                for value in response.iter_lines(
+                    decode_unicode=True,
+                    delimiter="data:",
+                    chunk_size=self.stream_chunk_size,
+                ):
                     try:
-                        value = self.loading_chunk
-                        # print(value)
-                        to_dict = json.loads(value[5:])
+                        to_dict = json.loads(value)
                         if "is_completion" in to_dict.keys():
                             # Metadata (response)
                             self.last_response_metadata[
                                 2 if to_dict.get("is_completion") else 1
                             ] = to_dict
                             continue
                         # Only data containing the `feedback body` make it to here
@@ -265,48 +207,43 @@
                         yield value if raw_response else to_dict
                     except json.decoder.JSONDecodeError:
                         # Caused by either empty string or [DONE]
                         if raw_response:
                             yield value
                         pass
 
-                    finally:
-                        cached_loading_chunk = self.loading_chunk
+            def for_non_stream():
+                response_to_be_returned = {}
+                for value in response.iter_lines(
+                    decode_unicode=True,
+                    delimiter="data:",
+                    chunk_size=self.stream_chunk_size,
+                ):
+                    try:
+                        to_dict = json.loads(value)
+                        if "is_completion" in to_dict.keys():
+                            # Metadata (response)
+                            self.last_response_metadata[
+                                2 if to_dict.get("is_completion") else 1
+                            ] = to_dict
+                            continue
+                        # Only data containing the `feedback body` make it to here
+                        self.last_response.update(to_dict)
+                        response_to_be_returned.update(to_dict)
+                    except json.decoder.JSONDecodeError:
+                        # Caused by either empty string or [DONE]
+                        pass
+                return response_to_be_returned
 
-                if self.socket_closed:
-                    t1.join()
-                    break
-
-            if (
-                self.last_response == cached_last_response
-                or self.last_response["message"]["status"] != "finished_successfully"
-            ):
-
-                # print(json.dumps(self.last_response, indent=4))
-                # print("Requesting more body")
-                # print('=='*40)
-                t1.join()
-                if self.__request_more_count >= self.request_more_times:
-                    raise MaximumRetrialError(
-                        f"Failed to generate response after {self.request_more_times} attempts"
-                    )
-
-                for value in for_stream():
-                    yield value
-
-                self.__request_more_count += 1
-            # else:
-            #   print(print(json.dumps(self.last_response_chunk, indent=4)))
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
+            return for_stream() if stream else for_non_stream()
 
-        return for_stream() if stream else for_non_stream()
+        else:
+            raise Exception(
+                f"Failed to fetch response - ({response.status_code}, {response.reason} : {response.headers.get('content-type')} : {response.text}"
+            )
 
     def chat(self, prompt: str, stream: bool = False) -> str:
         """Interact with ChatGPT on the fly
 
         Args:
             prompt (str): Message to ChatGPT
             stream (bool, optional): Yield the text response. Defaults to False.
```

### Comparing `webchatgpt-0.2.9/WebChatGPT/utils.py` & `webchatgpt-0.3.0/WebChatGPT/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime, timezone
 import json
 import logging
-import os
+import locale
 from uuid import uuid4
 from typing import Any
 from .errors import CookieExpiredError
 from .errors import VerificationError
 
 
 __common_error_support_info = "Incase you have no idea on how to get the cookies check the documentation at - \
@@ -23,14 +23,15 @@
     "Host": "chat.openai.com",
     "Origin": "https://chat.openai.com",
     "Referer": "https://chat.openai.com/",
     "Sec-Fetch-Dest": "empty",
     "Sec-Fetch-Mode": "cors",
     "Sec-Fetch-Site": "same-origin",
     "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:120.0) Gecko/20100101 Firefox/120.0",
+    "OAI-Language": locale.getlocale()[0].replace("_", "-"),
 }
 
 response_example = {
     "message": {
         "id": "b9ce2438-a00a-4c1e-9487-3abba1xxxxx",
         "author": {"role": "assistant", "name": None, "metadata": {}},
         "create_time": 1708178888.142936,
@@ -234,15 +235,15 @@
         ],
         # "conversation_id": self.conversation_metadata["id"],
         # "parent_message_id": "5b45a98c-0871-48ed-895b-f36f188cxxxx",
         "model": self.model,
         "timezone_offset_min": -180,
         "suggestions": [],
         "history_and_training_disabled": self.disable_history_and_training,
-        "arkose_token": None,
+        # "arkose_token": None,
         "conversation_mode": {"kind": "primary_assistant"},
         "force_paragen": False,
         "force_rate_limit": False,
     }
     if self.current_conversation_id:
         # Continuing conversation
         payload_template["conversation_id"] = self.current_conversation_id
```

### Comparing `webchatgpt-0.2.9/setup.py` & `webchatgpt-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="webchatgpt",
-    version="0.2.9",
+    version="0.3.0",
     license="GNU v3",
     author="Smartwa",
     maintainer="Smartwa",
     author_email="simatwacaleb@proton.me",
     description="Reverse Engineering of ChatGPT Web-Version",
     packages=["WebChatGPT"],
     url="https://github.com/Simatwa/WebChatGPT",
@@ -37,15 +37,14 @@
     install_requires=[
         "requests==2.31.0",
         "python-dotenv==1.0.0",
         "click==8.1.3",
         "rich==13.3.4",
         "clipman==3.1.0",
         "pyperclip==1.8.2",
-        "websocket-client==1.7.0",
     ],
     python_requires=">=3.10",
     keywords=[
         "chatgpt",
         "webchatgpt",
         "gpt",
         "chatgpt-cli",
```

### Comparing `webchatgpt-0.2.9/tests/test_webchatgpt.py` & `webchatgpt-0.3.0/tests/test_webchatgpt.py`

 * *Files identical despite different names*

### Comparing `webchatgpt-0.2.9/webchatgpt.egg-info/PKG-INFO` & `webchatgpt-0.3.0/webchatgpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webchatgpt
-Version: 0.2.9
+Version: 0.3.0
 Summary: Reverse Engineering of ChatGPT Web-Version
 Home-page: https://github.com/Simatwa/WebChatGPT
 Author: Smartwa
 Author-email: simatwacaleb@proton.me
 Maintainer: Smartwa
 License: GNU v3
 Project-URL: Bug Report, https://github.com/Simatwa/WebChatGPT/issues/new
@@ -32,22 +32,21 @@
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3
 Requires-Dist: rich==13.3.4
 Requires-Dist: clipman==3.1.0
 Requires-Dist: pyperclip==1.8.2
-Requires-Dist: websocket-client==1.7.0
 
 <h1 align="center"> WebChatGPT </h1>
 
 <p align="center">
 <a href="https://github.com/Simatwa/WebChatGPT/actions/workflows/python-test.yml"><img src="https://github.com/Simatwa/WebChatGPT/actions/workflows/python-test.yml/badge.svg" alt="Python Test"/></a>
 <a href="LICENSE"><img alt="License" src="https://img.shields.io/static/v1?logo=GPL&color=Blue&message=GNUv3&label=License"/></a>
-<a href="https://pypi.org/project/webchatgpt"><img alt="PyPi" src="https://img.shields.io/static/v1?logo=pypi&label=Pypi&message=v0.2.7&color=green"/></a>
+<a href="https://pypi.org/project/webchatgpt"><img alt="PyPi" src="https://img.shields.io/pypi/v/webchatgpt?color=green"/></a>
 <a href="https://github.com/psf/black"><img alt="Black" src="https://img.shields.io/static/v1?logo=Black&label=Code-style&message=Black"/></a>
 <a href="#"><img alt="Passing" src="https://img.shields.io/static/v1?logo=Docs&label=Docs&message=Passing&color=green"/></a>
 <a href="#"><img alt="coverage" src="https://img.shields.io/static/v1?logo=Coverage&label=Coverage&message=90%&color=yellowgreen"/></a>
 <a href="#" alt="progress"><img alt="Progress" src="https://img.shields.io/static/v1?logo=Progress&label=Progress&message=95%&color=green"/></a>
 <a href="https://pepy.tech/project/webchatgpt"><img src="https://static.pepy.tech/personalized-badge/webchatgpt?period=total&units=international_system&left_color=grey&right_color=green&left_text=Downloads" alt="Downloads"></a>
 <!--<a href="https://github.com/Simatwa/WebChatGPT/releases"><img src="https://img.shields.io/github/downloads/Simatwa/WebChatGPT/total?label=Downloads&color=success" alt="Downloads"></img></a> -->
 <a href="https://github.com/Simatwa/WebChatGPT/releases"><img src="https://img.shields.io/github/v/release/Simatwa/WebChatGPT?color=success&label=Release&logo=github" alt="Latest release"></img></a>
@@ -62,17 +61,14 @@
 
 <p align="center">
 <a href="https://en.wikipedia.org/wiki/Reverse_engineering">Reverse Engineering</a> of ChatGPT in Python.
 </p> 
 
 Unlike the [official Openai library](https://github.com/openai/openai-python), this library makes REST-API calls to [ChatGPT](https://chat.openai.com) via the **browser** endpoints. *No API-KEY required*
 
-> [!CAUTION]
-> **Currently** very unreliable!
-
 ```python
 from WebChatGPT import ChatGPT
 bot = ChatGPT(
     "<path-to-openai-cookies.json>"
 )
 response = bot.chat('<Your prompt>')
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: webchatgpt Version: 0.2.9 Summary: Reverse
+Metadata-Version: 2.1 Name: webchatgpt Version: 0.3.0 Summary: Reverse
 Engineering of ChatGPT Web-Version Home-page: https://github.com/Simatwa/
 WebChatGPT Author: Smartwa Author-email: simatwacaleb@proton.me Maintainer:
 Smartwa License: GNU v3 Project-URL: Bug Report, https://github.com/Simatwa/
 WebChatGPT/issues/new Project-URL: Homepage, https://github.com/Simatwa/
 WebChatGPT Project-URL: Source Code, https://github.com/Simatwa/WebChatGPT
 Project-URL: Issue Tracker, https://github.com/Simatwa/WebChatGPT/issues
 Project-URL: Download, https://github.com/Simatwa/WebChatGPT/releases Project-
@@ -16,42 +16,40 @@
 Libraries :: Python Modules Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests==2.31.0 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: click==8.1.3 Requires-Dist: rich==13.3.4 Requires-Dist:
-clipman==3.1.0 Requires-Dist: pyperclip==1.8.2 Requires-Dist: websocket-
-client==1.7.0
+clipman==3.1.0 Requires-Dist: pyperclip==1.8.2
                            ************ WWeebbCChhaattGGPPTT ************
   _[_P_y_t_h_o_n_ _T_e_s_t_]_[_L_i_c_e_n_s_e_]_[_P_y_P_i_]_[_B_l_a_c_k_]_[_P_a_s_s_i_n_g_]_[_c_o_v_e_r_a_g_e_]_[_P_r_o_g_r_e_s_s_]_[_D_o_w_n_l_o_a_d_s_]
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_r_e_l_e_a_s_e_ _d_a_t_e_]_[_h_t_t_p_s_:_/_/_h_i_t_s_._s_e_e_y_o_u_f_a_r_m_._c_o_m_/_a_p_i_/_c_o_u_n_t_/_i_n_c_r_/
      _b_a_d_g_e_._s_v_g_?_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_g_i_t_h_u_b_._c_o_m_/_S_i_m_a_t_w_a_/_W_e_b_C_h_a_t_G_P_T_]_[_w_a_k_a_t_i_m_e_]
   [https://github.com/Simatwa/WebChatGPT/blob/main/assets/demo.gif?raw=true]
                    _R_e_v_e_r_s_e_ _E_n_g_i_n_e_e_r_i_n_g of ChatGPT in Python.
 Unlike the [official Openai library](https://github.com/openai/openai-python),
 this library makes REST-API calls to [ChatGPT](https://chat.openai.com) via the
-**browser** endpoints. *No API-KEY required* > [!CAUTION] > **Currently** very
-unreliable! ```python from WebChatGPT import ChatGPT bot = ChatGPT( "" )
-response = bot.chat('') print(response) #Ouput : What can I do for you today?
-``` ## Prerequisites - [x] Python>=3.10 Installed - [x] Chrome or Firefox
-browser - [x] [export-cookie-for-puppeteer](https://github.com/ktty1220/export-
-cookie-for-puppeteer) extension installed. ## Installation & usage ###
-Installation Either of the following ways will get you ready : 1. From pypi:
-``` pip install --upgrade webchatgpt ``` 2. From source ``` pip install
-git+https://github.com/Simatwa/WebChatGPT.git ``` ## Usage The script utilizes
-[HTTP Cookies](https://en.wikipedia.org/wiki/HTTP_cookie) and [OAuth](https://
-en.wikipedia.org/wiki/OAuth) to justify the REST-API requests at [Openai]
-(https://openai.com). In order to do that, we will use the [export-cookie-for-
-puppeteer](https://github.com/ktty1220/export-cookie-for-puppeteer) extension
-to extract the cookies which will later on used to retrieve the OAuth. ###
-Procedure 1. Login to https://chat.openai.com 2. Upon successfull login, use
-**Export cookie JSON File Puppeteer** to export cookies. If you haven't
-installed the extension, here are the quick installation links for you. -
-[Google Chrome](https://chrome.google.com/webstore/detail/
+**browser** endpoints. *No API-KEY required* ```python from WebChatGPT import
+ChatGPT bot = ChatGPT( "" ) response = bot.chat('') print(response) #Ouput :
+What can I do for you today? ``` ## Prerequisites - [x] Python>=3.10 Installed
+- [x] Chrome or Firefox browser - [x] [export-cookie-for-puppeteer](https://
+github.com/ktty1220/export-cookie-for-puppeteer) extension installed. ##
+Installation & usage ### Installation Either of the following ways will get you
+ready : 1. From pypi: ``` pip install --upgrade webchatgpt ``` 2. From source
+``` pip install git+https://github.com/Simatwa/WebChatGPT.git ``` ## Usage The
+script utilizes [HTTP Cookies](https://en.wikipedia.org/wiki/HTTP_cookie) and
+[OAuth](https://en.wikipedia.org/wiki/OAuth) to justify the REST-API requests
+at [Openai](https://openai.com). In order to do that, we will use the [export-
+cookie-for-puppeteer](https://github.com/ktty1220/export-cookie-for-puppeteer)
+extension to extract the cookies which will later on used to retrieve the
+OAuth. ### Procedure 1. Login to https://chat.openai.com 2. Upon successfull
+login, use **Export cookie JSON File Puppeteer** to export cookies. If you
+haven't installed the extension, here are the quick installation links for you.
+- [Google Chrome](https://chrome.google.com/webstore/detail/
 nmckokihipjgplolmcmjakknndddifde) - [Firefox](https://addons.mozilla.org/ja/
 firefox/addon/
 %E3%82%AF%E3%83%83%E3%82%AD%E3%83%BCjson%E3%83%95%E3%82%A1%E3%82%A4%E3%83%AB%E5%87%BA%E5%8A%9B-
 for-puppeteer/) By doing that you are good to go. - Converse Interactively: ```
 $ webchatgpt interactive -C "" ``` - Have a quick response ``` $ webchatgpt
 generate -C "" ``` - Since `generate` is the default option so something like
 this will this workout. `$ webchatgpt -C ""` Alternatives to `-C ` : On the
```

