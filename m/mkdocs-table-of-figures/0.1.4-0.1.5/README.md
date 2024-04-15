# Comparing `tmp/mkdocs-table-of-figures-0.1.4.tar.gz` & `tmp/mkdocs-table-of-figures-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-table-of-figures-0.1.4.tar", last modified: Fri Jun  9 15:40:58 2023, max compression
+gzip compressed data, was "mkdocs-table-of-figures-0.1.5.tar", last modified: Mon Apr 15 14:45:16 2024, max compression
```

## Comparing `mkdocs-table-of-figures-0.1.4.tar` & `mkdocs-table-of-figures-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 15:40:58.459045 mkdocs-table-of-figures-0.1.4/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.4/MANIFEST.in
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5439 2023-06-09 15:40:58.457044 mkdocs-table-of-figures-0.1.4/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      824 2023-06-09 15:40:31.000000 mkdocs-table-of-figures-0.1.4/changelog.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.4/license
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 15:40:58.362122 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     6482 2023-06-09 15:40:47.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        0 2023-06-09 15:40:58.441491 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     5439 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)      417 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)        1 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       83 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       14 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       24 2023-06-09 15:40:57.000000 mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     4117 2023-06-09 15:39:23.000000 mkdocs-table-of-figures-0.1.4/readme.md
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)       38 2023-06-09 15:40:58.460045 mkdocs-table-of-figures-0.1.4/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1000) thibaud-brrd  (1000)     1135 2023-06-09 15:40:33.000000 mkdocs-table-of-figures-0.1.4/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-15 14:45:16.188695 mkdocs-table-of-figures-0.1.5/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2023-05-09 09:20:19.000000 mkdocs-table-of-figures-0.1.5/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5439 2024-04-15 14:45:16.188695 mkdocs-table-of-figures-0.1.5/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1076 2024-04-15 14:27:16.000000 mkdocs-table-of-figures-0.1.5/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2023-04-28 08:21:37.000000 mkdocs-table-of-figures-0.1.5/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-15 14:45:16.088699 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6880 2024-04-15 14:30:57.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2024-04-15 14:45:16.172038 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     5439 2024-04-15 14:45:15.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      417 2024-04-15 14:45:15.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2024-04-15 14:45:15.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       83 2024-04-15 14:45:15.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       14 2024-04-15 14:45:15.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       24 2024-04-15 14:45:15.000000 mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4117 2023-06-09 15:39:23.000000 mkdocs-table-of-figures-0.1.5/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2024-04-15 14:45:16.188695 mkdocs-table-of-figures-0.1.5/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1135 2024-04-15 14:09:36.000000 mkdocs-table-of-figures-0.1.5/setup.py
```

### Comparing `mkdocs-table-of-figures-0.1.4/PKG-INFO` & `mkdocs-table-of-figures-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.4
+Version: 0.1.5
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
```

### Comparing `mkdocs-table-of-figures-0.1.4/changelog.md` & `mkdocs-table-of-figures-0.1.5/changelog.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on Keep a Changelog, and this project adheres to Semantic Versioning.
 
+## [0.1.5] - 2024-04-15
+
+### Added
+
+- support for relative link to figures when tof file is contain in a subdirectory in `plugin.py`
+- markdown="span" to support new md-in-html requirements based on mkdocs-material documentation in `plugin.py`
+
 ## [0.1.4] - 2023-06-09
 
 ### Added
 
 - md_in_html support for relative link to image in `plugin.py`
 
 ## [0.1.3] - 2023-06-09
```

### Comparing `mkdocs-table-of-figures-0.1.4/license` & `mkdocs-table-of-figures-0.1.5/license`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures/plugin.py` & `mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,19 +30,23 @@
         self._logger.setLevel(logging.INFO)
 
         self.enabled = True
         self.total_time = 0
 
         self.counter = 1
         self.figures = []
+        self.file_directories_count = 0
+        self.file_relative_path = ''
         self.page = None
         self.keep_md_format = False
         self.listening = True
 
     def on_config(self, config):
+        self.file_directories_count = self.config.file.count('/')
+        self.file_relative_path = '../' * self.file_directories_count
         if 'markdown_extensions' in config and 'md_in_html' in config.markdown_extensions:
             self.keep_md_format = True
         return config
     
 
     def on_files(self, files, config):
         tof = os.path.join(self.config.temp_dir, self.config.file)
@@ -84,29 +88,30 @@
                     matches = sorted(matches, key=lambda x: x.start())
 
                     position_offset = 0
                     for match in matches:
                         checkpoint = markdown
 
                         try:
-                            link = f'{page.abs_url}#figure-{self.counter}'
+                            link = f'{self.file_relative_path}{page.file.src_uri}#figure-{self.counter}'
                             replacement = match.group(0)
                             if match.re.pattern == pattern_img and match.group(1):
                                 self.figures.append({"number": self.counter, "description": match.group(1), "link": link})
-                                replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n  <img src="{config.site_url + match.group(2)[1:] if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(1)}</figcaption>\n</figure>'
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  <img src="{config.site_url + match.group(2) if match.group(2).startswith("/") else match.group(2)}" alt="{match.group(1)}">\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                                 if self.keep_md_format:
-                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown>\n  ![{match.group(1)}]({match.group(2)})\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(1)}</figcaption>\n</figure>'
+                                    replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  ![{match.group(1)}]({match.group(2)})\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(1)}</figcaption>\n</figure>'
                             elif match.re.pattern == pattern_mermaid and match.group(2):
                                 self.figures.append({"number": self.counter, "description": match.group(2), "link": link})
-                                replacement = f'<figure id="figure-{self.counter}" class="figure-image">\n{match.group(1)}\n  <figcaption>{self.config.figure_label} {self.counter} - {match.group(2)}</figcaption>\n</figure>'
+                                replacement = f'<figure id="figure-{self.counter}" class="figure-image" markdown="span">\n  {match.group(1)}\n  <figcaption>{self.config.figure_label} {self.counter} — {match.group(2)}</figcaption>\n</figure>'
                             
+                            print(replacement)
                             if replacement == match.group(0):
-                                self._logger.debug(f'Ignoring image/diagram at {page.abs_url}')
+                                self._logger.debug(f'Ignoring image/diagram at {self.file_relative_path}{page.file.src_uri}')
                             else:
-                                self._logger.debug(f'Formating image/diagram as figure at {page.abs_url}')
+                                self._logger.debug(f'Formating image/diagram as figure at {self.file_relative_path}{page.file.src_uri}')
                                 self.counter += 1
                                 markdown = markdown[:match.start() + position_offset] + replacement + markdown[match.end() + position_offset:]
                                 position_offset += len(replacement) - len(match.group(0))
                         except:
                             markdown = checkpoint
                             
                 except:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mkdocs-table-of-figures-0.1.4/mkdocs_table_of_figures.egg-info/PKG-INFO` & `mkdocs-table-of-figures-0.1.5/mkdocs_table_of_figures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-table-of-figures
-Version: 0.1.4
+Version: 0.1.5
 Summary: A MkDocs plugin listing all figures to create a table of figures page
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-table-of-figures
```

### Comparing `mkdocs-table-of-figures-0.1.4/readme.md` & `mkdocs-table-of-figures-0.1.5/readme.md`

 * *Files identical despite different names*

### Comparing `mkdocs-table-of-figures-0.1.4/setup.py` & `mkdocs-table-of-figures-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-table-of-figures',
-    version='0.1.4',
+    version='0.1.5',
     description='A MkDocs plugin listing all figures to create a table of figures page',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-table-of-figures',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
```

