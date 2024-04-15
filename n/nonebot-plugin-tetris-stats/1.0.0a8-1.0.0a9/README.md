# Comparing `tmp/nonebot_plugin_tetris_stats-1.0.0a8.tar.gz` & `tmp/nonebot_plugin_tetris_stats-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-1.0.0a8.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-1.0.0a9.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-1.0.0a8.tar` & `nonebot_plugin_tetris_stats-1.0.0a9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    34523 2023-11-22 08:12:58.719261 nonebot_plugin_tetris_stats-1.0.0a8/LICENSE
--rw-r--r--   0        0        0     2242 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/README.md
--rw-r--r--   0        0        0      683 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0      331 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/config.py
--rw-r--r--   0        0        0     6222 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
--rw-r--r--   0        0        0     3262 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
--rw-r--r--   0        0        0     5475 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
--rw-r--r--   0        0        0        0 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/__init__.py
--rw-r--r--   0        0        0     1303 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/db/__init__.py
--rw-r--r--   0        0        0     2287 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/db/models.py
--rw-r--r--   0        0        0     2914 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      108 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/constant.py
--rw-r--r--   0        0        0     6963 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0     1002 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py
--rw-r--r--   0        0        0      400 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
--rw-r--r--   0        0        0     1114 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
--rw-r--r--   0        0        0     9808 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
--rw-r--r--   0        0        0      334 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/base.py
--rw-r--r--   0        0        0     1682 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py
--rw-r--r--   0        0        0      447 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py
--rw-r--r--   0        0        0      266 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user.py
--rw-r--r--   0        0        0     4115 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py
--rw-r--r--   0        0        0     2750 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py
--rw-r--r--   0        0        0      231 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/typing.py
--rw-r--r--   0        0        0      555 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
--rw-r--r--   0        0        0     3651 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
--rw-r--r--   0        0        0      107 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
--rw-r--r--   0        0        0     4890 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py
--rw-r--r--   0        0        0      212 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/schemas/response.py
--rw-r--r--   0        0        0     4620 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
--rw-r--r--   0        0        0      104 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
--rw-r--r--   0        0        0     8039 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py
--rw-r--r--   0        0        0      379 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py
--rw-r--r--   0        0        0     3847 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py
--rw-r--r--   0        0        0      690 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py
--rw-r--r--   0        0        0     3009 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/browser.py
--rw-r--r--   0        0        0      773 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/exception.py
--rw-r--r--   0        0        0     8201 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/metrics.py
--rw-r--r--   0        0        0      440 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/platform.py
--rw-r--r--   0        0        0     3039 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/recorder.py
--rw-r--r--   0        0        0     4445 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/request.py
--rw-r--r--   0        0        0     1390 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/retry.py
--rw-r--r--   0        0        0      922 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/typing.py
--rw-r--r--   0        0        0       93 2023-11-22 08:12:58.723261 nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/version.py
--rw-r--r--   0        0        0     2855 2023-11-22 08:12:58.727261 nonebot_plugin_tetris_stats-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     2242 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/README.md
+-rw-r--r--   0        0        0      683 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0      331 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/config.py
+-rw-r--r--   0        0        0     6222 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
+-rw-r--r--   0        0        0     3262 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
+-rw-r--r--   0        0        0     5475 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
+-rw-r--r--   0        0        0        0 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/__init__.py
+-rw-r--r--   0        0        0     1303 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/db/__init__.py
+-rw-r--r--   0        0        0     2287 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/db/models.py
+-rw-r--r--   0        0        0     2914 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
+-rw-r--r--   0        0        0      108 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/constant.py
+-rw-r--r--   0        0        0     6971 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
+-rw-r--r--   0        0        0     1002 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py
+-rw-r--r--   0        0        0      400 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
+-rw-r--r--   0        0        0     1114 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
+-rw-r--r--   0        0        0     9808 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py
+-rw-r--r--   0        0        0      334 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/base.py
+-rw-r--r--   0        0        0     1682 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py
+-rw-r--r--   0        0        0      447 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/response.py
+-rw-r--r--   0        0        0      266 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user.py
+-rw-r--r--   0        0        0     4115 2023-11-22 10:34:55.363324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py
+-rw-r--r--   0        0        0     2750 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py
+-rw-r--r--   0        0        0      231 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/typing.py
+-rw-r--r--   0        0        0      555 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
+-rw-r--r--   0        0        0     3651 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
+-rw-r--r--   0        0        0      107 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
+-rw-r--r--   0        0        0     4890 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py
+-rw-r--r--   0        0        0      212 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/schemas/response.py
+-rw-r--r--   0        0        0     4620 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
+-rw-r--r--   0        0        0      104 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
+-rw-r--r--   0        0        0     8039 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py
+-rw-r--r--   0        0        0      379 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/response.py
+-rw-r--r--   0        0        0     3847 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py
+-rw-r--r--   0        0        0      690 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py
+-rw-r--r--   0        0        0     3009 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/browser.py
+-rw-r--r--   0        0        0      773 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/exception.py
+-rw-r--r--   0        0        0     8201 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/metrics.py
+-rw-r--r--   0        0        0      440 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/platform.py
+-rw-r--r--   0        0        0     3039 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/recorder.py
+-rw-r--r--   0        0        0     4445 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/request.py
+-rw-r--r--   0        0        0     1390 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/retry.py
+-rw-r--r--   0        0        0      922 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/typing.py
+-rw-r--r--   0        0        0       93 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/version.py
+-rw-r--r--   0        0        0     2855 2023-11-22 10:34:55.367324 nonebot_plugin_tetris_stats-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0     3525 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.0.0a9/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/LICENSE` & `nonebot_plugin_tetris_stats-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/README.md` & `nonebot_plugin_tetris_stats-1.0.0a9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/__init__.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/db/__init__.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/db/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/db/models.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/db/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                         - func.julianday(latest_data.create_time - timedelta(hours=24))
                     )
                 )
                 .limit(1)
             )
         ).one()
     message = ''
-    if (datetime.now(UTC) - latest_data.create_time) > timedelta(hours=7):
+    if (datetime.now(UTC) - latest_data.create_time.replace(tzinfo=UTC)) > timedelta(hours=7):
         message += 'Warning: 数据超过7小时未更新, 请联系Bot主人查看后台\n'
     message += f'{rank.upper()} 段 分数线 {latest_data.tr_line:.2f} TR, {latest_data.player_count} 名玩家\n'
     if compare_data.id != latest_data.id:
         message += f'对比 {(latest_data.create_time-compare_data.create_time).total_seconds()/3600:.2f} 小时前趋势: {f"↑{difference:.2f}" if (difference:=latest_data.tr_line-compare_data.tr_line) > 0 else f"↓{-difference:.2f}" if difference < 0 else "→"}'
     else:
         message += '暂无对比数据'
     avg = get_metrics(pps=latest_data.avg_pps, apm=latest_data.avg_apm, vs=latest_data.avg_vs)
@@ -179,13 +179,13 @@
         f'ADPM: {low_vs.adpm} ( {low_vs.vs}vs ) By: {latest_data.low_vs[0]["name"].upper()}\n'
         '\n'
         '最高数据:\n'
         f"L'PM: {max_pps.lpm} ( {max_pps.pps} pps ) By: {latest_data.high_pps[0]['name'].upper()}\n"
         f'APM: {latest_data.high_apm[1]} By: {latest_data.high_apm[0]["name"].upper()}\n'
         f'ADPM: {max_vs.adpm} ( {max_vs.vs}vs ) By: {latest_data.high_vs[0]["name"].upper()}\n'
         '\n'
-        f'数据更新时间: {latest_data.create_time.replace(tzinfo=ZoneInfo("UTC")).astimezone(ZoneInfo("Asia/Shanghai")).strftime("%Y-%m-%d %H:%M:%S")}'
+        f'数据更新时间: {latest_data.create_time.replace(tzinfo=UTC).astimezone(ZoneInfo("Asia/Shanghai")).strftime("%Y-%m-%d %H:%M:%S")}'
     )
     await matcher.finish(message)
 
 
 add_default_handlers(alc)
```

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/league_all.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/schemas/user_records.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/schemas.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/schemas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/processor.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/schemas/user_profile.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/browser.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/exception.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/metrics.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/recorder.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/recorder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/request.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/retry.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/nonebot_plugin_tetris_stats/utils/typing.py` & `nonebot_plugin_tetris_stats-1.0.0a9/nonebot_plugin_tetris_stats/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/pyproject.toml` & `nonebot_plugin_tetris_stats-1.0.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'nonebot-plugin-tetris-stats'
-version = '1.0.0.a8'
+version = '1.0.0.a9'
 description = '一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件'
 authors = ['scdhh <wallfjjd@gmail.com>']
 readme = 'README.md'
 homepage = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 repository = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 license = 'AGPL-3.0'
```

### Comparing `nonebot_plugin_tetris_stats-1.0.0a8/PKG-INFO` & `nonebot_plugin_tetris_stats-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: 一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: AGPL-3.0
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.0.0a8
+Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.0.0a9
 Summary: ä¸æ¬¾åºäº NoneBot2 çç¨äºæ¥è¯¢ Tetris
 ç¸å³æ¸¸ææ°æ®çæä»¶ Home-page: https://github.com/shoucandanghehe/
 nonebot-plugin-tetris-stats License: AGPL-3.0 Author: scdhh Author-email:
 wallfjjd@gmail.com Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
 Approved :: GNU Affero General Public License v3 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
```

