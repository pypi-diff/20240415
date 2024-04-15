# Comparing `tmp/ragdaemon-0.1.5.tar.gz` & `tmp/ragdaemon-0.1.6.tar.gz`

## Comparing `ragdaemon-0.1.5.tar` & `ragdaemon-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,61 @@
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/requirements.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/__init__.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/__main__.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/app.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/context.py
--rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/daemon.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/errors.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/llm.py
--rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/utils.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/__init__.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/base_annotator.py
--rw-r--r--   0        0        0     9485 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/chunker.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/chunker_line.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/chunker_llm.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/diff.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/hierarchy.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/annotators/layout_hierarchy.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/__init__.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/chroma_database.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/database.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/database/lite_database.py
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/favicon.ico
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/controlPanel.js
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/main.js
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/camera.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/controls.js
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/edge.js
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/node.js
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/raycaster.js
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/renderer.js
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/static/js/three/scene.js
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/templates/index.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/ragdaemon/templates/search_results.html
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/conftest.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_context.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_daemon.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_database.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/test_sample.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_chunker.py
--rw-r--r--   0        0        0     3968 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_diff.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_hierarchy.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/annotators/test_layout_hierarchy.py
--rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/chunker_graph.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/context_message.txt
--rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/diff_graph.json
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/hierarchy_graph.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/data/layout_hierarchy_graph.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/README.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/src/__init__.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/src/interface.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/tests/sample/src/operations.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/.gitignore
--rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/LICENSE
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/README.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 ragdaemon-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    30472 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/diff.txt
+-rw-r--r--   0        0        0    10345 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tutorial.ipynb
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/__init__.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/__main__.py
+-rw-r--r--   0        0        0     4228 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/app.py
+-rw-r--r--   0        0        0     7967 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/context.py
+-rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/daemon.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/errors.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/graph.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/llm.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/utils.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/__init__.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/base_annotator.py
+-rw-r--r--   0        0        0     9897 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/chunker.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/chunker_line.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/chunker_llm.py
+-rw-r--r--   0        0        0     6922 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/diff.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/hierarchy.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/annotators/layout_hierarchy.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/database/__init__.py
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/database/chroma_database.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/database/database.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/database/lite_database.py
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/favicon.ico
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/controlPanel.js
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/main.js
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/camera.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/controls.js
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/edge.js
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/node.js
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/raycaster.js
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/renderer.js
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/static/js/three/scene.js
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/templates/index.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/ragdaemon/templates/search_results.html
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/conftest.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/test_comments.py
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/test_context.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/test_daemon.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/test_database.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/test_sample.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/annotators/test_chunker.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/annotators/test_diff.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/annotators/test_hierarchy.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/annotators/test_layout_hierarchy.py
+-rw-r--r--   0        0        0     8870 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/data/chunker_graph.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/data/context_message.txt
+-rw-r--r--   0        0        0    11144 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/data/diff_graph.json
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/data/hierarchy_graph.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/data/layout_hierarchy_graph.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/sample/README.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/sample/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/sample/src/__init__.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/sample/src/interface.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/tests/sample/src/operations.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/README.md
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 ragdaemon-0.1.6/PKG-INFO
```

### Comparing `ragdaemon-0.1.5/ragdaemon/app.py` & `ragdaemon-0.1.6/ragdaemon/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import asyncio
 import socket
 import webbrowser
 from contextlib import asynccontextmanager
 from pathlib import Path
+from typing import Any
 
 import uvicorn
 from fastapi import FastAPI, Request
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from spice import Spice
 from starlette.templating import Jinja2Templates
@@ -82,20 +83,25 @@
 app.mount("/static", StaticFiles(directory=app_dir / "static"), name="static")
 templates = Jinja2Templates(directory=app_dir / "templates")
 
 
 @app.get("/", response_class=HTMLResponse)
 async def home(request: Request):
     # Serialize graph and send to frontend
-    nodes = [{"id": node, **data} for node, data in daemon.graph.nodes(data=True)]
-    edges = [
-        {"source": source, "target": target, **data}
-        for source, target, data in daemon.graph.edges(data=True)
+    nodes = [
+        {"id": node, **data} for node, data in daemon.graph.nodes(data=True) if data
     ]
-    metadata = daemon.graph.graph
+    edges = list[dict[str, Any]]()
+    for edge in daemon.graph.edges():
+        source = edge[0]
+        target = edge[1]
+        data = daemon.graph.get_edge_data(*edge)
+        if data:
+            edges.append({"source": source, "target": target, **data[0]})
+    metadata = dict(daemon.graph.graph)
     return templates.TemplateResponse(
         "index.html",
         {"request": request, "nodes": nodes, "edges": edges, "metadata": metadata},
     )
 
 
 @app.get("/search", response_class=HTMLResponse)
```

### Comparing `ragdaemon-0.1.5/ragdaemon/context.py` & `ragdaemon-0.1.6/ragdaemon/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,63 @@
 from pathlib import Path
-from typing import Any
-
-import networkx as nx
+from typing import Any, Optional
 
 from ragdaemon.annotators.diff import parse_diff_id
 from ragdaemon.database import Database
+from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import parse_path_ref
 
 
+from typing import Union, Dict
+from dict2xml import dict2xml
+
+NestedStrDict = Union[str, Dict[str, "NestedStrDict"]]
+
+
+class Comment:
+    def __init__(
+        self,
+        content: NestedStrDict,
+        tags: list[str] = [],
+    ):
+        self.content = content
+        self.tags = tags
+
+    def render(self) -> str:
+        return dict2xml(self.content, indent="    ")
+
+
+def render_comments(comments: list[Comment]) -> str:
+    return "\n".join(comment.render() for comment in comments)
+
+
 class ContextBuilder:
     """Renders items from a graph into an llm-readable string."""
 
-    def __init__(self, graph: nx.MultiDiGraph, db: Database, verbose: bool = False):
+    def __init__(self, graph: KnowledgeGraph, db: Database, verbose: bool = False):
         self.graph = graph
         self.db = db
         self.verbose = verbose
         self.context = dict[
             str, dict[str, Any]
         ]()  # {path: {lines, tags, document, diff}}
 
     def _add_path(self, path_str: str):
         """Create a new record in the context for the given path."""
-        cwd = self.graph.graph["cwd"]
         if path_str not in self.graph:  # e.g. deleted file
             document = ""
         else:
             checksum = self.graph.nodes[path_str]["checksum"]
             document = self.db.get(checksum)["documents"][0]
         message = {
             "lines": set(),
             "tags": set(),
             "document": document,
             "diffs": set(),
+            "comments": dict[int, list[Comment]](),
         }
         self.context[path_str] = message
 
     def add_ref(self, path_ref: str, tags: list[str] = []):
         """Manually include path_refs"""
         path, lines = parse_path_ref(path_ref)
         path_str = path.as_posix()
@@ -54,14 +76,46 @@
             return
         path_str = path.as_posix()
         if path_str not in self.context:
             self._add_path(path_str)
         self.context[path_str]["diffs"].add(id)
         self.context[path_str]["tags"].add("diff")
 
+    def add_comment(
+        self,
+        path_str: str,
+        comment: NestedStrDict,
+        line: Optional[int] = None,
+        tags: list[str] = [],
+    ):
+        path_str = Path(path_str).as_posix()
+        if not self.context.get(path_str):
+            self._add_path(path_str)
+        if not line:
+            line = 0  # file-level comment
+        self.context[path_str]["comments"].setdefault(line, []).append(
+            Comment(
+                content=comment,
+                tags=tags,
+            )
+        )
+
+    def remove_comments(self, path_str: str, tags: list[str] = []):
+        if path_str not in self.context:
+            if self.verbose:
+                print(f"Warning: no matching message found for {path_str}.")
+            return
+        if tags:
+            for line, comments in self.context[path_str]["comments"].items():
+                self.context[path_str]["comments"][line] = [
+                    comment for comment in comments if not set(tags) & set(comment.tags)
+                ]
+        else:
+            self.context[path_str]["comments"] = dict[int, list[Comment]]()
+
     def remove_ref(self, ref: str, tags: list[str] = []):
         """Remove the given id from the context."""
         path, lines = parse_path_ref(ref)
         path_str = path.as_posix()
         if path_str not in self.context:
             if self.verbose:
                 print(f"Warning: no matching message found for {path_str}.")
@@ -75,14 +129,16 @@
         if not self.context[path_str]["lines"] and not self.context[path_str]["diffs"]:
             del self.context[path_str]
         return ref
 
     def remove_diff(self, id: str):
         """Remove the given id from the context."""
         _, path, _ = parse_diff_id(id)
+        if not path:  # e.g. diff 'parent' nodes
+            return
         path_str = path.as_posix()
         if path_str not in self.context:
             if self.verbose:
                 print(f"Warning: no matching message found for {path_str}.")
             return
         self.context[path_str]["diffs"].remove(id)
         self.context[path_str]["tags"].remove("diff")
@@ -94,47 +150,51 @@
         """Return a formatted context message for the given nodes."""
         output = ""
         for path_str, data in self.context.items():
             if output:
                 output += "\n"
             tags = "" if not data["tags"] else f" ({', '.join(sorted(data['tags']))})"
             output += f"{path_str}{tags}\n"
+            if 0 in data["comments"]:
+                output += render_comments(data["comments"][0]) + "\n"
             if data["lines"]:
                 file_lines = data["document"].splitlines()
                 last_rendered = 0
                 for line in sorted(data["lines"]):
                     if line - last_rendered > 1:
                         output += "...\n"
-                    output += f"{line}:{file_lines[line]}\n"
+                    line_content = f"{line}:{file_lines[line]}"
+                    if line in data["comments"]:
+                        line_content += "\n" + render_comments(data["comments"][line])
+                    output += line_content + "\n"
                     last_rendered = line
                 if last_rendered < len(file_lines) - 1:
                     output += "...\n"
             if data["diffs"]:
                 output += self.render_diffs(data["diffs"])
         return output
 
     def render_diffs(self, ids: set[str]) -> str:
         output = ""
         diff_str, _, _ = parse_diff_id(next(iter(ids)))
         git_command = "--git diff"
         if diff_str != "DEFAULT":
             git_command += f" {diff_str}"
         output += f"{git_command}\n"
-        cwd = self.graph.graph["cwd"]
         for id in sorted(ids):
             checksum = self.graph.nodes[id]["checksum"]
             document = self.db.get(checksum)["documents"][0]
             # TODO: Add line numbers
             without_git_command = "\n".join(document.splitlines()[1:])
             output += without_git_command + "\n"
         return output
 
     def to_refs(self) -> list[str]:
         """Return a list of path:interval,interval for everything in current context."""
-        refs = dict[Path, str]()
+        refs = dict[str, str]()
         for path, data in self.context.items():
             if len(data["lines"]) == 0:
                 continue
             elif len(data["lines"]) == data["document"].splitlines():
                 refs[path] = ""
                 continue
             segments = []
```

### Comparing `ragdaemon-0.1.5/ragdaemon/daemon.py` & `ragdaemon-0.1.6/ragdaemon/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
 import json
 import time
 from pathlib import Path
 from typing import Any, Optional
 
-import networkx as nx
+from networkx.readwrite import json_graph
 from spice import Spice
 
 from ragdaemon.annotators import Annotator, annotators_map
 from ragdaemon.context import ContextBuilder
 from ragdaemon.database import DEFAULT_EMBEDDING_MODEL, Database, get_db
+from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
 from ragdaemon.utils import get_non_gitignored_files
 
 
 def default_annotators():
     return {
         "hierarchy": {},
@@ -21,16 +22,16 @@
         "diff": {},
     }
 
 
 class Daemon:
     """Build and maintain a searchable knowledge graph of codebase."""
 
-    graph: nx.MultiDiGraph
-    db: Database = None
+    graph: KnowledgeGraph
+    _db: Database
 
     def __init__(
         self,
         cwd: Path,
         annotators: Optional[dict[str, dict]] = None,
         verbose: bool = False,
         graph_path: Optional[Path] = None,
@@ -51,51 +52,51 @@
                 default_embeddings_model=DEFAULT_EMBEDDING_MODEL,
             )
         self.spice_client = spice_client
         self.model = model
         self.provider = provider
 
         # Initialize an empty graph
-        self.graph = nx.MultiDiGraph()
+        self.graph = KnowledgeGraph()
         self.graph.graph["cwd"] = self.cwd.as_posix()
         if self.verbose:
             print("Initialized empty graph.")
 
         annotators = annotators if annotators is not None else default_annotators()
         if self.verbose:
             print(f"Initializing annotators: {list(annotators.keys())}...")
         self.pipeline: dict[str, Annotator] = {
             ann: annotators_map[ann](
                 **kwargs, verbose=self.verbose, spice_client=spice_client
             )
             for ann, kwargs in annotators.items()
         }
 
+    @property
+    def db(self) -> Database:
+        if not hasattr(self, "_db"):
+            self._db = get_db(
+                self.cwd,
+                spice_client=self.spice_client,
+                model=self.model,
+                provider=self.provider,
+            )
+        return self._db
+
     def save(self):
         """Saves the graph to disk."""
-        data = nx.readwrite.json_graph.node_link_data(self.graph)
+        data = json_graph.node_link_data(self.graph)
         with open(self.graph_path, "w") as f:
             json.dump(data, f, indent=4)
         if self.verbose:
             print(f"Saved updated graph to {self.graph_path}")
 
     async def update(self, refresh=False):
         """Iteratively build the knowledge graph"""
-
-        # Establish a dedicated database client for this instance
-        if self.db is None:
-            self.db = get_db(
-                self.cwd,
-                spice_client=self.spice_client,
-                model=self.model,
-                provider=self.provider,
-            )
-
         _graph = self.graph.copy()
-        self.graph.graph["refreshing"] = True
         for annotator in self.pipeline.values():
             if refresh or not annotator.is_complete(_graph, self.db):
                 _graph = await annotator.annotate(_graph, self.db, refresh=refresh)
         self.graph = _graph
         self.save()
 
     async def watch(self, interval=2, debounce=5):
```

### Comparing `ragdaemon-0.1.5/ragdaemon/utils.py` & `ragdaemon-0.1.6/ragdaemon/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,16 @@
         else:
             lines.add(int(ref))
     return lines or None
 
 
 def parse_path_ref(ref: str) -> tuple[Path, set[int] | None]:
     match = re.match(r"^(.*?)(?::([0-9,\-]+))?$", ref)
+    if not match:
+        return Path(ref), None
     groups = match.groups()
     if len(groups) == 2 and all(groups):
         path_str, lines_ref = match.group(1), match.group(2)
         lines = parse_lines_ref(lines_ref)
     else:
         path_str, lines = ref, None
     return Path(path_str), lines
@@ -85,15 +87,15 @@
 def get_document(ref: str, cwd: Path, type: str = "file") -> str:
     if type == "diff":
         if ":" in ref:
             diff_ref, lines_ref = ref.split(":", 1)
             lines = parse_lines_ref(lines_ref)
         else:
             diff_ref, lines = ref, None
-        diff = get_git_diff(diff_ref, cwd)
+        diff = get_git_diff(diff_ref, str(cwd))
         if lines:
             text = "\n".join(
                 [line for i, line in enumerate(diff.split("\n")) if i + 1 in lines]
             )
         else:
             text = diff
         ref = f"git diff{'' if diff_ref == 'DEFAULT' else f' {diff_ref}'}"
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/__init__.py` & `ragdaemon-0.1.6/ragdaemon/annotators/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/base_annotator.py` & `ragdaemon-0.1.6/ragdaemon/annotators/base_annotator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-import networkx as nx
+from typing import Optional
+
 from spice import Spice
 
 from ragdaemon.database import Database
+from ragdaemon.graph import KnowledgeGraph
 
 
 class Annotator:
     name: str = "base_annotator"
 
-    def __init__(self, verbose: bool = False, spice_client: Spice = None):
+    def __init__(self, verbose: bool = False, spice_client: Optional[Spice] = None):
         self.verbose = verbose
         self.spice_client = spice_client
         pass
 
-    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
+    def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         raise NotImplementedError()
 
     async def annotate(
-        self, graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
-    ) -> nx.MultiDiGraph:
+        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+    ) -> KnowledgeGraph:
         raise NotImplementedError()
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/chunker.py` & `ragdaemon-0.1.6/ragdaemon/annotators/chunker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Chunk data a list of objects following [
-    {id: path/to/file:class.method, start_line: int, end_line: int} 
+    {id: path/to/file:class.method, start_line: int, end_line: int}
 ]
 
 It's stored on the file node as data['chunks'] and json.dumped into the database.
 
 A chunker annotator:
 1. Is complete when all files (with matching extensions) have a 'chunks' field
 2. Generates chunks using a subclass method (llm, ctags..)
@@ -14,20 +14,22 @@
 
 The Chunker base class below handles everything except step 2.
 """
 
 import asyncio
 import json
 from pathlib import Path
+from typing import Any, Coroutine, Callable, Optional
 
-import networkx as nx
 from tqdm.asyncio import tqdm
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import Database
+from ragdaemon.graph import KnowledgeGraph
+from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import get_document, hash_str
 
 
 def is_chunk_valid(chunk: dict) -> bool:
     # Includes the correct fields
     if not set(chunk.keys()) == {"id", "start_line", "end_line"}:
         return False
@@ -39,29 +41,36 @@
         return False
     # TODO: Validate the ref, i.e. a parent chunk exists
 
     return True
 
 
 async def get_file_chunk_data(
-    cwd, node, data, chunk_function: callable, db: Database, verbose: bool = False
-) -> list[dict]:
+    cwd,
+    node,
+    data,
+    chunk_function: Callable[
+        [str, list[str], bool], Coroutine[Any, Any, list[dict[str, str]]]
+    ],
+    db: Database,
+    verbose: bool = False,
+):
     """Get or add chunk data to database, load into file data"""
     file_lines = (cwd / Path(node)).read_text().splitlines()
     if len(file_lines) == 0:
         chunks = []
     else:
         chunks = await chunk_function(node, file_lines, verbose)
         if not all(is_chunk_valid(chunk) for chunk in chunks):
             raise ValueError(f"Invalid chunk data: {chunks}")
     if chunks:
         # Generate a 'BASE chunk' with all lines not already part of a chunk
         base_chunk_lines = set(range(1, len(file_lines) + 1))
         for chunk in chunks:
-            for i in range(chunk["start_line"], chunk["end_line"] + 1):
+            for i in range(int(chunk["start_line"]), int(chunk["end_line"]) + 1):
                 base_chunk_lines.discard(i)
         if len(base_chunk_lines) > 0:
             base_chunk_lines_sorted = sorted(list(base_chunk_lines))
             base_chunk_refs = []
             start = base_chunk_lines_sorted[0]
             end = start
             for i in base_chunk_lines_sorted[1:]:
@@ -92,36 +101,35 @@
     db.update(data["checksum"], metadatas=metadatas)
     data["chunks"] = chunks
 
 
 def add_file_chunks_to_graph(
     file: str,
     data: dict,
-    graph: nx.MultiDiGraph,
+    graph: KnowledgeGraph,
     db: Database,
     refresh: bool = False,
     verbose: bool = False,
-) -> dict[str:list]:
+) -> dict[str, list[Any]]:
     """Load chunks from file data into db/graph"""
-    cwd = Path(graph.graph["cwd"])
     add_to_db = {"ids": [], "documents": [], "metadatas": []}
     if not isinstance(data["chunks"], list):
         data["chunks"] = json.loads(data["chunks"])
     chunks = data["chunks"]
     if not refresh and len(data["chunks"]) == 0:
         return add_to_db
     edges_to_add = set()
     base_id = f"{file}:BASE"
     edges_to_add.add((file, base_id))
     for chunk in chunks:
         try:
             # Get the checksum record from database
             id = chunk["id"]
             ref = chunk["ref"]
-            document = get_document(ref, cwd)
+            document = get_document(ref, Path(graph.graph["cwd"]))
             checksum = hash_str(document)
             records = db.get(checksum)["metadatas"]
             if not refresh and len(records) > 0:
                 record = records[0]
             else:
                 record = {
                     "id": id,
@@ -158,15 +166,15 @@
         graph.add_edge(source, origin, type="hierarchy")
     return add_to_db
 
 
 class Chunker(Annotator):
     name = "chunker"
 
-    def __init__(self, *args, chunk_extensions: list[str] = None, **kwargs):
+    def __init__(self, *args, chunk_extensions: Optional[list[str]] = None, **kwargs):
         super().__init__(*args, **kwargs)
         if chunk_extensions is None:
             chunk_extensions = [
                 ".py",
                 ".js",
                 ".java",
                 ".html",
@@ -184,16 +192,18 @@
                 ".ts",
                 ".jsx",
                 ".tsx",
                 ".scss",
             ]
         self.chunk_extensions = chunk_extensions
 
-    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
-        for _, data in graph.nodes(data=True):
+    def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
+        for node, data in graph.nodes(data=True):
+            if data is None:
+                raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") != "file":
                 continue
             chunks = data.get("chunks", None)
             if chunks is None:
                 if self.chunk_extensions is None:
                     return False
                 extension = Path(data["ref"]).suffix
@@ -204,15 +214,15 @@
                     chunks = json.loads(chunks)
                 for chunk in chunks:
                     if chunk["id"] not in graph:
                         return False
         return True
 
     async def chunk_file(
-        self, file: str, file_lines: str, verbose: bool = False
+        self, file: str, file_lines: list[str], verbose: bool
     ) -> list[dict[str, str]]:
         """Return a list of {id, start_line, end_line}'s for the given file.
 
         Args:
             file (str): The file name
             file_lines (list[str]): The file content as a list of lines
 
@@ -220,26 +230,28 @@
             id (str): The complete call path, e.g. `path/to/file:class.method`
             start_line (int): Where the function, class or method begins
             end_line (int): Where it ends - INCLUSIVE
         """
         raise NotImplementedError()
 
     async def annotate(
-        self, graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
-    ) -> nx.MultiDiGraph:
+        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+    ) -> KnowledgeGraph:
         # Remove any existing chunk nodes from the graph
         for node, data in graph.nodes(data=True):
+            if data is None:
+                raise RagdaemonError(f"Node {node} has no data.")
             if data.get("type") == "chunk":
                 graph.remove_node(node)
 
         cwd = Path(graph.graph["cwd"])
         file_nodes = [
             (file, data)
             for file, data in graph.nodes(data=True)
-            if data.get("type") == "file"
+            if data is not None and data.get("type") == "file"
         ]
         if self.chunk_extensions is not None:
             file_nodes = [
                 (file, data)
                 for file, data in file_nodes
                 if Path(data["ref"]).suffix in self.chunk_extensions
             ]
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/chunker_line.py` & `ragdaemon-0.1.6/ragdaemon/annotators/chunker_line.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,27 @@
     name = "chunker_line"
 
     def __init__(self, *args, lines_per_chunk=50, **kwargs):
         super().__init__(*args, **kwargs)
         self.n = lines_per_chunk
 
     async def chunk_file(
-        self, file_id: str, file_lines: list[str], verbose=False
+        self, file: str, file_lines: list[str], verbose: bool
     ) -> list[dict[str, str]]:
         """Split text files into chunks N lines long.
 
         Chunker.annotate will generate a 'BASE' chunk from the lines
         not assigned to chunks as a hierarchical root of all chunks.
         Here we set aside the first N lines as the BASE chunk.
         """
         if len(file_lines) < self.n:
             return []
-        chunks = []
+        chunks = list[dict[str, str]]()
         for i, start_line in enumerate(range(self.n, len(file_lines), self.n)):
             chunks.append(
                 {
-                    "id": f"{file_id}:chunk_{i + 1}",
-                    "start_line": start_line,
-                    "end_line": min(start_line + self.n - 1, len(file_lines)),
+                    "id": f"{file}:chunk_{i + 1}",
+                    "start_line": str(start_line),
+                    "end_line": str(min(start_line + self.n - 1, len(file_lines))),
                 }
             )
         return chunks
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/chunker_llm.py` & `ragdaemon-0.1.6/ragdaemon/annotators/chunker_llm.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import asyncio
 import json
 
 from ragdaemon.annotators.chunker import Chunker, is_chunk_valid
+from ragdaemon.errors import RagdaemonError
+from spice import SpiceMessage
 
 chunker_prompt = """\
 Split the provided code file into chunks.
 Return a list of functions, classes and methods in this code file as JSON data.
 Each item in the list should contain:
 1. `id` - the complete call path, e.g. `path/to/file:class.method`
 2. `start_line` - where the function, class or method begins
@@ -14,69 +16,70 @@
 If there are no chunks, return an empty list.
 
 EXAMPLE:
 --------------------------------------------------------------------------------
 src/graph.py
 1:import pathlib as Path
 2:
-3:import networkx as nx
-4:
-5:
-6:class KnowledgeGraph:
-7:    def __init__(self, cwd: Path):
-8:        self.cwd = cwd
-9:
-10:_knowledge_graph = None
-11:def get_knowledge_graph():
-12:    global _knowledge_graph
-13:    if _knowledge_graph is None:
-14:        _knowledge_graph = KnowledgeGraph(Path.cwd())
-15:    return _knowledge_graph
-16:
+3:
+4:class KnowledgeGraph:
+5:    def __init__(self, cwd: Path):
+6:        self.cwd = cwd
+7:
+8:_knowledge_graph = None
+9:def get_knowledge_graph():
+10:    global _knowledge_graph
+11:    if _knowledge_graph is None:
+12:        _knowledge_graph = KnowledgeGraph(Path.cwd())
+13:    return _knowledge_graph
+14:
 
 RESPONSE:
 {
     "chunks": [
-        {"id": "src/graph.py:KnowledgeGraph", "start_line": 6, "end_line": 8},
-        {"id": "src/graph.py:KnowledgeGraph.__init__", "start_line": 7, "end_line": 8},
-        {"id": "src/graph.py:get_knowledge_graph", "start_line": 11, "end_line": 15}
+        {"id": "src/graph.py:KnowledgeGraph", "start_line": 4, "end_line": 6},
+        {"id": "src/graph.py:KnowledgeGraph.__init__", "start_line": 5, "end_line": 6},
+        {"id": "src/graph.py:get_knowledge_graph", "start_line": 9, "end_line": 13}
     ]
 }
 --------------------------------------------------------------------------------
 """
 
 
 semaphore = asyncio.Semaphore(50)
 
 
 class ChunkerLLM(Chunker):
     name = "chunker_llm"
 
     async def get_llm_response(self, file_message: str) -> dict:
+        if self.spice_client is None:
+            raise RagdaemonError("Spice client is not initialized.")
         global semaphore
         async with semaphore:
-            messages = [
+            messages: list[SpiceMessage] = [
                 {"role": "system", "content": chunker_prompt},
                 {"role": "user", "content": file_message},
             ]
             response = await self.spice_client.get_response(
                 messages=messages,
                 response_format={"type": "json_object"},
             )
             return json.loads(response.text)
 
     async def chunk_file(
-        self, file_id: str, file_lines: list[str], verbose=False, tries=1
+        self, file: str, file_lines: list[str], verbose: bool
     ) -> list[dict[str, str]]:
+        tries: int = 1
         for tries in range(tries, 0, -1):
             tries -= 1
             numbered_lines = "\n".join(
                 f"{i+1}:{line}" for i, line in enumerate(file_lines)
             )
-            file_message = f"{file_id}\n{numbered_lines}"
+            file_message = f"{file}\n{numbered_lines}"
             response = await self.get_llm_response(file_message)
             chunks = response.get("chunks", [])
             if not chunks or all(is_chunk_valid(chunk) for chunk in chunks):
                 return chunks
             if tries > 1 and verbose:
                 print(f"Error with chunker response:\n{response}.\n{tries} tries left.")
         return []
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/diff.py` & `ragdaemon-0.1.6/ragdaemon/annotators/diff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import json
 import re
 from pathlib import Path
 
-import networkx as nx
 from spice import Spice
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import (
     DEFAULT_EMBEDDING_MODEL,
     MAX_TOKENS_PER_EMBEDDING,
     Database,
 )
+from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.utils import get_document, hash_str, parse_path_ref
 
 
-def get_chunks_from_diff(id: str, diff: str) -> list[dict[str, str]]:
+def get_chunks_from_diff(id: str, diff: str) -> dict[str, str]:
     # Match files and line numbers
     file_regex = re.compile(r"^diff --git a/(.+) b/(.+)$")
     hunk_header_regex = re.compile(r"^@@ -\d+,\d+ \+(\d+),(\d+) @@.*$")
 
     chunks = {}
     file = None
-    chunk_id = None
+    i = None
+    chunk_id: str | None = None
     chunk_ref_start = None
     for i, line in enumerate(diff.split("\n")):
         file_match = file_regex.match(line)
         hunk_header_match = hunk_header_regex.match(line)
         if (file_match or hunk_header_match) and (
             file and chunk_id and chunk_ref_start
         ):
@@ -45,23 +46,23 @@
             if end_line > start_line:
                 lines_ref = f":{start_line}-{end_line}"
             elif end_line == start_line:
                 lines_ref = f":{start_line}"
             else:
                 lines_ref = ""
             chunk_id = f"{id}:{file}{lines_ref}"
-    if file and chunk_id and chunk_ref_start:
+    if i and file and chunk_id and chunk_ref_start:
         chunk_ref_end = i
         chunk_ref = f"{id}:{chunk_ref_start}-{chunk_ref_end}"
         chunks[chunk_id] = chunk_ref
 
     return chunks
 
 
-def parse_diff_id(id: str) -> tuple[str, Path, set[int] | None]:
+def parse_diff_id(id: str) -> tuple[str, Path | None, set[int] | None]:
     if ":" in id:
         diff_ref, path_ref = id.split(":", 1)
         path, lines = parse_path_ref(path_ref)
     else:
         diff_ref, path, lines = id, None, None
     return diff_ref, path, lines
 
@@ -75,28 +76,30 @@
         super().__init__(*args, **kwargs)
         self.diff_args = diff
 
     @property
     def id(self) -> str:
         return "DEFAULT" if not self.diff_args else self.diff_args
 
-    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
-        cwd = graph.graph["cwd"]
+    def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
+        cwd = Path(graph.graph["cwd"])
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
         return self.id in graph and graph.nodes[self.id]["checksum"] == checksum
 
     async def annotate(
-        self, graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
-    ) -> nx.MultiDiGraph:
+        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+    ) -> KnowledgeGraph:
         graph_nodes = {
-            node for node, data in graph.nodes(data=True) if data.get("type") == "diff"
+            node
+            for node, data in graph.nodes(data=True)
+            if data and data.get("type") == "diff"
         }
         graph.remove_nodes_from(graph_nodes)
-        cwd = graph.graph["cwd"]
+        cwd = Path(graph.graph["cwd"])
         document = get_document(self.diff_args, cwd, type="diff")
         checksum = hash_str(document)
         existing_records = db.get(checksum)
         if refresh or len(existing_records["ids"]) == 0:
             chunks = get_chunks_from_diff(id=self.id, diff=document)
             data = {
                 "id": self.id,
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/hierarchy.py` & `ragdaemon-0.1.6/ragdaemon/annotators/hierarchy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import fnmatch
 from pathlib import Path
 
-import networkx as nx
 from spice import Spice
 
 from ragdaemon.annotators.base_annotator import Annotator
 from ragdaemon.database import MAX_TOKENS_PER_EMBEDDING, Database
+from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.errors import RagdaemonError
 from ragdaemon.llm import DEFAULT_COMPLETION_MODEL
 from ragdaemon.utils import get_document, get_non_gitignored_files, hash_str
 
 
 def match_path_with_patterns(path: Path, cwd: Path, patterns: list[str] = []) -> bool:
     """Check if the given absolute path matches any of the patterns.
@@ -38,16 +38,16 @@
 
 def get_active_checksums(
     cwd: Path,
     db: Database,
     refresh: bool = False,
     verbose: bool = False,
     ignore_patterns: list[str] = [],
-) -> dict[Path:str]:
-    checksums: dict[Path:str] = {}
+) -> dict[Path, str]:
+    checksums: dict[Path, str] = {}
     git_paths = get_non_gitignored_files(cwd)
     add_to_db = {
         "ids": [],
         "documents": [],
         "metadatas": [],
     }
     for path in git_paths:
@@ -100,36 +100,36 @@
 class Hierarchy(Annotator):
     name = "hierarchy"
 
     def __init__(self, *args, ignore_patterns: list[str] = [], **kwargs):
         self.ignore_patterns = ignore_patterns
         super().__init__(*args, **kwargs)
 
-    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
+    def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         cwd = Path(graph.graph["cwd"])
         return graph.graph.get("files_checksum") == files_checksum(
             cwd, self.ignore_patterns
         )
 
     async def annotate(
-        self, old_graph: nx.MultiDiGraph, db: Database = None, refresh: bool = False
-    ) -> nx.MultiDiGraph:
+        self, graph: KnowledgeGraph, db: Database, refresh: bool = False
+    ) -> KnowledgeGraph:
         """Build a graph of active files and directories with hierarchy edges."""
-        cwd = Path(old_graph.graph["cwd"])
+        cwd = Path(graph.graph["cwd"])
         checksums = get_active_checksums(
             cwd,
             db,
             refresh=refresh,
             verbose=self.verbose,
             ignore_patterns=self.ignore_patterns,
         )
         _files_checksum = files_checksum(cwd, self.ignore_patterns)
 
         # Initialize an empty graph. We'll build it from scratch.
-        graph = nx.MultiDiGraph()
+        graph = KnowledgeGraph()
         graph.graph["cwd"] = str(cwd)
         edges_to_add = set()
         for path, checksum in checksums.items():
             # add db reecord
             id = path.as_posix()
             results = db.get(checksum)
             data = results["metadatas"][0]
```

### Comparing `ragdaemon-0.1.5/ragdaemon/annotators/layout_hierarchy.py` & `ragdaemon-0.1.6/ragdaemon/annotators/layout_hierarchy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import networkx as nx
 import numpy as np
 from tqdm import tqdm
 
-from ragdaemon.database import Database
 from ragdaemon.annotators.base_annotator import Annotator
+from ragdaemon.database import Database
+from ragdaemon.graph import KnowledgeGraph
+from ragdaemon.errors import RagdaemonError
 
 
 def fruchterman_reingold_3d(
     G,
     iterations=40,
     repulsive_force=0.2,
     spring_length=0.2,
@@ -80,28 +81,30 @@
         for node in G.nodes()
     }
 
 
 class LayoutHierarchy(Annotator):
     name = "layout_hierarchy"
 
-    def is_complete(self, graph: nx.MultiDiGraph, db: Database = None) -> bool:
+    def is_complete(self, graph: KnowledgeGraph, db: Database) -> bool:
         # Check that they have data.layout.hierarchy
-        for _, data in graph.nodes(data=True):
+        for node, data in graph.nodes(data=True):
+            if data is None:
+                raise RagdaemonError(f"Node {node} has no data.")
             if not data.get("layout", {}).get("hierarchy"):
                 return False
         return True
 
     async def annotate(
         self,
-        graph: nx.MultiDiGraph,
-        db: Database = None,
+        graph: KnowledgeGraph,
+        db: Database,
         refresh: bool = False,
         iterations: int = 40,
-    ) -> nx.MultiDiGraph:
+    ) -> KnowledgeGraph:
         """
         a. Regenerate x/y/z for all nodes
         b. Update all nodes
         c. Save to chroma
         """
         pos = fruchterman_reingold_3d(
             graph, iterations=iterations, verbose=self.verbose
```

### Comparing `ragdaemon-0.1.5/ragdaemon/database/__init__.py` & `ragdaemon-0.1.6/ragdaemon/database/__init__.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/database/database.py` & `ragdaemon-0.1.6/ragdaemon/database/database.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,58 +1,36 @@
 from pathlib import Path
 from typing import Optional
 
-import networkx as nx
+from ragdaemon.graph import KnowledgeGraph
 
 
 class Database:
     _collection = None  # Collection | LiteDB
 
     def __init__(self, cwd: Path, db_path: Path) -> None:
         raise NotImplementedError
 
     def __getattr__(self, name):
         """Delegate attribute access to the collection."""
         return getattr(self._collection, name)
 
+    def query(self, query: str, active_checksums: list[str]) -> list[dict]:
+        raise NotImplementedError
+
     def query_graph(
-        self, query: str, graph: nx.MultiDiGraph, n: Optional[int] = None
+        self, query: str, graph: KnowledgeGraph, n: Optional[int] = None
     ) -> list[dict]:
         """Return documents, metadatas and distances, sorted, for nodes in the graph.
 
         Chroma's default search covers all records, including inactive ones, so we
         manually flag the active records, query them, and then unflag them.
         """
-        metadatas = self._collection.get(
-            [
-                data["checksum"]
-                for _, data in graph.nodes(data=True)
-                if "checksum" in data
-            ]
-        )["metadatas"]
-        metadatas = [{**data, "active": True} for data in metadatas]
-        if len(metadatas) == 0:
-            return []
-        self._collection.update(
-            ids=[m["checksum"] for m in metadatas], metadatas=metadatas
-        )
-        response = self._collection.query(
-            query_texts=query,
-            where={"active": True},
-            n_results=len(metadatas),
-        )
-        metadatas = [{**data, "active": False} for data in metadatas]
-        self._collection.update(
-            ids=[m["checksum"] for m in metadatas], metadatas=metadatas
-        )
-        results = [
-            {**data, "document": document, "distance": distance}
-            for data, document, distance in zip(
-                response["metadatas"][0],
-                response["documents"][0],
-                response["distances"][0],
-            )
+        active_checksums = [
+            data["checksum"]
+            for _, data in graph.nodes(data=True)
+            if data and "checksum" in data
         ]
-        results = sorted(results, key=lambda x: x["distance"])
+        results = self.query(query, active_checksums)
         if n:
             results = results[:n]
         return results
```

### Comparing `ragdaemon-0.1.5/ragdaemon/database/lite_database.py` & `ragdaemon-0.1.6/ragdaemon/database/lite_database.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 
 class LiteDB(Database):
     def __init__(self, cwd: Path, db_path: Path):
         self.cwd = cwd
         self.db_path = db_path
         self._collection = LiteCollection()
 
+    def query(self, query: str, active_checksums: list[str]) -> list[dict]:
+        response = self._collection.query(query, active_checksums)
+        results = [
+            {**data, "document": document, "distance": distance}
+            for data, document, distance in zip(
+                response["metadatas"][0],
+                response["documents"][0],
+                response["distances"][0],
+            )
+        ]
+        results = sorted(results, key=lambda x: x["distance"])
+        return results
+
 
 class LiteCollection:
     """A fast alternative to ChromaDB for testing (and anything else).
 
     Matches the chroma Collection API except:
     - No embeddings
     - In-memory
@@ -42,68 +55,56 @@
         ids = [ids] if isinstance(ids, str) else ids
         metadatas = [metadatas] if isinstance(metadatas, dict) else metadatas
         for checksum, metadata in zip(ids, metadatas):
             if checksum not in self.data:
                 raise ValueError(f"Record {checksum} does not exist.")
             self.data[checksum]["metadatas"] = metadata
 
-    def query(self, query_texts: list[str] | str, where: dict, n_results: int) -> dict:
+    def query(self, query: str, active_checksums: list[str]) -> dict[str, list[Any]]:
         # Select active/filtered records
-        records = [{"id": id, **data} for id, data in self.data.items()]
-        if where:
-            filtered_records = list[dict[str, Any]]()
-            for record in records:
-                selected = all(
-                    record.get("metadatas", {}).get(key) == value
-                    for key, value in where.items()
-                )
-                if selected:
-                    filtered_records.append(record)
-            records = filtered_records
-        if not query_texts:
+        records = [
+            {"id": k, **v} for k, v in self.data.items() if k in active_checksums
+        ]
+        if not query:
             return {
                 "ids": [r["id"] for r in records],
                 "metadatas": [r["metadatas"] for r in records],
                 "documents": [r["document"] for r in records],
                 "distances": [0] * len(records),
             }
-        if isinstance(query_texts, str):
-            query_texts = [query_texts]
 
         # Pull out some fields to string match against
-        strings_to_compare = dict[str, list[tuple[str, float]]]()
+        strings_to_compare = dict[str, list[tuple]]()
         for record in records:
             stc = list[tuple]()  # string, category_weight
             data = record["metadatas"]
             if data["type"] == "diff" and ":" in data["ref"]:
                 path = Path(data["ref"].split(":")[1])
             else:
                 path, _ = parse_path_ref(data["ref"])
             stc.append((path.name, 2))
             stc.append((path.as_posix(), 1))
             stc.append((record["document"], 0.5))
             strings_to_compare[record["id"]] = stc
 
         output = {"ids": [], "metadatas": [], "documents": [], "distances": []}
-        for text in query_texts:
-            # Compare each query text against each records' strings
-            distances = list[tuple[str, float]]()
-            for id, stc in strings_to_compare.items():
-                score = 0
-                for string, weight in stc:
-                    if string in text or text in string:
-                        score += weight
-                distance = 10 if not score else 1 / score
-                distances.append((id, distance))
-            # Sort by distance
-            ids, distances = zip(*sorted(distances, key=lambda x: x[1]))
-            output["ids"].append(ids)
-            output["metadatas"].append([self.data[id]["metadatas"] for id in ids])
-            output["documents"].append([self.data[id]["document"] for id in ids])
-            output["distances"].append(distances)
+        distances = list[tuple[str, float]]()
+        for id, stc in strings_to_compare.items():
+            score = 0
+            for string, weight in stc:
+                if string in query or query in string:
+                    score += weight
+            distance = 10 if not score else 1 / score
+            distances.append((id, distance))
+        # Sort by distance
+        ids, distances = zip(*sorted(distances, key=lambda x: x[1]))
+        output["ids"].append(ids)
+        output["metadatas"].append([self.data[id]["metadatas"] for id in ids])
+        output["documents"].append([self.data[id]["document"] for id in ids])
+        output["distances"].append(distances)
 
         return output
 
     def upsert(
         self,
         ids: list[str] | str,
         metadatas: list[dict] | dict,
```

### Comparing `ragdaemon-0.1.5/ragdaemon/static/favicon.ico` & `ragdaemon-0.1.6/ragdaemon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/static/js/controlPanel.js` & `ragdaemon-0.1.6/ragdaemon/static/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/static/js/main.js` & `ragdaemon-0.1.6/ragdaemon/static/js/main.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/static/js/three/edge.js` & `ragdaemon-0.1.6/ragdaemon/static/js/three/edge.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/static/js/three/node.js` & `ragdaemon-0.1.6/ragdaemon/static/js/three/node.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/static/js/three/raycaster.js` & `ragdaemon-0.1.6/ragdaemon/static/js/three/raycaster.js`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/ragdaemon/templates/index.html` & `ragdaemon-0.1.6/ragdaemon/templates/index.html`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/conftest.py` & `ragdaemon-0.1.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/test_context.py` & `ragdaemon-0.1.6/tests/test_context.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from pathlib import Path
 
-import networkx as nx
-
 from ragdaemon.context import ContextBuilder
+from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import get_document
 
 
 def test_daemon_render_context(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Base Chunk
-    context = ContextBuilder(nx.MultiDiGraph(), mock_db)
+    context = ContextBuilder(KnowledgeGraph(), mock_db)
     context.context = {
         path_str: {
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
+            "comments": dict(),
         }
     }
     actual = context.render()
     assert (
         actual
         == """\
 src/interface.py (test-flag)
@@ -38,47 +38,49 @@
     # Function Chunk
     context.context = {
         path_str: {
             "lines": set([5, 6, 7, 8, 9, 10, 11, 12, 13, 14]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
+            "comments": dict(),
         }
     }
     actual = context.render()
     assert (
         actual
         == """\
 src/interface.py (test-flag)
 ...
 5:def parse_arguments():
 6:    parser = argparse.ArgumentParser(description="Basic Calculator")
 7:    parser.add_argument("operation", type=str, help="Calculation operation")
 8:    args = parser.parse_args()
 9:
 10:    # use re to parse symbol, nubmer before, nubmer after
-11:    match = re.match(r"(\d+)(\D)(\d+)", args.operation)
+11:    match = re.match(r"(\\d+)(\\D)(\\d+)", args.operation)
 12:    if match is None:
 13:        raise ValueError("Invalid operation")
 14:    return int(match.group(1)), match.group(2), int(match.group(3))
 ...
 """
     )
 
 
 def test_to_refs(cwd, mock_db):
     path_str = Path("src/interface.py").as_posix()
     ref = path_str
 
     # Setup Context
-    context = ContextBuilder(nx.MultiDiGraph(), mock_db)
+    context = ContextBuilder(KnowledgeGraph(), mock_db)
     context.context = {
         path_str: {
             "lines": set([1, 2, 3, 4, 15]),
             "tags": ["test-flag"],
             "document": get_document(ref, cwd),
             "diffs": set(),
+            "comments": dict(),
         }
     }
     expected_refs = [f"{path_str}:1-4,15-15"]
     actual_refs = context.to_refs()
     assert actual_refs == expected_refs, f"Expected {expected_refs}, got {actual_refs}"
```

### Comparing `ragdaemon-0.1.5/tests/test_daemon.py` & `ragdaemon-0.1.6/tests/test_daemon.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,27 +13,27 @@
 @pytest.mark.asyncio
 async def test_daemon_get_context(cwd):
     # Full Context
     annotators = default_annotators()
     del annotators["diff"]
     daemon = Daemon(cwd.resolve(), annotators=annotators)
     await daemon.update()
-    actual = daemon.get_context("test", max_tokens=1e6).render()
+    actual = daemon.get_context("test", max_tokens=1000).render()
 
     with open("tests/data/context_message.txt", "r") as f:
         expected = f.read()
     assert get_message_chunk_set(actual) == get_message_chunk_set(expected)
 
     # Included Files
     context = daemon.get_context("test")
     context.add_ref("src/interface.py:11-12", tags=["user-included"])
     actual = daemon.get_context("test", context_builder=context, auto_tokens=0).render()
     assert (
         actual
         == """\
 src/interface.py (user-included)
 ...
-11:    match = re.match(r"(\d+)(\D)(\d+)", args.operation)
+11:    match = re.match(r"(\\d+)(\\D)(\\d+)", args.operation)
 12:    if match is None:
 ...
 """
     )
```

### Comparing `ragdaemon-0.1.5/tests/test_sample.py` & `ragdaemon-0.1.6/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/annotators/test_chunker.py` & `ragdaemon-0.1.6/tests/annotators/test_chunker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,56 @@
-import json
 from pathlib import Path
 from unittest.mock import AsyncMock
 
-import networkx as nx
 import pytest
 
 from ragdaemon.annotators import Chunker, ChunkerLLM
 from ragdaemon.daemon import Daemon
+from ragdaemon.graph import KnowledgeGraph
 
 
-def test_chunker_is_complete(cwd):
+def test_chunker_is_complete(cwd, mock_db):
     chunker = Chunker()
 
-    empty_graph = nx.MultiDiGraph()
-    assert chunker.is_complete(empty_graph), "Empty graph is complete."
+    empty_graph = KnowledgeGraph()
+    assert chunker.is_complete(empty_graph, mock_db), "Empty graph is complete."
 
-    with open("tests/data/hierarchy_graph.json", "r") as f:
-        data = json.load(f)
-        hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
+    hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
     assert not chunker.is_complete(
-        hierarchy_graph
+        hierarchy_graph, mock_db
     ), "Hierarchy graph should not be complete."
 
     incomplete_graph = hierarchy_graph.copy()
     first_node = list(incomplete_graph.nodes)[0]
     incomplete_graph.nodes[first_node]["chunks"] = []
     assert not chunker.is_complete(
-        incomplete_graph
+        incomplete_graph, mock_db
     ), "Incomplete graph should not be complete"
 
-    for _, data in incomplete_graph.nodes(data=True):
+    for node, data in incomplete_graph.nodes(data=True):
+        assert data, f"Node {node} is missing data"
         if data["type"] == "file":
             data["chunks"] = []
-    assert chunker.is_complete(incomplete_graph), "Empty chunks should be complete"
-
-    with open("tests/data/chunker_graph.json", "r") as f:
-        data = json.load(f)
-        chunker_graph = nx.readwrite.json_graph.node_link_graph(data)
-    assert chunker.is_complete(chunker_graph), "Chunker graph should be complete."
+    assert chunker.is_complete(
+        incomplete_graph, mock_db
+    ), "Empty chunks should be complete"
+
+    chunker_graph = KnowledgeGraph.load("tests/data/chunker_graph.json")
+    assert chunker.is_complete(
+        chunker_graph, mock_db
+    ), "Chunker graph should be complete."
 
 
 @pytest.mark.asyncio
 async def test_chunker_llm_annotate(cwd, mock_get_llm_response, mock_db):
     daemon = Daemon(
         cwd=cwd,
         annotators={"hierarchy": {}},
         graph_path=(Path.cwd() / "tests/data/hierarchy_graph.json"),
     )
     chunker = ChunkerLLM(spice_client=AsyncMock())
     actual = await chunker.annotate(daemon.graph, mock_db)
 
     for node, data in actual.nodes(data=True):
+        assert data, f"Node {node} is missing data"
         if data["type"] == "file" and Path(node).suffix in chunker.chunk_extensions:
             assert "chunks" in data, f"File {node} is missing chunks"
```

### Comparing `ragdaemon-0.1.5/tests/annotators/test_diff.py` & `ragdaemon-0.1.6/tests/annotators/test_diff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 
-import networkx as nx
 import pytest
 
+from networkx.readwrite import json_graph
 from ragdaemon.annotators.diff import Diff, get_chunks_from_diff, parse_diff_id
 from ragdaemon.context import ContextBuilder
 from ragdaemon.daemon import Daemon
+from ragdaemon.graph import KnowledgeGraph
 from ragdaemon.utils import get_git_diff
 
 
 def test_diff_get_chunks_from_diff(git_history):
     diff = get_git_diff("HEAD", cwd=git_history)
     actual = get_chunks_from_diff("HEAD", diff)
     expected = {
@@ -32,26 +33,26 @@
         assert actual_ref == expected_ref
         assert actual_path == expected_path
         assert actual_lines == expected_lines
 
 
 @pytest.mark.asyncio
 async def test_diff_annotate(git_history, mock_db):
-    with open("tests/data/chunker_graph.json", "r") as f:
-        data = json.load(f)
-        graph = nx.readwrite.json_graph.node_link_graph(data)
+    graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
     graph.graph["cwd"] = git_history.as_posix()
     annotator = Diff()
     actual = await annotator.annotate(graph, mock_db)
-    actual_nodes = {n for n, d in actual.nodes(data=True) if d["type"] == "diff"}
+    actual_nodes = {n for n, d in actual.nodes(data=True) if d and d["type"] == "diff"}
 
     with open("tests/data/diff_graph.json", "r") as f:
         data = json.load(f)
-        expected = nx.readwrite.json_graph.node_link_graph(data)
-    expected_nodes = {n for n, d in expected.nodes(data=True) if d["type"] == "diff"}
+        expected = json_graph.node_link_graph(data)
+    expected_nodes = {
+        n for n, d in expected.nodes(data=True) if d and d["type"] == "diff"
+    }
 
     assert actual_nodes == expected_nodes
 
 
 @pytest.mark.asyncio
 async def test_diff_render(git_history, mock_db):
     daemon = Daemon(cwd=git_history)
```

### Comparing `ragdaemon-0.1.5/tests/annotators/test_hierarchy.py` & `ragdaemon-0.1.6/tests/annotators/test_hierarchy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 import json
 from pathlib import Path
 
-import networkx as nx
+from networkx.readwrite import json_graph
 import pytest
 
 from ragdaemon.annotators.hierarchy import Hierarchy, get_active_checksums
+from ragdaemon.graph import KnowledgeGraph
 
 
 def test_get_active_checksums(cwd, mock_db):
     checksums = get_active_checksums(cwd, mock_db)
     assert isinstance(checksums, dict), "Checksums is not a dict"
     assert all(isinstance(k, Path) for k in checksums), "Keys are not all Paths"
     assert all(
         isinstance(v, str) for v in checksums.values()
     ), "Values are not all strings"
 
-    with open("tests/data/hierarchy_graph.json", "r") as f:
-        data = json.load(f)
-        hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
+    hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
     expected = {
         (node, data["checksum"])
         for node, data in hierarchy_graph.nodes(data=True)
-        if "checksum" in data
+        if data and "checksum" in data
     }
     actual = {(path.as_posix(), checksum) for path, checksum in checksums.items()}
     assert actual == expected, "Checksums are not equal"
 
 
-def test_hierarchy_is_complete(cwd):
-    empty_graph = nx.MultiDiGraph()
+def test_hierarchy_is_complete(cwd, mock_db):
+    empty_graph = KnowledgeGraph()
     empty_graph.graph["cwd"] = cwd.as_posix()
     hierarchy = Hierarchy()
 
-    assert not hierarchy.is_complete(empty_graph), "Empty graph should not be complete."
+    assert not hierarchy.is_complete(
+        empty_graph, mock_db
+    ), "Empty graph should not be complete."
     incomplete_graph = empty_graph.copy()
     path_str = cwd.as_posix()
-    incomplete_graph.add_node(path_str, path=path_str, type="directory", id=path_str)
+    record = {"id": path_str, "type": "directory", "ref": path_str}
+    incomplete_graph.add_node(path_str, **record)
     assert not hierarchy.is_complete(
-        incomplete_graph
+        incomplete_graph, mock_db
     ), "Incomplete graph should not be complete"
 
 
 @pytest.mark.asyncio
 async def test_hierarchy_annotate(cwd, mock_db):
-    graph = nx.MultiDiGraph()
+    graph = KnowledgeGraph()
     graph.graph["cwd"] = cwd.as_posix()
     hierarchy = Hierarchy()
     actual = await hierarchy.annotate(graph, mock_db)
 
     # Load the template graph
     with open("tests/data/hierarchy_graph.json", "r") as f:
         data = json.load(f)
-        expected = nx.readwrite.json_graph.node_link_graph(data)
+        expected = json_graph.node_link_graph(data)
     for node in expected:  # Add the ID field back in
         expected.nodes[node]["id"] = node
 
     assert set(actual.nodes) == set(expected.nodes), "Nodes are not equal"
     assert set(actual.edges) == set(expected.edges), "Edges are not equal"
 
     assert hierarchy.is_complete(actual, mock_db), "Graph should be complete"
```

### Comparing `ragdaemon-0.1.5/tests/annotators/test_layout_hierarchy.py` & `ragdaemon-0.1.6/tests/annotators/test_layout_hierarchy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,50 @@
-import json
-
-import networkx as nx
 import pytest
 
 from ragdaemon.annotators.layout_hierarchy import LayoutHierarchy
+from ragdaemon.graph import KnowledgeGraph
 
 
-def test_layout_hierarchy_is_complete(cwd):
+def test_layout_hierarchy_is_complete(cwd, mock_db):
     layout_hierarchy = LayoutHierarchy()
 
-    empty_graph = nx.MultiDiGraph()
-    assert layout_hierarchy.is_complete(empty_graph), "Empty graph is complete."
+    empty_graph = KnowledgeGraph()
+    assert layout_hierarchy.is_complete(
+        empty_graph, mock_db
+    ), "Empty graph is complete."
 
-    with open("tests/data/hierarchy_graph.json", "r") as f:
-        data = json.load(f)
-        hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
+    hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
     assert not layout_hierarchy.is_complete(
-        hierarchy_graph
+        hierarchy_graph, mock_db
     ), "Hierarchy graph should not be complete."
 
     incomplete_graph = hierarchy_graph.copy()
     first_node = list(incomplete_graph.nodes)[0]
     incomplete_graph.nodes[first_node]["layout"] = {
         "hierarchy": {"x": 0, "y": 0, "z": 0}
     }
     assert not layout_hierarchy.is_complete(
-        incomplete_graph
+        incomplete_graph, mock_db
     ), "Incomplete graph should not be complete"
 
-    with open("tests/data/layout_hierarchy_graph.json", "r") as f:
-        data = json.load(f)
-        layout_hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
+    layout_hierarchy_graph = KnowledgeGraph.load(
+        "tests/data/layout_hierarchy_graph.json"
+    )
     assert layout_hierarchy.is_complete(
-        layout_hierarchy_graph
+        layout_hierarchy_graph, mock_db
     ), "Layout hierarchy graph should be complete."
 
 
 @pytest.mark.asyncio
 async def test_layout_hierarchy_annotate(cwd, mock_db):
-    with open("tests/data/hierarchy_graph.json", "r") as f:
-        data = json.load(f)
-        hierarchy_graph = nx.readwrite.json_graph.node_link_graph(data)
+    hierarchy_graph = KnowledgeGraph.load("tests/data/hierarchy_graph.json")
     actual = await LayoutHierarchy().annotate(hierarchy_graph, mock_db)
 
     all_coordinates = set()
     for node, data in actual.nodes(data=True):
+        assert data, f"Node {node} is missing data"
         coordinates = data.get("layout", {}).get("hierarchy", {})
         assert coordinates, f"Node {node} is missing hierarchy layout"
         all_coordinates.add((coordinates["x"], coordinates["y"], coordinates["z"]))
     assert (
         len(all_coordinates) == actual.number_of_nodes()
     ), "Coordinates are not unique"
```

### Comparing `ragdaemon-0.1.5/tests/data/chunker_graph.json` & `ragdaemon-0.1.6/tests/data/chunker_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/data/context_message.txt` & `ragdaemon-0.1.6/tests/data/context_message.txt`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/data/diff_graph.json` & `ragdaemon-0.1.6/tests/data/diff_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/data/hierarchy_graph.json` & `ragdaemon-0.1.6/tests/data/hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/data/layout_hierarchy_graph.json` & `ragdaemon-0.1.6/tests/data/layout_hierarchy_graph.json`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/tests/sample/src/interface.py` & `ragdaemon-0.1.6/tests/sample/src/interface.py`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/LICENSE` & `ragdaemon-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/README.md` & `ragdaemon-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `ragdaemon-0.1.5/pyproject.toml` & `ragdaemon-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages=["ragdaemon"]
 
 [project]
 name = "ragdaemon"
-version = "0.1.5"
+version = "0.1.6"
 description = "Generate and render a call graph for a Python project."
 readme = "README.md"
 dependencies = [
     "chromadb==0.4.24",
+    "dict2xml==1.7.5",
     "fastapi==0.109.2",
     "Jinja2==3.1.3",
     "networkx==3.2.1",
-    "spiceai==0.1.11",
+    "spiceai~=0.1.0",
     "starlette==0.36.3",
-    "tiktoken==0.6.0",
     "tqdm==4.66.2",
     "uvicorn==0.27.1",
 ]
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -29,7 +29,15 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/AbanteAI/ragdaemon"
 
 [project.scripts]
 ragdaemon = "ragdaemon.__main__:run"
+
+[project.optional-dependencies]
+dev = [
+    "ruff",
+    "pyright",
+    "pytest",
+    "pytest-asyncio"
+]
```

### Comparing `ragdaemon-0.1.5/PKG-INFO` & `ragdaemon-0.1.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.3
 Name: ragdaemon
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generate and render a call graph for a Python project.
 Project-URL: Homepage, https://github.com/AbanteAI/ragdaemon
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: chromadb==0.4.24
+Requires-Dist: dict2xml==1.7.5
 Requires-Dist: fastapi==0.109.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: networkx==3.2.1
-Requires-Dist: spiceai==0.1.11
+Requires-Dist: spiceai~=0.1.0
 Requires-Dist: starlette==0.36.3
-Requires-Dist: tiktoken==0.6.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: uvicorn==0.27.1
+Provides-Extra: dev
+Requires-Dist: pyright; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-asyncio; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Ragdaemon
 
 Ragdaemon is a Retrieval-Augmented Generation (RAG) system for code. It runs a daemon (background process) to watch your active code, put it in a knowledge graph, and query the knowledge graph to (among other things) generate context for LLM completions.
 
 Three ways to use Ragdaemon:
```

