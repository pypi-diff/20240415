# Comparing `tmp/nonebot_plugin_nai3-0.0.9.tar.gz` & `tmp/nonebot_plugin_nai3-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.1.0.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.9.tar` & `nonebot_plugin_nai3-0.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.9/LICENSE
--rw-r--r--   0        0        0     8561 2024-04-14 23:09:41.177004 nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      555 2024-04-14 12:42:27.741067 nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2426 2024-04-14 12:58:41.611610 nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      864 2024-04-14 23:08:45.840659 nonebot_plugin_nai3-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     4364 2024-04-14 13:30:50.170244 nonebot_plugin_nai3-0.0.9/README.md
--rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.1.0/LICENSE
+-rw-r--r--   0        0        0    12618 2024-04-15 04:37:50.400079 nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      691 2024-04-15 03:42:07.432330 nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2440 2024-04-14 23:34:30.728833 nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0     1071 2024-04-15 04:42:08.927585 nonebot_plugin_nai3-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4992 2024-04-15 04:37:38.339584 nonebot_plugin_nai3-0.1.0/README.md
+-rw-r--r--   0        0        0     5592 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.1.0/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.9/LICENSE` & `nonebot_plugin_nai3-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 from nonebot.plugin import get_plugin_config
 from pydantic import BaseModel
 
 
 class Config(BaseModel):
     nai3_token: str = "xxx"
-    nai3_negative: str = "nsfw, lowres, {bad}, error, fewer, extra, missing, worst quality, jpeg artifacts, bad quality, watermark, unfinished, displeasing, chromatic aberration, signature, extra digits, artistic error, username, scan, [abstract]"
+    nai3_negative: str = (
+        "nsfw, lowres, {bad}, error, fewer, extra, missing, worst quality, jpeg artifacts, bad quality, watermark, unfinished, displeasing, chromatic aberration, signature, extra digits, artistic error, username, scan, [abstract]"  # noqa: E501
+    )
     nai3_limit: int = 10
     nai3_cooltime_group: int = 30
     nai3_cooltime_user: int = 300
     nai3_proxy: str = None
+    nai3_r18: bool = False
+    smms_api_url: str = "https://sm.ms/api/v2"
+    smms_token: str = None
 
 
 nai3_config = get_plugin_config(Config)
```

### Comparing `nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.1.0/nonebot_plugin_nai3/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "Referer": "https://novelai.net",
     "Sec-Ch-Ua": '"Chromium";v="122", "Not(A:Brand";v="24", "Microsoft Edge";v="122"',
     "Sec-Ch-Ua-mobile": "?0",
     "Sec-Ch-Ua-Platform": '"Windows"',
     "Sec-Fetch-Dest": "empty",
     "Sec-Fetch-Mode": "cors",
     "Sec-Fetch-Site": "same-site",
-    "User-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36",
+    "User-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/106.0.0.0 Safari/537.36",  # noqa: E501
 }
 
 
 json_for_t2i = {
     "input": str,
     "model": "nai-diffusion-3",
     "action": "generate",
```

### Comparing `nonebot_plugin_nai3-0.0.9/pyproject.toml` & `nonebot_plugin_nai3-0.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.9"
+version = "0.1.0"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.2.1"
 httpx = "^0.24.1"
 nonebot-adapter-onebot = "^2.2.3"
 ujson = "^5.9.0"
+nudenet = "^3.0.8"
+nonebot-plugin-smms = "^0.1.0"
+
+[tool.poetry.group.dev.dependencies]
+pre-commit = "^3.7.0"
 
 # https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
 [tool.black]
-line-length = 500
+line-length = 120
 
 # https://beta.ruff.rs/docs/settings/
 [tool.ruff]
-line-length = 500
+line-length = 120
 # https://beta.ruff.rs/docs/rules/
-select = ["E", "W", "F"]
-ignore = ["F401"]
+lint.select = ["E", "W", "F"]
+lint.ignore = ["E501"]
 # Exclude a variety of commonly ignored directories.
 respect-gitignore = true
-ignore-init-module-imports = true
+lint.ignore-init-module-imports = true
+
+[tool.isort]
+profile = "black"
+line_length = 120
+skip_gitignore = true
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_nai3-0.0.9/README.md` & `nonebot_plugin_nai3-0.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -68,22 +68,32 @@
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 | nai3_proxy | 否 | str | None | 代理 |
+| SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
+| SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
 - 3.输入 `console.log(JSON.parse(localStorage.session).auth_token)` 回车, 返回的字符串即为 token
 - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079)
 
+⚠️ SMMS token 的获取:
+
+- 登录SM.MS"
+- 点击"Sign Up"注册一个账号"
+- 输入账号邮箱和密码"
+- 点击"User" > "Dashboard""
+- 点击"API Token", 就可以看到Token, 复制即可使用"
+
 ## 🎉 使用
 
 ```
 指令: nai3/nai
 参数:
     prompt          提示词(支持你喜欢的画风串), 默认: None
     -n/--negative   负面提示词, 默认: nsfw,...
@@ -96,42 +106,51 @@
 示例: nai3 1girl, loli, cute -r mb -s 5.0
 返回: 
 ```
 
 ![img](./img/1.png)
 
 ```
-指令: nai3黑名单/黑名单(需要超级用户, 群主或群管理员权限)
+指令: nai3黑名单/nai黑名单(需要超级用户, 群主或群管理员权限)
 参数:
     添加    添加黑名单
     删除    删除黑名单
     用户    指定添加类型
     群聊    指定添加类型
     群号/QQ号/@sb.
 示例: nai3黑名单添加用户 @脑积水
 返回: 
 ```
 
 ![img](./img/2.png)
 
+```
+指令: nai3帮助/nai帮助
+返回: 展示以上帮助
+```
+
 ## 📖 待办
 
 + [x] 文生图
 + [ ] 图生图
 + [x] 自定义参数
 + [ ] ~~队列功能~~
 + [x] 冷却功能
 + [x] 上限功能
 + [x] 黑名单功能
 + [x] 代理
-+ [ ] R18 检测
++ [x] R18 检测
 + [ ] 翻译
-+ [ ] 帮助指令
++ [x] 帮助指令
++ [x] 检测到 R18 图片生成链接并上报超级用户
++ [ ] 图片保存
 + [ ] ...
 
 ## 🤝 鸣谢
 
-本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv) 
+本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+
+本项目使用 [nonebot-plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) 上传图片
 
 
 <hr>
 <img width="300px" src="https://count.getloli.com/get/@zhulinyv?theme=rule34"></img>
```

#### html2text {}

```diff
@@ -19,29 +19,37 @@
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
-ä»£ç | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
+ä»£ç | | SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API
+å°å | | SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç
+(bushi) | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
 (localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
 [e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) ## ð
-ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt æç¤ºè¯
-(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative è´é¢æç¤ºè¯,
-é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç, ["mb", "pc", "sq"]
-ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm,
-é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨, é»è®¤: k_euler
---schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl, loli, cute -r mb
--s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤: nai3é»åå/é»åå
-(éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å 
-æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è
-æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
-@èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð å¾å + [x] æçå¾ + [ ]
-å¾çå¾ + [x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
-ä¸éåè½ + [x] é»åååè½ + [x] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
-[ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) â ï¸
+SMMS token çè·å: - ç»å½SM.MS" - ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" -
+è¾å¥è´¦å·é®ç®±åå¯ç " - ç¹å»"User" > "Dashboard"" - ç¹å»"API Token",
+å°±å¯ä»¥çå°Token, å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai
+åæ°: prompt æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--
+negative è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/
+åè¾¨ç, ["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale
+æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤:
+False --sampler éæ ·å¨, é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤:
+native ç¤ºä¾: nai3 1girl, loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/
+1.png) ``` æä»¤: nai3é»åå/naié»åå(éè¦è¶çº§ç¨æ·,
+ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å  æ·»å é»åå å é¤
+å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/
+QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./
+img/2.png) ``` æä»¤: nai3å¸®å©/naiå¸®å© è¿å: å±ç¤ºä»¥ä¸å¸®å© ``` ##
+ð å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
+~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
+[x] ä»£ç + [x] R18 æ£æµ + [ ] ç¿»è¯ + [x] å¸®å©æä»¤ + [x] æ£æµå° R18
+å¾ççæé¾æ¥å¹¶ä¸æ¥è¶çº§ç¨æ· + [ ] å¾çä¿å­ + [ ] ... ## ð¤
+é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv) æ¬é¡¹ç®ä½¿ç¨ [nonebot-
+plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) ä¸ä¼ å¾ç
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

### Comparing `nonebot_plugin_nai3-0.0.9/PKG-INFO` & `nonebot_plugin_nai3-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.9
+Version: 0.1.0
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
+Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0)
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
+Requires-Dist: nudenet (>=3.0.8,<4.0.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/raw/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/raw/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
@@ -87,22 +89,32 @@
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
 | nai3_negative | 否 | str | nsfw,... | 负面提示词 |
 | nai3_limit | 否 | int | 10 | 每人最多生成次数 |
 | nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
 | nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 | nai3_proxy | 否 | str | None | 代理 |
+| SMMS_API_URL | 否 | str | "https://sm.ms/api/v2" | SMMS 图床 API 地址 |
+| SMMS_TOKEN | 否 | str | None | 不配置将损失一张 R18 图片(bushi) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
 - 3.输入 `console.log(JSON.parse(localStorage.session).auth_token)` 回车, 返回的字符串即为 token
 - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079)
 
+⚠️ SMMS token 的获取:
+
+- 登录SM.MS"
+- 点击"Sign Up"注册一个账号"
+- 输入账号邮箱和密码"
+- 点击"User" > "Dashboard""
+- 点击"API Token", 就可以看到Token, 复制即可使用"
+
 ## 🎉 使用
 
 ```
 指令: nai3/nai
 参数:
     prompt          提示词(支持你喜欢的画风串), 默认: None
     -n/--negative   负面提示词, 默认: nsfw,...
@@ -115,43 +127,52 @@
 示例: nai3 1girl, loli, cute -r mb -s 5.0
 返回: 
 ```
 
 ![img](./img/1.png)
 
 ```
-指令: nai3黑名单/黑名单(需要超级用户, 群主或群管理员权限)
+指令: nai3黑名单/nai黑名单(需要超级用户, 群主或群管理员权限)
 参数:
     添加    添加黑名单
     删除    删除黑名单
     用户    指定添加类型
     群聊    指定添加类型
     群号/QQ号/@sb.
 示例: nai3黑名单添加用户 @脑积水
 返回: 
 ```
 
 ![img](./img/2.png)
 
+```
+指令: nai3帮助/nai帮助
+返回: 展示以上帮助
+```
+
 ## 📖 待办
 
 + [x] 文生图
 + [ ] 图生图
 + [x] 自定义参数
 + [ ] ~~队列功能~~
 + [x] 冷却功能
 + [x] 上限功能
 + [x] 黑名单功能
 + [x] 代理
-+ [ ] R18 检测
++ [x] R18 检测
 + [ ] 翻译
-+ [ ] 帮助指令
++ [x] 帮助指令
++ [x] 检测到 R18 图片生成链接并上报超级用户
++ [ ] 图片保存
 + [ ] ...
 
 ## 🤝 鸣谢
 
-本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv) 
+本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+
+本项目使用 [nonebot-plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) 上传图片
 
 
 <hr>
 <img width="300px" src="https://count.getloli.com/get/@zhulinyv?theme=rule34"></img>
```

#### html2text {}

```diff
@@ -1,16 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.9 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.1.0 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: ujson
-(>=5.9.0,<6.0.0) Description-Content-Type: text/markdown
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot-plugin-smms (>=0.1.0,<0.2.0) Requires-
+Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: nudenet (>=3.0.8,<4.0.0)
+Requires-Dist: ujson (>=5.9.0,<6.0.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                        ************ nnoonneebboott__pplluuggiinn__nnaaii33 ************
                    ****** ?â??¨?é???è?¿? NNoovveellAAII ?ç???æ???å??¾?ç???â??¨ ******
        [https://img.shields.io/badge/Python-3.9+-blue]_[_l_i_c_e_n_s_e_][https://
       img.shields.io/github/issues/zhulinyv/nonebot_plugin_nai3][https://
       img.shields.io/github/stars/zhulinyv/nonebot_plugin_nai3][https://
@@ -28,29 +29,37 @@
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
 | | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
 nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
 int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
 ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
 | ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_proxy | å¦ | str | None |
-ä»£ç | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
+ä»£ç | | SMMS_API_URL | å¦ | str | "https://sm.ms/api/v2" | SMMS å¾åº API
+å°å | | SMMS_TOKEN | å¦ | str | None | ä¸éç½®å°æå¤±ä¸å¼  R18 å¾ç
+(bushi) | â ï¸ token çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
 (localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
 [e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) ## ð
-ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt æç¤ºè¯
-(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative è´é¢æç¤ºè¯,
-é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç, ["mb", "pc", "sq"]
-ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm,
-é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨, é»è®¤: k_euler
---schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl, loli, cute -r mb
--s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤: nai3é»åå/é»åå
-(éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å 
-æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è
-æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
-@èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð å¾å + [x] æçå¾ + [ ]
-å¾çå¾ + [x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
-ä¸éåè½ + [x] é»åååè½ + [x] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
-[ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) â ï¸
+SMMS token çè·å: - ç»å½SM.MS" - ç¹å»"Sign Up"æ³¨åä¸ä¸ªè´¦å·" -
+è¾å¥è´¦å·é®ç®±åå¯ç " - ç¹å»"User" > "Dashboard"" - ç¹å»"API Token",
+å°±å¯ä»¥çå°Token, å¤å¶å³å¯ä½¿ç¨" ## ð ä½¿ç¨ ``` æä»¤: nai3/nai
+åæ°: prompt æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--
+negative è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/
+åè¾¨ç, ["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale
+æç¤ºè¯ç¸å³æ§, é»è®¤: 5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤:
+False --sampler éæ ·å¨, é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤:
+native ç¤ºä¾: nai3 1girl, loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/
+1.png) ``` æä»¤: nai3é»åå/naié»åå(éè¦è¶çº§ç¨æ·,
+ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å  æ·»å é»åå å é¤
+å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/
+QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./
+img/2.png) ``` æä»¤: nai3å¸®å©/naiå¸®å© è¿å: å±ç¤ºä»¥ä¸å¸®å© ``` ##
+ð å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
+~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
+[x] ä»£ç + [x] R18 æ£æµ + [ ] ç¿»è¯ + [x] å¸®å©æä»¤ + [x] æ£æµå° R18
+å¾ççæé¾æ¥å¹¶ä¸æ¥è¶çº§ç¨æ· + [ ] å¾çä¿å­ + [ ] ... ## ð¤
+é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv) æ¬é¡¹ç®ä½¿ç¨ [nonebot-
+plugin-smms](https://github.com/mobyw/nonebot-plugin-smms) ä¸ä¼ å¾ç
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

