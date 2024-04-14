# Comparing `tmp/alana-0.0.3.tar.gz` & `tmp/alana-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alana-0.0.3.tar", last modified: Sat Apr 13 15:00:50 2024, max compression
+gzip compressed data, was "alana-0.0.4.tar", last modified: Sun Apr 14 12:45:17 2024, max compression
```

## Comparing `alana-0.0.3.tar` & `alana-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:00:50.387466 alana-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 15:00:44.000000 alana-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 15:00:50.387466 alana-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-13 15:00:44.000000 alana-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:00:50.383466 alana-0.0.3/alana/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 15:00:44.000000 alana-0.0.3/alana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 15:00:44.000000 alana-0.0.3/alana/alana.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-13 15:00:44.000000 alana-0.0.3/alana/color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-04-13 15:00:44.000000 alana-0.0.3/alana/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:00:50.387466 alana-0.0.3/alana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-13 15:00:50.000000 alana-0.0.3/alana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:00:50.387466 alana-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-13 15:00:44.000000 alana-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:17.596342 alana-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 12:45:09.000000 alana-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-14 12:45:17.596342 alana-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-04-14 12:45:09.000000 alana-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:17.596342 alana-0.0.4/alana/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-14 12:45:09.000000 alana-0.0.4/alana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-14 12:45:09.000000 alana-0.0.4/alana/color.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-04-14 12:45:09.000000 alana-0.0.4/alana/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-14 12:45:09.000000 alana-0.0.4/alana/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:17.596342 alana-0.0.4/alana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-14 12:45:17.000000 alana-0.0.4/alana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-14 12:45:17.000000 alana-0.0.4/alana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:45:17.000000 alana-0.0.4/alana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 12:45:17.000000 alana-0.0.4/alana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 12:45:17.000000 alana-0.0.4/alana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:45:17.596342 alana-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-14 12:45:09.000000 alana-0.0.4/setup.py
```

### Comparing `alana-0.0.3/LICENSE` & `alana-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alana-0.0.3/alana/color.py` & `alana-0.0.4/alana/color.py`

 * *Files identical despite different names*

```diff
@@ -32,8 +32,7 @@
     log(loud, output, logger)
     return output
 
 def cyan(var: Any, loud: bool = True, logger: Optional[logging.Logger] = None) -> str:
     output = f"{Fore.CYAN} {var} {Style.RESET_ALL}"
     log(loud, output, logger)
     return output
-
```

### Comparing `alana-0.0.3/setup.py` & `alana-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
    name='alana',
-   version='0.0.3',  # Update the version number as needed
+   version='0.0.4',  # Update the version number as needed
    author='Alana',
    author_email='hi@alana.computer',
    description='Utilities for Alana, and maybe you too. Mostly geared toward LLM-heavy workflows.',
    long_description=long_description,
    long_description_content_type="text/markdown",
    url='https://github.com/alat-rights/alana-utilities',
    packages=find_packages(),
```

