# Comparing `tmp/Agently-3.2.2.5.tar.gz` & `tmp/Agently-3.3.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.2.5.tar", last modified: Mon Apr 15 12:27:39 2024, max compression
+gzip compressed data, was "Agently-3.3.0.0a6.tar", last modified: Sat Apr 13 09:29:57 2024, max compression
```

## Comparing `Agently-3.2.2.5.tar` & `Agently-3.3.0.0a6.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.387664 Agently-3.2.2.5/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.359880 Agently-3.2.2.5/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.361022 Agently-3.2.2.5/Agently/Agent/
--rw-r--r--   0 moxin      (501) staff       (20)    14416 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Agent/Agent.py
--rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Agent/AgentFactory.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.361455 Agently-3.2.2.5/Agently/Facility/
--rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Facility/FacilityManager.py
--rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.361937 Agently-3.2.2.5/Agently/Request/
--rw-r--r--   0 moxin      (501) staff       (20)     9943 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Request/Request.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.362367 Agently-3.2.2.5/Agently/WebSocket/
--rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/WebSocket/WebSocket.py
--rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.363678 Agently-3.2.2.5/Agently/Workflow/
--rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/Chunk.py
--rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/MainExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/Schema.py
--rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/Workflow.py
--rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.364235 Agently-3.2.2.5/Agently/Workflow/executors/
--rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/executors/StartExecutor.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/executors/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.366002 Agently-3.2.2.5/Agently/Workflow/lib/
--rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/BreakingHub.py
--rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/ChunkExecutorManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/Store.py
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/constants.py
--rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.368028 Agently-3.2.2.5/Agently/Workflow/utils/
--rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/utils/exec_tree.py
--rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/utils/find.py
--rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/utils/logger.py
--rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/utils/runtime_supports.py
--rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/utils/verify.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.368405 Agently-3.2.2.5/Agently/Workflow/yamlflow/
--rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/yamlflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.370144 Agently-3.2.2.5/Agently/Workflow/yamlflow/preset_chunks/
--rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/yamlflow/preset_chunks/Print.py
--rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/yamlflow/preset_chunks/Start.py
--rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
--rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/yamlflow/preset_chunks/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/Workflow/yamlflow/yamlflow.py
--rw-r--r--   0 moxin      (501) staff       (20)      569 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/_global.py
--rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.370285 Agently-3.2.2.5/Agently/plugins/
--rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.374627 Agently-3.2.2.5/Agently/plugins/agent_component/
--rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Decorator.py
--rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/EventListener.py
--rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/ReplyReformer.py
--rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Role.py
--rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Search.py
--rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Segment.py
--rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Session.py
--rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Status.py
--rw-r--r--   0 moxin      (501) staff       (20)     8963 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/Tool.py
--rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     3308 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/YAMLLoader.py
--rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.374979 Agently-3.2.2.5/Agently/plugins/agent_component/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.376167 Agently-3.2.2.5/Agently/plugins/facility/
--rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/Embedding.py
--rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/RoleManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/StatusManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.376697 Agently-3.2.2.5/Agently/plugins/facility/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/utils/FacilityABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.379361 Agently-3.2.2.5/Agently/plugins/request/
--rw-r--r--   0 moxin      (501) staff       (20)    11956 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/AzureOpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/Claude.py
--rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/ERNIE.py
--rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/Google.py
--rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/Kimi.py
--rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/MiniMax.py
--rw-r--r--   0 moxin      (501) staff       (20)    13093 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/OAIClient.py
--rw-r--r--   0 moxin      (501) staff       (20)    11670 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/OpenAI.py
--rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/ZhipuAI.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.380886 Agently-3.2.2.5/Agently/plugins/request/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/utils/RequestABC.py
--rw-r--r--   0 moxin      (501) staff       (20)      162 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/utils/format.py
--rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.381636 Agently-3.2.2.5/Agently/plugins/storage/
--rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/storage/FileStorage.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/storage/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.383070 Agently-3.2.2.5/Agently/plugins/storage/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/storage/utils/StorageABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.383784 Agently-3.2.2.5/Agently/plugins/tool/
--rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/tool/Code.py
--rw-r--r--   0 moxin      (501) staff       (20)     5915 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/tool/Web.py
--rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/tool/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.384299 Agently-3.2.2.5/Agently/plugins/tool/utils/
--rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/tool/utils/ToolABC.py
--rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/plugins/tool/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)      211 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.386987 Agently-3.2.2.5/Agently/utils/
--rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/AliasManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/DataOps.py
--rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/IdGenerator.py
--rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/PluginManager.py
--rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/RuntimeCtx.py
--rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/StorageDelegate.py
--rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/ToolManager.py
--rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/__init__.py
--rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/check_version.py
--rw-r--r--   0 moxin      (501) staff       (20)     2868 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/load_json.py
--rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-15 12:20:14.000000 Agently-3.2.2.5/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-15 12:27:39.387244 Agently-3.2.2.5/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      876 2024-04-15 12:27:39.000000 Agently-3.2.2.5/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-04-15 12:27:39.000000 Agently-3.2.2.5/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-15 12:27:39.000000 Agently-3.2.2.5/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      143 2024-04-15 12:27:39.000000 Agently-3.2.2.5/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-15 12:27:39.000000 Agently-3.2.2.5/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      876 2024-04-15 12:27:39.387476 Agently-3.2.2.5/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-15 12:27:39.387700 Agently-3.2.2.5/setup.cfg
--rw-------   0 moxin      (501) staff       (20)     1006 2024-04-15 12:27:35.000000 Agently-3.2.2.5/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.608206 Agently-3.3.0.0a6/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.541693 Agently-3.3.0.0a6/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.542864 Agently-3.3.0.0a6/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14256 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.543395 Agently-3.3.0.0a6/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.544841 Agently-3.3.0.0a6/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)     9783 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.545208 Agently-3.3.0.0a6/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.546520 Agently-3.3.0.0a6/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3165 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.547062 Agently-3.3.0.0a6/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.549071 Agently-3.3.0.0a6/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      483 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.551755 Agently-3.3.0.0a6/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.552207 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.553832 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      569 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.554032 Agently-3.3.0.0a6/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.577741 Agently-3.3.0.0a6/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2870 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1384 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8287 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8963 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3308 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/YAMLLoader.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.578150 Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.579956 Agently-3.3.0.0a6/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.580856 Agently-3.3.0.0a6/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.584323 Agently-3.3.0.0a6/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)    11956 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/AzureOpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10303 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7372 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    13093 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11670 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.584880 Agently-3.3.0.0a6/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      162 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/format.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4330 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.600946 Agently-3.3.0.0a6/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.601511 Agently-3.3.0.0a6/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.602583 Agently-3.3.0.0a6/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5915 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.602962 Agently-3.3.0.0a6/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-04-13 09:28:26.000000 Agently-3.3.0.0a6/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.607517 Agently-3.3.0.0a6/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2773 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-04-12 15:13:29.000000 Agently-3.3.0.0a6/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-04-13 09:29:57.607753 Agently-3.3.0.0a6/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      913 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      163 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-04-13 09:29:57.000000 Agently-3.3.0.0a6/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      913 2024-04-13 09:29:57.608008 Agently-3.3.0.0a6/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-04-13 09:29:57.608244 Agently-3.3.0.0a6/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)     1014 2024-04-13 09:24:41.000000 Agently-3.3.0.0a6/setup.py
```

### Comparing `Agently-3.2.2.5/Agently/Agent/Agent.py` & `Agently-3.3.0.0a6/Agently/Agent/Agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,24 +203,21 @@
                     await handle_response(response)
             else:
                 for response in event_generator:
                     await handle_response(response)
 
             # Load JSON and fix if Required
             if self.request.response_cache["type"] == "JSON":
-                reply = await load_json(
+                self.request.response_cache["reply"] = await load_json(
                     self.request.response_cache["reply"],
                     self.request.response_cache["prompt"]["input"],
                     self.request.response_cache["prompt"]["output"],
                     self.request,
                     is_debug = is_debug,
                 )
-                if isinstance(reply, str) and reply.startswith("$$$JSON_ERROR:"):
-                    raise Exception(reply[14:])
-                self.request.response_cache["reply"] = reply
 
             await handle_response({ "event": "response:finally", "data": self.request.response_cache })
 
             self.request_runtime_ctx.empty()
             return self.request.response_cache["reply"]
         except Exception as e:
             self.request_runtime_ctx.empty()
```

### Comparing `Agently-3.2.2.5/Agently/Agent/AgentFactory.py` & `Agently-3.3.0.0a6/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Facility/FacilityManager.py` & `Agently-3.3.0.0a6/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Request/Request.py` & `Agently-3.3.0.0a6/Agently/Request/Request.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,24 +145,21 @@
                 async for response in event_generator:
                     handle_response(response)
             else:
                 for response in event_generator:
                     handle_response(response)
                 
             if self.response_cache["type"] == "JSON":
-                reply = await load_json(
+                self.response_cache["reply"] = await load_json(
                     self.response_cache["reply"],
                     self.response_cache["prompt"]["input"],
                     self.response_cache["prompt"]["output"],
                     self,
                     is_debug = is_debug,
                 )
-                if isinstance(reply, str) and reply.startswith("$$$JSON_ERROR:"):
-                    raise Exception(reply[14:])
-                self.response_cache["reply"] = reply
             return self.response_cache["reply"]
         except Exception as e:
             self.request_runtime_ctx.empty()
             raise(e)
 
     def get_result(self, request_type: str=None):
         reply_queue = queue.Queue()
```

### Comparing `Agently-3.2.2.5/Agently/WebSocket/WebSocket.py` & `Agently-3.3.0.0a6/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/Chunk.py` & `Agently-3.3.0.0a6/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/MainExecutor.py` & `Agently-3.3.0.0a6/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/Schema.py` & `Agently-3.3.0.0a6/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/Workflow.py` & `Agently-3.3.0.0a6/Agently/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/lib/constants.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/lib/painter.py` & `Agently-3.3.0.0a6/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/utils/exec_tree.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/utils/find.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/utils/logger.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.3.0.0a6/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/yamlflow/preset_chunks/__init__.py` & `Agently-3.3.0.0a6/Agently/Workflow/yamlflow/preset_chunks/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/Workflow/yamlflow/yamlflow.py` & `Agently-3.3.0.0a6/Agently/Workflow/yamlflow/yamlflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/__init__.py` & `Agently-3.3.0.0a6/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/_global.py` & `Agently-3.3.0.0a6/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Decorator.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/EventListener.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Role.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Search.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Segment.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Session.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Status.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/Tool.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/YAMLLoader.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/YAMLLoader.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.3.0.0a6/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/facility/Embedding.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/facility/RoleManager.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/facility/StatusManager.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/facility/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/AzureOpenAI.py` & `Agently-3.3.0.0a6/Agently/plugins/request/AzureOpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/Claude.py` & `Agently-3.3.0.0a6/Agently/plugins/request/Claude.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/ERNIE.py` & `Agently-3.3.0.0a6/Agently/plugins/request/ERNIE.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/Google.py` & `Agently-3.3.0.0a6/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/Kimi.py` & `Agently-3.3.0.0a6/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/MiniMax.py` & `Agently-3.3.0.0a6/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/OAIClient.py` & `Agently-3.3.0.0a6/Agently/plugins/request/OAIClient.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/OpenAI.py` & `Agently-3.3.0.0a6/Agently/plugins/request/OpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/ZhipuAI.py` & `Agently-3.3.0.0a6/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.3.0.0a6/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/utils/format.py` & `Agently-3.3.0.0a6/Agently/plugins/request/utils/format.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/request/utils/transform.py` & `Agently-3.3.0.0a6/Agently/plugins/request/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/storage/FileStorage.py` & `Agently-3.3.0.0a6/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/storage/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.3.0.0a6/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/tool/Code.py` & `Agently-3.3.0.0a6/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/tool/Web.py` & `Agently-3.3.0.0a6/Agently/plugins/tool/Web.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/plugins/tool/__init__.py` & `Agently-3.3.0.0a6/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/AliasManager.py` & `Agently-3.3.0.0a6/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/DataOps.py` & `Agently-3.3.0.0a6/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/PluginManager.py` & `Agently-3.3.0.0a6/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/RuntimeCtx.py` & `Agently-3.3.0.0a6/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/StorageDelegate.py` & `Agently-3.3.0.0a6/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/ToolManager.py` & `Agently-3.3.0.0a6/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/check_version.py` & `Agently-3.3.0.0a6/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently/utils/load_json.py` & `Agently-3.3.0.0a6/Agently/utils/load_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,14 @@
     else:
         return errors
 
 async def fix_json(origin: str, input_dict: any, output_dict: any, request: object, *, is_debug: bool=False, errors = list):
     try:
         fixed_result = await request\
             .input({
-                "input": input_dict,
-                "expect JSON String format": output_dict,
                 "error JSON String": origin ,
                 "error info": errors,
             })\
             .output('FIXED {error JSON String} JSON STRING ONLY WITHOUT EXPLANATION that can be parsed by Python')\
             .start_async()
         json_string = find_json(fixed_result)
         if is_debug:
@@ -42,15 +40,15 @@
             print("\n--------------------------\n")
         fixed_result = json5.loads(json_string)
         if is_debug:
             print("[Parse JSON to Dict] Done")
             print("\n--------------------------\n")
         return fixed_result
     except Exception as e:
-        return f"$$$JSON_ERROR:[Agent Request] Error still occured when try to fix JSON decode error: { str(e) }\nOrigin JSON String:\n{ origin }" 
+        raise Exception(f"[Agent Request] Error still occured when try to fix JSON decode error: { str(e) }\nOrigin JSON String:\n{ json_string }")
 
 async def load_json(origin: str, input_dict: any, output_dict: any, request: object, *, is_debug: bool=False):
     try:
         json_string = find_json(origin)
         if is_debug:
             print("[Cleaned JSON String]:\n", json_string)
             print("\n--------------------------\n")
```

### Comparing `Agently-3.2.2.5/Agently/utils/transform.py` & `Agently-3.3.0.0a6/Agently/utils/transform.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/Agently.egg-info/PKG-INFO` & `Agently-3.3.0.0a6/Agently.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.5
+Version: 3.3.0.0a6
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
+Requires-Dist: AgentlyCmd==0.0.0.2
 Requires-Dist: nest_asyncio
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: tornado
 Requires-Dist: openai
 Requires-Dist: erniebot
```

### Comparing `Agently-3.2.2.5/Agently.egg-info/SOURCES.txt` & `Agently-3.3.0.0a6/Agently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.5/PKG-INFO` & `Agently-3.3.0.0a6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.5
+Version: 3.3.0.0a6
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
+Requires-Dist: AgentlyCmd==0.0.0.2
 Requires-Dist: nest_asyncio
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: tornado
 Requires-Dist: openai
 Requires-Dist: erniebot
```

### Comparing `Agently-3.2.2.5/setup.py` & `Agently-3.3.0.0a6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
 
 setuptools.setup(
     name = "Agently",
-    version = "3.2.2.5",
+    version = "3.3.0.0-alpha-6",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
     #packages = ["Agently"],
```

