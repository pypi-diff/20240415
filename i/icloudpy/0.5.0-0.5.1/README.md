# Comparing `tmp/icloudpy-0.5.0.tar.gz` & `tmp/icloudpy-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icloudpy-0.5.0.tar", last modified: Thu Oct 12 04:54:13 2023, max compression
+gzip compressed data, was "icloudpy-0.5.1.tar", last modified: Mon Apr 15 14:19:18 2024, max compression
```

## Comparing `icloudpy-0.5.0.tar` & `icloudpy-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 04:54:13.280546 icloudpy-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-10-12 04:54:02.000000 icloudpy-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-10-12 04:54:02.000000 icloudpy-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14980 2023-10-12 04:54:13.280546 icloudpy-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14587 2023-10-12 04:54:02.000000 icloudpy-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 04:54:13.280546 icloudpy-0.5.0/icloudpy/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22304 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11873 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 04:54:13.280546 icloudpy-0.5.0/icloudpy/services/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10532 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/calendar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/drive.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/findmyiphone.py
--rw-r--r--   0 runner    (1001) docker     (127)    26390 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/photos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/reminders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/services/ubiquity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2023-10-12 04:54:02.000000 icloudpy-0.5.0/icloudpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 04:54:13.280546 icloudpy-0.5.0/icloudpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14980 2023-10-12 04:54:13.000000 icloudpy-0.5.0/icloudpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2023-10-12 04:54:13.000000 icloudpy-0.5.0/icloudpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 04:54:13.000000 icloudpy-0.5.0/icloudpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-10-12 04:54:13.000000 icloudpy-0.5.0/icloudpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-12 04:54:13.000000 icloudpy-0.5.0/icloudpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-12 04:54:13.000000 icloudpy-0.5.0/icloudpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-10-12 04:54:02.000000 icloudpy-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 04:54:13.280546 icloudpy-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-10-12 04:54:02.000000 icloudpy-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:19:18.672619 icloudpy-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-15 14:19:08.000000 icloudpy-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-15 14:19:08.000000 icloudpy-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-04-15 14:19:18.672619 icloudpy-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2024-04-15 14:19:08.000000 icloudpy-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:19:18.672619 icloudpy-0.5.1/icloudpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22410 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11794 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:19:18.672619 icloudpy-0.5.1/icloudpy/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10532 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13226 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/findmyiphone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26390 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/photos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/reminders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/services/ubiquity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-15 14:19:08.000000 icloudpy-0.5.1/icloudpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:19:18.672619 icloudpy-0.5.1/icloudpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14981 2024-04-15 14:19:18.000000 icloudpy-0.5.1/icloudpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-15 14:19:18.000000 icloudpy-0.5.1/icloudpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:19:18.000000 icloudpy-0.5.1/icloudpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 14:19:18.000000 icloudpy-0.5.1/icloudpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 14:19:18.000000 icloudpy-0.5.1/icloudpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 14:19:18.000000 icloudpy-0.5.1/icloudpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 14:19:08.000000 icloudpy-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:19:18.672619 icloudpy-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-15 14:19:08.000000 icloudpy-0.5.1/setup.py
```

### Comparing `icloudpy-0.5.0/LICENSE` & `icloudpy-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/PKG-INFO` & `icloudpy-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icloudpy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python library to interact with iCloud web service
 Home-page: https://github.com/mandarons/icloudpy
 Author: Mandar Patil
 Author-email: mandarons@pm.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -29,15 +29,15 @@
 
 Authentication without using a saved password is as simple as passing your username and password to the `ICloudPyService` class:
 
 ```python
 from icloudpy import ICloudPyService
 api = ICloudPyService('jappleseed@apple.com', 'password')
 # For China region
-api = ICloudPyService('jappleseed@apple.com', 'password' auth_endpoint="https://www.icloud.com.cn",setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",)
+api = ICloudPyService('jappleseed@apple.com', 'password', home_endpoint="https://www.icloud.com.cn",setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",)
 ```
 
 In the event that the username/password combination is invalid, a `ICloudPyFailedLoginException` exception is thrown.
 
 You can also store your password in the system keyring using the command-line tool:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: icloudpy Version: 0.5.0 Summary: Python library to
+Metadata-Version: 2.1 Name: icloudpy Version: 0.5.1 Summary: Python library to
 interact with iCloud web service Home-page: https://github.com/mandarons/
 icloudpy Author: Mandar Patil Author-email: mandarons@pm.me Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE # iCloudPy [![CI - Main](https://github.com/mandarons/
 icloudpy/actions/workflows/ci-main-test-coverage.yml/badge.svg)](https://
 github.com/mandarons/icloudpy/actions/workflows/ci-main-test-coverage.yml) [!
@@ -18,16 +18,16 @@
 wrapper library written in Python. It is a major reuse of [pyiCloud](https://
 github.com/picklepete/pyicloud) python library. iCloudPy connects to iCloud
 using your `username` and `password`, stores the session locally and then
 performs various queries to iCloud server. ## Authentication Authentication
 without using a saved password is as simple as passing your username and
 password to the `ICloudPyService` class: ```python from icloudpy import
 ICloudPyService api = ICloudPyService('jappleseed@apple.com', 'password') # For
-China region api = ICloudPyService('jappleseed@apple.com', 'password'
-auth_endpoint="https://www.icloud.com.cn",setup_endpoint="https://
+China region api = ICloudPyService('jappleseed@apple.com', 'password',
+home_endpoint="https://www.icloud.com.cn",setup_endpoint="https://
 setup.icloud.com.cn/setup/ws/1",) ``` In the event that the username/password
 combination is invalid, a `ICloudPyFailedLoginException` exception is thrown.
 You can also store your password in the system keyring using the command-line
 tool: ```bash > icloud --username=jappleseed@apple.com ICloud Password for
 jappleseed@apple.com: Save password in keyring? (y/N) # For China region >
 icloud --username=jappleseed@apple.com --region=china ICloud Password for
 jappleseed@apple.com: Save password in keyring? (y/N) ``` If you have stored a
```

### Comparing `icloudpy-0.5.0/README.md` & `icloudpy-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Authentication without using a saved password is as simple as passing your username and password to the `ICloudPyService` class:
 
 ```python
 from icloudpy import ICloudPyService
 api = ICloudPyService('jappleseed@apple.com', 'password')
 # For China region
-api = ICloudPyService('jappleseed@apple.com', 'password' auth_endpoint="https://www.icloud.com.cn",setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",)
+api = ICloudPyService('jappleseed@apple.com', 'password', home_endpoint="https://www.icloud.com.cn",setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",)
 ```
 
 In the event that the username/password combination is invalid, a `ICloudPyFailedLoginException` exception is thrown.
 
 You can also store your password in the system keyring using the command-line tool:
 
 ```bash
```

#### html2text {}

```diff
@@ -13,16 +13,16 @@
 wrapper library written in Python. It is a major reuse of [pyiCloud](https://
 github.com/picklepete/pyicloud) python library. iCloudPy connects to iCloud
 using your `username` and `password`, stores the session locally and then
 performs various queries to iCloud server. ## Authentication Authentication
 without using a saved password is as simple as passing your username and
 password to the `ICloudPyService` class: ```python from icloudpy import
 ICloudPyService api = ICloudPyService('jappleseed@apple.com', 'password') # For
-China region api = ICloudPyService('jappleseed@apple.com', 'password'
-auth_endpoint="https://www.icloud.com.cn",setup_endpoint="https://
+China region api = ICloudPyService('jappleseed@apple.com', 'password',
+home_endpoint="https://www.icloud.com.cn",setup_endpoint="https://
 setup.icloud.com.cn/setup/ws/1",) ``` In the event that the username/password
 combination is invalid, a `ICloudPyFailedLoginException` exception is thrown.
 You can also store your password in the system keyring using the command-line
 tool: ```bash > icloud --username=jappleseed@apple.com ICloud Password for
 jappleseed@apple.com: Save password in keyring? (y/N) # For China region >
 icloud --username=jappleseed@apple.com --region=china ICloud Password for
 jappleseed@apple.com: Save password in keyring? (y/N) ``` If you have stored a
```

### Comparing `icloudpy-0.5.0/icloudpy/base.py` & `icloudpy-0.5.1/icloudpy/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,16 +249,18 @@
         try:
             with open(self.session_path, encoding="utf-8") as session_f:
                 self.session_data = json.load(session_f)
         except:  # pylint: disable=bare-except
             LOGGER.info("Session file does not exist")
         if self.session_data.get("client_id"):
             self.client_id = self.session_data.get("client_id")
+            self.params["clientId"] = self.client_id
         else:
             self.session_data.update({"client_id": self.client_id})
+            self.params["clientId"] = self.client_id
 
         self.session = ICloudPySession(self)
         self.session.verify = verify
         self.session.headers.update(
             {"Origin": self.home_endpoint, "Referer": f"{self.home_endpoint}/"}
         )
```

### Comparing `icloudpy-0.5.0/icloudpy/cmdline.py` & `icloudpy-0.5.1/icloudpy/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,14 @@
 
         try:
             api = (
                 ICloudPyService(
                     apple_id=username.strip(),
                     password=password.strip(),
                     cookie_directory=session_directory,
-                    auth_endpoint="https://idmsa.apple.com.cn/appleauth/auth",
                     home_endpoint="https://www.icloud.com.cn",
                     setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",
                 )
                 if server_region == "china"
                 else ICloudPyService(
                     apple_id=username.strip(),
                     password=password.strip(),
```

### Comparing `icloudpy-0.5.0/icloudpy/exceptions.py` & `icloudpy-0.5.1/icloudpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/__init__.py` & `icloudpy-0.5.1/icloudpy/services/__init__.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/account.py` & `icloudpy-0.5.1/icloudpy/services/account.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/calendar.py` & `icloudpy-0.5.1/icloudpy/services/calendar.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,17 +42,17 @@
     def refresh_client(self, from_dt=None, to_dt=None):
         """
         Refreshes the CalendarService endpoint, ensuring that the
         event data is up-to-date. If no 'from_dt' or 'to_dt' datetimes
         have been given, the range becomes this month.
         """
         today = datetime.today()
-        first_day, last_day = monthrange(today.year, today.month)
+        _, last_day = monthrange(today.year, today.month)
         if not from_dt:
-            from_dt = datetime(today.year, today.month, first_day)
+            from_dt = datetime(today.year, today.month, 1)
         if not to_dt:
             to_dt = datetime(today.year, today.month, last_day)
         params = dict(self.params)
         params.update(
             {
                 "lang": "en-us",
                 "usertz": get_localzone().zone,
@@ -72,16 +72,16 @@
         return self.response.get("Event")
 
     def calendars(self):
         """
         Retrieves calendars of this month.
         """
         today = datetime.today()
-        first_day, last_day = monthrange(today.year, today.month)
-        from_dt = datetime(today.year, today.month, first_day)
+        _, last_day = monthrange(today.year, today.month)
+        from_dt = datetime(today.year, today.month, 1)
         to_dt = datetime(today.year, today.month, last_day)
         params = dict(self.params)
         params.update(
             {
                 "lang": "en-us",
                 "usertz": get_localzone().zone,
                 "startDate": from_dt.strftime("%Y-%m-%d"),
```

### Comparing `icloudpy-0.5.0/icloudpy/services/contacts.py` & `icloudpy-0.5.1/icloudpy/services/contacts.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/drive.py` & `icloudpy-0.5.1/icloudpy/services/drive.py`

 * *Files 4% similar despite different names*

```diff
@@ -325,14 +325,18 @@
         """Gets the node list of directories."""
         if self.type == "file":
             return None
         return [child.name for child in self.get_children()]
 
     def mkdir(self, folder):
         """Create a new directory directory."""
+        # remove cached entries information first so that it will be re-read on next get_children()
+        self._children = None
+        if "items" in self.data:
+            self.data.pop("items")
         return self.connection.create_folders(self.data["drivewsid"], folder)
 
     def rename(self, name):
         """Rename an iCloud Drive item."""
         return self.connection.rename_items(
             self.data["drivewsid"], self.data["etag"], name
         )
```

### Comparing `icloudpy-0.5.0/icloudpy/services/findmyiphone.py` & `icloudpy-0.5.1/icloudpy/services/findmyiphone.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/photos.py` & `icloudpy-0.5.1/icloudpy/services/photos.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/reminders.py` & `icloudpy-0.5.1/icloudpy/services/reminders.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/services/ubiquity.py` & `icloudpy-0.5.1/icloudpy/services/ubiquity.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy/utils.py` & `icloudpy-0.5.1/icloudpy/utils.py`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/icloudpy.egg-info/PKG-INFO` & `icloudpy-0.5.1/icloudpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icloudpy
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python library to interact with iCloud web service
 Home-page: https://github.com/mandarons/icloudpy
 Author: Mandar Patil
 Author-email: mandarons@pm.me
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -29,15 +29,15 @@
 
 Authentication without using a saved password is as simple as passing your username and password to the `ICloudPyService` class:
 
 ```python
 from icloudpy import ICloudPyService
 api = ICloudPyService('jappleseed@apple.com', 'password')
 # For China region
-api = ICloudPyService('jappleseed@apple.com', 'password' auth_endpoint="https://www.icloud.com.cn",setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",)
+api = ICloudPyService('jappleseed@apple.com', 'password', home_endpoint="https://www.icloud.com.cn",setup_endpoint="https://setup.icloud.com.cn/setup/ws/1",)
 ```
 
 In the event that the username/password combination is invalid, a `ICloudPyFailedLoginException` exception is thrown.
 
 You can also store your password in the system keyring using the command-line tool:
 
 ```bash
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: icloudpy Version: 0.5.0 Summary: Python library to
+Metadata-Version: 2.1 Name: icloudpy Version: 0.5.1 Summary: Python library to
 interact with iCloud web service Home-page: https://github.com/mandarons/
 icloudpy Author: Mandar Patil Author-email: mandarons@pm.me Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE # iCloudPy [![CI - Main](https://github.com/mandarons/
 icloudpy/actions/workflows/ci-main-test-coverage.yml/badge.svg)](https://
 github.com/mandarons/icloudpy/actions/workflows/ci-main-test-coverage.yml) [!
@@ -18,16 +18,16 @@
 wrapper library written in Python. It is a major reuse of [pyiCloud](https://
 github.com/picklepete/pyicloud) python library. iCloudPy connects to iCloud
 using your `username` and `password`, stores the session locally and then
 performs various queries to iCloud server. ## Authentication Authentication
 without using a saved password is as simple as passing your username and
 password to the `ICloudPyService` class: ```python from icloudpy import
 ICloudPyService api = ICloudPyService('jappleseed@apple.com', 'password') # For
-China region api = ICloudPyService('jappleseed@apple.com', 'password'
-auth_endpoint="https://www.icloud.com.cn",setup_endpoint="https://
+China region api = ICloudPyService('jappleseed@apple.com', 'password',
+home_endpoint="https://www.icloud.com.cn",setup_endpoint="https://
 setup.icloud.com.cn/setup/ws/1",) ``` In the event that the username/password
 combination is invalid, a `ICloudPyFailedLoginException` exception is thrown.
 You can also store your password in the system keyring using the command-line
 tool: ```bash > icloud --username=jappleseed@apple.com ICloud Password for
 jappleseed@apple.com: Save password in keyring? (y/N) # For China region >
 icloud --username=jappleseed@apple.com --region=china ICloud Password for
 jappleseed@apple.com: Save password in keyring? (y/N) ``` If you have stored a
```

### Comparing `icloudpy-0.5.0/icloudpy.egg-info/SOURCES.txt` & `icloudpy-0.5.1/icloudpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `icloudpy-0.5.0/setup.py` & `icloudpy-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from codecs import open
 
 from setuptools import find_packages, setup
 
 REPO_URL = "https://github.com/mandarons/icloudpy"
-VERSION = "0.5.0"
+VERSION = "0.5.1"
 
 with open("README.md") as fh:
     long_description = fh.read()
 with open("requirements.txt") as fh:
     required = fh.read().splitlines()
 
 setup(
```

