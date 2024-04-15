# Comparing `tmp/free_verify_proxy-1.1.6.tar.gz` & `tmp/free_verify_proxy-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "free_verify_proxy-1.1.6.tar", last modified: Tue Apr  9 15:40:35 2024, max compression
+gzip compressed data, was "free_verify_proxy-1.1.7.tar", last modified: Mon Apr 15 14:26:02 2024, max compression
```

## Comparing `free_verify_proxy-1.1.6.tar` & `free_verify_proxy-1.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:40:35.932864 free_verify_proxy-1.1.6/free_verify_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/free_proxy_verifyer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/free_verify_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10062 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/free_verify_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 15:40:35.000000 free_verify_proxy-1.1.6/free_verify_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 15:40:35.936864 free_verify_proxy-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-09 15:40:27.000000 free_verify_proxy-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:26:02.928386 free_verify_proxy-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-15 14:26:02.928386 free_verify_proxy-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:26:02.928386 free_verify_proxy-1.1.7/free_verify_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/free_verify_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/free_verify_proxy/free_proxy_verifyer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/free_verify_proxy/free_verify_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/free_verify_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:26:02.928386 free_verify_proxy-1.1.7/free_verify_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-04-15 14:26:02.000000 free_verify_proxy-1.1.7/free_verify_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 14:26:02.000000 free_verify_proxy-1.1.7/free_verify_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:26:02.000000 free_verify_proxy-1.1.7/free_verify_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 14:26:02.000000 free_verify_proxy-1.1.7/free_verify_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 14:26:02.000000 free_verify_proxy-1.1.7/free_verify_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:26:02.928386 free_verify_proxy-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-15 14:25:50.000000 free_verify_proxy-1.1.7/setup.py
```

### Comparing `free_verify_proxy-1.1.6/LICENSE.txt` & `free_verify_proxy-1.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `free_verify_proxy-1.1.6/PKG-INFO` & `free_verify_proxy-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: free_verify_proxy
-Version: 1.1.6
+Version: 1.1.7
 Summary: A simple package to provide http and https working proxy lists.
 Home-page: https://github.com/mominurr/free_verify_proxy
 Author: Mominur Rahman
 Author-email: mominurr518@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # free_verify_proxy
 
 free_verify_proxy is a Python library that collects free proxy from different sources and verifies whether the proxy is working or not. It checks the functionality of given proxies by making requests to various proxy detection servers. This library is useful for anyone who needs to ensure the reliability of proxies for their applications.
 
+# NOTE:
+if collected proxy lists are smaller than number_of_threads then it is not verified proxy lists. Just return collected proxy lists.
 
 # Proxy Sources
 
 ## Public Proxy Lists (HTTP/HTTPS)
 
 - [SSL Proxies](https://www.sslproxies.org/)
 - [Free Proxy List](https://free-proxy-list.net)
```

### Comparing `free_verify_proxy-1.1.6/README.md` & `free_verify_proxy-1.1.7/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # free_verify_proxy
 
 free_verify_proxy is a Python library that collects free proxy from different sources and verifies whether the proxy is working or not. It checks the functionality of given proxies by making requests to various proxy detection servers. This library is useful for anyone who needs to ensure the reliability of proxies for their applications.
 
+# NOTE:
+if collected proxy lists are smaller than number_of_threads then it is not verified proxy lists. Just return collected proxy lists.
 
 # Proxy Sources
 
 ## Public Proxy Lists (HTTP/HTTPS)
 
 - [SSL Proxies](https://www.sslproxies.org/)
 - [Free Proxy List](https://free-proxy-list.net)
```

### Comparing `free_verify_proxy-1.1.6/free_verify_proxy/free_proxy_verifyer.py` & `free_verify_proxy-1.1.7/free_verify_proxy/free_proxy_verifyer.py`

 * *Files identical despite different names*

### Comparing `free_verify_proxy-1.1.6/free_verify_proxy/free_verify_proxy.py` & `free_verify_proxy-1.1.7/free_verify_proxy/free_verify_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         Args:
             number_of_threads (int, optional): Number of threads to use for verification. Defaults to 100.
 
             timeout (tuple, optional): Timeout for proxy verification. Defaults to (5,5).
             
         """
         proxy_lists = proxyLists().get_free_proxy_lists()
+        if len(proxy_lists) == 0 or number_of_threads+1 > len(proxy_lists):
+            return proxy_lists
         verified_proxies = []
         with concurrent.futures.ThreadPoolExecutor(max_workers=number_of_threads+1) as executor:
             futures = []
             chunk_size = len(proxy_lists) // number_of_threads
             for i in range(0, len(proxy_lists), chunk_size):
                 chunk = proxy_lists[i:i + chunk_size]
                 future = executor.submit(self.verifyer, chunk, timeout)
```

### Comparing `free_verify_proxy-1.1.6/free_verify_proxy/proxy.py` & `free_verify_proxy-1.1.7/free_verify_proxy/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,17 @@
                 except:
                     break
                 for row_1 in table_row:
                     columns_1 = row_1.find_all('td')
                     if len(columns_1)>=8:
                         proxy=f"{columns_1[0].text.strip()}:{columns_1[1].text.strip()}"
                         proxies_list.append(proxy)
-                page+=1
             except:
                 pass
-
+            page+=1
         return proxies_list
 
 
     def get_proxyscrape(self):
         proxies_list=[]
         try:
             url="https://api.proxyscrape.com/v3/free-proxy-list/get?request=displayproxies&protocol=http&country=all&anonymity=elite&timeout=10000&proxy_format=ipport&format=json"
```

### Comparing `free_verify_proxy-1.1.6/free_verify_proxy.egg-info/PKG-INFO` & `free_verify_proxy-1.1.7/free_verify_proxy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: free-verify-proxy
-Version: 1.1.6
+Version: 1.1.7
 Summary: A simple package to provide http and https working proxy lists.
 Home-page: https://github.com/mominurr/free_verify_proxy
 Author: Mominur Rahman
 Author-email: mominurr518@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # free_verify_proxy
 
 free_verify_proxy is a Python library that collects free proxy from different sources and verifies whether the proxy is working or not. It checks the functionality of given proxies by making requests to various proxy detection servers. This library is useful for anyone who needs to ensure the reliability of proxies for their applications.
 
+# NOTE:
+if collected proxy lists are smaller than number_of_threads then it is not verified proxy lists. Just return collected proxy lists.
 
 # Proxy Sources
 
 ## Public Proxy Lists (HTTP/HTTPS)
 
 - [SSL Proxies](https://www.sslproxies.org/)
 - [Free Proxy List](https://free-proxy-list.net)
```

### Comparing `free_verify_proxy-1.1.6/setup.py` & `free_verify_proxy-1.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='free_verify_proxy',
-    version='1.1.6',
+    version='1.1.7',
     author='Mominur Rahman',
     author_email='mominurr518@email.com',
     description='A simple package to provide http and https working proxy lists.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/mominurr/free_verify_proxy',
     packages=find_packages(),
```

