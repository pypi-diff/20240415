# Comparing `tmp/xagent-0.0.5.tar.gz` & `tmp/xagent-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xagent-0.0.5.tar", last modified: Fri Mar 29 02:12:59 2024, max compression
+gzip compressed data, was "xagent-0.0.6.tar", last modified: Mon Apr 15 04:06:31 2024, max compression
```

## Comparing `xagent-0.0.5.tar` & `xagent-0.0.6.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.268711 xagent-0.0.5/
--rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.5/LICENSE
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-03-29 02:12:59.268511 xagent-0.0.5/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)     1598 2024-03-28 09:35:56.000000 xagent-0.0.5/README.md
--rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-03-29 02:12:59.268757 xagent-0.0.5/setup.cfg
--rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.5/setup.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.266677 xagent-0.0.5/tests/
--rw-r--r--   0 chenhao    (501) staff       (20)      335 2024-03-14 09:35:14.000000 xagent-0.0.5/tests/test_service.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.268246 xagent-0.0.5/xagent.egg-info/
--rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-03-29 02:12:59.000000 xagent-0.0.5/xagent.egg-info/PKG-INFO
--rw-r--r--   0 chenhao    (501) staff       (20)      994 2024-03-29 02:12:59.000000 xagent-0.0.5/xagent.egg-info/SOURCES.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-03-29 02:12:59.000000 xagent-0.0.5/xagent.egg-info/dependency_links.txt
--rw-r--r--   0 chenhao    (501) staff       (20)      103 2024-03-29 02:12:59.000000 xagent-0.0.5/xagent.egg-info/requires.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-03-29 02:12:59.000000 xagent-0.0.5/xagent.egg-info/top_level.txt
--rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-03-29 02:12:59.000000 xagent-0.0.5/xagent.egg-info/zip-safe
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.253286 xagent-0.0.5/xagents/
--rw-r--r--   0 chenhao    (501) staff       (20)      566 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/__init__.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.255184 xagent-0.0.5/xagents/agent/
--rw-r--r--   0 chenhao    (501) staff       (20)      187 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/agent/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)      949 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/agent/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)      788 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/agent/memory.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5801 2024-03-19 07:41:09.000000 xagent-0.0.5/xagents/agent/xagent.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1090 2024-03-28 09:35:52.000000 xagent-0.0.5/xagents/config.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.258329 xagent-0.0.5/xagents/kb/
--rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.5/xagents/kb/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     8889 2024-03-29 02:09:53.000000 xagent-0.0.5/xagents/kb/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     6559 2024-03-20 02:46:15.000000 xagent-0.0.5/xagents/kb/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)    11039 2024-03-28 09:35:52.000000 xagent-0.0.5/xagents/kb/kb.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2492 2024-03-20 03:10:39.000000 xagent-0.0.5/xagents/kb/kb_file.py
--rw-r--r--   0 chenhao    (501) staff       (20)     4582 2024-03-21 08:50:06.000000 xagent-0.0.5/xagents/kb/vector_store.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.261516 xagent-0.0.5/xagents/loader/
--rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.5/xagents/loader/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3651 2024-03-28 09:35:52.000000 xagent-0.0.5/xagents/loader/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)      983 2024-03-28 09:36:52.000000 xagent-0.0.5/xagents/loader/common.py
--rw-r--r--   0 chenhao    (501) staff       (20)      863 2024-03-19 10:49:45.000000 xagent-0.0.5/xagents/loader/markdown.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1960 2024-03-28 09:36:56.000000 xagent-0.0.5/xagents/loader/pdf.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3913 2024-03-18 07:41:58.000000 xagent-0.0.5/xagents/loader/splitter.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1764 2024-03-19 10:49:57.000000 xagent-0.0.5/xagents/loader/structed.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.264591 xagent-0.0.5/xagents/model/
--rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.5/xagents/model/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)     2733 2024-03-28 10:32:09.000000 xagent-0.0.5/xagents/model/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1701 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/model/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5117 2024-03-29 02:07:36.000000 xagent-0.0.5/xagents/model/local.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.5/xagents/model/openai.py
--rw-r--r--   0 chenhao    (501) staff       (20)     3466 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/model/wind.py
--rw-r--r--   0 chenhao    (501) staff       (20)     5079 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/model/zhipu.py
-drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-03-29 02:12:59.266311 xagent-0.0.5/xagents/tool/
--rw-r--r--   0 chenhao    (501) staff       (20)      252 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/tool/__init__.py
--rw-r--r--   0 chenhao    (501) staff       (20)      950 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/tool/api.py
--rw-r--r--   0 chenhao    (501) staff       (20)      938 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/tool/common_tool.py
--rw-r--r--   0 chenhao    (501) staff       (20)     1685 2024-03-14 09:35:14.000000 xagent-0.0.5/xagents/tool/core.py
--rw-r--r--   0 chenhao    (501) staff       (20)      555 2024-03-15 08:10:20.000000 xagent-0.0.5/xagents/util.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:31.003597 xagent-0.0.6/
+-rw-r--r--   0 chenhao    (501) staff       (20)     1063 2024-03-14 09:35:14.000000 xagent-0.0.6/LICENSE
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-15 04:06:31.003375 xagent-0.0.6/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     3568 2024-04-15 04:02:55.000000 xagent-0.0.6/README.md
+-rw-r--r--   0 chenhao    (501) staff       (20)       38 2024-04-15 04:06:31.003703 xagent-0.0.6/setup.cfg
+-rw-r--r--   0 chenhao    (501) staff       (20)     1207 2024-03-21 03:48:59.000000 xagent-0.0.6/setup.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:31.001157 xagent-0.0.6/tests/
+-rw-r--r--   0 chenhao    (501) staff       (20)      944 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_loader.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2569 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_local_model.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4886 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4747 2024-04-15 04:02:55.000000 xagent-0.0.6/tests/test_zhipu_api_model.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:31.003088 xagent-0.0.6/xagent.egg-info/
+-rw-r--r--   0 chenhao    (501) staff       (20)      231 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/PKG-INFO
+-rw-r--r--   0 chenhao    (501) staff       (20)     1097 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/SOURCES.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/dependency_links.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)      123 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/requires.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        8 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/top_level.txt
+-rw-r--r--   0 chenhao    (501) staff       (20)        1 2024-04-15 04:06:30.000000 xagent-0.0.6/xagent.egg-info/zip-safe
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.986846 xagent-0.0.6/xagents/
+-rw-r--r--   0 chenhao    (501) staff       (20)      667 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/__init__.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.988963 xagent-0.0.6/xagents/agent/
+-rw-r--r--   0 chenhao    (501) staff       (20)      213 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3157 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1067 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      811 2024-04-08 07:28:32.000000 xagent-0.0.6/xagents/agent/memory.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     7027 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/agent/xagent.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1337 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/config.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.991715 xagent-0.0.6/xagents/kb/
+-rw-r--r--   0 chenhao    (501) staff       (20)      178 2024-03-19 07:40:40.000000 xagent-0.0.6/xagents/kb/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     9629 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/kb/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     6559 2024-03-20 02:46:15.000000 xagent-0.0.6/xagents/kb/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)    11172 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/kb/kb.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2492 2024-03-20 03:10:39.000000 xagent-0.0.6/xagents/kb/kb_file.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4583 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/kb/vector_store.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.994953 xagent-0.0.6/xagents/loader/
+-rw-r--r--   0 chenhao    (501) staff       (20)      152 2024-03-19 10:48:10.000000 xagent-0.0.6/xagents/loader/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4112 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/loader/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      983 2024-03-28 09:36:52.000000 xagent-0.0.6/xagents/loader/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1358 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/loader/doc.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      863 2024-03-19 10:49:45.000000 xagent-0.0.6/xagents/loader/markdown.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2721 2024-04-08 07:28:32.000000 xagent-0.0.6/xagents/loader/pdf.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     3917 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/loader/splitter.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1809 2024-04-08 07:28:32.000000 xagent-0.0.6/xagents/loader/structed.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.997525 xagent-0.0.6/xagents/model/
+-rw-r--r--   0 chenhao    (501) staff       (20)      179 2024-03-20 06:50:45.000000 xagent-0.0.6/xagents/model/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2800 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2442 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/common.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     2224 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/local.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1234 2024-03-21 07:20:01.000000 xagent-0.0.6/xagents/model/openai.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     4064 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/model/zhipu.py
+drwxr-xr-x   0 chenhao    (501) staff       (20)        0 2024-04-15 04:06:30.999209 xagent-0.0.6/xagents/tool/
+-rw-r--r--   0 chenhao    (501) staff       (20)      226 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/__init__.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1358 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/api.py
+-rw-r--r--   0 chenhao    (501) staff       (20)     1631 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/common_tool.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      453 2024-04-15 04:02:55.000000 xagent-0.0.6/xagents/tool/core.py
+-rw-r--r--   0 chenhao    (501) staff       (20)      555 2024-03-15 08:10:20.000000 xagent-0.0.6/xagents/util.py
```

### Comparing `xagent-0.0.5/LICENSE` & `xagent-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/setup.py` & `xagent-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/xagent.egg-info/SOURCES.txt` & `xagent-0.0.6/xagent.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 LICENSE
 README.md
 setup.py
 ./xagents/__init__.py
 ./xagents/config.py
 ./xagents/util.py
 ./xagents/agent/__init__.py
-./xagents/agent/core.py
+./xagents/agent/api.py
+./xagents/agent/common.py
 ./xagents/agent/memory.py
 ./xagents/agent/xagent.py
 ./xagents/kb/__init__.py
 ./xagents/kb/api.py
 ./xagents/kb/common.py
 ./xagents/kb/kb.py
 ./xagents/kb/kb_file.py
 ./xagents/kb/vector_store.py
 ./xagents/loader/__init__.py
 ./xagents/loader/api.py
 ./xagents/loader/common.py
+./xagents/loader/doc.py
 ./xagents/loader/markdown.py
 ./xagents/loader/pdf.py
 ./xagents/loader/splitter.py
 ./xagents/loader/structed.py
 ./xagents/model/__init__.py
 ./xagents/model/api.py
-./xagents/model/core.py
+./xagents/model/common.py
 ./xagents/model/local.py
 ./xagents/model/openai.py
-./xagents/model/wind.py
 ./xagents/model/zhipu.py
 ./xagents/tool/__init__.py
 ./xagents/tool/api.py
 ./xagents/tool/common_tool.py
 ./xagents/tool/core.py
-tests/test_service.py
+tests/test_loader.py
+tests/test_local_model.py
+tests/test_xagent.py
+tests/test_zhipu_api_model.py
 xagent.egg-info/PKG-INFO
 xagent.egg-info/SOURCES.txt
 xagent.egg-info/dependency_links.txt
 xagent.egg-info/requires.txt
 xagent.egg-info/top_level.txt
 xagent.egg-info/zip-safe
```

### Comparing `xagent-0.0.5/xagents/__init__.py` & `xagent-0.0.6/xagents/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,19 +11,23 @@
 from xagents.config import *
 from snippets import print_info, set_logger
 
 
 
     
 set_logger(env = XAGENT_ENV, module_name=__name__, log_dir=LOG_DIR)
+set_logger(XAGENT_ENV, "__main__")
+
 
 def show_env():
     print_info("current XAgent env", logger)
     logger.info(f"{XAGENT_ENV=}")
     logger.info(f"{KNOWLEDGE_BASE_DIR=}")
     logger.info(f"{TEMP_DIR=}")
     logger.info(f"{LOG_DIR=}")
+    logger.info(f"{AGENT_DIR=}")
+    logger.info(f"{DATA_DIR=}")
     print_info("", logger)
 
 show_env()
```

### Comparing `xagent-0.0.5/xagents/agent/core.py` & `xagent-0.0.6/xagents/agent/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,35 +2,39 @@
 # -*- encoding: utf-8 -*-
 '''
 @Time    :   2023/12/07 17:54:34
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
-from typing import Generator, List, Optional, Union
+from typing import List, Optional
 
 from abc import abstractmethod
 
 from pydantic import BaseModel, Field
 
+from agit.common import LLMResp
+from xagents.config import DEFAULT_KB_PROMPT_TEMPLATE
 from xagents.kb.common import RecalledChunk
-from xagents.tool.core import ToolCall
 
 
-class AgentResp(BaseModel):
-    content: Union[str, Generator] = Field(description="返回的消息活生成器")
+class AgentResp(LLMResp):
     references: Optional[List[RecalledChunk]] = Field(description="召回的片段")
-    tool_call:Optional[ToolCall] = Field(description="工具调用")
+
 
 
 class AbstractAgent:
 
     def __init__(self, name) -> None:
         self.name = name
 
     @abstractmethod
     def chat(self, message: str, stream=True, do_remember=True) -> AgentResp:
         raise NotImplementedError
 
     @abstractmethod
     def remember(self, role: str, message: str):
         raise NotImplementedError
+
+class KBConfig(BaseModel):
+    name: str = Field(description="知识库名称")
+    prompt_template:str = Field(description="应用知识库的提示词模板, 必须包含{context}和{question}两个字段", default=DEFAULT_KB_PROMPT_TEMPLATE)
```

### Comparing `xagent-0.0.5/xagents/agent/memory.py` & `xagent-0.0.6/xagents/agent/memory.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 @Time    :   2023/12/07 18:33:25
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 from abc import abstractmethod
+import copy
 
 
 class AbstractMemory:
     @abstractmethod
     def remember(self, role: str, content: str):
         raise NotImplementedError
 
@@ -28,11 +29,11 @@
         self.size = size
         self.memory = []
 
     def remember(self, role: str, content: str):
         self.memory.append(dict(role=role, content=content))
 
     def to_llm_history(self):
-        return self.memory
+        return copy.copy(self.memory)
 
     def clear(self):
         self.memory.clear()
```

### Comparing `xagent-0.0.5/xagents/agent/xagent.py` & `xagent-0.0.6/xagents/agent/xagent.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,103 +4,142 @@
 @Time    :   2023/12/07 17:57:13
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 import os
-from typing import Generator, List, Union
+from typing import Generator, List, Optional
 
-from xagents.agent.core import AbstractAgent, AgentResp
-from xagents.config import DEFAULT_KB_PROMPT_TEMPLATE, LOG_DIR
+from pydantic import BaseModel, Field
+
+from agit.common import LLMResp
+from xagents.model.common import LLMGenConfig
+from xagents.agent.common import AbstractAgent, AgentResp, KBConfig
+from xagents.config import LOG_DIR
 from xagents.kb.common import RecalledChunk
-from xagents.kb.core import KnowledgeBaseInfo
-from xagents.kb.api import get_knowledge_base
+from xagents.kb.api import KBSearchConfig, get_knowledge_base
 from xagents.model.api import get_llm_model
-from agent.memory import BaseMemory
+from xagents.agent.memory import BaseMemory
 from xagents.tool.api import invoke_tool_call
 from xagents.tool.core import BaseTool, ToolCall
+from snippets import dump, load
 
 from loguru import logger
 
 agent_log_path = os.path.join(LOG_DIR, "xagent.log")
 
-# logger.add(agent_log_path, rotation="00:00", retention="7 days", level="INFO", filter=__name__, format=LoguruFormat.SIMPLE)
+
+class XAgentInfo(BaseModel):
+    name: str = Field(description="agent的名称，唯一键")
+    llm_config: dict = Field(description="llm的配置信息")
+    memory_config: dict = Field(description="memory的配置信息")
+    kb_config: Optional[KBConfig] = Field(description="kb的配置信息")
+    tools: List[BaseTool] = Field(description="工具列表")
 
 
 class XAgent(AbstractAgent):
 
     def __init__(self, name: str,
                  llm_config: dict,
                  memory_config: dict,
-                 tools: List[BaseTool] = [],
-                 kb: Union[str, KnowledgeBaseInfo] = None,
-                 kb_prompt_template: str = DEFAULT_KB_PROMPT_TEMPLATE) -> None:
+                 kb_config: KBConfig,
+                 tools: List[BaseTool] = []) -> None:
         super().__init__(name=name)
+        self.info = XAgentInfo(name=name, llm_config=llm_config, memory_config=memory_config, kb_config=kb_config, tools=tools)
+
         self.llm_model = get_llm_model(llm_config)
         self.memory = BaseMemory(**memory_config)
-        if kb:
-            if isinstance(kb, str):
-                logger.debug(f"loading kb: {kb}")
-                self.kb = get_knowledge_base(kb)
-            else:
-                self.kb = kb
-        else:
-            self.kb = None
-        self.kb_prompt_template = kb_prompt_template
+        self._load_kb(kb_config)
         self.tools = tools
 
+    def _load_kb(self, kb_config: KBConfig):
+        if not kb_config:
+            self.kb = None
+            self.kb_prompt_template = None
+        else:
+            self.kb = get_knowledge_base(kb_config.name)
+            self.kb_prompt_template = kb_config.prompt_template
+            logger.info("load kb finish")
+
+    def get_info(self):
+        return self.info
+
     def search_kb(self, query: str, **kwargs) -> List[RecalledChunk]:
-        if not self.kb:
-            logger.warning('No knowledge base found! Will return empty recall chunks')
-            return []
         chunks = self.kb.search(query=query, **kwargs)
         return chunks
 
     def use_tool(self, tool_call: ToolCall):
         resp = invoke_tool_call(tool_call)
+        tool_call.resp = resp
         return resp
 
-    def chat(self, message: str, stream=True, do_remember=True,
-             use_kb=False, top_k=3, score_threshold=None, temperature=0.01,
-             do_split_query=False, fake_chat=False, file_names: List[str] = None,
-             do_expand=False, expand_len: int = 500, forward_rate: float = 0.5, rerank_config: dict = dict(),
-             **kwargs) -> AgentResp:
+    @staticmethod
+    def _get_agent_config_path(dir_path: str, agent_name: str):
+        return os.path.join(dir_path, agent_name+".json")
+
+    def save(self, save_dir: str):
+        save_path = self._get_agent_config_path(save_dir, self.name)
+        logger.info(f"save agent:{self.name} to {save_path}")
+        logger.debug(f"agent info:{self.get_info()}")
+        dump(self.get_info().model_dump(), save_path)
+
+    @classmethod
+    def load(cls, save_dir: str, name: str) -> "XAgent":
+        config_path = cls._get_agent_config_path(save_dir, name)
+        if not os.path.exists(config_path):
+            raise FileExistsError(f"config file {config_path} not found")
+
+        kwargs = load(config_path)
+        if kwargs.get("kb_config"):
+            kwargs["kb_config"] = KBConfig.model_validate(kwargs["kb_config"])
+        logger.debug(f"{kwargs=}")
+
+        return XAgent(**kwargs)
+
+    def chat(self, message: str, do_remember=True, details=False, stream=False,
+             use_kb=False, kb_search_config: KBSearchConfig = KBSearchConfig(),
+             fake_chat=False, llm_gen_config: LLMGenConfig = LLMGenConfig(), **kwargs) -> AgentResp:
         logger.info(f"agent get message:{message}")
 
         if use_kb:
-            logger.info("agent searching kb")
-            chunks = self.search_kb(query=message, top_k=top_k, score_threshold=score_threshold, do_split_query=do_split_query,
-                                    do_expand=do_expand, expand_len=expand_len, forward_rate=forward_rate, file_names=file_names, rerank_config=rerank_config)
-            logger.info(f"agent get {len(chunks)} chunks :{chunks}")
-            logger.info(f"sample chunks:{chunks[:3]}")
-            context = "\n".join(f"{idx+1}." + c.to_plain_text() for idx, c in enumerate(chunks))
 
-            prompt = self.kb_prompt_template.format(question=message, context=context)
+            if not self.kb or not self.kb_prompt_template:
+                logger.warning(f"agent:{self.name} has no related knowledge base, will not chat with kb! ")
+                prompt = message
+                chunks = None
+
+            else:
+                logger.info("agent searching kb")
+                chunks = self.search_kb(query=message, **kb_search_config.model_dump())
+                # logger.info(f"agent get {len(chunks)} chunks :{chunks}")
+                # logger.info(f"sample chunks:{chunks[:3]}")
+                context = "\n".join(f"{idx+1}." + c.to_plain_text() for idx, c in enumerate(chunks))
+
+                prompt = self.kb_prompt_template.format(question=message, context=context)
         else:
             prompt = message
             chunks = None
 
         if fake_chat:
             fake_resp = "这是MOCK的回答信息,如果需要真实回答,请设置fake_chat=False"
-            model_resp = (e for e in fake_resp) if stream else fake_resp
+            llm_resp = (e for e in fake_resp) if stream else fake_resp
             tool_call = None
         else:
-            tool_call, model_resp = self.llm_model.generate(prompt=prompt, history=self.memory.to_llm_history(), tools=self.tools,
-                                                            temperature=temperature, stream=stream, **kwargs)
+            history = self.memory.to_llm_history()
+            llm_resp: LLMResp = self.llm_model.generate(prompt=prompt, history=history, tools=self.tools, details=details, stream=stream,
+                                                        **llm_gen_config.model_dump(), **kwargs)
             # 调用tool
-            if tool_call:
-                logger.debug(f"calling tool:{tool_call.name}")
-                self.use_tool(tool_call)
-                history = self.memory.to_llm_history() + [dict(role="user", content=prompt)]
-                model_resp = self.llm_model.observe(tool_call, tools=self.tools, history=history,
-                                                    stream=stream, temperature=temperature, **kwargs)
-                model_resp = "".join(model_resp)
-                logger.debug(f"observe tool call resp: {model_resp}")
-                model_resp = (e for e in model_resp)
+            tool_calls = llm_resp.tool_calls
+            if tool_calls:
+                for tool_call in tool_calls:
+                    logger.debug(f"calling tool:{tool_call.name}")
+                    self.use_tool(tool_call)
+                    llm_resp = self.llm_model.observe(prompt=prompt, tool_call=tool_call, tools=self.tools, history=history, details=details, stream=stream,
+                                                      **llm_gen_config.model_dump(), **kwargs)
 
         def _remember_callback(resp_str):
             if do_remember:
                 self.remember("user", message)
                 self.remember("assistant", resp_str)
 
         def _add_remember_callback(gen: Generator) -> Generator:
@@ -109,21 +148,21 @@
                 acc.append(ele)
                 yield ele
             resp_str = "".join(acc)
             logger.info(f"agent generate response:{resp_str}")
             _remember_callback("".join(acc))
 
         if stream:
-            model_message = _add_remember_callback(model_resp)
+            content = _add_remember_callback(llm_resp.content)
         else:
-            model_message = model_resp
-            logger.info(f"generate response:{model_message}")
-            _remember_callback(model_message)
+            content = llm_resp.content
+            logger.info(f"generate response:{content}")
+            _remember_callback(content)
 
-        resp = AgentResp(content=model_message, references=chunks, tool_call=tool_call)
+        resp = AgentResp(content=content, tool_calls=llm_resp.tool_calls, usage=llm_resp.usage, references=chunks, details=llm_resp.details)
         return resp
 
     def remember(self, role: str, message: str):
         logger.debug(f"remembering {role=}, {message=}")
         self.memory.remember(role, message)
 
     def clear_memory(self):
```

### Comparing `xagent-0.0.5/xagents/kb/api.py` & `xagent-0.0.6/xagents/kb/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from typing import List
 from fastapi import UploadFile
 from loguru import logger
+from pydantic import BaseModel, Field
 from xagents.kb.kb_file import KnowledgeBaseFile
 from xagents.kb.kb import KnowledgeBase
 from xagents.config import *
 from xagents.kb.common import KnowledgeBaseInfo, KnowledgeBaseFileInfo, RecalledChunk, get_config_path, get_kb_dir, DistanceStrategy
 
 
 def list_knowledge_base_names() -> List[str]:
@@ -117,14 +118,25 @@
     """
     kb = get_knowledge_base(name=name)
     kb.rebuild_index(reindex=reindex, batch_size=batch_size)
     msg = f"知识库【{name}】重建索引成功"
     return msg
 
 
+class KBSearchConfig(BaseModel):
+    top_k:int = Field(default=3, description="返回几个chunk")
+    score_threshold:float = Field(default=0., description="分数阈值")
+    do_split_query:bool = Field(default=False, description="是否分词")
+    file_names:List[str] = Field(default=[], description="需要筛选的知识库文件文件名列表")
+    rerank_config:dict = Field(default={}, description="rerank的配置")
+    do_expand:bool = Field(default=False, description="对结果是否进行上下文扩展")
+    expand_len:int = Field(default=500, description="上下文扩展的长度")
+    forward_rate:float = Field(default=0.5, description="上下文扩展向下扩展的比例")
+    
+
 def search_knowledge_base(name: str,
                           query: str, top_k: int = 3, score_threshold: float = None,
                           do_split_query=False, file_names: List[str] = [], rerank_config: dict = {},
                           do_expand=False, expand_len: int = 500, forward_rate: float = 0.5) -> List[RecalledChunk]:
     kb = get_knowledge_base(name=name)
     
     chunks = kb.search(query=query, top_k=top_k, score_threshold=score_threshold, do_split_query=do_split_query,
@@ -153,15 +165,14 @@
 
 def create_kb_file(kb_name: str, file: UploadFile | str, do_cut=True, do_index=True,
                    batch_size:int=16,
                    cut_config: dict = dict(separator='\n',
                                            max_len=200,
                                            min_len=10)) -> KnowledgeBaseFileInfo:
     """创建知识库文件
-
     Args:
         kb_name (str): 知识库名称
         file (UploadFile | str): 知识库文件，UploadFile(fast_api)或者str(文件路径)
         do_cut (bool, optional): 是否切分文件. Defaults to True.
         do_index (bool, optional): 是否添加到索引. Defaults to True.
         cut_config (dict, optional): 切分文件的参数. Defaults to dict(separator='\n', max_len=200, min_len=10).
 
@@ -234,15 +245,14 @@
 
     kb_file = get_kb_file(kb_name=kb_name, file_name=file_name)
     chunk_num = kb_file.cut(separator=separator, max_len=max_len, min_len=min_len)
     return chunk_num
 
 
 def reindex_kb_file(kb_name: str, file_name: str, reindex=False,  batch_size=16) -> str:
-
     """添加知识库文件到索引中
 
     Args:
         kb_name (str): 知识库名称
         file_name (str): 知识库文件名称
         reindex (bool, optional): 如果知识库文件已经存在，是否重新构建索引. Defaults to False.
```

### Comparing `xagent-0.0.5/xagents/kb/common.py` & `xagent-0.0.6/xagents/kb/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/xagents/kb/kb.py` & `xagent-0.0.6/xagents/kb/kb.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         # 每个子query做检索
         for query in queries:
             score_threshold = _get_score(score_threshold)
             logger.debug(f"searching {query} with vecstore_cls: {index.__class__.__name__}, {_filter=}, {top_k=}, {score_threshold=}")
 
             docs_with_score = index.similarity_search_with_score(query, k=top_k, score_threshold=score_threshold, filter=_filter)
             logger.debug(f"{len(docs_with_score)} origin chunks found for {query}")
-            logger.debug(f"{query}'s related docs{[d.page_content[:5] for d,s in docs_with_score]}")
+            # logger.debug(f"{query}'s related docs{[d.page_content[:5] for d,s in docs_with_score]}")
             # logger.debug(docs_with_score[0])
 
             tmp_recalled_chunks = [RecalledChunk.from_document(d, score=_get_score(s), query=query) for d, s in docs_with_score]
             recalled_chunks.extend(tmp_recalled_chunks)
 
         # 去重，避免召回相同切片
         recalled_chunks = list(set(recalled_chunks))
@@ -238,14 +238,16 @@
         return rs
     else:
         # 不需要切分也转成list形式，方便后续统一处理
         return [query]
 
 
 # 扩展上下文到给定的长度
+#TODO 扩展时，避免重复的chunk
+#TODO 扩展时，截断chunk以达到固定数目，Agent问答单测可以检验此问题
 def expand_chunk(chunk: RecalledChunk, expand_len: int, forward_rate=0.5) -> RecalledChunk:
     logger.debug(f"expanding chunk {chunk}")
     chunk_path = get_chunk_path(chunk.kb_name, chunk.file_name)
     chunks = []
     for item in load(chunk_path):
         tmp = Chunk(**item)
         chunks.append(tmp)
```

### Comparing `xagent-0.0.5/xagents/kb/kb_file.py` & `xagent-0.0.6/xagents/kb/kb_file.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/xagents/kb/vector_store.py` & `xagent-0.0.6/xagents/kb/vector_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from langchain.vectorstores.faiss import FAISS
 import faiss
 from langchain.vectorstores import VectorStore
 from langchain.docstore.in_memory import InMemoryDocstore
 from langchain.vectorstores.elasticsearch import ElasticsearchStore
 from langchain.vectorstores import VectorStore as VectorStore
 
-from xagents.model.core import EMBD
+from xagents.model.common import EMBD
 from xagents.kb.common import DistanceStrategy
 
 from loguru import logger
 
 
 class XVecStore(VectorStore):
     @classmethod
@@ -65,15 +65,15 @@
     @classmethod
     def from_config(cls, config: dict) ->"XFAISS":
         local_dir: str = config["local_dir"]
         embedding: EMBD = config["embedding"]
         distance_strategy = config.get("distance_strategy", DistanceStrategy.MAX_INNER_PRODUCT)
 
         if os.path.exists(local_dir):
-            logger.debug(f"loading vecstore from {local_dir}")
+            logger.info(f"loading vecstore from {local_dir}")
             vecstore = cls.load_local(local_dir=local_dir, embedding=embedding, distance_strategy=distance_strategy)
         else:
             logger.info(f"{local_dir} not exists, create a new local vecstore")
 
             dim_len = embedding.get_dim()
 
             # faiss = dependable_faiss_import()
```

### Comparing `xagent-0.0.5/xagents/loader/api.py` & `xagent-0.0.6/xagents/loader/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 @Contact :   jerrychen1990@gmail.com
 '''
 
 import os
 from loguru import logger
 from typing import Iterable, List, Type
 from xagents.loader.pdf import PDFLoader
+from xagents.loader.doc import DOCLoader
+
 from xagents.loader.markdown import MarkDownLoader
 from xagents.loader.structed import StructedLoader
 from xagents.loader.common import Chunk, AbstractLoader
 
 from xagents.loader.splitter import BaseSplitter
 from snippets import flat, log_cost_time
 
@@ -22,14 +24,16 @@
     "pdf": PDFLoader,
     "markdown": MarkDownLoader,
     "md": MarkDownLoader,
     "json": StructedLoader,
     "jsonl": StructedLoader,
     "csv": StructedLoader,
     "txt": MarkDownLoader,
+    "doc": DOCLoader,
+    "docx": DOCLoader,
     "": MarkDownLoader
 }
 
 
 def get_loader_cls(file_path: str) -> Type[AbstractLoader]:
     """根据file路径后缀，加载对应的文档加载器
 
@@ -43,69 +47,83 @@
         Type[AbstractLoader]: 文档加载器class
     """
     ext = os.path.splitext(file_path)[-1].lower().replace(".", "")
     if ext not in _EXT2LOADER:
         msg = f"{ext} not support!"
         raise ValueError(msg)
 
-    loader_cls = _EXT2LOADER[ext]    
+    loader_cls = _EXT2LOADER[ext]
     return loader_cls
 
+
 @log_cost_time(name="load file", logger=logger)
 def load_file(file_path: str, **kwargs) -> Iterable[Chunk]:
     loader_cls = get_loader_cls(file_path)
     loader: AbstractLoader = loader_cls(**kwargs)
     logger.debug(f"loading {file_path} with loader:{loader}")
     pages = loader.load(file_path)
     return pages
 
-def convert2txt(file_path:str, dst_path:str=None, **kwargs)->str:
+
+def convert2txt(file_path: str, dst_path: str = None, **kwargs) -> str:
     """将原始文件转移成txt格式
 
     Args:
         file_path (str): 原始文件路径
         dst_path (str, optional): 目标路径，未传的话，和原始文件同目录. Defaults to None.
 
     Returns:
         str: 目标路径
     """
     chunks = load_file(file_path, **kwargs)
     if not dst_path:
-        dst_path =file_path+".txt"
+        dst_path = file_path+".txt"
     with open(dst_path, 'w', encoding='utf-8') as f:
         for chunk in chunks:
             f.write(chunk.content)
     return dst_path
 
+
 def parse_file(file_path: str,
-               extract_images = False,
-               max_page:int = None,
-               do_cut:bool = True,
+               extract_images=False,
+               extract_tables=False,
+               max_page: int = None,
+               do_cut: bool = True,
                separator: str = '\n',
                max_len: int = 200,
                min_len: int = 10) -> List[Chunk]:
     """切分文档，并且按照jsonl格式存储在chunk目录下
 
     Args:
-        kb_name (str): 知识库名称
-        file_name (str): 文件名称
+        file_path (str): 文件路径
         extract_images (str, Optional): 是否识别图片中的文字
+        extract_images (str, Optional): 是否识别文档中的表格
         do_cut(str, Optional): 是否做切片,默认True
         max+page(int, Optional):最多处理多少页，默认为None，即识别所有页
         separator (str, optional): 切分符. Defaults to '\n'.
         max_len (int, optional): 最大切片长度. Defaults to 200.
         min_len (int, optional): 最小切片长度. Defaults to 10.
 
     Returns:
         切片列表
     """
     splitter = BaseSplitter(max_len=max_len, min_len=min_len, separator=separator)
 
-    origin_chunks: Iterable[Chunk] = load_file(file_path=file_path, max_page=max_page, extract_images=extract_images)
+    origin_chunks: Iterable[Chunk] = load_file(file_path=file_path, max_page=max_page, extract_images=extract_images, extract_tables=extract_tables)
     origin_chunks = list(origin_chunks)
     logger.debug(f"load {len(origin_chunks)} origin_chunks")
     if do_cut:
         split_chunks = flat([splitter.split_chunk(origin_chunk) for origin_chunk in origin_chunks])
         logger.info(f"split {len(origin_chunks)} origin_chunks to {len(split_chunks)} chunks")
         return split_chunks
     else:
-        return origin_chunks
+        return origin_chunks
+
+
+if __name__ == "__main__":
+    file_path = "/Users/chenhao/Downloads/汽车手册V16.txt"
+
+    chunks = parse_file(file_path, do_cut=True, separator="==")
+    print(f"{len(chunks)=}")
+    for chunk in chunks[:4]:
+        print(chunk)
+        # print(chunk.content)
```

### Comparing `xagent-0.0.5/xagents/loader/common.py` & `xagent-0.0.6/xagents/loader/common.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/xagents/loader/markdown.py` & `xagent-0.0.6/xagents/loader/markdown.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/xagents/loader/pdf.py` & `xagent-0.0.6/xagents/loader/pdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,48 +11,64 @@
 from xagents.config import *
 from xagents.loader.common import Chunk, ContentType, AbstractLoader
 from loguru import logger
 
 
 
 class PDFLoader(AbstractLoader):
-    def __init__(self, max_page:int=None, extract_images=False):
+    def __init__(self, max_page:int=None, extract_images=False, extract_tables=False, **kwargs):
         """构建pdf加载器
 
         Args:
             max_page (int, optional): 最大页数. Defaults to None：不限定页数
             extract_images (bool, optional): 是否使用ocr抽取其中的图片. Defaults to False.
         """
+        super().__init__(**kwargs)
         self.max_page = max_page
         self.extract_images = extract_images
+        self.extract_tables = extract_tables
 
     def load(self, file_path: str) -> Iterable[Chunk]:
         from langchain_community.document_loaders.pdf import PyMuPDFLoader
+        import pdfplumber
+
         logger.info(f"loading pdf file {file_path}")
         loader = PyMuPDFLoader(file_path, extract_images=self.extract_images)
         pages = loader.lazy_load()
+        table_loader = pdfplumber.open(file_path)
         idx = 0
         for page in pages:
-            idx +=1 
+            tpage = table_loader.pages[idx]
+            idx +=1
             if self.max_page and idx > self.max_page:
                 break
             chunk = Chunk(content=page.page_content, page_idx=idx, content_type=ContentType.TEXT)
             yield chunk
 
+            if self.extract_tables:
+                tables = tpage.extract_tables()
+                for table in tables:
+                    table_content = ""
+                    for row in table:
+                        table_content += "|".join(["null" if col is None else col.replace("\n", "\\n") for col in row]) + "\n"
+                    chunk = Chunk(content=table_content, page_idx=idx, content_type=ContentType.TABLE)
+                    yield chunk
+
 
 if __name__ == "__main__":
     from xagents.config import XAGENT_HOME
     import sys
     logger.add(sys.stdout)
-    loader = PDFLoader(max_page=5, extract_images=True)
+    loader = PDFLoader(max_page=5, extract_images=True, extract_tables=True)
     doc_path = os.path.join(XAGENT_HOME, "data/kb_file")
     logger.info(f"parsing all file in {doc_path}")
     print(doc_path)
 
     for doc in os.listdir(doc_path):
         logger.info(f"loading doc {doc}")
         if doc.endswith(".pdf"):
             pages = loader.load(os.path.join(doc_path, doc))
             for page in pages:
                 logger.info(f"*********************page:{page.page_idx}*********************")
+                logger.info(page.content_type)
                 logger.info(page.content)
                 logger.info("\n\n")
```

### Comparing `xagent-0.0.5/xagents/loader/splitter.py` & `xagent-0.0.6/xagents/loader/splitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,16 @@
         self.parse_table = parse_table
         self.separator = separator
         self.max_len = max_len
         self.min_len = min_len
 
     def _parse_text(self, text: str) -> str:
         text = text.strip()
-        text = re.sub("\s+", " ", text)
-        text = re.sub(f"\.{3,}", "", text)
+        # text = re.sub("\s+", " ", text)
+        # text = re.sub(f"\.{3,}", "", text)
         text = text.strip()
         return text
 
     def split(self, text: str) -> List[str]:
         # logger.info(f"{text=}")
         # logger.info(f"{self.separator=}")
```

### Comparing `xagent-0.0.5/xagents/loader/structed.py` & `xagent-0.0.6/xagents/loader/structed.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from snippets import read2list
 
 
 class StructedLoader(AbstractLoader):
 
     def __init__(self, content_key="content",
                  search_content_key="search_content",
-                 page_idx_key="page", content_type_key="chunk_type") -> None:
+                 page_idx_key="page", content_type_key="chunk_type", **kwargs) -> None:
+        super().__init__(**kwargs)
         self.content_key = content_key
         self.page_idx_key = page_idx_key
         self.content_type_key = content_type_key
         self.search_content_key = search_content_key
 
     @classmethod
     def list_kwargs(cls) -> dict:
```

### Comparing `xagent-0.0.5/xagents/model/api.py` & `xagent-0.0.6/xagents/model/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 @Time    :   2023/12/12 15:50:25
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 import copy
 from typing import List
 from loguru import logger
-from xagents.model.core import LLM, EMBD, Reranker
-from xagents.model.zhipu import ZhipuReranker, ZhipuEmbedding, GLM
-from xagents.model.local import ZhipuLocalEmbedding, LocalLLM
+from xagents.model.common import LLM, EMBD, Reranker
+from xagents.model.zhipu import ZhipuReranker, ZhipuEmbedding, API_GLM
+from xagents.model.local import LocalEmbedding, TGI_GLM
 
 
-_LLM_MODELS = [GLM, LocalLLM]
+_LLM_MODELS = [API_GLM, TGI_GLM]
 _LLM_MODELS_DICT = {model.__name__: model for model in _LLM_MODELS}
 
+## 向前兼容
+_LLM_MODELS_DICT.update(GLM=API_GLM)
 
-_EMBD_MODELS = [ZhipuEmbedding, ZhipuLocalEmbedding]
+
+_EMBD_MODELS = [ZhipuEmbedding, LocalEmbedding]
 _EMBD_MODELS_DICT = {model.__name__: model for model in _EMBD_MODELS}
 
 _RERANK_MODELS = [ZhipuReranker]
 _RERANK_MODELS_DICT = {model.__name__: model for model in _RERANK_MODELS}
 
 
 def list_llm_models() -> List[str]:
@@ -68,18 +71,18 @@
 
 
 if __name__ == "__main__":
     # config = dict(model_cls="GLM", name="glm", version="chatglm_turbo")
     # model = get_llm_model(config)
     # resp = model.generate(prompt="你好", stream=False)
     # print(resp)
-    # rerank_config = dict(model_cls="ZhipuReranker", url="http://36.103.177.140:8000/get_rel_score")
+    # rerank_config = dict(model_cls="ZhipuReranker", url="http://hz-model.bigmodel.cn/reranker/get_rel_score")
     # rerank_model = get_rerank_model(rerank_config)
     # score = rerank_model.cal_similarity("你好","你滚")
     # print(score)
     embedding_model_list = list_embd_models()
     print(embedding_model_list)
-    embedding_model_config = dict(cls='LocalEmbedding')
+    embedding_model_config = dict(cls='ZhipuLocalEmbedding')
     cur_embedding_model = get_embd_model(embedding_model_config)
     print(cur_embedding_model)
```

### Comparing `xagent-0.0.5/xagents/model/core.py` & `xagent-0.0.6/xagents/model/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,38 +4,53 @@
 @Time    :   2023/12/07 17:45:15
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 
 from abc import abstractmethod
-from typing import Generator, Tuple, Union
+from typing import Generator, Optional, Union
+
+from agit.llm import LLMResp
+from agit.common import ToolCall
 
 from langchain_core.embeddings import Embeddings
+from pydantic import BaseModel, Field
+
+
 
-from xagents.tool.core import ToolCall
 
 StrOrGen = Union[str, Generator]
 
+class LLMGenConfig(BaseModel):
+    system:Optional[str] = Field(description="系统信息", default=None)
+    temperature: float = Field(default=0.95, ge=0, le=1, description="生成文本的温度")
+    top_p: float = Field(default=0.7, ge=0, le=1, description="生成文本的top_p")
+
+class LLMGen(BaseModel):
+    content: StrOrGen = Field(description="生成的文本内容, 字符串或生成器")
+    tool_call: Optional[ToolCall] = Field(description="工具调用")
+    detail: dict = Field()
+    
 
 class LLM:
     """语言模型的基类
     """
-    def __init__(self, name: str, version: str):
+    def __init__(self, version: str, name: str=None):
         """初始化函数
 
         Args:
             name (str): LLM的名称
             version (str): 模型版本
         """
-        self.name = name
+        self.name = name if name else self.__class__.__name__ +"-" + version
         self.version = version
 
     @abstractmethod
-    def generate(self, prompt:str, history=[], system:str=None, stream=True, **kwargs)->Tuple[ToolCall,StrOrGen]:
+    def generate(self, prompt:str, history=[], system:str=None, stream=True, **kwargs)->LLMResp:
         """生成结果
 
         Args:
             prompt (str): 给LLM的提示词
             history (list, optional): 历史message列表. Defaults to [].
             system (_type_, optional): system信息. Defaults to None.
             stream (bool, optional): 是否返回generator. Defaults to True.
@@ -43,14 +58,20 @@
             Tuple[ToolCall,StrOrGen]: ToolCall:工具调用实例，可以为空, StrOrGen:模型回复内容，字符串或generator
         """
         raise NotImplementedError
 
     @classmethod
     def list_version(cls):
         raise NotImplementedError
+    
+    def __str__(self):
+        return f"[{self.name}]-{self.version}"
+
+    def __repr__(self):
+        return self.__str__()
 
 
 class EMBD(Embeddings):
     @classmethod
     def get_dim(cls) -> int:
         raise NotImplementedError
```

### Comparing `xagent-0.0.5/xagents/model/openai.py` & `xagent-0.0.6/xagents/model/openai.py`

 * *Files identical despite different names*

### Comparing `xagent-0.0.5/xagents/tool/api.py` & `xagent-0.0.6/xagents/tool/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 @Time    :   2024/01/04 18:26:54
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
 from typing import Any, List
 
-from xagents.tool.common_tool import calculator
+from xagents.tool.common_tool import calculator, travel_searcher
 from xagents.tool.core import BaseTool, ToolCall
+from loguru import logger
 
 
-_ALL_TOOLS = [calculator]
+_ALL_TOOLS = [calculator, travel_searcher]
 _TOOL_MAP = {e.name:e for e in _ALL_TOOLS}
 
 
 def invoke_tool_call(tool_call:ToolCall)->Any:
     tool = get_tool(tool_call.name)
     resp = tool.execute(**tool_call.parameters)
     tool_call.resp = resp
@@ -28,12 +29,24 @@
         raise ValueError(f"Unknown tool: {tool_name}")
     tool:BaseTool = _TOOL_MAP[tool_name]
     return tool
     
 def list_tools() -> List[BaseTool]:
     return _ALL_TOOLS
     
+def get_tools(tools_config:List[dict]) -> List[BaseTool]:
+    tools = []
+    for config in tools_config:
+        try:
+            tool_name = config.get("name")
+            tool = get_tool(tool_name)
+            tools.append(tool)   
+        except Exception as e:
+            logger.warning(f"Failed to load tool: {tool_name}")
+    return tools
+
+
 if __name__ == "__main__":
     tool_call = ToolCall(name="calculator", parameters={"expression": "1+1"})
     resp = invoke_tool_call(tool_call)
     print(resp)
```

### Comparing `xagent-0.0.5/xagents/tool/common_tool.py` & `xagent-0.0.6/xagents/tool/common_tool.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,31 +2,37 @@
 # -*- encoding: utf-8 -*-
 '''
 @Time    :   2024/01/04 14:04:02
 @Author  :   ChenHao
 @Contact :   jerrychen1990@gmail.com
 '''
 
-from xagents.tool.core import BaseTool, Parameter
+from xagents.tool.core import BaseTool
+from agit.common import Parameter
 
-    
-def exec_python(expression:str)->dict:
+
+def exec_python(expression: str) -> dict:
     try:
         rs = eval(expression)
     except Exception as e:
         rs = "执行失败"
     return dict(result=rs)
-    
-    
+
+
+def mock_travel_search(departure: str, destination: str, date: str):
+    return dict(result="查询成功，有如下车次:A00001, A00002, A00003")
+
+
 calculator = BaseTool(name="计算器", description="根据提供的数学表达式，用python解释器来执行，得到计算结果,计算结果以json格式来返回,json包含一个字段，名字为result",
                       parameters=[Parameter(name="expression", type="string", description="数学表达式，可以通过python来执行的", required=True)],
                       callable=exec_python)
-            
-            
+
+travel_searcher = BaseTool(name="车次查询", description="根据用户提供的信息，查询对应的车次",
+                           parameters=[Parameter(name="departure", description="出发城市或车站", type="string", required=True),
+                                       Parameter(name="destination", description="目的地城市或车站", type="string", required=True),
+                                       Parameter(name="date", description="要查询的车次日期", type="string", required=True)],
+                           callable=mock_travel_search)
+
+
 if __name__ == "__main__":
     rs = calculator.execute("(351345-54351)/54351")
     print(rs)
-    
-    
-    
-    
-
```

### Comparing `xagent-0.0.5/xagents/util.py` & `xagent-0.0.6/xagents/util.py`

 * *Files identical despite different names*

