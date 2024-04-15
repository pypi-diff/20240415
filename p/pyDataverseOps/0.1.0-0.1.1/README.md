# Comparing `tmp/PyDataverseOps-0.1.0.tar.gz` & `tmp/PyDataverseOps-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDataverseOps-0.1.0.tar", last modified: Mon Apr 15 17:02:55 2024, max compression
+gzip compressed data, was "PyDataverseOps-0.1.1.tar", last modified: Mon Apr 15 17:09:52 2024, max compression
```

## Comparing `PyDataverseOps-0.1.0.tar` & `PyDataverseOps-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:02:55.795058 PyDataverseOps-0.1.0/
--rw-rw-rw-   0        0        0     4411 2024-04-15 17:02:55.794110 PyDataverseOps-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 17:02:55.792139 PyDataverseOps-0.1.0/PyDataverseOps.egg-info/
--rw-rw-rw-   0        0        0     4411 2024-04-15 17:02:55.000000 PyDataverseOps-0.1.0/PyDataverseOps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-04-15 17:02:55.000000 PyDataverseOps-0.1.0/PyDataverseOps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:02:55.000000 PyDataverseOps-0.1.0/PyDataverseOps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-15 17:02:55.000000 PyDataverseOps-0.1.0/PyDataverseOps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:02:55.000000 PyDataverseOps-0.1.0/PyDataverseOps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3480 2024-04-15 17:02:03.000000 PyDataverseOps-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 17:02:55.795058 PyDataverseOps-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1162 2024-04-15 17:00:49.000000 PyDataverseOps-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:09:52.893104 PyDataverseOps-0.1.1/
+-rw-rw-rw-   0        0        0     4423 2024-04-15 17:09:52.893104 PyDataverseOps-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 17:09:52.891052 PyDataverseOps-0.1.1/PyDataverseOps.egg-info/
+-rw-rw-rw-   0        0        0     4423 2024-04-15 17:09:52.000000 PyDataverseOps-0.1.1/PyDataverseOps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-15 17:09:52.000000 PyDataverseOps-0.1.1/PyDataverseOps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:09:52.000000 PyDataverseOps-0.1.1/PyDataverseOps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-15 17:09:52.000000 PyDataverseOps-0.1.1/PyDataverseOps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:09:52.000000 PyDataverseOps-0.1.1/PyDataverseOps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3492 2024-04-15 17:09:31.000000 PyDataverseOps-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:09:52.893104 PyDataverseOps-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1162 2024-04-15 17:09:46.000000 PyDataverseOps-0.1.1/setup.py
```

### Comparing `PyDataverseOps-0.1.0/PKG-INFO` & `PyDataverseOps-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDataverseOps
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to facilitate operations on Microsoft Dataverse
 Home-page: https://github.com/ray2199/PyDataverseOps.git
 Author: Akash Yadav
 Author-email: akash21091999@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -41,15 +41,15 @@
 cd your-repository-folder
 ```
 
 
 Then install the library using pip:
 
 ```bash
-pip install .
+pip install pyDataverseOps
 ```
 
 ## Requirements
 - Python 3.6+
 - pandas
 - requests
 
@@ -61,15 +61,15 @@
 - `domain`: Your Dataverse domain.
 - `tenant_id`: Tenant ID for OAuth authentication.
 - `client_id`: Client ID for OAuth authentication.
 - `client_secret`: Client Secret for OAuth authentication.
 
 ### Example Initialization
 ```python
-from pydataverseops import pyDataverseOps
+from dataverse_ops import pyDataverseOps
 
 dv_ops = pyDataverseOps(
     domain='your_dataverse_domain',
     tenant_id='your_tenant_id',
     client_id='your_client_id',
     client_secret='your_client_secret'
 )
```

### Comparing `PyDataverseOps-0.1.0/PyDataverseOps.egg-info/PKG-INFO` & `PyDataverseOps-0.1.1/PyDataverseOps.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDataverseOps
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library to facilitate operations on Microsoft Dataverse
 Home-page: https://github.com/ray2199/PyDataverseOps.git
 Author: Akash Yadav
 Author-email: akash21091999@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -41,15 +41,15 @@
 cd your-repository-folder
 ```
 
 
 Then install the library using pip:
 
 ```bash
-pip install .
+pip install pyDataverseOps
 ```
 
 ## Requirements
 - Python 3.6+
 - pandas
 - requests
 
@@ -61,15 +61,15 @@
 - `domain`: Your Dataverse domain.
 - `tenant_id`: Tenant ID for OAuth authentication.
 - `client_id`: Client ID for OAuth authentication.
 - `client_secret`: Client Secret for OAuth authentication.
 
 ### Example Initialization
 ```python
-from pydataverseops import pyDataverseOps
+from dataverse_ops import pyDataverseOps
 
 dv_ops = pyDataverseOps(
     domain='your_dataverse_domain',
     tenant_id='your_tenant_id',
     client_id='your_client_id',
     client_secret='your_client_secret'
 )
```

### Comparing `PyDataverseOps-0.1.0/README.md` & `PyDataverseOps-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 cd your-repository-folder
 ```
 
 
 Then install the library using pip:
 
 ```bash
-pip install .
+pip install pyDataverseOps
 ```
 
 ## Requirements
 - Python 3.6+
 - pandas
 - requests
 
@@ -38,15 +38,15 @@
 - `domain`: Your Dataverse domain.
 - `tenant_id`: Tenant ID for OAuth authentication.
 - `client_id`: Client ID for OAuth authentication.
 - `client_secret`: Client Secret for OAuth authentication.
 
 ### Example Initialization
 ```python
-from pydataverseops import pyDataverseOps
+from dataverse_ops import pyDataverseOps
 
 dv_ops = pyDataverseOps(
     domain='your_dataverse_domain',
     tenant_id='your_tenant_id',
     client_id='your_client_id',
     client_secret='your_client_secret'
 )
```

### Comparing `PyDataverseOps-0.1.0/setup.py` & `PyDataverseOps-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="PyDataverseOps",
-    version="0.1.0",
+    version="0.1.1",
     author="Akash Yadav",
     author_email="akash21091999@gmail.com",
     description="A Python library to facilitate operations on Microsoft Dataverse",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/ray2199/PyDataverseOps.git",  # Replace with your repository URL
     packages=find_packages(),
```

