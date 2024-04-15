# Comparing `tmp/edwh_uptime_plugin-0.3.5.tar.gz` & `tmp/edwh_uptime_plugin-0.3.6.tar.gz`

## Comparing `edwh_uptime_plugin-0.3.5.tar` & `edwh_uptime_plugin-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,27 @@
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/__about__.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/__init__.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/dumpers.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/helpers.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/tasks.py
--rw-r--r--   0        0        0     9590 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/uptimerobot.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/tests/test_api.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/README.md
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     5282 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/d_5ce624dd6693747a___init___py.html
+-rw-r--r--   0        0        0    68016 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/d_5ce624dd6693747a_uptime_plugin_py.html
+-rw-r--r--   0        0        0    66890 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/d_5ce624dd6693747a_uptimerobot_py.html
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/d_a44f0ac069e85531___init___py.html
+-rw-r--r--   0        0        0    19045 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/d_a44f0ac069e85531_test_api_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/status.json
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/htmlcov/style.css
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/__about__.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/__init__.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/dumpers.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/helpers.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/tasks.py
+-rw-r--r--   0        0        0     9588 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/uptimerobot.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/tests/test_api.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/README.md
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 edwh_uptime_plugin-0.3.6/PKG-INFO
```

### Comparing `edwh_uptime_plugin-0.3.5/CHANGELOG.md` & `edwh_uptime_plugin-0.3.6/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.3.6 (2024-04-15)
+
+### Fix
+
+* Set default of apikey to empty string instead of None ([`c46ed10`](https://github.com/educationwarehouse/edwh-uptime-plugin/commit/c46ed10a7bb1bb23eb71a224a463348d7b012c30))
+
 ## v0.3.5 (2024-04-09)
 
 ### Fix
 
 * **deps:** Include two missing dependencies ([`09fb42e`](https://github.com/educationwarehouse/edwh-uptime-plugin/commit/09fb42e88c5c79dc02fc8cf80e31173a1d03b14f))
 
 ## v0.3.4 (2024-03-15)
```

### Comparing `edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/dumpers.py` & `edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/dumpers.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/tasks.py` & `edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/tasks.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.5/src/edwh_uptime_plugin/uptimerobot.py` & `edwh_uptime_plugin-0.3.6/src/edwh_uptime_plugin/uptimerobot.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     _verbose: bool = False
 
     @property
     def api_key(self) -> str:
         if not self._api_key:
             self._api_key = check_env(
                 "UPTIMEROBOT_APIKEY",
-                default=None,
+                default="",
                 comment="The API key used to manage UptimeRobot monitors.",
             )
 
         return self._api_key
 
     @property
     def has_api_key(self) -> bool:
```

### Comparing `edwh_uptime_plugin-0.3.5/tests/test_api.py` & `edwh_uptime_plugin-0.3.6/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.5/LICENSE.txt` & `edwh_uptime_plugin-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.5/README.md` & `edwh_uptime_plugin-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.5/pyproject.toml` & `edwh_uptime_plugin-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_uptime_plugin-0.3.5/PKG-INFO` & `edwh_uptime_plugin-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: edwh-uptime-plugin
-Version: 0.3.5
+Version: 0.3.6
 Summary: UptimeRobot plugin for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-uptime-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-uptime-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-uptime-plugin
 Author-email: Remco Boerma <remco.b@educationwarehouse.nl>, Robin van der Noord <robin.vdn@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

