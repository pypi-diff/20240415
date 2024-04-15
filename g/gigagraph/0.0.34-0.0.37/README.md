# Comparing `tmp/gigagraph-0.0.34.tar.gz` & `tmp/gigagraph-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigagraph-0.0.34.tar", max compression
+gzip compressed data, was "gigagraph-0.0.37.tar", max compression
```

## Comparing `gigagraph-0.0.34.tar` & `gigagraph-0.0.37.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0     1067 2024-02-09 11:26:26.015908 gigagraph-0.0.34/LICENSE
--rw-r--r--   0        0        0    51426 2024-04-11 10:30:48.721273 gigagraph-0.0.34/README.md
--rw-r--r--   0        0        0       69 2024-03-06 08:45:49.220137 gigagraph-0.0.34/langgraph/__init__.py
--rw-r--r--   0        0        0      294 2024-02-09 11:26:26.068963 gigagraph-0.0.34/langgraph/channels/__init__.py
--rw-r--r--   0        0        0     1682 2024-04-11 10:29:15.660408 gigagraph-0.0.34/langgraph/channels/any_value.py
--rw-r--r--   0        0        0     4254 2024-04-11 10:29:15.660791 gigagraph-0.0.34/langgraph/channels/base.py
--rw-r--r--   0        0        0     2028 2024-04-11 10:29:15.661181 gigagraph-0.0.34/langgraph/channels/binop.py
--rw-r--r--   0        0        0     3180 2024-04-11 10:29:15.661495 gigagraph-0.0.34/langgraph/channels/context.py
--rw-r--r--   0        0        0     1917 2024-04-11 10:29:15.661804 gigagraph-0.0.34/langgraph/channels/ephemeral_value.py
--rw-r--r--   0        0        0     1706 2024-04-11 10:29:15.662068 gigagraph-0.0.34/langgraph/channels/last_value.py
--rw-r--r--   0        0        0     1715 2024-04-11 10:29:15.662340 gigagraph-0.0.34/langgraph/channels/named_barrier_value.py
--rw-r--r--   0        0        0     2584 2024-04-11 10:29:15.663095 gigagraph-0.0.34/langgraph/channels/topic.py
--rw-r--r--   0        0        0      235 2024-02-09 11:26:26.072245 gigagraph-0.0.34/langgraph/checkpoint/__init__.py
--rw-r--r--   0        0        0     5101 2024-04-11 10:29:15.663498 gigagraph-0.0.34/langgraph/checkpoint/aiosqlite.py
--rw-r--r--   0        0        0     4286 2024-04-11 10:31:54.484801 gigagraph-0.0.34/langgraph/checkpoint/base.py
--rw-r--r--   0        0        0     1816 2024-04-11 10:29:15.663924 gigagraph-0.0.34/langgraph/checkpoint/memory.py
--rw-r--r--   0        0        0     5853 2024-04-11 10:29:15.664301 gigagraph-0.0.34/langgraph/checkpoint/sqlite.py
--rw-r--r--   0        0        0      130 2024-04-11 10:29:15.664581 gigagraph-0.0.34/langgraph/constants.py
--rw-r--r--   0        0        0      197 2024-02-09 11:26:26.074907 gigagraph-0.0.34/langgraph/graph/__init__.py
--rw-r--r--   0        0        0    13169 2024-04-11 10:29:15.665930 gigagraph-0.0.34/langgraph/graph/graph.py
--rw-r--r--   0        0        0     1429 2024-04-11 10:29:15.666282 gigagraph-0.0.34/langgraph/graph/message.py
--rw-r--r--   0        0        0    10606 2024-04-11 10:29:15.666834 gigagraph-0.0.34/langgraph/graph/state.py
--rw-r--r--   0        0        0      306 2024-02-09 11:26:26.077283 gigagraph-0.0.34/langgraph/prebuilt/__init__.py
--rw-r--r--   0        0        0     5464 2024-04-11 10:29:15.667324 gigagraph-0.0.34/langgraph/prebuilt/agent_executor.py
--rw-r--r--   0        0        0    10662 2024-03-06 08:45:49.224367 gigagraph-0.0.34/langgraph/prebuilt/chat_agent_executor.py
--rw-r--r--   0        0        0     2232 2024-04-11 10:29:15.667616 gigagraph-0.0.34/langgraph/prebuilt/tool_executor.py
--rw-r--r--   0        0        0    46963 2024-04-11 10:29:15.668709 gigagraph-0.0.34/langgraph/pregel/__init__.py
--rw-r--r--   0        0        0     1240 2024-04-11 10:29:15.669066 gigagraph-0.0.34/langgraph/pregel/debug.py
--rw-r--r--   0        0        0     3344 2024-04-11 10:29:15.669359 gigagraph-0.0.34/langgraph/pregel/io.py
--rw-r--r--   0        0        0       53 2024-02-09 11:26:26.080872 gigagraph-0.0.34/langgraph/pregel/log.py
--rw-r--r--   0        0        0     7750 2024-04-11 10:29:15.669754 gigagraph-0.0.34/langgraph/pregel/read.py
--rw-r--r--   0        0        0      752 2024-04-11 10:29:15.669958 gigagraph-0.0.34/langgraph/pregel/types.py
--rw-r--r--   0        0        0     3057 2024-04-11 10:29:15.670248 gigagraph-0.0.34/langgraph/pregel/validate.py
--rw-r--r--   0        0        0     3867 2024-04-11 10:29:15.670561 gigagraph-0.0.34/langgraph/pregel/write.py
--rw-r--r--   0        0        0        0 2024-03-12 15:00:07.691355 gigagraph-0.0.34/langgraph/py.typed
--rw-r--r--   0        0        0     2282 2024-04-11 10:29:15.670837 gigagraph-0.0.34/langgraph/utils.py
--rw-r--r--   0        0        0      308 2024-03-06 08:45:49.226704 gigagraph-0.0.34/langgraph/version.py
--rw-r--r--   0        0        0     2237 2024-04-11 10:34:41.186243 gigagraph-0.0.34/pyproject.toml
--rw-r--r--   0        0        0    52050 1970-01-01 00:00:00.000000 gigagraph-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-02-09 11:26:26.015908 gigagraph-0.0.37/LICENSE
+-rw-r--r--   0        0        0    51559 2024-04-15 10:02:14.913807 gigagraph-0.0.37/README.md
+-rw-r--r--   0        0        0       69 2024-03-06 08:45:49.220137 gigagraph-0.0.37/langgraph/__init__.py
+-rw-r--r--   0        0        0      294 2024-02-09 11:26:26.068963 gigagraph-0.0.37/langgraph/channels/__init__.py
+-rw-r--r--   0        0        0     1682 2024-04-15 10:02:15.008130 gigagraph-0.0.37/langgraph/channels/any_value.py
+-rw-r--r--   0        0        0     4254 2024-04-15 10:02:15.008653 gigagraph-0.0.37/langgraph/channels/base.py
+-rw-r--r--   0        0        0     2028 2024-04-15 10:02:15.009503 gigagraph-0.0.37/langgraph/channels/binop.py
+-rw-r--r--   0        0        0     3180 2024-04-15 10:02:15.010265 gigagraph-0.0.37/langgraph/channels/context.py
+-rw-r--r--   0        0        0     1917 2024-04-15 10:02:15.010661 gigagraph-0.0.37/langgraph/channels/ephemeral_value.py
+-rw-r--r--   0        0        0     1706 2024-04-15 10:02:15.011057 gigagraph-0.0.37/langgraph/channels/last_value.py
+-rw-r--r--   0        0        0     1715 2024-04-15 10:02:15.011411 gigagraph-0.0.37/langgraph/channels/named_barrier_value.py
+-rw-r--r--   0        0        0     2584 2024-04-15 10:02:15.011871 gigagraph-0.0.37/langgraph/channels/topic.py
+-rw-r--r--   0        0        0      302 2024-04-15 10:02:15.013003 gigagraph-0.0.37/langgraph/checkpoint/__init__.py
+-rw-r--r--   0        0        0     5336 2024-04-15 10:02:15.014124 gigagraph-0.0.37/langgraph/checkpoint/aiosqlite.py
+-rw-r--r--   0        0        0     4187 2024-04-15 10:02:15.015222 gigagraph-0.0.37/langgraph/checkpoint/base.py
+-rw-r--r--   0        0        0     2958 2024-04-15 10:02:15.016282 gigagraph-0.0.37/langgraph/checkpoint/memory.py
+-rw-r--r--   0        0        0     5570 2024-04-15 10:02:15.017297 gigagraph-0.0.37/langgraph/checkpoint/sqlite.py
+-rw-r--r--   0        0        0      130 2024-04-15 10:02:15.018515 gigagraph-0.0.37/langgraph/constants.py
+-rw-r--r--   0        0        0      197 2024-02-09 11:26:26.074907 gigagraph-0.0.37/langgraph/graph/__init__.py
+-rw-r--r--   0        0        0    13150 2024-04-15 10:02:15.019737 gigagraph-0.0.37/langgraph/graph/graph.py
+-rw-r--r--   0        0        0     1429 2024-04-15 10:02:15.020907 gigagraph-0.0.37/langgraph/graph/message.py
+-rw-r--r--   0        0        0    10606 2024-04-15 10:02:15.021710 gigagraph-0.0.37/langgraph/graph/state.py
+-rw-r--r--   0        0        0      372 2024-04-15 10:02:15.022782 gigagraph-0.0.37/langgraph/prebuilt/__init__.py
+-rw-r--r--   0        0        0     5464 2024-04-15 10:02:15.023557 gigagraph-0.0.37/langgraph/prebuilt/agent_executor.py
+-rw-r--r--   0        0        0     8356 2024-04-15 10:02:15.024860 gigagraph-0.0.37/langgraph/prebuilt/chat_agent_executor.py
+-rw-r--r--   0        0        0     2232 2024-04-15 10:02:15.025852 gigagraph-0.0.37/langgraph/prebuilt/tool_executor.py
+-rw-r--r--   0        0        0     3320 2024-04-15 10:02:15.026606 gigagraph-0.0.37/langgraph/prebuilt/tool_node.py
+-rw-r--r--   0        0        0    46579 2024-04-15 10:02:15.028119 gigagraph-0.0.37/langgraph/pregel/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-15 10:02:15.028845 gigagraph-0.0.37/langgraph/pregel/debug.py
+-rw-r--r--   0        0        0     3305 2024-04-15 10:02:15.030157 gigagraph-0.0.37/langgraph/pregel/io.py
+-rw-r--r--   0        0        0       53 2024-02-09 11:26:26.080872 gigagraph-0.0.37/langgraph/pregel/log.py
+-rw-r--r--   0        0        0     7750 2024-04-15 10:02:15.031108 gigagraph-0.0.37/langgraph/pregel/read.py
+-rw-r--r--   0        0        0      752 2024-04-15 10:02:15.031470 gigagraph-0.0.37/langgraph/pregel/types.py
+-rw-r--r--   0        0        0     3057 2024-04-15 10:02:15.032091 gigagraph-0.0.37/langgraph/pregel/validate.py
+-rw-r--r--   0        0        0     3867 2024-04-15 10:02:15.032754 gigagraph-0.0.37/langgraph/pregel/write.py
+-rw-r--r--   0        0        0        0 2024-04-15 10:02:15.032946 gigagraph-0.0.37/langgraph/py.typed
+-rw-r--r--   0        0        0     2282 2024-04-15 10:02:15.033610 gigagraph-0.0.37/langgraph/utils.py
+-rw-r--r--   0        0        0      308 2024-03-06 08:45:49.226704 gigagraph-0.0.37/langgraph/version.py
+-rw-r--r--   0        0        0     2240 2024-04-15 10:02:15.034893 gigagraph-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0    52186 1970-01-01 00:00:00.000000 gigagraph-0.0.37/PKG-INFO
```

### Comparing `gigagraph-0.0.34/LICENSE` & `gigagraph-0.0.37/LICENSE`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/README.md` & `gigagraph-0.0.37/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: gigagraph
+Version: 0.0.37
+Summary: langgraph
+Home-page: https://github.com/ai-forever/gigagraph
+License: MIT
+Requires-Python: >=3.9.0,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gigachain-core (>=0.1.42rc1,<0.2.0)
+Project-URL: Repository, https://github.com/ai-forever/gigagraph
+Description-Content-Type: text/markdown
+
 # GigaGraph
 
 ⚡ Разработка языковых агентов в виде графов ⚡
 
 ## Описание
 
 GigaGraph — это библиотека, дающая возможность работать с LLM (большие языковые модели) для создания приложений, которые используют множество взаимодействующих цепочек (акторов) и сохраняют данные о состоянии.
@@ -498,15 +515,16 @@
 
 ### Reflection / Self-Critique
 
 When output quality is a major concern, it's common to incorporate some combination of self-critique or reflection and external validation to refine your system's outputs. The following examples demonstrate research that implement this type of design.
 
 - [Basic Reflection](./examples/reflection/reflection.ipynb): add a simple "reflect" step in your graph to prompt your system to revise its outputs.
 - [Reflexion](./examples/reflexion/reflexion.ipynb): critique missing and superflous aspects of the agent's response to guide subsequent steps. Based on [Reflexion](https://arxiv.org/abs/2303.11366), by Shinn, et. al.
-- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406), by Zhou, et. al.
+- [Giga Reflexion](./examples/reflexion_giga/reflexion.ipynb): реализация Reflexion на GigaChat
+- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406/LanguageAgentTreeSearch/), by Zhou, et. al.
 
 ### Multi-agent Examples
 ### Примеры с несколькими агентами
 
 - [Совместная работа нескольких агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/multi-agent-collaboration.ipynb). Пример демонстрирует как создать двух агентов, которые работают вместе для решения задачи.
 - [Несколько агентов с «руководителем»](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/agent_supervisor.ipynb). Пример демонстрирует как организовать работу агентов используя LLM в роли «руководителя», который решает как распределять работу.
 - [Иерархичные команды агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/hierarchical_agent_teams.ipynb): пример демонстрирует как организовать «команды» агентов, которые будут взаимодействовать для решения задачи, в виде вложенных графов.
@@ -839,7 +857,8 @@
 app = create_agent_executor(agent_runnable, tools)
 
 inputs = {"input": "what is the weather in sf", "chat_history": []}
 for s in app.stream(inputs):
     print(list(s.values())[0])
     print("----")
 ```
+
```

### Comparing `gigagraph-0.0.34/langgraph/channels/any_value.py` & `gigagraph-0.0.37/langgraph/channels/any_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/base.py` & `gigagraph-0.0.37/langgraph/channels/base.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/binop.py` & `gigagraph-0.0.37/langgraph/channels/binop.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/context.py` & `gigagraph-0.0.37/langgraph/channels/context.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/ephemeral_value.py` & `gigagraph-0.0.37/langgraph/channels/ephemeral_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/last_value.py` & `gigagraph-0.0.37/langgraph/channels/last_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/named_barrier_value.py` & `gigagraph-0.0.37/langgraph/channels/named_barrier_value.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/channels/topic.py` & `gigagraph-0.0.37/langgraph/channels/topic.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/checkpoint/aiosqlite.py` & `gigagraph-0.0.37/langgraph/checkpoint/aiosqlite.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 import pickle
 from contextlib import AbstractAsyncContextManager
 from types import TracebackType
 from typing import AsyncIterator, Optional
 
 import aiosqlite
-from langchain_core.pydantic_v1 import Field
 from langchain_core.runnables import RunnableConfig
 from typing_extensions import Self
 
-from langgraph.checkpoint.base import BaseCheckpointSaver, Checkpoint, CheckpointTuple
+from langgraph.checkpoint.base import (
+    BaseCheckpointSaver,
+    Checkpoint,
+    CheckpointAt,
+    CheckpointTuple,
+    SerializerProtocol,
+)
 
 
 class AsyncSqliteSaver(BaseCheckpointSaver, AbstractAsyncContextManager):
+    serde = pickle
+
     conn: aiosqlite.Connection
 
-    is_setup: bool = Field(False, init=False, repr=False)
+    is_setup: bool
 
-    class Config:
-        arbitrary_types_allowed = True
+    def __init__(
+        self,
+        conn: aiosqlite.Connection,
+        *,
+        serde: Optional[SerializerProtocol] = None,
+        at: Optional[CheckpointAt] = None,
+    ):
+        super().__init__(serde=serde, at=at)
+        self.conn = conn
+        self.is_setup = False
 
     @classmethod
     def from_conn_string(cls, conn_string: str) -> "AsyncSqliteSaver":
         return AsyncSqliteSaver(conn=aiosqlite.connect(conn_string))
 
     async def __aenter__(self) -> Self:
         return self
@@ -63,15 +78,15 @@
                     config["configurable"]["thread_id"],
                     config["configurable"]["thread_ts"],
                 ),
             ) as cursor:
                 if value := await cursor.fetchone():
                     return CheckpointTuple(
                         config,
-                        pickle.loads(value[0]),
+                        self.serde.loads(value[0]),
                         {
                             "configurable": {
                                 "thread_id": config["configurable"]["thread_id"],
                                 "thread_ts": value[1],
                             }
                         }
                         if value[1]
@@ -86,15 +101,15 @@
                     return CheckpointTuple(
                         {
                             "configurable": {
                                 "thread_id": value[0],
                                 "thread_ts": value[1],
                             }
                         },
-                        pickle.loads(value[3]),
+                        self.serde.loads(value[3]),
                         {
                             "configurable": {
                                 "thread_id": value[0],
                                 "thread_ts": value[2],
                             }
                         }
                         if value[2]
@@ -106,15 +121,15 @@
         async with self.conn.execute(
             "SELECT thread_id, thread_ts, parent_ts, checkpoint FROM checkpoints WHERE thread_id = ? ORDER BY thread_ts DESC",
             (config["configurable"]["thread_id"],),
         ) as cursor:
             async for thread_id, thread_ts, parent_ts, value in cursor:
                 yield CheckpointTuple(
                     {"configurable": {"thread_id": thread_id, "thread_ts": thread_ts}},
-                    pickle.loads(value),
+                    self.serde.loads(value),
                     {"configurable": {"thread_id": thread_id, "thread_ts": parent_ts}}
                     if parent_ts
                     else None,
                 )
 
     async def aput(
         self, config: RunnableConfig, checkpoint: Checkpoint
@@ -122,15 +137,15 @@
         await self.setup()
         async with self.conn.execute(
             "INSERT OR REPLACE INTO checkpoints (thread_id, thread_ts, parent_ts, checkpoint) VALUES (?, ?, ?, ?)",
             (
                 config["configurable"]["thread_id"],
                 checkpoint["ts"],
                 config["configurable"].get("thread_ts"),
-                pickle.dumps(checkpoint),
+                self.serde.dumps(checkpoint),
             ),
         ):
             await self.conn.commit()
         return {
             "configurable": {
                 "thread_id": config["configurable"]["thread_id"],
                 "thread_ts": checkpoint["ts"],
```

### Comparing `gigagraph-0.0.34/langgraph/checkpoint/base.py` & `gigagraph-0.0.37/langgraph/checkpoint/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,22 @@
-import asyncio
 from abc import ABC
 from collections import defaultdict
 from copy import deepcopy
 from datetime import datetime, timezone
-from typing import Any, AsyncIterator, Iterator, NamedTuple, Optional, TypedDict
+from typing import (
+    Any,
+    AsyncIterator,
+    Iterator,
+    NamedTuple,
+    Optional,
+    Protocol,
+    TypedDict,
+)
 
-from langchain_core.load.serializable import Serializable
-from langchain_core.runnables import RunnableConfig
-from langchain_core.runnables.utils import ConfigurableFieldSpec
+from langchain_core.runnables import ConfigurableFieldSpec, RunnableConfig
 
 from langgraph.utils import StrEnum
 
 
 class Checkpoint(TypedDict):
     """State snapshot at a given point in time."""
 
@@ -89,16 +94,33 @@
     name="Thread Timestamp",
     description="Pass to fetch a past checkpoint. If None, fetches the latest checkpoint.",
     default=None,
     is_shared=True,
 )
 
 
-class BaseCheckpointSaver(Serializable, ABC):
-    at: CheckpointAt = CheckpointAt.END_OF_RUN
+class SerializerProtocol(Protocol):
+    def dumps(self, obj: Any) -> bytes: ...
+
+    def loads(self, data: bytes) -> Any: ...
+
+
+class BaseCheckpointSaver(ABC):
+    at: CheckpointAt = CheckpointAt.END_OF_STEP
+
+    serde: SerializerProtocol
+
+    def __init__(
+        self,
+        *,
+        serde: Optional[SerializerProtocol] = None,
+        at: Optional[CheckpointAt] = None,
+    ) -> None:
+        self.serde = serde or self.serde
+        self.at = at or self.at
 
     @property
     def config_specs(self) -> list[ConfigurableFieldSpec]:
         return [CheckpointThreadId, CheckpointThreadTs]
 
     def get(self, config: RunnableConfig) -> Optional[Checkpoint]:
         if value := self.get_tuple(config):
@@ -114,26 +136,16 @@
         raise NotImplementedError
 
     async def aget(self, config: RunnableConfig) -> Optional[Checkpoint]:
         if value := await self.aget_tuple(config):
             return value.checkpoint
 
     async def aget_tuple(self, config: RunnableConfig) -> Optional[CheckpointTuple]:
-        return await asyncio.get_running_loop().run_in_executor(
-            None, self.get_tuple, config
-        )
+        raise NotImplementedError
 
     async def alist(self, config: RunnableConfig) -> AsyncIterator[CheckpointTuple]:
-        loop = asyncio.get_running_loop()
-        iter = loop.run_in_executor(None, self.list, config)
-        while True:
-            try:
-                yield await loop.run_in_executor(None, next, iter)
-            except StopIteration:
-                return
+        raise NotImplementedError
 
     async def aput(
         self, config: RunnableConfig, checkpoint: Checkpoint
     ) -> RunnableConfig:
-        return await asyncio.get_running_loop().run_in_executor(
-            None, self.put, config, checkpoint
-        )
+        raise NotImplementedError
```

### Comparing `gigagraph-0.0.34/langgraph/graph/graph.py` & `gigagraph-0.0.37/langgraph/graph/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,37 +58,37 @@
 
     def _route(
         self,
         input: Any,
         config: RunnableConfig,
         *,
         reader: Optional[Callable[[], Any]],
-        writer: Callable[[str], Optional[Runnable]],
+        writer: Callable[[list[str]], Optional[Runnable]],
     ) -> Runnable:
         result = self.condition.invoke(reader(config) if reader else input, config)
-        if isinstance(result, str):
+        if not isinstance(result, list):
             result = [result]
         if self.ends:
             destinations = [self.ends[r] for r in result]
         else:
             destinations = result
         return writer(destinations) or input
 
     async def _aroute(
         self,
         input: Any,
         config: RunnableConfig,
         *,
         reader: Optional[Callable[[], Any]],
-        writer: Callable[[str], Optional[Runnable]],
+        writer: Callable[[list[str]], Optional[Runnable]],
     ) -> Runnable:
         result = await self.condition.ainvoke(
             reader(config) if reader else input, config
         )
-        if isinstance(result, str):
+        if not isinstance(result, list):
             result = [result]
         if self.ends:
             destinations = [self.ends[r] for r in result]
         else:
             destinations = result
         return writer(destinations) or input
 
@@ -351,15 +351,14 @@
                 n = graph.add_node(node, key)
                 start_nodes[key] = n
                 end_nodes[key] = n
         for start, end in sorted(self.graph._all_edges):
             graph.add_edge(start_nodes[start], end_nodes[end])
         for start, branches in self.graph.branches.items():
             for name, branch in branches.items():
-                name = f"{start}_{name}"
                 cond = graph.add_node(branch.condition, name)
                 graph.add_edge(start_nodes[start], cond)
                 ends = branch.ends or {
                     **{k: k for k in self.graph.nodes},
                     END: END,
                 }
                 for label, end in ends.items():
```

### Comparing `gigagraph-0.0.34/langgraph/graph/message.py` & `gigagraph-0.0.37/langgraph/graph/message.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/graph/state.py` & `gigagraph-0.0.37/langgraph/graph/state.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/prebuilt/agent_executor.py` & `gigagraph-0.0.37/langgraph/prebuilt/agent_executor.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/prebuilt/tool_executor.py` & `gigagraph-0.0.37/langgraph/prebuilt/tool_executor.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/pregel/__init__.py` & `gigagraph-0.0.37/langgraph/pregel/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -694,21 +694,19 @@
                     _apply_writes(checkpoint, channels, pending_writes)
 
                     if debug:
                         print_checkpoint(step, channels)
 
                     # yield current value or updates
                     if stream_mode == "values":
-                        if step_output := map_output_values(
+                        yield from map_output_values(
                             output_keys, pending_writes, channels
-                        ):
-                            yield step_output
+                        )
                     else:
-                        if step_output := map_output_updates(output_keys, next_tasks):
-                            yield step_output
+                        yield from map_output_updates(output_keys, next_tasks)
 
                     # save end of step checkpoint
                     if self.checkpointer is not None and (
                         self.checkpointer.at == CheckpointAt.END_OF_STEP
                     ):
                         checkpoint = create_checkpoint(checkpoint, channels)
                         checkpoint_config = self.checkpointer.put(
@@ -908,21 +906,21 @@
                     _apply_writes(checkpoint, channels, pending_writes)
 
                     if debug:
                         print_checkpoint(step, channels)
 
                     # yield current value or updates
                     if stream_mode == "values":
-                        if step_output := map_output_values(
+                        for chunk in map_output_values(
                             output_keys, pending_writes, channels
                         ):
-                            yield step_output
+                            yield chunk
                     else:
-                        if step_output := map_output_updates(output_keys, next_tasks):
-                            yield step_output
+                        for chunk in map_output_updates(output_keys, next_tasks):
+                            yield chunk
 
                     # save end of step checkpoint
                     if self.checkpointer is not None and (
                         self.checkpointer.at == CheckpointAt.END_OF_STEP
                     ):
                         checkpoint = create_checkpoint(checkpoint, channels)
                         checkpoint_config = await self.checkpointer.aput(
@@ -969,32 +967,31 @@
         input_keys: Optional[Union[str, Sequence[str]]] = None,
         interrupt_before_nodes: Optional[Sequence[str]] = None,
         interrupt_after_nodes: Optional[Sequence[str]] = None,
         debug: Optional[bool] = None,
         **kwargs: Any,
     ) -> Union[dict[str, Any], Any]:
         output_keys = output_keys if output_keys is not None else self.output_channels
-        output_is_dict = not isinstance(output_keys, str)
         if stream_mode == "values":
-            latest: Union[dict[str, Any], Any] = {} if output_is_dict else None
+            latest: Union[dict[str, Any], Any] = None
         else:
             chunks = []
         for chunk in self.stream(
             input,
             config,
             stream_mode=stream_mode,
             output_keys=output_keys,
             input_keys=input_keys,
             interrupt_before_nodes=interrupt_before_nodes,
             interrupt_after_nodes=interrupt_after_nodes,
             debug=debug,
             **kwargs,
         ):
             if stream_mode == "values":
-                latest = {**latest, **chunk} if output_is_dict else chunk
+                latest = chunk
             else:
                 chunks.append(chunk)
         if stream_mode == "values":
             return latest
         else:
             return chunks
 
@@ -1008,32 +1005,31 @@
         input_keys: Optional[Union[str, Sequence[str]]] = None,
         interrupt_before_nodes: Optional[Sequence[str]] = None,
         interrupt_after_nodes: Optional[Sequence[str]] = None,
         debug: Optional[bool] = None,
         **kwargs: Any,
     ) -> Union[dict[str, Any], Any]:
         output_keys = output_keys if output_keys is not None else self.output_channels
-        output_is_dict = not isinstance(output_keys, str)
         if stream_mode == "values":
-            latest: Union[dict[str, Any], Any] = {} if output_is_dict else None
+            latest: Union[dict[str, Any], Any] = None
         else:
             chunks = []
         async for chunk in self.astream(
             input,
             config,
             stream_mode=stream_mode,
             output_keys=output_keys,
             input_keys=input_keys,
             interrupt_before_nodes=interrupt_before_nodes,
             interrupt_after_nodes=interrupt_after_nodes,
             debug=debug,
             **kwargs,
         ):
             if stream_mode == "values":
-                latest = {**latest, **chunk} if output_is_dict else chunk
+                latest = chunk
             else:
                 chunks.append(chunk)
         if stream_mode == "values":
             return latest
         else:
             return chunks
```

### Comparing `gigagraph-0.0.34/langgraph/pregel/debug.py` & `gigagraph-0.0.37/langgraph/pregel/debug.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/pregel/io.py` & `gigagraph-0.0.37/langgraph/pregel/io.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,42 +61,40 @@
                 logger.warning(f"Input channel {k} not found in {input_channels}")
 
 
 def map_output_values(
     output_channels: Union[str, Sequence[str]],
     pending_writes: Sequence[tuple[str, Any]],
     channels: Mapping[str, BaseChannel],
-) -> Optional[Union[dict[str, Any], Any]]:
+) -> Iterator[Union[dict[str, Any], Any]]:
     """Map pending writes (a sequence of tuples (channel, value)) to output chunk."""
     if isinstance(output_channels, str):
         if any(chan == output_channels for chan, _ in pending_writes):
-            return read_channel(channels, output_channels)
+            yield read_channel(channels, output_channels)
     else:
-        if updated := {c for c, _ in pending_writes if c in output_channels}:
-            return read_channels(channels, updated)
-    return None
+        if {c for c, _ in pending_writes if c in output_channels}:
+            yield read_channels(channels, output_channels)
 
 
 def map_output_updates(
     output_channels: Union[str, Sequence[str]],
     tasks: list[PregelExecutableTask],
-) -> Optional[dict[str, Union[Any, dict[str, Any]]]]:
+) -> Iterator[dict[str, Union[Any, dict[str, Any]]]]:
     """Map pending writes (a sequence of tuples (channel, value)) to output chunk."""
     output_tasks = [
         t for t in tasks if not t.config or TAG_HIDDEN not in t.config.get("tags")
     ]
     if isinstance(output_channels, str):
         if updated := {
             node: value
             for node, _, _, writes, _ in output_tasks
             for chan, value in writes
             if chan == output_channels
         }:
-            return updated
+            yield updated
     else:
         if updated := {
             node: {chan: value for chan, value in writes if chan in output_channels}
             for node, _, _, writes, _ in output_tasks
             if any(chan in output_channels for chan, _ in writes)
         }:
-            return updated
-    return None
+            yield updated
```

### Comparing `gigagraph-0.0.34/langgraph/pregel/read.py` & `gigagraph-0.0.37/langgraph/pregel/read.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/pregel/types.py` & `gigagraph-0.0.37/langgraph/pregel/types.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/pregel/validate.py` & `gigagraph-0.0.37/langgraph/pregel/validate.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/pregel/write.py` & `gigagraph-0.0.37/langgraph/pregel/write.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/langgraph/utils.py` & `gigagraph-0.0.37/langgraph/utils.py`

 * *Files identical despite different names*

### Comparing `gigagraph-0.0.34/pyproject.toml` & `gigagraph-0.0.37/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "gigagraph"
-version = "0.0.34"
-description = "gigagraph"
+version = "0.0.37"
+description = "langgraph"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigagraph"
 packages = [
     {include = "langgraph"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9.0,<4.0"
-gigachain-core = "^0.1.38"
+gigachain-core = "^0.1.42rc1"
 
 
 [tool.poetry.group.test.dependencies]
 # The only dependencies that should be added are
 # dependencies used for running tests (e.g., pytest, freezegun, response).
 # Any dependencies that do not meet that criteria will be removed.
 pytest = "^7.3.0"
@@ -40,15 +40,15 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 jupyter = "^1.0.0"
 gigachain = "^0.1.0"
 langchainhub = "^0.1.14"
-gigachain-openai = "^0.0.5"
+gigachain-openai = "^0.1.2"
 
 [tool.ruff]
 select = [ "E", "F", "I" ]
 ignore = [ "E501" ]
 
 [tool.mypy]
 ignore_missing_imports = "True"
```

### Comparing `gigagraph-0.0.34/PKG-INFO` & `gigagraph-0.0.37/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: gigagraph
-Version: 0.0.34
-Summary: gigagraph
-Home-page: https://github.com/ai-forever/gigagraph
-License: MIT
-Requires-Python: >=3.9.0,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: gigachain-core (>=0.1.38,<0.2.0)
-Project-URL: Repository, https://github.com/ai-forever/gigagraph
-Description-Content-Type: text/markdown
-
 # GigaGraph
 
 ⚡ Разработка языковых агентов в виде графов ⚡
 
 ## Описание
 
 GigaGraph — это библиотека, дающая возможность работать с LLM (большие языковые модели) для создания приложений, которые используют множество взаимодействующих цепочек (акторов) и сохраняют данные о состоянии.
@@ -515,15 +498,16 @@
 
 ### Reflection / Self-Critique
 
 When output quality is a major concern, it's common to incorporate some combination of self-critique or reflection and external validation to refine your system's outputs. The following examples demonstrate research that implement this type of design.
 
 - [Basic Reflection](./examples/reflection/reflection.ipynb): add a simple "reflect" step in your graph to prompt your system to revise its outputs.
 - [Reflexion](./examples/reflexion/reflexion.ipynb): critique missing and superflous aspects of the agent's response to guide subsequent steps. Based on [Reflexion](https://arxiv.org/abs/2303.11366), by Shinn, et. al.
-- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406), by Zhou, et. al.
+- [Giga Reflexion](./examples/reflexion_giga/reflexion.ipynb): реализация Reflexion на GigaChat
+- [Language Agent Tree Search](./examples/lats/lats.ipynb): execute multiple agents in parallel, using reflection and environmental rewards to drive a Monte Carlo Tree Search. Based on [LATS](https://arxiv.org/abs/2310.04406/LanguageAgentTreeSearch/), by Zhou, et. al.
 
 ### Multi-agent Examples
 ### Примеры с несколькими агентами
 
 - [Совместная работа нескольких агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/multi-agent-collaboration.ipynb). Пример демонстрирует как создать двух агентов, которые работают вместе для решения задачи.
 - [Несколько агентов с «руководителем»](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/agent_supervisor.ipynb). Пример демонстрирует как организовать работу агентов используя LLM в роли «руководителя», который решает как распределять работу.
 - [Иерархичные команды агентов](https://github.com/langchain-ai/langgraph/blob/main/examples/multi_agent/hierarchical_agent_teams.ipynb): пример демонстрирует как организовать «команды» агентов, которые будут взаимодействовать для решения задачи, в виде вложенных графов.
@@ -856,8 +840,7 @@
 app = create_agent_executor(agent_runnable, tools)
 
 inputs = {"input": "what is the weather in sf", "chat_history": []}
 for s in app.stream(inputs):
     print(list(s.values())[0])
     print("----")
 ```
-
```

