# Comparing `tmp/CopaData-3.40.2.tar.gz` & `tmp/CopaData-3.40.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\CopaData-3.40.2.tar", last modified: Fri Jan 31 06:42:07 2020, max compression
+gzip compressed data, was "dist\CopaData-3.40.3.tar", last modified: Fri Jul 17 06:12:10 2020, max compression
```

## Comparing `CopaData-3.40.2.tar` & `CopaData-3.40.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2020-01-31 06:42:07.000000 CopaData-3.40.2/
-drwxrwxrwx   0        0        0        0 2020-01-31 06:42:07.000000 CopaData-3.40.2/CopaData/
--rw-rw-rw-   0        0        0       97 2020-01-16 15:58:46.000000 CopaData-3.40.2/CopaData/__init__.py
--rw-rw-rw-   0        0        0    46773 2020-01-31 06:30:45.000000 CopaData-3.40.2/CopaData/pyZAN.py
-drwxrwxrwx   0        0        0        0 2020-01-31 06:42:07.000000 CopaData-3.40.2/CopaData.egg-info/
--rw-rw-rw-   0        0        0     1811 2020-01-31 06:42:05.000000 CopaData-3.40.2/CopaData.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2020-01-31 06:42:06.000000 CopaData-3.40.2/CopaData.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-01-31 06:42:05.000000 CopaData-3.40.2/CopaData.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2020-01-31 06:42:06.000000 CopaData-3.40.2/CopaData.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1811 2020-01-31 06:42:07.000000 CopaData-3.40.2/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2020-01-16 15:58:46.000000 CopaData-3.40.2/README.md
--rw-rw-rw-   0        0        0       42 2020-01-31 06:42:07.000000 CopaData-3.40.2/setup.cfg
--rw-rw-rw-   0        0        0      686 2020-01-31 06:41:39.000000 CopaData-3.40.2/setup.py
+drwxrwxrwx   0        0        0        0 2020-07-17 06:12:10.000000 CopaData-3.40.3/
+drwxrwxrwx   0        0        0        0 2020-07-17 06:12:10.000000 CopaData-3.40.3/CopaData/
+-r--r--r--   0        0        0       97 2020-07-14 06:37:39.000000 CopaData-3.40.3/CopaData/__init__.py
+-r--r--r--   0        0        0    46756 2020-07-17 05:59:24.000000 CopaData-3.40.3/CopaData/pyZAN.py
+drwxrwxrwx   0        0        0        0 2020-07-17 06:12:10.000000 CopaData-3.40.3/CopaData.egg-info/
+-rw-rw-rw-   0        0        0     1811 2020-07-17 06:12:10.000000 CopaData-3.40.3/CopaData.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2020-07-17 06:12:10.000000 CopaData-3.40.3/CopaData.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-07-17 06:12:10.000000 CopaData-3.40.3/CopaData.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2020-07-17 06:12:10.000000 CopaData-3.40.3/CopaData.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1811 2020-07-17 06:12:10.000000 CopaData-3.40.3/PKG-INFO
+-r--r--r--   0        0        0     1050 2020-07-14 06:37:39.000000 CopaData-3.40.3/README.md
+-rw-rw-rw-   0        0        0       42 2020-07-17 06:12:10.000000 CopaData-3.40.3/setup.cfg
+-r--r--r--   0        0        0      686 2020-07-17 06:00:05.000000 CopaData-3.40.3/setup.py
```

### Comparing `CopaData-3.40.2/CopaData/pyZAN.py` & `CopaData-3.40.3/CopaData/pyZAN.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,21 +48,21 @@
             self._useIntegratedSecurity = use_integrated_security
             self._user = user
             self._password = password
             self._cnxn = None
             
             if self._useIntegratedSecurity : 
                 self._cnxn = pyodbc.connect("DRIVER={SQL Server Native Client 11.0};Server="
-                + self._server + "; Initial Catalog ="
-                + self._metadb + "; Trusted_Connection=Yes")
+                + self._server + ";Initial Catalog="
+                + self._metadb + ";Trusted_Connection=Yes")
             else:
                 self._cnxn = pyodbc.connect("DRIVER={SQL Server Native Client 11.0};Server="
-                + self._server + "; Initial Catalog ="
-                + self._metadb + "; User = "
-                + self._user + "; Password = " + self._password)
+                + self._server + ";Initial Catalog="
+                + self._metadb + ";UID="
+                + self._user + ";PWD=" + self._password)
 
             #Check zenon Analyzer metadata database version. Must be at least version 7 for 3.30
             try:
                 result = pd.read_sql(
                     f"SELECT [{self._metadb}].[dbo].[zrsGetDatabaseVersion]()", self._cnxn)
                 self._version = result.iloc[0][0]
                 if(self._version < 7):
```

### Comparing `CopaData-3.40.2/CopaData.egg-info/PKG-INFO` & `CopaData-3.40.3/CopaData.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CopaData
-Version: 3.40.2
+Version: 3.40.3
 Summary: Read metadata and online data from zenon Analyzer Server
 Home-page: https://www.copadata.com
 Author: COPA-DATA
 Author-email: development@copadata.com
 License: UNKNOWN
 Description: ## Package description
         This package contains data connectivity modules developed by COPA-DATA.
```

### Comparing `CopaData-3.40.2/PKG-INFO` & `CopaData-3.40.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CopaData
-Version: 3.40.2
+Version: 3.40.3
 Summary: Read metadata and online data from zenon Analyzer Server
 Home-page: https://www.copadata.com
 Author: COPA-DATA
 Author-email: development@copadata.com
 License: UNKNOWN
 Description: ## Package description
         This package contains data connectivity modules developed by COPA-DATA.
```

### Comparing `CopaData-3.40.2/README.md` & `CopaData-3.40.3/README.md`

 * *Files identical despite different names*

### Comparing `CopaData-3.40.2/setup.py` & `CopaData-3.40.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="CopaData",
-    version="3.40.2",
+    version="3.40.3",
     author="COPA-DATA",
     author_email="development@copadata.com",
     description="Read metadata and online data from zenon Analyzer Server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.copadata.com",
     packages=setuptools.find_packages(),
```

