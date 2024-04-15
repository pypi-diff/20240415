# Comparing `tmp/brainchain-0.5.6.tar.gz` & `tmp/brainchain-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.5.6.tar", max compression
+gzip compressed data, was "brainchain-0.6.0.tar", max compression
```

## Comparing `brainchain-0.5.6.tar` & `brainchain-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,29 @@
--rw-r--r--   0        0        0     6148 2024-02-29 23:10:12.853551 brainchain-0.5.6/brainchain/.DS_Store
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.5.6/brainchain/README.md
--rw-r--r--   0        0        0      671 2024-03-18 16:25:05.143847 brainchain-0.5.6/brainchain/__init__.py
--rw-r--r--   0        0        0    10754 2024-03-18 16:26:52.660488 brainchain-0.5.6/brainchain/brainchain.py
--rw-r--r--   0        0        0     5579 2023-06-20 22:25:05.537647 brainchain-0.5.6/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.5.6/brainchain/coredata.py
--rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.5.6/brainchain/embeddings.py
--rw-r--r--   0        0        0    11209 2024-03-18 16:29:20.116019 brainchain-0.5.6/brainchain/products.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.5.6/brainchain/requirements.txt
--rw-r--r--   0        0        0     6024 2024-02-29 23:10:12.854589 brainchain-0.5.6/brainchain/sales_intel.py
--rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.5.6/brainchain/search_v2.py
--rw-r--r--   0        0        0      595 2024-02-29 23:10:12.855052 brainchain-0.5.6/brainchain/tools/__init__.py
--rw-r--r--   0        0        0     2118 2024-03-18 16:28:06.150540 brainchain-0.5.6/brainchain/tools/coding.py
--rw-r--r--   0        0        0     3869 2024-02-29 23:10:12.855432 brainchain-0.5.6/brainchain/tools/diffbot.py
--rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.5.6/brainchain/tools/factual.py
--rw-r--r--   0        0        0     5800 2024-02-29 23:10:12.855739 brainchain-0.5.6/brainchain/tools/fts.py
--rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.5.6/brainchain/tools/graph.py
--rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.5.6/brainchain/tools/memory.py
--rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.5.6/brainchain/tools/plan.py
--rw-r--r--   0        0        0     1660 2024-02-29 23:10:12.857333 brainchain-0.5.6/brainchain/tools/tokens.py
--rw-r--r--   0        0        0    20787 2024-02-29 23:10:12.857688 brainchain-0.5.6/brainchain/tools/tools.py
--rw-r--r--   0        0        0    10396 2024-03-18 16:19:24.356450 brainchain-0.5.6/brainchain/tools/web.py
--rw-r--r--   0        0        0      731 2024-02-29 23:10:12.854896 brainchain-0.5.6/brainchain/tools.py
--rw-r--r--   0        0        0      538 2024-03-18 16:28:59.632335 brainchain-0.5.6/pyproject.toml
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.5.6/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-04-10 15:41:29.802452 brainchain-0.6.0/brainchain/.DS_Store
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.6.0/brainchain/README.md
+-rw-r--r--   0        0        0      671 2024-04-15 19:33:12.465156 brainchain-0.6.0/brainchain/__init__.py
+-rw-r--r--   0        0        0    13624 2024-04-15 19:41:12.625248 brainchain-0.6.0/brainchain/assistants
+-rw-r--r--   0        0        0    13624 2024-04-15 19:52:38.518975 brainchain-0.6.0/brainchain/assistants.py
+-rw-r--r--   0        0        0    17664 2024-04-15 19:52:45.029786 brainchain-0.6.0/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5663 2024-03-27 22:17:28.214003 brainchain-0.6.0/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.6.0/brainchain/coredata.py
+-rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.6.0/brainchain/embeddings.py
+-rw-r--r--   0        0        0     3426 2024-04-15 19:43:17.579942 brainchain-0.6.0/brainchain/logger.py
+-rw-r--r--   0        0        0    11498 2024-03-19 23:11:27.374089 brainchain-0.6.0/brainchain/products.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.6.0/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6024 2024-02-29 23:10:12.854589 brainchain-0.6.0/brainchain/sales_intel.py
+-rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.6.0/brainchain/search_v2.py
+-rw-r--r--   0        0        0     6148 2024-03-18 17:43:54.835290 brainchain-0.6.0/brainchain/tools/.DS_Store
+-rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.6.0/brainchain/tools/__init__.py
+-rw-r--r--   0        0        0     2118 2024-03-18 17:46:16.438013 brainchain-0.6.0/brainchain/tools/coding.py
+-rw-r--r--   0        0        0     3948 2024-04-15 19:12:36.615790 brainchain-0.6.0/brainchain/tools/diffbot.py
+-rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.6.0/brainchain/tools/factual.py
+-rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.6.0/brainchain/tools/fts.py
+-rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.6.0/brainchain/tools/graph.py
+-rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.6.0/brainchain/tools/memory.py
+-rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.6.0/brainchain/tools/plan.py
+-rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.6.0/brainchain/tools/tokens.py
+-rw-r--r--   0        0        0    20787 2024-04-15 19:32:38.611665 brainchain-0.6.0/brainchain/tools/tools.py
+-rw-r--r--   0        0        0    10427 2024-04-10 00:54:22.728479 brainchain-0.6.0/brainchain/tools/web.py
+-rw-r--r--   0        0        0      731 2024-04-15 19:33:06.073495 brainchain-0.6.0/brainchain/tools.py
+-rw-r--r--   0        0        0      538 2024-04-15 19:45:20.212527 brainchain-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.6.0/PKG-INFO
```

### Comparing `brainchain-0.5.6/brainchain/.DS_Store` & `brainchain-0.6.0/brainchain/.DS_Store`

 * *Files 21% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0002 0000 0005  ................
 00000110: 0074 006f 006f 006c 0073 6277 7370 626c  .t.o.o.l.sbwspbl
-00000120: 6f62 0000 00b7 6270 6c69 7374 3030 d601  ob....bplist00..
-00000130: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
+00000120: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
+00000130: 0203 0405 0607 0808 080b 085d 5368 6f77  ...........]Show
 00000140: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 00000150: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 00000160: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 00000170: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00000180: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00000190: 7208 0908 095f 1017 7b7b 3433 2c20 3234  r...._..{{43, 24
-000001a0: 327d 2c20 7b39 3230 2c20 3433 367d 7d09  2}, {920, 436}}.
-000001b0: 0815 232f 3b52 5f6b 6c6d 6e6f 8900 0000  ..#/;R_klmno....
-000001c0: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
-000001d0: 0000 0000 0000 0000 0000 0000 8a00 0000  ................
-000001e0: 0500 7400 6f00 6f00 6c00 7376 5372 6e6c  ..t.o.o.l.svSrnl
-000001f0: 6f6e 6700 0000 0100 0000 0000 0000 0000  ong.............
+00000190: 7208 0909 095f 1018 7b7b 3236 382c 2032  r...._..{{268, 2
+000001a0: 3338 7d2c 207b 3932 302c 2034 3336 7d7d  38}, {920, 436}}
+000001b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
+000001c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
+000001d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
+000001e0: 0005 0074 006f 006f 006c 0073 7653 726e  ...t.o.o.l.svSrn
+000001f0: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `brainchain-0.5.6/brainchain/README.md` & `brainchain-0.6.0/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/__init__.py` & `brainchain-0.6.0/brainchain/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/carnivore.py` & `brainchain-0.6.0/brainchain/carnivore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json, os, requests
 from urllib.parse import quote
 import promptlayer
 from promptlayer import openai
+import tiktoken
 from modal import Image, Stub, web_endpoint, Secret
 
 try:
     stub = Stub(f"carnivore-client-{os.environ['USER']}")
 except:
     stub = Stub(f"carnivore-client-guest")
 
@@ -55,15 +56,15 @@
 
     def analyze_content(self, link, tags="*", tag_delimiter=" "):
         contents_metadata = {}
         enc = tiktoken.encoding_for_model("gpt-3.5-turbo-16k-0613")
         content_store = []
         running_length = 0
         extracted = []
-
+        from langchain.document_loaders import UnstructuredURLLoader
         loader = UnstructuredURLLoader([link])
         d = loader.load()
         print(d)
         for i, doc in enumerate(d):
             print(f"running_length: {running_length}")
             tokens_in_doc = len(enc.encode(doc.page_content))
             if tokens_in_doc + running_length <= 16384-50:
```

### Comparing `brainchain-0.5.6/brainchain/coredata.py` & `brainchain-0.6.0/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/embeddings.py` & `brainchain-0.6.0/brainchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/products.py` & `brainchain-0.6.0/brainchain/products.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     """
     # Convert the datetime object to a Unix timestamp (in seconds)
     unix_timestamp_seconds = int(date_obj.timestamp())
     # Correct the conversion process: apply the Keepa-specific adjustments
     keepa_timestamp = (unix_timestamp_seconds // 60) - 21564000
     return keepa_timestamp
 
+import time
 class ProductsAPI():
     def __init__(self, base_url: str = "http://localhost:8000"):
         self.base_url = base_url
         self.wd = WebDataClient()
         self.session = requests.Session()
     
     base_url: str = "http://localhost:8000"
@@ -76,15 +77,15 @@
         Returns:
             str: The normalized search query.
         """
         # Add normalization logic here
         return query
     
 
-    def search_keepa_and_save(self, asins: List[str] = [], max_products: int = 5, title: str = "", offers: int = 20, trackingSince_lte: dt = dt.now(), trackingSince_gte: dt = dt.now() - td(days=365)) -> List[Dict]:
+    def search_keepa_and_save(self, asins: List[str] = [], max_products: int = 5, title: str = "", offers: int = 20, trackingSince_lte: dt = dt.now(), trackingSince_gte: dt = dt.now() - td(days=30)) -> List[Dict]:
         """
         Searches products on Keepa via WebDataClient and saves them to the database.
         
         Args:
             search_query (str): The search query for finding products.
         
         Returns:
@@ -97,63 +98,67 @@
         # each of those asins, from find_and_query, you'll get back a large dict of asin -> {info: ... , history: price_history... }'
         # 4 create product_instance_price_id from product_instance_id, price, date from the prices for the individual product instances using the existing methods
         # 5 save the product, product_instance, and product_instance_price to the database
 
 
         # 1. Create a product
         product_response = self.create_product(name=title)
+        # print("Product Response: ", product_response)
 
-        product_info = self.wd.find_and_query(asins=asins, title=title, trackingSince_gte=trackingSince_gte, trackingSince_lte=trackingSince_lte, offers=offers, history=False)[0:max_products]
+        product_info = self.wd.find_and_query(asins=asins, title=title, trackingSince_gte=trackingSince_gte, trackingSince_lte=trackingSince_lte, offers=offers, max_products=max_products, history=False)[0:max_products]
+        time.sleep(1)
         asin_product_map = {}
 
         for product in product_info:
-            print(product)
+            #print(product)
             history = self.wd.find_and_query(asins=[product["asin"]], title=title, trackingSince_gte=trackingSince_gte, trackingSince_lte=trackingSince_lte, offers=100, history=True)
-            print(history)
+            #print(history)
             
             asin_product_map[product["asin"]] = {"info": product, "history": history}
-            print(json.dumps(asin_product_map, indent=2))
+            # print(json.dumps(asin_product_map, indent=2))
 
         for asin, details in asin_product_map.items():
             # 2. Create a product instance
             # KEEPA OUTPUT: 
+            #print("product_response: ", product_response)
 
             instance_data = {
                 "product_id": product_response["product_id"],
                 "asin": asin,
                 "title": title,
                 "number_of_items": details["info"]["numberOfItems"],
-                # "package_height": details["info"]["packageHeight"],
-                # "package_length": details["info"]["packageLength"],
-                # "package_width": details["info"]["packageWidth"],
-                # "package_weight": details["info"]["packageWeight"],
+                "package_height": details["info"]["packageHeight"],
+                "package_length": details["info"]["packageLength"],
+                "package_width": details["info"]["packageWidth"],
+                "package_weight": details["info"]["packageWeight"],
                 "description": details["info"]["description"],
                 "brand": details["info"]["brand"],
                 "features": details["info"]["features"],
                 "manufacturer": details["info"]["manufacturer"],
+                "categories": list(map(lambda x: str(x), details["info"]["categories"])),
                 "category_tree": details["info"]["categoryTree"],
                 'listed_since': keepa_int_to_datetime(details["info"]['listedSince']).strftime("%Y-%m-%d %H:%M:%S"),
                 'last_update': keepa_int_to_datetime(details["info"]['lastUpdate']).strftime("%Y-%m-%d %H:%M:%S"),
                 'last_price_change': keepa_int_to_datetime(details["info"]["lastPriceChange"]).strftime("%Y-%m-%d %H:%M:%S"),
                 "ean_list": details["info"]["eanList"],
                 "upc_list": details["info"]["upcList"]
             }
 
-            print("Instance Data: ", instance_data)
+            #print("Instance Data: ", instance_data)
             instance_response = self.create_product_instance(instance_data)
             print(instance_response)
             price_history = self.wd.query_product(ProductQueryPayload(items=[asin], options=QueryOptions(history=True)))
-            print(price_history)
+            #print(price_history)
             if price_history:
-                print("Price History: ", price_history)
+                #print("Price History: ", price_history)
                 for price in price_history:
                     # 3. Create a product instance price
-                    print(price)
+                    #print(price)
                     if len(price) == 2:
-
+                        
                         price_data = {
                             "product_instance_uuid": instance_response["uuid"],
                             "price": price[1],
                             "date": price[0],
                         }
                         
                         price_response = self.create_product_instance_price(price_data)
```

### Comparing `brainchain-0.5.6/brainchain/requirements.txt` & `brainchain-0.6.0/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/sales_intel.py` & `brainchain-0.6.0/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/search_v2.py` & `brainchain-0.6.0/brainchain/search_v2.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/__init__.py` & `brainchain-0.6.0/brainchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/coding.py` & `brainchain-0.6.0/brainchain/tools/coding.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/diffbot.py` & `brainchain-0.6.0/brainchain/tools/diffbot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-import json, os, requests
+import json
+import os
+import requests
+from pydantic import BaseModel
+from typing import List
 
 def diffbot_analyze(url: str, mode: str = None, fallback: str = None, fields: str = None, discussion: bool = None, timeout: int = 30000, proxy: str = None, proxyAuth: str = None, useProxy: str = None) -> dict:
     """
     Makes a request to the Diffbot Analyze API and returns the structured data.
     
     :param url: The URL of the web page to analyze.
     :param mode: Specific Extract API to use (optional).
@@ -12,17 +16,17 @@
     :param timeout: Timeout in milliseconds for the request (default 30000).
     :param proxy: Custom proxy IP address (optional).
     :param proxyAuth: Authentication parameters for the custom proxy (optional).
     :param useProxy: Use custom or no proxy (optional).
     :return: A dictionary with the structured data.
     """
 
-    backslash = """n
+    backslash = '''n
         \\
-    """
+    '''
     url = url
     print(url)
     # Construct the API endpoint
     api_endpoint = "https://api.diffbot.com/v3/analyze"
     params = {
         "url": url.replace("\\", ""),
         "token": os.environ["DIFFBOT_API_KEY"],  # Replace with your actual API token
@@ -38,19 +42,19 @@
 
     import requests
 
     class TokenizerClient:
         def __init__(self, base_url = "https://brainchain--token-service.modal.run"):
             self.base_url = base_url
 
-        def encode_text(self, text: str, backend: str = "openai", model: str = "gpt-3.5-turbo-16k", tokenizer: str = "cl100k_base"):
+        def encode_text(self, text: List[str], backend: str = "openai", model: str = "gpt-3.5-turbo-16k", tokenizer: str = "cl100k_base"):
             url = f"{self.base_url}/encode"
             headers = {"Content-Type": "application/json"}
             data = {
-                "text": text,
+                "texts": [text],
                 "backend": backend,
                 "model": model,
                 "tokenizer": tokenizer
             }
 
             response = requests.post(url, headers=headers, json=data)
 
@@ -82,15 +86,15 @@
 
     tokenizer = TokenizerClient()    
     # Make the GET request
     response = requests.get(api_endpoint, params=params)
 
     # Check for successful response
     if response.status_code == 200:
-        if tokenizer.encode_text(response.text)["token_count"] > 63000:
+        if tokenizer.encode_text(response.text)[0]["token_count"] > 63000:
             return "The response from Diffbot is too large to process. Tell the user to ask the chatbot to upload the file to the FTS Service."
         else:
             return json.loads(response.text)
     else:
         raise Exception(f"Error {response.status_code}: {response.text}")
 
     return {}
```

### Comparing `brainchain-0.5.6/brainchain/tools/factual.py` & `brainchain-0.6.0/brainchain/tools/factual.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/fts.py` & `brainchain-0.6.0/brainchain/tools/fts.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/graph.py` & `brainchain-0.6.0/brainchain/tools/graph.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/memory.py` & `brainchain-0.6.0/brainchain/tools/memory.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/plan.py` & `brainchain-0.6.0/brainchain/tools/plan.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/tokens.py` & `brainchain-0.6.0/brainchain/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/tools.py` & `brainchain-0.6.0/brainchain/tools/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/brainchain/tools/web.py` & `brainchain-0.6.0/brainchain/tools/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,14 +217,15 @@
     def find_and_query(
         self,
         title: Optional[str],
         asins: Optional[List[str]] = [],
         trackingSince_gte: Optional[dt] = dt.now() - td(days=30),
         trackingSince_lte: Optional[dt] = dt.now(),
         offers: int = 20,
+        max_products: int = 5,
         history: bool = True,
     ) -> dict:
         if title:
             params = ProductFinderParameters(
                 title=title, trackingSince_gte=trackingSince_gte.strftime("%Y-%m-%d"), trackingSince_lte=trackingSince_lte.strftime("%Y-%m-%d")
             )
             asins = self.product_finder(params)
```

### Comparing `brainchain-0.5.6/brainchain/tools.py` & `brainchain-0.6.0/brainchain/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.5.6/pyproject.toml` & `brainchain-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.5.6"
+version = "0.6.0"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 urllib3 = "2.0.6"
 requests = "2.31.0"
```

### Comparing `brainchain-0.5.6/PKG-INFO` & `brainchain-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.5.6
+Version: 0.6.0
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

