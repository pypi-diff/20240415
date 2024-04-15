# Comparing `tmp/jupyter_server_ydoc-0.8.0a0.tar.gz` & `tmp/jupyter_server_ydoc-1.0.0a0.tar.gz`

## Comparing `jupyter_server_ydoc-0.8.0a0.tar` & `jupyter_server_ydoc-1.0.0a0.tar`

### file list

```diff
@@ -1,33 +1,26 @@
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.flake8
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.gitconfig
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    20877 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/CHANGELOG.md
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/CONTRIBUTING.rst
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/RELEASE.md
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/codecov.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/readthedocs.yml
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.github/workflows/check-release.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     4183 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.github/workflows/test.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/Makefile
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/README.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/doc-requirements.txt
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/environment.yml
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/make.bat
--rw-r--r--   0        0        0    11671 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/source/conf.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/source/index.rst
--rw-r--r--   0        0        0    10448 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/source/_static/jupyter_server_logo.svg
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/docs/source/contributors/contributing.rst
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/jupyter-config/jupyter_notebook_ydoc.json
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/jupyter-config/jupyter_server_ydoc.json
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/jupyter_server_ydoc/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/jupyter_server_ydoc/app.py
--rw-r--r--   0        0        0    18380 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/jupyter_server_ydoc/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/tests/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/tests/test_ydoc.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/LICENSE
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/README.md
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/pyproject.toml
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 jupyter_server_ydoc-0.8.0a0/PKG-INFO
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/setup.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter-config/jupyter_server_ydoc.json
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/_version.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/app.py
+-rw-r--r--   0        0        0    15708 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/handlers.py
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/loaders.py
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/rooms.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/stores.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/utils.py
+-rw-r--r--   0        0        0     4571 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/websocketserver.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/events/awareness.yaml
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/events/session.yaml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/conftest.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_app.py
+-rw-r--r--   0        0        0     2785 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_documents.py
+-rw-r--r--   0        0        0     4047 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2477 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_loaders.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/test_rooms.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/tests/utils.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/README.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0     4989 2020-02-02 00:00:00.000000 jupyter_server_ydoc-1.0.0a0/PKG-INFO
```

### Comparing `jupyter_server_ydoc-0.8.0a0/jupyter_server_ydoc/handlers.py` & `jupyter_server_ydoc-1.0.0a0/jupyter_server_ydoc/handlers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,431 +1,386 @@
 # Copyright (c) Jupyter Development Team.
 # Distributed under the terms of the Modified BSD License.
 
+from __future__ import annotations
+
 import asyncio
 import json
+import time
 import uuid
-from logging import Logger
-from pathlib import Path
-from typing import Any, Dict, Optional, Tuple
+from typing import Any
 
 from jupyter_server.auth import authorized
 from jupyter_server.base.handlers import APIHandler, JupyterHandler
-from jupyter_server.utils import ensure_async
-from jupyter_ydoc import ydocs as YDOCS  # type: ignore
+from jupyter_ydoc import ydocs as YDOCS
+from pycrdt_websocket.websocket_server import YRoom
+from pycrdt_websocket.ystore import BaseYStore
+from pycrdt_websocket.yutils import YMessageType, write_var_uint
 from tornado import web
 from tornado.websocket import WebSocketHandler
-from traitlets import Int, Unicode
-from traitlets.config import LoggingConfigurable
-from ypy_websocket.websocket_server import WebsocketServer, YRoom  # type: ignore
-from ypy_websocket.ystore import BaseYStore  # type: ignore
-from ypy_websocket.ystore import SQLiteYStore as _SQLiteYStore
-from ypy_websocket.ystore import TempFileYStore as _TempFileYStore
-from ypy_websocket.ystore import YDocNotFound
-from ypy_websocket.yutils import YMessageType  # type: ignore
+
+from .loaders import FileLoaderMapping
+from .rooms import DocumentRoom, TransientRoom
+from .utils import (
+    JUPYTER_COLLABORATION_AWARENESS_EVENTS_URI,
+    JUPYTER_COLLABORATION_EVENTS_URI,
+    LogLevel,
+    MessageType,
+    decode_file_path,
+    room_id_from_encoded_path,
+)
+from .websocketserver import JupyterWebsocketServer
 
 YFILE = YDOCS["file"]
 
 SERVER_SESSION = str(uuid.uuid4())
 
 
-class TempFileYStore(_TempFileYStore):
-    prefix_dir = "jupyter_ystore_"
-
-
-class SQLiteYStoreMetaclass(type(LoggingConfigurable), type(_SQLiteYStore)):  # type: ignore
-    pass
-
-
-class SQLiteYStore(LoggingConfigurable, _SQLiteYStore, metaclass=SQLiteYStoreMetaclass):
-    db_path = Unicode(
-        ".jupyter_ystore.db",
-        config=True,
-        help="""The path to the YStore database. Defaults to '.jupyter_ystore.db' in the current
-        directory.""",
-    )
-
-    document_ttl = Int(
-        None,
-        allow_none=True,
-        config=True,
-        help="""The document time-to-live in seconds. Defaults to None (document history is never
-        cleared).""",
-    )
-
-
-class DocumentRoom(YRoom):
-    """A Y room for a possibly stored document (e.g. a notebook)."""
-
-    def __init__(self, type: str, ystore: BaseYStore, log: Optional[Logger]):
-        super().__init__(ready=False, ystore=ystore, log=log)
-        self.type = type
-        self.cleaner: Optional["asyncio.Task[Any]"] = None
-        self.watcher: Optional["asyncio.Task[Any]"] = None
-        self.document = YDOCS.get(type, YFILE)(self.ydoc)
-
-
-class TransientRoom(YRoom):
-    """A Y room for sharing state (e.g. awareness)."""
-
-    def __init__(self, log: Optional[Logger]):
-        super().__init__(log=log)
-
-
-class JupyterWebsocketServer(WebsocketServer):
-
-    rooms: Dict[str, YRoom]
-    ypatch_nb: int
-    connected_user: Dict[int, str]
-
-    def __init__(self, *args, **kwargs):
-        self.ystore_class = kwargs.pop("ystore_class")
-        self.log = kwargs["log"]
-        super().__init__(*args, **kwargs)
-        self.ypatch_nb = 0
-        self.connected_users = {}
-        asyncio.create_task(self.monitor())
-
-    async def monitor(self):
-        while True:
-            await asyncio.sleep(60)
-            clients_nb = sum(len(room.clients) for room in self.rooms.values())
-            self.log.info("Processed %s Y patches in one minute", self.ypatch_nb)
-            self.log.info("Connected Y users: %s", clients_nb)
-            self.ypatch_nb = 0
-
-    def get_room(self, path: str) -> YRoom:
-        if path not in self.rooms:
-            if path.count(":") >= 2:
-                # it is a stored document (e.g. a notebook)
-                file_format, file_type, file_path = path.split(":", 2)
-                p = Path(file_path)
-                updates_file_path = str(p.parent / f".{file_type}:{p.name}.y")
-                ystore = self.ystore_class(path=updates_file_path, log=self.log)
-                self.rooms[path] = DocumentRoom(file_type, ystore, self.log)
-            else:
-                # it is a transient document (e.g. awareness)
-                self.rooms[path] = TransientRoom(self.log)
-        return self.rooms[path]
-
-
 class YDocWebSocketHandler(WebSocketHandler, JupyterHandler):
-    """`YDocWebSocketHandler` uses the singleton pattern for `WebsocketServer`,
-    which is a subclass of ypy-websocket's `WebsocketServer`.
+    """`YDocWebSocketHandler` uses the singleton pattern for ``WebsocketServer``,
+    which is a subclass of ypy-websocket's ``WebsocketServer``.
+
+    In ``WebsocketServer``, we expect to use a WebSocket object as follows:
 
-    In `WebsocketServer`, we expect to use a WebSocket object as follows:
     - receive messages until the connection is closed with
-      `for message in websocket: pass`.
+       ``for message in websocket: pass``.
     - send a message with `await websocket.send(message)`.
 
-    Tornado's WebSocket API is different, so `YDocWebSocketHandler` needs to be adapted:
-    - `YDocWebSocketHandler` is an async iterator, that will yield received messages.
-      Messages received in Tornado's `on_message(message)` are put in an async
-      `_message_queue`, from which we get them asynchronously.
-    - The `send(message)` method is async and calls Tornado's `write_message(message)`.
-    - Although it's currently not used in ypy-websocket, `recv()` is an async method for
-      receiving a message.
+    Tornado's WebSocket API is different, so ``YDocWebSocketHandler`` needs to be adapted:
+
+    - ``YDocWebSocketHandler`` is an async iterator, that will yield received messages.
+       Messages received in Tornado's `on_message(message)` are put in an async
+       ``_message_queue``, from which we get them asynchronously.
+    - The ``send(message)`` method is async and calls Tornado's ``write_message(message)``.
+    - Although it's currently not used in ypy-websocket, ``recv()`` is an async method for
+       receiving a message.
     """
 
-    saving_document: Optional["asyncio.Task[Any]"]
-    websocket_server: Optional[JupyterWebsocketServer] = None
-    _message_queue: "asyncio.Queue[Any]"
+    _message_queue: asyncio.Queue[Any]
+    _background_tasks: set[asyncio.Task]
+    _room_locks: dict[str, asyncio.Lock] = {}
+
+    def _room_lock(self, room_id: str) -> asyncio.Lock:
+        if room_id not in self._room_locks:
+            self._room_locks[room_id] = asyncio.Lock()
+        return self._room_locks[room_id]
+
+    def create_task(self, aw):
+        task = asyncio.create_task(aw)
+        self._background_tasks.add(task)
+        task.add_done_callback(self._background_tasks.discard)
+
+    async def prepare(self):
+        if not self._websocket_server.started.is_set():
+            self.create_task(self._websocket_server.start())
+            await self._websocket_server.started.wait()
+
+        # Get room
+        self._room_id: str = room_id_from_encoded_path(self.request.path)
+
+        async with self._room_lock(self._room_id):
+            if self._websocket_server.room_exists(self._room_id):
+                self.room: YRoom = await self._websocket_server.get_room(self._room_id)
+            else:
+                if self._room_id.count(":") >= 2:
+                    # DocumentRoom
+                    file_format, file_type, file_id = decode_file_path(self._room_id)
+                    if file_id in self._file_loaders:
+                        self._emit(
+                            LogLevel.WARNING,
+                            None,
+                            "There is another collaborative session accessing the same file.\nThe synchronization between rooms is not supported and you might lose some of your changes.",
+                        )
+
+                    file = self._file_loaders[file_id]
+                    updates_file_path = f".{file_type}:{file_id}.y"
+                    ystore = self._ystore_class(path=updates_file_path, log=self.log)
+                    self.room = DocumentRoom(
+                        self._room_id,
+                        file_format,
+                        file_type,
+                        file,
+                        self.event_logger,
+                        ystore,
+                        self.log,
+                        self._document_save_delay,
+                    )
+
+                else:
+                    # TransientRoom
+                    # it is a transient document (e.g. awareness)
+                    self.room = TransientRoom(self._room_id, self.log)
+
+            await self._websocket_server.start_room(self.room)
+            self._websocket_server.add_room(self._room_id, self.room)
+
+        res = super().prepare()
+        if res is not None:
+            return await res
+
+    def initialize(
+        self,
+        ywebsocket_server: JupyterWebsocketServer,
+        file_loaders: FileLoaderMapping,
+        ystore_class: type[BaseYStore],
+        document_cleanup_delay: float | None = 60.0,
+        document_save_delay: float | None = 1.0,
+    ) -> None:
+        self._background_tasks = set()
+        # File ID manager cannot be passed as argument as the extension may load after this one
+        self._file_id_manager = self.settings["file_id_manager"]
+        self._file_loaders = file_loaders
+        self._ystore_class = ystore_class
+        self._cleanup_delay = document_cleanup_delay
+        self._document_save_delay = document_save_delay
+        self._websocket_server = ywebsocket_server
+        self._message_queue = asyncio.Queue()
+
+    @property
+    def path(self):
+        """
+        Returns the room id. It needs to be called 'path' for compatibility with
+        the WebsocketServer (websocket.path).
+        """
+        return self._room_id
 
-    # Override max_message size to 1GB
     @property
     def max_message_size(self):
+        """
+        Override max_message size to 1GB
+        """
         return 1024 * 1024 * 1024
 
     def __aiter__(self):
         # needed to be compatible with WebsocketServer (async for message in websocket)
         return self
 
     async def __anext__(self):
         # needed to be compatible with WebsocketServer (async for message in websocket)
         message = await self._message_queue.get()
         if not message:
             raise StopAsyncIteration()
         return message
 
-    def get_file_info(self) -> Tuple[str, str, str]:
-        assert self.websocket_server is not None
-        assert isinstance(self.room, DocumentRoom)
-        room_name = self.websocket_server.get_room_name(self.room)
-        file_format: str
-        file_type: str
-        file_path: Optional[str]
-        file_id: str
-        file_format, file_type, file_id = room_name.split(":", 2)
-        file_path = self.settings["file_id_manager"].get_path(file_id)
-        if file_path is None:
-            raise RuntimeError(f"File {self.room.document.path} cannot be found anymore")
-        assert file_path is not None
-        if file_path != self.room.document.path:
-            self.log.debug(
-                "File with ID %s was moved from %s to %s",
-                self.room.document.path,
-                file_path,
-            )
-            self.room.document.path = file_path
-        return file_format, file_type, file_path
-
-    def set_file_info(self, value: str) -> None:
-        assert self.websocket_server is not None
-        self.websocket_server.rename_room(value, from_room=self.room)
-        self.path = value  # needed to be compatible with WebsocketServer (websocket.path)
-
     async def get(self, *args, **kwargs):
-        if self.get_current_user() is None:
+        """
+        Overrides default behavior to check whether the client is authenticated or not.
+        """
+        if self.current_user is None:
             self.log.warning("Couldn't authenticate WebSocket connection")
             raise web.HTTPError(403)
         return await super().get(*args, **kwargs)
 
-    async def open(self, path):
-        ystore_class = self.settings["collaborative_ystore_class"]
-        if self.websocket_server is None:
-            for k, v in self.config.get(ystore_class.__name__, {}).items():
-                setattr(ystore_class, k, v)
-            YDocWebSocketHandler.websocket_server = JupyterWebsocketServer(
-                rooms_ready=False,
-                auto_clean_rooms=False,
-                ystore_class=ystore_class,
-                log=self.log,
-            )
-        self._message_queue = asyncio.Queue()
-        self.lock = asyncio.Lock()
-        assert self.websocket_server is not None
-        self.room = self.websocket_server.get_room(path)
-        self.set_file_info(path)
-        self.saving_document = None
-        asyncio.create_task(self.websocket_server.serve(self))
-
-        # Close the connection if the document session expired
-        session_id = self.get_query_argument("sessionId", "")
-        if isinstance(self.room, DocumentRoom) and SERVER_SESSION != session_id:
-            self.close(1003, f"Document session {session_id} expired")
-
-        # cancel the deletion of the room if it was scheduled
-        if isinstance(self.room, DocumentRoom) and self.room.cleaner is not None:
-            self.room.cleaner.cancel()
-
-        if isinstance(self.room, DocumentRoom) and not self.room.ready:
-            file_format, file_type, file_path = self.get_file_info()
-            self.log.debug("Opening Y document from disk: %s", file_path)
-            model = await ensure_async(
-                self.contents_manager.get(file_path, type=file_type, format=file_format)
-            )
-            self.last_modified = model["last_modified"]
-            # check again if ready, because loading the file can be async
-            if not self.room.ready:
-                # try to apply Y updates from the YStore for this document
-                read_from_source = True
-                if self.room.ystore is not None:
-                    try:
-                        await self.room.ystore.apply_updates(self.room.ydoc)
-                        read_from_source = False
-                    except YDocNotFound:
-                        # YDoc not found in the YStore, create the document from the source file (no change history)
-                        pass
-                if not read_from_source:
-                    # if YStore updates and source file are out-of-sync, resync updates with source
-                    if self.room.document.source != model["content"]:
-                        read_from_source = True
-
-                if read_from_source:
-                    self.room.document.source = model["content"]
-                    if self.room.ystore:
-                        await self.room.ystore.encode_state_as_update(self.room.ydoc)
-                self.room.document.dirty = False
-                self.room.ready = True
-                self.room.watcher = asyncio.create_task(self.watch_file())
-                # save the document when changed
-                self.room.document.observe(self.on_document_change)
-
-    async def watch_file(self):
-        assert isinstance(self.room, DocumentRoom)
-        poll_interval = self.settings["collaborative_file_poll_interval"]
-        if not poll_interval:
-            self.room.watcher = None
-            return
-        while True:
-            await asyncio.sleep(poll_interval)
-            await self.maybe_load_document()
-
-    async def maybe_load_document(self):
-        assert isinstance(self.room, DocumentRoom)
-        file_format, file_type, file_path = self.get_file_info()
-        async with self.lock:
-            model = await ensure_async(
-                self.contents_manager.get(
-                    file_path, content=False, type=file_type, format=file_format
+    async def open(self, room_id):
+        """
+        On connection open.
+        """
+        self.create_task(self._websocket_server.serve(self))
+
+        if isinstance(self.room, DocumentRoom):
+            # Close the connection if the document session expired
+            session_id = self.get_query_argument("sessionId", "")
+            if SERVER_SESSION != session_id:
+                self.close(
+                    1003,
+                    f"Document session {session_id} expired. You need to reload this browser tab.",
                 )
-            )
-        # do nothing if the file was saved by us
-        if self.last_modified < model["last_modified"]:
-            self.log.debug("Reverting file that had out-of-band changes: %s", file_path)
-            model = await ensure_async(
-                self.contents_manager.get(file_path, type=file_type, format=file_format)
-            )
-            self.room.document.source = model["content"]
-            self.last_modified = model["last_modified"]
+
+            # cancel the deletion of the room if it was scheduled
+            if self.room.cleaner is not None:
+                self.room.cleaner.cancel()
+
+            try:
+                # Initialize the room
+                async with self._room_lock(self._room_id):
+                    await self.room.initialize()
+                self._emit_awareness_event(self.current_user.username, "join")
+            except Exception as e:
+                _, _, file_id = decode_file_path(self._room_id)
+                file = self._file_loaders[file_id]
+
+                # Close websocket and propagate error.
+                if isinstance(e, web.HTTPError):
+                    self.log.error(f"File {file.path} not found.\n{e!r}", exc_info=e)
+                    self.close(1004, f"File {file.path} not found.")
+                else:
+                    self.log.error(f"Error initializing: {file.path}\n{e!r}", exc_info=e)
+                    self.close(
+                        1003, f"Error initializing: {file.path}. You need to close the document."
+                    )
+
+                # Clean up the room and delete the file loader
+                if len(self.room.clients) == 0 or self.room.clients == [self]:
+                    self._message_queue.put_nowait(b"")
+                    self._cleanup_delay = 0
+                    await self._clean_room()
+
+            self._emit(LogLevel.INFO, "initialize", "New client connected.")
+        else:
+            if self._room_id != "JupyterLab:globalAwareness":
+                self._emit_awareness_event(self.current_user.username, "join")
 
     async def send(self, message):
+        """
+        Send a message to the client.
+        """
         # needed to be compatible with WebsocketServer (websocket.send)
         try:
             self.write_message(message, binary=True)
         except Exception as e:
             self.log.debug("Failed to write message", exc_info=e)
 
     async def recv(self):
+        """
+        Receive a message from the client.
+        """
         message = await self._message_queue.get()
         return message
 
-    def on_message(self, message):
-        assert self.websocket_server is not None
+    async def on_message(self, message):
+        """
+        On message receive.
+        """
         message_type = message[0]
+
         if message_type == YMessageType.AWARENESS:
             # awareness
             skip = False
             changes = self.room.awareness.get_changes(message[1:])
             added_users = changes["added"]
             removed_users = changes["removed"]
             for i, user in enumerate(added_users):
                 u = changes["states"][i]
                 if "user" in u:
                     name = u["user"]["name"]
-                    self.websocket_server.connected_users[user] = name
+                    self._websocket_server.connected_users[user] = name
                     self.log.debug("Y user joined: %s", name)
             for user in removed_users:
-                if user in self.websocket_server.connected_users:
-                    name = self.websocket_server.connected_users[user]
-                    del self.websocket_server.connected_users[user]
+                if user in self._websocket_server.connected_users:
+                    name = self._websocket_server.connected_users[user]
+                    del self._websocket_server.connected_users[user]
                     self.log.debug("Y user left: %s", name)
             # filter out message depending on changes
             if skip:
                 self.log.debug(
                     "Filtered out Y message of type: %s",
                     YMessageType(message_type).name,
                 )
                 return skip
+
+        if message_type == MessageType.CHAT:
+            msg = message[2:].decode("utf-8")
+
+            user = self.current_user
+            data = json.dumps(
+                {"sender": user.username, "timestamp": time.time(), "content": json.loads(msg)}
+            ).encode("utf8")
+
+            for client in self.room.clients:
+                if client != self:
+                    task = asyncio.create_task(
+                        client.send(bytes([MessageType.CHAT]) + write_var_uint(len(data)) + data)
+                    )
+                    self._websocket_server.background_tasks.add(task)
+                    task.add_done_callback(self._websocket_server.background_tasks.discard)
+
         self._message_queue.put_nowait(message)
-        self.websocket_server.ypatch_nb += 1
+        self._websocket_server.ypatch_nb += 1
 
     def on_close(self) -> None:
+        """
+        On connection close.
+        """
         # stop serving this client
         self._message_queue.put_nowait(b"")
         if isinstance(self.room, DocumentRoom) and self.room.clients == [self]:
             # no client in this room after we disconnect
             # keep the document for a while in case someone reconnects
-            self.room.cleaner = asyncio.create_task(self.clean_room())
-
-    async def clean_room(self) -> None:
+            self.log.info("Cleaning room: %s", self._room_id)
+            self.room.cleaner = asyncio.create_task(self._clean_room())
+        if self._room_id != "JupyterLab:globalAwareness":
+            self._emit_awareness_event(self.current_user.username, "leave")
+
+    def _emit(self, level: LogLevel, action: str | None = None, msg: str | None = None) -> None:
+        _, _, file_id = decode_file_path(self._room_id)
+        path = self._file_id_manager.get_path(file_id)
+
+        data = {"level": level.value, "room": self._room_id, "path": path}
+        if action:
+            data["action"] = action
+        if msg:
+            data["msg"] = msg
+
+        self.event_logger.emit(schema_id=JUPYTER_COLLABORATION_EVENTS_URI, data=data)
+
+    def _emit_awareness_event(self, username: str, action: str, msg: str | None = None) -> None:
+        data = {"roomid": self._room_id, "username": username, "action": action}
+        if msg:
+            data["msg"] = msg
+
+        self.event_logger.emit(schema_id=JUPYTER_COLLABORATION_AWARENESS_EVENTS_URI, data=data)
+
+    async def _clean_room(self) -> None:
+        """
+        Async task for cleaning up the resources.
+
+        When all the clients of a room leave, we setup a task to clean up the resources
+        after a certain amount of time. We need to wait a few seconds to clean up the room
+        because sometimes websockets unintentionally disconnect.
+
+        During the clean up, we need to delete the room to free resources since the room
+        contains a copy of the document. In addition, we remove the file if there is no rooms
+        subscribed to it.
+        """
         assert isinstance(self.room, DocumentRoom)
-        seconds = self.settings["collaborative_document_cleanup_delay"]
-        if seconds is None:
+
+        if self._cleanup_delay is None:
             return
-        await asyncio.sleep(seconds)
-        if self.room.watcher is not None:
-            self.room.watcher.cancel()
-        self.room.document.unobserve()
-        assert self.websocket_server is not None
-        file_format, file_type, file_path = self.get_file_info()
-        self.log.debug("Deleting Y document from memory: %s", file_path)
-        self.websocket_server.delete_room(room=self.room)
 
-    def on_document_change(self, event):
-        try:
-            dirty = event.keys["dirty"]["newValue"]
-            if not dirty:
-                # we cleared the dirty flag, nothing to save
-                return
-        except Exception:
-            pass
-        if self.saving_document is not None and not self.saving_document.done():
-            # the document is being saved, cancel that
-            self.saving_document.cancel()
-            self.saving_document = None
-        self.saving_document = asyncio.create_task(self.maybe_save_document())
+        await asyncio.sleep(self._cleanup_delay)
 
-    async def maybe_save_document(self):
-        assert isinstance(self.room, DocumentRoom)
-        seconds = self.settings["collaborative_document_save_delay"]
-        if seconds is None:
-            return
-        # save after X seconds of inactivity
-        await asyncio.sleep(seconds)
-        # if the room cannot be found, don't save
-        try:
-            file_format, file_type, file_path = self.get_file_info()
-        except Exception:
-            return
-        self.log.debug("Opening Y document from disk: %s", file_path)
-        async with self.lock:
-            model = await ensure_async(
-                self.contents_manager.get(file_path, type=file_type, format=file_format)
-            )
-        if self.last_modified < model["last_modified"]:
-            # file changed on disk, let's revert
-            self.log.debug("Reverting file that had out-of-band changes: %s", file_path)
-            self.room.document.source = model["content"]
-            self.last_modified = model["last_modified"]
-            return
-        if model["content"] != self.room.document.source:
-            # don't save if not needed
-            # this also prevents the dirty flag from bouncing between windows of
-            # the same document opened as different types (e.g. notebook/text editor)
-            model["format"] = file_format
-            model["content"] = self.room.document.source
-            self.log.debug("Saving Y document to disk: %s", file_path)
-            async with self.lock:
-                model = await ensure_async(self.contents_manager.save(model, file_path))
-                self.last_modified = model["last_modified"]
-        self.room.document.dirty = False
+        async with self._room_lock(self._room_id):
+            # Remove the room from the websocket server
+            self.log.info("Deleting Y document from memory: %s", self._room_id)
+            self._websocket_server.delete_room(room=self.room)
+
+            # Clean room
+            del self.room
+            self.log.info("Room %s deleted", self._room_id)
+            self._emit(LogLevel.INFO, "clean", "Room deleted.")
+
+            # Clean the file loader if there are not rooms using it
+            _, _, file_id = decode_file_path(self._room_id)
+            file = self._file_loaders[file_id]
+            if file.number_of_subscriptions == 0:
+                self.log.info("Deleting file %s", file.path)
+                await self._file_loaders.remove(file_id)
+                self._emit(LogLevel.INFO, "clean", "Loader deleted.")
+            del self._room_locks[self._room_id]
 
     def check_origin(self, origin):
+        """
+        Check origin
+        """
         return True
 
 
-class YDocRoomIdHandler(APIHandler):
-    auth_resource = "contents"
-
-    @web.authenticated
-    @authorized
-    async def put(self, path):
-        body = json.loads(self.request.body)
-        ws_url = f"{body['format']}:{body['type']}:"
-
-        file_id_manager = self.settings["file_id_manager"]
-
-        idx = file_id_manager.get_id(path)
-        if idx is not None:
-            # index already exists
-            self.set_status(200)
-            ws_url += str(idx)
-            self.log.info("Request for Y document '%s' with room ID: %s", path, ws_url)
-            return self.finish(ws_url)
-
-        # try indexing
-        idx = file_id_manager.index(path)
-        if idx is None:
-            # file does not exists
-            raise web.HTTPError(404, f"File {path!r} does not exist")
-
-        # index successfully created
-        self.set_status(201)
-        ws_url += str(idx)
-        self.log.info("Request for Y document '%s' with room ID: %s", path, ws_url)
-        return self.finish(ws_url)
-
-
 class DocSessionHandler(APIHandler):
+    """
+    Jupyter Server's handler to retrieve the document's session.
+    """
+
     auth_resource = "contents"
 
     @web.authenticated
     @authorized
     async def put(self, path):
+        """
+        Creates a new session for a given document or returns an existing one.
+        """
         body = json.loads(self.request.body)
         format = body["format"]
         content_type = body["type"]
         file_id_manager = self.settings["file_id_manager"]
 
         idx = file_id_manager.get_id(path)
         if idx is not None:
```

### Comparing `jupyter_server_ydoc-0.8.0a0/LICENSE` & `jupyter_server_ydoc-1.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_server_ydoc-0.8.0a0/PKG-INFO` & `jupyter_server_ydoc-1.0.0a0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-Metadata-Version: 2.1
-Name: jupyter_server_ydoc
-Version: 0.8.0a0
-Summary: A Jupyter Server Extension Providing Y Documents.
-Project-URL: Homepage, https://jupyter.org
+Metadata-Version: 2.3
+Name: jupyter-server-ydoc
+Version: 1.0.0a0
+Summary: jupyter-server extension integrating collaborative shared models.
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: # Licensing terms
         
         This project is licensed under the terms of the Modified BSD License
         (also known as New or Revised or 3-Clause BSD), as follows:
         
         - Copyright (c) 2021-, Jupyter Development Team
@@ -60,52 +59,42 @@
         
         With this in mind, the following banner should be used in any source code file
         to indicate the copyright and license terms:
         
             # Copyright (c) Jupyter Development Team.
             # Distributed under the terms of the Modified BSD License.
 License-File: LICENSE
-Keywords: ipython,jupyter
+Classifier: Framework :: Jupyter
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7
-Requires-Dist: jupyter-server-fileid<1,>=0.6.0
-Requires-Dist: jupyter-ydoc<0.4.0,>=0.2.0
-Requires-Dist: ypy-websocket<0.9.0,>=0.8.2
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Requires-Dist: jsonschema>=4.18.0
+Requires-Dist: jupyter-events>=0.10.0
+Requires-Dist: jupyter-server-fileid<1,>=0.7.0
+Requires-Dist: jupyter-server<3.0.0,>=2.4.0
+Requires-Dist: jupyter-ydoc<3.0.0,>=2.0.0
+Requires-Dist: pycrdt-websocket<0.13.0,>=0.12.5
 Provides-Extra: test
 Requires-Dist: coverage; extra == 'test'
-Requires-Dist: jupyter-server[test]>=2.0.0a0; extra == 'test'
+Requires-Dist: importlib-metadata>=4.8.3; (python_version < '3.10') and extra == 'test'
+Requires-Dist: jupyter-server-fileid[test]; extra == 'test'
+Requires-Dist: jupyter-server[test]>=2.4.0; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
-Requires-Dist: pytest-timeout; extra == 'test'
-Requires-Dist: pytest-tornasync; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
+Requires-Dist: websockets; extra == 'test'
 Description-Content-Type: text/markdown
 
-# Jupyter Server YDoc
+# jupyter-server-ydoc
 
-[![Build Status](https://github.com/jupyter-server/jupyter_server_ydoc/actions/workflows/test.yml/badge.svg?query=branch%3Amain++)](https://github.com/jupyter-server/jupyter_server_ydoc/actions?query=branch%3Amain++)
+jupyter-server extension integrating collaborative shared models.
 
-Jupyter Server YDoc is a Jupyter Server Extension providing support for Y documents.
-
-## Installation and Basic usage
-
-To install the latest release locally, make sure you have
-[pip installed](https://pip.readthedocs.io/en/stable/installing/) and run:
-
-    pip install jupyter_server_ydoc
-
-Jupyter Server YDoc currently supports Python>=3.6 on Linux, OSX and Windows.
-
-### Testing
-
-See [CONTRIBUTING](./CONTRIBUTING.rst#running-tests).
-
-## Contributing
-
-If you are interested in contributing to the project, see [CONTRIBUTING](./CONTRIBUTING.rst).
+The collaborative shared models are used for both:
+- real time collaboration, and
+- server-side execution of notebooks
```

