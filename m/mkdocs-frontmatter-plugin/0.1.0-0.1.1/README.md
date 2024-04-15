# Comparing `tmp/mkdocs_frontmatter_plugin-0.1.0.tar.gz` & `tmp/mkdocs_frontmatter_plugin-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_frontmatter_plugin-0.1.0.tar", max compression
+gzip compressed data, was "mkdocs_frontmatter_plugin-0.1.1.tar", max compression
```

## Comparing `mkdocs_frontmatter_plugin-0.1.0.tar` & `mkdocs_frontmatter_plugin-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       19 2024-04-15 14:06:47.642742 mkdocs_frontmatter_plugin-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-15 14:08:19.424332 mkdocs_frontmatter_plugin-0.1.0/mkdocs_frontmatter_plugin/__init__.py
--rw-r--r--   0        0        0     1558 2024-04-15 14:57:24.197278 mkdocs_frontmatter_plugin-0.1.0/mkdocs_frontmatter_plugin/config.py
--rw-r--r--   0        0        0     1156 2024-04-15 15:00:32.905342 mkdocs_frontmatter_plugin-0.1.0/mkdocs_frontmatter_plugin/plugin.py
--rw-r--r--   0        0        0      498 2024-04-15 15:05:16.824423 mkdocs_frontmatter_plugin-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 mkdocs_frontmatter_plugin-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-04-15 14:06:47.642742 mkdocs_frontmatter_plugin-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 14:08:19.424332 mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/__init__.py
+-rw-r--r--   0        0        0     1558 2024-04-15 14:57:24.197278 mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/config.py
+-rw-r--r--   0        0        0     1272 2024-04-15 15:13:47.844897 mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/plugin.py
+-rw-r--r--   0        0        0      498 2024-04-15 15:14:01.673270 mkdocs_frontmatter_plugin-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 mkdocs_frontmatter_plugin-0.1.1/PKG-INFO
```

### Comparing `mkdocs_frontmatter_plugin-0.1.0/mkdocs_frontmatter_plugin/config.py` & `mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_frontmatter_plugin-0.1.0/mkdocs_frontmatter_plugin/plugin.py` & `mkdocs_frontmatter_plugin-0.1.1/mkdocs_frontmatter_plugin/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,12 +28,15 @@
 
         # Prepend the table to the Markdown content
         updated_markdown = table + markdown
 
         return updated_markdown
 
     def construct_table(self, front_matter_dict):
-        table = "| Key | Value |\n"
+        table = "| **Properties** |  |\n"
         table += "| --- | --- |\n"
         for key, value in front_matter_dict.items():
+            # escape pipes in values
+            value = str(value).replace("|", "\\|")
             table += f"| {key} | {value} |\n"
+        table += "\n"
         return table
```

### Comparing `mkdocs_frontmatter_plugin-0.1.0/PKG-INFO` & `mkdocs_frontmatter_plugin-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-frontmatter-plugin
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Diego Canez
 Author-email: canezdiego@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

