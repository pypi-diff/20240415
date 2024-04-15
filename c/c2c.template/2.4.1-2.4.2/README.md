# Comparing `tmp/c2c_template-2.4.1.tar.gz` & `tmp/c2c_template-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2c_template-2.4.1.tar", max compression
+gzip compressed data, was "c2c_template-2.4.2.tar", max compression
```

## Comparing `c2c_template-2.4.1.tar` & `c2c_template-2.4.2.tar`

### file list

```diff
@@ -1,31 +1,7 @@
--rw-r--r--   0        0        0     1296 2024-04-09 07:20:57.927365 c2c_template-2.4.1/LICENSE
--rw-r--r--   0        0        0     3293 2024-04-09 07:20:57.927365 c2c_template-2.4.1/README.rst
--rw-r--r--   0        0        0      111 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/__init__.py
--rw-r--r--   0        0        0    29542 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/template/__init__.py
--rw-r--r--   0        0        0     2552 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/template/config.py
--rw-r--r--   0        0        0        0 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/template/py.typed
--rw-r--r--   0        0        0       34 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/builder.jinja
--rw-r--r--   0        0        0       93 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/builder_vars.yaml
--rw-r--r--   0        0        0       79 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/builder_vars_dict.yaml
--rw-r--r--   0        0        0      103 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/config.yaml
--rw-r--r--   0        0        0        6 2024-04-09 07:22:03.535424 c2c_template-2.4.1/c2c/tests/env.tmpl
--rw-r--r--   0        0        0        6 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/env.tmpl.mako
--rw-r--r--   0        0        0      121 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/extends-run-env.yaml
--rw-r--r--   0        0        0      105 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/include.yaml
--rw-r--r--   0        0        0       10 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/include_1.yaml
--rw-r--r--   0        0        0        8 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/include_2.yaml
--rw-r--r--   0        0        0       53 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/inherit.yaml
--rw-r--r--   0        0        0      180 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/jinja.jinja
--rw-r--r--   0        0        0       71 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/loop.yaml
--rw-r--r--   0        0        0       87 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/mako.mako
--rw-r--r--   0        0        0       47 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/no_interpreted.yaml
--rw-r--r--   0        0        0      410 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/path.yaml
--rw-r--r--   0        0        0      375 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/postprocess.yaml
--rw-r--r--   0        0        0       69 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/recursive.yaml
--rw-r--r--   0        0        0       64 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/recursive_int.yaml
--rw-r--r--   0        0        0      282 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/run-env.yaml
--rw-r--r--   0        0        0    17743 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/test_template.py
--rw-r--r--   0        0        0       97 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/update.yaml
--rw-r--r--   0        0        0      494 2024-04-09 07:20:57.927365 c2c_template-2.4.1/c2c/tests/vars.yaml
--rw-r--r--   0        0        0     2085 2024-04-09 07:22:10.771427 c2c_template-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     4358 1970-01-01 00:00:00.000000 c2c_template-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1296 2024-04-15 13:36:25.092636 c2c_template-2.4.2/LICENSE
+-rw-r--r--   0        0        0     3293 2024-04-15 13:36:25.092636 c2c_template-2.4.2/README.rst
+-rw-r--r--   0        0        0    29540 2024-04-15 13:36:25.092636 c2c_template-2.4.2/c2c/template/__init__.py
+-rw-r--r--   0        0        0     2552 2024-04-15 13:36:25.092636 c2c_template-2.4.2/c2c/template/config.py
+-rw-r--r--   0        0        0        0 2024-04-15 13:36:25.092636 c2c_template-2.4.2/c2c/template/py.typed
+-rw-r--r--   0        0        0     2091 2024-04-15 13:37:29.629406 c2c_template-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4358 1970-01-01 00:00:00.000000 c2c_template-2.4.2/PKG-INFO
```

### Comparing `c2c_template-2.4.1/LICENSE` & `c2c_template-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c2c_template-2.4.1/README.rst` & `c2c_template-2.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `c2c_template-2.4.1/c2c/template/__init__.py` & `c2c_template-2.4.2/c2c/template/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
         while skip is None or old_skip != len(skip) and len(skip) != 0:
             old_skip = sys.maxsize if skip is None else len(skip)
             self.used_vars, skip = self.format_walker(self.used_vars)
 
         if len(skip) > 0:
             LOG.error(
                 "The following variable isn't correctly interpreted due missing dependency:\n%s",
-                "\n".join(["'{}' depend on '{}'".format(*e) for e in skip]),
+                "\n".join([f"'{e[0]}' depend on '{e[1]}'" for e in skip]),
             )
             sys.exit(1)
 
 
 def do(options: Namespace) -> None:  # pylint: disable=invalid-name
     if options.cache is not None and options.vars is not None:
         LOG.error("The --vars and --cache options cannot be used together")
```

### Comparing `c2c_template-2.4.1/c2c/template/config.py` & `c2c_template-2.4.2/c2c/template/config.py`

 * *Files identical despite different names*

### Comparing `c2c_template-2.4.1/pyproject.toml` & `c2c_template-2.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,34 +8,34 @@
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict_optional = true
 strict = true
 
 [tool.poetry]
 name = "c2c.template"
-version = "2.4.1"
+version = "2.4.2"
 description = "Vars collector and template runner."
 readme = "README.rst"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/c2c.template"
 license = "BSD-2-Clause"
 keywords = ["template"]
-packages = [{ include = "c2c" }]
+packages = [{ include = "c2c/template" }]
 classifiers = [
     "Programming Language :: Python",
     "Environment :: Console",
     "Framework :: Bottle",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
     "Programming Language :: Python :: 3",
     "Typing :: Typed",
 ]
-include = ["tilecloud_chain/py.typed"]
+include = ["c2c/template/py.typed"]
 
 [tool.poetry.scripts]
 c2c-template = "c2c.template:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 bottle = "0.12.25"
```

### Comparing `c2c_template-2.4.1/PKG-INFO` & `c2c_template-2.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2c.template
-Version: 2.4.1
+Version: 2.4.2
 Summary: Vars collector and template runner.
 Home-page: https://github.com/camptocamp/c2c.template
 License: BSD-2-Clause
 Keywords: template
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.9
```

