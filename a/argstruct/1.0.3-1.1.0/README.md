# Comparing `tmp/argstruct-1.0.3.tar.gz` & `tmp/argstruct-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argstruct-1.0.3.tar", last modified: Thu Feb 22 09:27:28 2024, max compression
+gzip compressed data, was "argstruct-1.1.0.tar", last modified: Mon Apr 15 20:25:38 2024, max compression
```

## Comparing `argstruct-1.0.3.tar` & `argstruct-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:27:28.258966 argstruct-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)       81 2024-01-15 08:31:01.000000 argstruct-1.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      147 2024-01-14 21:16:27.000000 argstruct-1.0.3/.gitlab-ci.include.yml
--rw-rw-rw-   0 root         (0) root         (0)      298 2024-01-14 21:16:27.000000 argstruct-1.0.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-14 21:16:27.000000 argstruct-1.0.3/.mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    21013 2024-01-14 21:16:27.000000 argstruct-1.0.3/.pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:27:28.254966 argstruct-1.0.3/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      188 2024-01-14 21:16:27.000000 argstruct-1.0.3/.vscode/settings.json
--rw-rw-rw-   0 root         (0) root         (0)   115195 2024-02-22 09:12:06.000000 argstruct-1.0.3/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    35149 2024-01-15 21:48:08.000000 argstruct-1.0.3/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     7088 2024-01-14 21:16:27.000000 argstruct-1.0.3/Makefile
--rw-r--r--   0 root         (0) root         (0)     9884 2024-02-22 09:27:28.258966 argstruct-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     9065 2024-01-15 21:48:08.000000 argstruct-1.0.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)     3881 2024-01-15 10:34:30.000000 argstruct-1.0.3/project.mk
--rw-rw-rw-   0 root         (0) root         (0)     1146 2024-02-22 09:27:19.000000 argstruct-1.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-01-14 21:16:27.000000 argstruct-1.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-22 09:27:28.258966 argstruct-1.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:27:28.254966 argstruct-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:27:28.254966 argstruct-1.0.3/src/argstruct/
--rw-rw-rw-   0 root         (0) root         (0)     6832 2024-01-15 08:31:01.000000 argstruct-1.0.3/src/argstruct/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8361 2024-01-15 08:31:01.000000 argstruct-1.0.3/src/argstruct/documentation.py
--rw-rw-rw-   0 root         (0) root         (0)    10262 2024-02-22 09:12:06.000000 argstruct-1.0.3/src/argstruct/object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:27:28.258966 argstruct-1.0.3/src/argstruct/specs/
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-01-15 08:31:01.000000 argstruct-1.0.3/src/argstruct/specs/argmap.command.args-root.spec
--rw-rw-rw-   0 root         (0) root         (0)     1141 2024-01-14 21:16:27.000000 argstruct-1.0.3/src/argstruct/specs/argmap.command.args.spec
--rw-rw-rw-   0 root         (0) root         (0)     1122 2024-01-15 08:31:01.000000 argstruct-1.0.3/src/argstruct/specs/argmap.command.spec
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-01-15 08:31:01.000000 argstruct-1.0.3/src/argstruct/specs/argmap.commands.spec
--rw-rw-rw-   0 root         (0) root         (0)      495 2024-01-15 08:31:01.000000 argstruct-1.0.3/src/argstruct/specs/argmap.root.spec
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-22 09:27:28.258966 argstruct-1.0.3/src/argstruct.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9884 2024-02-22 09:27:28.000000 argstruct-1.0.3/src/argstruct.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      654 2024-02-22 09:27:28.000000 argstruct-1.0.3/src/argstruct.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-22 09:27:28.000000 argstruct-1.0.3/src/argstruct.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2024-02-22 09:27:28.000000 argstruct-1.0.3/src/argstruct.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-02-22 09:27:28.000000 argstruct-1.0.3/src/argstruct.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:25:38.667082 argstruct-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2024-01-15 08:31:01.000000 argstruct-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      147 2024-01-14 21:16:27.000000 argstruct-1.1.0/.gitlab-ci.include.yml
+-rw-rw-rw-   0 root         (0) root         (0)      298 2024-01-14 21:16:27.000000 argstruct-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-14 21:16:27.000000 argstruct-1.1.0/.mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    21013 2024-01-14 21:16:27.000000 argstruct-1.1.0/.pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:25:38.663082 argstruct-1.1.0/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      188 2024-01-14 21:16:27.000000 argstruct-1.1.0/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)   115201 2024-04-15 19:19:17.000000 argstruct-1.1.0/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2024-01-15 21:48:08.000000 argstruct-1.1.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     7088 2024-01-14 21:16:27.000000 argstruct-1.1.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)    10063 2024-04-15 20:25:38.667082 argstruct-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     9244 2024-04-15 19:19:17.000000 argstruct-1.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     3881 2024-04-15 19:19:17.000000 argstruct-1.1.0/project.mk
+-rw-rw-rw-   0 root         (0) root         (0)     1146 2024-04-15 20:25:31.000000 argstruct-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-01-14 21:16:27.000000 argstruct-1.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 20:25:38.667082 argstruct-1.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:25:38.659082 argstruct-1.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:25:38.663082 argstruct-1.1.0/src/argstruct/
+-rw-rw-rw-   0 root         (0) root         (0)     6832 2024-01-15 08:31:01.000000 argstruct-1.1.0/src/argstruct/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2024-04-15 19:19:17.000000 argstruct-1.1.0/src/argstruct/documentation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10391 2024-04-15 19:19:17.000000 argstruct-1.1.0/src/argstruct/object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:25:38.663082 argstruct-1.1.0/src/argstruct/specs/
+-rw-rw-rw-   0 root         (0) root         (0)      129 2024-04-15 19:19:17.000000 argstruct-1.1.0/src/argstruct/specs/DO_NOT_EDIT_THESE.md
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-01-15 08:31:01.000000 argstruct-1.1.0/src/argstruct/specs/argmap.command.args-root.spec
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2024-04-15 19:19:17.000000 argstruct-1.1.0/src/argstruct/specs/argmap.command.args.spec
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2024-01-15 08:31:01.000000 argstruct-1.1.0/src/argstruct/specs/argmap.command.spec
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-01-15 08:31:01.000000 argstruct-1.1.0/src/argstruct/specs/argmap.commands.spec
+-rw-rw-rw-   0 root         (0) root         (0)      495 2024-01-15 08:31:01.000000 argstruct-1.1.0/src/argstruct/specs/argmap.root.spec
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 20:25:38.663082 argstruct-1.1.0/src/argstruct.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10063 2024-04-15 20:25:38.000000 argstruct-1.1.0/src/argstruct.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      695 2024-04-15 20:25:38.000000 argstruct-1.1.0/src/argstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 20:25:38.000000 argstruct-1.1.0/src/argstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-04-15 20:25:38.000000 argstruct-1.1.0/src/argstruct.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-04-15 20:25:38.000000 argstruct-1.1.0/src/argstruct.egg-info/top_level.txt
```

### Comparing `argstruct-1.0.3/.pylintrc` & `argstruct-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `argstruct-1.0.3/Doxyfile` & `argstruct-1.1.0/Doxyfile`

 * *Files 0% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 
 # The PROJECT_NAME tag is a single word (or a sequence of words surrounded by
 # double-quotes, unless you are using Doxywizard) that should identify the
 # project for which the documentation is generated. This name is used in the
 # title of most generated pages and in a few other places.
 # The default value is: My Project.
 
-PROJECT_NAME           = "PROVer Shared Library"
+PROJECT_NAME           = "Reusable Argument Structure"
 
 # The PROJECT_NUMBER tag can be used to enter a project or revision number. This
 # could be handy for archiving the generated documentation or if some version
 # control system is used.
 
-PROJECT_NUMBER = "1.0.3"
+PROJECT_NUMBER = "1.1.0"
 
 # Using the PROJECT_BRIEF tag one can provide an optional one line description
 # for a project that appears at the top of each page and should give viewer a
 # quick idea about the purpose of the project. Keep the description short.
 
 PROJECT_BRIEF          =
```

### Comparing `argstruct-1.0.3/LICENSE.md` & `argstruct-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `argstruct-1.0.3/Makefile` & `argstruct-1.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `argstruct-1.0.3/PKG-INFO` & `argstruct-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argstruct
-Version: 1.0.3
+Version: 1.1.0
 Summary: Reusable Argument Structure
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-argstruct/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-argstruct/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -31,15 +31,15 @@
 
 ## About
 
 This library is intended to provide a structure for Arguments and API/ABI processing in a way that allows for the same structure to be reused for other things without duplication. This allows the same structure to generate documentation, code blocks, and other things, without having to duplicate data elsewhere. 
 
 This library uses the [ArgStruct Specification](https://gitlab.com/accidentallythecable-public/argstruct-spec)
 
-**ArgStruct Specification: 1.0**
+**ArgStruct Specification: 1.1**
 
 ## Usage
 
 First, an [ArgStruct](https://gitlab.com/accidentallythecable-public/argstruct-spec) Map must be created. an ArgStruct is made up of many ArgStructCommands.
 
 Each `ArgStructCommand` requires [some options](SPECS.md#spec-for-argmapcommand) in order to build up a Command. Within each `ArgStructCommand` is a dictionary of arguments (can be converted to a `ArgStructArgument`) and their configurations. Once the [ArgStruct](https://gitlab.com/accidentallythecable-public/argstruct-spec) Map is built, it can be utilized by loading the file (or its contents) into an `ArgStruct` object.
 
@@ -63,14 +63,20 @@
 cli_flag_names = [ "-s", "--some-argument" ]
 help = "My Argument Help info"
 [auth_args.other_argument]
 required = false
 type = "str"
 cli_flag_names = [ "-o", "--other-argument" ]
 help = "My Other Help Info"
+[auth_args.choice_argument]
+required = false
+type = "str"
+cli_flag_names = [ "-c", "--choice-argument" ]
+help = "An argument with allowable values"
+values = [ "a", "foo", "bar" ]
 
 # A new Command with Arguments
 [commands.mycommand]
 auth_required = false
 cli_hidden = true
 api_hidden = false
 help = "My Command Level Help"
```

### Comparing `argstruct-1.0.3/README.md` & `argstruct-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ## About
 
 This library is intended to provide a structure for Arguments and API/ABI processing in a way that allows for the same structure to be reused for other things without duplication. This allows the same structure to generate documentation, code blocks, and other things, without having to duplicate data elsewhere. 
 
 This library uses the [ArgStruct Specification](https://gitlab.com/accidentallythecable-public/argstruct-spec)
 
-**ArgStruct Specification: 1.0**
+**ArgStruct Specification: 1.1**
 
 ## Usage
 
 First, an [ArgStruct](https://gitlab.com/accidentallythecable-public/argstruct-spec) Map must be created. an ArgStruct is made up of many ArgStructCommands.
 
 Each `ArgStructCommand` requires [some options](SPECS.md#spec-for-argmapcommand) in order to build up a Command. Within each `ArgStructCommand` is a dictionary of arguments (can be converted to a `ArgStructArgument`) and their configurations. Once the [ArgStruct](https://gitlab.com/accidentallythecable-public/argstruct-spec) Map is built, it can be utilized by loading the file (or its contents) into an `ArgStruct` object.
 
@@ -45,14 +45,20 @@
 cli_flag_names = [ "-s", "--some-argument" ]
 help = "My Argument Help info"
 [auth_args.other_argument]
 required = false
 type = "str"
 cli_flag_names = [ "-o", "--other-argument" ]
 help = "My Other Help Info"
+[auth_args.choice_argument]
+required = false
+type = "str"
+cli_flag_names = [ "-c", "--choice-argument" ]
+help = "An argument with allowable values"
+values = [ "a", "foo", "bar" ]
 
 # A new Command with Arguments
 [commands.mycommand]
 auth_required = false
 cli_hidden = true
 api_hidden = false
 help = "My Command Level Help"
```

### Comparing `argstruct-1.0.3/project.mk` & `argstruct-1.1.0/project.mk`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 
 PROJECT_OWNER := AccidentallyTheCable
 PROJECT_EMAIL := cableninja@cableninja.net
 PROJECT_FIRST_YEAR := 2023
 PROJECT_LICENSE := GPLv3
 PROJECT_NAME := argstruct
 PROJECT_DESCRIPTION := Reusable Argument Structure
-PROJECT_VERSION := 1.0.0
+PROJECT_VERSION := 1.1.0
 
 ## Enable Feature 'Python'
 BUILD_PYTHON := 1
 ## Enable Feature 'Shell'
 BUILD_SHELL := 0
 ## Enable Feature 'Docker'
 BUILD_DOCKER := 0
 ## Enable python `dist` Phase for Projects destined for PYPI
 PYTHON_PYPI_PROJECT := 1
 ## Additional Flags for pylint. EX --ignore-paths=mypath
 PYLINT_EXTRA_FLAGS := 
 
 ### Any Further Project-specific make targets can go here
 ARGSTRUCT_DIR := $(shell pwd)/spec_doc/
-ARGSTRUCT_SPEC_VERSION := tags/release/1.0
+ARGSTRUCT_SPEC_VERSION := tags/release/1.1
 ARGSTRUCT_SPEC_HOST := gitlab.com
 ARGSTRUCT_SPEC_REPO := accidentallythecable-public/argstruct-spec
 ARGSTRUCT_TAG_VERSION := $(shell echo ${ARGSTRUCT_SPEC_VERSION} | sed -r 's%^tags/(.*)/([0-9]{1,}\.[0-9]{1,}(\.[0-9]{1,})?)$$%\2%g')
 ARGSTRUCT_TAG_TYPE := $(shell echo ${ARGSTRUCT_SPEC_VERSION} | sed -r 's%^tags/(.*)/[0-9]{1,}\.[0-9]{1,}(\.[0-9]{1,})?$$%\1%g')
 
 spec_project_version: spec_check spec_copy  ## Check ArgStruct Git Version, Copy Specker Specs from ArgStruct Spec repo
```

### Comparing `argstruct-1.0.3/pyproject.toml` & `argstruct-1.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "argstruct"
-version = "1.0.3"
+version = "1.1.0"
 authors = [
   { name="AccidentallyTheCable", email="cableninja@cableninja.net" },
 ]
 description = "Reusable Argument Structure"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "GPLv3" }
```

### Comparing `argstruct-1.0.3/src/argstruct/__init__.py` & `argstruct-1.1.0/src/argstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `argstruct-1.0.3/src/argstruct/documentation.py` & `argstruct-1.1.0/src/argstruct/documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     @param ArgStructCmdCallback \c command_callback Method to execute for each Command processed, Arguments: (command,commandStruct,command_options,result), and returns `result` after manipulation
     @param ArgStructArgCallback \c arg_callback Method to execute for each Argument from each Command processed, Arguments (command,commandStruct,argument,argumentStruct,arg_options,result), and returns `result` after manipulation
     @param Any \c command_options Option(s) to pass to the `command_callback`, default `None`
     @param Any \c arg_options Option(s) to pass to the `arg_callback`, default `None`
     @retval str All Commands processed into Markdown documentation (as a string)
     """
     output:str = ""
-    arg_headers:list[str] = [ "API Name", "CLI Flag(s)", "Description", "Required", "Type", "Default" ]
+    arg_headers:list[str] = [ "API Name", "CLI Flag(s)", "Description", "Required", "Type", "Default", "Allowed Values" ]
     if additional_columns is not None:
         arg_headers += additional_columns
     for cmd, cmd_config in commandlist.items():
         can_cli:bool = not cmd_config.get("cli_hidden")
         can_api:bool = not cmd_config.get("api_hidden")
         if not can_api and not can_cli:
             continue
@@ -95,14 +95,16 @@
         arg_row.append(arg_data["help"])
         arg_row.append("**Y**" if arg_data["required"] else "**N**")
         arg_row.append(arg_data["type"])
         if "default" in arg_data.keys():
             arg_row.append(str(arg_data["default"]))
         else:
             arg_row.append("**NONE**")
+        if "values" in arg_data.keys() and arg_data["values"] is not None:
+            arg_row.append(', '.join(arg_data["values"]))
         if arg_callback is not None:
             arg_row = arg_callback(command,command_config,arg,arg_data,arg_options,arg_row)
         out_list.append(arg_row)
     return out_list
 
 def markdown_documentation(
         argmap_file:Path,
@@ -124,15 +126,15 @@
     @retval str Processed Documentation
     For `command_callback` the `result` is a str rendered between access method and arguments
     For `arg_callback` the `result` is a list[str] of the current argument table row
     """
     argstruct_obj:ArgStruct = ArgStruct(argmap_file,ArgStruct.OVERRIDE_TYPE_TOML)
     argmap_data:dict[str,dict[str,ArgStructCommand]] = argstruct_obj.grouped
     auth_args:dict[str,dict[str,typing.Any]] = argstruct_obj.get("auth_args")
-    arg_headers:list[str] = [ "API Name", "CLI Flag(s)", "Description", "Required", "Type", "Default" ]
+    arg_headers:list[str] = [ "API Name", "CLI Flag(s)", "Description", "Required", "Type", "Default", "Allowed Values" ]
     if additional_columns is not None:
         arg_headers += additional_columns
     output:str = ""
     if len(auth_args) > 0:
         output += "## Authorization Arguments\n"
         autharg_table:list[list[str]] = [ arg_headers ]
         autharg_table += _build_doc_argmap("empty",ArgStruct.empty,auth_args,arg_callback,arg_options)
```

### Comparing `argstruct-1.0.3/src/argstruct/object.py` & `argstruct-1.1.0/src/argstruct/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             empty_command:dict[str,typing.Any] = {
                 "auth_required": False,
                 "cli_hidden": True,
                 "api_hidden": True,
                 "help": "EMPTY",
                 "group": "EMPTY",
                 "ui_label": "EMPTY",
+                "values": None,
             }
             ArgStruct.empty = ArgStructCommand(empty_command)
         self._argmap = merged_map
 
     def _build_maps(self) -> None:
         """Build ArgStructs
         @retval None Nothing
@@ -174,14 +175,16 @@
         }
         if arg_config["required"]:
             kargs["required"] = arg_config["required"]
         if arg_config["multi"]:
             kargs["nargs"] = "+"
         if arg_config["type"] == "bool":
             kargs["action"] = "store_true"
+        if arg_config["values"] is not None:
+            kargs["choices"] = arg_config["values"]
         if "default" in arg_config.keys():
             kargs["default"] = arg_config["default"]
         parser.add_argument(*aargs,**kargs)
 
     @staticmethod
     def validate(spec_name:str,argmap:dict[typing.Any,typing.Any]) -> bool:
         """Explicitly Validate ArgStruct Block
```

### Comparing `argstruct-1.0.3/src/argstruct/specs/argmap.command.args-root.spec` & `argstruct-1.1.0/src/argstruct/specs/argmap.command.args-root.spec`

 * *Files identical despite different names*

### Comparing `argstruct-1.0.3/src/argstruct/specs/argmap.command.args.spec` & `argstruct-1.1.0/src/argstruct/specs/argmap.command.args.spec`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'values'": "OrderedDict([('type', 'list'), ('required', False), ('default', None), ('comment', "*

 * *             "'Allowable values for argument'), ('example', ['a', 'foo', 'bar'])])"}*

```diff
@@ -45,9 +45,20 @@
             "str",
             "int",
             "list",
             "dict",
             "float",
             "bool"
         ]
+    },
+    "values": {
+        "comment": "Allowable values for argument",
+        "default": null,
+        "example": [
+            "a",
+            "foo",
+            "bar"
+        ],
+        "required": false,
+        "type": "list"
     }
 }
```

### Comparing `argstruct-1.0.3/src/argstruct/specs/argmap.command.spec` & `argstruct-1.1.0/src/argstruct/specs/argmap.command.spec`

 * *Files identical despite different names*

### Comparing `argstruct-1.0.3/src/argstruct.egg-info/PKG-INFO` & `argstruct-1.1.0/src/argstruct.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argstruct
-Version: 1.0.3
+Version: 1.1.0
 Summary: Reusable Argument Structure
 Author-email: AccidentallyTheCable <cableninja@cableninja.net>
 License: GPLv3
 Project-URL: Homepage, https://gitlab.com/accidentallythecable-public/python-modules/python-argstruct/
 Project-URL: Bug Tracker, https://gitlab.com/accidentallythecable-public/python-modules/python-argstruct/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -31,15 +31,15 @@
 
 ## About
 
 This library is intended to provide a structure for Arguments and API/ABI processing in a way that allows for the same structure to be reused for other things without duplication. This allows the same structure to generate documentation, code blocks, and other things, without having to duplicate data elsewhere. 
 
 This library uses the [ArgStruct Specification](https://gitlab.com/accidentallythecable-public/argstruct-spec)
 
-**ArgStruct Specification: 1.0**
+**ArgStruct Specification: 1.1**
 
 ## Usage
 
 First, an [ArgStruct](https://gitlab.com/accidentallythecable-public/argstruct-spec) Map must be created. an ArgStruct is made up of many ArgStructCommands.
 
 Each `ArgStructCommand` requires [some options](SPECS.md#spec-for-argmapcommand) in order to build up a Command. Within each `ArgStructCommand` is a dictionary of arguments (can be converted to a `ArgStructArgument`) and their configurations. Once the [ArgStruct](https://gitlab.com/accidentallythecable-public/argstruct-spec) Map is built, it can be utilized by loading the file (or its contents) into an `ArgStruct` object.
 
@@ -63,14 +63,20 @@
 cli_flag_names = [ "-s", "--some-argument" ]
 help = "My Argument Help info"
 [auth_args.other_argument]
 required = false
 type = "str"
 cli_flag_names = [ "-o", "--other-argument" ]
 help = "My Other Help Info"
+[auth_args.choice_argument]
+required = false
+type = "str"
+cli_flag_names = [ "-c", "--choice-argument" ]
+help = "An argument with allowable values"
+values = [ "a", "foo", "bar" ]
 
 # A new Command with Arguments
 [commands.mycommand]
 auth_required = false
 cli_hidden = true
 api_hidden = false
 help = "My Command Level Help"
```

### Comparing `argstruct-1.0.3/src/argstruct.egg-info/SOURCES.txt` & `argstruct-1.1.0/src/argstruct.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 src/argstruct/documentation.py
 src/argstruct/object.py
 src/argstruct.egg-info/PKG-INFO
 src/argstruct.egg-info/SOURCES.txt
 src/argstruct.egg-info/dependency_links.txt
 src/argstruct.egg-info/entry_points.txt
 src/argstruct.egg-info/top_level.txt
+src/argstruct/specs/DO_NOT_EDIT_THESE.md
 src/argstruct/specs/argmap.command.args-root.spec
 src/argstruct/specs/argmap.command.args.spec
 src/argstruct/specs/argmap.command.spec
 src/argstruct/specs/argmap.commands.spec
 src/argstruct/specs/argmap.root.spec
```

