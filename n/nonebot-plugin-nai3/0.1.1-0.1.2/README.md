# Comparing `tmp/nonebot_plugin_nai3-0.1.1.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.1.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.2.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.1.1.tar` & `nonebot_plugin_nai3-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.1/LICENSE
--rw-r--r--   0        0        0    12781 2024-04-15 04:53:21.331133 nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0     1071 2024-04-15 04:53:51.289440 nonebot_plugin_nai3-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4992 2024-04-15 04:37:38.339584 nonebot_plugin_nai3-0.1.1/README.md
--rw-r--r--   0        0        0     5592 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.2/LICENSE
+-rw-r--r--   0        0        0    12762 2024-04-15 06:06:34.338313 nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-04-15 06:07:30.637070 nonebot_plugin_nai3-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5132 2024-04-15 05:01:56.830191 nonebot_plugin_nai3-0.1.2/README.md
+-rw-r--r--   0        0        0     5731 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.1.1/LICENSE` & `nonebot_plugin_nai3-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,20 @@
     extra={
         "author": "zhulinyv",
         "version": __version__,
     },
 )
 
 
+if not os.path.exists("./data/nai3"):
+    os.makedirs("./data/nai3")
+    black_data = {"user": [], "group": []}
+    with open("./data/nai3/black_data.json", "w", encoding="utf-8") as f:
+        json.dump(black_data, f, indent=4, ensure_ascii=False)
+
 nai3_parser = ArgumentParser()
 nai3_parser.add_argument("prompt", nargs="*", help="提示词(支持你喜欢的画风串)", type=str)
 nai3_parser.add_argument("-n", "--negative", nargs="*", help="负面提示词", type=str, dest="negative")
 nai3_parser.add_argument("-r", "--resolution", help="画布形状/分辨率", type=str, dest="resolution")
 nai3_parser.add_argument("-s", "--scale", help="提示词相关性", type=float, dest="scale")
 nai3_parser.add_argument("-sm", help="sm", type=bool, dest="sm")
 nai3_parser.add_argument("-smdyn", help="smdyn", type=bool, dest="smdyn")
@@ -210,15 +216,15 @@
                         "FEMALE_GENITALIA_EXPOSED",
                         "ANUS_EXPOSED",
                         "MALE_GENITALIA_EXPOSED",
                     ]:
                         safe = "R18"
                 if safe == "R18":
                     await nai3.send(
-                        "图片已生成, 但检测到 R18 内容! 不可以涩涩!! 人家要火速告诉主人去!!", at_sender=True
+                        "图片已生成, 但检测到 R18 内容! 不可以涩涩!! 人家要火速告诉主人去!!!", at_sender=True
                     )
                     if nai3_config.smms_token:
                         file = await smms.upload(Path("./data/nai3/temp.png"))
                         for superuser in bot.config.superusers:
                             await bot.call_api(
                                 "send_msg",
                                 **{
@@ -237,20 +243,14 @@
 @nai3_black.handle()
 async def _(event: MessageEvent, msg: Message = CommandArg()):
     text_msg = msg.extract_plain_text().strip()
     id = await get_at(event)
     if id == -1:
         id = text_msg.replace("添加", "").replace("删除", "").replace("群聊", "").replace("用户", "")
 
-    if not os.path.exists("./data/nai3"):
-        os.makedirs("./data/nai3")
-        black_data = {"user": [], "group": []}
-        with open("./data/nai3/black_data.json", "w", encoding="utf-8") as f:
-            json.dump(black_data, f, indent=4, ensure_ascii=False)
-
     with open("./data/nai3/black_data.json", "r") as f:
         black_data = json.load(f)
     if "添加" in text_msg:
         if "群聊" in text_msg:
             black_data["group"].append(str(id))
         elif "用户" in text_msg:
             black_data["user"].append(str(id))
```

### Comparing `nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.1/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.2/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.1.1/pyproject.toml` & `nonebot_plugin_nai3-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.1.1"
+version = "0.1.2"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.1.1/README.md` & `nonebot_plugin_nai3-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,16 @@
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
-| nai3_proxy | 否 | str | None | 代理 |
+| nai3_proxy | 否 | str | None | post 请求生成图片使用的代理 |
+| nai3_r18 | 否 | bool | False | 是否允许 R18 图片(False 将会把图片链接发给超级用户) |
 | SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
 | SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
```

#### html2text {}

```diff
@@ -19,17 +19,19 @@
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
-ä»£ç | | SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API
-å°å | | SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç
-(bushi) | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
+post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
+æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
+SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API å°å | |
+SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) |
+â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
 (localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
 [e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
 NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) â ï¸
 SMMS token çè·å: - ç»å½SM.MS" - ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" -
 è¾å¥è´¦å·é®ç®±åå¯ç " - ç¹å»"User" > "Dashboard"" - ç¹å»"API Token",
 å°±å¯ä»¥çå°Token, å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai
```

### Comparing `nonebot_plugin_nai3-0.1.1/PKG-INFO` & `nonebot_plugin_nai3-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.1.1
+Version: 0.1.2
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -88,15 +88,16 @@
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
-| nai3_proxy | 否 | str | None | 代理 |
+| nai3_proxy | 否 | str | None | post 请求生成图片使用的代理 |
+| nai3_r18 | 否 | bool | False | 是否允许 R18 图片(False 将会把图片链接发给超级用户) |
 | SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
 | SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.1 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.2 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
@@ -29,17 +29,19 @@
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
-ä»£ç | | SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API
-å°å | | SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç
-(bushi) | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
+post è¯·æ±çæå¾çä½¿ç¨çä»£ç | | nai3_r18 | å¦ | bool | False |
+æ¯å¦åè®¸ R18 å¾ç(False å°ä¼æå¾çé¾æ¥åç»è¶çº§ç¨æ·) | |
+SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API å°å | |
+SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç(bushi) |
+â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
 (localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
 [e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
 NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) â ï¸
 SMMS token çè·å: - ç»å½SM.MS" - ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" -
 è¾å¥è´¦å·é®ç®±åå¯ç " - ç¹å»"User" > "Dashboard"" - ç¹å»"API Token",
 å°±å¯ä»¥çå°Token, å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai
```

