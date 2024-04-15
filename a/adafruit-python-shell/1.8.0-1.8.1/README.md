# Comparing `tmp/adafruit-python-shell-1.8.0.tar.gz` & `tmp/adafruit_python_shell-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-python-shell-1.8.0.tar", last modified: Thu Sep 14 19:37:59 2023, max compression
+gzip compressed data, was "adafruit_python_shell-1.8.1.tar", last modified: Mon Apr 15 21:11:06 2024, max compression
```

## Comparing `adafruit-python-shell-1.8.0.tar` & `adafruit_python_shell-1.8.1.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.606474 adafruit-python-shell-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.594473 adafruit-python-shell-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.598473 adafruit-python-shell-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.598473 adafruit-python-shell-1.8.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-09-14 19:37:59.606474 adafruit-python-shell-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.606474 adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-09-14 19:37:59.000000 adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-09-14 19:37:59.000000 adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 19:37:59.000000 adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-14 19:37:59.000000 adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-14 19:37:59.000000 adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21134 2023-09-14 19:37:50.000000 adafruit-python-shell-1.8.0/adafruit_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.606474 adafruit-python-shell-1.8.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 19:37:59.606474 adafruit-python-shell-1.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      264 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/optional_dependencies.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-09-14 19:37:50.000000 adafruit-python-shell-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-09-14 19:37:41.000000 adafruit-python-shell-1.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-14 19:37:59.606474 adafruit-python-shell-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.037414 adafruit_python_shell-1.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.033414 adafruit_python_shell-1.8.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.033414 adafruit_python_shell-1.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.033414 adafruit_python_shell-1.8.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-15 21:11:06.037414 adafruit_python_shell-1.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.037414 adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-15 21:11:06.000000 adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-15 21:11:06.000000 adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:11:06.000000 adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 21:11:06.000000 adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 21:11:06.000000 adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21229 2024-04-15 21:11:03.000000 adafruit_python_shell-1.8.1/adafruit_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.037414 adafruit_python_shell-1.8.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:11:06.037414 adafruit_python_shell-1.8.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/optional_dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-15 21:11:03.000000 adafruit_python_shell-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 21:10:55.000000 adafruit_python_shell-1.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:11:06.037414 adafruit_python_shell-1.8.1/setup.cfg
```

### Comparing `adafruit-python-shell-1.8.0/.github/workflows/build.yml` & `adafruit_python_shell-1.8.1/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
       id: repo-name
       run: |
         echo repo-name=$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         ) >> $GITHUB_OUTPUT
-    - name: Set up Python 3.x
+    - name: Set up Python 3.11
       uses: actions/setup-python@v4
       with:
-        python-version: '3.x'
+        python-version: '3.11'
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v3
       with:
         submodules: true
```

### Comparing `adafruit-python-shell-1.8.0/.github/workflows/release.yml` & `adafruit_python_shell-1.8.1/.github/workflows/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
       id: need-pypi
       run: |
         echo pyproject-toml=$( find . -wholename './pyproject.toml' ) >> $GITHUB_OUTPUT
     - name: Set up Python
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       uses: actions/setup-python@v4
       with:
-        python-version: '3.x'
+        python-version: '3.11'
     - name: Install dependencies
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         python -m pip install --upgrade pip
         pip install --upgrade build twine
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
```

### Comparing `adafruit-python-shell-1.8.0/.pre-commit-config.yaml` & `adafruit_python_shell-1.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/.pylintrc` & `adafruit_python_shell-1.8.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/CODE_OF_CONDUCT.md` & `adafruit_python_shell-1.8.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/LICENSE` & `adafruit_python_shell-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/LICENSES/CC-BY-4.0.txt` & `adafruit_python_shell-1.8.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/LICENSES/MIT.txt` & `adafruit_python_shell-1.8.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/LICENSES/Unlicense.txt` & `adafruit_python_shell-1.8.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/PKG-INFO` & `adafruit_python_shell-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-python-shell
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python helper for running Shell scripts in Python
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_Python_Shell
 Keywords: adafruit,blinka,circuitpython,micropython,python,shell,installation,raspberry,pi,console,terminal,installer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `adafruit-python-shell-1.8.0/README.rst` & `adafruit_python_shell-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/PKG-INFO` & `adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-python-shell
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python helper for running Shell scripts in Python
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_Python_Shell
 Keywords: adafruit,blinka,circuitpython,micropython,python,shell,installation,raspberry,pi,console,terminal,installer
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `adafruit-python-shell-1.8.0/adafruit_python_shell.egg-info/SOURCES.txt` & `adafruit_python_shell-1.8.1/adafruit_python_shell.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 LICENSE
 README.rst
 README.rst.license
 adafruit_shell.py
 optional_dependencies.txt
 pyproject.toml
 requirements.txt
+.github/release-drafter.yml
 .github/workflows/build.yml
+.github/workflows/release-drafter.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_python_shell.egg-info/PKG-INFO
 adafruit_python_shell.egg-info/SOURCES.txt
 adafruit_python_shell.egg-info/dependency_links.txt
```

### Comparing `adafruit-python-shell-1.8.0/adafruit_shell.py` & `adafruit_python_shell-1.8.1/adafruit_shell.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import fileinput
 import re
 import pwd
 from datetime import datetime
 from clint.textui import colored, prompt
 import adafruit_platformdetect
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 __repo__ = "https://github.com/adafruit/Adafruit_Python_Shell.git"
 
 
 # pylint: disable=too-many-public-methods
 class Shell:
     """
     Class to help with converting Shell scripts over to Python. Having all
@@ -551,15 +551,22 @@
             release = "Darwin"
         return release
 
     def get_raspbian_version(self):
         """Return a string containing the raspbian version"""
         if self.get_os() != "Raspbian":
             return None
-        raspbian_releases = ("bullseye", "buster", "stretch", "jessie", "wheezy")
+        raspbian_releases = (
+            "bookworm",
+            "bullseye",
+            "buster",
+            "stretch",
+            "jessie",
+            "wheezy",
+        )
         if os.path.exists("/etc/os-release"):
             with open("/etc/os-release", encoding="utf-8") as f:
                 release_file = f.read()
                 if "/sid" in release_file:
                     return "unstable"
                 for raspbian in raspbian_releases:
                     if raspbian in release_file:
```

### Comparing `adafruit-python-shell-1.8.0/docs/_static/favicon.ico` & `adafruit_python_shell-1.8.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/docs/conf.py` & `adafruit_python_shell-1.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/docs/index.rst` & `adafruit_python_shell-1.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-python-shell-1.8.0/pyproject.toml` & `adafruit_python_shell-1.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-python-shell"
 description = "Python helper for running Shell scripts in Python"
-version = "1.8.0"
+version = "1.8.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_Python_Shell"}
 keywords = [
     "adafruit",
```

