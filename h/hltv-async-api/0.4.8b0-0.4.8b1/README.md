# Comparing `tmp/hltv_async_api-0.4.8b0.tar.gz` & `tmp/hltv_async_api-0.4.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.8b0.tar", max compression
+gzip compressed data, was "hltv_async_api-0.4.8b1.tar", max compression
```

## Comparing `hltv_async_api-0.4.8b0.tar` & `hltv_async_api-0.4.8b1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      124 2024-04-15 17:17:42.599661 hltv_async_api-0.4.8b0/hltv_async_api/__init__.py
--rw-r--r--   0        0        0    33465 2024-04-15 17:24:45.836605 hltv_async_api-0.4.8b0/hltv_async_api/aiohltv.py
--rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.4.8b0/hltv_async_api/proxies.txt
--rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.4.8b0/LICENSE
--rw-r--r--   0        0        0      633 2024-04-15 17:40:32.195069 hltv_async_api-0.4.8b0/pyproject.toml
--rw-r--r--   0        0        0    11188 2024-04-15 17:36:08.973708 hltv_async_api-0.4.8b0/README.md
--rw-r--r--   0        0        0    11718 1970-01-01 00:00:00.000000 hltv_async_api-0.4.8b0/PKG-INFO
+-rw-r--r--   0        0        0      124 2024-04-15 17:17:42.599661 hltv_async_api-0.4.8b1/hltv_async_api/__init__.py
+-rw-r--r--   0        0        0    33465 2024-04-15 17:24:45.836605 hltv_async_api-0.4.8b1/hltv_async_api/aiohltv.py
+-rw-r--r--   0        0        0     1935 2024-04-03 12:53:56.200826 hltv_async_api-0.4.8b1/hltv_async_api/proxies.txt
+-rw-r--r--   0        0        0     1091 2024-04-02 00:22:12.491888 hltv_async_api-0.4.8b1/LICENSE
+-rw-r--r--   0        0        0      650 2024-04-15 17:54:37.096842 hltv_async_api-0.4.8b1/pyproject.toml
+-rw-r--r--   0        0        0    11188 2024-04-15 17:36:08.973708 hltv_async_api-0.4.8b1/README.md
+-rw-r--r--   0        0        0    11748 1970-01-01 00:00:00.000000 hltv_async_api-0.4.8b1/PKG-INFO
```

### Comparing `hltv_async_api-0.4.8b0/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.8b1/hltv_async_api/aiohltv.py`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.8b0/hltv_async_api/proxies.txt` & `hltv_async_api-0.4.8b1/hltv_async_api/proxies.txt`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.8b0/LICENSE` & `hltv_async_api-0.4.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.8b0/pyproject.toml` & `hltv_async_api-0.4.8b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hltv_async_api"
-version = "0.4.8b"
+version = "0.4.8b1"
 authors = ["Akim Slys <akimslys2003@gmail.com>"]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -15,8 +15,9 @@
 Issues = "https://github.com/akimerslys/aiohltv/issues"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 beautifulsoup4 = "^4.12.3"
 aiohttp = "^3.9.3"
 pytz = "^2024.1"
-setuptools = "^69.1.0"
+setuptools = "^69.1.0"
+lxml = "5.2.0"
```

### Comparing `hltv_async_api-0.4.8b0/README.md` & `hltv_async_api-0.4.8b1/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.8b0/PKG-INFO` & `hltv_async_api-0.4.8b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.8b0
+Version: 0.4.8b1
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Author: Akim Slys
 Author-email: akimslys2003@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: lxml (==5.2.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: setuptools (>=69.1.0,<70.0.0)
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Description-Content-Type: text/markdown
 
 # hltv-async-api an unofficial asynchronous HLTV API Wrapper for Python
```

