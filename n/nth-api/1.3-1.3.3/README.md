# Comparing `tmp/nth_api-1.3.tar.gz` & `tmp/nth_api-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nth_api-1.3.tar", last modified: Mon Apr 15 13:52:02 2024, max compression
+gzip compressed data, was "nth_api-1.3.3.tar", last modified: Mon Apr 15 14:02:43 2024, max compression
```

## Comparing `nth_api-1.3.tar` & `nth_api-1.3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 13:52:02.113709 nth_api-1.3/
--rw-rw-rw-   0        0        0    35147 2024-04-15 13:43:48.000000 nth_api-1.3/LICENSE
--rw-rw-rw-   0        0        0     2167 2024-04-15 13:52:02.111705 nth_api-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1739 2024-04-15 13:51:08.000000 nth_api-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 13:52:02.110705 nth_api-1.3/nth_api.egg-info/
--rw-rw-rw-   0        0        0     2167 2024-04-15 13:52:01.000000 nth_api-1.3/nth_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-04-15 13:52:01.000000 nth_api-1.3/nth_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 13:52:01.000000 nth_api-1.3/nth_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 13:52:01.000000 nth_api-1.3/nth_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 13:52:02.113709 nth_api-1.3/setup.cfg
--rw-rw-rw-   0        0        0      645 2024-04-15 13:51:08.000000 nth_api-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 14:02:43.745530 nth_api-1.3.3/
+-rw-rw-rw-   0        0        0    35147 2024-04-15 13:43:48.000000 nth_api-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     2167 2024-04-15 14:02:43.745530 nth_api-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1737 2024-04-15 14:01:36.000000 nth_api-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 14:02:43.745530 nth_api-1.3.3/nth_api.egg-info/
+-rw-rw-rw-   0        0        0     2167 2024-04-15 14:02:43.000000 nth_api-1.3.3/nth_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2024-04-15 14:02:43.000000 nth_api-1.3.3/nth_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:02:43.000000 nth_api-1.3.3/nth_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 14:02:43.000000 nth_api-1.3.3/nth_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 14:02:43.745530 nth_api-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      647 2024-04-15 14:02:22.000000 nth_api-1.3.3/setup.py
```

### Comparing `nth_api-1.3/LICENSE` & `nth_api-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nth_api-1.3/PKG-INFO` & `nth_api-1.3.3/nth_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: nth_api
-Version: 1.3
+Name: nth-api
+Version: 1.3.3
 Summary: Name-That-Hash api version
 Home-page: https://github.com/user-sspmynxdvb/nth_api
 Author: user-sspmynxdvb
 License: GNUv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
 
 ## 🤔 What is this?
 
-**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔
-**
+**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
 
 **Name-that-hash will name that hash type!**
 
 ## Installing
 
 ### pip
```

### Comparing `nth_api-1.3/README.md` & `nth_api-1.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
 
 ## 🤔 What is this?
 
-**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔
-**
+**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
 
 **Name-that-hash will name that hash type!**
 
 ## Installing
 
 ### pip
```

### Comparing `nth_api-1.3/nth_api.egg-info/PKG-INFO` & `nth_api-1.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 Metadata-Version: 2.1
-Name: nth-api
-Version: 1.3
+Name: nth_api
+Version: 1.3.3
 Summary: Name-That-Hash api version
 Home-page: https://github.com/user-sspmynxdvb/nth_api
 Author: user-sspmynxdvb
 License: GNUv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ****[Name-that-hash](https://github.com/HashPals/Name-That-Hash) api version****
 
 ## 🤔 What is this?
 
-**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔
-**
+**Have you ever come across a hash such as `5f4dcc3b5aa765d61d8327deb882cf99` and wondered what type of hash that is? 🤔**
 
 **Name-that-hash will name that hash type!**
 
 ## Installing
 
 ### pip
```

### Comparing `nth_api-1.3/setup.py` & `nth_api-1.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name="nth_api",
     author="user-sspmynxdvb",
-    version="1.3",
+    version="1.3.3",
     description="Name-That-Hash api version",
     license="GNUv3",
     url="https://github.com/user-sspmynxdvb/nth_api",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

