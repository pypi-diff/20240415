# Comparing `tmp/partcad-cli-0.5.6.tar.gz` & `tmp/partcad-cli-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "partcad-cli-0.5.6.tar", last modified: Mon Mar  4 10:56:55 2024, max compression
+gzip compressed data, was "partcad-cli-0.5.8.tar", last modified: Wed Mar  6 07:20:37 2024, max compression
```

## Comparing `partcad-cli-0.5.6.tar` & `partcad-cli-0.5.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:55.390024 partcad-cli-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-04 10:56:55.390024 partcad-cli-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-04 10:56:53.000000 partcad-cli-0.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 10:56:55.390024 partcad-cli-0.5.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:55.386024 partcad-cli-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:55.390024 partcad-cli-0.5.6/src/partcad_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4249 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_install.py
--rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_render.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-04 10:56:07.000000 partcad-cli-0.5.6/src/partcad_cli/cli_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:56:55.390024 partcad-cli-0.5.6/src/partcad_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-04 10:56:55.000000 partcad-cli-0.5.6/src/partcad_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-04 10:56:55.000000 partcad-cli-0.5.6/src/partcad_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:56:55.000000 partcad-cli-0.5.6/src/partcad_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-04 10:56:55.000000 partcad-cli-0.5.6/src/partcad_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-04 10:56:55.000000 partcad-cli-0.5.6/src/partcad_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-04 10:56:55.000000 partcad-cli-0.5.6/src/partcad_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:37.505504 partcad-cli-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-06 07:20:37.505504 partcad-cli-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-06 07:20:35.000000 partcad-cli-0.5.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 07:20:37.505504 partcad-cli-0.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:37.501504 partcad-cli-0.5.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:37.505504 partcad-cli-0.5.8/src/partcad_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4315 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6736 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-03-06 07:19:40.000000 partcad-cli-0.5.8/src/partcad_cli/cli_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 07:20:37.505504 partcad-cli-0.5.8/src/partcad_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4951 2024-03-06 07:20:37.000000 partcad-cli-0.5.8/src/partcad_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-06 07:20:37.000000 partcad-cli-0.5.8/src/partcad_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 07:20:37.000000 partcad-cli-0.5.8/src/partcad_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-06 07:20:37.000000 partcad-cli-0.5.8/src/partcad_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-06 07:20:37.000000 partcad-cli-0.5.8/src/partcad_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-06 07:20:37.000000 partcad-cli-0.5.8/src/partcad_cli.egg-info/top_level.txt
```

### Comparing `partcad-cli-0.5.6/PKG-INFO` & `partcad-cli-0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: partcad-cli
-Version: 0.5.6
+Version: 0.5.8
 Summary: Command-line interface to PartCAD
 Author-email: Roman Kuzmenko <openvmp@proton.me>
 Maintainer-email: Roman Kuzmenko <openvmp@proton.me>
 Project-URL: Homepage, https://github.com/openvmp/partcad
 Project-URL: Issues, https://github.com/openvmp/partcad/issues
 Keywords: cadquery,build123d,cad,design,openscad,step,stl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: partcad==0.5.6
+Requires-Dist: partcad==0.5.8
 Requires-Dist: pycairo
 Requires-Dist: renderlab
 Requires-Dist: rlPyCairo
 Requires-Dist: svglib
 Requires-Dist: ocp_vscode
 
 # PartCAD <!-- omit in toc -->
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: partcad-cli Version: 0.5.6 Summary: Command-line
+Metadata-Version: 2.1 Name: partcad-cli Version: 0.5.8 Summary: Command-line
 interface to PartCAD Author-email: Roman Kuzmenko
 proton.me> Maintainer-email: Roman Kuzmenko
 proton.me> Project-URL: Homepage, https://github.com/openvmp/partcad Project-
 URL: Issues, https://github.com/openvmp/partcad/issues Keywords:
 cadquery,build123d,cad,design,openscad,step,stl Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown Requires-Dist: partcad==0.5.6 Requires-
+Description-Content-Type: text/markdown Requires-Dist: partcad==0.5.8 Requires-
 Dist: pycairo Requires-Dist: renderlab Requires-Dist: rlPyCairo Requires-Dist:
 svglib Requires-Dist: ocp_vscode # PartCAD [![License](https://github.com/
 openvmp/partcad/blob/main/apache20.svg?raw=true)](./LICENSE.txt) [![CI on
 Linux, MacOS and Windows](https://github.com/openvmp/partcad/actions/workflows/
 python-test.yml/badge.svg)](https://github.com/openvmp/partcad/actions/
 workflows/python-test.yml) [![CD on Linux, MacOS and Windows](https://
 github.com/openvmp/partcad/actions/workflows/python-build.yml/badge.svg)]
```

### Comparing `partcad-cli-0.5.6/README.md` & `partcad-cli-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/pyproject.toml` & `partcad-cli-0.5.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "partcad-cli"
-version = "0.5.6"
+version = "0.5.8"
 description = "Command-line interface to PartCAD"
 readme = "README.md"
 keywords = ["cadquery", "build123d", "cad", "design", "openscad", "step", "stl"]
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
 authors = [
   {name = "Roman Kuzmenko", email = "openvmp@proton.me" }
```

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli.py` & `partcad-cli-0.5.8/src/partcad_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,10 +144,13 @@
 
         else:
             print("Unknown command.\n")
             parser.print_help()
     except:
         pc.logging.exception("PartCAD CLI exception")
 
+    if not args.no_ansi:
+        pc.logging_ansi_terminal_fini()
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_add.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_add.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_info.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_info.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_init.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_init.py`

 * *Files 25% similar despite different names*

```diff
@@ -34,8 +34,7 @@
         else:
             dst_path = args.config_path
     else:
         dst_path = "partcad.yaml"
 
     if not pc.create_package(dst_path, args.private):
         pc_logging.error("Failed creating '%s'!" % dst_path)
-        sys.exit(1)
```

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_inspect.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_inspect.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_install.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_install.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_list.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_list.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_render.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_render.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli/cli_status.py` & `partcad-cli-0.5.8/src/partcad_cli/cli_status.py`

 * *Files identical despite different names*

### Comparing `partcad-cli-0.5.6/src/partcad_cli.egg-info/PKG-INFO` & `partcad-cli-0.5.8/src/partcad_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: partcad-cli
-Version: 0.5.6
+Version: 0.5.8
 Summary: Command-line interface to PartCAD
 Author-email: Roman Kuzmenko <openvmp@proton.me>
 Maintainer-email: Roman Kuzmenko <openvmp@proton.me>
 Project-URL: Homepage, https://github.com/openvmp/partcad
 Project-URL: Issues, https://github.com/openvmp/partcad/issues
 Keywords: cadquery,build123d,cad,design,openscad,step,stl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: partcad==0.5.6
+Requires-Dist: partcad==0.5.8
 Requires-Dist: pycairo
 Requires-Dist: renderlab
 Requires-Dist: rlPyCairo
 Requires-Dist: svglib
 Requires-Dist: ocp_vscode
 
 # PartCAD <!-- omit in toc -->
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: partcad-cli Version: 0.5.6 Summary: Command-line
+Metadata-Version: 2.1 Name: partcad-cli Version: 0.5.8 Summary: Command-line
 interface to PartCAD Author-email: Roman Kuzmenko
 proton.me> Maintainer-email: Roman Kuzmenko
 proton.me> Project-URL: Homepage, https://github.com/openvmp/partcad Project-
 URL: Issues, https://github.com/openvmp/partcad/issues Keywords:
 cadquery,build123d,cad,design,openscad,step,stl Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown Requires-Dist: partcad==0.5.6 Requires-
+Description-Content-Type: text/markdown Requires-Dist: partcad==0.5.8 Requires-
 Dist: pycairo Requires-Dist: renderlab Requires-Dist: rlPyCairo Requires-Dist:
 svglib Requires-Dist: ocp_vscode # PartCAD [![License](https://github.com/
 openvmp/partcad/blob/main/apache20.svg?raw=true)](./LICENSE.txt) [![CI on
 Linux, MacOS and Windows](https://github.com/openvmp/partcad/actions/workflows/
 python-test.yml/badge.svg)](https://github.com/openvmp/partcad/actions/
 workflows/python-test.yml) [![CD on Linux, MacOS and Windows](https://
 github.com/openvmp/partcad/actions/workflows/python-build.yml/badge.svg)]
```

### Comparing `partcad-cli-0.5.6/src/partcad_cli.egg-info/SOURCES.txt` & `partcad-cli-0.5.8/src/partcad_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

