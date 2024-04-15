# Comparing `tmp/mkdocs_frontmatter_plugin-0.1.3.tar.gz` & `tmp/mkdocs_frontmatter_plugin-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_frontmatter_plugin-0.1.3.tar", max compression
+gzip compressed data, was "mkdocs_frontmatter_plugin-0.1.4.tar", max compression
```

## Comparing `mkdocs_frontmatter_plugin-0.1.3.tar` & `mkdocs_frontmatter_plugin-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       19 2024-04-15 14:06:47.642742 mkdocs_frontmatter_plugin-0.1.3/README.md
--rw-r--r--   0        0        0        0 2024-04-15 14:08:19.424332 mkdocs_frontmatter_plugin-0.1.3/mkdocs_frontmatter_plugin/__init__.py
--rw-r--r--   0        0        0     1605 2024-04-15 15:20:58.777464 mkdocs_frontmatter_plugin-0.1.3/mkdocs_frontmatter_plugin/config.py
--rw-r--r--   0        0        0     1827 2024-04-15 15:47:16.239221 mkdocs_frontmatter_plugin-0.1.3/mkdocs_frontmatter_plugin/plugin.py
--rw-r--r--   0        0        0      533 2024-04-15 15:47:31.523501 mkdocs_frontmatter_plugin-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 mkdocs_frontmatter_plugin-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-04-15 14:06:47.642742 mkdocs_frontmatter_plugin-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 14:08:19.424332 mkdocs_frontmatter_plugin-0.1.4/mkdocs_frontmatter_plugin/__init__.py
+-rw-r--r--   0        0        0     1605 2024-04-15 15:20:58.777464 mkdocs_frontmatter_plugin-0.1.4/mkdocs_frontmatter_plugin/config.py
+-rw-r--r--   0        0        0     2014 2024-04-15 17:20:29.150395 mkdocs_frontmatter_plugin-0.1.4/mkdocs_frontmatter_plugin/plugin.py
+-rw-r--r--   0        0        0      533 2024-04-15 17:20:33.420096 mkdocs_frontmatter_plugin-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 mkdocs_frontmatter_plugin-0.1.4/PKG-INFO
```

### Comparing `mkdocs_frontmatter_plugin-0.1.3/mkdocs_frontmatter_plugin/config.py` & `mkdocs_frontmatter_plugin-0.1.4/mkdocs_frontmatter_plugin/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_frontmatter_plugin-0.1.3/mkdocs_frontmatter_plugin/plugin.py` & `mkdocs_frontmatter_plugin-0.1.4/mkdocs_frontmatter_plugin/plugin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from mkdocs.plugins import BasePlugin
 from mkdocs_frontmatter_plugin.config import FrontMatterConfig
 from mkdocs_roamlinks_plugin.plugin import ROAMLINK_RE, RoamLinkReplacer
+from mkdocs.plugins import get_plugin_logger
 import re
-
 class FrontMatterPlugin(BasePlugin[FrontMatterConfig]):
     supports_multiple_instances = True
 
     # Initialize plugin
     def on_config(self, config):
         if not self.config.enabled:
             return
@@ -27,26 +27,32 @@
         if self.config.exclude:
             front_matter_dict = {
                 k: v
                 for k, v in front_matter_dict.items()
                 if k not in self.config.exclude
             }
 
+        base_docs_url = config["docs_dir"]
+        page_url = page.file.src_path
         table = self.construct_table(front_matter_dict, config["docs_dir"], page.file.src_path)
 
         # Prepend the table to the Markdown content
         updated_markdown = table + markdown
 
         return updated_markdown
 
     def construct_table(self, front_matter_dict, base_docs_url, page_url):
         table = "| **Properties** |  |\n"
         table += "| --- | --- |\n"
         for key, value in front_matter_dict.items():
             # escape pipes in values unless it's a markdown link
-            if re.match(ROAMLINK_RE, str(value)):
+            match = re.search(ROAMLINK_RE, str(value))
+            if match:
                 value = re.sub(ROAMLINK_RE, RoamLinkReplacer(base_docs_url, page_url), str(value))
             else:
                 value = str(value).replace("|", "\\|")
             table += f"| {key} | {value} |\n"
         table += "\n"
         return table
+
+
+log = get_plugin_logger(__name__)
```

### Comparing `mkdocs_frontmatter_plugin-0.1.3/pyproject.toml` & `mkdocs_frontmatter_plugin-0.1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-frontmatter-plugin"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Diego Canez <canezdiego@gmail.com>"]
 packages = [
     { include = "mkdocs_frontmatter_plugin", from = "." },
 ]
 readme = "README.md"
```

### Comparing `mkdocs_frontmatter_plugin-0.1.3/PKG-INFO` & `mkdocs_frontmatter_plugin-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-frontmatter-plugin
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Diego Canez
 Author-email: canezdiego@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

