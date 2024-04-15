# Comparing `tmp/simple_config_sync-0.1.5.tar.gz` & `tmp/simple_config_sync-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_config_sync-0.1.5.tar", last modified: Wed Mar 27 02:15:35 2024, max compression
+gzip compressed data, was "simple_config_sync-0.1.6.tar", last modified: Mon Apr 15 04:27:03 2024, max compression
```

## Comparing `simple_config_sync-0.1.5.tar` & `simple_config_sync-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,21 @@
--rw-r--r--   0        0        0      360 2024-02-28 02:46:26.939911 simple_config_sync-0.1.5/README.md
--rw-r--r--   0        0        0      762 2024-03-27 02:15:35.381741 simple_config_sync-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-26 07:16:06.313934 simple_config_sync-0.1.5/src/simple_config_sync/__init__.py
--rw-r--r--   0        0        0      146 2024-02-27 03:13:57.975540 simple_config_sync-0.1.5/src/simple_config_sync/core/__init__.py
--rw-r--r--   0        0        0     1203 2024-03-27 02:02:07.190528 simple_config_sync-0.1.5/src/simple_config_sync/core/assets/tui.tcss
--rw-r--r--   0        0        0     4736 2024-03-27 02:13:20.351783 simple_config_sync-0.1.5/src/simple_config_sync/core/config.py
--rw-r--r--   0        0        0      265 2024-02-27 17:11:02.534641 simple_config_sync-0.1.5/src/simple_config_sync/core/scripts.py
--rw-r--r--   0        0        0     3268 2024-03-27 02:05:17.418826 simple_config_sync-0.1.5/src/simple_config_sync/core/tui.py
--rw-r--r--   0        0        0        0 2024-02-26 07:16:06.312934 simple_config_sync-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 simple_config_sync-0.1.5/PKG-INFO
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/PKG-INFO
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      360 2024-02-28 02:46:26.000000 simple_config_sync-0.1.6/README.md
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      798 2024-04-15 04:03:46.000000 simple_config_sync-0.1.6/pyproject.toml
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       38 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/setup.cfg
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.692870 simple_config_sync-0.1.6/src/
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.693870 simple_config_sync-0.1.6/src/simple_config_sync/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-15 04:03:32.000000 simple_config_sync-0.1.6/src/simple_config_sync/__init__.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       68 2024-04-15 04:00:21.000000 simple_config_sync-0.1.6/src/simple_config_sync/__main__.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/src/simple_config_sync/core/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      193 2024-04-15 03:59:59.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/__init__.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      222 2024-04-15 04:09:41.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/cli.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     5052 2024-04-15 03:33:48.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/config.py
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)     3649 2024-04-15 03:58:29.000000 simple_config_sync-0.1.6/src/simple_config_sync/core/tui.py
+drwxr-xr-x   0 hmeqo     (1000) hmeqo     (1000)        0 2024-04-15 04:27:03.694870 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      814 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/PKG-INFO
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      520 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/SOURCES.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)        1 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/dependency_links.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)      124 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/entry_points.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       42 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/requires.txt
+-rw-r--r--   0 hmeqo     (1000) hmeqo     (1000)       19 2024-04-15 04:27:03.000000 simple_config_sync-0.1.6/src/simple_config_sync.egg-info/top_level.txt
```

### Comparing `simple_config_sync-0.1.5/src/simple_config_sync/core/config.py` & `simple_config_sync-0.1.6/src/simple_config_sync/core/config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,177 +1,185 @@
 import os
 import shutil
 from copy import deepcopy
+from functools import cached_property
 from pathlib import Path
 from typing import Literal
 
 import toml
 
-Status = Literal['added', 'modified', 'deleted', '']
+Status = Literal["added", "modified", "deleted", ""]
 
 
-default_config_path = Path('./config-sync.toml')
-default_lock_path = Path('./config-sync.lock')
+class Link:
+    def __init__(self, d: dict) -> None:
+        self.d = d
 
+    def __eq__(self, value: "Option") -> bool:
+        return self.d == value.d
 
-def load(config_path: Path | None = None, lock_path: Path | None = None) -> None:
-    config_path = config_path or default_config_path
-    lock_path = lock_path or default_lock_path
-
-    if not config_path.exists():
-        raise FileNotFoundError(f'Could not find config file: {config_path}')
-
-    config = toml.load(config_path)
-    lock_cfg = toml.load(lock_path) if lock_path.exists() else {}
-
-    ops: dict = config.get('options', {})
-    lock_ops: dict = lock_cfg.get('options', {})
-
-    options.clear()
-    options.update({k: SyncOp(ops.get(k), lock_ops.get(k)) for k in sorted(set(ops).union(lock_ops))})
-
-
-def make_lock_file(lock_path: Path | None = None) -> None:
-    lock_path = lock_path or default_lock_path
-
-    config = {'options': {}}
-    for k, op in options.items():
-        if op.status == 'deleted':
-            continue
-        config['options'][k] = op.d
-    with lock_path.open('w') as file:
-        toml.dump(config, file)
-
+    def uninstall(self) -> None:
+        if not self.target.exists():
+            return
+        if self.target.is_symlink():
+            self.target.unlink()
 
-class Link(dict):
-    def install(self):
-        if self.linked:
+    def clean_target(self) -> None:
+        if not self.target.exists():
             return
-        source = self.source
-        target = self.target
-        if target.is_symlink() or target.is_file():
-            target.unlink()
-        elif target.is_dir():
-            shutil.rmtree(target)
-        target.parent.mkdir(parents=True, exist_ok=True)
-        target.symlink_to(source.absolute(), source.is_dir())
+        if self.target.is_symlink() or self.target.is_file():
+            self.target.unlink()
+        else:
+            shutil.rmtree(self.target)
 
-    def uninstall(self):
-        target = self.target
-        if target.exists() and target.is_symlink():
-            target.unlink()
+    def sync(self):
+        if not self.source.exists():
+            raise FileNotFoundError(f"Source file not found: {self.source}")
+        if self.target.exists():
+            self.clean_target()
+        self.target.symlink_to(self.source.resolve(), self.source.is_dir())
 
     @property
-    def source(self) -> Path:
-        return Path(os.path.expandvars(self.get('source', ''))).expanduser()
+    def linked(self) -> bool:
+        if not self.target.exists() or not self.target.is_symlink():
+            return False
+        return self.source.resolve() == self.target.readlink()
 
-    @source.setter
-    def source(self, value: Path | str):
-        self['source'] = str(value)
+    @cached_property
+    def source(self) -> Path:
+        return Path(os.path.expandvars(self.d.get("source", ""))).expanduser()
 
-    @property
+    @cached_property
     def target(self) -> Path:
-        return Path(os.path.expandvars(self.get('target', ''))).expanduser()
-
-    @target.setter
-    def target(self, value: Path | str):
-        self['target'] = str(value)
-
-    @property
-    def target_exists(self) -> bool:
-        target = self.target
-        return target.exists() or target.is_symlink()
-
-    @property
-    def linked(self) -> bool:
-        target = self.target
-        if not target.is_symlink():
-            return False
-        return target.readlink() == self.source.absolute()
+        return Path(os.path.expandvars(self.d.get("target", ""))).expanduser()
 
 
 class Option:
-    def __init__(self, d: dict | None = None):
+    def __init__(self, d: dict | None) -> None:
         self.d = d or {}
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self) -> str:
-        return f'{self.__class__.__name__}({self.description})'
+        return f"{self.__class__.__name__}({self.description})"
 
     def __bool__(self) -> bool:
         return bool(self.d)
 
     @property
-    def group(self) -> str:
-        return self.d.get('group', '')
+    def name(self) -> str:
+        return self.d.get("name", "")
 
     @property
     def description(self) -> str:
-        return self.d.get('description', '')
+        return self.d.get("description", "")
 
     @property
     def links(self) -> list[Link]:
-        return [Link(i) for i in self.d.get('links', [])]
+        return [Link(i) for i in self.d.get("links", [])]
+
+    @property
+    def depends(self) -> dict[str, list]:
+        return self.d.get("depends", {})
 
     @property
     def synced(self) -> bool:
-        return self.d.get('synced', True)
+        return self.d.get("synced", False)
 
     @synced.setter
-    def synced(self, value: bool):
-        self.d['synced'] = value
+    def synced(self, value: bool) -> None:
+        self.d["synced"] = value
 
     @property
     def status(self) -> Status:
-        return self.d.get('status', '')
-
-    @property
-    def dependencies(self) -> list[str]:
-        return self.d.get('dependencies', [])
+        return self.d.get("status", "")
 
 
 class SyncOp(Option):
     def __init__(self, op: dict | None = None, lock_op: dict | None = None):
         assert op or lock_op
         self.op = Option(op)
         self.lock_op = Option(lock_op)
-        super().__init__(self.sync_lock())
-        self.synced = self.lock_op.synced if self.lock_op else self.op.synced
+        super().__init__(self._sync_op())
 
-    def sync_lock(self):
-        if self.status == 'deleted':
-            return deepcopy(self.lock_op.d)
-        return deepcopy(self.op.d)
-
-    def install(self):
-        for link in self.links:
-            link.install()
+    def _sync_op(self):
+        synced = self.op and (self.lock_op and self.lock_op.synced)
+        if self.status == "deleted":
+            return deepcopy(self.lock_op.d) | {"synced": synced}
+        return deepcopy(self.op.d) | {"synced": synced}
 
-    def uninstall(self):
-        self.status = 'deleted'
+    def sync(self):
+        if not self.synced:
+            self.uninstall()
+            return
         for link in self.lock_op.links:
             link.uninstall()
+        for link in self.op.links:
+            link.sync()
+        self.synced = True
 
-    def sync(self):
-        if self.status == 'deleted' or not self.synced:
-            self.uninstall()
-        else:
-            self.install()
+    def uninstall(self):
+        for link in self.lock_op.links:
+            link.uninstall()
+        self.synced = False
 
     @property
     def status(self) -> Status:
         if not self.op:
-            return 'deleted'
-        if not self.lock_op or self.lock_op.status == 'deleted' or not self.lock_op.synced:
-            return 'added'
+            return "deleted"
+        if not self.lock_op:
+            return "added"
         if self.op.links != self.lock_op.links:
-            return 'modified'
-        return ''
+            return "modified"
+        return ""
 
     @status.setter
     def status(self, value: Status):
-        self.d['status'] = value
+        self.d["status"] = value
+
+
+class Config:
+    def __init__(self) -> None:
+        self.path = Path("config-sync.toml")
+        self.lock_path = Path("config-sync.lock")
+        self._opts: list[Option] = []
+        self._lock_opts: list[Option] = []
+        self.opts: list[SyncOp] = []
+
+    def load(self) -> None:
+        with open(self.path) as f:
+            d = toml.load(f) or {}
+            opts = {i.get("name", ""): i for i in d.get("option", [])}
+        if self.lock_path.exists():
+            with open(self.lock_path) as f:
+                lock_d = toml.load(f) or {}
+            lock_opts = {i.get("name", ""): i for i in lock_d.get("option", [])}
+        else:
+            lock_opts = {}
+        self.opts.clear()
+        sync_opts = []
+        for i in opts:
+            sync_opts.append(SyncOp(opts[i], lock_opts.get(i)))
+        for i in lock_opts:
+            if i not in opts:
+                sync_opts.append(SyncOp(None, lock_opts[i]))
+        self.opts.extend(sync_opts)
+
+    def lock(self) -> None:
+        with open(self.lock_path, "w") as f:
+            toml.dump({"option": [i.d for i in self.opts if i.op]}, f)
+
+    def sync(self) -> None:
+        for op in self.opts:
+            op.sync()
+        self.lock()
+        self.load()
+
+    def uninstall(self) -> None:
+        for op in self.opts:
+            op.uninstall()
+        self.lock()
+        self.load()
 
 
-options: dict[str, SyncOp] = {}
+config = Config()
```

### Comparing `simple_config_sync-0.1.5/src/simple_config_sync/core/tui.py` & `simple_config_sync-0.1.6/src/simple_config_sync/core/tui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,118 @@
 from textual import on
 from textual.app import App, ComposeResult
 from textual.containers import Container, Horizontal, VerticalScroll
 from textual.reactive import reactive
 from textual.widgets import Button, Checkbox, Footer, Header, Static
 
-from . import config, scripts
+from .config import Link as _Link
+from .config import Option as _Option
+from .config import config
 
 
 class Link(Horizontal):
-    def __init__(self, link: config.Link, **kwds):
+    def __init__(self, link: _Link, **kwds):
         self.link = link
         super().__init__(**kwds)
 
     def compose(self) -> ComposeResult:
-        yield Static(f'{self.link.source} -> {self.link.target}')
+        yield Static(f"{self.link.source} -> {self.link.target}")
         if self.link.linked:
-            yield Static('Linked', classes='hint text-success')
-        elif self.link.target_exists:
-            yield Static('Target is exists, will override.', classes='hint text-warning')
+            yield Static("Linked", classes="hint text-success")
+        elif self.link.target.exists():
+            yield Static("Target is exists, will override.", classes="hint text-warning")
 
 
 class Option(Container):
-    cb_label = reactive('Sync')
+    cb_label = reactive("Sync")
 
-    def __init__(self, key: str, op: config.SyncOp, **kwds):
+    def __init__(self, op: _Option, **kwds):
         super().__init__(**kwds)
-        self.key = key
         self.op = op
 
     def compute_cb_label(self):
-        return 'Sync' if self.op.synced else 'Unsync'
+        return "Sync" if self.op.synced else "Unsync"
 
     def compose(self) -> ComposeResult:
-        yield Checkbox(self.cb_label, self.op.synced, id='sync')
-        with Container(id='content'):
-            with Container(id='info'):
-                yield Static(self.key, id='name', classes='text-primary')
-                if self.op.group:
-                    yield Static(f'({self.op.group})', id='group', classes='text-red')
-                yield Static(self.op.description, id='description')
-                yield Static(self.op.status, id='status', classes=self.op.status)
-            with Container(id='links'):
+        yield Checkbox(self.cb_label, self.op.synced, id="sync")
+        with Container(id="content"):
+            with Container(id="info"):
+                yield Static(self.op.name, id="name", classes="text-primary")
+                yield Static(self.op.description, id="description")
+                yield Static(self.op.status, id="status", classes=self.op.status)
+            with Container(id="depends"):
+                for i in self.op.depends:
+                    depends = ", ".join(self.op.depends[i])
+                    yield Static(f"{i.title()} Depends: {depends}")
+            with Container(id="links"):
                 for link in self.op.links:
                     yield Link(link)
 
-    @on(Checkbox.Changed, '#sync')
+    @on(Checkbox.Changed, "#sync")
     def on_check_changed(self, event: Checkbox.Changed) -> None:
         self.op.synced = event.value
         event.control.label = self.cb_label
 
 
 class OptionList(VerticalScroll):
-    options = reactive(config.options)
+    options = reactive(config.opts)
 
     def watch_options(self):
         self.update()
 
     def update(self):
         self.loading = True
         self.remove_children().__await__()
-        self.mount(*[Option(key, op) for key, op in self.options.items()]).__await__()
+        self.mount(*[Option(op) for op in self.options]).__await__()
         self.loading = False
 
 
 class Panel(Container):
     def compose(self) -> ComposeResult:
-        yield Button('Sync', 'success', id='sync')
-        yield Button('Uninstall', 'primary', id='uninstall')
-        yield Button('Read config', 'primary', id='read-config')
+        yield Button("Sync", "success", id="sync")
+        yield Button("Uninstall", "primary", id="uninstall")
+        yield Button("Read config", "primary", id="read-config")
 
-    @on(Button.Pressed, '#sync')
+    @on(Button.Pressed, "#sync")
     def on_sync(self, event: Button.Pressed):
-        scripts.sync()
-        self.app.query_one(OptionList).update()
+        getattr(self.app, "action_sync")()
 
-    @on(Button.Pressed, '#uninstall')
+    @on(Button.Pressed, "#uninstall")
     def on_uninstall(self, event: Button.Pressed):
-        scripts.uninstall()
-        self.app.query_one(OptionList).update()
+        getattr(self.app, "uninstall")()
 
-    @on(Button.Pressed, '#read-config')
+    @on(Button.Pressed, "#read-config")
     def on_read_config(self, event: Button.Pressed):
-        config.load()
-        self.app.query_one(OptionList).update()
+        getattr(self.app, "read_config")()
 
 
 class MainScreen(Container):
     def compose(self) -> ComposeResult:
         yield OptionList()
         yield Panel()
 
 
 class SimpleConfigSyncApp(App):
-    CSS_PATH = 'assets/tui.tcss'
+    CSS_PATH = "assets/tui.tcss"
 
     BINDINGS = [
-        ('q', 'quit', 'Quit'),
+        ("s", "sync", "Sync"),
+        ("u", "uninstall", "Uninstall"),
+        ("q", "quit", "Quit"),
     ]
 
     def compose(self) -> ComposeResult:
         yield Header()
         yield Footer()
         yield MainScreen()
+
+    def action_sync(self):
+        config.sync()
+        self.query_one(OptionList).update()
+
+    def action_uninstall(self):
+        config.uninstall()
+        self.query_one(OptionList).update()
+
+    def action_read_config(self):
+        config.load()
+        self.query_one(OptionList).update()
```

