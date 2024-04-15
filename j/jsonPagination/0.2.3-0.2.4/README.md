# Comparing `tmp/jsonPagination-0.2.3.tar.gz` & `tmp/jsonpagination-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonPagination-0.2.3.tar", last modified: Tue Mar 26 05:50:00 2024, max compression
+gzip compressed data, was "jsonpagination-0.2.4.tar", last modified: Mon Apr 15 15:14:37 2024, max compression
```

## Comparing `jsonPagination-0.2.3.tar` & `jsonpagination-0.2.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 05:50:00.581536 jsonPagination-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-03-26 05:49:56.000000 jsonPagination-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-03-26 05:50:00.581536 jsonPagination-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-03-26 05:49:56.000000 jsonPagination-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 05:50:00.581536 jsonPagination-0.2.3/jsonPagination/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-26 05:49:56.000000 jsonPagination-0.2.3/jsonPagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-26 05:49:56.000000 jsonPagination-0.2.3/jsonPagination/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16858 2024-03-26 05:49:56.000000 jsonPagination-0.2.3/jsonPagination/paginator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 05:50:00.581536 jsonPagination-0.2.3/jsonPagination.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-03-26 05:50:00.000000 jsonPagination-0.2.3/jsonPagination.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-26 05:50:00.000000 jsonPagination-0.2.3/jsonPagination.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 05:50:00.000000 jsonPagination-0.2.3/jsonPagination.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-26 05:50:00.000000 jsonPagination-0.2.3/jsonPagination.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-26 05:50:00.000000 jsonPagination-0.2.3/jsonPagination.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 05:50:00.581536 jsonPagination-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-26 05:49:56.000000 jsonPagination-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35239 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7896 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/jsonPagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/jsonPagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/jsonPagination/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17183 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/jsonPagination/paginator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/jsonPagination.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 15:14:37.000000 jsonpagination-0.2.4/jsonPagination.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 15:14:37.619175 jsonpagination-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-15 15:14:33.000000 jsonpagination-0.2.4/setup.py
```

### Comparing `jsonPagination-0.2.3/LICENSE` & `jsonpagination-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonPagination-0.2.3/PKG-INFO` & `jsonpagination-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonPagination
-Version: 0.2.3
+Version: 0.2.4
 Summary: A versatile JSON data downloader with pagination and multithreading support.
 Home-page: https://github.com/pl0psec/jsonPagination
 Author: pl0psec
 Author-email: contact@pl0psec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonPagination-0.2.3/README.md` & `jsonpagination-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jsonPagination-0.2.3/jsonPagination/exceptions.py` & `jsonpagination-0.2.4/jsonPagination/exceptions.py`

 * *Files identical despite different names*

### Comparing `jsonPagination-0.2.3/jsonPagination/paginator.py` & `jsonpagination-0.2.4/jsonPagination/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,24 @@
     """
     A class for fetching and paginating JSON data from APIs with support for multithreading,
     customizable authentication, and the option to disable SSL verification for HTTP requests.
     """
 
     def __init__(self, login_url=None, auth_data=None, current_page_field=None,
                  current_index_field=None, items_field='per_page', total_count_field='total',
-                 items_per_page=None, max_threads=5, download_one_page_only=False, verify_ssl=True,
+                 items_per_page=None, response_items_field=None, max_threads=5, download_one_page_only=False, verify_ssl=True,
                  data_field='data', log_level='INFO', retry_delay=30, ratelimit=None, headers=None):
         """
         Initializes the Paginator with the given configuration.
 
         Args:
             login_url (str, optional): URL for authentication to retrieve a token.
             auth_data (dict, optional): Credentials required for the login endpoint.
             current_page_field (str, optional): Field name for the current page number in the API request.
+            response_items_field (str, optional): Field name for the current page number in the API response.
             current_index_field (str, optional): Field name for the starting index in the API request (used for APIs that paginate by index rather than by page number).
             items_field (str, optional): Field name for the number of items per page in the API request.
             total_count_field (str, optional): Field name in the API response that holds the total number of items.
             items_per_page (int, optional): The number of items to request per page.
             max_threads (int, optional): Maximum number of threads to use for parallel requests.
             download_one_page_only (bool, optional): Whether to fetch only the first page of data.
             verify_ssl (bool, optional): Whether to verify SSL certificates for HTTP requests.
@@ -75,25 +76,26 @@
         self.verify_ssl = verify_ssl
         self.request_timeout = 120
 
         self.headers = headers if headers is not None else {}
 
         # Pagination
 
-        # Use `current_page_field` if provided, otherwise default to `current_index_field`
+        # Use `current_page_field` if provided, otherwise default to `current_index_field`        
         self.pagination_field = current_page_field if current_page_field else current_index_field
         self.is_page_based = bool(current_page_field)
 
         self.items_field = items_field
         self.total_count_field = total_count_field
         self.items_per_page = items_per_page or 10
 
         self.data_field = data_field
 
         self.items_per_page = items_per_page
+        self.response_items_field = response_items_field or items_per_page
         self.download_one_page_only = download_one_page_only
 
         # Threading
         self.max_threads = max_threads
         self.retry = 5
         self.retry_delay = retry_delay
 
@@ -197,24 +199,27 @@
             if self.last_request_time and (current_time - self.last_request_time) < self.request_interval:
                 sleep_time = self.request_interval - (current_time - self.last_request_time)
                 self.logger.debug("Rate limiting in effect, sleeping for %.2f seconds", sleep_time)
                 time.sleep(sleep_time)
 
             self.last_request_time = time.time()
 
-    def fetch_page(self, url, params, page, results, pbar=None):
+    def fetch_page(self, url, params, page, results, pbar=None, callback=None):
         """
         Fetches a single page of data from the API and updates the progress bar.
 
+        If a callback is provided, it is invoked after successfully fetching the page data.
+
         Args:
             url (str): The API endpoint URL.
             params (dict): Additional parameters to pass in the request.
             page (int): The page number to fetch.
             results (list): The list to which fetched data will be appended.
             pbar (tqdm, optional): A tqdm progress bar instance to update with progress.
+            callback (function, optional): A callback function to be invoked after each page is fetched.
         """
         def make_request():
             # Rate limiting enforcement
             self.enforce_ratelimit()
 
             # Update the params with the appropriate pagination parameters
             if self.is_page_based:
@@ -229,18 +234,24 @@
             # Construct the full URL for logging and request
             response = requests.get(url, headers=self.headers, params=params, timeout=self.request_timeout, verify=self.verify_ssl)
             self.logger.debug("Requesting URL: %s with status code: %d", response.request.url, response.status_code)
 
             if response.status_code == 200:
                 data = response.json()
                 fetched_data = data.get(self.data_field, []) if self.data_field else data
+
                 with self.retry_lock:
                     results.extend(fetched_data)
+
+                if callback:  # Invoke the callback function with the fetched data
+                    callback(fetched_data, 'page_fetch')  # Or any other step identifier
+
                 if pbar:
                     pbar.update(len(fetched_data))
+
                 return True
 
             if response.status_code == 401:
                 self.logger.error("Authentication failed with status code %d : %s", response.status_code, response.text)
                 raise AuthenticationFailed(f"Authentication failed with status code {response.status_code}")
 
             if response.status_code == 403:
@@ -249,15 +260,14 @@
                     time.sleep(10)  # Sleep and then retry the current request
                     self.last_request_time = time.time()  # Update the rate limit enforcement time
                     return False
 
                 self.logger.error("Access denied with status code %d : %s", response.status_code, response.text)
                 raise AuthenticationFailed(f"Access denied with status code {response.status_code}")
 
-
             return False  # Indicate that fetch was unsuccessful
 
         retries = self.retry
         while retries > 0:
             try:
                 success = make_request()
                 if success:
@@ -267,42 +277,30 @@
                 self.logger.warning("Retrying page %d after %d seconds, remaining retries: %d", page, self.retry_delay, retries)
                 time.sleep(self.retry_delay)  # Wait before retrying
             except RequestException as e:
                 self.logger.error("Network error fetching page %d: %s", page, e)
                 retries -= 1
                 time.sleep(self.retry_delay)  # Wait before retrying
 
-
-    def fetch_all_pages(self, url, params=None, flatten_json=False, headers=None):
+    def fetch_all_pages(self, url, params=None, flatten_json=False, headers=None, callback=None):
         """
         Fetches all pages of data from a paginated API endpoint, optionally flattening the JSON
-        structure of the results.
-
-        This method handles authentication (if necessary), iterates over all pages of the endpoint,
-        and can flatten the nested JSON structure of the returned data.
+        structure of the results. Invokes a callback function after each page if provided.
 
         Args:
             url (str): The URL of the API endpoint to fetch data from.
             params (dict, optional): Additional query parameters to include in the request.
             flatten_json (bool, optional): If set to True, the returned JSON structure will be
-                                        flattened. Defaults to False.
+                                           flattened. Defaults to False.
+            callback (function, optional): A callback function that is called after each page is fetched.
 
         Returns:
             list or dict: A list of JSON objects fetched from the API if `flatten_json` is False.
-                        If `flatten_json` is True, a single-level dictionary representing the
-                        flattened JSON structure is returned.
-
-        Raises:
-            DataFetchFailedException: If the initial request to the API fails.
-            ValueError: If required pagination fields are missing in the API response.
-
-        Note:
-            The method will automatically paginate through all available pages based on the
-            response's pagination fields. If pagination fields are missing, it returns the raw
-            response from the first request.
+                          If `flatten_json` is True, a single-level dictionary representing the
+                          flattened JSON structure is returned.
         """
         if not params:
             params = {}
 
         # Merge instance headers with method-specific headers, if any
 
         if self.login_url and not self.token and self.auth_data:
@@ -330,16 +328,22 @@
         json_data = response.json()
         total_count = json_data.get(self.total_count_field)
         if total_count is None:
             self.logger.warning("Total count field missing, cannot paginate properly.")
             return self.flatten_json(json_data) if flatten_json else json_data
 
         # Set items_per_page based on the initial API call if not set
-        if not self.items_per_page:
-            self.items_per_page = json_data.get(self.items_field, 200)  # Default to 200 if not specified
+        # if not self.items_per_page:
+            # self.items_per_page = json_data.get(self.items_field, 200)  # Default to 200 if not specified
+
+        # Set items_per_page based on the response, dynamically choosing the field or defaulting as necessary         
+        if self.response_items_field and self.response_items_field in json_data:
+            self.items_per_page = json_data.get(self.response_items_field)
+        else:
+            self.items_per_page = json_data.get(self.items_field, 200)
 
         # Determine pagination strategy
         if self.is_page_based:
             total_pages = 1 if self.download_one_page_only else max(-(-total_count // self.items_per_page), 1)
         else:  # Index-based pagination
             # Calculate how many sets of data (each of size 'items_per_page') are needed to cover 'total_count'
             total_pages = 1 if self.download_one_page_only else max(-(-total_count // self.items_per_page), 1)
@@ -348,28 +352,25 @@
 
         results = []
         with tqdm(total=total_count, desc="Downloading items") as pbar:
             threads = []
             for page in range(1, total_pages + 1):
                 page_params = params.copy()
 
-                if self.is_page_based:
-                    page_params[self.pagination_field] = page
-                else:  # Assuming each 'page' in index-based pagination fetches `items_per_page` items
-                    page_params[self.pagination_field] = (page - 1) * self.items_per_page
+                # Existing pagination logic...
 
-                thread = Thread(target=self.fetch_page, args=(url, page_params, page, results, pbar))
+                thread = Thread(target=self.fetch_page, args=(url, page_params, page, results, pbar, callback))
                 thread.start()
                 threads.append(thread)
 
                 if len(threads) >= self.max_threads:
                     for t in threads:
                         t.join()
                     threads = []
 
             for t in threads:
                 t.join()
 
         while not self.data_queue.empty():
             results.extend(self.data_queue.get())
-
+        
         return [self.flatten_json(item) if flatten_json else item for item in results]
```

### Comparing `jsonPagination-0.2.3/jsonPagination.egg-info/PKG-INFO` & `jsonpagination-0.2.4/jsonPagination.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonPagination
-Version: 0.2.3
+Version: 0.2.4
 Summary: A versatile JSON data downloader with pagination and multithreading support.
 Home-page: https://github.com/pl0psec/jsonPagination
 Author: pl0psec
 Author-email: contact@pl0psec.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonPagination-0.2.3/setup.py` & `jsonpagination-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='jsonPagination',
-    version='0.2.3',
+    version='0.2.4',
     author='pl0psec',
     author_email='contact@pl0psec.com',
     description='A versatile JSON data downloader with pagination and multithreading support.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pl0psec/jsonPagination',
     packages=find_packages(),
```

