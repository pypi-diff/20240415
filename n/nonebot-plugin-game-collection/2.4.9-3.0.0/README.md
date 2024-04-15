# Comparing `tmp/nonebot_plugin_game_collection-2.4.9.tar.gz` & `tmp/nonebot_plugin_game_collection-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_game_collection-2.4.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_game_collection-3.0.0.tar", max compression
```

## Comparing `nonebot_plugin_game_collection-2.4.9.tar` & `nonebot_plugin_game_collection-3.0.0.tar`

### file list

```diff
@@ -1,37 +1,5 @@
--rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-2.4.9/LICENSE
--rw-r--r--   0        0        0     5214 2023-11-01 04:17:24.022281 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/__init__.py
--rw-r--r--   0        0        0    23873 2023-11-01 04:28:31.405107 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Account.py
--rw-r--r--   0        0        0     2298 2023-10-29 02:46:51.855660 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/adapters/qq.py
--rw-r--r--   0        0        0     2386 2023-10-29 02:46:52.186444 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/adapters/v11.py
--rw-r--r--   0        0        0     2267 2023-10-29 02:45:27.499485 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Alchemy.py
--rw-r--r--   0        0        0     3759 2023-10-29 02:45:27.937361 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/config.py
--rw-r--r--   0        0        0    13292 2023-10-29 19:05:56.229230 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/data.py
--rw-r--r--   0        0        0      873 2023-10-29 02:45:28.703018 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Exceptions.py
--rw-r--r--   0        0        0     9955 2023-10-29 02:21:44.065612 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Fortress/core.py
--rw-r--r--   0        0        0    78278 2023-10-30 15:09:10.304026 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Game.py
--rw-r--r--   0        0        0    15602 2023-10-28 21:32:04.940762 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/HorseRace/events_main.py
--rw-r--r--   0        0        0     6374 2023-10-28 21:32:04.941262 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/HorseRace/horse.py
--rw-r--r--   0        0        0     5070 2023-10-28 21:32:04.941763 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/HorseRace/race_group.py
--rw-r--r--   0        0        0     9182 2023-10-28 21:32:04.941763 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/HorseRace/start.py
--rw-r--r--   0        0        0    12555 2023-10-29 18:53:06.324924 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Manager.py
--rw-r--r--   0        0        0    34378 2023-11-01 04:20:42.472733 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Market.py
--rw-r--r--   0        0        0    11013 2023-10-29 02:45:30.141754 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Processor.py
--rw-r--r--   0        0        0    20807 2023-10-29 02:45:30.496058 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/Prop.py
--rw-r--r--   0        0        0     5817 2023-10-29 02:46:03.573476 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/Stand.json
--rw-r--r--   0        0        0     5728 2023-10-29 02:46:03.757134 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/“日常，真的很日常”.json
--rw-r--r--   0        0        0     2174 2023-10-29 02:46:03.895253 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/克苏鲁.json
--rw-r--r--   0        0        0     1231 2023-10-29 02:46:04.008850 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/基础事件.json
--rw-r--r--   0        0        0     2742 2023-10-29 02:46:04.146968 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/复刻经典事件集合v1.json
--rw-r--r--   0        0        0     1606 2023-10-29 02:46:04.260567 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/崩坏集合v1.json
--rw-r--r--   0        0        0    25830 2023-10-29 02:46:04.432714 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/群友日常.json
--rw-r--r--   0        0        0     5180 2023-10-29 02:46:04.554819 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/芜湖事件合集.json
--rw-r--r--   0        0        0     1072 2023-10-29 02:46:04.691436 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/赫尔事件集v1.json
--rw-r--r--   0        0        0     2294 2023-10-29 02:46:04.793024 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/horserace/赫尔的赛马场事件簿.json
--rw-r--r--   0        0        0    12889 2023-10-29 02:46:24.801733 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/menu_data.json
--rw-r--r--   0        0        0     5254 2023-10-29 02:46:24.904180 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/props_library.json
--rw-r--r--   0        0        0     2286 2023-10-29 02:46:35.907210 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/resource/subprocess/ohlc.py
--rw-r--r--   0        0        0    22822 2023-10-28 21:45:43.228222 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/utils/chart.py
--rw-r--r--   0        0        0      711 2023-10-28 21:32:04.951026 nonebot_plugin_game_collection-2.4.9/nonebot_plugin_game_collection/utils/utils.py
--rw-r--r--   0        0        0      710 2023-11-01 04:30:09.335463 nonebot_plugin_game_collection-2.4.9/pyproject.toml
--rw-r--r--   0        0        0    26924 2023-10-28 21:32:04.943765 nonebot_plugin_game_collection-2.4.9/README.md
--rw-r--r--   0        0        0    26727 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-2.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-10-28 21:32:04.942263 nonebot_plugin_game_collection-3.0.0/LICENSE
+-rw-r--r--   0        0        0      707 2024-04-15 13:22:22.288690 nonebot_plugin_game_collection-3.0.0/nonebot_plugin_game_collection/__init__.py
+-rw-r--r--   0        0        0      362 2024-04-15 13:20:50.004753 nonebot_plugin_game_collection-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2984 2024-04-15 12:09:00.697493 nonebot_plugin_game_collection-3.0.0/README.md
+-rw-r--r--   0        0        0     3339 1970-01-01 00:00:00.000000 nonebot_plugin_game_collection-3.0.0/PKG-INFO
```

### Comparing `nonebot_plugin_game_collection-2.4.9/LICENSE` & `nonebot_plugin_game_collection-3.0.0/LICENSE`

 * *Files identical despite different names*

