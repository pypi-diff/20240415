# Comparing `tmp/systemd_language_server-0.3.4.tar.gz` & `tmp/systemd_language_server-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systemd_language_server-0.3.4.tar", max compression
+gzip compressed data, was "systemd_language_server-0.3.5.tar", max compression
```

## Comparing `systemd_language_server-0.3.4.tar` & `systemd_language_server-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2024-02-19 15:54:40.476800 systemd_language_server-0.3.4/LICENSE
--rw-r--r--   0        0        0      670 2024-02-19 15:54:40.476800 systemd_language_server-0.3.4/README.md
--rw-r--r--   0        0        0      989 2024-02-19 15:54:40.480800 systemd_language_server-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       46 2024-02-19 15:54:40.480800 systemd_language_server-0.3.4/systemd_language_server/__init__.py
--rw-r--r--   0        0        0     9110 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.automount.xml
--rw-r--r--   0        0        0   300199 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.exec.xml
--rw-r--r--   0        0        0    11224 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.kill.xml
--rw-r--r--   0        0        0    35101 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.mount.xml
--rw-r--r--   0        0        0    11477 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.path.xml
--rw-r--r--   0        0        0     6518 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.scope.xml
--rw-r--r--   0        0        0   106163 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.service.xml
--rw-r--r--   0        0        0    53014 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.socket.xml
--rw-r--r--   0        0        0    13426 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.swap.xml
--rw-r--r--   0        0        0    23762 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.timer.xml
--rw-r--r--   0        0        0   152945 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/assets/systemd.unit.xml
--rw-r--r--   0        0        0     9628 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/constants.py
--rw-r--r--   0        0        0     4274 2024-02-19 15:54:40.484800 systemd_language_server-0.3.4/systemd_language_server/server.py
--rw-r--r--   0        0        0     6907 2024-02-19 15:54:40.488800 systemd_language_server-0.3.4/systemd_language_server/unit.py
--rw-r--r--   0        0        0     1804 1970-01-01 00:00:00.000000 systemd_language_server-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-14 23:33:58.148894 systemd_language_server-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1849 2024-04-14 23:33:58.148894 systemd_language_server-0.3.5/README.md
+-rw-r--r--   0        0        0     1003 2024-04-14 23:33:58.152894 systemd_language_server-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-14 23:33:58.152894 systemd_language_server-0.3.5/systemd_language_server/__init__.py
+-rw-r--r--   0        0        0     9110 2024-04-14 23:33:58.152894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.automount.xml
+-rw-r--r--   0        0        0   300199 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.exec.xml
+-rw-r--r--   0        0        0    11224 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.kill.xml
+-rw-r--r--   0        0        0    35101 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.mount.xml
+-rw-r--r--   0        0        0    11477 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.path.xml
+-rw-r--r--   0        0        0     6518 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.scope.xml
+-rw-r--r--   0        0        0   106163 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.service.xml
+-rw-r--r--   0        0        0    53014 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.socket.xml
+-rw-r--r--   0        0        0    13426 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.swap.xml
+-rw-r--r--   0        0        0    23762 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.timer.xml
+-rw-r--r--   0        0        0   152945 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/assets/systemd.unit.xml
+-rw-r--r--   0        0        0     9628 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/constants.py
+-rw-r--r--   0        0        0     4705 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/server.py
+-rw-r--r--   0        0        0     6864 2024-04-14 23:33:58.156894 systemd_language_server-0.3.5/systemd_language_server/unit.py
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 systemd_language_server-0.3.5/PKG-INFO
```

### Comparing `systemd_language_server-0.3.4/LICENSE` & `systemd_language_server-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/pyproject.toml` & `systemd_language_server-0.3.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'systemd-language-server'
-version = '0.3.4'
+version = '0.3.5'
 description = 'Language server for systemd unit files'
 authors = ["Paweł Sacawa <pawel@sacawa.net>"]
 readme = "README.md"
 packages = [{ include = "systemd_language_server" }]
 scripts = { "systemd-language-server" = "systemd_language_server.server:main" }
 keywords = ['systemd', 'language', 'server', 'lsp', 'completion']
 license = "GPL3.0"
@@ -23,14 +23,15 @@
 
 [tool.poetry.dependencies]
 pygls = "^1.3"
 python = "^3.9"
 lxml = "^5.0.0"
 
 [tool.poetry.dev-dependencies]
+pytest = "^7"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.automount.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.automount.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.exec.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.exec.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.kill.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.kill.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.mount.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.mount.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.path.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.path.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.scope.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.scope.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.service.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.service.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.socket.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.socket.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.swap.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.swap.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.timer.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.timer.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/assets/systemd.unit.xml` & `systemd_language_server-0.3.5/systemd_language_server/assets/systemd.unit.xml`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/constants.py` & `systemd_language_server-0.3.5/systemd_language_server/constants.py`

 * *Files identical despite different names*

### Comparing `systemd_language_server-0.3.4/systemd_language_server/server.py` & `systemd_language_server-0.3.5/systemd_language_server/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-import logging
-import os.path
-import re
+import shutil
 import sys
 from argparse import ArgumentParser
-from pathlib import Path
 
 from lsprotocol.types import (
     INITIALIZE,
     TEXT_DOCUMENT_COMPLETION,
     TEXT_DOCUMENT_HOVER,
     CompletionItem,
     CompletionItemKind,
@@ -35,23 +32,65 @@
 
 
 class SystemdLanguageServer(LanguageServer):
     has_pandoc: bool = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.has_pandoc = os.path.exists("/bin/pandoc")
+        self.has_pandoc = shutil.which("pandoc") is not None
 
+        #  perhaps bizarrely, pygls LSP implementation forces dynamic feature registration
+        #  which frustrates a more tradition OOP design
 
-server = SystemdLanguageServer("systemd-language-server", "v0.1")
+        @self.feature(INITIALIZE)
+        def initialize(params: InitializedParams):
+            pass
 
+        @self.feature(
+            TEXT_DOCUMENT_COMPLETION, CompletionOptions(trigger_characters=["[', '="])
+        )
+        def textDocument_completion(params: CompletionParams) -> CompletionList | None:
+            """Complete systemd unit properties. Determine the required completion type and
+            dispatch it."""
+            items = []
+            uri = params.text_document.uri
+            document = self.workspace.get_text_document(uri)
+            current_line = document.lines[params.position.line].strip()
+            unit_type = get_unit_type(document)
+            section = get_current_section(document, params.position)
+
+            if current_line == "[":
+                return complete_unit_file_section(params, unit_type)
+            elif "=" not in current_line:
+                return complete_directive(params, unit_type, section, current_line)
+            elif len(current_line.split("=")) == 2:
+                return complete_directive_property(
+                    params, unit_type, section, current_line
+                )
+
+        @self.feature(TEXT_DOCUMENT_HOVER)
+        def textDocument_hover(params: HoverParams):
+            """Help for unit file directives."""
+            document = self.workspace.get_text_document(params.text_document.uri)
+            current_line = document.lines[params.position.line].strip()
+            unit_type = get_unit_type(document)
+            section = get_current_section(document, params.position)
+
+            if "=" in current_line:
+                directive = current_line.split("=")[0]
+                hover_range = range_for_directive(document, params.position)
+                contents = get_documentation_content(
+                    directive, unit_type, section, self.has_pandoc
+                )
+                if contents is None:
+                    return None
+                return Hover(contents=contents, range=hover_range)
 
-@server.feature(INITIALIZE)
-def initialize(params: InitializedParams):
-    pass
+
+server = SystemdLanguageServer("systemd-language-server", "v0.1")
 
 
 def complete_unit_file_section(params: CompletionParams, unit_type: UnitType):
     possible_sections = [UnitFileSection.install, UnitFileSection.unit]
     section = unit_type_to_unit_file_section(unit_type)
     if section is not None:
         possible_sections.append(section)
@@ -85,61 +124,21 @@
         CompletionItem(label=s, insert_text=s + "=", kind=CompletionItemKind.Property)
         for s in directives
         if s.startswith(current_line)
     ]
     return CompletionList(is_incomplete=False, items=items)
 
 
-@server.feature(
-    TEXT_DOCUMENT_COMPLETION, CompletionOptions(trigger_characters=["[', '="])
-)
-def textDocument_completion(params: CompletionParams) -> CompletionList | None:
-    """Complete systemd unit properties. Determine the required completion type and
-    dispatch it."""
-    items = []
-    uri = params.text_document.uri
-    document = server.workspace.get_document(uri)
-    current_line = document.lines[params.position.line].strip()
-    unit_type = get_unit_type(document)
-    section = get_current_section(document, params.position)
-
-    if current_line == "[":
-        return complete_unit_file_section(params, unit_type)
-    elif "=" not in current_line:
-        return complete_directive(params, unit_type, section, current_line)
-    elif len(current_line.split("=")) == 2:
-        return complete_directive_property(params, unit_type, section, current_line)
-
-
 def range_for_directive(document: TextDocument, position: Position) -> Range:
     """Range indicating directive (before =)"""
     current_line = document.lines[position.line].strip()
     idx = current_line.find("=")
     return Range(Position(position.line, 0), Position(position.line, idx - 1))
 
 
-@server.feature(TEXT_DOCUMENT_HOVER)
-def textDocument_hover(params: HoverParams):
-    """Help for unit file directives."""
-    document = server.workspace.get_document(params.text_document.uri)
-    current_line = document.lines[params.position.line].strip()
-    unit_type = get_unit_type(document)
-    section = get_current_section(document, params.position)
-
-    if "=" in current_line:
-        directive = current_line.split("=")[0]
-        hover_range = range_for_directive(document, params.position)
-        contents = get_documentation_content(
-            directive, unit_type, section, server.has_pandoc
-        )
-        if contents is None:
-            return None
-        return Hover(contents=contents, range=hover_range)
-
-
 def get_parser():
     parser = ArgumentParser()
     return parser
 
 
 def main():
     parser = get_parser()
```

### Comparing `systemd_language_server-0.3.4/systemd_language_server/unit.py` & `systemd_language_server-0.3.5/systemd_language_server/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 import re
 import subprocess
 from enum import Enum
 from glob import glob
 from io import StringIO
 from pathlib import Path
 
@@ -155,15 +154,15 @@
     return None
 
 
 def get_manual_sections(unit_type: UnitType, section: UnitFileSection | None):
     """Determine which docbook to search for documentation, based on unit type and file
     section. If no section is provided, search liberally, search liberally."""
     if section in [UnitFileSection.unit, UnitFileSection.install]:
-        return ["systemd.{}.xml".format(section.value.lower())]
+        return ["systemd.unit.xml"]
     ret = ["systemd.{}.xml".format(unit_type.value.lower())]
     if section is None:
         ret += ["systemd.unit.xml", "systemd.install.xml"]
     if unit_type.is_execable():
         ret += ["systemd.exec.xml", "systemd.kill.xml"]
     return ret
```

### Comparing `systemd_language_server-0.3.4/PKG-INFO` & `systemd_language_server-0.3.5/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,78 @@
-Metadata-Version: 2.1
-Name: systemd-language-server
-Version: 0.3.4
-Summary: Language server for systemd unit files
-Home-page: https://github.com/psacawa/systemd-language-server
-License: GPL3.0
-Keywords: systemd,language,server,lsp,completion
-Author: Paweł Sacawa
-Author-email: pawel@sacawa.net
-Requires-Python: >=3.9,<4.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: Other/Proprietary License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Software Development
-Classifier: Topic :: Text Editors :: Integrated Development Environments (IDE)
-Classifier: Topic :: Utilities
-Requires-Dist: lxml (>=5.0.0,<6.0.0)
-Requires-Dist: pygls (>=1.3,<2.0)
-Project-URL: Repository, https://github.com/psacawa/systemd-language-server
-Description-Content-Type: text/markdown
-
 # systemd-language-server
 
+[![PyPI](https://img.shields.io/pypi/v/systemd-language-server)](https://pypi.org/project/systemd-language-server)
+[![GitHub Actions (Tests)](https://github.com/psacawa/systemd-language-server/actions/workflows/test.yml/badge.svg)](https://github.com/psacawa/systemd-language-server/actions)
+[![GitHub](https://img.shields.io/github/license/psacawa/systemd-language-server)](https://github.com/psacawa/systemd-language-server/blob/master/LICENSE)
+
 Language server for systemd unit files. Result of an exercise to learn the language server protocol.
 
 ## Supported Features
 
 ### `textDocument/completion`
 
 Completion for
 
 - unit file directives
 - unit file sections
 <!-- - values of some directives -->
+
 ![](assets/completion.gif)
 
 ### `textDocument/hover`
 
 Documentation for directives supplied on hovering.
 
 ![](assets/hover.gif)
 
+For markup in hover windows (i.e. the fancy highlighting), `pandoc` must be found in `$PATH`. Otherwise, there will be fallback to plain text.
+
 ## Installation
 
 ```
 pip install systemd-language-server
 ```
 
-## Integrations
+## Example Integrations
 
 ### coc.nvim
 
 In `coc-settings.json`, under `.languageserver`:
 
 ```json
 ...
 "systemd-language-server": {
   "command": "systemd-language-server",
   "filetypes": ["systemd"]
 }
 ...
 ```
 
+### nvim-lspconfig
+
+```lua
+local lspconfig = require 'lspconfig'
+local configs = require 'lspconfig.configs'
+
+if not configs.systemd_ls then
+  configs.systemd_ls = {
+    default_config = {
+      cmd = { 'systemd-language-server' },
+      filetypes = { 'systemd' },
+      root_dir = function() return nil end,
+      single_file_support = true,
+      settings = {},
+    },
+    docs = {
+      description = [[
+https://github.com/psacawa/systemd-language-server
+
+Language Server for Systemd unit files.
+]]
+    }
+  }
+end
+
+lspconfig.systemd_ls.setup {}
+```
+
+Courtesy of @ValdezFOmar
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

