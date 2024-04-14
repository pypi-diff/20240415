# Comparing `tmp/clean_dotenv-0.0.6.tar.gz` & `tmp/clean_dotenv-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clean_dotenv-0.0.6.tar", last modified: Fri Mar 29 00:57:35 2024, max compression
+gzip compressed data, was "clean_dotenv-0.0.7.tar", last modified: Sun Apr 14 22:28:42 2024, max compression
```

## Comparing `clean_dotenv-0.0.6.tar` & `clean_dotenv-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hilko      (501) staff       (20)        0 2024-03-29 00:57:35.924978 clean_dotenv-0.0.6/
--rw-r--r--   0 hilko      (501) staff       (20)     1062 2024-02-17 13:05:42.000000 clean_dotenv-0.0.6/LICENSE
--rw-r--r--   0 hilko      (501) staff       (20)     4108 2024-03-29 00:57:35.924858 clean_dotenv-0.0.6/PKG-INFO
--rw-r--r--   0 hilko      (501) staff       (20)     3443 2024-03-23 13:51:13.000000 clean_dotenv-0.0.6/README.md
-drwxr-xr-x   0 hilko      (501) staff       (20)        0 2024-03-29 00:57:35.923105 clean_dotenv-0.0.6/clean_dotenv/
--rw-r--r--   0 hilko      (501) staff       (20)        0 2024-03-29 00:56:17.000000 clean_dotenv-0.0.6/clean_dotenv/__init__.py
--rw-r--r--   0 hilko      (501) staff       (20)      129 2024-03-29 00:56:17.000000 clean_dotenv-0.0.6/clean_dotenv/__main__.py
--rw-r--r--   0 hilko      (501) staff       (20)     2473 2024-03-29 00:56:17.000000 clean_dotenv-0.0.6/clean_dotenv/_main.py
--rw-r--r--   0 hilko      (501) staff       (20)     7721 2024-03-29 00:56:17.000000 clean_dotenv-0.0.6/clean_dotenv/_parser.py
-drwxr-xr-x   0 hilko      (501) staff       (20)        0 2024-03-29 00:57:35.924488 clean_dotenv-0.0.6/clean_dotenv.egg-info/
--rw-r--r--   0 hilko      (501) staff       (20)     4108 2024-03-29 00:57:35.000000 clean_dotenv-0.0.6/clean_dotenv.egg-info/PKG-INFO
--rw-r--r--   0 hilko      (501) staff       (20)      315 2024-03-29 00:57:35.000000 clean_dotenv-0.0.6/clean_dotenv.egg-info/SOURCES.txt
--rw-r--r--   0 hilko      (501) staff       (20)        1 2024-03-29 00:57:35.000000 clean_dotenv-0.0.6/clean_dotenv.egg-info/dependency_links.txt
--rw-r--r--   0 hilko      (501) staff       (20)       57 2024-03-29 00:57:35.000000 clean_dotenv-0.0.6/clean_dotenv.egg-info/entry_points.txt
--rw-r--r--   0 hilko      (501) staff       (20)       13 2024-03-29 00:57:35.000000 clean_dotenv-0.0.6/clean_dotenv.egg-info/top_level.txt
--rw-r--r--   0 hilko      (501) staff       (20)     1219 2024-03-29 00:57:35.925513 clean_dotenv-0.0.6/setup.cfg
--rw-r--r--   0 hilko      (501) staff       (20)       74 2024-02-17 14:01:23.000000 clean_dotenv-0.0.6/setup.py
+drwxr-xr-x   0 hilko      (501) staff       (20)        0 2024-04-14 22:28:42.954838 clean_dotenv-0.0.7/
+-rw-r--r--   0 hilko      (501) staff       (20)     1062 2024-02-17 13:05:42.000000 clean_dotenv-0.0.7/LICENSE
+-rw-r--r--   0 hilko      (501) staff       (20)     4270 2024-04-14 22:28:42.954727 clean_dotenv-0.0.7/PKG-INFO
+-rw-r--r--   0 hilko      (501) staff       (20)     3605 2024-04-14 22:26:13.000000 clean_dotenv-0.0.7/README.md
+drwxr-xr-x   0 hilko      (501) staff       (20)        0 2024-04-14 22:28:42.952398 clean_dotenv-0.0.7/clean_dotenv/
+-rw-r--r--   0 hilko      (501) staff       (20)        0 2024-03-29 00:56:17.000000 clean_dotenv-0.0.7/clean_dotenv/__init__.py
+-rw-r--r--   0 hilko      (501) staff       (20)      129 2024-03-29 00:56:17.000000 clean_dotenv-0.0.7/clean_dotenv/__main__.py
+-rw-r--r--   0 hilko      (501) staff       (20)     3064 2024-04-14 22:24:11.000000 clean_dotenv-0.0.7/clean_dotenv/_main.py
+-rw-r--r--   0 hilko      (501) staff       (20)     7721 2024-03-29 00:56:17.000000 clean_dotenv-0.0.7/clean_dotenv/_parser.py
+drwxr-xr-x   0 hilko      (501) staff       (20)        0 2024-04-14 22:28:42.954186 clean_dotenv-0.0.7/clean_dotenv.egg-info/
+-rw-r--r--   0 hilko      (501) staff       (20)     4270 2024-04-14 22:28:42.000000 clean_dotenv-0.0.7/clean_dotenv.egg-info/PKG-INFO
+-rw-r--r--   0 hilko      (501) staff       (20)      315 2024-04-14 22:28:42.000000 clean_dotenv-0.0.7/clean_dotenv.egg-info/SOURCES.txt
+-rw-r--r--   0 hilko      (501) staff       (20)        1 2024-04-14 22:28:42.000000 clean_dotenv-0.0.7/clean_dotenv.egg-info/dependency_links.txt
+-rw-r--r--   0 hilko      (501) staff       (20)       57 2024-04-14 22:28:42.000000 clean_dotenv-0.0.7/clean_dotenv.egg-info/entry_points.txt
+-rw-r--r--   0 hilko      (501) staff       (20)       13 2024-04-14 22:28:42.000000 clean_dotenv-0.0.7/clean_dotenv.egg-info/top_level.txt
+-rw-r--r--   0 hilko      (501) staff       (20)     1219 2024-04-14 22:28:42.955356 clean_dotenv-0.0.7/setup.cfg
+-rw-r--r--   0 hilko      (501) staff       (20)       74 2024-02-17 14:01:23.000000 clean_dotenv-0.0.7/setup.py
```

### Comparing `clean_dotenv-0.0.6/LICENSE` & `clean_dotenv-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clean_dotenv-0.0.6/PKG-INFO` & `clean_dotenv-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean_dotenv
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatically creates an .env.example which creates the same keys as your .env file, but without the values
 Home-page: https://github.com/hija/clean-dotenv
 Author: Hilko (hija)
 Author-email: mail@hilko.eu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,16 +33,16 @@
 ```
 
 An `.env` file should not be commited into a repo, since it can contain sensitive information[^1] (you should probably adding the `.env` file into your `.gitignore`). However, one needs to know which variables can be set in the `.env` file and as a result, a lot of projects (such as laravel), provide an `.env.example` file which is a template file. So you would copy the `.env.template`, rename it to `.env` and fill in the environment variables.
 
 However, there is one issue with this approach: If one introduces a new environment variable, they need to remember to add it to the `.env.example` file. Unfortunately, if they forget this, it will not be noticed, since the program is using the `.env` file and not the `.env.example`. This pre-commit hook tries to mitigate this problem by creating an `.env.example` file automatically (based on your `.env` file), so the example `.env` file would become the following `.env.example`:
 
 ```bash
-OPENAI_KEY=
-S3_BUCKET_NAME=
+OPENAI_KEY=""
+S3_BUCKET_NAME=""
 ```
 
 [^1]: https://www.zdnet.com/article/botnets-have-been-silently-mass-scanning-the-internet-for-unsecured-env-files/
  
 ## Installation
 
 ```bash
@@ -52,25 +52,26 @@
 
 ## Console scripts
 
 Consult `clean-dotenv --help` for the full set of options.
 
 Common options:
 
-- `--root path`: Defines the root path in which to look for .env files. This is **not recursive**
+- `--root_path`: Defines the root path in which to look for .env files. This is **not recursive**
+- `--keep value1 value2`: Defines which values shall be kept in the .env file. In this example, every variable except for value1 and value2 would be cleaned.
 
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/hija/clean-dotenv
-    rev: v0.0.5
+    rev: v0.0.7
     hooks:
     -   id: clean-dotenv
 ```
 
 ## What does it do?
 The tool looks for `.env` files in all directories and creates a new, corresponding filename `.env.example` which is save to commit, since it contains all the keys from your `.env` file, but without its values.
```

### Comparing `clean_dotenv-0.0.6/README.md` & `clean_dotenv-0.0.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 ```
 
 An `.env` file should not be commited into a repo, since it can contain sensitive information[^1] (you should probably adding the `.env` file into your `.gitignore`). However, one needs to know which variables can be set in the `.env` file and as a result, a lot of projects (such as laravel), provide an `.env.example` file which is a template file. So you would copy the `.env.template`, rename it to `.env` and fill in the environment variables.
 
 However, there is one issue with this approach: If one introduces a new environment variable, they need to remember to add it to the `.env.example` file. Unfortunately, if they forget this, it will not be noticed, since the program is using the `.env` file and not the `.env.example`. This pre-commit hook tries to mitigate this problem by creating an `.env.example` file automatically (based on your `.env` file), so the example `.env` file would become the following `.env.example`:
 
 ```bash
-OPENAI_KEY=
-S3_BUCKET_NAME=
+OPENAI_KEY=""
+S3_BUCKET_NAME=""
 ```
 
 [^1]: https://www.zdnet.com/article/botnets-have-been-silently-mass-scanning-the-internet-for-unsecured-env-files/
  
 ## Installation
 
 ```bash
@@ -35,25 +35,26 @@
 
 ## Console scripts
 
 Consult `clean-dotenv --help` for the full set of options.
 
 Common options:
 
-- `--root path`: Defines the root path in which to look for .env files. This is **not recursive**
+- `--root_path`: Defines the root path in which to look for .env files. This is **not recursive**
+- `--keep value1 value2`: Defines which values shall be kept in the .env file. In this example, every variable except for value1 and value2 would be cleaned.
 
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/hija/clean-dotenv
-    rev: v0.0.5
+    rev: v0.0.7
     hooks:
     -   id: clean-dotenv
 ```
 
 ## What does it do?
 The tool looks for `.env` files in all directories and creates a new, corresponding filename `.env.example` which is save to commit, since it contains all the keys from your `.env` file, but without its values.
```

### Comparing `clean_dotenv-0.0.6/clean_dotenv/_main.py` & `clean_dotenv-0.0.7/clean_dotenv/_main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import argparse
-from typing import Iterator
+from typing import Iterator, List
 import clean_dotenv._parser as DotEnvParser
 
 
-def _clean_env(path_to_env: str):
+def _clean_env(path_to_env: str, values_to_keep: List[str] = []):
     # Open the .env file and remove the sensitive data
     # We rely on python-dotenv to parse the file, since we do not want to write our own parser
     dotenv_elements = DotEnvParser.parse_stream(open(path_to_env))
 
     # Create new filename for the .env file --> test.env becomes test.env.example
     path_to_example_file = path_to_env + ".example"
 
@@ -18,15 +18,19 @@
         for i, dotenv_element in enumerate(dotenv_elements):
             if dotenv_element.multiline_whitespace:
                 print(dotenv_element.multiline_whitespace, end="", file=example_env_f)
             if dotenv_element.export:  # e.g. export AWS_KEY=...
                 print(dotenv_element.export, end="", file=example_env_f)
             if dotenv_element.key:
                 print(
-                    f"{dotenv_element.key}={dotenv_element.separator}{dotenv_element.separator}",
+                    (
+                        f"{dotenv_element.key}={dotenv_element.separator}{dotenv_element.value}{dotenv_element.separator}"
+                        if dotenv_element.key in values_to_keep
+                        else f"{dotenv_element.key}={dotenv_element.separator}{dotenv_element.separator}"
+                    ),
                     end="",
                     file=example_env_f,
                 )
             if dotenv_element.comment:
                 print(dotenv_element.comment, end="", file=example_env_f)
             if dotenv_element.end_of_line:
                 print(dotenv_element.end_of_line, end="", file=example_env_f)
@@ -36,30 +40,38 @@
     # Finds and yields .env files in the path_to_root
     for entry in os.scandir(path_to_root):
         if entry.name.endswith(".env") and entry.is_file():
             # Create a cleaned .env.example file for the found .env file
             yield entry.path
 
 
-def _main(path_to_root: str):
+def _main(path_to_root: str, values_to_keep: List[str] = []):
     # Find possible .env files
     for dotenv_file in _find_dotenv_files(path_to_root):
         # Clean dotenv file
-        _clean_env(dotenv_file)
+        _clean_env(path_to_env=dotenv_file, values_to_keep=values_to_keep)
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Automatically creates an .env.example which creates the same keys as your .env file, but without the values"
     )
     parser.add_argument(
         "--root_path",
         type=str,
         help="Root path in which .env files shall be looked for",
         default=os.getcwd(),
     )
+    parser.add_argument(
+        "-k",
+        "--keep",
+        nargs="*",
+        help="Variables which shall not be cleaned by clean-dotenv. Separate values by space.",
+        default=[],
+    )
+
     args = parser.parse_args()
-    _main(args.root_path)
+    _main(path_to_root=args.root_path, values_to_keep=args.keep)
 
 
 if __name__ == "__main__":
     raise SystemExit(main())
```

### Comparing `clean_dotenv-0.0.6/clean_dotenv/_parser.py` & `clean_dotenv-0.0.7/clean_dotenv/_parser.py`

 * *Files identical despite different names*

### Comparing `clean_dotenv-0.0.6/clean_dotenv.egg-info/PKG-INFO` & `clean_dotenv-0.0.7/clean_dotenv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clean_dotenv
-Version: 0.0.6
+Version: 0.0.7
 Summary: Automatically creates an .env.example which creates the same keys as your .env file, but without the values
 Home-page: https://github.com/hija/clean-dotenv
 Author: Hilko (hija)
 Author-email: mail@hilko.eu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -33,16 +33,16 @@
 ```
 
 An `.env` file should not be commited into a repo, since it can contain sensitive information[^1] (you should probably adding the `.env` file into your `.gitignore`). However, one needs to know which variables can be set in the `.env` file and as a result, a lot of projects (such as laravel), provide an `.env.example` file which is a template file. So you would copy the `.env.template`, rename it to `.env` and fill in the environment variables.
 
 However, there is one issue with this approach: If one introduces a new environment variable, they need to remember to add it to the `.env.example` file. Unfortunately, if they forget this, it will not be noticed, since the program is using the `.env` file and not the `.env.example`. This pre-commit hook tries to mitigate this problem by creating an `.env.example` file automatically (based on your `.env` file), so the example `.env` file would become the following `.env.example`:
 
 ```bash
-OPENAI_KEY=
-S3_BUCKET_NAME=
+OPENAI_KEY=""
+S3_BUCKET_NAME=""
 ```
 
 [^1]: https://www.zdnet.com/article/botnets-have-been-silently-mass-scanning-the-internet-for-unsecured-env-files/
  
 ## Installation
 
 ```bash
@@ -52,25 +52,26 @@
 
 ## Console scripts
 
 Consult `clean-dotenv --help` for the full set of options.
 
 Common options:
 
-- `--root path`: Defines the root path in which to look for .env files. This is **not recursive**
+- `--root_path`: Defines the root path in which to look for .env files. This is **not recursive**
+- `--keep value1 value2`: Defines which values shall be kept in the .env file. In this example, every variable except for value1 and value2 would be cleaned.
 
 ## As a pre-commit hook
 
 See [pre-commit](https://github.com/pre-commit/pre-commit) for instructions
 
 Sample `.pre-commit-config.yaml`
 
 ```yaml
 -   repo: https://github.com/hija/clean-dotenv
-    rev: v0.0.5
+    rev: v0.0.7
     hooks:
     -   id: clean-dotenv
 ```
 
 ## What does it do?
 The tool looks for `.env` files in all directories and creates a new, corresponding filename `.env.example` which is save to commit, since it contains all the keys from your `.env` file, but without its values.
```

### Comparing `clean_dotenv-0.0.6/setup.cfg` & `clean_dotenv-0.0.7/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = clean_dotenv
-version = 0.0.6
+version = 0.0.7
 description = Automatically creates an .env.example which creates the same keys as your .env file, but without the values
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hija/clean-dotenv
 author = Hilko (hija)
 author_email = mail@hilko.eu
 license = MIT
```

