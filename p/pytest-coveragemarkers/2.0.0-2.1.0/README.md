# Comparing `tmp/pytest-coveragemarkers-2.0.0.tar.gz` & `tmp/pytest_coveragemarkers-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-coveragemarkers-2.0.0.tar", max compression
+gzip compressed data, was "pytest_coveragemarkers-2.1.0.tar", max compression
```

## Comparing `pytest-coveragemarkers-2.0.0.tar` & `pytest_coveragemarkers-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1084 2022-05-12 13:13:42.186411 pytest-coveragemarkers-2.0.0/LICENSE
--rw-r--r--   0        0        0     5925 2022-11-28 13:53:31.104498 pytest-coveragemarkers-2.0.0/README.rst
--rw-r--r--   0        0        0     1448 2022-11-29 17:46:59.000304 pytest-coveragemarkers-2.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-23 23:58:22.297408 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/__init__.py
--rw-r--r--   0        0        0      533 2022-11-29 16:53:07.226143 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/coverage_markers/__init__.py
--rw-r--r--   0        0        0     6522 2022-11-29 16:50:52.142923 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/coverage_markers/marker_ops.py
--rw-r--r--   0        0        0        0 2022-11-17 21:59:56.636452 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filter_specs/__init__.py
--rw-r--r--   0        0        0       93 2022-11-24 00:04:27.278849 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filter_specs/epics_filter.json
--rw-r--r--   0        0        0        3 2022-11-24 00:04:27.280865 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filter_specs/no_filter.json
--rw-r--r--   0        0        0      327 2022-11-24 23:49:43.357057 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filtering/__init__.py
--rw-r--r--   0        0        0     2845 2022-11-24 22:43:11.849844 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filtering/filter_engine.py
--rw-r--r--   0        0        0     3212 2022-11-29 16:47:06.553165 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filtering/filter_ops.py
--rw-r--r--   0        0        0        0 2022-05-20 21:36:49.756786 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/marker_specs/__init__.py
--rw-r--r--   0        0        0       83 2022-10-26 15:53:05.525958 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/marker_specs/coverage_markers.yml
--rw-r--r--   0        0        0       65 2022-10-26 15:53:05.526486 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/marker_specs/epics.yml
--rw-r--r--   0        0        0       80 2022-10-26 15:53:05.526796 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/marker_specs/features.yml
--rw-r--r--   0        0        0       16 2022-10-26 15:53:05.527629 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/marker_specs/jira/bugs.yml
--rw-r--r--   0        0        0     1530 2022-11-29 16:53:07.226801 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/plugin.py
--rw-r--r--   0        0        0      216 2022-11-29 17:00:41.644779 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/utils/__init__.py
--rw-r--r--   0        0        0     1453 2022-11-27 18:27:46.100455 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/utils/checks.py
--rw-r--r--   0        0        0       62 2022-11-29 15:45:49.427150 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/utils/logger.py
--rw-r--r--   0        0        0     3658 2022-11-29 16:50:52.138817 pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/utils/yml_processing.py
--rw-r--r--   0        0        0     7763 2022-11-29 17:47:00.366201 pytest-coveragemarkers-2.0.0/setup.py
--rw-r--r--   0        0        0     6746 2022-11-29 17:47:00.366671 pytest-coveragemarkers-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-05-12 13:13:42.186411 pytest_coveragemarkers-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5925 2023-01-09 23:27:17.367406 pytest_coveragemarkers-2.1.0/README.rst
+-rw-r--r--   0        0        0     1448 2024-04-15 10:52:20.460630 pytest_coveragemarkers-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-09 23:27:17.371124 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/__init__.py
+-rw-r--r--   0        0        0      533 2023-01-09 23:27:17.372110 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/coverage_markers/__init__.py
+-rw-r--r--   0        0        0     6522 2023-01-10 00:21:48.172903 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/coverage_markers/marker_ops.py
+-rw-r--r--   0        0        0        0 2022-11-17 21:59:56.636452 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filter_specs/__init__.py
+-rw-r--r--   0        0        0       93 2023-01-09 23:27:17.373973 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filter_specs/epics_filter.json
+-rw-r--r--   0        0        0        3 2023-01-09 23:27:17.374663 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filter_specs/no_filter.json
+-rw-r--r--   0        0        0      327 2023-01-09 23:27:17.375591 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filtering/__init__.py
+-rw-r--r--   0        0        0     2845 2023-01-09 23:27:17.376511 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filtering/filter_engine.py
+-rw-r--r--   0        0        0     3212 2023-01-09 23:27:17.377540 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filtering/filter_ops.py
+-rw-r--r--   0        0        0        0 2022-05-20 21:36:49.756786 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/marker_specs/__init__.py
+-rw-r--r--   0        0        0       83 2022-10-26 15:53:05.525958 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/marker_specs/coverage_markers.yml
+-rw-r--r--   0        0        0       65 2022-10-26 15:53:05.526486 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/marker_specs/epics.yml
+-rw-r--r--   0        0        0       80 2022-10-26 15:53:05.526796 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/marker_specs/features.yml
+-rw-r--r--   0        0        0       16 2022-10-26 15:53:05.527629 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/marker_specs/jira/bugs.yml
+-rw-r--r--   0        0        0     1530 2024-03-29 21:48:31.756971 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/plugin.py
+-rw-r--r--   0        0        0      216 2023-01-09 23:27:17.379368 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/utils/__init__.py
+-rw-r--r--   0        0        0     1453 2023-01-09 23:27:17.380427 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/utils/checks.py
+-rw-r--r--   0        0        0       62 2023-01-09 23:27:17.380701 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/utils/logger.py
+-rw-r--r--   0        0        0     3658 2023-01-09 23:27:17.381346 pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/utils/yml_processing.py
+-rw-r--r--   0        0        0     7769 1970-01-01 00:00:00.000000 pytest_coveragemarkers-2.1.0/setup.py
+-rw-r--r--   0        0        0     6746 1970-01-01 00:00:00.000000 pytest_coveragemarkers-2.1.0/PKG-INFO
```

### Comparing `pytest-coveragemarkers-2.0.0/LICENSE` & `pytest_coveragemarkers-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/README.rst` & `pytest_coveragemarkers-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pyproject.toml` & `pytest_coveragemarkers-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "pytest-coveragemarkers"
-version = "2.0.0"
+version = "2.1.0"
 description = "Using pytest markers to track functional coverage and filtering of tests"
 authors = ["Gleams API user <Stephen.Swannell+ghapi@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["test", "pytest", "markers", "coverage"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11.0"
 pytest = "^7.1.2"
 PyYAML = ">=5.4.1"
 loguru = "^0.6.0"
 pytest-xdist = "^2.5.0"
-pytest-jtr = ">=1.1.1"
-rich = "^12.6.0"
+pytest-jtr = ">=1.2.0"
+rich = "^13.3.0"
 
 [tool.poetry.dev-dependencies]
 nox = "^2022.1.7"
 tox = "^3.25.0"
 nox-poetry = "^1.0.0"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
```

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/coverage_markers/__init__.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/coverage_markers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/coverage_markers/marker_ops.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/coverage_markers/marker_ops.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filtering/filter_engine.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filtering/filter_engine.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/filtering/filter_ops.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/filtering/filter_ops.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/plugin.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/utils/checks.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/utils/checks.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/pytest_coveragemarkers/utils/yml_processing.py` & `pytest_coveragemarkers-2.1.0/pytest_coveragemarkers/utils/yml_processing.py`

 * *Files identical despite different names*

### Comparing `pytest-coveragemarkers-2.0.0/setup.py` & `pytest_coveragemarkers-2.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 
 package_data = \
 {'': ['*'], 'pytest_coveragemarkers.marker_specs': ['jira/*']}
 
 install_requires = \
 ['PyYAML>=5.4.1',
  'loguru>=0.6.0,<0.7.0',
- 'pytest-jtr>=1.1.1',
+ 'pytest-jtr>=1.2.0',
  'pytest-xdist>=2.5.0,<3.0.0',
  'pytest>=7.1.2,<8.0.0',
- 'rich>=12.6.0,<13.0.0']
+ 'rich>=13.3.0,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['prep-dev-release = scripts.prep_release:dev',
                      'prep-major-release = scripts.release_process:prep_major',
                      'prep-minor-release = scripts.release_process:prep_minor',
                      'prep-patch-release = scripts.release_process:prep_patch',
                      'release = scripts.release_process:upload_release'],
  'pytest11': ['coveragemarkers = pytest_coveragemarkers.plugin']}
 
 setup_kwargs = {
     'name': 'pytest-coveragemarkers',
-    'version': '2.0.0',
+    'version': '2.1.0',
     'description': 'Using pytest markers to track functional coverage and filtering of tests',
     'long_description': '======================\npytest-coveragemarkers\n======================\n\n.. image:: https://img.shields.io/badge/security-bandit-yellow.svg\n    :target: https://github.com/PyCQA/bandit\n    :alt: Security Status\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n\nUsing pytest markers to track functional coverage and filtering of tests\n\n----\n\nThis `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_\'s `cookiecutter-pytest-plugin`_ template.\n\n\nFeatures\n--------\n\n* Definition of CoverageMarkers© in YAML format\n* Support for applying CoverageMarkers© to tests\n* Filtering of tests based on CoverageMarkers©\n* Inclusion of CoverageMarkers© in JSON report\n\n\nInstallation\n------------\n\nYou can install "pytest-coveragemarkers" from `PyPI`_::\n\n    $ pip install pytest-coveragemarkers\n    # or\n    $ poetry add pytest-coveragemarkers\n\nUsage\n-----\n\nStep 1: Define your coverage markers yaml.\n\n    Using the format:\n\n.. code-block:: yaml\n\n  markers:\n    - name: <marker_name>\n      allowed:\n        - <marker_value_1>\n        - <marker_value_2>\n    - name: <marker2_name>\n      allowed:\n        - <marker2_value_1>\n        - <marker2_value_2>\n\nThen decorate your tests with them\n\n\n.. code-block:: python\n\n    import pytest\n\n    @pytest.mark.marker_name([\'value1\', \'value2\'])\n    @pytest.mark.marker2_name([\'value1\', \'value2\'])\n    def test_x():\n        ...\n\n    @pytest.mark.marker2_name([\'value1\', \'value2\'])\n    def test_y():\n        ...\n\n\nThen when the tests are executed with\n\n.. code-block:: shell\n\n    pytest --json-report --markers-location=/full/path/to/coverage_markers.yml\n\nThen the JSON Test Report output from the test execution contains:\n\n.. code-block:: json\n\n    "tests": [\n    {\n      "nodeid": "...",\n      "metadata": {\n        "cov_markers": {\n          "marker_name": {\n            "value1": true,\n            "value2": true\n          },\n          "marker2_name": {\n            "value1": true,\n            "value2": true\n          }\n        }\n      }\n    },\n    ...\n    ]\n\nThis can then be used to generate test coverage details based on the coverage markers.\nA nice demo will be produced to give examples of usage.\n\nBut wait there is another benefit:\n\nWe can filter tests for execution based on their coverage markers\n\n.. code-block:: shell\n\n    pytest \\\n        --filter=\'{"and": [{"eq": ["marker_name.value1", true]}]}\' \\\n        --json-report \\\n        --markers-location=/full/path/to/coverage_markers.yml\n\nThe above command run against the tests defined above would select \'test_x\' and deselect \'test_y\' for execution\n\nOther examples of filters are:\n\n.. code-block: shell\n\n    \'{"or": [{"eq": ["marker_name.value1", true]}, {"eq": ["marker_name.value2", true]}]}\'\n\nYou can also supply the path to a json file containing your filter.\nUse argument --filter-location or key FilterLocation in the pytest.ini file.\n\nCoverage Marker Argument Format\n-------------------------------\n\nThe arguments supplied to Coverage Markers can follow multiple formats which allows the user to define the format that best suites them.\n\nE.g.\n\n.. code-block:: python\n\n    import pytest\n\n    @pytest.mark.marker_1(\'value1\')                 # single string argument\n    @pytest.mark.marker_2(\'value1\', \'value2\')       # multiple string arguments\n    @pytest.mark.marker_3([\'value1\', \'value2\'])     # list of arguments\n    @pytest.mark.marker_4((\'value1\', \'value2\'))     # tuple of arguments\n    def test_x():\n        ...\n\n\n\nTesting\n-------\n\nNox is used by this project to execute all tests.\nTo run a specific set of tests execute the below line::\n\n    $ poetry run nox -s <session_name>\n\nWhere session_name can be one of the following\n\n.. list-table:: Nox Sessions\n   :widths: 25 75\n   :header-rows: 1\n\n   * - Session Name\n     - Session Details\n   * - unit_tests\n     - Execute all tests marked as unit\n   * - functional_tests\n     - Execute all tests marked as functional\n\nThought Process\n---------------\n\n* The `pytest_docs`_ talks about using markers to set metadata on tests and use the markers to select required tests for execution.\n* For the markers I want to add, I also want to specify a list of values that go along with that marker.\n  E.g. If the marker was \'colour\' then supported values may be \'Red\', \'Green\', \'Gold\'.\n* I also want the list of values validated against supported values so no unsupported values can be added.\n  E.g. If the marker was \'colour\' then a value of \'Panda\' would not be allowed.\n* Then all this meta data I want to come out in the junit json report.\n* Next I want to use these markers and their supported values to filter tests. For this I need a more powerful filter engine.\n\nDocumentation\n-------------\n\nTo build the docs run::\n\n    poetry run mkdocs serve\n\n\nLicense\n-------\n\nDistributed under the terms of the `MIT`_ license, "pytest-coveragemarkers" is free and open source software\n\n\nIssues\n------\n\nIf you encounter any problems, please `file an issue`_ along with a detailed description.\n\n\nFuture Changes\n--------------\n\n* Type-Hints\n* Full Test Coverage\n* Full Documentation\n* Refactor/rewrite\n* Pick one, yml or json?\n\n.. _`Cookiecutter`: https://github.com/audreyr/cookiecutter\n.. _`@hackebrot`: https://github.com/hackebrot\n.. _`MIT`: http://opensource.org/licenses/MIT\n.. _`BSD-3`: http://opensource.org/licenses/BSD-3-Clause\n.. _`GNU GPL v3.0`: http://www.gnu.org/licenses/gpl-3.0.txt\n.. _`Apache Software License 2.0`: http://www.apache.org/licenses/LICENSE-2.0\n.. _`cookiecutter-pytest-plugin`: https://github.com/pytest-dev/cookiecutter-pytest-plugin\n.. _`file an issue`: https://github.com/Gleams99/pytest-coveragemarkers/issues\n.. _`pytest`: https://github.com/pytest-dev/pytest\n.. _`nox`: https://nox.thea.codes/en/stable/\n.. _`pip`: https://pypi.org/project/pip/\n.. _`PyPI`: https://pypi.org/project\n.. _`pytest_docs`: https://docs.pytest.org/en/7.1.x/how-to/mark.html?highlight=slow\n',
     'author': 'Gleams API user',
     'author_email': 'Stephen.Swannell+ghapi@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.11.0',
 }
```

### Comparing `pytest-coveragemarkers-2.0.0/PKG-INFO` & `pytest_coveragemarkers-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: pytest-coveragemarkers
-Version: 2.0.0
+Version: 2.1.0
 Summary: Using pytest markers to track functional coverage and filtering of tests
 License: MIT
 Keywords: test,pytest,markers,coverage
 Author: Gleams API user
 Author-email: Stephen.Swannell+ghapi@gmail.com
 Requires-Python: >=3.8,<3.11.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pytest (>=7.1.2,<8.0.0)
-Requires-Dist: pytest-jtr (>=1.1.1)
+Requires-Dist: pytest-jtr (>=1.2.0)
 Requires-Dist: pytest-xdist (>=2.5.0,<3.0.0)
-Requires-Dist: rich (>=12.6.0,<13.0.0)
+Requires-Dist: rich (>=13.3.0,<14.0.0)
 Description-Content-Type: text/x-rst
 
 ======================
 pytest-coveragemarkers
 ======================
 
 .. image:: https://img.shields.io/badge/security-bandit-yellow.svg
```

