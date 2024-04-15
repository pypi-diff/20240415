# Comparing `tmp/yamlex-1.0.7.tar.gz` & `tmp/yamlex-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamlex-1.0.7.tar", max compression
+gzip compressed data, was "yamlex-1.0.9.tar", max compression
```

## Comparing `yamlex-1.0.7.tar` & `yamlex-1.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11343 2024-03-21 00:02:39.363447 yamlex-1.0.7/LICENSE
--rw-r--r--   0        0        0    12332 2024-03-21 05:54:01.011515 yamlex-1.0.7/README.md
--rw-r--r--   0        0        0     1074 2024-03-22 12:11:48.055228 yamlex-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 23:58:07.038813 yamlex-1.0.7/yamlex/__init__.py
--rw-r--r--   0        0        0       66 2024-03-19 02:14:38.010009 yamlex-1.0.7/yamlex/__main__.py
--rw-r--r--   0        0        0    10987 2024-03-22 12:28:56.074694 yamlex-1.0.7/yamlex/cli.py
--rw-r--r--   0        0        0     4481 2024-03-22 12:25:34.806557 yamlex-1.0.7/yamlex/joiner.py
--rw-r--r--   0        0        0     9371 2024-03-20 22:49:39.847130 yamlex-1.0.7/yamlex/mapper.py
--rw-r--r--   0        0        0     9081 2024-03-21 05:07:58.114296 yamlex-1.0.7/yamlex/splitter.py
--rw-r--r--   0        0        0     3242 2024-03-22 12:36:29.601749 yamlex-1.0.7/yamlex/util.py
--rw-r--r--   0        0        0    13489 1970-01-01 00:00:00.000000 yamlex-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-03-21 00:02:39.363447 yamlex-1.0.9/LICENSE
+-rw-r--r--   0        0        0    12510 2024-03-22 14:45:45.040213 yamlex-1.0.9/README.md
+-rw-r--r--   0        0        0     1074 2024-03-22 16:34:21.442890 yamlex-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 23:58:07.038813 yamlex-1.0.9/yamlex/__init__.py
+-rw-r--r--   0        0        0       66 2024-03-19 02:14:38.010009 yamlex-1.0.9/yamlex/__main__.py
+-rw-r--r--   0        0        0    11226 2024-03-22 16:31:48.388811 yamlex-1.0.9/yamlex/cli.py
+-rw-r--r--   0        0        0     4481 2024-03-22 12:25:34.806557 yamlex-1.0.9/yamlex/joiner.py
+-rw-r--r--   0        0        0     9371 2024-03-20 22:49:39.847130 yamlex-1.0.9/yamlex/mapper.py
+-rw-r--r--   0        0        0     9081 2024-03-21 05:07:58.114296 yamlex-1.0.9/yamlex/splitter.py
+-rw-r--r--   0        0        0     3118 2024-03-22 16:29:52.213166 yamlex-1.0.9/yamlex/util.py
+-rw-r--r--   0        0        0    13667 1970-01-01 00:00:00.000000 yamlex-1.0.9/PKG-INFO
```

### Comparing `yamlex-1.0.7/LICENSE` & `yamlex-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `yamlex-1.0.7/README.md` & `yamlex-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,27 +57,29 @@
 # Help message
 $ yamlex join --help
  Usage: yamlex join [OPTIONS]                                                          
                                                                                        
  Join YAML files into a single file.                                                   
                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
-│ --source   -s      DIRECTORY  Path to directory where split YAML source files are   │
-│                               stored. [default: source or src/source]                 │
-│ --target   -t      FILE       Path for target extension.yaml file that will be      │
+│ --source     -s    DIRECTORY  Path to directory where split YAML source files are   │
+│                               stored. [default: source or src/source]               │
+│ --target     -t    FILE       Path for target extension.yaml file that will be      │
 │                               assembled from parts. [default:                       │
 │                               extension/extension.yaml or                           │
 │                               src/extension/extension.yaml]                         │
-│ --dev      -d                 Prefix extension name with 'custom:' and use explicit │
+│ --dev        -d               Prefix extension name with 'custom:' and use explicit │
 │                               version.                                              │
-│ --bump     -b                 Bump version in the version.properties file.          │
-│ --version  -v      TEXT       Explicitly set the version to use during assembly or  │
+│ --bump       -b               Bump version in the version.properties file.          │
+│ --multiline  -m               Non YAML files are embedded as multiline strings.     │
+│                               [default: True]                                       │
+│ --version    -v    TEXT       Explicitly set the version to use during assembly or  │
 │                               bump process.                                         │
 │                               [default: None]                                       │
-│ --force    -f                 Overwrite the files even if they were created         │
+│ --force      -f               Overwrite the files even if they were created         │
 │                               manually.                                             │
 │ --verbose                     Enable verbose output.                                │
 │ --quiet                       Disable any informational output. Only errors.        │
 │ --help                        Show this message and exit.                           │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
@@ -164,15 +166,15 @@
 │                             [default: .vscode/settings.json]                        │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
 │ --json            -j      DIRECTORY  Path to directory with valid extensions JSON   │
 │                                      schema files.                                  │
 │                                      [default: schema]                              │
 │ --source          -s      DIRECTORY  Path to directory where YAML source files will │
-│                                      be stored. [default: source or src/source]       │
+│                                      be stored. [default: source or src/source]     │
 │ --root            -r      DIRECTORY  Root directory relative to which the paths in  │
 │                                      settings file will be mapped.                  │
 │                                      [default: .]                                   │
 │ --extension-yaml  -e      FILE       Path to output extension.yaml file. [default:  │
 │                                      extension/extension.yaml or                    │
 │                                      src/extension/extension.yaml]                  │
 │ --verbose                            Enable verbose output.                         │
@@ -205,15 +207,15 @@
  Split central YAML file into parts.                                                   
                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
 │ --source   -s      FILE       Path to source extension.yaml file. [default:         │
 │                               extension/extension.yaml or                           │
 │                               src/extension/extension.yaml]                         │
 │ --target   -t      DIRECTORY  Path to directory where split YAML source files will  │
-│                               be stored. [default: source or src/source]              │
+│                               be stored. [default: source or src/source]            │
 │ --force    -f                 Overwrite the files even if they were created         │
 │                               manually.                                             │
 │ --verbose                     Enable verbose output.                                │
 │ --quiet                       Disable any informational output. Only errors.        │
 │ --help                        Show this message and exit.                           │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ```
```

#### html2text {}

```diff
@@ -25,19 +25,21 @@
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --source -s DIRECTORY Path to directory where split YAML source files are
 â â stored. [default: source or src/source] â â --target -t FILE Path
 for target extension.yaml file that will be â â assembled from parts.
 [default: â â extension/extension.yaml or â â src/extension/
 extension.yaml] â â --dev -d Prefix extension name with 'custom:' and use
 explicit â â version. â â --bump -b Bump version in the
-version.properties file. â â --version -v TEXT Explicitly set the version
-to use during assembly or â â bump process. â â [default: None] â â
---force -f Overwrite the files even if they were created â â manually. â
-â --verbose Enable verbose output. â â --quiet Disable any informational
-output. Only errors. â â --help Show this message and exit. â
+version.properties file. â â --multiline -m Non YAML files are embedded as
+multiline strings. â â [default: True] â â --version -v TEXT Explicitly
+set the version to use during assembly or â â bump process. â â
+[default: None] â â --force -f Overwrite the files even if they were
+created â â manually. â â --verbose Enable verbose output. â â --
+quiet Disable any informational output. Only errors. â â --help Show this
+message and exit. â
 â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 ``` When assembling, the `join` command will avoid overwriting a manually
 created `extension.yaml` file. The way it detects that the file is manually
 created is by checking whether the file contains the following comment:
 *generated by yamlex*. In order to overwrite this safety check, you can launch
 the `join` command with the `--force` flag. #### Folder structure The way
 `yamlex` assembles the `extension.yaml` from parts is by parsing the `--source`
```

### Comparing `yamlex-1.0.7/pyproject.toml` & `yamlex-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 maintainers = ["Vagiz Duseev <vagiz.duseev@dynatrace.com>"]
 name = "yamlex"
 packages = [
   {include = "yamlex"},
 ]
 readme = "README.md"
 repository = "https://github.com/dynatrace-extensions/dt-extensions-yamlex"
-version = "1.0.7"
+version = "1.0.9"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 wheel = "^0"
 typer = "^0.9"
 typing-extensions = "^4"
 ruamel-yaml = "^0.18"
```

### Comparing `yamlex-1.0.7/yamlex/cli.py` & `yamlex-1.0.9/yamlex/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     remove_yaml_comments,
 )
 from yamlex.util import (
     adjust_root_logger,
     get_default_extension_dir_path,
     get_default_extension_source_dir_path,
     is_manually_created,
-    write_file_with_generated_comment,
+    write_file,
     read_version,
     write_version,
 )
 
 
 logging.basicConfig(level=logging.INFO, format="%(message)s")
 
@@ -43,14 +43,22 @@
     bool,
     typer.Option(
         "--force",
         "-f",
         help="Overwrite the files even if they were created manually.",
     ),
 ]
+comment_option = Annotated[
+    str,
+    typer.Option(
+        "--comment",
+        "-c",
+        help="Comment to add at the top of the YAML.",
+    ),
+]
 verbose_option = Annotated[
     bool,
     typer.Option(
         "--verbose",
         help="Enable verbose output.",
     ),
 ]
@@ -184,15 +192,15 @@
                 "[dim]\\[default: extension/extension.yaml or src/extension/extension.yaml][/dim]"
             ),
             show_default=False,
             dir_okay=False,
             file_okay=True,
             exists=True,
             readable=True,
-        )
+        ),
     ] = None,
     target: Annotated[
         Optional[Path],
         typer.Option(
             "--target",
             "-t",
             help=(
@@ -200,16 +208,17 @@
                 "[dim]\\[default: source or src/source][/dim]"
             ),
             show_default=False,
             dir_okay=True,
             file_okay=False,
             exists=True,
             writable=True,
-        )
+        ),
     ] = None,
+    comment: comment_option = 'This file was generated by yamlex',
     force: force_option = False,
     verbose: verbose_option = False,
     quiet: quiet_option = False,
 ):
     adjust_root_logger(verbose, quiet)
 
     source = source or get_default_extension_dir_path() / "extension.yaml"
@@ -220,15 +229,15 @@
 
     split_parts = split_yaml(source, target)
 
     for path, part in split_parts.items():
         if is_manually_created(path) and not force:
             logger.info(f"(Skipping) Part: {path}")
         else:
-            write_file_with_generated_comment(path, part)
+            write_file(path, part, comment)
             logger.info(f"Part written: {path}")
 
 
 @app.command(help="Join YAML files into a single file.")
 def join(
     source: Annotated[
         Optional[Path],
@@ -288,14 +297,15 @@
         Optional[str],
         typer.Option(
             "--version",
             "-v",
             help="Explicitly set the version to use during assembly or bump process."
         ),
     ] = None,
+    comment: comment_option = 'This file was generated by yamlex',
     force: force_option = False,
     verbose: verbose_option = False,
     quiet: quiet_option = False,
     debug: debug_option = False,
 ):
     adjust_root_logger(verbose, quiet)
     
@@ -362,15 +372,15 @@
         logger.error(f"The {target} file was created manually. Use --force to overwrite it.")
         exit(2)
 
     # Remove comments
     remove_yaml_comments(extension)
 
     # Write to output file
-    write_file_with_generated_comment(target, extension)
+    write_file(target, extension, comment)
 
     if debug:
         print(extension)
 
 
 def run():
     app.command(name="j", hidden=True)(join)
```

### Comparing `yamlex-1.0.7/yamlex/joiner.py` & `yamlex-1.0.9/yamlex/joiner.py`

 * *Files identical despite different names*

### Comparing `yamlex-1.0.7/yamlex/mapper.py` & `yamlex-1.0.9/yamlex/mapper.py`

 * *Files identical despite different names*

### Comparing `yamlex-1.0.7/yamlex/splitter.py` & `yamlex-1.0.9/yamlex/splitter.py`

 * *Files identical despite different names*

### Comparing `yamlex-1.0.7/yamlex/util.py` & `yamlex-1.0.9/yamlex/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,44 +52,38 @@
 
 def is_manually_created(path: Path) -> bool:
     if path.exists():
         with open(path, "r") as f:
             content = f.read()
             if "generated by yamlex" not in content:
                 True
-    return False       
+    return False
 
 
-def get_generated_content_comment() -> str:
-    comment = (
-        "# This file was generated by yamlex\n"
-        "\n"
-    )
-    return comment
-
-
-def write_file_with_generated_comment(
+def write_file(
     file_path: Path,
     data: Union[dict, list],
+    comment: Optional[str] = None,
 ) -> None:
     # Convert dict to YAML. Dump to string first to add a comment
     stream = StringIO()
     parser.indent(mapping=2, sequence=4, offset=2)
     parser.dump(data, stream)
     text = stream.getvalue()
 
     # Make sure the directory we write to exists
     dir = file_path.parent.resolve()
     dir.mkdir(parents=True, exist_ok=True)
 
     # Write to output file
     with open(file_path, "w") as f:
-        # Write a comment to indicate that the file was automatically generated
-        comment = get_generated_content_comment()
-        f.write(comment)
+        if comment:
+            # Write a comment to indicate that the file was automatically generated
+            comment = f"# {comment}\n\n"
+            f.write(comment)
         f.write(text)
 
 
 def read_version(path: Path, default: Optional[str] = None) -> str:
     try:
         with open(path, "r") as f:
             content = f.read()
```

### Comparing `yamlex-1.0.7/PKG-INFO` & `yamlex-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamlex
-Version: 1.0.7
+Version: 1.0.9
 Summary: Command-line tool to simplify development of Dynatrace Extensions with big YAML
 Home-page: https://github.com/dynatrace-extensions/dt-extensions-yaml-assembler
 License: Apache-2.0
 Keywords: dynatrace,cli,extensions
 Author: Vagiz Duseev
 Author-email: vagiz.duseev@dynatrace.com
 Maintainer: Vagiz Duseev
@@ -84,27 +84,29 @@
 # Help message
 $ yamlex join --help
  Usage: yamlex join [OPTIONS]                                                          
                                                                                        
  Join YAML files into a single file.                                                   
                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
-│ --source   -s      DIRECTORY  Path to directory where split YAML source files are   │
-│                               stored. [default: source or src/source]                 │
-│ --target   -t      FILE       Path for target extension.yaml file that will be      │
+│ --source     -s    DIRECTORY  Path to directory where split YAML source files are   │
+│                               stored. [default: source or src/source]               │
+│ --target     -t    FILE       Path for target extension.yaml file that will be      │
 │                               assembled from parts. [default:                       │
 │                               extension/extension.yaml or                           │
 │                               src/extension/extension.yaml]                         │
-│ --dev      -d                 Prefix extension name with 'custom:' and use explicit │
+│ --dev        -d               Prefix extension name with 'custom:' and use explicit │
 │                               version.                                              │
-│ --bump     -b                 Bump version in the version.properties file.          │
-│ --version  -v      TEXT       Explicitly set the version to use during assembly or  │
+│ --bump       -b               Bump version in the version.properties file.          │
+│ --multiline  -m               Non YAML files are embedded as multiline strings.     │
+│                               [default: True]                                       │
+│ --version    -v    TEXT       Explicitly set the version to use during assembly or  │
 │                               bump process.                                         │
 │                               [default: None]                                       │
-│ --force    -f                 Overwrite the files even if they were created         │
+│ --force      -f               Overwrite the files even if they were created         │
 │                               manually.                                             │
 │ --verbose                     Enable verbose output.                                │
 │ --quiet                       Disable any informational output. Only errors.        │
 │ --help                        Show this message and exit.                           │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
@@ -191,15 +193,15 @@
 │                             [default: .vscode/settings.json]                        │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
 │ --json            -j      DIRECTORY  Path to directory with valid extensions JSON   │
 │                                      schema files.                                  │
 │                                      [default: schema]                              │
 │ --source          -s      DIRECTORY  Path to directory where YAML source files will │
-│                                      be stored. [default: source or src/source]       │
+│                                      be stored. [default: source or src/source]     │
 │ --root            -r      DIRECTORY  Root directory relative to which the paths in  │
 │                                      settings file will be mapped.                  │
 │                                      [default: .]                                   │
 │ --extension-yaml  -e      FILE       Path to output extension.yaml file. [default:  │
 │                                      extension/extension.yaml or                    │
 │                                      src/extension/extension.yaml]                  │
 │ --verbose                            Enable verbose output.                         │
@@ -232,15 +234,15 @@
  Split central YAML file into parts.                                                   
                                                                                        
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
 │ --source   -s      FILE       Path to source extension.yaml file. [default:         │
 │                               extension/extension.yaml or                           │
 │                               src/extension/extension.yaml]                         │
 │ --target   -t      DIRECTORY  Path to directory where split YAML source files will  │
-│                               be stored. [default: source or src/source]              │
+│                               be stored. [default: source or src/source]            │
 │ --force    -f                 Overwrite the files even if they were created         │
 │                               manually.                                             │
 │ --verbose                     Enable verbose output.                                │
 │ --quiet                       Disable any informational output. Only errors.        │
 │ --help                        Show this message and exit.                           │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: yamlex Version: 1.0.7 Summary: Command-line tool to
+Metadata-Version: 2.1 Name: yamlex Version: 1.0.9 Summary: Command-line tool to
 simplify development of Dynatrace Extensions with big YAML Home-page: https://
 github.com/dynatrace-extensions/dt-extensions-yaml-assembler License: Apache-
 2.0 Keywords: dynatrace,cli,extensions Author: Vagiz Duseev Author-email:
 vagiz.duseev@dynatrace.com Maintainer: Vagiz Duseev Maintainer-email:
 vagiz.duseev@dynatrace.com Requires-Python: >=3.9,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
@@ -40,19 +40,21 @@
 ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ®
 â --source -s DIRECTORY Path to directory where split YAML source files are
 â â stored. [default: source or src/source] â â --target -t FILE Path
 for target extension.yaml file that will be â â assembled from parts.
 [default: â â extension/extension.yaml or â â src/extension/
 extension.yaml] â â --dev -d Prefix extension name with 'custom:' and use
 explicit â â version. â â --bump -b Bump version in the
-version.properties file. â â --version -v TEXT Explicitly set the version
-to use during assembly or â â bump process. â â [default: None] â â
---force -f Overwrite the files even if they were created â â manually. â
-â --verbose Enable verbose output. â â --quiet Disable any informational
-output. Only errors. â â --help Show this message and exit. â
+version.properties file. â â --multiline -m Non YAML files are embedded as
+multiline strings. â â [default: True] â â --version -v TEXT Explicitly
+set the version to use during assembly or â â bump process. â â
+[default: None] â â --force -f Overwrite the files even if they were
+created â â manually. â â --verbose Enable verbose output. â â --
+quiet Disable any informational output. Only errors. â â --help Show this
+message and exit. â
 â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
 ``` When assembling, the `join` command will avoid overwriting a manually
 created `extension.yaml` file. The way it detects that the file is manually
 created is by checking whether the file contains the following comment:
 *generated by yamlex*. In order to overwrite this safety check, you can launch
 the `join` command with the `--force` flag. #### Folder structure The way
 `yamlex` assembles the `extension.yaml` from parts is by parsing the `--source`
```

