# Comparing `tmp/linktest-2.4.3.tar.gz` & `tmp/linktest-2.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.4.3.tar", last modified: Sun Apr 14 16:24:48 2024, max compression
+gzip compressed data, was "linktest-2.4.4.tar", last modified: Mon Apr 15 03:13:47 2024, max compression
```

## Comparing `linktest-2.4.3.tar` & `linktest-2.4.4.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-14 16:24:48.519912 linktest-2.4.3/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-14 16:24:48.519662 linktest-2.4.3/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-14 16:24:48.510177 linktest-2.4.3/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-14 16:23:39.000000 linktest-2.4.3/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    15915 2024-04-12 11:05:25.000000 linktest-2.4.3/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4308 2024-04-14 16:16:30.000000 linktest-2.4.3/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37292 2024-04-12 14:18:40.000000 linktest-2.4.3/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10265 2024-04-09 02:55:29.000000 linktest-2.4.3/linktest/logged_requests copy.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104608 2024-04-12 14:06:49.000000 linktest-2.4.3/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7937 2024-04-12 10:48:42.000000 linktest-2.4.3/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-14 16:23:49.000000 linktest-2.4.3/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11013 2024-04-14 15:04:52.000000 linktest-2.4.3/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-11 08:19:05.000000 linktest-2.4.3/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-14 16:24:48.519264 linktest-2.4.3/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1304 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-14 16:24:48.000000 linktest-2.4.3/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-14 16:24:48.519958 linktest-2.4.3/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-14 16:24:42.000000 linktest-2.4.3/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-15 03:13:47.621563 linktest-2.4.4/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-15 03:13:47.620673 linktest-2.4.4/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-15 03:13:47.614783 linktest-2.4.4/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-04-15 03:04:10.000000 linktest-2.4.4/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10302 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9661 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7260 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16523 2024-04-15 03:08:44.000000 linktest-2.4.4/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4308 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    37292 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8745 2024-04-15 02:34:23.000000 linktest-2.4.4/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   104601 2024-04-15 03:00:01.000000 linktest-2.4.4/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4526 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1077 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1926 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8022 2024-04-15 02:53:30.000000 linktest-2.4.4/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-15 03:04:18.000000 linktest-2.4.4/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3055 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    11013 2024-04-15 02:56:41.000000 linktest-2.4.4/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-04-14 16:25:33.000000 linktest-2.4.4/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-04-15 03:13:47.618780 linktest-2.4.4/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-04-15 03:13:47.000000 linktest-2.4.4/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1271 2024-04-15 03:13:47.000000 linktest-2.4.4/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-04-15 03:13:47.000000 linktest-2.4.4/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-04-15 03:13:47.000000 linktest-2.4.4/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-04-15 03:13:47.000000 linktest-2.4.4/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-04-15 03:13:47.621728 linktest-2.4.4/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-04-15 03:13:41.000000 linktest-2.4.4/setup.py
```

### Comparing `linktest-2.4.3/linktest/appium_utils.py` & `linktest-2.4.4/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/auto_generate_testcase_list.py` & `linktest-2.4.4/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.4.4/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/base_testcase.py` & `linktest-2.4.4/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/clean_data.py` & `linktest-2.4.4/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/conver_xml_into_db.py` & `linktest-2.4.4/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/database_helper.py` & `linktest-2.4.4/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/date_utilities.py` & `linktest-2.4.4/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/doctor.py` & `linktest-2.4.4/linktest/doctor.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,30 +24,31 @@
 #  1. 
 #  2. Environment (test environment: UAT, QA, LIVE ...)
 #  3. TESTCASE_TIMEOUT (After Testcase_Timeout seconds, if the testcase still running then throw TimeoutException)
 #  4. RERUN_FLAG (control rerun failed testcases. Default is False)
 #  5. DEBUG_RUN (TESTCASE_TIMEOUT will be worked on this mode)
 #  6. QUEUE_SIZE (set queue_size as 8 means that there are at most 8 test cases can be executed concurrently)
 #  7. CLOSE_BROWSER (auto close the browser after UI Testcase's execution done)
-#  8. implicitly_wait which only used for webdriver(browser)
+#  8. WEBDRIVER_IMPLICIT_WAIT which only used for webdriver(browser)
 #  9. Configuration for Mobile Test ( update follow your business)
 #  10. APPIUM_SERVER_DEFAULT_IP = "127.0.0.1"
-#  11.APPIUM_SERVER_DEFAULT_PORT = 4723
-#  12.IOS_DESIRED_CAPABILITIES_IN_SETTINGS_FIRST
-#  13.ios_desired_capabilities
-#  14.ios_implicitly_wait
-#  15.android_apk_path
-#  16.customized_android_capabilities
-#  17.android_implicitly_wait
-#  18.DEVICE_ID_NAME_DICT
-#  19.ANDROID_TESTCASE_ACCOUNT
-#  20.# SaveScreenshotForPassedTestCaseFlag
+#  11. APPIUM_SERVER_DEFAULT_PORT = 4723
+#  12. IOS_DESIRED_CAPABILITIES_IN_SETTINGS_FIRST
+#  13. ios_desired_capabilities
+#  14. ios_implicitly_wait
+#  15. android_apk_path
+#  16. customized_android_capabilities
+#  17. android_implicitly_wait
+#  18. DEVICE_ID_NAME_DICT
+#  19. ANDROID_TESTCASE_ACCOUNT
+#  20. SAVE_SCREENSHOT_FOR_PASSED_TESTS
 #  21. Configuration for Browser option ( update follow your business)
 #  22. generate_xunit_result (default value is False)
-#  23. auto_download_chromedriver (default value is False)
+#  23. AUTO_DOWNLOAD_CHROMEDRIVER (default value is False)
+#  24. ALWAYS_GENERATE_CURL (default value is False)
 
 import logging
 
 # ------ testcase's log setting ------
 - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
 - LOG_LEVEL = logging.DEBUG # default value is DEBUG
 - LOG_TO_FILE = True # default value is True
@@ -74,21 +75,30 @@
 
 # set queue_size as 8 means that there are at most 8 test cases can be executed concurrently
 QUEUE_SIZE = 8
 
 # auto close browser after the testcase's execution done, Default value is True
 CLOSE_BROWSER = True
 
-# SaveScreenshotForPassedTestCaseFlag default value if False
-SaveScreenshotForPassedTestCaseFlag = False
+# Whether to save screenshots for passed test cases.
+# If set to True, screenshots will be saved for all test cases, including passed ones.
+# If set to False, screenshots will be saved only for failed test cases.
+# Default value is False.
+SAVE_SCREENSHOT_FOR_PASSED_TESTS = False
+
+# WebDriver implicit wait time in seconds.
+# It specifies the maximum time the WebDriver should wait for an element to be present before throwing an exception.
+# Default value is 20 seconds.
+WEBDRIVER_IMPLICIT_WAIT = 20
 
-# set the webdriver's implicitly_wait default value: 60
-implicitly_wait = 60
+# Whether to always generate a curl command for each test case regardless of its execution result (passed or failed). default value is False
+ALWAYS_GENERATE_CURL = False
 
-auto_download_chromedriver = False
+# auto download chromedriver, default value is False
+AUTO_DOWNLOAD_CHROMEDRIVER = False
 
 # configure for Database
 if ENVIRONMENT == Environment.UAT:
     DATABASE = {
         "Server": "uat-server",
         "User": "uat-user",
         "Password": "uat-password"
```

### Comparing `linktest-2.4.3/linktest/framework_log.py` & `linktest-2.4.4/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/generate_html_log.py` & `linktest-2.4.4/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/get_adb_devices.py` & `linktest-2.4.4/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/get_ios_devices_list.py` & `linktest-2.4.4/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/get_platform_info.py` & `linktest-2.4.4/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/get_project_info.py` & `linktest-2.4.4/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/html_report.py` & `linktest-2.4.4/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/logged_requests.py` & `linktest-2.4.4/linktest/logged_requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         @author: Wang Lin
         """
 
         def wrapper(*args, **kw):
             instance = args[0]  # 获取类实例引用
             res = func(*args, **kw)
 
-            if not hasattr(settings, "always_generate_curl") or settings.always_generate_curl is False:
+            if not hasattr(settings, "ALWAYS_GENERATE_CURL") or settings.ALWAYS_GENERATE_CURL is False:
                 if res.status_code == 200:
                     return res
 
             instance.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> cURL Start >>>>>>>>>>>>>>>>>>>>>>>>>")
             instance.logger.info(os.linesep + curlify.to_curl(res.request) + os.linesep)
             instance.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< cURL End <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
```

### Comparing `linktest-2.4.3/linktest/main.py` & `linktest-2.4.4/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 - Automatically re-runs failed test cases.
 - Generates HTML reports automatically (stored under project/output).
 - Allows setting individual timeouts for each test case, or utilizes settings.TESTCASE_TIMEOUT as the default.
 - Offers multiple test case execution methods (see details below).
 - Cross-platform compatibility (supports MacOS, Linux, Windows).
 - Supports DataSet (CSV) integration.
 - Support to specify the delimiter in CSV files.
-- Facilitates setting Authentication tokens for UI test cases.
+- Facilitates setting Authentication TOKEN for UI test cases.
 - Automatically installs the appropriate Chromedriver for UI test cases based on the Chrome version.
 - Allows saving execution logs into testdb, which can be integrated with linktest-dashboard to display execution log summaries, details, and histories.
 - Supports assigning multiple tags to a single test case for easy grouping.
 - Allows setting priorities for test cases, offering another way to group test cases.
 - Automatically store HTTP request and response data in the corresponding log file.
 - Easily and directly save specified data to the GlobalDataList between different test cases (useful for aggregation and summary functions).
 - integrate with test-engine-platform (easy to write the E2E testcases)
@@ -30,15 +30,15 @@
     - RERUN_FLAG (controls rerunning of failed test cases; default is False)
     - DEBUG_RUN (keeps the browser active after execution is done; default value is False)
     - Show_All_Chrome_Driver_Logs (determines whether to show all webdriver logs; default value is False)
     - QUEUE_SIZE (setting queue_size to 8, for example, means that a maximum of 8 test cases can be executed concurrently)
     - SAVE_LOG_TO_DB (saves execution logs into testdb; must be used in conjunction with linktest-dashboard)
     - generate_xunit_result (saves xunit report; default value is False; used for TestLink integration)
     - auto_log_request (default value is True; automatically logs request actions)
-    - auto_download_chromedriver (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
+    - AUTO_DOWNLOAD_CHROMEDRIVER (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
 
     # ------ Configuration Related to the TestCase's Log ------
     - LOG_FORMAT = '[%(asctime)s] %(levelname)-8s %(name)-12s %(message)s'
     - LOG_LEVEL = logging.DEBUG # default value is DEBUG
     - LOG_TO_FILE = True # default value is True
     - LOG_TO_CONSOLE = True # default value is True
 
@@ -215,15 +215,15 @@
     # here set timeout for testcase, otherwise this testcase's timeout will be : settings.TESTCASE_TIMEOUT
     timeout = 10
 
     def run_test(self):
         self.logger.debug("load mobile app")
         self.app_driver.launch_app()
 
------- Frontend/UI Testcase (with Token) demo ------:
+------ Frontend/UI Testcase (with TOKEN) demo ------:
 
 from linktest.ui_testcase import UITestCase
 
 class OrderListWithToken(UITestCase):
     tag = "order, tc9527"
 
     token = "token-xxx"
@@ -1121,16 +1121,16 @@
                                 if executing_testcase.ExecutionStatusSetByFramework == "failed":
                                     webdriver.save_screenshot(
                                         testcase_full_folder + os.sep + browser + "_" +
                                         executing_testcase.screenshot_name)
                                     executing_testcase.screenshot_path_list_for_db.append(
                                         testcase_full_folder + os.sep + browser + "_" +
                                         executing_testcase.screenshot_name)
-                                elif hasattr(settings, "SaveScreenshotForPassedTestCaseFlag"):
-                                    if settings.SaveScreenshotForPassedTestCaseFlag is True:
+                                elif hasattr(settings, "SAVE_SCREENSHOT_FOR_PASSED_TESTS"):
+                                    if settings.SAVE_SCREENSHOT_FOR_PASSED_TESTS is True:
                                         webdriver.save_screenshot(
                                             testcase_full_folder + os.sep + browser + "_" +
                                             executing_testcase.screenshot_name)
                                         executing_testcase.screenshot_path_list_for_db.append(
                                             testcase_full_folder + os.sep + browser + "_" +
                                             executing_testcase.screenshot_name)
```

### Comparing `linktest-2.4.3/linktest/memory_usage.py` & `linktest-2.4.4/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/re_func.py` & `linktest-2.4.4/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/run.py` & `linktest-2.4.4/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/run_testcase_thread.py` & `linktest-2.4.4/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/scp_report_to_specified_path.py` & `linktest-2.4.4/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/selenium_helper.py` & `linktest-2.4.4/linktest/selenium_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -133,33 +133,33 @@
 
         try:
             browser.maximize_window()
         except BaseException:
             traceback.print_exc()
 
         if SeleniumHelper.set_implicitly_wait_flag is False:
-            # user can set the "implicitly_wait" in settings.
-            # eg: implicitly_wait = 60
-            # if there are no implicitly_wait found in settings, then set a default value: 60 (in seconds)
-            if hasattr(settings, "implicitly_wait"):
-                if type(settings.implicitly_wait) == int or type(settings.implicitly_wait) == float:
-                    browser.implicitly_wait(settings.implicitly_wait)
-                    print("set implicitly_wait: %s" % settings.implicitly_wait)
+            # user can set the "WEBDRIVER_IMPLICIT_WAIT" in settings.
+            # eg: WEBDRIVER_IMPLICIT_WAIT = 60
+            # if there are no WEBDRIVER_IMPLICIT_WAIT found in settings, then set a default value: 20 (in seconds)
+            if hasattr(settings, "WEBDRIVER_IMPLICIT_WAIT"):
+                if type(settings.WEBDRIVER_IMPLICIT_WAIT) == int or type(settings.WEBDRIVER_IMPLICIT_WAIT) == float:
+                    browser.implicitly_wait(settings.WEBDRIVER_IMPLICIT_WAIT)
+                    print("set WEBDRIVER_IMPLICIT_WAIT: %s" % settings.WEBDRIVER_IMPLICIT_WAIT)
                 else:
-                    # if the type of settings.implicitly_wait is not correct, here set a default value: 60
-                    browser.implicitly_wait(60)
+                    # if the type of settings.WEBDRIVER_IMPLICIT_WAIT is not correct, here set a default value: 20
+                    browser.implicitly_wait(20)
                     print(
-                        "the type of implicitly_wait:%s is not 'int' or 'float', here set a default value: 60" % settings.implicitly_wait)
+                        "the type of WEBDRIVER_IMPLICIT_WAIT:%s is not 'int' or 'float', here set a default value: 20")
             else:
-                # if there are no implicitly_wait found in settings, then set a default value: 60
-                browser.implicitly_wait(60)
+                # if there are no WEBDRIVER_IMPLICIT_WAIT found in settings, then set a default value: 20
+                browser.implicitly_wait(20)
                 print(
-                    "there are no implicitly_wait found in settings, then set a default value: 60")
+                    "there are no WEBDRIVER_IMPLICIT_WAIT found in settings, then set a default value: 20")
 
-            # set SeleniumHelper.set_implicitly_wait_flag = True after set the implicitly_wait.
+            # set SeleniumHelper.set_implicitly_wait_flag = True after set the WEBDRIVER_IMPLICIT_WAIT.
             SeleniumHelper.set_implicitly_wait_flag = True
 
         return browser
 
     @staticmethod
     def switch_to_new_window(browser, old_handle_list=None):
         """
```

### Comparing `linktest-2.4.3/linktest/timeout_thread.py` & `linktest-2.4.4/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/ui_testcase.py` & `linktest-2.4.4/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/update_config.py` & `linktest-2.4.4/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/webdriver_wrapper.py` & `linktest-2.4.4/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest/xml_report.py` & `linktest-2.4.4/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.4.3/linktest.egg-info/SOURCES.txt` & `linktest-2.4.4/linktest.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 linktest/get_adb_devices.py
 linktest/get_ios_devices_list.py
 linktest/get_platform_info.py
 linktest/get_project_info.py
 linktest/html_report.py
 linktest/ios_testcase.py
 linktest/linktest_setup.py
-linktest/logged_requests copy.py
 linktest/logged_requests.py
 linktest/main.py
 linktest/memory_usage.py
 linktest/re_func.py
 linktest/run.py
 linktest/run_testcase_thread.py
 linktest/scp_report_to_specified_path.py
```

