# Comparing `tmp/nonebot_plugin_nai3-0.1.0.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.1.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.0.tar` & `nonebot_plugin_nai3-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.0/LICENSE
--rw-r--r--   0        0        0    12618 2024-04-15 04:37:50.400079 nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-04-15 04:42:08.927585 nonebot_plugin_nai3-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4992 2024-04-15 04:37:38.339584 nonebot_plugin_nai3-0.1.0/README.md
--rw-r--r--   0        0        0     5592 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.1/LICENSE
+-rw-r--r--   0        0        0    12781 2024-04-15 04:53:21.331133 nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-04-15 04:53:51.289440 nonebot_plugin_nai3-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4992 2024-04-15 04:37:38.339584 nonebot_plugin_nai3-0.1.1/README.md
+-rw-r--r--   0        0        0     5592 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.0/LICENSE` & `nonebot_plugin_nai3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,22 +120,22 @@
 
     # 判断冷却时间并阻断
     if event.get_user_id() not in bot.config.superusers:
         logger.debug(event.get_user_id())
         logger.debug(bot.config.superusers)
         if now_time - cd[gid]["cool_time"] < nai3_config.nai3_cooltime_group:
             await nai3.finish(
-                "群聊绘画冷却中, 剩余时间: {}...".format(
+                "群聊绘画冷却中, 剩余时间: {} 秒...".format(
                     round(nai3_config.nai3_cooltime_group - now_time + cd[gid]["cool_time"], 3)
                 ),
                 at_sender=True,
             )
         if now_time - cd[gid]["user"][uid]["cool_time"] < nai3_config.nai3_cooltime_user:
             await nai3.finish(
-                "个人绘画冷却中, 剩余时间: {}...".format(
+                "个人绘画冷却中, 剩余时间: {} 秒...".format(
                     round(nai3_config.nai3_cooltime_user - now_time + cd[gid]["cool_time"], 3)
                 ),
                 at_sender=True,
             )
         if cd[gid]["user"][uid]["limit"] <= 0:
             await nai3.finish("今天已经没次数了哦~", at_send=True)
 
@@ -209,22 +209,24 @@
                         "FEMALE_BREAST_EXPOSED",
                         "FEMALE_GENITALIA_EXPOSED",
                         "ANUS_EXPOSED",
                         "MALE_GENITALIA_EXPOSED",
                     ]:
                         safe = "R18"
                 if safe == "R18":
-                    await nai3.send("检测到 R18 内容, 不可以涩涩!", at_sender=True)
+                    await nai3.send(
+                        "图片已生成, 但检测到 R18 内容! 不可以涩涩!! 人家要火速告诉主人去!!", at_sender=True
+                    )
                     if nai3_config.smms_token:
                         file = await smms.upload(Path("./data/nai3/temp.png"))
                         for superuser in bot.config.superusers:
                             await bot.call_api(
                                 "send_msg",
                                 **{
-                                    "message": file.url,
+                                    "message": f"群: {gid}, 用户: {uid}, 画了一张涩图!\n{file.url}",
                                     "user_id": superuser,
                                 },
                             )
                             asyncio.sleep(3)
                     return
             await nai3.send(f"种子: {seed}\n" + MessageSegment.image("./data/nai3/temp.png"), at_sender=True)
             return
```

### Comparing `nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.0/pyproject.toml` & `nonebot_plugin_nai3-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.0"
+version = "0.1.1"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.0/README.md` & `nonebot_plugin_nai3-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.0/PKG-INFO` & `nonebot_plugin_nai3-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.0
+Version: 0.1.1
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.0 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.1 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
```

