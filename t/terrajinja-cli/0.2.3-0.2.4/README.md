# Comparing `tmp/terrajinja-cli-0.2.3.tar.gz` & `tmp/terrajinja-cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrajinja-cli-0.2.3.tar", last modified: Tue Mar 26 18:08:59 2024, max compression
+gzip compressed data, was "terrajinja-cli-0.2.4.tar", last modified: Mon Apr 15 12:34:05 2024, max compression
```

## Comparing `terrajinja-cli-0.2.3.tar` & `terrajinja-cli-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:59.394163 terrajinja-cli-0.2.3/
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)     1061 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      320 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3310 2024-03-26 18:08:59.393164 terrajinja-cli-0.2.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)     2500 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/README.md
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 18:08:59.394163 terrajinja-cli-0.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1349 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:59.389163 terrajinja-cli-0.2.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:59.389163 terrajinja-cli-0.2.3/src/terrajinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:59.391163 terrajinja-cli-0.2.3/src/terrajinja/cli/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/src/terrajinja/cli/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      714 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/src/terrajinja/cli/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6370 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/src/terrajinja/cli/parse_args.py
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/src/terrajinja/cli/parse_jinja.py
--rw-rw-rw-   0 root         (0) root         (0)     6617 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/src/terrajinja/cli/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:59.393164 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3310 2024-03-26 18:08:59.000000 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      558 2024-03-26 18:08:59.000000 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 18:08:59.000000 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-03-26 18:08:59.000000 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-03-26 18:08:59.000000 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-26 18:08:59.000000 terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 18:08:59.393164 terrajinja-cli-0.2.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2190 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/tests/test_parse_args.py
--rw-rw-rw-   0 root         (0) root         (0)     2357 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/tests/test_parse_jinja.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-03-26 18:08:58.000000 terrajinja-cli-0.2.3/tests/test_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:34:05.428236 terrajinja-cli-0.2.4/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      320 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-04-15 12:34:05.428236 terrajinja-cli-0.2.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 12:34:05.428236 terrajinja-cli-0.2.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1349 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:34:05.424236 terrajinja-cli-0.2.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:34:05.423236 terrajinja-cli-0.2.4/src/terrajinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:34:05.426236 terrajinja-cli-0.2.4/src/terrajinja/cli/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/src/terrajinja/cli/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      714 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/src/terrajinja/cli/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6370 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/src/terrajinja/cli/parse_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/src/terrajinja/cli/parse_jinja.py
+-rw-rw-rw-   0 root         (0) root         (0)     6704 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/src/terrajinja/cli/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:34:05.427236 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3310 2024-04-15 12:34:05.000000 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-15 12:34:05.000000 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 12:34:05.000000 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-15 12:34:05.000000 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-15 12:34:05.000000 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-15 12:34:05.000000 terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 12:34:05.427236 terrajinja-cli-0.2.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/tests/test_parse_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     2357 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/tests/test_parse_jinja.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-04-15 12:34:04.000000 terrajinja-cli-0.2.4/tests/test_parser.py
```

### Comparing `terrajinja-cli-0.2.3/LICENSE` & `terrajinja-cli-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/PKG-INFO` & `terrajinja-cli-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-cli-0.2.3/README.md` & `terrajinja-cli-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/setup.py` & `terrajinja-cli-0.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = [line.strip()
           for line in open('requirements.txt').readlines()
           if line.strip() and not line.startswith('#')]
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
-version = '0.2.3'
+version = '0.2.4'
 name= 'terrajinja-cli'
 package_path= name.replace('-', '.')
 
 # only the cli has an entry point
 entry_points=None
 if name=='terrajinja-cli':
     entry_points={
```

### Comparing `terrajinja-cli-0.2.3/src/terrajinja/cli/__main__.py` & `terrajinja-cli-0.2.4/src/terrajinja/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/src/terrajinja/cli/parse_args.py` & `terrajinja-cli-0.2.4/src/terrajinja/cli/parse_args.py`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/src/terrajinja/cli/parse_jinja.py` & `terrajinja-cli-0.2.4/src/terrajinja/cli/parse_jinja.py`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/src/terrajinja/cli/parser.py` & `terrajinja-cli-0.2.4/src/terrajinja/cli/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,16 @@
             for sub in ["deployments", "templates", "parameters"]:
                 destination_path = os.path.join(args.config_directory, sub)
                 if not os.path.exists(destination_path):
                     print(f'destination path: {destination_path} does not exist, did you run tjcli init?')
                     exit(1)
 
             for file in pathlib.Path(template_named_dir).rglob('*'):
+                if str(file).endswith('description.txt'):
+                    continue
                 short_path = str(file)[len(template_dir) + len(args.add) + 2:]
                 target = os.path.join(args.config_directory, short_path)
                 if file.is_dir():
                     pathlib.Path(target).mkdir(parents=True, exist_ok=True)
 
                 if file.is_file():
                     if os.path.exists(target):
```

### Comparing `terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/PKG-INFO` & `terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-cli-0.2.3/src/terrajinja_cli.egg-info/SOURCES.txt` & `terrajinja-cli-0.2.4/src/terrajinja_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/tests/test_parse_args.py` & `terrajinja-cli-0.2.4/tests/test_parse_args.py`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/tests/test_parse_jinja.py` & `terrajinja-cli-0.2.4/tests/test_parse_jinja.py`

 * *Files identical despite different names*

### Comparing `terrajinja-cli-0.2.3/tests/test_parser.py` & `terrajinja-cli-0.2.4/tests/test_parser.py`

 * *Files identical despite different names*

