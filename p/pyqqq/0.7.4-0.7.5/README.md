# Comparing `tmp/pyqqq-0.7.4.tar.gz` & `tmp/pyqqq-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq-0.7.4.tar", max compression
+gzip compressed data, was "pyqqq-0.7.5.tar", max compression
```

## Comparing `pyqqq-0.7.4.tar` & `pyqqq-0.7.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.4/README.md
--rw-r--r--   0        0        0      770 2024-04-12 06:26:03.418307 pyqqq-0.7.4/pyproject.toml
--rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.4/pyqqq/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.4/pyqqq/brokerage/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.4/pyqqq/brokerage/ebest/__init__.py
--rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.4/pyqqq/brokerage/ebest/domestic_stock.py
--rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.4/pyqqq/brokerage/ebest/oauth.py
--rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.4/pyqqq/brokerage/ebest/simple.py
--rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.4/pyqqq/brokerage/ebest/tr_client.py
--rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.4/pyqqq/brokerage/kis/__init__.py
--rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.4/pyqqq/brokerage/kis/domestic_stock.py
--rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.4/pyqqq/brokerage/kis/oauth.py
--rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.4/pyqqq/brokerage/kis/overseas_stock.py
--rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.4/pyqqq/brokerage/kis/simple.py
--rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.4/pyqqq/brokerage/kis/tr_client.py
--rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.4/pyqqq/config.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.4/pyqqq/data/__init__.py
--rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.4/pyqqq/data/domestic.py
--rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.4/pyqqq/data/minutes.py
--rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.4/pyqqq/data/realtime.py
--rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.4/pyqqq/data/ticks.py
--rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.4/pyqqq/datatypes.py
--rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.4/pyqqq/executors/__init__.py
--rw-r--r--   0        0        0    37232 2024-04-12 05:34:14.147583 pyqqq-0.7.4/pyqqq/executors/hook.py
--rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.4/pyqqq/utils/__init__.py
--rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.4/pyqqq/utils/array.py
--rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.4/pyqqq/utils/display.py
--rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.4/pyqqq/utils/kvstore.py
--rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.4/pyqqq/utils/limiter.py
--rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.4/pyqqq/utils/logger.py
--rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.4/pyqqq/utils/market_schedule.py
--rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.4/pyqqq/utils/retry.py
--rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0      588 2024-03-22 02:18:48.554710 pyqqq-0.7.5/README.md
+-rw-r--r--   0        0        0      770 2024-04-15 01:46:57.812691 pyqqq-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-03-22 09:17:58.927909 pyqqq-0.7.5/pyqqq/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 06:48:22.487560 pyqqq-0.7.5/pyqqq/brokerage/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-04 04:13:28.619719 pyqqq-0.7.5/pyqqq/brokerage/ebest/__init__.py
+-rw-r--r--   0        0        0    39223 2024-04-11 09:59:48.694231 pyqqq-0.7.5/pyqqq/brokerage/ebest/domestic_stock.py
+-rw-r--r--   0        0        0     2643 2024-03-22 09:17:58.928327 pyqqq-0.7.5/pyqqq/brokerage/ebest/oauth.py
+-rw-r--r--   0        0        0    24122 2024-04-11 10:24:05.106743 pyqqq-0.7.5/pyqqq/brokerage/ebest/simple.py
+-rw-r--r--   0        0        0     7679 2024-03-28 00:52:30.410339 pyqqq-0.7.5/pyqqq/brokerage/ebest/tr_client.py
+-rw-r--r--   0        0        0        0 2024-02-16 05:40:46.772778 pyqqq-0.7.5/pyqqq/brokerage/kis/__init__.py
+-rw-r--r--   0        0        0   187461 2024-04-04 05:49:48.946800 pyqqq-0.7.5/pyqqq/brokerage/kis/domestic_stock.py
+-rw-r--r--   0        0        0     5319 2024-03-22 09:17:58.928711 pyqqq-0.7.5/pyqqq/brokerage/kis/oauth.py
+-rw-r--r--   0        0        0    69895 2024-03-05 09:07:38.156266 pyqqq-0.7.5/pyqqq/brokerage/kis/overseas_stock.py
+-rw-r--r--   0        0        0    24359 2024-04-11 03:46:13.044337 pyqqq-0.7.5/pyqqq/brokerage/kis/simple.py
+-rw-r--r--   0        0        0     2364 2024-03-07 05:33:47.158607 pyqqq-0.7.5/pyqqq/brokerage/kis/tr_client.py
+-rw-r--r--   0        0        0      448 2024-04-12 04:14:38.633056 pyqqq-0.7.5/pyqqq/config.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.877621 pyqqq-0.7.5/pyqqq/data/__init__.py
+-rw-r--r--   0        0        0     6546 2024-04-09 03:46:33.909510 pyqqq-0.7.5/pyqqq/data/domestic.py
+-rw-r--r--   0        0        0     5939 2024-04-11 09:40:12.485317 pyqqq-0.7.5/pyqqq/data/minutes.py
+-rw-r--r--   0        0        0     1535 2024-04-11 09:38:01.803182 pyqqq-0.7.5/pyqqq/data/realtime.py
+-rw-r--r--   0        0        0     4156 2024-04-01 05:25:31.374959 pyqqq-0.7.5/pyqqq/data/ticks.py
+-rw-r--r--   0        0        0     1254 2024-03-11 08:57:50.712529 pyqqq-0.7.5/pyqqq/datatypes.py
+-rw-r--r--   0        0        0        0 2024-04-12 06:24:35.199779 pyqqq-0.7.5/pyqqq/executors/__init__.py
+-rw-r--r--   0        0        0    38287 2024-04-12 09:46:36.906208 pyqqq-0.7.5/pyqqq/executors/hook.py
+-rw-r--r--   0        0        0        0 2024-03-07 01:02:36.878098 pyqqq-0.7.5/pyqqq/utils/__init__.py
+-rw-r--r--   0        0        0      951 2024-04-11 09:42:23.010351 pyqqq-0.7.5/pyqqq/utils/array.py
+-rw-r--r--   0        0        0     1174 2024-04-02 08:54:34.954991 pyqqq-0.7.5/pyqqq/utils/display.py
+-rw-r--r--   0        0        0     3963 2024-03-12 02:15:43.150036 pyqqq-0.7.5/pyqqq/utils/kvstore.py
+-rw-r--r--   0        0        0     1511 2024-02-26 08:31:21.240645 pyqqq-0.7.5/pyqqq/utils/limiter.py
+-rw-r--r--   0        0        0     1070 2024-03-22 09:17:58.929708 pyqqq-0.7.5/pyqqq/utils/logger.py
+-rw-r--r--   0        0        0     5150 2024-04-01 04:16:07.867878 pyqqq-0.7.5/pyqqq/utils/market_schedule.py
+-rw-r--r--   0        0        0     1425 2024-02-26 08:29:26.774617 pyqqq-0.7.5/pyqqq/utils/retry.py
+-rw-r--r--   0        0        0     1504 1970-01-01 00:00:00.000000 pyqqq-0.7.5/PKG-INFO
```

### Comparing `pyqqq-0.7.4/README.md` & `pyqqq-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyproject.toml` & `pyqqq-0.7.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq"
-version = "0.7.4"
+version = "0.7.5"
 description = "Package for quantitative strategy development on the PyQQQ platform"
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "pyqqq"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq-0.7.4/pyqqq/__init__.py` & `pyqqq-0.7.5/pyqqq/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/ebest/domestic_stock.py` & `pyqqq-0.7.5/pyqqq/brokerage/ebest/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/ebest/oauth.py` & `pyqqq-0.7.5/pyqqq/brokerage/ebest/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/ebest/simple.py` & `pyqqq-0.7.5/pyqqq/brokerage/ebest/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/ebest/tr_client.py` & `pyqqq-0.7.5/pyqqq/brokerage/ebest/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/kis/domestic_stock.py` & `pyqqq-0.7.5/pyqqq/brokerage/kis/domestic_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/kis/oauth.py` & `pyqqq-0.7.5/pyqqq/brokerage/kis/oauth.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/kis/overseas_stock.py` & `pyqqq-0.7.5/pyqqq/brokerage/kis/overseas_stock.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/kis/simple.py` & `pyqqq-0.7.5/pyqqq/brokerage/kis/simple.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/brokerage/kis/tr_client.py` & `pyqqq-0.7.5/pyqqq/brokerage/kis/tr_client.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/data/domestic.py` & `pyqqq-0.7.5/pyqqq/data/domestic.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/data/minutes.py` & `pyqqq-0.7.5/pyqqq/data/minutes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/data/realtime.py` & `pyqqq-0.7.5/pyqqq/data/realtime.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/data/ticks.py` & `pyqqq-0.7.5/pyqqq/data/ticks.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/datatypes.py` & `pyqqq-0.7.5/pyqqq/datatypes.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/executors/hook.py` & `pyqqq-0.7.5/pyqqq/executors/hook.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 
 class HookExecutor:
     def __init__(
         self, strategy_module, interval: dtm.timedelta = dtm.timedelta(seconds=60)
     ):
         self.strategy_module = strategy_module
         self.brokerage = None
-        self.auth = None
         self.stock_broker = None
         self.app_key = None
         self.app_secret = None
         self.account_number = None
         self.account_product_code = None
         self.paper_trading = False
         self.broker_settings = {}
         self.current_ts = 0
+        self.stock_broker_factory = None
+        self.market_schedule_factory = None
+        self.time_factory = None
+        self.keep_alive = lambda: True
 
         self.interval = interval  # 전략 호출 주기
         self.stop_loss_config = {}  # 손절 조건 설정
         self.take_profit_config = {}  # 익절 조건 설정
         self.market_open_time_margin = dtm.timedelta(
             minutes=5
         )  # 개장 시간과 거래 시간 사이의 여유 시간
@@ -57,25 +60,49 @@
             self._update_config(user_config)
 
         if self.brokerage == "kis":
             assert self.app_key is not None, "KIS_APP_KEY is required"
             assert self.app_secret is not None, "KIS_APP_SECRET is required"
             assert self.account_number is not None, "KIS_CANO is required"
             assert self.account_product_code is not None, "KIS_ACNT_PRDT_CD is required"
-
-            self.auth = KISAuth(self.app_key, self.app_secret, self.paper_trading)
-            self.stock_broker = KISSimpleDomesticStock(
-                self.auth, self.account_number, self.account_product_code
-            )
         else:
             assert self.app_key is not None, "EBEST_APP_KEY is required"
             assert self.app_secret is not None, "EBEST_APP_SECRET is required"
 
-            self.auth = EBestAuth(self.app_key, self.app_secret, self.paper_trading)
-            self.stock_broker = EBestSimpleDomesticStock(self.auth)
+        self.stock_broker = self.create_stock_broker()
+
+    def now(self) -> dtm.datetime:
+        if self.time_factory is None:
+            return dtm.datetime.now()
+        else:
+            return self.time_factory()
+
+    def today(self) -> dtm.date:
+        return self.now().date()
+
+    def create_stock_broker(self):
+        if self.stock_broker_factory is None:
+            if self.brokerage == "kis":
+                auth = KISAuth(self.app_key, self.app_secret, self.paper_trading)
+                return KISSimpleDomesticStock(
+                    auth, self.account_number, self.account_product_code
+                )
+            elif self.brokerage == "ebest":
+                auth = EBestAuth(self.app_key, self.app_secret, self.paper_trading)
+                return EBestSimpleDomesticStock(auth)
+        else:
+            args = {
+                "brokerage": self.brokerage,
+                "app_key": self.app_key,
+                "app_secret": self.app_secret,
+                "account_number": self.account_number,
+                "account_product_code": self.account_product_code,
+                "paper_trading": self.paper_trading,
+            }
+            return self.stock_broker_factory(**args)
 
     def _has_hook(self, func_name: str) -> bool:
         """사용자가 구현한 함수가 있는지 확인"""
         return hasattr(self.strategy_module, func_name) and callable(
             getattr(self.strategy_module, func_name)
         )
 
@@ -368,44 +395,50 @@
                 price=price,
                 quantity=quantity,
                 side=side,
                 order_type=order_type,
             )
 
     def is_trading_day(self) -> bool:
-        schedule = get_market_schedule(dtm.date.today())
+        schedule = self.get_market_schedule()
 
         return not schedule.full_day_closed
 
     @property
     def market_open_time(self) -> dtm.datetime:
         """오늘 개장 시간"""
-        schedule = get_market_schedule(dtm.date.today())
+        schedule = self.get_market_schedule()
 
         if schedule.open_time:
             open_time = schedule.open_time
         else:
             open_time = dtm.time(9, 0)
 
-        return dtm.datetime.combine(dtm.datetime.today().date(), open_time)
+        return dtm.datetime.combine(self.today(), open_time)
 
     @property
     def market_close_time(self) -> dtm.datetime:
         """오늘 폐장 시간 (동시호가 시작)"""
 
-        schedule = get_market_schedule(dtm.date.today())
+        schedule = self.get_market_schedule()
 
         if schedule.close_time:
             close_time = schedule.close_time
         else:
             close_time = dtm.time(15, 30)
 
-        return dtm.datetime.combine(
-            dtm.datetime.today().date(), close_time
-        ) - dtm.timedelta(minutes=10)
+        return dtm.datetime.combine(self.today(), close_time) - dtm.timedelta(
+            minutes=10
+        )
+
+    def get_market_schedule(self):
+        if self.market_schedule_factory is None:
+            return get_market_schedule(self.today())
+        else:
+            return self.market_schedule_factory()
 
     @property
     def user_defined_market_open_time(self) -> dtm.datetime:
         """사용자가 설정한 여유 시간 간격을 반영한 개장 시간"""
         return self.market_open_time + self.market_open_time_margin
 
     @property
@@ -422,17 +455,15 @@
         """사용자가 설정한 여유 시간 간격을 반영한 폐장 시간"""
         return self.market_close_time - self.market_close_time_margin
 
     @property
     def before_market_open_hook_call_time(self) -> dtm.datetime:
         """개장 전에 호출되는 hook이 호출되는 시간"""
         if type(self.before_market_open_schedule) == dtm.time:
-            return dtm.datetime.combine(
-                dtm.datetime.today().date(), self.before_market_open_schedule
-            )
+            return dtm.datetime.combine(self.today(), self.before_market_open_schedule)
         else:
             return self.user_defined_market_open_time - self.before_market_open_schedule
 
     @property
     def before_market_open_hook_call_time_threshold(self) -> dtm.datetime:
         """개장 전에 호출되는 hook이 호출되는 시간에 대한 threshold
 
@@ -440,37 +471,35 @@
         """
         return self.before_market_open_hook_call_time + dtm.timedelta(minutes=5)
 
     @property
     def after_market_close_hook_call_time(self) -> dtm.datetime:
         """폐장 후에 호출되는 hook이 호출되는 시간"""
         if type(self.after_market_close_schedule) == dtm.time:
-            return dtm.datetime.combine(
-                dtm.datetime.today().date(), self.after_market_close_schedule
-            )
+            return dtm.datetime.combine(self.today(), self.after_market_close_schedule)
         else:
             return (
                 self.user_defined_market_close_time + self.after_market_close_schedule
             )
 
     @property
     def after_market_close_hook_call_time_threshold(self) -> dtm.datetime:
         """폐장 후에 호출되는 hook이 호출되는 시간에 대한 threshold
 
         기본값은 폐장 후에 5분 이내에 앱이 실행 중이어야 폐장 후 콜백을 호출함
         """
         return self.after_market_close_hook_call_time + dtm.timedelta(minutes=5)
 
     def is_trading_time(self) -> bool:
-        schedule = get_market_schedule(dtm.date.today())
+        schedule = self.get_market_schedule()
 
         if schedule.full_day_closed:
             return False
 
-        now = dtm.datetime.now()
+        now = self.now()
 
         if now < self.market_open_time:
             return False
 
         if now > self.market_close_time:
             return False
 
@@ -489,15 +518,15 @@
 
         market_opened = False
         market_closed = False
         before_market_open_hook_called = False
         after_market_close_hook_called = False
 
         while True:
-            now = dtm.datetime.now()
+            now = self.now()
             self.current_ts = int(now.timestamp() * 1000)
 
             if now.date() != today:
                 today = now.date()
                 market_opened = False
                 market_closed = False
                 before_market_open_hook_called = False
@@ -594,14 +623,17 @@
                 break
             except asyncio.CancelledError:
                 logger.info("Got cancelled error. stop loop")
                 break
             except Exception:
                 traceback.print_exc()
 
+            if not self.keep_alive():
+                break
+
             await asyncio.sleep(1)
 
     async def trade(self) -> None:
         """
         일정 주기마다 전반적인 트레이딩 시스템을 실행
 
         Steps:
```

### Comparing `pyqqq-0.7.4/pyqqq/utils/array.py` & `pyqqq-0.7.5/pyqqq/utils/array.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/utils/display.py` & `pyqqq-0.7.5/pyqqq/utils/display.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/utils/kvstore.py` & `pyqqq-0.7.5/pyqqq/utils/kvstore.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/utils/limiter.py` & `pyqqq-0.7.5/pyqqq/utils/limiter.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/utils/logger.py` & `pyqqq-0.7.5/pyqqq/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/utils/market_schedule.py` & `pyqqq-0.7.5/pyqqq/utils/market_schedule.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/pyqqq/utils/retry.py` & `pyqqq-0.7.5/pyqqq/utils/retry.py`

 * *Files identical despite different names*

### Comparing `pyqqq-0.7.4/PKG-INFO` & `pyqqq-0.7.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq
-Version: 0.7.4
+Version: 0.7.5
 Summary: Package for quantitative strategy development on the PyQQQ platform
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

