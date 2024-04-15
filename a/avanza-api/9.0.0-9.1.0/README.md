# Comparing `tmp/avanza-api-9.0.0.tar.gz` & `tmp/avanza_api-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avanza-api-9.0.0.tar", last modified: Sat Jan  6 10:51:32 2024, max compression
+gzip compressed data, was "avanza_api-9.1.0.tar", last modified: Mon Apr 15 19:47:49 2024, max compression
```

## Comparing `avanza-api-9.0.0.tar` & `avanza_api-9.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 10:51:32.747921 avanza-api-9.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-06 10:51:25.000000 avanza-api-9.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-01-06 10:51:32.747921 avanza-api-9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-01-06 10:51:25.000000 avanza-api-9.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 10:51:32.743921 avanza-api-9.0.0/avanza/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-01-06 10:51:25.000000 avanza-api-9.0.0/avanza/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    99989 2024-01-06 10:51:25.000000 avanza-api-9.0.0/avanza/avanza.py
--rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-01-06 10:51:25.000000 avanza-api-9.0.0/avanza/avanza_socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-01-06 10:51:25.000000 avanza-api-9.0.0/avanza/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-01-06 10:51:25.000000 avanza-api-9.0.0/avanza/entities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-06 10:51:32.747921 avanza-api-9.0.0/avanza_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-01-06 10:51:32.000000 avanza-api-9.0.0/avanza_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-01-06 10:51:32.000000 avanza-api-9.0.0/avanza_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-06 10:51:32.000000 avanza-api-9.0.0/avanza_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-06 10:51:32.000000 avanza-api-9.0.0/avanza_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-06 10:51:32.000000 avanza-api-9.0.0/avanza_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-06 10:51:32.747921 avanza-api-9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-01-06 10:51:25.000000 avanza-api-9.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:47:49.941053 avanza_api-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-15 19:47:41.000000 avanza_api-9.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-15 19:47:49.941053 avanza_api-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-04-15 19:47:41.000000 avanza_api-9.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:47:49.941053 avanza_api-9.1.0/avanza/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101813 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/avanza.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6785 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/avanza_socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-15 19:47:41.000000 avanza_api-9.1.0/avanza/entities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:47:49.941053 avanza_api-9.1.0/avanza_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 19:47:49.000000 avanza_api-9.1.0/avanza_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 19:47:49.941053 avanza_api-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-15 19:47:41.000000 avanza_api-9.1.0/setup.py
```

### Comparing `avanza-api-9.0.0/LICENSE` & `avanza_api-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `avanza-api-9.0.0/PKG-INFO` & `avanza_api-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avanza-api
-Version: 9.0.0
+Version: 9.1.0
 Summary: A Python library for the unofficial Avanza API
 Home-page: https://github.com/Qluxzz/avanza
 Author: André Andersson
 Author-email: andre.eric.andersson@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `avanza-api-9.0.0/README.md` & `avanza_api-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `avanza-api-9.0.0/avanza/avanza.py` & `avanza_api-9.1.0/avanza/avanza.py`

 * *Files 1% similar despite different names*

```diff
@@ -801,14 +801,75 @@
             }
         """
         return self.__call(
             HttpMethod.GET,
             Route.ACCOUNTS_POSITIONS_PATH.value
         )
 
+    def get_account_performance_chart_data(self, url_parameters_ids: list[str], time_period: TimePeriod):
+        """ Get performance chart for accounts.
+
+        Args:
+            url_parameters_ids: Scrambled account ids. 
+                Can be found in the overview response.
+            time_period: Time period to get chart data for
+
+        Returns:
+        {
+            "interval": {
+                "timePeriod": str,
+                "from": str,
+                "to": str,
+            },
+            "absoluteSeries": [
+                {
+                "performance": {
+                    "value": float,
+                    "unit": str,
+                    "unitType": str,
+                "decimalPrecision": int
+                },
+                "timestamp": int
+            }
+            ],
+            "relativeSeries": [
+            {
+                "performance": {
+                    "value": float,
+                    "unit": str,
+                    "unitType": str,
+                    "decimalPrecision": int
+                },
+                "timestamp": int
+                }
+            ],
+            "valueSeries": [
+                {
+                    "performance": {
+                        "value": float,
+                        "unit": str,
+                        "unitType": str,
+                        "decimalPrecision": int
+                    },
+                    "timestamp": int
+                }
+            ],
+            "earliestAvailableDate": str,
+            "timePeriod": str
+        }
+        """
+        return self.__call(
+            HttpMethod.POST,
+            Route.ACCOUNT_PERFORMANCE_CHART_PATH.value,
+            {
+                "scrambledAccountIds": url_parameters_ids, 
+                "timePeriod": time_period.value
+            }
+        )
+    
     def get_watchlists(self):
         """ Get your "Bevakningslistor"
 
         Returns:
 
             [{
                 'editable': bool,
```

### Comparing `avanza-api-9.0.0/avanza/avanza_socket.py` & `avanza_api-9.1.0/avanza/avanza_socket.py`

 * *Files identical despite different names*

### Comparing `avanza-api-9.0.0/avanza/constants.py` & `avanza_api-9.1.0/avanza/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     THREE_MONTHS = 'THREE_MONTHS'
     THIS_YEAR = 'THIS_YEAR'
     ONE_YEAR = 'ONE_YEAR'
     THREE_YEARS = 'THREE_YEARS'
     FIVE_YEARS = 'FIVE_YEARS'
     THREE_YEARS_ROLLING = 'THREE_YEARS_ROLLING'
     FIVE_YEARS_ROLLING = 'FIVE_YEARS_ROLLING'
+    ALL_TIME = 'ALL_TIME'
 
 
 class Resolution(enum.Enum):
     MINUTE = 'MINUTE'
     TWO_MINUTES = 'TWO_MINUTES'
     FIVE_MINUTES = 'FIVE_MINUTES'
     TEN_MINUTES = 'TEN_MINUTES'
@@ -102,14 +103,15 @@
     POST = 1
     GET = 2
     PUT = 3
     DELETE = 4
 
 class Route(enum.Enum):
     ACCOUNTS_POSITIONS_PATH = '/_api/position-data/positions'
+    ACCOUNT_PERFORMANCE_CHART_PATH = '/_api/account-performance/overview/chart/accounts/timeperiod'
     AUTHENTICATION_PATH = '/_api/authentication/sessions/usercredentials'
     CATEGORIZED_ACCOUNTS = '/_api/account-overview/overview/categorizedAccounts'
     CHARTDATA_PATH = '/_api/price-chart/stock/{}'
     CURRENT_OFFERS_PATH = '/_api/customer-offer/currentoffers/'
     DEALS_AND_ORDERS_PATH = '/_mobile/account/dealsandorders'
     FUND_PATH = '/_api/fund-guide/guide/{}'
     INSIGHTS_PATH = '/_api/insights-development/?timePeriod={}&accountIds={}'
```

### Comparing `avanza-api-9.0.0/avanza/entities.py` & `avanza_api-9.1.0/avanza/entities.py`

 * *Files identical despite different names*

### Comparing `avanza-api-9.0.0/avanza_api.egg-info/PKG-INFO` & `avanza_api-9.1.0/avanza_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avanza-api
-Version: 9.0.0
+Version: 9.1.0
 Summary: A Python library for the unofficial Avanza API
 Home-page: https://github.com/Qluxzz/avanza
 Author: André Andersson
 Author-email: andre.eric.andersson@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `avanza-api-9.0.0/setup.py` & `avanza_api-9.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'avanza-api'
 DESCRIPTION = 'A Python library for the unofficial Avanza API'
 URL = 'https://github.com/Qluxzz/avanza'
 EMAIL = 'andre.eric.andersson@gmail.com'
 AUTHOR = 'André Andersson'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '9.0.0'
+VERSION = '9.1.0'
 
 REQUIRED = [
     'requests>=2',
     'pyotp>=2',
     'websockets>=8'
 ]
```

