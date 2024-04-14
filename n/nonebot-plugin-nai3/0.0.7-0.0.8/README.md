# Comparing `tmp/nonebot_plugin_nai3-0.0.7.tar.gz` & `tmp/nonebot_plugin_nai3-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.0.8.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.7.tar` & `nonebot_plugin_nai3-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.7/LICENSE
--rw-r--r--   0        0        0     8265 2024-04-14 10:15:04.711349 nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      527 2024-04-14 10:08:34.777191 nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2242 2024-04-14 09:09:14.219821 nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      864 2024-04-14 10:14:54.594690 nonebot_plugin_nai3-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4271 2024-04-14 10:14:33.143274 nonebot_plugin_nai3-0.0.7/README.md
--rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.8/LICENSE
+-rw-r--r--   0        0        0     8609 2024-04-14 12:59:22.863533 nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      555 2024-04-14 12:42:27.741067 nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2426 2024-04-14 12:58:41.611610 nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0      864 2024-04-14 13:01:54.179224 nonebot_plugin_nai3-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4364 2024-04-14 13:01:30.277514 nonebot_plugin_nai3-0.0.8/README.md
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.8/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.7/LICENSE` & `nonebot_plugin_nai3-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from nonebot.params import CommandArg, ShellCommandArgs
 from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
 from nonebot.plugin.on import on_command, on_shell_command
 from nonebot.rule import ArgumentParser
 
 from .config import Config, nai3_config
-from .utils import format_str, get_at, headers, json_for_t2i, list_to_str
+from .utils import format_str, get_at, headers, json_for_t2i, list_to_str, proxies
 
 ADMIN = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
 
 try:
     __version__ = version("nonebot_plugin_nai3")
 except Exception:
     __version__ = "0.0.0"
@@ -83,22 +83,25 @@
     except FileNotFoundError:
         pass
 
     now_time = time.time()
     try:
         cd[gid]["user"][uid]["limit"]
     except KeyError:
-        cd[gid] = {"cool_time": now_time - nai3_config.nai3_cooltime_group, "user": {uid: {"limit": nai3_config.nai3_limit, "cool_time": now_time - nai3_config.nai3_cooltime_user}}}
+        cd[gid] = {"cool_time": now_time - nai3_config.nai3_cooltime_group, "user": {uid: {"limit": 999 if event.get_user_id() in bot.config.superusers else nai3_config.nai3_limit, "cool_time": now_time - nai3_config.nai3_cooltime_user}}}
 
-    if now_time - cd[gid]["cool_time"] < nai3_config.nai3_cooltime_group:
-        await nai3.finish("群聊绘画冷却中, 剩余时间: {}...".format(round(nai3_config.nai3_cooltime_group - now_time + cd[gid]["cool_time"], 3)), at_sender=True)
-    if now_time - cd[gid]["user"][uid]["cool_time"] < nai3_config.nai3_cooltime_user:
-        await nai3.finish("个人绘画冷却中, 剩余时间: {}...".format(round(nai3_config.nai3_cooltime_user - now_time + cd[gid]["cool_time"], 3)), at_sender=True)
-    if cd[gid]["user"][uid]["limit"] <= 0:
-        await nai3.finish("今天已经没次数了哦~", at_send=True)
+    if event.get_user_id() not in bot.config.superusers:
+        logger.debug(event.get_user_id())
+        logger.debug(bot.config.superusers)
+        if now_time - cd[gid]["cool_time"] < nai3_config.nai3_cooltime_group:
+            await nai3.finish("群聊绘画冷却中, 剩余时间: {}...".format(round(nai3_config.nai3_cooltime_group - now_time + cd[gid]["cool_time"], 3)), at_sender=True)
+        if now_time - cd[gid]["user"][uid]["cool_time"] < nai3_config.nai3_cooltime_user:
+            await nai3.finish("个人绘画冷却中, 剩余时间: {}...".format(round(nai3_config.nai3_cooltime_user - now_time + cd[gid]["cool_time"], 3)), at_sender=True)
+        if cd[gid]["user"][uid]["limit"] <= 0:
+            await nai3.finish("今天已经没次数了哦~", at_send=True)
 
     await nai3.send("脑积水已收到绘画指令, 正在生成图片(剩余次数: {})...".format(cd[gid]["user"][uid]["limit"]), at_sender=True)
 
     json_for_t2i["input"] = format_str(list_to_str(args.prompt))
     resolution = args.resolution if args.resolution else "mb"
     if resolution == "mb":
         width = 832
@@ -122,26 +125,26 @@
     json_for_t2i["parameters"]["seed"] = seed
     json_for_t2i["parameters"]["negative_prompt"] = format_str(list_to_str(args.negative)) if args.negative else nai3_config.nai3_negative
 
     logger.debug(">>>>>")
     logger.debug(json_for_t2i)
 
     try:
-        async with AsyncClient() as client:
-            response = await client.post("https://image.novelai.net/ai/generate-image", json=json_for_t2i, headers=headers, timeout=300)
+        async with AsyncClient(proxies=proxies if nai3_config.nai3_proxy else None) as client:
+            response = await client.post("https://image.novelai.net/ai/generate-image", json=json_for_t2i, headers=headers, timeout=500)
             while response.status_code == 429:
                 await asyncio.sleep(random.randint(4, 8))
-                response = await client.post("https://image.novelai.net/ai/generate-image", json=json_for_t2i, headers=headers, timeout=300)
+                response = await client.post("https://image.novelai.net/ai/generate-image", json=json_for_t2i, headers=headers, timeout=500)
                 logger.debug(response.status_code)
             logger.debug("<<<<<")
             with zipfile.ZipFile(io.BytesIO(response.content), mode="r") as zip:
                 with zip.open("image_0.png") as image:
                     now_time = time.time()
                     cd[gid]["cool_time"] = now_time
-                    cd[gid]["user"][uid]["limit"] = cd[gid]["user"][uid]["limit"] - 1
+                    cd[gid]["user"][uid]["limit"] = 999 if event.get_user_id() in bot.config.superusers else cd[gid]["user"][uid]["limit"] - 1
                     cd[gid]["user"][uid]["cool_time"] = now_time
                     await nai3.send(f"种子: {seed}\n" + MessageSegment.image(image.read()), at_sender=True)
                     return
     except Exception as e:
         await nai3.finish(f"出现错误: {e}", at_sender=True)
```

### Comparing `nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,10 +4,11 @@
 
 class Config(BaseModel):
     nai3_token: str = "xxx"
     nai3_negative: str = "nsfw, lowres, {bad}, error, fewer, extra, missing, worst quality, jpeg artifacts, bad quality, watermark, unfinished, displeasing, chromatic aberration, signature, extra digits, artistic error, username, scan, [abstract]"
     nai3_limit: int = 10
     nai3_cooltime_group: int = 30
     nai3_cooltime_user: int = 300
+    nai3_proxy: str = None
 
 
 nai3_config = get_plugin_config(Config)
```

### Comparing `nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,22 @@
         "negative_prompt": str,
         "reference_image_multiple": [],
         "reference_information_extracted_multiple": [],
         "reference_strength_multiple": [],
     },
 }
 
+try:
+    proxies = {
+        "http://": "http://" + nai3_config.nai3_proxy,
+        "https://": "http://" + nai3_config.nai3_proxy,
+    }
+except Exception:
+    proxies = None
+
 
 def list_to_str(str_list: list):
     empty_str = ""
     for i in str_list:
         if i[-1] == ",":
             empty_str += f"{i}"
         else:
```

### Comparing `nonebot_plugin_nai3-0.0.7/pyproject.toml` & `nonebot_plugin_nai3-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.7"
+version = "0.0.8"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.0.7/README.md` & `nonebot_plugin_nai3-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
+| nai3_proxy | 否 | str | None | 代理 |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
 - 3.输入 `console.log(JSON.parse(localStorage.session).auth_token)` 回车, 返回的字符串即为 token
 - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079)
@@ -95,15 +96,15 @@
 示例: nai3 1girl, loli, cute -r mb -s 5.0
 返回: 
 ```
 
 ![img](./img/1.png)
 
 ```
-指令: nai3黑名单/黑名单
+指令: nai3黑名单/黑名单(需要超级用户, 群主或群管理员权限)
 参数:
     添加    添加黑名单
     删除    删除黑名单
     用户    指定添加类型
     群聊    指定添加类型
     群号/QQ号/@sb.
 示例: nai3黑名单添加用户 @脑积水
```

#### html2text {}

```diff
@@ -18,29 +18,30 @@
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
-| ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | â ï¸ token çè·å: - 1.ç»å½
-https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
-3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
-è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
-github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
-446d-9401-e559628ad079) ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
-æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
-è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
-["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
-5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
-é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
-loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤:
-nai3é»åå/é»åå åæ°: æ·»å  æ·»å é»åå å é¤ å é¤é»åå
-ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾:
-nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð
-å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
-~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
-[ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤
-é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
-github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+| ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
+ä»£ç | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
+æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
+(localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
+[e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
+NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) ## ð
+ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt æç¤ºè¯
+(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative è´é¢æç¤ºè¯,
+é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç, ["mb", "pc", "sq"]
+ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm,
+é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨, é»è®¤: k_euler
+--schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl, loli, cute -r mb
+-s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤: nai3é»åå/é»åå
+(éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å 
+æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è
+æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
+@èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð å¾å + [x] æçå¾ + [ ]
+å¾çå¾ + [x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
+ä¸éåè½ + [x] é»åååè½ + [ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
+[ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
+NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

### Comparing `nonebot_plugin_nai3-0.0.7/PKG-INFO` & `nonebot_plugin_nai3-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.7
+Version: 0.0.8
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -86,14 +86,15 @@
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
+| nai3_proxy | 否 | str | None | 代理 |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
 - 3.输入 `console.log(JSON.parse(localStorage.session).auth_token)` 回车, 返回的字符串即为 token
 - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079)
@@ -114,15 +115,15 @@
 示例: nai3 1girl, loli, cute -r mb -s 5.0
 返回: 
 ```
 
 ![img](./img/1.png)
 
 ```
-指令: nai3黑名单/黑名单
+指令: nai3黑名单/黑名单(需要超级用户, 群主或群管理员权限)
 参数:
     添加    添加黑名单
     删除    删除黑名单
     用户    指定添加类型
     群聊    指定添加类型
     群号/QQ号/@sb.
 示例: nai3黑名单添加用户 @脑积水
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.7 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.8 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: ujson
@@ -27,29 +27,30 @@
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
-| ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | â ï¸ token çè·å: - 1.ç»å½
-https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
-3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
-è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
-github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
-446d-9401-e559628ad079) ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
-æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
-è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
-["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
-5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
-é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
-loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤:
-nai3é»åå/é»åå åæ°: æ·»å  æ·»å é»åå å é¤ å é¤é»åå
-ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾:
-nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð
-å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
-~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
-[ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤
-é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
-github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+| ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
+ä»£ç | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
+æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
+(localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
+[e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
+NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) ## ð
+ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt æç¤ºè¯
+(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative è´é¢æç¤ºè¯,
+é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç, ["mb", "pc", "sq"]
+ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm,
+é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨, é»è®¤: k_euler
+--schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl, loli, cute -r mb
+-s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤: nai3é»åå/é»åå
+(éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å 
+æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è
+æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
+@èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð å¾å + [x] æçå¾ + [ ]
+å¾çå¾ + [x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
+ä¸éåè½ + [x] é»åååè½ + [ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
+[ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
+NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

