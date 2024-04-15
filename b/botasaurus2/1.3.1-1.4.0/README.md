# Comparing `tmp/botasaurus2-1.3.1.tar.gz` & `tmp/botasaurus2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.3.1.tar", max compression
+gzip compressed data, was "botasaurus2-1.4.0.tar", max compression
```

## Comparing `botasaurus2-1.3.1.tar` & `botasaurus2-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.3.1/README.md
--rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.3.1/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57375 2024-04-14 12:45:15.716616 botasaurus2-1.3.1/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.3.1/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.3.1/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.3.1/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.3.1/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.3.1/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.3.1/botasaurus/constants.py
--rw-r--r--   0        0        0    15143 2024-04-14 12:45:15.716616 botasaurus2-1.3.1/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12338 2024-04-11 15:00:22.756112 botasaurus2-1.3.1/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    39088 2024-04-14 10:41:23.389902 botasaurus2-1.3.1/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.3.1/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.3.1/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.3.1/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.3.1/botasaurus/output.py
--rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.3.1/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.3.1/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.3.1/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8520 2024-03-19 20:47:06.020789 botasaurus2-1.3.1/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.3.1/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-04-14 12:45:15.716616 botasaurus2-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.0/README.md
+-rw-r--r--   0        0        0      799 2024-03-19 20:47:06.016789 botasaurus2-1.4.0/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57375 2024-04-14 12:45:15.716616 botasaurus2-1.4.0/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.0/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.0/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.0/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.0/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.0/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.0/botasaurus/constants.py
+-rw-r--r--   0        0        0    15399 2024-04-15 14:47:35.316830 botasaurus2-1.4.0/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12478 2024-04-14 12:58:38.479280 botasaurus2-1.4.0/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    39191 2024-04-15 14:48:04.476281 botasaurus2-1.4.0/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.0/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.0/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.0/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.0/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.0/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.0/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.0/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.0/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.0/botasaurus/window_size.py
+-rw-r--r--   0        0        0      848 2024-04-15 14:58:49.766049 botasaurus2-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.0/PKG-INFO
```

### Comparing `botasaurus2-1.3.1/LICENSE` & `botasaurus2-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/README.md` & `botasaurus2-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/__init__.py` & `botasaurus2-1.4.0/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/accept_google_cookies.py` & `botasaurus2-1.4.0/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/anti_detect_driver.py` & `botasaurus2-1.4.0/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/anti_detect_requests.py` & `botasaurus2-1.4.0/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/base_data.py` & `botasaurus2-1.4.0/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/beep_utils.py` & `botasaurus2-1.4.0/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/botasaurus_storage.py` & `botasaurus2-1.4.0/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/bt.py` & `botasaurus2-1.4.0/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/cache.py` & `botasaurus2-1.4.0/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.4.0/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/captcha.py` & `botasaurus2-1.4.0/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/check_and_download_driver.py` & `botasaurus2-1.4.0/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/cl.py` & `botasaurus2-1.4.0/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/close.py` & `botasaurus2-1.4.0/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/create_driver_utils.py` & `botasaurus2-1.4.0/botasaurus/create_driver_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from time import sleep
 import os
 from sys import argv
 from shutil import rmtree
+from pathlib import Path
 
 import selenium
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver.chrome.service import Service as ChromeService
 from selenium.common.exceptions import SessionNotCreatedException
 
@@ -34,17 +35,17 @@
         cmd='Network.clearBrowserCache', params={}))
 
 def add_useragent(options, user_agent):
     if user_agent:
         options.add_argument(f'--user-agent={user_agent}')
 
 
-def create_profile_path(user_id):
+def create_profile_path(user_id, base_dir='.'):
     PROFILES_PATH = 'profiles'
-    PATH = f'{PROFILES_PATH}/{user_id}'
+    PATH = Path(base_dir) / f'{PROFILES_PATH}/{user_id}'
     path = relative_path(PATH, 0)
     return path
 
 
 def delete_corrupted_files(user_id):
     is_success = silentremove(
         f'{create_profile_path(user_id)}/SingletonCookie')
@@ -59,15 +60,15 @@
 
 def delete_profile_path(user_id):
     path = create_profile_path(user_id)
     rmtree(path, ignore_errors=True)
 
 
 
-def add_essential_options(options, profile, window_size, user_agent):
+def add_essential_options(options, profile, window_size, user_agent, base_dir='.'):
     options.add_argument("--start-maximized")
     if window_size != WindowSize.REAL:
         if window_size == None:
             if profile == None:
                 window_size = WindowSizeInstance.get_random()
             else:
                 window_size = WindowSizeInstance.get_hashed(profile)
@@ -100,15 +101,15 @@
                 user_agent = user_agent
 
         add_useragent(options, user_agent)
 
     has_user = profile is not None
 
     if has_user:
-        path = create_profile_path(profile)
+        path = create_profile_path(profile, base_dir=base_dir)
         user_data_path = f"--user-data-dir={path}"
         options.add_argument(user_data_path)
 
     return {"window_size": window_size, "user_agent": user_agent, "profile": profile}
 
 def hide_automation_bar(options):
     options.add_argument('--disable-blink-features=AutomationControlled')
@@ -169,36 +170,36 @@
         driver_download_state = DOWNLOADED
 
 # def do_download_driver():
     
 #     from .download_driver import download_driver
 #     download_driver()
 
-def save_cookies(driver, profile):
-            current_profile_data = get_current_profile_path(profile) + 'profile.json'
+def save_cookies(driver, profile, base_dir='.'):
+            current_profile_data = Path(base_dir) / get_current_profile_path(profile) + 'profile.json'
             current_profile_data_path =  relative_path(current_profile_data, 0)
 
             driver._enable_network()
             # execute_cdp_cmd('Network.enable', {})
             cookies = (driver.execute_cdp_cmd('Network.getAllCookies', {}))
             # driver.execute_cdp_cmd('Network.disable', {})
 
             if type(cookies) is not list:
                 cookies = cookies.get('cookies')
             write_json(cookies, current_profile_data_path)
 
 
-def load_cookies(driver: AntiDetectDriver, profile):
-    current_profile = get_current_profile_path(profile)
+def load_cookies(driver: AntiDetectDriver, profile, base_dir='.'):
+    current_profile = Path(base_dir) / get_current_profile_path(profile)
     current_profile_path = relative_path(current_profile, 0)
 
     if not os.path.exists(current_profile_path):
         os.makedirs(current_profile_path)
 
-    current_profile_data = get_current_profile_path(profile) + 'profile.json'
+    current_profile_data = Path(base_dir) / get_current_profile_path(profile) + 'profile.json'
     current_profile_data_path = relative_path(current_profile_data, 0)
 
     if not os.path.isfile(current_profile_data_path):
         return
 
     cookies = read_json(current_profile_data_path)
     # Enables network tracking so we may use Network.setCookie method
@@ -272,15 +273,15 @@
             raise
 
 
 def create_about(proxy, lang, beep, driver_attributes,):
     about = AboutBrowser(window_size=driver_attributes.get('window_size'), user_agent=driver_attributes.get('user_agent'), profile=driver_attributes.get('profile'),proxy=proxy, lang=lang, beep=beep, is_new=True)
     return about
 
-def create_options_and_driver_attributes_and_close_proxy(tiny_profile, profile, window_size, user_agent, proxy,  headless, lang):
+def create_options_and_driver_attributes_and_close_proxy(tiny_profile, profile, window_size, user_agent, proxy,  headless, lang, base_dir='.'):
         if tiny_profile and profile is None:
             raise Exception('Profile must be given when using tiny profile')
 
         options = Options()
 
         if is_gitpod_environment():
             # todo: Maybe need to add check to see running in ec2/gcp then I need to also add this or we can make this an error based option add on
@@ -294,15 +295,15 @@
             if headless:
                 options.add_argument('--headless=new')
 
         if lang is not None:
             options.add_argument(f'--lang={lang}')
 
         driver_attributes = add_essential_options(
-            options, None if tiny_profile else profile, window_size, user_agent)
+            options, None if tiny_profile else profile, window_size, user_agent, base_dir=base_dir)
         
         hide_automation_bar(options)
 
         # Necessary Options
         # options.add_argument("--ignore-certificate-errors")
         # options.add_argument("--disable-extensions")
 
@@ -349,17 +350,17 @@
 
         if default_patterns:
             default_patterns = list(dict.fromkeys(default_patterns))
             driver._enable_network()  # Assuming this method is correctly defined in the driver
             driver.execute_cdp_cmd('Network.setBlockedURLs', {"urls": default_patterns})
 
 
-def do_create_driver(tiny_profile, profile, window_size, user_agent, proxy, is_eager, headless, lang, block_resources, block_images, beep) -> AntiDetectDriver:
+def do_create_driver(tiny_profile, profile, window_size, user_agent, proxy, is_eager, headless, lang, block_resources, block_images, beep, base_dir='.') -> AntiDetectDriver:
 
-        options, driver_attributes, close_proxy = create_options_and_driver_attributes_and_close_proxy(tiny_profile, profile, window_size, user_agent, proxy, headless, lang,)
+        options, driver_attributes, close_proxy = create_options_and_driver_attributes_and_close_proxy(tiny_profile, profile, window_size, user_agent, proxy, headless, lang, base_dir)
         desired_capabilities  = create_capabilities(is_eager)
 
         driver = create_selenium_driver(options, desired_capabilities)
 
         driver.about = create_about(proxy, lang, beep, driver_attributes,  )
 
         if tiny_profile:
@@ -368,17 +369,17 @@
         block_resources_if_should(driver, block_resources, block_images)
 
         if close_proxy:
             driver.close_proxy = close_proxy
 
         return driver
 
-def do_create_driver_with_custom_driver_creator(tiny_profile, profile, window_size, user_agent, proxy, is_eager, headless, lang, block_resources, block_images, beep, create_driver) -> AntiDetectDriver:
+def do_create_driver_with_custom_driver_creator(tiny_profile, profile, window_size, user_agent, proxy, is_eager, headless, lang, block_resources, block_images, beep, create_driver, base_dir='.') -> AntiDetectDriver:
 
-        options, driver_attributes, close_proxy = create_options_and_driver_attributes_and_close_proxy(tiny_profile, profile, window_size, user_agent, proxy, headless, lang,)
+        options, driver_attributes, close_proxy = create_options_and_driver_attributes_and_close_proxy(tiny_profile, profile, window_size, user_agent, proxy, headless, lang, base_dir=base_dir)
         desired_capabilities  = create_capabilities(is_eager)
 
         driver = create_driver(options, desired_capabilities)
         # create_selenium_driver(options, desired_capabilities)
 
         driver.about = create_about(proxy, lang, beep, driver_attributes,  )
```

### Comparing `botasaurus2-1.3.1/botasaurus/create_stealth_driver.py` & `botasaurus2-1.4.0/botasaurus/create_stealth_driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,50 +245,52 @@
             print("Chrome failed to launch. Retrying with additional server options. To add server options by default, include '--server' in your launch command.")
             return launch_chrome(start_url, options._arguments)
         raise
 
 def do_create_stealth_driver(data, options, desired_capabilities, start_url, wait,  raise_exception,add_arguments, remote: bool = False):
     options = clean_options(options)
     if add_arguments:
-      add_arguments(data, options)
+        add_arguments(data, options)
+    remote_driver_options = Options()
     
-    chrome = launch_server_safe_chrome(options, start_url)
-    debug_port = chrome.port
-
-    should_wait = start_url and wait
-    if should_wait:
-            print(f"Waiting {wait} seconds before connecting to Chrome...")
-            sleep(wait)
+    if not remote:
+        chrome = launch_server_safe_chrome(options, start_url)
+        debug_port = chrome.port
+
+        should_wait = start_url and wait
+        if should_wait:
+                print(f"Waiting {wait} seconds before connecting to Chrome...")
+                sleep(wait)
 
-    remote_driver_options = Options()
 
-    remote_driver_options.add_experimental_option(
-        "debuggerAddress", f"127.0.0.1:{debug_port}"
-    )
+        remote_driver_options.add_experimental_option(
+            "debuggerAddress", f"127.0.0.1:{debug_port}"
+        )
     remote_driver = create_selenium_driver(remote_driver_options, desired_capabilities, remote=remote)
-    pid = chrome.pid
+    if not remote:
+        pid = chrome.pid
 
-    remote_driver.kill_chrome_by_pid = lambda: kill_process_by_pid(pid)
+        remote_driver.kill_chrome_by_pid = lambda: kill_process_by_pid(pid)
 
-    if not should_wait:
-            sleep(1) # Still do some wait to prevent exceptions
+        if not should_wait:
+                sleep(1) # Still do some wait to prevent exceptions
 
-    # input('after create')
-    try:
-        if start_url:
-            bypass_detection(remote_driver, raise_exception)
-    except CloudflareDetection as e:
-        
+        # input('after create')
         try:
-            remote_driver.close()
-            remote_driver.quit()
-        except:
-            pass
+            if start_url:
+                bypass_detection(remote_driver, raise_exception)
+        except CloudflareDetection as e:
+            
+            try:
+                remote_driver.close()
+                remote_driver.quit()
+            except:
+                pass
 
-        raise e
+            raise e
 
 
     return remote_driver
 
 
 def create_stealth_driver(start_url:Optional[Union[Callable[[Any], str], str]]="NONE", wait=8,
```

### Comparing `botasaurus2-1.3.1/botasaurus/creators.py` & `botasaurus2-1.4.0/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/decorator_helpers.py` & `botasaurus2-1.4.0/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/decorators.py` & `botasaurus2-1.4.0/botasaurus/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -436,16 +436,16 @@
             raise_exception = kwargs.get("raise_exception", raise_exception)
             create_driver = kwargs.get("create_driver", create_driver)
             capabilities = kwargs.get("capabilities", capabilities)
             local_storage_dir = kwargs.get("local_storage_dir", local_storage_dir)
             remote = kwargs.get("remote", remote)
             
             local_storage = LocalStorageClass(local_storage_dir)
-            profile = ProfileClass(local_storage_dir)
-            Profile = profile  # TODO: alter thourghout this module
+            Profile = ProfileClass(local_storage_dir / Path('profiles'))
+            Profile.profile = profile
             fn_name = func.__name__
 
             if cache:
                 _create_cache_directory_if_not_exists(func)
 
             # # Pool to hold reusable drivers
             _driver_pool = wrapper_browser._driver_pool if keep_drivers_alive else []
@@ -486,14 +486,15 @@
                         tiny_profile,
                         evaluated_profile,
                         evaluated_window_size,
                         evaluated_user_agent,
                         evaluated_proxy,
                         evaluated_headless,
                         evaluated_lang,
+                        base_dir=local_storage_dir
                     )
 
                     update_options(data, options, add_arguments, extensions)
 
                     desired_capabilities = create_capabilities(
                         is_eager, capabilities
                     )
@@ -533,14 +534,15 @@
                                     tiny_profile,
                                     evaluated_profile,
                                     evaluated_window_size,
                                     evaluated_user_agent,
                                     evaluated_proxy,
                                     evaluated_headless,
                                     evaluated_lang,
+                                    base_dir=local_storage_dir
                                 )
                                 update_options(data, options, add_arguments, extensions)
                                 desired_capabilities = create_capabilities(is_eager)
                                 about = create_about(
                                     evaluated_proxy,
                                     evaluated_lang,
                                     beep,
```

### Comparing `botasaurus2-1.3.1/botasaurus/download_driver.py` & `botasaurus2-1.4.0/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/get_chrome_version.py` & `botasaurus2-1.4.0/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/got_adapter.py` & `botasaurus2-1.4.0/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/ip_utils.py` & `botasaurus2-1.4.0/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/list_utils.py` & `botasaurus2-1.4.0/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/local_storage.py` & `botasaurus2-1.4.0/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/local_storage_driver.py` & `botasaurus2-1.4.0/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/output.py` & `botasaurus2-1.4.0/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/profile.py` & `botasaurus2-1.4.0/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/sitemap.py` & `botasaurus2-1.4.0/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/str_utils.py` & `botasaurus2-1.4.0/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/temp_mail.py` & `botasaurus2-1.4.0/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/user_agent.py` & `botasaurus2-1.4.0/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/user_generator.py` & `botasaurus2-1.4.0/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/botasaurus/utils.py` & `botasaurus2-1.4.0/botasaurus/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 import traceback
 from datetime import datetime
 from http.client import RemoteDisconnected
 from time import sleep
 from urllib.error import ContentTooShortError, URLError
 from sys import platform, exit
+from pathlib import Path
 
 from selenium.webdriver.remote.webelement import WebElement
 
 from .list_utils import flatten_depth
 
 
 def is_errors_instance(instances, error):
@@ -28,14 +29,16 @@
     return platform == "linux" or platform == "linux2"
 
 def is_windows():
     return os.name == 'nt'
 
 def relative_path(path, goback=0):
     levels = [".."] * (goback + -1)
+    if isinstance(path, Path):
+        path = str(path.resolve())
     return os.path.abspath(os.path.join(os.getcwd(), *levels, path.strip()))
 
 def retry(func, retry_wait=None, retries=5):
     tries = 0
     while tries < retries:
         tries += 1
         try:
```

### Comparing `botasaurus2-1.3.1/botasaurus/window_size.py` & `botasaurus2-1.4.0/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.3.1/pyproject.toml` & `botasaurus2-1.4.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.3.1"
+version = "1.4.0"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
```

### Comparing `botasaurus2-1.3.1/PKG-INFO` & `botasaurus2-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.3.1
+Version: 1.4.0
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
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.3.1 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.0 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.5.0,<0.6.0)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
```

