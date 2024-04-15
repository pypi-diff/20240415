# Comparing `tmp/w_render-0.2.4.tar.gz` & `tmp/w_render-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w_render-0.2.4.tar", last modified: Fri Apr 12 20:05:50 2024, max compression
+gzip compressed data, was "w_render-0.2.5.tar", last modified: Mon Apr 15 13:33:23 2024, max compression
```

## Comparing `w_render-0.2.4.tar` & `w_render-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.900494 w_render-0.2.4/
--rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-12 20:05:50.900494 w_render-0.2.4/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      605 2023-08-31 19:42:54.000000 w_render-0.2.4/README.md
--rw-rw-r--   0 repente   (1000) repente   (1000)       38 2024-04-12 20:05:50.900494 w_render-0.2.4/setup.cfg
--rw-rw-r--   0 repente   (1000) repente   (1000)     3297 2024-04-12 20:02:53.000000 w_render-0.2.4/setup.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.900494 w_render-0.2.4/w_render.egg-info/
--rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-12 20:05:50.000000 w_render-0.2.4/w_render.egg-info/PKG-INFO
--rw-rw-r--   0 repente   (1000) repente   (1000)      763 2024-04-12 20:05:50.000000 w_render-0.2.4/w_render.egg-info/SOURCES.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)        1 2024-04-12 20:05:50.000000 w_render-0.2.4/w_render.egg-info/dependency_links.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)      158 2024-04-12 20:05:50.000000 w_render-0.2.4/w_render.egg-info/entry_points.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       80 2024-04-12 20:05:50.000000 w_render-0.2.4/w_render.egg-info/requires.txt
--rw-rw-r--   0 repente   (1000) repente   (1000)       11 2024-04-12 20:05:50.000000 w_render-0.2.4/w_render.egg-info/top_level.txt
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.812497 w_render-0.2.4/web_render/
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.840496 w_render-0.2.4/web_render/base/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:27:26.000000 w_render-0.2.4/web_render/base/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     2337 2023-09-03 20:30:16.000000 w_render-0.2.4/web_render/base/__main__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     8581 2024-04-12 20:04:08.000000 w_render-0.2.4/web_render/base/abstract.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1125 2023-08-24 07:40:40.000000 w_render-0.2.4/web_render/base/client.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     4320 2023-08-24 21:59:25.000000 w_render-0.2.4/web_render/base/server.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     3666 2023-08-28 08:54:18.000000 w_render-0.2.4/web_render/base/test_webrender.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1508 2023-08-24 07:24:47.000000 w_render-0.2.4/web_render/config.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.852496 w_render-0.2.4/web_render/flask/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-07-28 09:55:28.000000 w_render-0.2.4/web_render/flask/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1817 2023-08-28 08:31:02.000000 w_render-0.2.4/web_render/flask/__main__.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.860495 w_render-0.2.4/web_render/flask/core/
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.868495 w_render-0.2.4/web_render/flask/core/main/
--rw-rw-r--   0 repente   (1000) repente   (1000)      837 2023-08-24 07:40:41.000000 w_render-0.2.4/web_render/flask/core/main/view.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.884495 w_render-0.2.4/web_render/flask/core/render_api/
--rw-rw-r--   0 repente   (1000) repente   (1000)     1372 2023-08-24 07:40:41.000000 w_render-0.2.4/web_render/flask/core/render_api/logic.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1075 2023-08-24 07:24:47.000000 w_render-0.2.4/web_render/flask/core/render_api/view.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      207 2023-08-24 07:24:47.000000 w_render-0.2.4/web_render/flask/core/routing.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.900494 w_render-0.2.4/web_render/flask/core/service/
--rw-rw-r--   0 repente   (1000) repente   (1000)      389 2023-08-24 07:24:47.000000 w_render-0.2.4/web_render/flask/core/service/interface.py
--rw-rw-r--   0 repente   (1000) repente   (1000)      377 2023-08-24 07:24:47.000000 w_render-0.2.4/web_render/interface.py
-drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-12 20:05:50.900494 w_render-0.2.4/web_render/script/
--rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:28:05.000000 w_render-0.2.4/web_render/script/__init__.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1507 2023-08-24 08:38:56.000000 w_render-0.2.4/web_render/script/render_server.py
--rw-rw-r--   0 repente   (1000) repente   (1000)     1498 2023-08-24 12:59:54.000000 w_render-0.2.4/web_render/tool.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.313669 w_render-0.2.5/
+-rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-15 13:33:23.313669 w_render-0.2.5/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      605 2023-08-31 19:42:54.000000 w_render-0.2.5/README.md
+-rw-rw-r--   0 repente   (1000) repente   (1000)       38 2024-04-15 13:33:23.313669 w_render-0.2.5/setup.cfg
+-rw-rw-r--   0 repente   (1000) repente   (1000)     3297 2024-04-15 13:31:13.000000 w_render-0.2.5/setup.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.313669 w_render-0.2.5/w_render.egg-info/
+-rw-r--r--   0 repente   (1000) repente   (1000)      993 2024-04-15 13:33:23.000000 w_render-0.2.5/w_render.egg-info/PKG-INFO
+-rw-rw-r--   0 repente   (1000) repente   (1000)      790 2024-04-15 13:33:23.000000 w_render-0.2.5/w_render.egg-info/SOURCES.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)        1 2024-04-15 13:33:23.000000 w_render-0.2.5/w_render.egg-info/dependency_links.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)      158 2024-04-15 13:33:23.000000 w_render-0.2.5/w_render.egg-info/entry_points.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       80 2024-04-15 13:33:23.000000 w_render-0.2.5/w_render.egg-info/requires.txt
+-rw-rw-r--   0 repente   (1000) repente   (1000)       11 2024-04-15 13:33:23.000000 w_render-0.2.5/w_render.egg-info/top_level.txt
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.205672 w_render-0.2.5/web_render/
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.229671 w_render-0.2.5/web_render/base/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:27:26.000000 w_render-0.2.5/web_render/base/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     2337 2023-09-03 20:30:16.000000 w_render-0.2.5/web_render/base/__main__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     8874 2024-04-15 13:25:12.000000 w_render-0.2.5/web_render/base/abstract.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1125 2023-08-24 07:40:40.000000 w_render-0.2.5/web_render/base/client.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1730 2024-04-15 13:30:29.000000 w_render-0.2.5/web_render/base/extends.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     4320 2023-08-24 21:59:25.000000 w_render-0.2.5/web_render/base/server.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     4107 2024-04-15 13:30:00.000000 w_render-0.2.5/web_render/base/test_webrender.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1508 2023-08-24 07:24:47.000000 w_render-0.2.5/web_render/config.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.229671 w_render-0.2.5/web_render/flask/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-07-28 09:55:28.000000 w_render-0.2.5/web_render/flask/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1817 2023-08-28 08:31:02.000000 w_render-0.2.5/web_render/flask/__main__.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.241670 w_render-0.2.5/web_render/flask/core/
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.273670 w_render-0.2.5/web_render/flask/core/main/
+-rw-rw-r--   0 repente   (1000) repente   (1000)      837 2023-08-24 07:40:41.000000 w_render-0.2.5/web_render/flask/core/main/view.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.305669 w_render-0.2.5/web_render/flask/core/render_api/
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1372 2023-08-24 07:40:41.000000 w_render-0.2.5/web_render/flask/core/render_api/logic.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1075 2023-08-24 07:24:47.000000 w_render-0.2.5/web_render/flask/core/render_api/view.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      207 2023-08-24 07:24:47.000000 w_render-0.2.5/web_render/flask/core/routing.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.313669 w_render-0.2.5/web_render/flask/core/service/
+-rw-rw-r--   0 repente   (1000) repente   (1000)      389 2023-08-24 07:24:47.000000 w_render-0.2.5/web_render/flask/core/service/interface.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)      377 2023-08-24 07:24:47.000000 w_render-0.2.5/web_render/interface.py
+drwxrwxr-x   0 repente   (1000) repente   (1000)        0 2024-04-15 13:33:23.313669 w_render-0.2.5/web_render/script/
+-rw-rw-r--   0 repente   (1000) repente   (1000)        0 2023-08-24 07:28:05.000000 w_render-0.2.5/web_render/script/__init__.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1507 2023-08-24 08:38:56.000000 w_render-0.2.5/web_render/script/render_server.py
+-rw-rw-r--   0 repente   (1000) repente   (1000)     1498 2023-08-24 12:59:54.000000 w_render-0.2.5/web_render/tool.py
```

### Comparing `w_render-0.2.4/PKG-INFO` & `w_render-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w-render
-Version: 0.2.4
+Version: 0.2.5
 Summary: Render a dynamical sites.
 Author: Andrey Plugin
 Author-email: 9keepa@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `w_render-0.2.4/README.md` & `w_render-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/setup.py` & `w_render-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     long_description = fh.read()
 
 # Функция, которая принимает несколько аргументов. Она присваивает эти значения пакету.
 setup(
     # Имя дистрибутива пакета. Оно должно быть уникальным, поэтому добавление вашего имени пользователя в конце является обычным делом.
     name="w-render",
     # Номер версии вашего пакета. Обычно используется семантическое управление версиями.
-    version="0.2.4",
+    version="0.2.5",
     # Имя автора.
     author="Andrey Plugin",
     # Его почта.
     author_email="9keepa@gmail.com",
     # Краткое описание, которое будет показано на странице PyPi.
     description="Render a dynamical sites.",
     # Длинное описание, которое будет отображаться на странице PyPi. Использует README.md репозитория для заполнения.
```

### Comparing `w_render-0.2.4/w_render.egg-info/PKG-INFO` & `w_render-0.2.5/w_render.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: w-render
-Version: 0.2.4
+Version: 0.2.5
 Summary: Render a dynamical sites.
 Author: Andrey Plugin
 Author-email: 9keepa@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `w_render-0.2.4/w_render.egg-info/SOURCES.txt` & `w_render-0.2.5/w_render.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 web_render/config.py
 web_render/interface.py
 web_render/tool.py
 web_render/base/__init__.py
 web_render/base/__main__.py
 web_render/base/abstract.py
 web_render/base/client.py
+web_render/base/extends.py
 web_render/base/server.py
 web_render/base/test_webrender.py
 web_render/flask/__init__.py
 web_render/flask/__main__.py
 web_render/flask/core/routing.py
 web_render/flask/core/main/view.py
 web_render/flask/core/render_api/logic.py
```

### Comparing `w_render-0.2.4/web_render/base/__main__.py` & `w_render-0.2.5/web_render/base/__main__.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/base/abstract.py` & `w_render-0.2.5/web_render/base/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from selenium.webdriver.chrome.options import Options
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.chrome.service import Service
 from web_render.tool import log
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.support.wait import WebDriverWait
+from .extends import auth_http_proxy
 import undetected_chromedriver as uc
 import platform
 import subprocess
 
 
 logger = log(__name__)
 
@@ -136,14 +137,19 @@
         logger.info(f"Close {self.browser}")
 
 
 def make_selenium_webdriver(config: Dict):
     co = Options()
     if config.get("PROXY_SERVER"):
         co.add_argument(f"--proxy-server={config['PROXY_SERVER']}")
+    if config.get("AUTH_PROXY_SERVER"):
+        ip, auth = config.get("AUTH_PROXY_SERVER").strip().split("@")
+        host, port = ip.split(":")
+        login, pwd = auth.split(":")
+        co.add_encoded_extension(auth_http_proxy(host, port, login, pwd))
     if config.get('HEADLESS'):
         co.add_argument('--headless=new')
 
     co.add_argument('--disable-blink-features=AutomationControlled')
     co.add_argument('--no-sandbox')
     co.add_argument('--disable-dev-shm-usage')
     co.add_argument("start-maximized")
```

### Comparing `w_render-0.2.4/web_render/base/client.py` & `w_render-0.2.5/web_render/base/client.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/base/server.py` & `w_render-0.2.5/web_render/base/server.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/base/test_webrender.py` & `w_render-0.2.5/web_render/base/test_webrender.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,28 +8,28 @@
 from functools import partial
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import TimeoutException
 logging.disable(logging.WARNING)
 # import sys
 # sys.stderr = open("test_error.log", 'a')
 
-CHROME_DRIVER_VERSION = "116.0.5845.110"
+CHROME_DRIVER_VERSION = "123.0.6312.105"
 
 class TestServices(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         cls.partial_browser = partial(make_selenium_webdriver)
 
     def setUp(self):
         pass
 
     def test_01(self):
         with SeleniumRender(self.partial_browser({"CHROME_DRIVER_VERSION":CHROME_DRIVER_VERSION})) as render:
-            render.set_url("https://ya.ru/")
+            render.set_url("https://2ip.ru")
             self.assertTrue(len(render.browser.find_elements(By.CSS_SELECTOR, 'script')))
 
     def test_02(self):
         with SeleniumRender(self.partial_browser({"CHROME_DRIVER_VERSION":CHROME_DRIVER_VERSION})) as render:
             render.set_url("https://www.ozon.ru/category/smartfony-15502/", web_wait={
                     "name": "CheckNumberElementsInPage",
                     "params": {
@@ -52,15 +52,15 @@
                 )
 
 
     def test_03_undetected(self):
         with SeleniumRender(self.partial_browser({
             "CHROME_DRIVER_VERSION":CHROME_DRIVER_VERSION,
             "UNDETECTED_CHROMEDRIVER": True,
-            "HEADLESS": True
+            "HEADLESS": False
         })) as render:
             render.set_url("https://www.ozon.ru/category/smartfony-15502/", web_wait={
                     "name": "CheckNumberElementsInPage",
                     "params": {
                         "selector":"[data-widget=searchResultsV2] a.tile-hover-target[data-prerender]",
                         "count": 30
                     }
@@ -74,16 +74,24 @@
                         "selector":"[data-widget=searchResultsV2] a.tile-hover-target[data-prerender]",
                         "count": 30
                     }
                 }
             )
             self.assertTrue(30<=len(render.browser.find_elements(By.CSS_SELECTOR, "[data-widget=searchResultsV2] a.tile-hover-target[data-prerender]")))
 
+    def test_04(self):
 
-
+        auth_proxy = "168.196.237.197:9183@DbMPBg:PE5xjW"
+        with SeleniumRender(self.partial_browser({
+            "CHROME_DRIVER_VERSION":CHROME_DRIVER_VERSION,
+            "AUTH_PROXY_SERVER": auth_proxy
+        })) as render:
+            render.set_url("https://2ip.ru")
+            res = render.browser.find_element(By.CSS_SELECTOR, "#d_clip_button span").text
+            self.assertTrue(res in auth_proxy)
 
     @classmethod
     def tearDownClass(cls):
         pass
 
 def suite():
     suite = unittest.TestSuite()
```

### Comparing `w_render-0.2.4/web_render/config.py` & `w_render-0.2.5/web_render/config.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/flask/__main__.py` & `w_render-0.2.5/web_render/flask/__main__.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/flask/core/main/view.py` & `w_render-0.2.5/web_render/flask/core/main/view.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/flask/core/render_api/logic.py` & `w_render-0.2.5/web_render/flask/core/render_api/logic.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/flask/core/render_api/view.py` & `w_render-0.2.5/web_render/flask/core/render_api/view.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/script/render_server.py` & `w_render-0.2.5/web_render/script/render_server.py`

 * *Files identical despite different names*

### Comparing `w_render-0.2.4/web_render/tool.py` & `w_render-0.2.5/web_render/tool.py`

 * *Files identical despite different names*

