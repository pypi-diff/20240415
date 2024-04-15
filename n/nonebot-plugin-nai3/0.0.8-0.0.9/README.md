# Comparing `tmp/nonebot_plugin_nai3-0.0.8.tar.gz` & `tmp/nonebot_plugin_nai3-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.0.9.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.8.tar` & `nonebot_plugin_nai3-0.0.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.8/LICENSE
--rw-r--r--   0        0        0     8609 2024-04-14 12:59:22.863533 nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      555 2024-04-14 12:42:27.741067 nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     2426 2024-04-14 12:58:41.611610 nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      864 2024-04-14 13:01:54.179224 nonebot_plugin_nai3-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4364 2024-04-14 13:01:30.277514 nonebot_plugin_nai3-0.0.8/README.md
--rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.9/LICENSE
+-rw-r--r--   0        0        0     8561 2024-04-14 23:09:41.177004 nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      555 2024-04-14 12:42:27.741067 nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2426 2024-04-14 12:58:41.611610 nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0      864 2024-04-14 23:08:45.840659 nonebot_plugin_nai3-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4364 2024-04-14 13:30:50.170244 nonebot_plugin_nai3-0.0.9/README.md
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.9/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.8/LICENSE` & `nonebot_plugin_nai3-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,18 @@
     __version__ = version("nonebot_plugin_nai3")
 except Exception:
     __version__ = "0.0.0"
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-nai3",
     description="通过 NovelAI 生成图片",
-    usage="通过 NovelAI 生成图片",
+    usage="nai3/nai prompt args",
     homepage="https://github.com/zhulinyv/nonebot_plugin_nai3",
     type="application",
-    supported_adapters={
-        "~onebot.v11",
-        "~onebot.v12",
-    },
+    supported_adapters={"~onebot.v11"},
     config=Config,
     extra={
         "author": "zhulinyv",
         "version": __version__,
     },
 )
```

### Comparing `nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.8/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.0.9/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.8/pyproject.toml` & `nonebot_plugin_nai3-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.8"
+version = "0.0.9"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.0.8/README.md` & `nonebot_plugin_nai3-0.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 + [x] 文生图
 + [ ] 图生图
 + [x] 自定义参数
 + [ ] ~~队列功能~~
 + [x] 冷却功能
 + [x] 上限功能
 + [x] 黑名单功能
-+ [ ] 代理
++ [x] 代理
 + [ ] R18 检测
 + [ ] 翻译
 + [ ] 帮助指令
 + [ ] ...
 
 ## 🤝 鸣谢
```

#### html2text {}

```diff
@@ -36,12 +36,12 @@
 --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl, loli, cute -r mb
 -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤: nai3é»åå/é»åå
 (éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å 
 æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è
 æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
 @èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð å¾å + [x] æçå¾ + [ ]
 å¾çå¾ + [x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
-ä¸éåè½ + [x] é»åååè½ + [ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
+ä¸éåè½ + [x] é»åååè½ + [x] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
 [ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
 NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

### Comparing `nonebot_plugin_nai3-0.0.8/PKG-INFO` & `nonebot_plugin_nai3-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.8
+Version: 0.0.9
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -137,15 +137,15 @@
 + [x] 文生图
 + [ ] 图生图
 + [x] 自定义参数
 + [ ] ~~队列功能~~
 + [x] 冷却功能
 + [x] 上限功能
 + [x] 黑名单功能
-+ [ ] 代理
++ [x] 代理
 + [ ] R18 检测
 + [ ] 翻译
 + [ ] 帮助指令
 + [ ] ...
 
 ## 🤝 鸣谢
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.8 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.9 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: ujson
@@ -45,12 +45,12 @@
 --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl, loli, cute -r mb
 -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤: nai3é»åå/é»åå
 (éè¦è¶çº§ç¨æ·, ç¾¤ä¸»æç¾¤ç®¡çåæé) åæ°: æ·»å 
 æ·»å é»åå å é¤ å é¤é»åå ç¨æ· æå®æ·»å ç±»å ç¾¤è
 æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾: nai3é»ååæ·»å ç¨æ·
 @èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð å¾å + [x] æçå¾ + [ ]
 å¾çå¾ + [x] èªå®ä¹åæ° + [ ] ~~éååè½~~ + [x] å·å´åè½ + [x]
-ä¸éåè½ + [x] é»åååè½ + [ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
+ä¸éåè½ + [x] é»åååè½ + [x] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ +
 [ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-
 NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

