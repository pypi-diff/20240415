# Comparing `tmp/deknp-0.1.8.tar.gz` & `tmp/deknp-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deknp-0.1.8.tar", last modified: Thu Feb 15 08:24:29 2024, max compression
+gzip compressed data, was "deknp-0.1.9.tar", last modified: Fri Feb 16 07:52:34 2024, max compression
```

## Comparing `deknp-0.1.8.tar` & `deknp-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rw-r--r--   0        0        0       49 2024-02-15 08:24:27.934705 deknp-0.1.8/README.md
--rw-r--r--   0        0        0      630 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/__entry__.py
--rw-r--r--   0        0        0        0 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/__init__.py
--rw-r--r--   0        0        0     7058 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/__init__.py
--rw-r--r--   0        0        0      332 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/__init__.py
--rw-r--r--   0        0        0     1447 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/babel_config.py
--rw-r--r--   0        0        0     6555 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/base/__init__.py
--rw-r--r--   0        0        0      275 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/dv3.py
--rw-r--r--   0        0        0     1410 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/dv3_server.py
--rw-r--r--   0        0        0     1248 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/dv3_svg.py
--rw-r--r--   0        0        0     1654 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/dv3_yaml.py
--rw-r--r--   0        0        0     1051 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/favicon_ico.py
--rw-r--r--   0        0        0        0 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/fix/__init__.py
--rw-r--r--   0        0        0     1143 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/fix/svgpathtools.py
--rw-r--r--   0        0        0     1724 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/override_root.py
--rw-r--r--   0        0        0      507 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/package_json.py
--rw-r--r--   0        0        0     1479 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/packages.py
--rw-r--r--   0        0        0      910 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/requests.py
--rw-r--r--   0        0        0     1979 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/uniapp_vars.py
--rw-r--r--   0        0        0     2926 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/vite_config.py
--rw-r--r--   0        0        0     1614 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/plugins/vue_config.py
--rw-r--r--   0        0        0      831 2024-02-15 08:24:27.934705 deknp-0.1.8/deknp/core/run.py
--rw-r--r--   0        0        0      610 2024-02-15 08:24:29.566740 deknp-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-15 08:24:27.934705 deknp-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      490 1970-01-01 00:00:00.000000 deknp-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      324 2024-02-16 07:52:32.148477 deknp-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/__init__.py
+-rw-r--r--   0        0        0       42 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/click/__entry__.py
+-rw-r--r--   0        0        0      759 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/click/__init__.py
+-rw-r--r--   0        0        0     7058 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/__init__.py
+-rw-r--r--   0        0        0      332 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/__init__.py
+-rw-r--r--   0        0        0     1447 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/babel_config.py
+-rw-r--r--   0        0        0     6555 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/base/__init__.py
+-rw-r--r--   0        0        0      275 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/dv3.py
+-rw-r--r--   0        0        0     1410 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/dv3_server.py
+-rw-r--r--   0        0        0     1248 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/dv3_svg.py
+-rw-r--r--   0        0        0     1654 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/dv3_yaml.py
+-rw-r--r--   0        0        0     1051 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/favicon_ico.py
+-rw-r--r--   0        0        0        0 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/fix/__init__.py
+-rw-r--r--   0        0        0     1143 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/fix/svgpathtools.py
+-rw-r--r--   0        0        0     1724 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/override_root.py
+-rw-r--r--   0        0        0      507 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/package_json.py
+-rw-r--r--   0        0        0     1479 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/packages.py
+-rw-r--r--   0        0        0      910 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/requests.py
+-rw-r--r--   0        0        0     1979 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/uniapp_vars.py
+-rw-r--r--   0        0        0     2926 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/vite_config.py
+-rw-r--r--   0        0        0     1614 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/plugins/vue_config.py
+-rw-r--r--   0        0        0      831 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/core/run.py
+-rw-r--r--   0        0        0        0 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/gen/__init__.py
+-rw-r--r--   0        0        0      218 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/gen/templatefiles/shell/.deknp.apprebuild.pysh
+-rw-r--r--   0        0        0      215 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/gen/templatefiles/shell/.deknp.appupdate.pysh
+-rw-r--r--   0        0        0      504 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/gen/templatefiles/shell/.deknp.asapp.pysh
+-rw-r--r--   0        0        0      432 2024-02-16 07:52:32.148477 deknp-0.1.9/deknp/gen/tmpl.py
+-rw-r--r--   0        0        0      589 2024-02-16 07:52:34.760504 deknp-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-16 07:52:32.148477 deknp-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 deknp-0.1.9/PKG-INFO
```

### Comparing `deknp-0.1.8/deknp/__entry__.py` & `deknp-0.1.9/deknp/click/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import typer
 from typing_extensions import Annotated
-from .core import execute_install, execute_package_sure, execute_server, run_plugin_yaml, clear_pkg_cache
+from ..core import execute_install, execute_package_sure, execute_server, run_plugin_yaml, clear_pkg_cache
+from ..gen.tmpl import ShellGenerator
 
 app = typer.Typer(add_completion=False)
 
 
-def main():
-    app()
-
-
 @app.command()
 def install():
     execute_install()
 
 
 @app.command()
 def sure(force: Annotated[bool, typer.Option("--force/--no-force")] = False):
@@ -33,7 +30,12 @@
 def clearcache():
     clear_pkg_cache()
 
 
 @app.command()
 def yaml():
     run_plugin_yaml()
+
+
+@app.command()
+def shell(path: Annotated[str, typer.Argument()] = "."):
+    ShellGenerator(path, None).render()
```

### Comparing `deknp-0.1.8/deknp/core/__init__.py` & `deknp-0.1.9/deknp/core/__init__.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/babel_config.py` & `deknp-0.1.9/deknp/core/plugins/babel_config.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/base/__init__.py` & `deknp-0.1.9/deknp/core/plugins/base/__init__.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/dv3_server.py` & `deknp-0.1.9/deknp/core/plugins/dv3_server.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/dv3_svg.py` & `deknp-0.1.9/deknp/core/plugins/dv3_svg.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/dv3_yaml.py` & `deknp-0.1.9/deknp/core/plugins/dv3_yaml.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/favicon_ico.py` & `deknp-0.1.9/deknp/core/plugins/favicon_ico.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/fix/svgpathtools.py` & `deknp-0.1.9/deknp/core/plugins/fix/svgpathtools.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/override_root.py` & `deknp-0.1.9/deknp/core/plugins/override_root.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/packages.py` & `deknp-0.1.9/deknp/core/plugins/packages.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/requests.py` & `deknp-0.1.9/deknp/core/plugins/requests.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/uniapp_vars.py` & `deknp-0.1.9/deknp/core/plugins/uniapp_vars.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/vite_config.py` & `deknp-0.1.9/deknp/core/plugins/vite_config.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/plugins/vue_config.py` & `deknp-0.1.9/deknp/core/plugins/vue_config.py`

 * *Files identical despite different names*

### Comparing `deknp-0.1.8/deknp/core/run.py` & `deknp-0.1.9/deknp/core/run.py`

 * *Files identical despite different names*

