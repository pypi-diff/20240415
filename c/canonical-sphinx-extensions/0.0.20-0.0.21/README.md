# Comparing `tmp/canonical-sphinx-extensions-0.0.20.tar.gz` & `tmp/canonical_sphinx_extensions-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonical-sphinx-extensions-0.0.20.tar", last modified: Wed Mar 27 13:25:45 2024, max compression
+gzip compressed data, was "canonical_sphinx_extensions-0.0.21.tar", last modified: Mon Apr 15 12:48:56 2024, max compression
```

## Comparing `canonical-sphinx-extensions-0.0.20.tar` & `canonical_sphinx_extensions-0.0.21.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.608123 canonical-sphinx-extensions-0.0.20/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-03-27 13:25:45.608123 canonical-sphinx-extensions-0.0.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.608123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-03-27 13:25:45.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-27 13:25:45.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:25:45.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 13:25:45.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-27 13:25:45.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/
--rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/_static/config-options.css
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/_static/config-options.js
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/custom-rst-roles/
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/custom-rst-roles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/filtered-toc/
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/filtered-toc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/_static/related-links.css
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.604123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/_static/terminal-output.css
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.608123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:25:45.608123 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/_static/youtube.css
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-27 13:25:39.000000 canonical-sphinx-extensions-0.0.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-03-27 13:25:45.608123 canonical-sphinx-extensions-0.0.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.970325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12420 2024-04-15 12:48:56.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-15 12:48:56.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:48:56.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-15 12:48:56.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-15 12:48:56.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/
+-rw-r--r--   0 runner    (1001) docker     (127)     8610 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/_static/config-options.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/_static/config-options.js
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/custom-rst-roles/
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/custom-rst-roles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/filtered-toc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/filtered-toc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/_static/related-links.css
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/_static/terminal-output.css
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:48:56.974325 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/_static/youtube.css
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 12:48:51.000000 canonical_sphinx_extensions-0.0.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-15 12:48:56.978325 canonical_sphinx_extensions-0.0.21/setup.cfg
```

### Comparing `canonical-sphinx-extensions-0.0.20/LICENSE` & `canonical_sphinx_extensions-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/PKG-INFO` & `canonical_sphinx_extensions-0.0.21/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonical-sphinx-extensions
-Version: 0.0.20
+Version: 0.0.21
 Summary: A collection of Sphinx extensions used by Canonical documentation
 Home-page: https://github.com/canonical/canonical-sphinx-extensions
 Author: Ruth Fuchss
 Author-email: ruth.fuchss@canonical.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -281,27 +281,43 @@
 You can override the style in your own style sheet.
 
 #### Add a terminal view
 
 To add a terminal view to your page, use the `:terminal:` directive and specify the the input (as `:input:` option) and output (as the main content of the directive).
 Any lines prefixed with `:input:` in the main content are treated as input as well.
 
-To override the prompt (`user@host:~$` by default), specify the `:user:` and/or `:host:` options.
+To override the prompt (`user@host:~$` by default), specify the `:user:`, `:dir:` and/or `:host:` options.
 To make the terminal scroll horizontally instead of wrapping long lines, add `:scroll:`.
 
 For example, in MyST syntax:
 
 ````
+Single command sample:
+
 ```{terminal}
-:input: command number one
+:input: single command
 :user: root
 :host: vm
+:dir: /tmp/dir/
 
 output line one
 output line two
+```
+
+Multiple command sample:
+
+```{terminal}
+:user: root
+:host: vm
+:dir: /tmp/dir/
+
+:input: a command
+output line one
+output line two
+
 :input: another command
 more output
 ```
 ````
 
 ### Filtered ToC
```

### Comparing `canonical-sphinx-extensions-0.0.20/README.md` & `canonical_sphinx_extensions-0.0.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -266,27 +266,43 @@
 You can override the style in your own style sheet.
 
 #### Add a terminal view
 
 To add a terminal view to your page, use the `:terminal:` directive and specify the the input (as `:input:` option) and output (as the main content of the directive).
 Any lines prefixed with `:input:` in the main content are treated as input as well.
 
-To override the prompt (`user@host:~$` by default), specify the `:user:` and/or `:host:` options.
+To override the prompt (`user@host:~$` by default), specify the `:user:`, `:dir:` and/or `:host:` options.
 To make the terminal scroll horizontally instead of wrapping long lines, add `:scroll:`.
 
 For example, in MyST syntax:
 
 ````
+Single command sample:
+
 ```{terminal}
-:input: command number one
+:input: single command
 :user: root
 :host: vm
+:dir: /tmp/dir/
 
 output line one
 output line two
+```
+
+Multiple command sample:
+
+```{terminal}
+:user: root
+:host: vm
+:dir: /tmp/dir/
+
+:input: a command
+output line one
+output line two
+
 :input: another command
 more output
 ```
 ````
 
 ### Filtered ToC
```

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/PKG-INFO` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonical-sphinx-extensions
-Version: 0.0.20
+Version: 0.0.21
 Summary: A collection of Sphinx extensions used by Canonical documentation
 Home-page: https://github.com/canonical/canonical-sphinx-extensions
 Author: Ruth Fuchss
 Author-email: ruth.fuchss@canonical.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -281,27 +281,43 @@
 You can override the style in your own style sheet.
 
 #### Add a terminal view
 
 To add a terminal view to your page, use the `:terminal:` directive and specify the the input (as `:input:` option) and output (as the main content of the directive).
 Any lines prefixed with `:input:` in the main content are treated as input as well.
 
-To override the prompt (`user@host:~$` by default), specify the `:user:` and/or `:host:` options.
+To override the prompt (`user@host:~$` by default), specify the `:user:`, `:dir:` and/or `:host:` options.
 To make the terminal scroll horizontally instead of wrapping long lines, add `:scroll:`.
 
 For example, in MyST syntax:
 
 ````
+Single command sample:
+
 ```{terminal}
-:input: command number one
+:input: single command
 :user: root
 :host: vm
+:dir: /tmp/dir/
 
 output line one
 output line two
+```
+
+Multiple command sample:
+
+```{terminal}
+:user: root
+:host: vm
+:dir: /tmp/dir/
+
+:input: a command
+output line one
+output line two
+
 :input: another command
 more output
 ```
 ````
 
 ### Filtered ToC
```

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/SOURCES.txt` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/canonical_sphinx_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/__init__.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/_static/config-options.css` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/_static/config-options.css`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/_static/config-options.js` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/_static/config-options.js`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/config-options/common.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/config-options/common.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/custom-rst-roles/__init__.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/custom-rst-roles/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/filtered-toc/__init__.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/filtered-toc/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/__init__.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/_static/related-links.css` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/_static/related-links.css`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/related-links/common.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/related-links/common.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/__init__.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     required_arguments = 0
     optional_arguments = 0
     has_content = True
     option_spec = {
         "input": directives.unchanged,
         "user": directives.unchanged,
         "host": directives.unchanged,
+        "dir": directives.unchanged,
         "scroll": directives.unchanged,
     }
 
     @staticmethod
     def input_line(prompt_text, command):
 
         inpline = nodes.container()
@@ -30,31 +31,31 @@
         inp["classes"].append("command")
         inpline.append(inp)
 
         return inpline
 
     def run(self):
 
-        # if :user: or :host: are provided, replace those in the prompt
+        # Build prompt with :user:, :host: and :dir: (whichever is provided)
 
-        command = "" if "input" not in self.options else self.options["input"]
-        user = "user" if "user" not in self.options else self.options["user"]
-        host = "host" if "host" not in self.options else self.options["host"]
-        prompt_text = user + "@" + host + ":~$ "
-        if user == "root":
-            prompt_text = prompt_text[:-2] + "# "
+        command = self.options["input"] if "input" in self.options else ""
+        user = self.options["user"] if "user" in self.options else "user"
+        host = self.options["host"] if "host" in self.options else "host"
+        dir = self.options["dir"] if "dir" in self.options else "~"
+        prompt_text = f"{user}@{host}:{dir}{'#' if user == 'root' else '$'} "
 
         out = nodes.container()
         out["classes"].append("terminal")
         if "scroll" in self.options:
             out["classes"].append("scroll")
 
-        # Add the original prompt and input
+        # Add the original prompt and input if the command is present
 
-        out.append(self.input_line(prompt_text, command))
+        if command:
+            out.append(self.input_line(prompt_text, command))
 
         # Go through the content and append all lines as output
         # except for the ones that start with ":input: " - those get
         # a prompt
 
         for output in self.content:
             if output.startswith(":input: "):
```

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/terminal-output/common.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/terminal-output/common.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/__init__.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/_static/youtube.css` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/_static/youtube.css`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/canonical-sphinx-extensions/youtube-links/common.py` & `canonical_sphinx_extensions-0.0.21/canonical-sphinx-extensions/youtube-links/common.py`

 * *Files identical despite different names*

### Comparing `canonical-sphinx-extensions-0.0.20/setup.cfg` & `canonical_sphinx_extensions-0.0.21/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = canonical-sphinx-extensions
-version = 0.0.20
+version = 0.0.21
 author = Ruth Fuchss
 author_email = ruth.fuchss@canonical.com
 description = A collection of Sphinx extensions used by Canonical documentation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/canonical/canonical-sphinx-extensions
```

