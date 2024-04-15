# Comparing `tmp/nox-2024.3.2.tar.gz` & `tmp/nox-2024.4.15.tar.gz`

## Comparing `nox-2024.3.2.tar` & `nox-2024.4.15.tar`

### file list

```diff
@@ -1,81 +1,83 @@
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 nox-2024.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nox-2024.3.2/.readthedocs.yml
--rw-r--r--   0        0        0    25093 2020-02-02 00:00:00.000000 nox-2024.3.2/CHANGELOG.md
--rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 nox-2024.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 nox-2024.3.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 nox-2024.3.2/action.yml
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 nox-2024.3.2/noxfile.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nox-2024.3.2/requirements-conda-test.txt
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nox-2024.3.2/requirements-dev.txt
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nox-2024.3.2/requirements-test.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/FUNDING.yml
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/action_helper.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/workflows/action.yml
--rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 nox-2024.3.2/.github/workflows/ci.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/Makefile
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/conf.py
--rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/config.rst
--rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/cookbook.rst
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/index.rst
--rw-r--r--   0        0        0    14923 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/tutorial.rst
--rw-r--r--   0        0        0    17371 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/usage.rst
--rw-r--r--   0        0        0  3379966 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/_static/alice-full.png
--rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/_static/alice.gif
--rw-r--r--   0        0        0   507218 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/_static/alice.png
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 nox-2024.3.2/docs/_static/custom.css
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/__init__.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/__main__.py
--rw-r--r--   0        0        0     4520 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/_decorators.py
--rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/_option_set.py
--rw-r--r--   0        0        0    20677 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/_options.py
--rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/_parametrize.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/_typing.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/_version.py
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/command.py
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/logger.py
--rw-r--r--   0        0        0    14188 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/manifest.py
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/popen.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/py.typed
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/registry.py
--rw-r--r--   0        0        0    34636 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/sessions.py
--rw-r--r--   0        0        0    14753 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/tasks.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/tox4_to_nox.jinja2
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/tox_to_nox.jinja2
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/tox_to_nox.py
--rw-r--r--   0        0        0    19786 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/virtualenv.py
--rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 nox-2024.3.2/nox/workflow.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/conftest.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test__option_set.py
--rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test__parametrize.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test__version.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_action_helper.py
--rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_command.py
--rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_logger.py
--rw-r--r--   0        0        0    28349 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_main.py
--rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_manifest.py
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_registry.py
--rw-r--r--   0        0        0    41487 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_sessions.py
--rw-r--r--   0        0        0    21250 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_tasks.py
--rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_tox_to_nox.py
--rw-r--r--   0        0        0    27300 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_virtualenv.py
--rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/test_workflow.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_multiple_sessions.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_nested.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_normalization.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_options.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_options_pythons.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_pythons.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_spaces.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nox-2024.3.2/tests/resources/noxfile_tags.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 nox-2024.3.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nox-2024.3.2/LICENSE
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 nox-2024.3.2/README.md
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 nox-2024.3.2/pyproject.toml
--rw-r--r--   0        0        0     4661 2020-02-02 00:00:00.000000 nox-2024.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 nox-2024.4.15/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nox-2024.4.15/.readthedocs.yml
+-rw-r--r--   0        0        0    26779 2020-02-02 00:00:00.000000 nox-2024.4.15/CHANGELOG.md
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 nox-2024.4.15/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 nox-2024.4.15/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 nox-2024.4.15/action.yml
+-rw-r--r--   0        0        0     6698 2020-02-02 00:00:00.000000 nox-2024.4.15/noxfile.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nox-2024.4.15/requirements-conda-test.txt
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nox-2024.4.15/requirements-dev.txt
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nox-2024.4.15/requirements-test.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/action_helper.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/dependabot.yml
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/workflows/action.yml
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 nox-2024.4.15/.github/workflows/ci.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/Makefile
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/conf.py
+-rw-r--r--   0        0        0    15314 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/config.rst
+-rw-r--r--   0        0        0     6028 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/cookbook.rst
+-rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/index.rst
+-rw-r--r--   0        0        0    16371 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/tutorial.rst
+-rw-r--r--   0        0        0    17279 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/usage.rst
+-rw-r--r--   0        0        0  3379966 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/_static/alice-full.png
+-rw-r--r--   0        0        0    10140 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/_static/alice.gif
+-rw-r--r--   0        0        0   507218 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/_static/alice.png
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 nox-2024.4.15/docs/_static/custom.css
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/__init__.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/__main__.py
+-rw-r--r--   0        0        0     4660 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/_decorators.py
+-rw-r--r--   0        0        0    11752 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/_option_set.py
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/_options.py
+-rw-r--r--   0        0        0     6201 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/_parametrize.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/_typing.py
+-rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/_version.py
+-rw-r--r--   0        0        0     4835 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/command.py
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/logger.py
+-rw-r--r--   0        0        0    14366 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/manifest.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/popen.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/project.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/py.typed
+-rw-r--r--   0        0        0     3259 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/registry.py
+-rw-r--r--   0        0        0    39672 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/sessions.py
+-rw-r--r--   0        0        0    14796 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/tasks.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/tox4_to_nox.jinja2
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/tox_to_nox.jinja2
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/tox_to_nox.py
+-rw-r--r--   0        0        0    21491 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/virtualenv.py
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 nox-2024.4.15/nox/workflow.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/conftest.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test__option_set.py
+-rw-r--r--   0        0        0     8538 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test__parametrize.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test__version.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_action_helper.py
+-rw-r--r--   0        0        0    15520 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_command.py
+-rw-r--r--   0        0        0     3116 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_logger.py
+-rw-r--r--   0        0        0    28349 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_main.py
+-rw-r--r--   0        0        0    14410 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_manifest.py
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_registry.py
+-rw-r--r--   0        0        0    44993 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_sessions.py
+-rw-r--r--   0        0        0    22105 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_tasks.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_toml.py
+-rw-r--r--   0        0        0     7132 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_tox_to_nox.py
+-rw-r--r--   0        0        0    30159 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_virtualenv.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/test_workflow.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_multiple_sessions.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_nested.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_normalization.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_options.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_options_pythons.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_pythons.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_spaces.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nox-2024.4.15/tests/resources/noxfile_tags.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 nox-2024.4.15/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 nox-2024.4.15/LICENSE
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 nox-2024.4.15/README.md
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nox-2024.4.15/pyproject.toml
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 nox-2024.4.15/PKG-INFO
```

### Comparing `nox-2024.3.2/.pre-commit-config.yaml` & `nox-2024.4.15/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
       - id: mypy
         files: ^nox/
         args: []
         additional_dependencies:
           - jinja2
           - packaging
           - importlib_metadata
+          - tomli
+          - uv
 
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.6
     hooks:
       - id: codespell
 
   - repo: https://github.com/pre-commit/pygrep-hooks
```

### Comparing `nox-2024.3.2/CHANGELOG.md` & `nox-2024.4.15/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,36 @@
 # Changelog
 
+## 2024.04.15
+
+We'd like to thank the following folks who contributed to this release:
+- @cjolowicz
+- @henryiii
+- @mayeut
+
+New features:
+* Added support for [PEP 723](https://peps.python.org/pep-0723/) (inline script metadata) with `nox.project.load_toml` by @henryiii in https://github.com/wntrblm/nox/pull/811
+* Added support for `micromamba` by @henryiii in https://github.com/wntrblm/nox/pull/807
+* Added `venv_backend` property to sessions by @henryiii in https://github.com/wntrblm/nox/pull/798
+* Added the ability to use `None` to remove environment variables by @henryiii in https://github.com/wntrblm/nox/pull/812
+* Added support for skipping sessions by default using `default=False` by @henryiii in https://github.com/wntrblm/nox/pull/810
+
+## Bugfixes
+
+* Use static arguments instead of `**kwargs` by @henryiii in https://github.com/wntrblm/nox/pull/815
+* Do not depend on `pipx` in Nox GitHub action by @mayeut in https://github.com/wntrblm/nox/pull/768
+* Disallow `UV_SYSTEM_PYTHON` by @henryiii in https://github.com/wntrblm/nox/pull/817
+* Ensure 'uv' always works in a uv venv by @henryiii in https://github.com/wntrblm/nox/pull/818
+* Look for `uv` next to `python` if it's not on `PATH` by @cjolowicz in https://github.com/wntrblm/nox/pull/795
+* Fixed missing f-string in `--help` message by @cjolowicz in https://github.com/wntrblm/nox/pull/790
+* Don't error if not installing to passthrough by @henryiii in https://github.com/wntrblm/nox/pull/809
+* Avoid mixing `venv` and `conda` from environment by @henryiii in https://github.com/wntrblm/nox/pull/804
+* Skip test for conda env when `conda` isn't installed by @cjolowicz in https://github.com/wntrblm/nox/pull/794
+
+
 ## 2024.03.02
 
 We'd like to thank the following folks who contributed to this release:
 - @DiddiLeija
 - @MicaelJarniac
 - @chrysle
 - @edgarrmondragon
```

### Comparing `nox-2024.3.2/CODE_OF_CONDUCT.md` & `nox-2024.4.15/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/CONTRIBUTING.md` & `nox-2024.4.15/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/noxfile.py` & `nox-2024.4.15/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,25 @@
 import sqlite3
 import sys
 
 import nox
 
 ON_WINDOWS_CI = "CI" in os.environ and platform.system() == "Windows"
 
+nox.needs_version = ">=2024.3.2"
+nox.options.default_venv_backend = "uv|virtualenv"
+
 # Skip 'conda_tests' if user doesn't have conda installed
 nox.options.sessions = ["tests", "cover", "lint", "docs"]
 if shutil.which("conda"):
     nox.options.sessions.append("conda_tests")
+if shutil.which("mamba"):
+    nox.options.sessions.append("mamba_tests")
+if shutil.which("micromamba"):
+    nox.options.sessions.append("micromamba_tests")
 
 
 # Because there is a dependency conflict between argcomplete and the latest tox
 # (both depend on a different version of importlibmetadata for Py 3.7) pip
 # installs tox 3 as the latest one for Py 3.7.
 @nox.session
 @nox.parametrize(
@@ -72,32 +79,51 @@
 
     if sys.platform.startswith("win"):
         with contextlib.closing(sqlite3.connect(coverage_file)) as con, con:
             con.execute("UPDATE file SET path = REPLACE(path, '\\', '/')")
             con.execute("DELETE FROM file WHERE SUBSTR(path, 2, 1) == ':'")
 
 
-@nox.session(python=["3.7", "3.8", "3.9", "3.10"], venv_backend="conda")
+@nox.session(venv_backend="conda")
 def conda_tests(session: nox.Session) -> None:
-    """Run test suite with pytest."""
-    session.create_tmp()  # Fixes permission errors on Windows
+    """Run test suite set up with conda."""
+    session.conda_install(
+        "--file", "requirements-conda-test.txt", channel="conda-forge"
+    )
+    session.install("-e", ".", "--no-deps")
+    session.run("pytest", *session.posargs)
+
+
+@nox.session(venv_backend="mamba")
+def mamba_tests(session: nox.Session) -> None:
+    """Run test suite set up with mamba."""
+    session.conda_install(
+        "--file", "requirements-conda-test.txt", channel="conda-forge"
+    )
+    session.install("-e", ".", "--no-deps")
+    session.run("pytest", *session.posargs)
+
+
+@nox.session(venv_backend="micromamba")
+def micromamba_tests(session: nox.Session) -> None:
+    """Run test suite set up with micromamba."""
     session.conda_install(
-        "--file", "requirements-conda-test.txt", "--channel", "conda-forge"
+        "--file", "requirements-conda-test.txt", channel="conda-forge"
     )
     session.install("-e", ".", "--no-deps")
     session.run("pytest", *session.posargs)
 
 
 @nox.session
 def cover(session: nox.Session) -> None:
     """Coverage analysis."""
     if ON_WINDOWS_CI:
         return
 
-    session.install("coverage[toml]>=5.3")
+    session.install("coverage[toml]>=7.3")
     session.run("coverage", "combine")
     session.run("coverage", "report", "--fail-under=100", "--show-missing")
     session.run("coverage", "erase")
 
 
 @nox.session(python="3.9")
 def lint(session: nox.Session) -> None:
@@ -170,15 +196,14 @@
 )
 def github_actions_default_tests(session: nox.Session) -> None:
     """Check default versions installed by the nox GHA Action"""
     assert sys.version_info[:2] == (3, 11)
     _check_python_version(session)
 
 
-# The following sessions are only to be run in CI to check the nox GHA action
 @nox.session(
     python=[
         "3.7",
         "3.8",
         "3.9",
         "3.10",
         "3.11",
@@ -188,7 +213,23 @@
         "pypy3.9",
         "pypy3.10",
     ]
 )
 def github_actions_all_tests(session: nox.Session) -> None:
     """Check all versions installed by the nox GHA Action"""
     _check_python_version(session)
+
+
+@nox.session(
+    python=[
+        "3.10",
+        "3.11",
+        "3.12",
+        "pypy3.8",
+        "pypy3.9",
+        "pypy3.10",
+    ]
+)
+def github_actions_macos_14(session: nox.Session) -> None:
+    """Check default versions installed by the nox GHA Action"""
+    assert sys.version_info[:2] == (3, 11)
+    _check_python_version(session)
```

### Comparing `nox-2024.3.2/.github/action_helper.py` & `nox-2024.4.15/.github/action_helper.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/.github/ISSUE_TEMPLATE/bug.yml` & `nox-2024.4.15/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/.github/ISSUE_TEMPLATE/feature_request.yml` & `nox-2024.4.15/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/.github/workflows/action.yml` & `nox-2024.4.15/.github/workflows/action.yml`

 * *Files 12% similar despite different names*

```diff
@@ -28,18 +28,28 @@
             macos-12,
             macos-13,
           ]
     steps:
       - uses: actions/checkout@v4
       - uses: ./
       - run: nox --non-interactive --error-on-missing-interpreter --session github_actions_default_tests
+
   action-all-tests:
     runs-on: windows-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions/setup-python@v5
         with:
           python-version: 3.9
       - uses: ./
         with:
           python-versions: "3.4, 3.5, 3.6, 3.7, 3.8, 3.9, 3.10, 3.11, 3.12, pypy-2.7, pypy-3.7, pypy-3.8, pypy-3.9, pypy-3.10"
       - run: nox --non-interactive --error-on-missing-interpreter --session github_actions_all_tests
+
+  action-macos14-tests:
+    runs-on: macos-14
+    steps:
+      - uses: actions/checkout@v4
+      - uses: ./
+        with:
+          python-versions: "3.10, 3.11, 3.12, pypy-3.8, pypy-3.9, pypy-3.10"
+      - run: nox --non-interactive --error-on-missing-interpreter --session github_actions_macos_14
```

### Comparing `nox-2024.3.2/.github/workflows/ci.yml` & `nox-2024.4.15/.github/workflows/ci.yml`

 * *Files 7% similar despite different names*

```diff
@@ -13,33 +13,40 @@
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   build:
     runs-on: ${{ matrix.os }}
     strategy:
+      fail-fast: false
       matrix:
         os: [ubuntu-20.04, windows-latest, macos-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
+      - name: Setup uv
+        uses: yezz123/setup-uv@v4
+        if: matrix.python-version != '3.7'
       - name: Set up Miniconda
         uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
           miniforge-variant: Mambaforge
           use-mamba: true
-      - name: Install Nox-under-test
-        run: |
-          python -m pip install --disable-pip-version-check .
+      - name: Install Nox-under-test (uv)
+        if: matrix.python-version != '3.7'
+        run:  uv pip install --system .
+      - name: Install Nox-under-test (pip)
+        if: matrix.python-version == '3.7'
+        run: python -m pip install --disable-pip-version-check .
       - name: Run tests on ${{ matrix.os }} (tox <4)
         run: nox --non-interactive --error-on-missing-interpreter --session "tests(python='${{ matrix.python-version }}', tox_version='<4')" -- --full-trace
       - name: Run tox-to-nox tests on ${{ matrix.os }} (tox latest)
         run: nox --non-interactive --error-on-missing-interpreter --session "tests(python='${{ matrix.python-version }}', tox_version='latest')" -- tests/test_tox_to_nox.py --full-trace
         if: matrix.python-version != '3.7'
       - name: Save coverage report
         uses: actions/upload-artifact@v4
@@ -52,17 +59,18 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python 3.11
         uses: actions/setup-python@v5
         with:
           python-version: "3.11"
+      - name: Setup uv
+        uses: yezz123/setup-uv@v4
       - name: Install Nox-under-test
-        run: |
-          python -m pip install --disable-pip-version-check .
+        run:  uv pip install --system .
       - name: Download individual coverage reports
         uses: actions/download-artifact@v4
         with:
           pattern: coverage-*
           merge-multiple: true
       - name: Display structure of downloaded files
         run: ls -aR
@@ -74,29 +82,29 @@
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python 3.9
         uses: actions/setup-python@v5
         with:
           python-version: 3.9
       - name: Install Nox-under-test
-        run: |
-          python -m pip install --disable-pip-version-check .
+        run: python -m pip install --disable-pip-version-check .
       - name: Lint
         run: nox --non-interactive --error-on-missing-interpreter --session "lint"
   docs:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python 3.9
         uses: actions/setup-python@v5
         with:
           python-version: 3.9
+      - name: Setup uv
+        uses: yezz123/setup-uv@v4
       - name: Install Nox-under-test
-        run: |
-          python -m pip install --disable-pip-version-check .
+        run:  uv pip install --system .
       - name: Docs
         run: nox --non-interactive --error-on-missing-interpreter --session "docs"
   deploy:
     needs: build
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     steps:
```

### Comparing `nox-2024.3.2/docs/Makefile` & `nox-2024.4.15/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/conf.py` & `nox-2024.4.15/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/config.rst` & `nox-2024.4.15/docs/config.rst`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 
     @nox.session
     def tests(session):
         session.run('pytest')
 
 You can also configure sessions to run against multiple Python versions as described in :ref:`virtualenv config` and  parametrize sessions as described in :ref:`parametrized sessions <parametrized>`.
 
+By default, all sessions will be run if no sessions are specified. You can
+remove sessions from this default list by passing ``default=False`` in the
+``@nox.session(...)`` decorator. You can also specify a list of sessions to run by
+default using the ``nox.options.sessions = [...]`` configuration option.
 
 Session description
 -------------------
 
 You can add a description to your session using a `docstring <https://www.python.org/dev/peps/pep-0257>`__.
 The first line will be shown when listing the sessions. For example:
 
@@ -163,30 +167,38 @@
 
     @nox.session(
         python=['2.7', '3.6'],
         reuse_venv=True)
     def tests(session):
         pass
 
-You are not limited to virtualenv, there is a selection of backends you can choose from as venv, conda, mamba, or virtualenv (default):
+You are not limited to virtualenv, there is a selection of backends you can choose from as venv, uv, conda, mamba, micromamba, or virtualenv (default):
 
 .. code-block:: python
 
     @nox.session(venv_backend='venv')
     def tests(session):
         pass
 
+You can chain together optional backends with ``|``, such as ``uv|virtualenv``
+or ``micromamba|mamba|conda``, and the first available backend will be selected.
+You cannot put anything after a backend that can't be missing like ``venv`` or
+``virtualenv``.
+
 Finally, custom backend parameters are supported:
 
 .. code-block:: python
 
     @nox.session(venv_params=['--no-download'])
     def tests(session):
         pass
 
+If you need to check to see which backend was selected, you can access it via
+``session.venv_backend``.
+
 
 Passing arguments into sessions
 -------------------------------
 
 Often it's useful to pass arguments into your test session. Here's a quick
 example that demonstrates how to use arguments to run tests against a
 particular file:
@@ -409,15 +421,15 @@
 
     nox.options.envdir = ".cache"
 
     @nox.session
     def tests(session):
         ...
 
-Or, if you wanted to provide a set of sessions that are run by default:
+Or, if you wanted to provide a set of sessions that are run by default (this overrides the ``default=`` argument to sessions):
 
 .. code-block:: python
 
     import nox
 
     nox.options.sessions = ["lint", "tests-3.6"]
```

### Comparing `nox-2024.3.2/docs/cookbook.rst` & `nox-2024.4.15/docs/cookbook.rst`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/index.rst` & `nox-2024.4.15/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/tutorial.rst` & `nox-2024.4.15/docs/tutorial.rst`

 * *Files 5% similar despite different names*

```diff
@@ -165,14 +165,54 @@
         )
         session.install(".")
         ...
 
 These commands will run even if you are only installing, and will not run if
 the environment is being reused without reinstallation.
 
+
+Loading dependencies from pyproject.toml or scripts
+---------------------------------------------------
+
+One common need is loading a dependency list from a ``pyproject.toml`` file
+(say to prepare an environment without installing the package) or supporting
+`PEP 723 <https://peps.python.org/pep-0723>`_ scripts. Nox provides a helper to
+load these with ``nox.project.load_toml``. It can be passed a filepath to a toml
+file or to a script file following PEP 723. For example, if you have the
+following ``peps.py``:
+
+
+.. code-block:: python
+
+    # /// script
+    # requires-python = ">=3.11"
+    # dependencies = [
+    #   "requests<3",
+    #   "rich",
+    # ]
+    # ///
+
+    import requests
+    from rich.pretty import pprint
+
+    resp = requests.get("https://peps.python.org/api/peps.json")
+    data = resp.json()
+    pprint([(k, v["title"]) for k, v in data.items()][:10])
+
+You can make a session for it like this:
+
+.. code-block:: python
+
+   @nox.session
+   def peps(session):
+       requirements = nox.project.load_toml("peps.py")["dependencies"]
+       session.install(*requirements)
+       session.run("peps.py")
+
+
 Running commands
 ----------------
 
 The ``session.run`` function lets you run commands within the context of your
 session's virtual environment. Here's a few examples:
 
 You can install and run Python tools:
@@ -393,29 +433,33 @@
     def test(session):
         ...
 
 Install packages with conda:
 
 .. code-block:: python
 
-    session.conda_install("pytest")
+    session.conda_install("pytest", channels=["conda-forge"])
 
 It is possible to install packages with pip into the conda environment, but
 it's a best practice only install pip packages with the ``--no-deps`` option.
-This prevents pip from breaking the conda environment by installing
-incompatible versions of packages already installed with conda.
+This prevents pip from breaking the conda environment by installing incompatible
+versions of packages already installed with conda. You should always specify
+channels for consistency; default channels can vary (and ``micromamba`` has none).
 
 .. code-block:: python
 
     session.install("contexter", "--no-deps")
     session.install("-e", ".", "--no-deps")
 
 ``"mamba"`` is also allowed as a choice for ``venv_backend``, which will
 use/require `mamba <https://github.com/mamba-org/mamba>`_ instead of conda.
 
+``"micromamba"`` is also allowed as a choice for ``venv_backend``, which will
+use/require `micromamba <https://mamba.readthedocs.io/en/latest/user_guide/micromamba.html#>`_
+instead of conda.
 
 Parametrization
 ---------------
 
 Just like Nox can handle running against multiple interpreters, Nox can also
 handle running your sessions with a list of different arguments using the
 :func:`nox.parametrize` decorator.
```

### Comparing `nox-2024.3.2/docs/usage.rst` & `nox-2024.4.15/docs/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
 
 
 .. _opt-default-venv-backend:
 
 Changing the sessions default backend
 -------------------------------------
 
-By default Nox uses ``virtualenv`` as the virtual environment backend for the sessions, but it also supports ``uv``, ``conda``, ``mamba``, and ``venv`` as well as no backend (passthrough to whatever python environment Nox is running on). You can change the default behaviour by using ``-db <backend>`` or ``--default-venv-backend <backend>``. Supported names are ``('none', 'uv', 'virtualenv', 'conda', 'mamba', 'venv')``.
+By default Nox uses ``virtualenv`` as the virtual environment backend for the sessions, but it also supports ``uv``, ``conda``, ``mamba``, ``micromamba``, and ``venv`` as well as no backend (passthrough to whatever python environment Nox is running on). You can change the default behaviour by using ``-db <backend>`` or ``--default-venv-backend <backend>``. Supported names are ``('none', 'uv', 'virtualenv', 'conda', 'mamba', 'venv')``.
 
 
 .. tabs::
 
    .. code-tab:: console CLI options
 
          nox -db conda
@@ -138,43 +138,39 @@
 
    .. code-tab:: console Environment variables
 
          NOX_DEFAULT_VENV_BACKEND=conda
 
 .. note::
 
-   The ``uv``, ``conda``, and ``mamba`` backends require their respective
-   programs be pre-installed. ``uv`` is distributed as a Python package
-   and can be installed with the ``nox[uv]`` extra.
+   The ``uv``, ``conda``, ``mamba``, and ``micromamba`` backends require their
+   respective programs be pre-installed. ``uv`` is distributed as a Python
+   package and can be installed with the ``nox[uv]`` extra.
 
 You can also set this option with the ``NOX_DEFAULT_VENV_BACKEND`` environment variable, or in the Noxfile with ``nox.options.default_venv_backend``. In case more than one is provided, the command line argument overrides the environment variable, which in turn overrides the Noxfile configuration.
 
 Note that using this option does not change the backend for sessions where ``venv_backend`` is explicitly set.
 
 .. warning::
 
    The ``uv`` backend does not install anything by default, including ``pip``,
    as ``uv pip`` is used to install programs instead. If you need to manually
    interact with pip, you should install it with ``session.install("pip")``.
 
-.. warning::
-
-   Currently the ``uv`` backend requires the ``<program name> @ .`` syntax to
-   install a local folder in non-editable mode; it does not (yet) compute the
-   name from the install process like pip does if the name is omitted. Editable
-   installs do not require a name.
+Backends that could be missing (``uv``, ``conda``, ``mamba``, and ``micromamba``) can have a fallback using ``|``, such as ``uv|virtualenv`` or ``micromamba|mamba|conda``. This will use the first item that is available on the users system.
 
-Backends that could be missing (``uv``, ``conda``, and ``mamba``) can have a fallback using ``|``, such as ``uv|virtualenv`` or ``mamba|conda``. This will use the first item that is available on the users system.
+If you need to check to see which backend was selected, you can access it via
+``session.venv_backend`` in your noxfile.
 
 .. _opt-force-venv-backend:
 
 Forcing the sessions backend
 ----------------------------
 
-You might work in a different environment than a project's default continuous integration settings, and might wish to get a quick way to execute the same tasks but on a different venv backend. For this purpose, you can temporarily force the backend used by **all** sessions in the current Nox execution by using ``-fb <backend>`` or ``--force-venv-backend <backend>``. No exceptions are made, the backend will be forced for all sessions run whatever the other options values and Noxfile configuration. Supported names are ``('none', 'uv', 'virtualenv', 'conda', 'mamba', 'venv')``.
+You might work in a different environment than a project's default continuous integration settings, and might wish to get a quick way to execute the same tasks but on a different venv backend. For this purpose, you can temporarily force the backend used by **all** sessions in the current Nox execution by using ``-fb <backend>`` or ``--force-venv-backend <backend>``. No exceptions are made, the backend will be forced for all sessions run whatever the other options values and Noxfile configuration. Supported names are ``('none', 'uv', 'virtualenv', 'conda', 'mamba', 'micromamba', 'venv')``.
 
 .. code-block:: console
 
     nox -fb conda
     nox --force-venv-backend conda
```

### Comparing `nox-2024.3.2/docs/_static/alice-full.png` & `nox-2024.4.15/docs/_static/alice-full.png`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/_static/alice.gif` & `nox-2024.4.15/docs/_static/alice.gif`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/_static/alice.png` & `nox-2024.4.15/docs/_static/alice.png`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/docs/_static/custom.css` & `nox-2024.4.15/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/__init__.py` & `nox-2024.4.15/nox/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,16 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from nox import project
 from nox._options import noxfile_options as options
 from nox._parametrize import Param as param
 from nox._parametrize import parametrize_decorator as parametrize
 from nox.registry import session_decorator as session
 from nox.sessions import Session
 
 needs_version: str | None = None
 
-__all__ = ["needs_version", "parametrize", "param", "session", "options", "Session"]
+__all__ = [
+    "needs_version",
+    "parametrize",
+    "param",
+    "session",
+    "options",
+    "Session",
+    "project",
+]
```

### Comparing `nox-2024.3.2/nox/__main__.py` & `nox-2024.4.15/nox/__main__.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/_decorators.py` & `nox-2024.4.15/nox/_decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -65,23 +65,26 @@
         python: _typing.Python = None,
         reuse_venv: bool | None = None,
         name: str | None = None,
         venv_backend: Any = None,
         venv_params: Any = None,
         should_warn: Mapping[str, Any] | None = None,
         tags: Sequence[str] | None = None,
+        *,
+        default: bool = True,
     ) -> None:
         self.func = func
         self.python = python
         self.reuse_venv = reuse_venv
         self.name = name
         self.venv_backend = venv_backend
         self.venv_params = venv_params
         self.should_warn = dict(should_warn or {})
         self.tags = list(tags or [])
+        self.default = default
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def copy(self, name: str | None = None) -> Func:
         """Copy this function with a new name."""
 
@@ -90,14 +93,15 @@
             self.python,
             self.reuse_venv,
             name,
             self.venv_backend,
             self.venv_params,
             self.should_warn,
             self.tags,
+            default=self.default,
         )
 
 
 class Call(Func):
     """This represents a call of a function with a particular set of arguments."""
 
     def __init__(self, func: Func, param_spec: Param) -> None:
@@ -121,14 +125,15 @@
             python,
             func.reuse_venv,
             None,
             func.venv_backend,
             func.venv_params,
             func.should_warn,
             func.tags,
+            default=func.default,
         )
         self.call_spec = call_spec
         self.session_signature = session_signature
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         kwargs.update(self.call_spec)
         return super().__call__(*args, **kwargs)
```

### Comparing `nox-2024.3.2/nox/_option_set.py` & `nox-2024.4.15/nox/_option_set.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/_options.py` & `nox-2024.4.15/nox/_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,29 +420,29 @@
         "--default-venv-backend",
         group=options.groups["environment"],
         noxfile=True,
         default=lambda: os.environ.get("NOX_DEFAULT_VENV_BACKEND"),
         merge_func=_default_venv_backend_merge_func,
         help=(
             "Virtual environment backend to use by default for Nox sessions, this is"
-            " ``'virtualenv'`` by default but any of ``{list(ALL_VENVS)!r}`` are accepted."
+            f" ``'virtualenv'`` by default but any of ``{list(ALL_VENVS)!r}`` are accepted."
         ),
         choices=list(ALL_VENVS),
     ),
     _option_set.Option(
         "force_venv_backend",
         "-fb",
         "--force-venv-backend",
         group=options.groups["environment"],
         noxfile=True,
         merge_func=_force_venv_backend_merge_func,
         help=(
             "Virtual environment backend to force-use for all Nox sessions in this run,"
             " overriding any other venv backend declared in the Noxfile and ignoring"
-            " the default backend. Any of ``{list(ALL_VENVS)!r}`` are accepted."
+            f" the default backend. Any of ``{list(ALL_VENVS)!r}`` are accepted."
         ),
         choices=list(ALL_VENVS),
     ),
     _option_set.Option(
         "no_venv",
         "--no-venv",
         group=options.groups["environment"],
```

### Comparing `nox-2024.3.2/nox/_parametrize.py` & `nox-2024.4.15/nox/_parametrize.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/_typing.py` & `nox-2024.4.15/nox/_typing.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/_version.py` & `nox-2024.4.15/nox/_version.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/command.py` & `nox-2024.4.15/nox/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,26 +13,31 @@
 # limitations under the License.
 
 from __future__ import annotations
 
 import os
 import shlex
 import shutil
+import subprocess
 import sys
 from collections.abc import Iterable, Mapping, Sequence
-from typing import Any
 
 from nox.logger import logger
-from nox.popen import popen
+from nox.popen import DEFAULT_INTERRUPT_TIMEOUT, DEFAULT_TERMINATE_TIMEOUT, popen
 
 if sys.version_info < (3, 8):
     from typing_extensions import Literal
 else:
     from typing import Literal
 
+TYPE_CHECKING = False
+
+if TYPE_CHECKING:
+    from typing import IO
+
 ExternalType = Literal["error", True, False]
 
 
 class CommandFailed(Exception):
     """Raised when an executed command returns a non-success status code."""
 
     def __init__(self, reason: str | None = None) -> None:
@@ -51,43 +56,44 @@
     if full_path:
         return os.fspath(full_path)
 
     logger.error(f"Program {program} not found.")
     raise CommandFailed(f"Program {program} not found")
 
 
-def _clean_env(env: Mapping[str, str] | None = None) -> dict[str, str] | None:
+def _clean_env(env: Mapping[str, str | None] | None = None) -> dict[str, str] | None:
     if env is None:
         return None
 
-    clean_env: dict[str, str] = {}
+    clean_env = {k: v for k, v in env.items() if v is not None}
 
     # Ensure systemroot is passed down, otherwise Windows will explode.
     if sys.platform == "win32":
-        clean_env["SYSTEMROOT"] = os.environ.get("SYSTEMROOT", "")
-
-    clean_env.update(env)
+        clean_env.setdefault("SYSTEMROOT", os.environ.get("SYSTEMROOT", ""))
 
     return clean_env
 
 
 def _shlex_join(args: Sequence[str | os.PathLike[str]]) -> str:
     return " ".join(shlex.quote(os.fspath(arg)) for arg in args)
 
 
 def run(
     args: Sequence[str | os.PathLike[str]],
     *,
-    env: Mapping[str, str] | None = None,
+    env: Mapping[str, str | None] | None = None,
     silent: bool = False,
     paths: Sequence[str] | None = None,
     success_codes: Iterable[int] | None = None,
     log: bool = True,
     external: ExternalType = False,
-    **popen_kws: Any,
+    stdout: int | IO[str] | None = None,
+    stderr: int | IO[str] = subprocess.STDOUT,
+    interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+    terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
 ) -> str | bool:
     """Run a command-line program."""
 
     if success_codes is None:
         success_codes = [0]
 
     cmd, args = args[0], args[1:]
@@ -117,15 +123,21 @@
                     " external=True into run() to silence this message."
                 )
 
     env = _clean_env(env)
 
     try:
         return_code, output = popen(
-            [cmd_path, *str_args], silent=silent, env=env, **popen_kws
+            [cmd_path, *str_args],
+            silent=silent,
+            env=env,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
         )
 
         if return_code not in success_codes:
             suffix = ":" if silent else ""
             logger.error(
                 f"Command {full_cmd} failed with exit code {return_code}{suffix}"
             )
```

### Comparing `nox-2024.3.2/nox/logger.py` & `nox-2024.4.15/nox/logger.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/manifest.py` & `nox-2024.4.15/nox/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,19 @@
             session_name
             for session_name in specified_sessions
             if _normalize_arg(session_name) not in all_sessions
         ]
         if missing_sessions:
             raise KeyError(f"Sessions not found: {', '.join(missing_sessions)}")
 
+    def filter_by_default(self) -> None:
+        """Filter sessions in the queue based on the default flag."""
+
+        self._queue = [x for x in self._queue if x.func.default]
+
     def filter_by_python_interpreter(self, specified_pythons: Sequence[str]) -> None:
         """Filter sessions in the queue based on the user-specified
         python interpreter versions.
 
         Args:
             specified_pythons (Sequence[str]): A list of specified
                 python interpreter versions.
```

### Comparing `nox-2024.3.2/nox/popen.py` & `nox-2024.4.15/nox/popen.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 import contextlib
 import locale
 import subprocess
 import sys
 from collections.abc import Mapping, Sequence
 from typing import IO
 
+DEFAULT_INTERRUPT_TIMEOUT = 0.3
+DEFAULT_TERMINATE_TIMEOUT = 0.2
+
 
 def shutdown_process(
     proc: subprocess.Popen[bytes],
     interrupt_timeout: float | None,
     terminate_timeout: float | None,
 ) -> tuple[bytes, bytes]:
     """Gracefully shutdown a child process."""
@@ -60,16 +63,16 @@
 
 def popen(
     args: Sequence[str],
     env: Mapping[str, str] | None = None,
     silent: bool = False,
     stdout: int | IO[str] | None = None,
     stderr: int | IO[str] = subprocess.STDOUT,
-    interrupt_timeout: float | None = 0.3,
-    terminate_timeout: float | None = 0.2,
+    interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+    terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
 ) -> tuple[int, str]:
     if silent and stdout is not None:
         raise ValueError(
             "Can not specify silent and stdout; passing a custom stdout always silences"
             " the commands output in Nox's log."
         )
```

### Comparing `nox-2024.3.2/nox/registry.py` & `nox-2024.4.15/nox/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,27 +39,31 @@
     python: Python | None = ...,
     py: Python | None = ...,
     reuse_venv: bool | None = ...,
     name: str | None = ...,
     venv_backend: Any | None = ...,
     venv_params: Any | None = ...,
     tags: Sequence[str] | None = ...,
+    *,
+    default: bool = ...,
 ) -> Callable[[F], F]:
     ...
 
 
 def session_decorator(
     func: F | None = None,
     python: Python | None = None,
     py: Python | None = None,
     reuse_venv: bool | None = None,
     name: str | None = None,
     venv_backend: Any | None = None,
     venv_params: Any | None = None,
     tags: Sequence[str] | None = None,
+    *,
+    default: bool = True,
 ) -> F | Callable[[F], F]:
     """Designate the decorated function as a session."""
     # If `func` is provided, then this is the decorator call with the function
     # being sent as part of the Python syntax (`@nox.session`).
     # If `func` is None, however, then this is a plain function call, and it
     # must return the decorator that ultimately is applied
     # (`@nox.session(...)`).
@@ -71,28 +75,36 @@
             python=python,
             py=py,
             reuse_venv=reuse_venv,
             name=name,
             venv_backend=venv_backend,
             venv_params=venv_params,
             tags=tags,
+            default=default,
         )
 
     if py is not None and python is not None:
         raise ValueError(
             "The py argument to nox.session is an alias for the python "
             "argument, please only specify one."
         )
 
     if python is None:
         python = py
 
     final_name = name or func.__name__
     fn = Func(
-        func, python, reuse_venv, final_name, venv_backend, venv_params, tags=tags
+        func,
+        python,
+        reuse_venv,
+        final_name,
+        venv_backend,
+        venv_params,
+        tags=tags,
+        default=default,
     )
     _REGISTRY[final_name] = fn
     return fn
 
 
 def get() -> collections.OrderedDict[str, Func]:
     """Return a shallow copy of the registry.
```

### Comparing `nox-2024.3.2/nox/sessions.py` & `nox-2024.4.15/nox/sessions.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 import argparse
 import contextlib
 import enum
 import hashlib
 import os
 import pathlib
 import re
+import shutil
+import subprocess
 import sys
 import unicodedata
 from collections.abc import (
     Callable,
     Generator,
     Iterable,
     Mapping,
@@ -37,17 +39,21 @@
     NoReturn,
 )
 
 import nox.command
 import nox.virtualenv
 from nox._decorators import Func
 from nox.logger import logger
+from nox.popen import DEFAULT_INTERRUPT_TIMEOUT, DEFAULT_TERMINATE_TIMEOUT
 from nox.virtualenv import CondaEnv, PassthroughEnv, ProcessEnv, VirtualEnv
 
 if TYPE_CHECKING:
+    from typing import IO
+
+    from nox.command import ExternalType
     from nox.manifest import Manifest
 
 
 @contextlib.contextmanager
 def _chdir(path: str) -> Generator[None, None, None]:
     """
     Change the current working directory to the given path.
@@ -190,14 +196,22 @@
         """The virtualenv that all commands are run in."""
         venv = self._runner.venv
         if venv is None:
             raise ValueError("A virtualenv has not been created for this session")
         return venv
 
     @property
+    def venv_backend(self) -> str:
+        """The venv_backend selected."""
+        venv = self._runner.venv
+        if venv is None:
+            return "none"
+        return venv.venv_backend
+
+    @property
     def python(self) -> str | Sequence[str] | bool | None:
         """The python version passed into ``@nox.session``."""
         return self._runner.func.python
 
     @property
     def bin_paths(self) -> list[str] | None:
         """The bin directories for the virtualenv."""
@@ -257,31 +271,36 @@
         """
         self.log(f"cd {dir}")
         return _WorkingDirContext(dir)
 
     cd = chdir
     """An alias for :meth:`chdir`."""
 
-    def _run_func(
-        self, func: Callable[..., Any], args: Iterable[Any], kwargs: Mapping[str, Any]
-    ) -> Any:
+    def _run_func(self, func: Callable[..., Any], args: Iterable[Any]) -> Any:
         """Legacy support for running a function through :func`run`."""
-        self.log(f"{func}(args={args!r}, kwargs={kwargs!r})")
+        self.log(f"{func}(args={args!r})")
         try:
-            return func(*args, **kwargs)
+            return func(*args)
         except Exception as e:
             logger.exception(f"Function {func!r} raised {e!r}.")
             raise nox.command.CommandFailed() from e
 
     def run(
         self,
         *args: str | os.PathLike[str],
-        env: Mapping[str, str] | None = None,
+        env: Mapping[str, str | None] | None = None,
         include_outer_env: bool = True,
-        **kwargs: Any,
+        silent: bool = False,
+        success_codes: Iterable[int] | None = None,
+        log: bool = True,
+        external: ExternalType | None = None,
+        stdout: int | IO[str] | None = None,
+        stderr: int | IO[str] = subprocess.STDOUT,
+        interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+        terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
     ) -> Any | None:
         """Run a command.
 
         Commands must be specified as a list of strings, for example::
 
             session.run('pytest', '-k', 'fast', 'tests/')
             session.run('flake8', '--import-order-style=google')
@@ -338,15 +357,17 @@
                 "git", "rev-parse", "--short", "HEAD",
                 external=True, silent=True
             )
 
             print("Current Git commit is", out.strip())
 
         :param env: A dictionary of environment variables to expose to the
-            command. By default, all environment variables are passed.
+            command. By default, all environment variables are passed. You
+            can block an environment variable from the outer environment by
+            setting it to None.
         :type env: dict or None
         :param include_outer_env: Boolean parameter that determines if the
             environment variables from the nox invocation environment should
             be passed to the command. ``True`` by default.
         :type include_outer_env: bool
         :param bool silent: Silence command output, unless the command fails.
             If ``True``, returns the command output (unless the command fails).
@@ -388,23 +409,37 @@
             logger.info(f"Skipping {args[0]} run, as --install-only is set.")
             return None
 
         return self._run(
             *args,
             env=env,
             include_outer_env=include_outer_env,
-            **kwargs,
+            silent=silent,
+            success_codes=success_codes,
+            log=log,
+            external=external,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
         )
 
     def run_install(
         self,
         *args: str | os.PathLike[str],
-        env: Mapping[str, str] | None = None,
+        env: Mapping[str, str | None] | None = None,
         include_outer_env: bool = True,
-        **kwargs: Any,
+        silent: bool = False,
+        success_codes: Iterable[int] | None = None,
+        log: bool = True,
+        external: ExternalType | None = None,
+        stdout: int | IO[str] | None = None,
+        stderr: int | IO[str] = subprocess.STDOUT,
+        interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+        terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
     ) -> Any | None:
         """Run a command in the install step.
 
         This is a variant of :meth:`run` that runs even in the presence of
         ``--install-only``. This method returns early if ``--no-install`` is
         specified and the virtualenv is being reused. (In nox 2023.04.22 and
         earlier, this was called ``run_always``, and that continues to be
@@ -456,72 +491,133 @@
         if not args:
             raise ValueError("At least one argument required to run_install().")
 
         return self._run(
             *args,
             env=env,
             include_outer_env=include_outer_env,
-            **kwargs,
+            silent=silent,
+            success_codes=success_codes,
+            log=log,
+            external=external,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
         )
 
     def run_always(
         self,
         *args: str | os.PathLike[str],
-        env: Mapping[str, str] | None = None,
+        env: Mapping[str, str | None] | None = None,
         include_outer_env: bool = True,
-        **kwargs: Any,
+        silent: bool = False,
+        success_codes: Iterable[int] | None = None,
+        log: bool = True,
+        external: ExternalType | None = None,
+        stdout: int | IO[str] | None = None,
+        stderr: int | IO[str] = subprocess.STDOUT,
+        interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+        terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
     ) -> Any | None:
         """This is an alias to ``run_install``, which better describes the use case.
 
         :meta private:
         """
 
         return self.run_install(
-            *args, env=env, include_outer_env=include_outer_env, **kwargs
+            *args,
+            env=env,
+            include_outer_env=include_outer_env,
+            silent=silent,
+            success_codes=success_codes,
+            log=log,
+            external=external,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
         )
 
     def _run(
         self,
         *args: str | os.PathLike[str],
-        env: Mapping[str, str] | None = None,
-        include_outer_env: bool = True,
-        **kwargs: Any,
+        env: Mapping[str, str | None] | None = None,
+        include_outer_env: bool,
+        silent: bool,
+        success_codes: Iterable[int] | None,
+        log: bool,
+        external: ExternalType | None,
+        stdout: int | IO[str] | None,
+        stderr: int | IO[str],
+        interrupt_timeout: float | None,
+        terminate_timeout: float | None,
     ) -> Any:
         """Like run(), except that it runs even if --install-only is provided."""
         # Legacy support - run a function given.
         if callable(args[0]):
-            return self._run_func(args[0], args[1:], kwargs)  # type: ignore[unreachable]
+            return self._run_func(args[0], args[1:])  # type: ignore[unreachable]
+
+        # Using `"uv"` when `uv` is the backend is guaranteed to work, even if it was co-installed with nox.
+        if (
+            self.virtualenv.venv_backend == "uv"
+            and args[0] == "uv"
+            and nox.virtualenv.UV != "uv"
+            and shutil.which("uv", path=self.bin) is None  # Session uv takes priority
+        ):
+            args = (nox.virtualenv.UV, *args[1:])
 
         # Combine the env argument with our virtualenv's env vars.
         if include_outer_env:
-            overlay_env = env
-            env = self.env.copy()
-            if overlay_env is not None:
-                env.update(overlay_env)
+            overlay_env = env or {}
+            env = {**self.env, **overlay_env}
 
         # If --error-on-external-run is specified, error on external programs.
-        if self._runner.global_config.error_on_external_run:
-            kwargs.setdefault("external", "error")
+        if self._runner.global_config.error_on_external_run and external is None:
+            external = "error"
 
         # Allow all external programs when running outside a sandbox.
-        if not self.virtualenv.is_sandboxed:
-            kwargs["external"] = True
+        if (
+            not self.virtualenv.is_sandboxed
+            or args[0] in self.virtualenv.allowed_globals
+        ):
+            external = True
 
-        if args[0] in self.virtualenv.allowed_globals:
-            kwargs["external"] = True
+        if external is None:
+            external = False
 
         # Run a shell command.
-        return nox.command.run(args, env=env, paths=self.bin_paths, **kwargs)
+        return nox.command.run(
+            args,
+            env=env,
+            paths=self.bin_paths,
+            silent=silent,
+            success_codes=success_codes,
+            log=log,
+            external=external,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
+        )
 
     def conda_install(
         self,
         *args: str,
         auto_offline: bool = True,
         channel: str | Sequence[str] = "",
-        **kwargs: Any,
+        env: Mapping[str, str] | None = None,
+        include_outer_env: bool = True,
+        silent: bool | None = None,
+        success_codes: Iterable[int] | None = None,
+        log: bool = True,
+        stdout: int | IO[str] | None = None,
+        stderr: int | IO[str] = subprocess.STDOUT,
+        interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+        terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
     ) -> None:
         """Install invokes `conda install`_ to install packages inside of the
         session's environment.
 
         To install packages directly::
 
             session.conda_install('pandas')
@@ -542,42 +638,46 @@
 
             session.install('.', '--no-deps')
             # Install in editable mode.
             session.install('-e', '.', '--no-deps')
 
         You can specify a conda channel using `channel=`; a falsey value will
         not change the current channels. You can specify a list of channels if
-        needed.
+        needed. It is highly recommended to specify this; micromamba does not
+        set default channels, and default channels vary for conda. Note that
+        "defaults" is also not permissivly licenced like "conda-forge" is.
 
         Additional keyword args are the same as for :meth:`run`.
 
         .. _conda install:
         """
         venv = self._runner.venv
 
         prefix_args: tuple[str, ...] = ()
         if isinstance(venv, CondaEnv):
             prefix_args = ("--prefix", venv.location)
-        elif not isinstance(venv, PassthroughEnv):  # pragma: no cover
+        elif not isinstance(venv, PassthroughEnv):
             raise ValueError(
                 "A session without a conda environment can not install dependencies"
                 " from conda."
             )
 
         if not args:
             raise ValueError("At least one argument required to install().")
 
-        if self._runner.global_config.no_install and venv._reused:
+        if self._runner.global_config.no_install and (
+            isinstance(venv, PassthroughEnv) or venv._reused
+        ):
             return
 
         # Escape args that should be (conda-specific; pip install does not need this)
         args = _dblquote_pkg_install_args(args)
 
-        if "silent" not in kwargs:
-            kwargs["silent"] = True
+        if silent is None:
+            silent = True
 
         extraopts: list[str] = []
         if auto_offline and venv.is_offline():
             logger.warning(
                 "Automatically setting the `--offline` flag as conda repo seems"
                 " unreachable."
             )
@@ -592,19 +692,40 @@
         self._run(
             venv.conda_cmd,
             "install",
             "--yes",
             *extraopts,
             *prefix_args,
             *args,
+            env=env,
+            include_outer_env=include_outer_env,
+            silent=silent,
+            success_codes=success_codes,
+            log=log,
             external="error",
-            **kwargs,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
         )
 
-    def install(self, *args: str, **kwargs: Any) -> None:
+    def install(
+        self,
+        *args: str,
+        env: Mapping[str, str] | None = None,
+        include_outer_env: bool = True,
+        silent: bool | None = None,
+        success_codes: Iterable[int] | None = None,
+        log: bool = True,
+        external: ExternalType | None = None,
+        stdout: int | IO[str] | None = None,
+        stderr: int | IO[str] = subprocess.STDOUT,
+        interrupt_timeout: float | None = DEFAULT_INTERRUPT_TIMEOUT,
+        terminate_timeout: float | None = DEFAULT_TERMINATE_TIMEOUT,
+    ) -> None:
         """Install invokes `pip`_ to install packages inside of the session's
         virtualenv.
 
         To install packages directly::
 
             session.install('pytest')
             session.install('requests', 'mock')
@@ -636,35 +757,49 @@
         if not isinstance(
             venv, (CondaEnv, VirtualEnv, PassthroughEnv)
         ):  # pragma: no cover
             raise ValueError(
                 "A session without a virtualenv can not install dependencies."
             )
         if isinstance(venv, PassthroughEnv):
+            if self._runner.global_config.no_install:
+                return
             raise ValueError(
                 f"Session {self.name} does not have a virtual environment, so use of"
                 " session.install() is no longer allowed since it would modify the"
                 " global Python environment. If you're really sure that is what you"
                 ' want to do, use session.run("pip", "install", ...) instead.'
             )
         if not args:
             raise ValueError("At least one argument required to install().")
 
         if self._runner.global_config.no_install and venv._reused:
             return
 
-        if "silent" not in kwargs:
-            kwargs["silent"] = True
+        if silent is None:
+            silent = True
 
         if isinstance(venv, VirtualEnv) and venv.venv_backend == "uv":
-            self._run("uv", "pip", "install", *args, external="error", **kwargs)
+            cmd = ["uv", "pip", "install"]
         else:
-            self._run(
-                "python", "-m", "pip", "install", *args, external="error", **kwargs
-            )
+            cmd = ["python", "-m", "pip", "install"]
+        self._run(
+            *cmd,
+            *args,
+            env=env,
+            include_outer_env=include_outer_env,
+            external="error",
+            silent=silent,
+            success_codes=success_codes,
+            log=log,
+            stdout=stdout,
+            stderr=stderr,
+            interrupt_timeout=interrupt_timeout,
+            terminate_timeout=terminate_timeout,
+        )
 
     def notify(
         self,
         target: str | SessionRunner,
         posargs: Iterable[str] | None = None,
     ) -> None:
         """Place the given session at the end of the queue.
```

### Comparing `nox-2024.3.2/nox/tasks.py` & `nox-2024.4.15/nox/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,17 @@
         logger.error(f"No sessions found in {global_config.noxfile}.")
         return 3
 
     # Filter by the name of any explicit sessions.
     # This can raise KeyError if a specified session does not exist;
     # log this if it happens. The sessions does not come from the Noxfile
     # if keywords is not empty.
-    if global_config.sessions is not None:
+    if global_config.sessions is None:
+        manifest.filter_by_default()
+    else:
         try:
             manifest.filter_by_name(global_config.sessions)
         except KeyError as exc:
             logger.error("Error while collecting sessions.")
             logger.error(exc.args[0])
             return 3
```

### Comparing `nox-2024.3.2/nox/tox4_to_nox.jinja2` & `nox-2024.4.15/nox/tox4_to_nox.jinja2`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/tox_to_nox.jinja2` & `nox-2024.4.15/nox/tox_to_nox.jinja2`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/tox_to_nox.py` & `nox-2024.4.15/nox/tox_to_nox.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/nox/virtualenv.py` & `nox-2024.4.15/nox/virtualenv.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,58 @@
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
 from collections.abc import Callable, Mapping
+from pathlib import Path
 from socket import gethostbyname
 from typing import Any, ClassVar
 
 import nox
 import nox.command
 from nox.logger import logger
 
 # Problematic environment variables that are stripped from all commands inside
 # of a virtualenv. See https://github.com/theacodes/nox/issues/44
 _BLACKLISTED_ENV_VARS = frozenset(
-    ["PIP_RESPECT_VIRTUALENV", "PIP_REQUIRE_VIRTUALENV", "__PYVENV_LAUNCHER__"]
+    [
+        "PIP_RESPECT_VIRTUALENV",
+        "PIP_REQUIRE_VIRTUALENV",
+        "__PYVENV_LAUNCHER__",
+        "UV_SYSTEM_PYTHON",
+    ]
 )
 _SYSTEM = platform.system()
 
 
+def find_uv() -> tuple[bool, str]:
+    uv_on_path = shutil.which("uv")
+
+    # Look for uv in Nox's environment, to handle `pipx install nox[uv]`.
+    with contextlib.suppress(ImportError, FileNotFoundError):
+        from uv import find_uv_bin
+
+        uv_bin = find_uv_bin()
+
+        # If the returned value is the same as calling "uv" already, don't
+        # expand (simpler logging)
+        if uv_on_path and Path(uv_bin).samefile(uv_on_path):
+            return True, "uv"
+
+        return True, uv_bin
+
+    # Fall back to PATH.
+    return uv_on_path is not None, "uv"
+
+
+HAS_UV, UV = find_uv()
+
+
 class InterpreterNotFound(OSError):
     def __init__(self, interpreter: str) -> None:
         super().__init__(f"Python interpreter {interpreter} not found")
         self.interpreter = interpreter
 
 
 class ProcessEnv(abc.ABC):
@@ -53,22 +82,24 @@
     # Does this environment provide any process isolation?
     is_sandboxed = False
 
     # Special programs that aren't included in the environment.
     allowed_globals: ClassVar[tuple[Any, ...]] = ()
 
     def __init__(
-        self, bin_paths: None = None, env: Mapping[str, str] | None = None
+        self, bin_paths: None = None, env: Mapping[str, str | None] | None = None
     ) -> None:
         self._bin_paths = bin_paths
-        self.env = os.environ.copy()
         self._reused = False
 
-        if env is not None:
-            self.env.update(env)
+        # Filter envs now so `.env` is dict[str, str] (easier to use)
+        # even though .command's env supports None.
+        env = env or {}
+        env = {**os.environ, **env}
+        self.env = {k: v for k, v in env.items() if v is not None}
 
         for key in _BLACKLISTED_ENV_VARS:
             self.env.pop(key, None)
 
         if self.bin_paths:
             self.env["PATH"] = os.pathsep.join(
                 [*self.bin_paths, self.env.get("PATH", "")]
@@ -89,14 +120,21 @@
     @abc.abstractmethod
     def create(self) -> bool:
         """Create a new environment.
 
         Returns True if the environment is new, and False if it was reused.
         """
 
+    @property
+    @abc.abstractmethod
+    def venv_backend(self) -> str:
+        """
+        Returns the string used to select this environment.
+        """
+
 
 def locate_via_py(version: str) -> str | None:
     """Find the Python executable using the Windows Launcher.
 
     This is based on :pep:397 which details that executing
     ``py.exe -{version}`` should execute Python with the requested
     version. We then make the Python process print out its full
@@ -176,14 +214,18 @@
         return CondaEnv.is_offline()  # pragma: no cover
 
     def create(self) -> bool:
         """Does nothing, since this is an existing environment. Always returns
         False since it's always reused."""
         return False
 
+    @property
+    def venv_backend(self) -> str:
+        return "none"
+
 
 class CondaEnv(ProcessEnv):
     """Conda environment management class.
 
     Args:
         location (str): The location on the filesystem where the conda environment
             should be created.
@@ -199,15 +241,15 @@
             If not specified, this will use the currently running Python.
         reuse_existing (Optional[bool]): Flag indicating if the conda environment
             should be reused if it already exists at ``location``.
         conda_cmd (str): The name of the command, can be "conda" (default) or "mamba".
     """
 
     is_sandboxed = True
-    allowed_globals = ("conda", "mamba")
+    allowed_globals = ("conda", "mamba", "micromamba")
 
     def __init__(
         self,
         location: str,
         interpreter: str | None = None,
         reuse_existing: bool = False,
         venv_params: Any = None,
@@ -216,15 +258,15 @@
     ):
         self.location_name = location
         self.location = os.path.abspath(location)
         self.interpreter = interpreter
         self.reuse_existing = reuse_existing
         self.venv_params = venv_params or []
         self.conda_cmd = conda_cmd
-        super().__init__(env={"CONDA_PREFIX": self.location})
+        super().__init__(env={"CONDA_PREFIX": self.location, "VIRTUAL_ENV": None})
 
     def _clean_location(self) -> bool:
         """Deletes existing conda environment"""
         is_conda = os.path.isdir(os.path.join(self.location, "conda-meta"))
         if os.path.exists(self.location):
             if self.reuse_existing and is_conda:
                 return False
@@ -268,24 +310,32 @@
             logger.debug(f"Re-using existing conda env at {self.location_name}.")
 
             self._reused = True
 
             return False
 
         cmd = [self.conda_cmd, "create", "--yes", "--prefix", self.location]
+        if self.conda_cmd == "micromamba" and not any(
+            v.startswith(("--channel=", "-c")) or v == "--channel"
+            for v in self.venv_params
+        ):
+            # Micromamba doesn't have any default channels
+            cmd.append("--channel=conda-forge")
 
         cmd.extend(self.venv_params)
 
         # Ensure the pip package is installed.
         cmd.append("pip")
 
         python_dep = f"python={self.interpreter}" if self.interpreter else "python"
         cmd.append(python_dep)
 
-        logger.info(f"Creating conda env in {self.location_name} with {python_dep}")
+        logger.info(
+            f"Creating {self.conda_cmd} env in {self.location_name} with {python_dep}"
+        )
         nox.command.run(cmd, silent=True, log=nox.options.verbose or False)
 
         return True
 
     @staticmethod
     def is_offline() -> bool:
         """Return `True` if we are sure that the user is not able to connect to https://repo.anaconda.com.
@@ -299,14 +349,18 @@
         try:
             # DNS resolution to detect situation (1) or (2).
             host = gethostbyname("repo.anaconda.com")
             return host is None
         except BaseException:  # pragma: no cover
             return True
 
+    @property
+    def venv_backend(self) -> str:
+        return self.conda_cmd
+
 
 class VirtualEnv(ProcessEnv):
     """Virtualenv management class.
 
     Args:
         location (str): The location on the filesystem where the virtual environment
             should be created.
@@ -321,15 +375,15 @@
 
             If not specified, this will use the currently running Python.
         reuse_existing (Optional[bool]): Flag indicating if the virtual environment
             should be reused if it already exists at ``location``.
     """
 
     is_sandboxed = True
-    allowed_globals = ("uv",)
+    allowed_globals = (UV,)
 
     def __init__(
         self,
         location: str,
         interpreter: str | None = None,
         reuse_existing: bool = False,
         *,
@@ -337,20 +391,20 @@
         venv_params: Any = None,
     ):
         self.location_name = location
         self.location = os.path.abspath(location)
         self.interpreter = interpreter
         self._resolved: None | str | InterpreterNotFound = None
         self.reuse_existing = reuse_existing
-        self.venv_backend = venv_backend
+        self._venv_backend = venv_backend
         self.venv_params = venv_params or []
         if venv_backend not in {"virtualenv", "venv", "uv"}:
             msg = f"venv_backend {venv_backend} not recognized"
             raise ValueError(msg)
-        super().__init__(env={"VIRTUAL_ENV": self.location})
+        super().__init__(env={"VIRTUAL_ENV": self.location, "CONDA_PREFIX": None})
 
     def _clean_location(self) -> bool:
         """Deletes any existing virtual environment"""
         if os.path.exists(self.location):
             if (
                 self.reuse_existing
                 and self._check_reused_environment_type()
@@ -520,15 +574,15 @@
 
         if self.venv_backend == "virtualenv":
             cmd = [sys.executable, "-m", "virtualenv", self.location]
             if self.interpreter:
                 cmd.extend(["-p", self._resolved_interpreter])
         elif self.venv_backend == "uv":
             cmd = [
-                "uv",
+                UV,
                 "venv",
                 "-p",
                 self._resolved_interpreter if self.interpreter else sys.executable,
                 self.location,
             ]
         else:
             cmd = [self._resolved_interpreter, "-m", "venv", self.location]
@@ -540,25 +594,31 @@
             f"Creating virtual environment ({self.venv_backend}) using"
             f" {resolved_interpreter_name} in {self.location_name}"
         )
         nox.command.run(cmd, silent=True, log=nox.options.verbose or False)
 
         return True
 
+    @property
+    def venv_backend(self) -> str:
+        return self._venv_backend
+
 
 ALL_VENVS: dict[str, Callable[..., ProcessEnv]] = {
     "conda": functools.partial(CondaEnv, conda_cmd="conda"),
     "mamba": functools.partial(CondaEnv, conda_cmd="mamba"),
+    "micromamba": functools.partial(CondaEnv, conda_cmd="micromamba"),
     "virtualenv": functools.partial(VirtualEnv, venv_backend="virtualenv"),
     "venv": functools.partial(VirtualEnv, venv_backend="venv"),
     "uv": functools.partial(VirtualEnv, venv_backend="uv"),
     "none": PassthroughEnv,
 }
 
 # Any environment in this dict could be missing, and is only available if the
 # value is True. If an environment is always available, it should not be in this
 # dict. "virtualenv" is not considered optional since it's a dependency of nox.
 OPTIONAL_VENVS = {
     "conda": shutil.which("conda") is not None,
     "mamba": shutil.which("mamba") is not None,
-    "uv": shutil.which("uv") is not None,
+    "micromamba": shutil.which("micromamba") is not None,
+    "uv": HAS_UV,
 }
```

### Comparing `nox-2024.3.2/nox/workflow.py` & `nox-2024.4.15/nox/workflow.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/conftest.py` & `nox-2024.4.15/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test__option_set.py` & `nox-2024.4.15/tests/test__option_set.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test__parametrize.py` & `nox-2024.4.15/tests/test__parametrize.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test__version.py` & `nox-2024.4.15/tests/test__version.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_action_helper.py` & `nox-2024.4.15/tests/test_action_helper.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_command.py` & `nox-2024.4.15/tests/test_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,27 @@
         silent=True,
         env={"SIGIL": "123"},
     )
 
     assert "123" in result
 
 
+def test_run_env_remove(monkeypatch):
+    monkeypatch.setenv("EMPTY", "notempty")
+    nox.command.run(
+        [PYTHON, "-c", 'import os; assert "EMPTY" in os.environ'],
+        silent=True,
+    )
+    nox.command.run(
+        [PYTHON, "-c", 'import os; assert "EMPTY" not in os.environ'],
+        silent=True,
+        env={"EMPTY": None},
+    )
+
+
 @mock.patch("sys.platform", "win32")
 def test_run_env_systemroot():
     systemroot = os.environ.setdefault("SYSTEMROOT", "sigil")
 
     result = nox.command.run(
         [PYTHON, "-c", 'import os; print(os.environ["SYSTEMROOT"])'], silent=True
     )
@@ -178,15 +191,23 @@
     executable = tmp_path.joinpath(executable_name)
     executable.touch()
     executable.chmod(0o700)
 
     with mock.patch("nox.command.popen") as mock_command:
         mock_command.return_value = (0, "")
         nox.command.run([executable_name], silent=True, paths=[str(tmp_path)])
-        mock_command.assert_called_with([str(executable)], env=mock.ANY, silent=True)
+        mock_command.assert_called_with(
+            [str(executable)],
+            env=None,
+            silent=True,
+            stdout=None,
+            stderr=subprocess.STDOUT,
+            interrupt_timeout=0.3,
+            terminate_timeout=0.2,
+        )
 
 
 def test_run_external_warns(tmpdir, caplog):
     caplog.set_level(logging.WARNING)
 
     nox.command.run([PYTHON, "--version"], silent=True, paths=[tmpdir.strpath])
```

### Comparing `nox-2024.3.2/tests/test_logger.py` & `nox-2024.4.15/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_main.py` & `nox-2024.4.15/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_manifest.py` & `nox-2024.4.15/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_registry.py` & `nox-2024.4.15/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_sessions.py` & `nox-2024.4.15/tests/test_sessions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,67 @@
 
 from __future__ import annotations
 
 import argparse
 import logging
 import operator
 import os
+import shutil
+import subprocess
 import sys
 import tempfile
 from pathlib import Path
 from unittest import mock
 
 import pytest
 
 import nox.command
 import nox.manifest
+import nox.popen
 import nox.registry
 import nox.sessions
 import nox.virtualenv
 from nox import _options
 from nox.logger import logger
 
+HAS_CONDA = shutil.which("conda") is not None
+has_conda = pytest.mark.skipif(not HAS_CONDA, reason="Missing conda command.")
+
+
+def run_with_defaults(**kwargs):
+    return {
+        "env": None,
+        "silent": False,
+        "paths": None,
+        "success_codes": None,
+        "log": True,
+        "external": False,
+        "stdout": None,
+        "stderr": subprocess.STDOUT,
+        "interrupt_timeout": nox.popen.DEFAULT_INTERRUPT_TIMEOUT,
+        "terminate_timeout": nox.popen.DEFAULT_TERMINATE_TIMEOUT,
+        **kwargs,
+    }
+
+
+def _run_with_defaults(**kwargs):
+    return {
+        "env": None,
+        "include_outer_env": True,
+        "silent": False,
+        "success_codes": None,
+        "log": True,
+        "external": False,
+        "stdout": None,
+        "stderr": subprocess.STDOUT,
+        "interrupt_timeout": nox.popen.DEFAULT_INTERRUPT_TIMEOUT,
+        "terminate_timeout": nox.popen.DEFAULT_TERMINATE_TIMEOUT,
+        **kwargs,
+    }
+
 
 def test__normalize_path():
     envdir = "envdir"
     normalize = nox.sessions._normalize_path
     assert normalize(envdir, "hello") == os.path.join("envdir", "hello")
     assert normalize(envdir, b"hello") == os.path.join("envdir", "hello")
     assert normalize(envdir, "hello(world)") == os.path.join("envdir", "hello-world")
@@ -131,14 +169,16 @@
         session, runner = self.make_session_and_runner()
 
         runner.venv = None
 
         with pytest.raises(ValueError, match="virtualenv"):
             _ = session.virtualenv
 
+        assert session.venv_backend == "none"
+
     def test_interactive(self):
         session, runner = self.make_session_and_runner()
 
         with mock.patch("nox.sessions.sys.stdin.isatty") as m_isatty:
             m_isatty.return_value = True
 
             assert session.interactive is True
@@ -240,18 +280,15 @@
 
         with mock.patch.object(nox.command, "run") as run:
             session.install("spam")
             session.run("spam", "eggs")
 
         run.assert_called_once_with(
             ("python", "-m", "pip", "install", "spam"),
-            env=mock.ANY,
-            external=mock.ANY,
-            paths=mock.ANY,
-            silent=mock.ANY,
+            **run_with_defaults(paths=mock.ANY, silent=True, env={}, external="error"),
         )
 
     def test_run_success(self):
         session, _ = self.make_session_and_runner()
         result = session.run(sys.executable, "-c", "print(123)")
         assert result
 
@@ -261,22 +298,23 @@
         with pytest.raises(nox.command.CommandFailed):
             session.run(sys.executable, "-c", "import sys; sys.exit(1)")
 
     def test_run_overly_env(self):
         session, runner = self.make_session_and_runner()
         runner.venv.env["A"] = "1"
         runner.venv.env["B"] = "2"
+        runner.venv.env["C"] = "4"
         result = session.run(
             sys.executable,
             "-c",
-            'import os; print(os.environ["A"], os.environ["B"])',
-            env={"B": "3"},
+            'import os; print(os.environ["A"], os.environ["B"], os.environ.get("C", "5"))',
+            env={"B": "3", "C": None},
             silent=True,
         )
-        assert result.strip() == "1 3"
+        assert result.strip() == "1 3 5"
 
     def test_by_default_all_invocation_env_vars_are_passed(self):
         session, runner = self.make_session_and_runner()
         runner.venv.env["I_SHOULD_BE_INCLUDED"] = "happy"
         runner.venv.env["I_SHOULD_BE_INCLUDED_TOO"] = "happier"
         runner.venv.env["EVERYONE_SHOULD_BE_INCLUDED_TOO"] = "happiest"
         result = session.run(
@@ -312,17 +350,15 @@
         runner.venv = nox.virtualenv.PassthroughEnv()
 
         with mock.patch("nox.command.run", autospec=True) as run:
             session.run(sys.executable, "--version")
 
         run.assert_called_once_with(
             (sys.executable, "--version"),
-            external=True,
-            env=mock.ANY,
-            paths=None,
+            **run_with_defaults(external=True, env=mock.ANY),
         )
 
     def test_run_external_condaenv(self):
         # condaenv sessions should always allow conda.
         session, runner = self.make_session_and_runner()
         runner.venv = mock.create_autospec(nox.virtualenv.CondaEnv)
         runner.venv.allowed_globals = ("conda",)
@@ -331,17 +367,17 @@
         runner.venv.create.return_value = True
 
         with mock.patch("nox.command.run", autospec=True) as run:
             session.run("conda", "--version")
 
         run.assert_called_once_with(
             ("conda", "--version"),
-            external=True,
-            env=mock.ANY,
-            paths=["/path/to/env/bin"],
+            **run_with_defaults(
+                external=True, env=mock.ANY, paths=["/path/to/env/bin"]
+            ),
         )
 
     def test_run_external_with_error_on_external_run(self):
         session, runner = self.make_session_and_runner()
 
         runner.global_config.error_on_external_run = True
 
@@ -364,14 +400,28 @@
 
         with pytest.raises(ValueError) as exc_info:
             session.run_install()
 
         exc_args = exc_info.value.args
         assert exc_args == ("At least one argument required to run_install().",)
 
+    def test_run_no_install_passthrough(self):
+        session, runner = self.make_session_and_runner()
+        runner.venv = nox.virtualenv.PassthroughEnv()
+        runner.global_config.no_install = True
+
+        session.install("numpy")
+        session.conda_install("numpy")
+
+    def test_run_no_conda_install(self):
+        session, runner = self.make_session_and_runner()
+
+        with pytest.raises(ValueError, match="A session without a conda"):
+            session.conda_install("numpy")
+
     def test_run_install_success(self):
         session, _ = self.make_session_and_runner()
 
         assert session.run_install(operator.add, 1300, 37) == 1337
 
     def test_run_install_install_only(self, caplog):
         session, runner = self.make_session_and_runner()
@@ -527,16 +577,15 @@
                 "install",
                 "--yes",
                 *args,
                 "--prefix",
                 "/path/to/conda/env",
                 "requests",
                 "urllib3",
-                silent=True,
-                external="error",
+                **_run_with_defaults(silent=True, external="error"),
             )
 
     @pytest.mark.parametrize(
         ("no_install", "reused", "run_called"),
         [
             (True, True, False),
             (True, False, True),
@@ -602,16 +651,15 @@
                 "install",
                 "--yes",
                 "--prefix",
                 "/path/to/conda/env",
                 "requests",
                 # this will be double quoted if unquoted constraint is present
                 passed_arg,
-                silent=False,
-                external="error",
+                **_run_with_defaults(silent=False, external="error"),
             )
 
     def test_install_bad_args_no_arg(self):
         session, _ = self.make_session_and_runner()
 
         with pytest.raises(ValueError, match="arg"):
             session.install()
@@ -637,25 +685,26 @@
         runner.venv.venv_backend = "venv"
 
         class SessionNoSlots(nox.sessions.Session):
             pass
 
         session = SessionNoSlots(runner=runner)
 
+        assert session.venv_backend == "venv"
+
         with mock.patch.object(session, "_run", autospec=True) as run:
             session.install("requests", "urllib3")
             run.assert_called_once_with(
                 "python",
                 "-m",
                 "pip",
                 "install",
                 "requests",
                 "urllib3",
-                silent=True,
-                external="error",
+                **_run_with_defaults(silent=True, external="error"),
             )
 
     def test_install_non_default_kwargs(self):
         runner = nox.sessions.SessionRunner(
             name="test",
             signatures=["test"],
             func=mock.sentinel.func,
@@ -676,16 +725,15 @@
             run.assert_called_once_with(
                 "python",
                 "-m",
                 "pip",
                 "install",
                 "requests",
                 "urllib3",
-                silent=False,
-                external="error",
+                **_run_with_defaults(silent=False, external="error"),
             )
 
     def test_install_no_venv_failure(self):
         runner = nox.sessions.SessionRunner(
             name="test",
             signatures=["test"],
             func=mock.sentinel.func,
@@ -822,16 +870,66 @@
             session.install("requests", "urllib3", silent=False)
             run.assert_called_once_with(
                 "uv",
                 "pip",
                 "install",
                 "requests",
                 "urllib3",
-                silent=False,
-                external="error",
+                **_run_with_defaults(silent=False, external="error"),
+            )
+
+    def test_install_uv_command(self, monkeypatch):
+        runner = nox.sessions.SessionRunner(
+            name="test",
+            signatures=["test"],
+            func=mock.sentinel.func,
+            global_config=_options.options.namespace(posargs=[]),
+            manifest=mock.create_autospec(nox.manifest.Manifest),
+        )
+        runner.venv = mock.create_autospec(nox.virtualenv.VirtualEnv)
+        runner.venv.env = {}
+        runner.venv.venv_backend = "uv"
+
+        class SessionNoSlots(nox.sessions.Session):
+            pass
+
+        session = SessionNoSlots(runner=runner)
+
+        monkeypatch.setattr(nox.virtualenv, "UV", "/some/uv")
+        monkeypatch.setattr(shutil, "which", lambda x, path=None: None)
+
+        with mock.patch.object(nox.command, "run", autospec=True) as run:
+            session.install("requests", "urllib3", silent=False)
+            run.assert_called_once()
+
+            ((call_args,), _) = run.call_args
+            assert call_args == (
+                "/some/uv",
+                "pip",
+                "install",
+                "requests",
+                "urllib3",
+            )
+
+        # user installs uv in the session venv
+        monkeypatch.setattr(
+            shutil, "which", lambda x, path="": path + "/uv" if x == "uv" else None
+        )
+
+        with mock.patch.object(nox.command, "run", autospec=True) as run:
+            session.install("requests", "urllib3", silent=False)
+            run.assert_called_once()
+
+            ((call_args,), _) = run.call_args
+            assert call_args == (
+                "uv",
+                "pip",
+                "install",
+                "requests",
+                "urllib3",
             )
 
     def test___slots__(self):
         session, _ = self.make_session_and_runner()
         with pytest.raises(AttributeError):
             session.foo = "bar"
         with pytest.raises(AttributeError):
@@ -942,15 +1040,20 @@
             ("nox.virtualenv.VirtualEnv.create", None, nox.virtualenv.VirtualEnv),
             (
                 "nox.virtualenv.VirtualEnv.create",
                 "virtualenv",
                 nox.virtualenv.VirtualEnv,
             ),
             ("nox.virtualenv.VirtualEnv.create", "venv", nox.virtualenv.VirtualEnv),
-            ("nox.virtualenv.CondaEnv.create", "conda", nox.virtualenv.CondaEnv),
+            pytest.param(
+                "nox.virtualenv.CondaEnv.create",
+                "conda",
+                nox.virtualenv.CondaEnv,
+                marks=has_conda,
+            ),
         ],
     )
     def test__create_venv_options(self, create_method, venv_backend, expected_backend):
         runner = self.make_runner()
         runner.func.python = "coolpython"
         runner.func.reuse_venv = True
         runner.func.venv_backend = venv_backend
```

### Comparing `nox-2024.3.2/tests/test_tasks.py` & `nox-2024.4.15/tests/test_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,24 @@
     pass
 
 
 session_func.python = None
 session_func.venv_backend = None
 session_func.should_warn = {}
 session_func.tags = []
+session_func.default = True
 
 
 def session_func_with_python():
     pass
 
 
 session_func_with_python.python = "3.8"
 session_func_with_python.venv_backend = None
+session_func_with_python.default = True
 
 
 def session_func_venv_pythons_warning():
     pass
 
 
 session_func_venv_pythons_warning.python = ["3.7"]
@@ -342,14 +344,48 @@
     tasks.merge_noxfile_options(nox_module, config)
     manifest = Manifest({"test": test, "bar": bar}, config)
     return_value = tasks.filter_manifest(manifest, config)
     assert return_value is manifest
     assert len(manifest) == 2
 
 
+@pytest.mark.parametrize("selection", [None, ["qux"], ["quuz"], ["qux", "quuz"]])
+def test_default_false(selection):
+    @nox.session()
+    def qux():
+        pass
+
+    @nox.session()
+    def quux():
+        pass
+
+    @nox.session(default=False)
+    def quuz():
+        pass
+
+    @nox.session(default=False)
+    def corge():
+        pass
+
+    config = _options.options.namespace(sessions=selection, pythons=(), posargs=[])
+    manifest = Manifest(
+        {
+            "qux": qux,
+            "quux": quux,
+            "quuz": quuz,
+            "corge": corge,
+        },
+        config,
+    )
+    return_value = tasks.filter_manifest(manifest, config)
+    assert return_value is manifest
+    expected = 2 if selection is None else len(selection)
+    assert len(manifest) == expected
+
+
 def test_honor_list_request_noop():
     config = _options.options.namespace(list_sessions=False)
     manifest = {"thing": mock.sentinel.THING}
     return_value = tasks.honor_list_request(manifest, global_config=config)
     assert return_value is manifest
```

### Comparing `nox-2024.3.2/tests/test_tox_to_nox.py` & `nox-2024.4.15/tests/test_tox_to_nox.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/test_virtualenv.py` & `nox-2024.4.15/tests/test_virtualenv.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+import functools
 import os
 import re
 import shutil
 import subprocess
 import sys
+import types
+from pathlib import Path
 from textwrap import dedent
 from typing import NamedTuple
 from unittest import mock
 
 import pytest
 from packaging import version
 
@@ -48,22 +51,21 @@
     returncode: int = 0
 
 
 @pytest.fixture
 def make_one(tmpdir):
     def factory(*args, venv_backend: str = "virtualenv", **kwargs):
         location = tmpdir.join("venv")
-        if venv_backend in {"mamba", "conda"}:
-            venv = nox.virtualenv.CondaEnv(
-                location.strpath, *args, conda_cmd=venv_backend, **kwargs
-            )
-        else:
-            venv = nox.virtualenv.VirtualEnv(
-                location.strpath, *args, venv_backend=venv_backend, **kwargs
+        try:
+            venv_fn = nox.virtualenv.ALL_VENVS[venv_backend]
+        except KeyError:
+            venv_fn = functools.partial(
+                nox.virtualenv.VirtualEnv, venv_backend=venv_backend
             )
+        venv = venv_fn(location.strpath, *args, **kwargs)
         return (venv, location)
 
     return factory
 
 
 @pytest.fixture
 def make_conda(tmpdir):
@@ -359,17 +361,23 @@
     venv, dir_ = make_one()
     assert len(venv.bin_paths) == 1
     assert venv.bin_paths[0] == venv.bin
     assert dir_.join("Scripts").strpath == venv.bin
 
 
 def test_create(monkeypatch, make_one):
+    monkeypatch.setenv("CONDA_PREFIX", "no-prefix-allowed")
+    monkeypatch.setenv("NOT_CONDA_PREFIX", "something-else")
+
     venv, dir_ = make_one()
     venv.create()
 
+    assert "CONDA_PREFIX" not in venv.env
+    assert "NOT_CONDA_PREFIX" in venv.env
+
     if IS_WINDOWS:
         assert dir_.join("Scripts", "python.exe").check()
         assert dir_.join("Scripts", "pip.exe").check()
         assert dir_.join("Lib").check()
     else:
         assert dir_.join("bin", "python").check()
         assert dir_.join("bin", "pip").check()
@@ -472,35 +480,88 @@
 
     venv, _ = make_one(reuse_existing=True, venv_backend="conda")
     reused = not venv.create()
 
     assert reused
 
 
+# This mocks micromamba so that it doesn't need to be installed.
+@has_conda
+def test_micromamba_environment(make_one, monkeypatch):
+    conda_path = shutil.which("conda")
+    which = shutil.which
+    monkeypatch.setattr(
+        shutil, "which", lambda x: conda_path if x == "micromamba" else which(x)
+    )
+    venv, _ = make_one(reuse_existing=True, venv_backend="micromamba")
+    run = mock.Mock()
+    monkeypatch.setattr(nox.command, "run", run)
+    venv.create()
+    run.assert_called_once()
+    # .args requires Python 3.8+
+    ((args,), _) = run.call_args
+    assert args[0] == "micromamba"
+    assert "--channel=conda-forge" in args
+
+
+# This mocks micromamba so that it doesn't need to be installed.
+@pytest.mark.parametrize(
+    "params",
+    [["--channel=default"], ["-cdefault"], ["-c", "default"], ["--channel", "default"]],
+)
+@has_conda
+def test_micromamba_channel_environment(make_one, monkeypatch, params):
+    conda_path = shutil.which("conda")
+    which = shutil.which
+    monkeypatch.setattr(
+        shutil, "which", lambda x: conda_path if x == "micromamba" else which(x)
+    )
+    venv, _ = make_one(reuse_existing=True, venv_backend="micromamba")
+    run = mock.Mock()
+    monkeypatch.setattr(nox.command, "run", run)
+    venv.venv_params = params
+    venv.create()
+    run.assert_called_once()
+    # .args requires Python 3.8+
+    ((args,), _) = run.call_args
+    assert args[0] == "micromamba"
+    for p in params:
+        assert p in args
+    assert "--channel=conda-forge" not in args
+
+
 @pytest.mark.parametrize(
     ("frm", "to", "result"),
     [
         ("virtualenv", "venv", True),
         ("venv", "virtualenv", True),
         ("virtualenv", "uv", True),
         pytest.param("uv", "virtualenv", False, marks=has_uv),
         pytest.param("conda", "virtualenv", False, marks=has_conda),
     ],
 )
 def test_stale_environment(make_one, frm, to, result, monkeypatch):
     monkeypatch.setenv("NOX_ENABLE_STALENESS_CHECK", "1")
     venv, _ = make_one(reuse_existing=True, venv_backend=frm)
     venv.create()
+    assert venv.venv_backend == frm
 
     venv, _ = make_one(reuse_existing=True, venv_backend=to)
     reused = venv._check_reused_environment_type()
+    assert venv.venv_backend == to
 
     assert reused == result
 
 
+def test_passthrough_environment_venv_backend(make_one):
+    venv, _ = make_one(venv_backend="none")
+    venv.create()
+    assert venv.venv_backend == "none"
+
+
 @has_uv
 def test_create_reuse_stale_virtualenv_environment(make_one, monkeypatch):
     monkeypatch.setenv("NOX_ENABLE_STALENESS_CHECK", "1")
     venv, location = make_one(reuse_existing=True, venv_backend="venv")
     venv.create()
 
     # Drop a uv-style pyvenv.cfg into the environment.
@@ -534,14 +595,41 @@
 
     reused = not venv.create()
 
     # The environment is reused because it looks like a uv environment
     assert reused
 
 
+UV_IN_PIPX_VENV = "/home/user/.local/pipx/venvs/nox/bin/uv"
+
+
+@pytest.mark.parametrize(
+    ["which_result", "find_uv_bin_result", "found", "path"],
+    [
+        ("/usr/bin/uv", UV_IN_PIPX_VENV, True, UV_IN_PIPX_VENV),
+        ("/usr/bin/uv", FileNotFoundError, True, "uv"),
+        (None, UV_IN_PIPX_VENV, True, UV_IN_PIPX_VENV),
+        (None, FileNotFoundError, False, "uv"),
+    ],
+)
+def test_find_uv(monkeypatch, which_result, find_uv_bin_result, found, path):
+    def find_uv_bin():
+        if find_uv_bin_result is FileNotFoundError:
+            raise FileNotFoundError
+        return find_uv_bin_result
+
+    monkeypatch.setattr(shutil, "which", lambda _: which_result)
+    monkeypatch.setattr(Path, "samefile", lambda a, b: a == b)
+    monkeypatch.setitem(
+        sys.modules, "uv", types.SimpleNamespace(find_uv_bin=find_uv_bin)
+    )
+
+    assert nox.virtualenv.find_uv() == (found, path)
+
+
 def test_create_reuse_venv_environment(make_one, monkeypatch):
     # Making the reuse requirement more strict
     monkeypatch.setenv("NOX_ENABLE_STALENESS_CHECK", "1")
 
     venv, location = make_one(reuse_existing=True, venv_backend="venv")
     venv.create()
```

### Comparing `nox-2024.3.2/tests/test_workflow.py` & `nox-2024.4.15/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/resources/noxfile.py` & `nox-2024.4.15/tests/resources/noxfile.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/resources/noxfile_multiple_sessions.py` & `nox-2024.4.15/tests/resources/noxfile_multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/resources/noxfile_nested.py` & `nox-2024.4.15/tests/resources/noxfile_nested.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/resources/noxfile_options.py` & `nox-2024.4.15/tests/resources/noxfile_options.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/resources/noxfile_options_pythons.py` & `nox-2024.4.15/tests/resources/noxfile_options_pythons.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/tests/resources/noxfile_spaces.py` & `nox-2024.4.15/tests/resources/noxfile_spaces.py`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/.gitignore` & `nox-2024.4.15/.gitignore`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/LICENSE` & `nox-2024.4.15/LICENSE`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/README.md` & `nox-2024.4.15/README.md`

 * *Files identical despite different names*

### Comparing `nox-2024.3.2/pyproject.toml` & `nox-2024.4.15/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "hatchling.build"
 requires = [
   "hatchling",
 ]
 
 [project]
 name = "nox"
-version = "2024.03.02"
+version = "2024.04.15"
 description = "Flexible test automation."
 readme = "README.md"
 keywords = [
   "automation",
   "testing",
   "tox",
 ]
@@ -40,24 +40,25 @@
   "Topic :: Software Development :: Testing",
 ]
 dependencies = [
   "argcomplete<4.0,>=1.9.4",
   "colorlog<7.0.0,>=2.6.1",
   'importlib-metadata; python_version < "3.8"',
   "packaging>=20.9",
+  'tomli>=1; python_version < "3.11"',
   'typing-extensions>=3.7.4; python_version < "3.8"',
   "virtualenv>=20.14.1",
 ]
 [project.optional-dependencies]
 tox_to_nox = [
   "jinja2",
   "tox",
 ]
 uv = [
-  "uv",
+  "uv>=0.1.6",
 ]
 [project.urls]
 bug-tracker = "https://github.com/wntrblm/nox/issues"
 documentation = "https://nox.thea.codes"
 homepage = "https://github.com/wntrblm/nox"
 repository = "https://github.com/wntrblm/nox"
 [project.scripts]
@@ -103,15 +104,15 @@
 [tool.coverage.run]
 branch = true
 omit = [ "nox/_typing.py" ]
 relative_files = true
 source_pkgs = [ "nox" ]
 
 [tool.coverage.report]
-exclude_lines = [ "pragma: no cover", "if TYPE_CHECKING:", "@overload" ]
+exclude_also = [ "def __dir__()", "if TYPE_CHECKING:", "@overload" ]
 
 [tool.mypy]
 files = [ "nox/**/*.py", "noxfile.py" ]
 python_version = "3.7"
 strict = true
 warn_unreachable = true
 enable_error_code = [ "ignore-without-code", "redundant-expr", "truthy-bool" ]
```

### Comparing `nox-2024.3.2/PKG-INFO` & `nox-2024.4.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nox
-Version: 2024.3.2
+Version: 2024.4.15
 Summary: Flexible test automation.
 Project-URL: bug-tracker, https://github.com/wntrblm/nox/issues
 Project-URL: documentation, https://nox.thea.codes
 Project-URL: homepage, https://github.com/wntrblm/nox
 Project-URL: repository, https://github.com/wntrblm/nox
 Author: Alethea Katherine Flowers
 Author-email: me@thea.codes
@@ -29,21 +29,22 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.7
 Requires-Dist: argcomplete<4.0,>=1.9.4
 Requires-Dist: colorlog<7.0.0,>=2.6.1
 Requires-Dist: importlib-metadata; python_version < '3.8'
 Requires-Dist: packaging>=20.9
+Requires-Dist: tomli>=1; python_version < '3.11'
 Requires-Dist: typing-extensions>=3.7.4; python_version < '3.8'
 Requires-Dist: virtualenv>=20.14.1
 Provides-Extra: tox_to_nox
 Requires-Dist: jinja2; extra == 'tox_to_nox'
 Requires-Dist: tox; extra == 'tox_to_nox'
 Provides-Extra: uv
-Requires-Dist: uv; extra == 'uv'
+Requires-Dist: uv>=0.1.6; extra == 'uv'
 Description-Content-Type: text/markdown
 
 <p align="center">
 <img src="https://github.com/wntrblm/nox/raw/main/docs/_static/alice.png" alt="logo" width=50%>
 </p>
 
 # Nox
```

