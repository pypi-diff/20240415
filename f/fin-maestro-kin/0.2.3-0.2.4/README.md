# Comparing `tmp/fin_maestro_kin-0.2.3.tar.gz` & `tmp/fin_maestro_kin-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_maestro_kin-0.2.3.tar", max compression
+gzip compressed data, was "fin_maestro_kin-0.2.4.tar", max compression
```

## Comparing `fin_maestro_kin-0.2.3.tar` & `fin_maestro_kin-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/__init__.py
--rw-r--r--   0        0        0     1606 2024-04-12 20:53:43.495343 fin_maestro_kin-0.2.3/fin_maestro_kin/constants.py
--rw-r--r--   0        0        0      675 2024-04-12 19:12:33.740169 fin_maestro_kin-0.2.3/fin_maestro_kin/main.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/__init__.py
--rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
--rw-r--r--   0        0        0    12569 2024-04-12 20:19:01.630418 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/helper.py
--rw-r--r--   0        0        0    19034 2024-04-12 20:25:36.577477 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
--rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
--rw-r--r--   0        0        0        0 2024-04-12 15:03:25.791170 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
--rw-r--r--   0        0        0      514 2024-04-12 20:45:58.837209 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/helper.py
--rw-r--r--   0        0        0     1865 2024-04-12 20:45:18.468552 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/__init__.py
--rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
--rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/trend_detector/__init__.py
--rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/trend_detector/trend_detector.py
--rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.3/LICENSE
--rw-r--r--   0        0        0      642 2024-04-13 06:33:03.660401 fin_maestro_kin-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     5339 2024-03-31 06:18:04.202217 fin_maestro_kin-0.2.3/README.md
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/__init__.py
+-rw-r--r--   0        0        0     1606 2024-04-13 06:37:31.640875 fin_maestro_kin-0.2.4/fin_maestro_kin/constants.py
+-rw-r--r--   0        0        0     1025 2024-04-15 18:30:00.477406 fin_maestro_kin-0.2.4/fin_maestro_kin/main.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/__init__.py
+-rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
+-rw-r--r--   0        0        0    12705 2024-04-15 18:39:19.947514 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/helper.py
+-rw-r--r--   0        0        0    19042 2024-04-15 18:33:45.624559 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
+-rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
+-rw-r--r--   0        0        0        0 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-13 06:37:31.671927 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/helper.py
+-rw-r--r--   0        0        0     1865 2024-04-13 06:37:31.687590 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
+-rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/trend_detector/__init__.py
+-rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.4/fin_maestro_kin/modules/trend_detector/trend_detector.py
+-rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.4/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-15 18:48:30.804605 fin_maestro_kin-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     5347 2024-04-15 16:54:12.969094 fin_maestro_kin-0.2.4/README.md
+-rw-r--r--   0        0        0     6235 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.4/PKG-INFO
```

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/constants.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/constants.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/helper.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,21 +165,25 @@
 
 
 def process_most_active_securities_data(data):
     rounded_data = convert_dataframe_to_dict(data)
     processed_data = []
     for entry in rounded_data:
         processed_entry = {
-            "security": entry["ASM_SECURITY"],
-            "average_daily_turnover": entry["ASM_AVG_DLY_TURNOVER"],
-            "number_of_trades": entry["ASM_NO_OF_TRADES"],
-            "share_in_total_turnover": entry["ASM_SHARE_IN_TOTAL_TURNOVER"],
-            "traded_quantity": entry["ASM_TRADED_QUANTITY"],
-            "turnover": entry["ASM_TURNOVER"],
-            "timestamp": entry["TIMESTAMP"]
+            "symbol": entry["symbol"],
+            "last_price": entry["lastPrice"],
+            "percentage_change": entry["pChange"],
+            "total_traded_volume": entry["totalTradedVolume"],
+            "traded_quantity": entry["quantityTraded"],
+            "total_traded_value": entry["totalTradedValue"],
+            "previous_close": entry["previousClose"],
+            "ex_date": entry["exDate"],
+            "purpose": entry["purpose"],
+            "year_high": entry["yearHigh"],
+            "year_low": entry["yearLow"]
         }
         processed_data.append(processed_entry)
     return processed_data
 
 
 def process_monthly_advances_declines_data(data):
     rounded_data = convert_dataframe_to_dict(data)
```

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         processed_data = process_corporate_actions_data(data)
         return JSONResponse(content={"corporate_actions_data": processed_data})
     except Exception as e:
         raise HTTPException(status_code=500, detail=f"Error fetching corporate actions data: {e}")
     
 
 def nse_monthly_most_active_securities():
-    request_url = "https://www.nseindia.com/api/historical/most-active-securities-monthly"
+    request_url = "https://www.nseindia.com/api/live-analysis-most-active-securities?index=volume"
     response = fetch_data_from_nse(request_url)
     payload = response.get('data', [])
     
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
```

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/helper.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/helper.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/trend_detector/trend_detector.py` & `fin_maestro_kin-0.2.4/fin_maestro_kin/modules/trend_detector/trend_detector.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/LICENSE` & `fin_maestro_kin-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.3/pyproject.toml` & `fin_maestro_kin-0.2.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fin-maestro-kin"
-version = "0.2.3"
+version = "0.2.4"
 description = "Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API."
 authors = ["DEV_FINWIZ <devjuneja43@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `fin_maestro_kin-0.2.3/README.md` & `fin_maestro_kin-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,8 +83,8 @@
    - Enter http://localhost:8000/docs in the address bar to access the Fin-Maestro-Kin API documentation.
 
 4. **Additional Docker Desktop Features:**
    - Docker Desktop provides a user-friendly graphical interface for managing Docker containers.
    - You can monitor container status, view container logs, and interact with running containers using the Docker Desktop GUI.
 
 ## Usage
-After deploying the container, interact with Fin Maestro Kin by sending HTTP requests to the exposed endpoints. Refer to the API [documentation](http://localhost:8000/docs) for detailed information on available endpoints and request formats.
+After deploying the container, interact with Fin Maestro Kin by sending HTTP requests to the exposed endpoints. Refer to the API [documentation](https://fin-maestro-kin.apidog.io/) for detailed information on available endpoints and request formats.
```

#### html2text {}

```diff
@@ -54,9 +54,10 @@
 container is running, access the application by opening a web browser. - Enter
 http://localhost:8000/docs in the address bar to access the Fin-Maestro-Kin API
 documentation. 4. **Additional Docker Desktop Features:** - Docker Desktop
 provides a user-friendly graphical interface for managing Docker containers. -
 You can monitor container status, view container logs, and interact with
 running containers using the Docker Desktop GUI. ## Usage After deploying the
 container, interact with Fin Maestro Kin by sending HTTP requests to the
-exposed endpoints. Refer to the API [documentation](http://localhost:8000/docs)
-for detailed information on available endpoints and request formats.
+exposed endpoints. Refer to the API [documentation](https://fin-maestro-
+kin.apidog.io/) for detailed information on available endpoints and request
+formats.
```

### Comparing `fin_maestro_kin-0.2.3/PKG-INFO` & `fin_maestro_kin-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fin-maestro-kin
-Version: 0.2.3
+Version: 0.2.4
 Summary: Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API.
 License: MIT
 Author: DEV_FINWIZ
 Author-email: devjuneja43@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -108,9 +108,9 @@
    - Enter http://localhost:8000/docs in the address bar to access the Fin-Maestro-Kin API documentation.
 
 4. **Additional Docker Desktop Features:**
    - Docker Desktop provides a user-friendly graphical interface for managing Docker containers.
    - You can monitor container status, view container logs, and interact with running containers using the Docker Desktop GUI.
 
 ## Usage
-After deploying the container, interact with Fin Maestro Kin by sending HTTP requests to the exposed endpoints. Refer to the API [documentation](http://localhost:8000/docs) for detailed information on available endpoints and request formats.
+After deploying the container, interact with Fin Maestro Kin by sending HTTP requests to the exposed endpoints. Refer to the API [documentation](https://fin-maestro-kin.apidog.io/) for detailed information on available endpoints and request formats.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.3 Summary: Where Data
+Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.4 Summary: Where Data
 Meets FastAPI Brilliance with Fin-Maestro-Kin â Your All-in-One Finance API.
 License: MIT Author: DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
@@ -67,9 +67,10 @@
 container is running, access the application by opening a web browser. - Enter
 http://localhost:8000/docs in the address bar to access the Fin-Maestro-Kin API
 documentation. 4. **Additional Docker Desktop Features:** - Docker Desktop
 provides a user-friendly graphical interface for managing Docker containers. -
 You can monitor container status, view container logs, and interact with
 running containers using the Docker Desktop GUI. ## Usage After deploying the
 container, interact with Fin Maestro Kin by sending HTTP requests to the
-exposed endpoints. Refer to the API [documentation](http://localhost:8000/docs)
-for detailed information on available endpoints and request formats.
+exposed endpoints. Refer to the API [documentation](https://fin-maestro-
+kin.apidog.io/) for detailed information on available endpoints and request
+formats.
```

