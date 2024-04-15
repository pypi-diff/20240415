# Comparing `tmp/botasaurus2-1.4.0.tar.gz` & `tmp/botasaurus2-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.4.0.tar", max compression
+gzip compressed data, was "botasaurus2-1.4.1.tar", max compression
```

## Comparing `botasaurus2-1.4.0.tar` & `botasaurus2-1.4.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.0/README.md
--rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.4.0/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57375 2024-04-14 12:45:15.716616 botasaurus2-1.4.0/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.0/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.0/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.0/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.0/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.0/botasaurus/constants.py
--rw-r--r--   0        0        0    15399 2024-04-15 14:47:35.316830 botasaurus2-1.4.0/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12478 2024-04-14 12:58:38.479280 botasaurus2-1.4.0/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    39191 2024-04-15 14:48:04.476281 botasaurus2-1.4.0/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.0/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.0/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.0/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.0/botasaurus/output.py
--rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.0/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.0/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.0/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.0/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-04-15 14:58:49.766049 botasaurus2-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.1/README.md
+-rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.1/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.1/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.1/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.1/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.1/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.1/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.1/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.1/botasaurus/constants.py
+-rw-r--r--   0        0        0    15646 2024-04-15 20:14:57.124256 botasaurus2-1.4.1/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12609 2024-04-15 20:12:50.183439 botasaurus2-1.4.1/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    39245 2024-04-15 20:00:38.392226 botasaurus2-1.4.1/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.1/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.1/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.1/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.1/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.1/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.1/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.1/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.1/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.1/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-15 20:20:58.710065 botasaurus2-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.1/PKG-INFO
```

### Comparing `botasaurus2-1.4.0/LICENSE` & `botasaurus2-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/README.md` & `botasaurus2-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/__init__.py` & `botasaurus2-1.4.1/botasaurus/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from .decorators import RetryException,browser, request, AsyncQueueResult, AsyncResult
 from .anti_detect_driver import AntiDetectDriver
+from .anti_detect_driver import AntiDetectDriverRemote
 from .anti_detect_requests import AntiDetectRequests
 import botasaurus.bt as bt
 
 logger = logging.getLogger()
 logger.setLevel(logging.DEBUG)
 console_handler = logging.StreamHandler()
 console_handler.setLevel(logging.DEBUG)
```

### Comparing `botasaurus2-1.4.0/botasaurus/accept_google_cookies.py` & `botasaurus2-1.4.1/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/anti_detect_driver.py` & `botasaurus2-1.4.1/botasaurus/anti_detect_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webdriver import WebDriver
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.remote.webdriver import WebDriver
+from selenium.webdriver.remote.command import Command
 from selenium.common.exceptions import (
     StaleElementReferenceException,
     JavascriptException,
     NoSuchElementException,
     NoSuchWindowException,
     TimeoutException,
 )
@@ -1725,14 +1726,28 @@
                 EC.frame_to_be_available_and_switch_to_it(
                     (by, value)
                 )
             )
         except TimeoutException as err:
             logger.error(err)
 
-class AntiDetectDriverRemote(WebDriver):
+class AntiDetectDriverRemote(AntiDetectDriver, WebDriver):
     def __init__(self, *args, **kwargs):
         self.about: AboutBrowser = None
         self.is_network_enabled = False
         self.close_proxy = False
         self.timeout = 12
         WebDriver.__init__(self, *args, **kwargs)
+
+    def quit(self,):
+        """Quits the driver and closes every associated window.
+
+        :Usage:
+            ::
+
+                driver.quit()
+        """
+        try:
+            self.execute(Command.QUIT)
+        finally:
+            self.stop_client()
+            self.command_executor.close()
```

### Comparing `botasaurus2-1.4.0/botasaurus/anti_detect_requests.py` & `botasaurus2-1.4.1/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/base_data.py` & `botasaurus2-1.4.1/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/beep_utils.py` & `botasaurus2-1.4.1/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/botasaurus_storage.py` & `botasaurus2-1.4.1/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/bt.py` & `botasaurus2-1.4.1/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/cache.py` & `botasaurus2-1.4.1/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.4.1/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/captcha.py` & `botasaurus2-1.4.1/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/check_and_download_driver.py` & `botasaurus2-1.4.1/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/cl.py` & `botasaurus2-1.4.1/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/close.py` & `botasaurus2-1.4.1/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/create_driver_utils.py` & `botasaurus2-1.4.1/botasaurus/create_driver_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from time import sleep
 import os
+import logging
+from time import sleep
 from sys import argv
 from shutil import rmtree
 from pathlib import Path
 
 import selenium
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
@@ -16,14 +17,17 @@
 from .user_agent import UserAgent, UserAgentInstance
 from .utils import get_current_profile_path,  read_json, relative_path, silentremove, write_json
 from .window_size import WindowSize, WindowSizeInstance
 
 DEFAULT_BLOCKED_RESOURCES = ['.css', '.jpg', '.jpeg', '.png', '.svg', '.gif', '.woff', '.pdf', '.zip']
 DEFAULT_BLOCKED_RESOURCES_EXCEPT_CSS = ['.jpg', '.jpeg', '.png', '.svg', '.gif', '.woff', '.pdf', '.zip']
 
+logger = logging.getLogger('standard')
+
+
 def get_eager_strategy():
     caps = DesiredCapabilities().CHROME
     caps["pageLoadStrategy"] = "none"   # Do not wait for full page load
     return caps
 
 
 def delete_cache(driver):
@@ -37,16 +41,16 @@
 def add_useragent(options, user_agent):
     if user_agent:
         options.add_argument(f'--user-agent={user_agent}')
 
 
 def create_profile_path(user_id, base_dir='.'):
     PROFILES_PATH = 'profiles'
-    PATH = Path(base_dir) / f'{PROFILES_PATH}/{user_id}'
-    path = relative_path(PATH, 0)
+    path = Path(base_dir) / f'{PROFILES_PATH}/{user_id}'
+    # path = relative_path(path, 0)
     return path
 
 
 def delete_corrupted_files(user_id):
     is_success = silentremove(
         f'{create_profile_path(user_id)}/SingletonCookie')
     silentremove(f'{create_profile_path(user_id)}/SingletonSocket')
@@ -102,18 +106,19 @@
 
         add_useragent(options, user_agent)
 
     has_user = profile is not None
 
     if has_user:
         path = create_profile_path(profile, base_dir=base_dir)
-        user_data_path = f"--user-data-dir={path}"
+        logger.debug(path)
+        user_data_path = f"--user-data-dir=/{path}"
         options.add_argument(user_data_path)
 
-    return {"window_size": window_size, "user_agent": user_agent, "profile": profile}
+    return options, {"window_size": window_size, "user_agent": user_agent, "profile": profile}
 
 def hide_automation_bar(options):
     options.add_argument('--disable-blink-features=AutomationControlled')
     # options.add_argument("--disable-blink-features")
 
     options.add_experimental_option(
         "excludeSwitches", ["enable-automation"])
@@ -236,28 +241,31 @@
                            attempt_download=True,
                            remote=False):
 
     try:
         if desired_capabilities:
             for name, value in desired_capabilities.items():
                 options.set_capability(name, value)
+        if remote:
+            logger.debug(desired_capabilities)
+            logger.debug(options.to_capabilities())
+            logger.debug(options.arguments)
+            return AntiDetectDriverRemote(
+                command_executor="http://localhost:4444/wd/hub",
+                options=options
+            )
         path = relative_path(get_driver_path(), 0)
         if selenium.__version__ == '4.5.0':
             driver = AntiDetectDriver(
                 desired_capabilities=desired_capabilities,
                 chrome_options=options,
                 executable_path=path,
             )
             return driver
         service = ChromeService(executable_path=path)
-        if remote:
-            return AntiDetectDriverRemote(
-                command_executor="http://localhost:4444/wd/hub",
-                options=options
-            )
         return AntiDetectDriver(options=options, service=service)
         
     except SessionNotCreatedException as e:
         if "This version of ChromeDriver only supports Chrome version" in str(e) and attempt_download:
             # Handle the specific case where ChromeDriver version is not compatible
             do_download_driver()
             # Retry creating the Selenium driver once more
@@ -294,15 +302,15 @@
         else:
             if headless:
                 options.add_argument('--headless=new')
 
         if lang is not None:
             options.add_argument(f'--lang={lang}')
 
-        driver_attributes = add_essential_options(
+        options, driver_attributes = add_essential_options(
             options, None if tiny_profile else profile, window_size, user_agent, base_dir=base_dir)
         
         hide_automation_bar(options)
 
         # Necessary Options
         # options.add_argument("--ignore-certificate-errors")
         # options.add_argument("--disable-extensions")
```

### Comparing `botasaurus2-1.4.0/botasaurus/create_stealth_driver.py` & `botasaurus2-1.4.1/botasaurus/create_stealth_driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-from javascript_fixes.errors import JavaScriptError
+import logging
 from sys import argv
+from javascript_fixes.errors import JavaScriptError
 from .exceptions import CloudflareDetection
 from .check_and_download_driver import check_and_download_driver
 from typing import Callable, Any, Optional, Union
 from .opponent import Opponent
 from .anti_detect_driver import AntiDetectDriver
 from time import sleep, time
 from .chrome_launcher_adapter import ChromeLauncherAdapter
 from .create_driver_utils import create_selenium_driver, do_create_driver_with_custom_driver_creator
 from selenium.webdriver.chrome.options import Options
 import subprocess
 from os import name
 
+logger = logging.getLogger('standard')
+
+
 def kill_process_by_pid(pid):
     if pid is None:
         raise ValueError("A PID must be provided")
     try:
         if name == 'nt':
             subprocess.run(['taskkill', '/PID', str(pid), '/F'], check=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         else:  # macOS and Linux share the same command for killing a process by PID
@@ -246,29 +250,30 @@
             return launch_chrome(start_url, options._arguments)
         raise
 
 def do_create_stealth_driver(data, options, desired_capabilities, start_url, wait,  raise_exception,add_arguments, remote: bool = False):
     options = clean_options(options)
     if add_arguments:
         add_arguments(data, options)
-    remote_driver_options = Options()
-    
+    remote_driver_options = options
     if not remote:
+        remote_driver_options = Options()
         chrome = launch_server_safe_chrome(options, start_url)
         debug_port = chrome.port
 
         should_wait = start_url and wait
         if should_wait:
                 print(f"Waiting {wait} seconds before connecting to Chrome...")
                 sleep(wait)
 
 
         remote_driver_options.add_experimental_option(
             "debuggerAddress", f"127.0.0.1:{debug_port}"
         )
+    logger.debug(remote_driver_options)
     remote_driver = create_selenium_driver(remote_driver_options, desired_capabilities, remote=remote)
     if not remote:
         pid = chrome.pid
 
         remote_driver.kill_chrome_by_pid = lambda: kill_process_by_pid(pid)
 
         if not should_wait:
```

### Comparing `botasaurus2-1.4.0/botasaurus/creators.py` & `botasaurus2-1.4.1/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/decorator_helpers.py` & `botasaurus2-1.4.1/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/decorators.py` & `botasaurus2-1.4.1/botasaurus/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+import os
+import sys
+import logging
+from datetime import datetime
+from time import sleep
+from pathlib import Path
 from joblib import Parallel, delayed
 from selenium.webdriver.chrome.options import Options
 from selenium.common.exceptions import WebDriverException
 from functools import wraps
 from queue import Queue
 from threading import Thread
 from traceback import print_exc, format_exc
 from typing import Any, Callable, Optional, Union, List
-import os
-import sys
-from datetime import datetime
-from time import sleep
-from pathlib import Path
 from .exceptions import CloudflareDetection
 
 from .check_and_download_driver import check_and_download_driver
 
 from .utils import is_errors_instance, write_file
 
 from .formats import Formats
@@ -51,14 +52,17 @@
 # from .local_storage import LocalStorage
 from .local_storage import LocalStorageClass
 from .profile import ProfileClass
 from .usage import Usage
 from .list_utils import flatten
 
 
+logger = logging.getLogger('standard')
+
+
 class RetryException(Exception):
     pass
 
 
 def get_driver_url_safe(driver):
     try:
         return driver.current_url
@@ -488,17 +492,15 @@
                         evaluated_window_size,
                         evaluated_user_agent,
                         evaluated_proxy,
                         evaluated_headless,
                         evaluated_lang,
                         base_dir=local_storage_dir
                     )
-
                     update_options(data, options, add_arguments, extensions)
-
                     desired_capabilities = create_capabilities(
                         is_eager, capabilities
                     )
                     about = create_about(
                         evaluated_proxy,
                         evaluated_lang,
                         beep,
```

### Comparing `botasaurus2-1.4.0/botasaurus/download_driver.py` & `botasaurus2-1.4.1/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/get_chrome_version.py` & `botasaurus2-1.4.1/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/got_adapter.py` & `botasaurus2-1.4.1/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/ip_utils.py` & `botasaurus2-1.4.1/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/list_utils.py` & `botasaurus2-1.4.1/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/local_storage.py` & `botasaurus2-1.4.1/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/local_storage_driver.py` & `botasaurus2-1.4.1/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/output.py` & `botasaurus2-1.4.1/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/profile.py` & `botasaurus2-1.4.1/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/sitemap.py` & `botasaurus2-1.4.1/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/str_utils.py` & `botasaurus2-1.4.1/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/temp_mail.py` & `botasaurus2-1.4.1/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/user_agent.py` & `botasaurus2-1.4.1/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/user_generator.py` & `botasaurus2-1.4.1/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/utils.py` & `botasaurus2-1.4.1/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/botasaurus/window_size.py` & `botasaurus2-1.4.1/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.0/pyproject.toml` & `botasaurus2-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.4.0"
+version = "1.4.1"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
```

### Comparing `botasaurus2-1.4.0/PKG-INFO` & `botasaurus2-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.4.0
+Version: 1.4.1
 Summary: Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers.
 License: MIT
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.0 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.1 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

