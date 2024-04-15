# Comparing `tmp/mkdocs-htmlproofer-plugin-1.2.0.tar.gz` & `tmp/mkdocs-htmlproofer-plugin-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-htmlproofer-plugin-1.2.0.tar", last modified: Tue Mar  5 14:09:41 2024, max compression
+gzip compressed data, was "mkdocs-htmlproofer-plugin-1.2.1.tar", last modified: Mon Apr 15 15:58:09 2024, max compression
```

## Comparing `mkdocs-htmlproofer-plugin-1.2.0.tar` & `mkdocs-htmlproofer-plugin-1.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2024-03-05 14:09:41.362658 mkdocs-htmlproofer-plugin-1.2.0/
--rw-r--r--   0 tianlzhang   (503) staff       (20)     1070 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.2.0/LICENSE.md
--rw-r--r--   0 tianlzhang   (503) staff       (20)     5814 2024-03-05 14:09:41.362463 mkdocs-htmlproofer-plugin-1.2.0/PKG-INFO
--rw-r--r--   0 tianlzhang   (503) staff       (20)     4912 2024-03-05 14:08:53.000000 mkdocs-htmlproofer-plugin-1.2.0/README.md
-drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2024-03-05 14:09:41.359202 mkdocs-htmlproofer-plugin-1.2.0/htmlproofer/
--rw-r--r--   0 tianlzhang   (503) staff       (20)        0 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.2.0/htmlproofer/__init__.py
--rw-r--r--   0 tianlzhang   (503) staff       (20)    12660 2024-03-05 14:08:53.000000 mkdocs-htmlproofer-plugin-1.2.0/htmlproofer/plugin.py
-drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2024-03-05 14:09:41.362085 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/
--rw-r--r--   0 tianlzhang   (503) staff       (20)     5814 2024-03-05 14:09:41.000000 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO
--rw-r--r--   0 tianlzhang   (503) staff       (20)      386 2024-03-05 14:09:41.000000 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 tianlzhang   (503) staff       (20)        1 2024-03-05 14:09:41.000000 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 tianlzhang   (503) staff       (20)       68 2024-03-05 14:09:41.000000 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/entry_points.txt
--rw-r--r--   0 tianlzhang   (503) staff       (20)       47 2024-03-05 14:09:41.000000 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/requires.txt
--rw-r--r--   0 tianlzhang   (503) staff       (20)       12 2024-03-05 14:09:41.000000 mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/top_level.txt
--rw-r--r--   0 tianlzhang   (503) staff       (20)      175 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.2.0/pyproject.toml
--rw-r--r--   0 tianlzhang   (503) staff       (20)       38 2024-03-05 14:09:41.362705 mkdocs-htmlproofer-plugin-1.2.0/setup.cfg
--rw-r--r--   0 tianlzhang   (503) staff       (20)     1431 2024-03-05 14:09:16.000000 mkdocs-htmlproofer-plugin-1.2.0/setup.py
+drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2024-04-15 15:58:09.838146 mkdocs-htmlproofer-plugin-1.2.1/
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     1070 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.2.1/LICENSE.md
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     5814 2024-04-15 15:58:09.837936 mkdocs-htmlproofer-plugin-1.2.1/PKG-INFO
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     4912 2024-03-05 14:08:53.000000 mkdocs-htmlproofer-plugin-1.2.1/README.md
+drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2024-04-15 15:58:09.834577 mkdocs-htmlproofer-plugin-1.2.1/htmlproofer/
+-rw-r--r--   0 tianlzhang   (503) staff       (20)        0 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.2.1/htmlproofer/__init__.py
+-rw-r--r--   0 tianlzhang   (503) staff       (20)    12719 2024-04-15 15:57:00.000000 mkdocs-htmlproofer-plugin-1.2.1/htmlproofer/plugin.py
+drwxr-xr-x   0 tianlzhang   (503) staff       (20)        0 2024-04-15 15:58:09.837501 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     5814 2024-04-15 15:58:09.000000 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 tianlzhang   (503) staff       (20)      386 2024-04-15 15:58:09.000000 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)        1 2024-04-15 15:58:09.000000 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       68 2024-04-15 15:58:09.000000 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       47 2024-04-15 15:58:09.000000 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/requires.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       12 2024-04-15 15:58:09.000000 mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/top_level.txt
+-rw-r--r--   0 tianlzhang   (503) staff       (20)      175 2023-03-01 08:26:22.000000 mkdocs-htmlproofer-plugin-1.2.1/pyproject.toml
+-rw-r--r--   0 tianlzhang   (503) staff       (20)       38 2024-04-15 15:58:09.838193 mkdocs-htmlproofer-plugin-1.2.1/setup.cfg
+-rw-r--r--   0 tianlzhang   (503) staff       (20)     1431 2024-04-15 15:57:22.000000 mkdocs-htmlproofer-plugin-1.2.1/setup.py
```

### Comparing `mkdocs-htmlproofer-plugin-1.2.0/LICENSE.md` & `mkdocs-htmlproofer-plugin-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs-htmlproofer-plugin-1.2.0/PKG-INFO` & `mkdocs-htmlproofer-plugin-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-htmlproofer-plugin
-Version: 1.2.0
+Version: 1.2.1
 Summary: A MkDocs plugin that validates URL in rendered HTML files
 Home-page: https://github.com/manuzhang/mkdocs-htmlproofer-plugin
 Author: Manu Zhang
 Author-email: owenzhang1990@gmail.com
 License: MIT
 Keywords: mkdocs python markdown
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-htmlproofer-plugin-1.2.0/README.md` & `mkdocs-htmlproofer-plugin-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-htmlproofer-plugin-1.2.0/htmlproofer/plugin.py` & `mkdocs-htmlproofer-plugin-1.2.1/htmlproofer/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,17 +112,18 @@
         strainer = SoupStrainer(('a', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'li', 'sup', 'img'))
 
         content = output_content if self.config['validate_rendered_template'] else page.content
         soup = BeautifulSoup(content, 'html.parser', parse_only=strainer)
 
         all_element_ids = set(tag['id'] for tag in soup.select('[id]'))
         all_element_ids.add('')  # Empty anchor is commonly used, but not real
-        for a in soup.find_all('a', href=True):
-            url = a['href']
 
+        urls = set(a['href'] for a in soup.find_all('a', href=True)) | set(img['src'] for img in soup.find_all('img'))
+
+        for url in urls:
             if any(fnmatch.fnmatch(url, ignore_url) for ignore_url in self.config['ignore_urls']):
                 if self.config['warn_on_ignored_urls']:
                     log_warning(f"ignoring URL {url} from {page.file.src_path}")
             else:
                 url_status = self.get_url_status(url, page.file.src_path, all_element_ids, opt_files)
                 if self.bad_url(url_status) and self.is_error(self.config, url, url_status):
                     self.report_invalid_url(url, url_status, page.file.src_path)
@@ -190,26 +191,28 @@
     @staticmethod
     def is_url_target_valid(url: str, src_path: str, files: Dict[str, File]) -> bool:
         match = MARKDOWN_ANCHOR_PATTERN.match(url)
         if match is None:
             return True
 
         url_target, _, optional_anchor = match.groups()
-        _, extension = os.path.splitext(url_target)
-        if extension == ".html":
-            # URL is a link to another local Markdown file that may include an anchor.
-            target_markdown = HtmlProoferPlugin.find_target_markdown(url_target, src_path, files)
-            if target_markdown is None:
-                # The corresponding Markdown page was not found.
-                return False
-            if optional_anchor and not HtmlProoferPlugin.contains_anchor(target_markdown, optional_anchor):
-                # The corresponding Markdown header for this anchor was not found.
-                return False
-        elif HtmlProoferPlugin.find_source_file(url_target, src_path, files) is None:
+        source_file = HtmlProoferPlugin.find_source_file(url_target, src_path, files)
+        if source_file is None:
             return False
+
+        # If there's an anchor (fragment) on the link, we try to find it in the source_file
+        if optional_anchor:
+            _, extension = os.path.splitext(source_file.src_uri)
+            # Currently only Markdown-based pages are supported, but conceptually others could be added below
+            if extension == ".md":
+                if source_file.page is None or source_file.page.markdown is None:
+                    return False
+                if not HtmlProoferPlugin.contains_anchor(source_file.page.markdown, optional_anchor):
+                    return False
+
         return True
 
     @staticmethod
     def find_target_markdown(url: str, src_path: str, files: Dict[str, File]) -> Optional[str]:
         """From a built URL, find the original Markdown source from the project that built it."""
 
         file = HtmlProoferPlugin.find_source_file(url, src_path, files)
```

### Comparing `mkdocs-htmlproofer-plugin-1.2.0/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO` & `mkdocs-htmlproofer-plugin-1.2.1/mkdocs_htmlproofer_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-htmlproofer-plugin
-Version: 1.2.0
+Version: 1.2.1
 Summary: A MkDocs plugin that validates URL in rendered HTML files
 Home-page: https://github.com/manuzhang/mkdocs-htmlproofer-plugin
 Author: Manu Zhang
 Author-email: owenzhang1990@gmail.com
 License: MIT
 Keywords: mkdocs python markdown
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs-htmlproofer-plugin-1.2.0/setup.py` & `mkdocs-htmlproofer-plugin-1.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(fname: str):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='mkdocs-htmlproofer-plugin',
-    version='1.2.0',
+    version='1.2.1',
     description='A MkDocs plugin that validates URL in rendered HTML files',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     keywords='mkdocs python markdown',
     url='https://github.com/manuzhang/mkdocs-htmlproofer-plugin',
     author='Manu Zhang',
     author_email='owenzhang1990@gmail.com',
```

