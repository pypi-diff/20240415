# Comparing `tmp/hltv_async_api-0.4.6.tar.gz` & `tmp/hltv_async_api-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.6.tar", last modified: Mon Apr 15 17:11:15 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.7.tar", last modified: Mon Apr 15 17:26:38 2024, max compression
```

## Comparing `hltv_async_api-0.4.6.tar` & `hltv_async_api-0.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 17:11:15.843173 hltv_async_api-0.4.6/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.6/LICENSE
--rw-rw-rw-   0        0        0    11823 2024-04-15 17:11:15.842171 hltv_async_api-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0    11200 2024-04-09 13:03:53.000000 hltv_async_api-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 17:11:15.831171 hltv_async_api-0.4.6/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-15 17:06:53.000000 hltv_async_api-0.4.6/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    33435 2024-04-15 09:56:27.000000 hltv_async_api-0.4.6/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-15 17:11:15.841173 hltv_async_api-0.4.6/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0    11823 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-15 17:11:15.000000 hltv_async_api-0.4.6/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-15 17:06:53.000000 hltv_async_api-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 17:11:15.843173 hltv_async_api-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      947 2024-04-15 17:06:53.000000 hltv_async_api-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:26:38.612148 hltv_async_api-0.4.7/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0    11823 2024-04-15 17:26:38.610148 hltv_async_api-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0    11200 2024-04-09 13:03:53.000000 hltv_async_api-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:26:38.597149 hltv_async_api-0.4.7/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-15 17:17:42.000000 hltv_async_api-0.4.7/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    33465 2024-04-15 17:24:45.000000 hltv_async_api-0.4.7/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:26:38.609150 hltv_async_api-0.4.7/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0    11823 2024-04-15 17:26:38.000000 hltv_async_api-0.4.7/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-15 17:26:38.000000 hltv_async_api-0.4.7/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:26:38.000000 hltv_async_api-0.4.7/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 17:26:38.000000 hltv_async_api-0.4.7/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      539 2024-04-15 17:26:35.000000 hltv_async_api-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:26:38.612148 hltv_async_api-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      947 2024-04-15 17:17:42.000000 hltv_async_api-0.4.7/setup.py
```

### Comparing `hltv_async_api-0.4.6/LICENSE` & `hltv_async_api-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.6/PKG-INFO` & `hltv_async_api-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.6
+Version: 0.4.7
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.4.6/README.md` & `hltv_async_api-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.6/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.7/hltv_async_api/aiohltv.py`

 * *Files 0% similar despite different names*

```diff
@@ -826,11 +826,11 @@
     print(await hltv.get_event_info(7437, 'betboom-dacha-belgrade-2024-europe-closed-qualifier'))
     print(await hltv.get_event_results(7437))
     print(await hltv.get_upcoming_matches(1, 3))
     print(await hltv.get_match_info('2370913', 'FURIA', 'MOUZ', 'betboom-dacha-belgrade-2024-europe-closed-qualifier'))
     print(await hltv.get_last_news())
     print(await hltv.get_top_teams())
     print(await hltv.get_best_players())
-
+    await hltv.close_session()
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.4.6/hltv_async_api.egg-info/PKG-INFO` & `hltv_async_api-0.4.7/hltv_async_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hltv_async_api
-Version: 0.4.6
+Version: 0.4.7
 Summary: Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python
 Home-page: https://github.com/akimerslys/aiohltv
 Author: akimerslys
 Author-email: Akim Slys <akimslys2003@gmail.com>
 Project-URL: Homepage, https://github.com/akimerslys/aiohltv
 Project-URL: Issues, https://github.com/akimerslys/aiohltv/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hltv_async_api-0.4.6/pyproject.toml` & `hltv_async_api-0.4.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.6"
+version = "0.4.7"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 Homepage = "https://github.com/akimerslys/aiohltv"
-Issues = "https://github.com/akimerslys/aiohltv/issues"
+Issues = "https://github.com/akimerslys/aiohltv/issues"
```

### Comparing `hltv_async_api-0.4.6/setup.py` & `hltv_async_api-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.4.6',
+    version='0.4.7',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

