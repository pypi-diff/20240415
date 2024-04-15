# Comparing `tmp/mkdocs_frontmatter_plugin-0.1.1.tar.gz` & `tmp/mkdocs_frontmatter_plugin-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_frontmatter_plugin-0.1.1.tar", max compression
+gzip compressed data, was "mkdocs_frontmatter_plugin-0.1.2.tar", max compression
```

## Comparing `mkdocs_frontmatter_plugin-0.1.1.tar` & `mkdocs_frontmatter_plugin-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       19 2024-04-15 14:06:47.642742 mkdocs_frontmatter_plugin-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-15 14:08:19.424332 mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/__init__.py
--rw-r--r--   0        0        0     1558 2024-04-15 14:57:24.197278 mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/config.py
--rw-r--r--   0        0        0     1272 2024-04-15 15:13:47.844897 mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/plugin.py
--rw-r--r--   0        0        0      498 2024-04-15 15:14:01.673270 mkdocs_frontmatter_plugin-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 mkdocs_frontmatter_plugin-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-04-15 14:06:47.642742 mkdocs_frontmatter_plugin-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 14:08:19.424332 mkdocs_frontmatter_plugin-0.1.2/mkdocs_frontmatter_plugin/__init__.py
+-rw-r--r--   0        0        0     1605 2024-04-15 15:20:58.777464 mkdocs_frontmatter_plugin-0.1.2/mkdocs_frontmatter_plugin/config.py
+-rw-r--r--   0        0        0     1631 2024-04-15 15:31:23.002357 mkdocs_frontmatter_plugin-0.1.2/mkdocs_frontmatter_plugin/plugin.py
+-rw-r--r--   0        0        0      533 2024-04-15 15:33:38.497087 mkdocs_frontmatter_plugin-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 mkdocs_frontmatter_plugin-0.1.2/PKG-INFO
```

### Comparing `mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/config.py` & `mkdocs_frontmatter_plugin-0.1.2/mkdocs_frontmatter_plugin/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,8 +26,9 @@
 # Classes
 # -----------------------------------------------------------------------------
 
 # Tags plugin configuration
 class FrontMatterConfig(Config):
     enabled = Type(bool, default = True)
 
-    attributes = Optional(ListOfItems(Type(str)))
+    attributes = Optional(ListOfItems(Type(str)))
+    exclude = Optional(ListOfItems(Type(str)))
```

### Comparing `mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/plugin.py` & `mkdocs_frontmatter_plugin-0.1.2/mkdocs_frontmatter_plugin/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 from mkdocs.plugins import BasePlugin
 from mkdocs_frontmatter_plugin.config import FrontMatterConfig
-
+from mkdocs_roamlinks_plugin.plugin import ROAMLINK_RE
+import re
 
 class FrontMatterPlugin(BasePlugin[FrontMatterConfig]):
     supports_multiple_instances = True
 
     # Initialize plugin
     def on_config(self, config):
         if not self.config.enabled:
             return
 
     def on_page_markdown(self, markdown, page, config, **kwargs):
         if not self.config.enabled:
             return
 
-        front_matter_dict = page.meta
+        front_matter_dict: dict = page.meta
 
         # Construct table from front matter data
         if self.config.attributes:
             front_matter_dict = {
                 k: v
                 for k, v in front_matter_dict.items()
                 if k in self.config.attributes
             }
+        if self.config.exclude:
+            front_matter_dict = {
+                k: v
+                for k, v in front_matter_dict.items()
+                if k not in self.config.exclude
+            }
 
         table = self.construct_table(front_matter_dict)
 
         # Prepend the table to the Markdown content
         updated_markdown = table + markdown
 
         return updated_markdown
 
     def construct_table(self, front_matter_dict):
         table = "| **Properties** |  |\n"
         table += "| --- | --- |\n"
         for key, value in front_matter_dict.items():
-            # escape pipes in values
-            value = str(value).replace("|", "\\|")
+            # escape pipes in values unless it's a markdown link
+            if not re.match(ROAMLINK_RE, str(value)):
+                value = str(value).replace("|", "\\|")
             table += f"| {key} | {value} |\n"
         table += "\n"
         return table
```

