# Comparing `tmp/check-bump-1.0.0.tar.gz` & `tmp/check_bump-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "check-bump-1.0.0.tar", last modified: Fri Mar 29 10:07:51 2024, max compression
+gzip compressed data, was "check_bump-1.0.2.tar", last modified: Mon Apr 15 21:20:50 2024, max compression
```

## Comparing `check-bump-1.0.0.tar` & `check_bump-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:07:51.623912 check-bump-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-29 10:07:47.000000 check-bump-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-29 10:07:51.623912 check-bump-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-03-29 10:07:47.000000 check-bump-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:07:51.619912 check-bump-1.0.0/check_bump/
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-03-29 10:07:47.000000 check-bump-1.0.0/check_bump/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:07:51.619912 check-bump-1.0.0/check_bump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-29 10:07:51.000000 check-bump-1.0.0/check_bump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-03-29 10:07:51.000000 check-bump-1.0.0/check_bump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 10:07:51.000000 check-bump-1.0.0/check_bump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-29 10:07:51.000000 check-bump-1.0.0/check_bump.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-29 10:07:51.000000 check-bump-1.0.0/check_bump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 10:07:51.000000 check-bump-1.0.0/check_bump.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-29 10:07:47.000000 check-bump-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-29 10:07:47.000000 check-bump-1.0.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 10:07:51.623912 check-bump-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 10:07:51.619912 check-bump-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-29 10:07:47.000000 check-bump-1.0.0/tests/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:20:50.273291 check_bump-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 21:20:43.000000 check_bump-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-15 21:20:50.273291 check_bump-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3307 2024-04-15 21:20:43.000000 check_bump-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:20:50.269291 check_bump-1.0.2/check_bump/
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-15 21:20:43.000000 check_bump-1.0.2/check_bump/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:20:50.269291 check_bump-1.0.2/check_bump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-15 21:20:50.000000 check_bump-1.0.2/check_bump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 21:20:50.000000 check_bump-1.0.2/check_bump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:20:50.000000 check_bump-1.0.2/check_bump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-15 21:20:50.000000 check_bump-1.0.2/check_bump.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-15 21:20:50.000000 check_bump-1.0.2/check_bump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 21:20:50.000000 check_bump-1.0.2/check_bump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-15 21:20:43.000000 check_bump-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 21:20:43.000000 check_bump-1.0.2/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:20:50.273291 check_bump-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:20:50.269291 check_bump-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-15 21:20:43.000000 check_bump-1.0.2/tests/test_unit.py
```

### Comparing `check-bump-1.0.0/LICENSE` & `check_bump-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `check-bump-1.0.0/PKG-INFO` & `check_bump-1.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: check-bump
-Version: 1.0.0
-Summary: Do not allow prints in your code
+Version: 1.0.2
+Summary: Check if pyproject.toml version was bumped
 Author-email: Radoslaw Gryta <radek.gryta@gmail.com>
 Project-URL: Homepage, https://github.com/rgryta/Check-Bump
 Project-URL: Bug Tracker, https://github.com/rgryta/Check-Bump/issues
 Keywords: versioning,check,CI,CD,version,bump
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,27 +47,69 @@
 
 ## Requirements
 
 This package requires `tomlkit` package.
 
 ## Usage
 
+### Command
+
 Simply execute `check-bump` within a directory where your `pyproject.toml` is located. Or provide a path using `--path` argument.
 
 ```bash
 user$ check-bump --help
 usage: check-bump [-h] [-p PATH]
 
 Detect and retrieve version bump
 
 options:
   -h, --help            show this help message and exit
   -p PATH, --path PATH  path to pyproject.toml file
 ```
 
+### Github Actions
+
+#### Inputs
+
+##### `path`
+
+**Optional** Relative path of pyproject.toml file. Example: `'python_src/pyproject.toml'`
+
+##### `prefix`
+
+**Optional** Prefix to provide for version output. Example: `'v'`
+
+#### Outputs
+
+##### `bump`
+
+**always** Whether there was a bump or not. Values: `'true'`|`'false'`
+
+##### `version`
+
+**optional** Current (if bumped) version with prefix. If there was no version bump - no output is provided.
+
+## Example usage
+
+```yml
+- name: Check bump
+  id: vbump
+  uses: rgryta/Check-Bump@main
+  with:
+    prefix: 'v'
+```
+
+And then you can later reference like:
+```yml
+- name: Tag repository
+  if: steps.vbump.outputs.bump == 'true'
+  run: |
+    echo "I was bumped to version: ${{ steps.vbump.outputs.version }}"
+```
+
 ## Development
 
 ### Installation
 
 Install virtual environment and check_bump package in editable mode with dev dependencies.
 
 ```bash
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: check-bump Version: 1.0.0 Summary: Do not allow
-prints in your code Author-email: Radoslaw Gryta
+Metadata-Version: 2.1 Name: check-bump Version: 1.0.2 Summary: Check if
+pyproject.toml version was bumped Author-email: Radoslaw Gryta
 gmail.com> Project-URL: Homepage, https://github.com/rgryta/Check-Bump Project-
 URL: Bug Tracker, https://github.com/rgryta/Check-Bump/issues Keywords:
 versioning,check,CI,CD,version,bump Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: tomlkit Provides-Extra: dev
 Requires-Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev"
@@ -16,25 +16,35 @@
                             ********** CChheecckk BBuummpp **********
                _[_B_u_i_l_d_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_p_y_l_i_n_t_]_[_N_o_P_r_i_n_t_]
 ## About Want to add version bump checks to your CI/CD pipeline? This packages
 makes it easy. Simply execute `check-vbump` within a directory where your
 `pyproject.toml` is located. If there was a version bump, process will finish
 with exit code 0 - read stdout for the new version. Otherwise, process will
 finish with exit code 1. ## Requirements This package requires `tomlkit`
-package. ## Usage Simply execute `check-bump` within a directory where your
-`pyproject.toml` is located. Or provide a path using `--path` argument. ```bash
-user$ check-bump --help usage: check-bump [-h] [-p PATH] Detect and retrieve
-version bump options: -h, --help show this help message and exit -p PATH, --
-path PATH path to pyproject.toml file ``` ## Development ### Installation
-Install virtual environment and check_bump package in editable mode with dev
-dependencies. ```bash python -m venv venv source venv/bin/activate pip install
--e .[dev] ``` ### Formatting Use black and isort (with black profile) to format
-the code. ```bash isort . black . ``` ### Syntax checks Use pylint to check the
-code for errors and potential problems. Also use noprint to detect print
-statements in the code (use logging instead!). ```bash isort -c . black --check
-. pylint check_bump tests noprint -ve check_bump tests ``` ### Testing For
-testing use coverage with pytest workers - this is due to errors that pytest-
-cov sometimes has with Python 3.9 and above. ```bash coverage run -m pytest -xv
-tests coverage report -m --fail-under=30 coverage erase ``` ### Clean up Clean
-up the project directory from temporary files and directories. Purge virual
-environment. ```bash coverage erase rm -rf check_bump.egg-info/ dist/ build/ rm
--rf venv/ ```
+package. ## Usage ### Command Simply execute `check-bump` within a directory
+where your `pyproject.toml` is located. Or provide a path using `--path`
+argument. ```bash user$ check-bump --help usage: check-bump [-h] [-p PATH]
+Detect and retrieve version bump options: -h, --help show this help message and
+exit -p PATH, --path PATH path to pyproject.toml file ``` ### Github Actions
+#### Inputs ##### `path` **Optional** Relative path of pyproject.toml file.
+Example: `'python_src/pyproject.toml'` ##### `prefix` **Optional** Prefix to
+provide for version output. Example: `'v'` #### Outputs ##### `bump` **always**
+Whether there was a bump or not. Values: `'true'`|`'false'` ##### `version`
+**optional** Current (if bumped) version with prefix. If there was no version
+bump - no output is provided. ## Example usage ```yml - name: Check bump id:
+vbump uses: rgryta/Check-Bump@main with: prefix: 'v' ``` And then you can later
+reference like: ```yml - name: Tag repository if: steps.vbump.outputs.bump ==
+'true' run: | echo "I was bumped to version: ${{ steps.vbump.outputs.version
+}}" ``` ## Development ### Installation Install virtual environment and
+check_bump package in editable mode with dev dependencies. ```bash python -
+m venv venv source venv/bin/activate pip install -e .[dev] ``` ### Formatting
+Use black and isort (with black profile) to format the code. ```bash isort .
+black . ``` ### Syntax checks Use pylint to check the code for errors and
+potential problems. Also use noprint to detect print statements in the code
+(use logging instead!). ```bash isort -c . black --check . pylint check_bump
+tests noprint -ve check_bump tests ``` ### Testing For testing use coverage
+with pytest workers - this is due to errors that pytest-cov sometimes has with
+Python 3.9 and above. ```bash coverage run -m pytest -xv tests coverage report
+-m --fail-under=30 coverage erase ``` ### Clean up Clean up the project
+directory from temporary files and directories. Purge virual environment.
+```bash coverage erase rm -rf check_bump.egg-info/ dist/ build/ rm -rf venv/
+```
```

### Comparing `check-bump-1.0.0/README.md` & `check_bump-1.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,27 +18,69 @@
 
 ## Requirements
 
 This package requires `tomlkit` package.
 
 ## Usage
 
+### Command
+
 Simply execute `check-bump` within a directory where your `pyproject.toml` is located. Or provide a path using `--path` argument.
 
 ```bash
 user$ check-bump --help
 usage: check-bump [-h] [-p PATH]
 
 Detect and retrieve version bump
 
 options:
   -h, --help            show this help message and exit
   -p PATH, --path PATH  path to pyproject.toml file
 ```
 
+### Github Actions
+
+#### Inputs
+
+##### `path`
+
+**Optional** Relative path of pyproject.toml file. Example: `'python_src/pyproject.toml'`
+
+##### `prefix`
+
+**Optional** Prefix to provide for version output. Example: `'v'`
+
+#### Outputs
+
+##### `bump`
+
+**always** Whether there was a bump or not. Values: `'true'`|`'false'`
+
+##### `version`
+
+**optional** Current (if bumped) version with prefix. If there was no version bump - no output is provided.
+
+## Example usage
+
+```yml
+- name: Check bump
+  id: vbump
+  uses: rgryta/Check-Bump@main
+  with:
+    prefix: 'v'
+```
+
+And then you can later reference like:
+```yml
+- name: Tag repository
+  if: steps.vbump.outputs.bump == 'true'
+  run: |
+    echo "I was bumped to version: ${{ steps.vbump.outputs.version }}"
+```
+
 ## Development
 
 ### Installation
 
 Install virtual environment and check_bump package in editable mode with dev dependencies.
 
 ```bash
```

#### html2text {}

```diff
@@ -1,25 +1,35 @@
                             ********** CChheecckk BBuummpp **********
                _[_B_u_i_l_d_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_p_y_l_i_n_t_]_[_N_o_P_r_i_n_t_]
 ## About Want to add version bump checks to your CI/CD pipeline? This packages
 makes it easy. Simply execute `check-vbump` within a directory where your
 `pyproject.toml` is located. If there was a version bump, process will finish
 with exit code 0 - read stdout for the new version. Otherwise, process will
 finish with exit code 1. ## Requirements This package requires `tomlkit`
-package. ## Usage Simply execute `check-bump` within a directory where your
-`pyproject.toml` is located. Or provide a path using `--path` argument. ```bash
-user$ check-bump --help usage: check-bump [-h] [-p PATH] Detect and retrieve
-version bump options: -h, --help show this help message and exit -p PATH, --
-path PATH path to pyproject.toml file ``` ## Development ### Installation
-Install virtual environment and check_bump package in editable mode with dev
-dependencies. ```bash python -m venv venv source venv/bin/activate pip install
--e .[dev] ``` ### Formatting Use black and isort (with black profile) to format
-the code. ```bash isort . black . ``` ### Syntax checks Use pylint to check the
-code for errors and potential problems. Also use noprint to detect print
-statements in the code (use logging instead!). ```bash isort -c . black --check
-. pylint check_bump tests noprint -ve check_bump tests ``` ### Testing For
-testing use coverage with pytest workers - this is due to errors that pytest-
-cov sometimes has with Python 3.9 and above. ```bash coverage run -m pytest -xv
-tests coverage report -m --fail-under=30 coverage erase ``` ### Clean up Clean
-up the project directory from temporary files and directories. Purge virual
-environment. ```bash coverage erase rm -rf check_bump.egg-info/ dist/ build/ rm
--rf venv/ ```
+package. ## Usage ### Command Simply execute `check-bump` within a directory
+where your `pyproject.toml` is located. Or provide a path using `--path`
+argument. ```bash user$ check-bump --help usage: check-bump [-h] [-p PATH]
+Detect and retrieve version bump options: -h, --help show this help message and
+exit -p PATH, --path PATH path to pyproject.toml file ``` ### Github Actions
+#### Inputs ##### `path` **Optional** Relative path of pyproject.toml file.
+Example: `'python_src/pyproject.toml'` ##### `prefix` **Optional** Prefix to
+provide for version output. Example: `'v'` #### Outputs ##### `bump` **always**
+Whether there was a bump or not. Values: `'true'`|`'false'` ##### `version`
+**optional** Current (if bumped) version with prefix. If there was no version
+bump - no output is provided. ## Example usage ```yml - name: Check bump id:
+vbump uses: rgryta/Check-Bump@main with: prefix: 'v' ``` And then you can later
+reference like: ```yml - name: Tag repository if: steps.vbump.outputs.bump ==
+'true' run: | echo "I was bumped to version: ${{ steps.vbump.outputs.version
+}}" ``` ## Development ### Installation Install virtual environment and
+check_bump package in editable mode with dev dependencies. ```bash python -
+m venv venv source venv/bin/activate pip install -e .[dev] ``` ### Formatting
+Use black and isort (with black profile) to format the code. ```bash isort .
+black . ``` ### Syntax checks Use pylint to check the code for errors and
+potential problems. Also use noprint to detect print statements in the code
+(use logging instead!). ```bash isort -c . black --check . pylint check_bump
+tests noprint -ve check_bump tests ``` ### Testing For testing use coverage
+with pytest workers - this is due to errors that pytest-cov sometimes has with
+Python 3.9 and above. ```bash coverage run -m pytest -xv tests coverage report
+-m --fail-under=30 coverage erase ``` ### Clean up Clean up the project
+directory from temporary files and directories. Purge virual environment.
+```bash coverage erase rm -rf check_bump.egg-info/ dist/ build/ rm -rf venv/
+```
```

### Comparing `check-bump-1.0.0/check_bump/__init__.py` & `check_bump-1.0.2/check_bump/__init__.py`

 * *Files identical despite different names*

### Comparing `check-bump-1.0.0/check_bump.egg-info/PKG-INFO` & `check_bump-1.0.2/check_bump.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: check-bump
-Version: 1.0.0
-Summary: Do not allow prints in your code
+Version: 1.0.2
+Summary: Check if pyproject.toml version was bumped
 Author-email: Radoslaw Gryta <radek.gryta@gmail.com>
 Project-URL: Homepage, https://github.com/rgryta/Check-Bump
 Project-URL: Bug Tracker, https://github.com/rgryta/Check-Bump/issues
 Keywords: versioning,check,CI,CD,version,bump
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -47,27 +47,69 @@
 
 ## Requirements
 
 This package requires `tomlkit` package.
 
 ## Usage
 
+### Command
+
 Simply execute `check-bump` within a directory where your `pyproject.toml` is located. Or provide a path using `--path` argument.
 
 ```bash
 user$ check-bump --help
 usage: check-bump [-h] [-p PATH]
 
 Detect and retrieve version bump
 
 options:
   -h, --help            show this help message and exit
   -p PATH, --path PATH  path to pyproject.toml file
 ```
 
+### Github Actions
+
+#### Inputs
+
+##### `path`
+
+**Optional** Relative path of pyproject.toml file. Example: `'python_src/pyproject.toml'`
+
+##### `prefix`
+
+**Optional** Prefix to provide for version output. Example: `'v'`
+
+#### Outputs
+
+##### `bump`
+
+**always** Whether there was a bump or not. Values: `'true'`|`'false'`
+
+##### `version`
+
+**optional** Current (if bumped) version with prefix. If there was no version bump - no output is provided.
+
+## Example usage
+
+```yml
+- name: Check bump
+  id: vbump
+  uses: rgryta/Check-Bump@main
+  with:
+    prefix: 'v'
+```
+
+And then you can later reference like:
+```yml
+- name: Tag repository
+  if: steps.vbump.outputs.bump == 'true'
+  run: |
+    echo "I was bumped to version: ${{ steps.vbump.outputs.version }}"
+```
+
 ## Development
 
 ### Installation
 
 Install virtual environment and check_bump package in editable mode with dev dependencies.
 
 ```bash
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: check-bump Version: 1.0.0 Summary: Do not allow
-prints in your code Author-email: Radoslaw Gryta
+Metadata-Version: 2.1 Name: check-bump Version: 1.0.2 Summary: Check if
+pyproject.toml version was bumped Author-email: Radoslaw Gryta
 gmail.com> Project-URL: Homepage, https://github.com/rgryta/Check-Bump Project-
 URL: Bug Tracker, https://github.com/rgryta/Check-Bump/issues Keywords:
 versioning,check,CI,CD,version,bump Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.8 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: tomlkit Provides-Extra: dev
 Requires-Dist: black; extra == "dev" Requires-Dist: isort; extra == "dev"
@@ -16,25 +16,35 @@
                             ********** CChheecckk BBuummpp **********
                _[_B_u_i_l_d_]_[_P_y_P_I_]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_p_y_l_i_n_t_]_[_N_o_P_r_i_n_t_]
 ## About Want to add version bump checks to your CI/CD pipeline? This packages
 makes it easy. Simply execute `check-vbump` within a directory where your
 `pyproject.toml` is located. If there was a version bump, process will finish
 with exit code 0 - read stdout for the new version. Otherwise, process will
 finish with exit code 1. ## Requirements This package requires `tomlkit`
-package. ## Usage Simply execute `check-bump` within a directory where your
-`pyproject.toml` is located. Or provide a path using `--path` argument. ```bash
-user$ check-bump --help usage: check-bump [-h] [-p PATH] Detect and retrieve
-version bump options: -h, --help show this help message and exit -p PATH, --
-path PATH path to pyproject.toml file ``` ## Development ### Installation
-Install virtual environment and check_bump package in editable mode with dev
-dependencies. ```bash python -m venv venv source venv/bin/activate pip install
--e .[dev] ``` ### Formatting Use black and isort (with black profile) to format
-the code. ```bash isort . black . ``` ### Syntax checks Use pylint to check the
-code for errors and potential problems. Also use noprint to detect print
-statements in the code (use logging instead!). ```bash isort -c . black --check
-. pylint check_bump tests noprint -ve check_bump tests ``` ### Testing For
-testing use coverage with pytest workers - this is due to errors that pytest-
-cov sometimes has with Python 3.9 and above. ```bash coverage run -m pytest -xv
-tests coverage report -m --fail-under=30 coverage erase ``` ### Clean up Clean
-up the project directory from temporary files and directories. Purge virual
-environment. ```bash coverage erase rm -rf check_bump.egg-info/ dist/ build/ rm
--rf venv/ ```
+package. ## Usage ### Command Simply execute `check-bump` within a directory
+where your `pyproject.toml` is located. Or provide a path using `--path`
+argument. ```bash user$ check-bump --help usage: check-bump [-h] [-p PATH]
+Detect and retrieve version bump options: -h, --help show this help message and
+exit -p PATH, --path PATH path to pyproject.toml file ``` ### Github Actions
+#### Inputs ##### `path` **Optional** Relative path of pyproject.toml file.
+Example: `'python_src/pyproject.toml'` ##### `prefix` **Optional** Prefix to
+provide for version output. Example: `'v'` #### Outputs ##### `bump` **always**
+Whether there was a bump or not. Values: `'true'`|`'false'` ##### `version`
+**optional** Current (if bumped) version with prefix. If there was no version
+bump - no output is provided. ## Example usage ```yml - name: Check bump id:
+vbump uses: rgryta/Check-Bump@main with: prefix: 'v' ``` And then you can later
+reference like: ```yml - name: Tag repository if: steps.vbump.outputs.bump ==
+'true' run: | echo "I was bumped to version: ${{ steps.vbump.outputs.version
+}}" ``` ## Development ### Installation Install virtual environment and
+check_bump package in editable mode with dev dependencies. ```bash python -
+m venv venv source venv/bin/activate pip install -e .[dev] ``` ### Formatting
+Use black and isort (with black profile) to format the code. ```bash isort .
+black . ``` ### Syntax checks Use pylint to check the code for errors and
+potential problems. Also use noprint to detect print statements in the code
+(use logging instead!). ```bash isort -c . black --check . pylint check_bump
+tests noprint -ve check_bump tests ``` ### Testing For testing use coverage
+with pytest workers - this is due to errors that pytest-cov sometimes has with
+Python 3.9 and above. ```bash coverage run -m pytest -xv tests coverage report
+-m --fail-under=30 coverage erase ``` ### Clean up Clean up the project
+directory from temporary files and directories. Purge virual environment.
+```bash coverage erase rm -rf check_bump.egg-info/ dist/ build/ rm -rf venv/
+```
```

### Comparing `check-bump-1.0.0/pyproject.toml` & `check_bump-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "check-bump"
-version = "1.0.0"
+version = "1.0.2"
 authors = [
     { name="Radoslaw Gryta", email="radek.gryta@gmail.com" },
 ]
-description = "Do not allow prints in your code"
+description = "Check if pyproject.toml version was bumped"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["versioning", "check", "CI", "CD", "version", "bump"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
@@ -34,24 +34,30 @@
 
 [tool.setuptools.dynamic]
 optional-dependencies = { dev = {file = ["requirements_dev.txt"]} }
 
 ####### BUMPV #######
 
 [tool.bumpversion]
-current_version = "1.0.0"
+current_version = "1.0.2"
 allow_dirty = true
 commit = true
 message = "[Version {new_version}]"
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = "version = \"{current_version}\""
 replace = "version = \"{new_version}\""
 
+
+[[tool.bumpversion.files]]
+filename = "action.yml"
+search = "      run: pip install \"check-bump=={current_version}\""
+replace = "      run: pip install \"check-bump=={new_version}\""
+
 ####### BLACK #######
 
 [tool.black]
 line-length = 120
 preview = true
 
 ####### COVERAGE #######
```

