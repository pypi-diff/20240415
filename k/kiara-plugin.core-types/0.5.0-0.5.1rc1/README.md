# Comparing `tmp/kiara_plugin.core_types-0.5.0.tar.gz` & `tmp/kiara_plugin_core_types-0.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.core_types-0.5.0.tar", last modified: Wed Nov  8 12:12:47 2023, max compression
+gzip compressed data, was "kiara_plugin_core_types-0.5.1rc1.tar", last modified: Mon Apr 15 13:40:31 2024, max compression
```

## Comparing `kiara_plugin.core_types-0.5.0.tar` & `kiara_plugin_core_types-0.5.1rc1.tar`

### file list

```diff
@@ -1,108 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.058041 kiara_plugin.core_types-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6288 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      698 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.058041 kiara_plugin.core_types-0.5.0/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/docs/SUMMARY.md.rej
--rw-r--r--   0 runner    (1001) docker     (127)      846 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.058041 kiara_plugin.core_types-0.5.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33121 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/jobs/logic_and_false.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/jobs/logic_and_true.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/jobs/logic_xor_false.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/jobs/logic_xor_true.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.066041 kiara_plugin.core_types-0.5.0/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/examples/pipelines/example_pipeline_core_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.058041 kiara_plugin.core_types-0.5.0/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.070041 kiara_plugin.core_types-0.5.0/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.058041 kiara_plugin.core_types-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.058041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.070041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.070041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/data_types/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.070041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.070041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/logic/nand.json
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/logic/nor.json
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/logic/xor.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4533 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/renderers/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.070041 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2023-11-08 12:12:47.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-11-08 12:12:47.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-08 12:12:47.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      414 2023-11-08 12:12:47.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-08 12:12:47.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-08 12:12:47.000000 kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.062041 kiara_plugin.core_types-0.5.0/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_and_false/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_and_false/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_and_true/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_and_true/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_xor_false/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_xor_false/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_xor_true/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/job_tests/logic_xor_true/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:47.074041 kiara_plugin.core_types-0.5.0/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      236 2023-11-08 12:12:36.000000 kiara_plugin.core_types-0.5.0/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/SUMMARY.md.rej
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.918612 kiara_plugin_core_types-0.5.1rc1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/check_date_in_range.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/check_date_in_range_string_inputs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_and_false.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_and_true.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_xor_false.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/logic_xor_true.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/jobs/parse_date_1.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/examples/pipelines/example_pipeline_core_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.922612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9763 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/nand.json
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/nor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/xor.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4533 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 13:40:31.000000 kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.914612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range_string_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/check_date_in_range_string_inputs/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_false/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_false/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_true/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_and_true/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_false/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_false/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_true/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/logic_xor_true/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/parse_date_fail/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/parse_date_fail/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/job_tests/parse_date_fail/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.926612 kiara_plugin_core_types-0.5.1rc1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/jobs/parse_date_fail.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:31.930612 kiara_plugin_core_types-0.5.1rc1/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/resources/pipelines/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      236 2024-04-15 13:40:24.000000 kiara_plugin_core_types-0.5.1rc1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.core_types-0.5.0/.cruft.json` & `kiara_plugin_core_types-0.5.1rc1/.cruft.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'61841496d46e8ce4f79da1126443524bde03f977'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "2118176ad585467dd6385e9f7f4de1b420b51f54",
+    "commit": "61841496d46e8ce4f79da1126443524bde03f977",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.core_types-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_core_types-0.5.1rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/.github/workflows/build-darwin.yaml` & `kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-darwin.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 jobs:
   test-darwin:
     name: pytest on darwin
     runs-on: macos-11
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
+        python_version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.core_types
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
       - name: Test with pytest
         run: make test
```

### Comparing `kiara_plugin.core_types-0.5.0/.github/workflows/build-linux.yaml` & `kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-linux.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,54 +22,52 @@
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.core_types
-        run: pip install -U .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: display installed kiara and module package versions
         run: pip list | grep kiara
-      - name: Test with pytest
-        run: make test
+      - name: test with pytest
+        run: pytest --cov-report=xml --cov=kiara_plugin.core_types tests
+      - name: Coveralls
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel: true
+          flag-name: run ${{ join(matrix.*, ' - ') }}
+          format: cobertura
+          file: coverage.xml
 
-# Uncomment this if you have coveralls.io setup with this repo
-#  coverage:
-#    name: create and publish test coverage
-#    runs-on: ubuntu-latest
-#    steps:
-#      - name: "Set up Python 3.9"
-#        uses: actions/setup-python@v4
-#        with:
-#          python-version: "3.9"
-#      - uses: actions/checkout@v3
-#      - name: install kiara
-#        run: pip install -U .[all,dev_testing]
-#      - name: display installed kiara and module package versions
-#        run: pip list | grep kiara
-#      - name: Run coverage
-#        run: coverage run -m pytest tests
-#      - name: coveralls
-#        uses: coverallsapp/github-action@v2
+  coverage:
+    name: test coverage
+    runs-on: ubuntu-latest
+    needs:
+      - test-linux
+    steps:
+      - name: Coveralls Finished
+        uses: coverallsapp/github-action@v2
+        with:
+          parallel-finished: true
 
-# Uncomment this if you want to run mypy
   mypy-linux:
     name: mypy check on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.core_types
-        run: pip install -U .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: Test with mypy
         run: make mypy
 
   linting-linux:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
@@ -94,15 +92,14 @@
   build_python_package:
     name: build python package
     runs-on: ubuntu-latest
     needs:
       - test-linux
       - mypy-linux
       - linting-linux
-
     steps:
       - name: Set up Python 3.11
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - uses: actions/checkout@v3
         with:
@@ -136,15 +133,17 @@
       - name: publish to PyPI  # make sure you have pypi trusted publishing configured for this repo
         uses: pypa/gh-action-pypi-publish@release/v1
 
   build_and_release_conda_package:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
     needs:
-      - build_python_package
+      - test-linux
+      - mypy-linux
+      - linting-linux
     steps:
       - name: "Set up Python 3.11"
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
       - name: pip cache
         id: pip-cache
```

### Comparing `kiara_plugin.core_types-0.5.0/.github/workflows/build-windows.yaml` & `kiara_plugin_core_types-0.5.1rc1/.github/workflows/build-windows.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -12,10 +12,10 @@
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.core_types
-        run: pip install -U --extra-index-url https://pypi.fury.io/dharpa/ .[all,dev_testing]
+        run: pip install -U .[dev_testing]
       - name: Test with pytest
         run: make test
```

### Comparing `kiara_plugin.core_types-0.5.0/.pre-commit-config.yaml` & `kiara_plugin_core_types-0.5.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/LICENSE` & `kiara_plugin_core_types-0.5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/Makefile` & `kiara_plugin_core_types-0.5.1rc1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/README.md` & `kiara_plugin_core_types-0.5.1rc1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,45 @@
+Metadata-Version: 2.1
+Name: kiara_plugin.core_types
+Version: 0.5.1rc1
+Summary: Core data types for kiara.
+Author-email: Markus Binsteiner <markus@frkl.io>
+License: MPL-2.0
+Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.core_types
+Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.core_types
+Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.core_types
+Keywords: kiara
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS.md
+Requires-Dist: kiara==0.5.10rc10
+Requires-Dist: python-dateutil>=2.8.0
+Provides-Extra: dev-documentation
+Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
+Provides-Extra: dev-testing
+Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
+Provides-Extra: dev-utils
+Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
+Provides-Extra: dev-all
+Requires-Dist: kiara[dev_all]; extra == "dev-all"
+Provides-Extra: streamlit
+Requires-Dist: kiara_plugin.streamlit; extra == "streamlit"
+
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.core_types.svg)](https://pypi.python.org/pypi/kiara_plugin.core_types/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.core_types.svg)](https://pypi.python.org/pypi/kiara_plugin.core_types/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.core_types.svg)](https://pypi.python.org/pypi/kiara_plugin.core_types/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.core_types/goto?ref=develop)
 [![Coverage Status](https://coveralls.io/repos/github/DHARPA-Project/kiara_plugin.core_types/badge.svg?branch=develop)](https://coveralls.io/github/DHARPA-Project/kiara_plugin.core_types?branch=develop)
 [![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 
@@ -28,80 +66,62 @@
 
 
 ### Prepare development environment
 
 If you only want to work on the modules, and not the core *Kiara* codebase, follow the instructions below. Otherwise, please
 check the notes on how to setup a *Kiara* development environment under (TODO).
 
-#### Linux & Mac OS X (using make)
+#### Using `pixi` (recommended)
 
-For *NIX-like operating system, setting up a development environment is relatively easy:
+The recommended way to setup a development environment is to use [pixi](https://github.com/prefix-dev/pixi). Check out [their install instructions](https://github.com/prefix-dev/pixi#installation).
 
-```console
-git clone https://github.com/DHARPA-Project/kiara_plugin.core_types.git
-cd kiara_plugin.core_types
-python3 -m venv .venv
-source .venv/bin/activate
-make init
-```
+Once you have `pixi` installed, you need to initialize the environment once:
 
-#### Windows (or manual pip install)
+```
+pixi run install-dev-env
+```
 
-It's impossible to lay out all the ways Python can be installed on a machine, and virtual- (or conda-)envs can be created, so I'll assume you know how to do this.
-One simple way is to install the [Anaconda (individual edition)](https://docs.anaconda.com/anaconda/install/index.html), then use the Anaconda navigator to create a new environment, install the 'git' package in it (if your system does not already have it), and use the 'Open Terminal' option of that environment to start up a terminal that has that virtual-/conda-environment activated.
+You also need to do this whenever a depdendency of this plugin is updated (for example the core `kiara` package).
 
-Once that is done, `cd` into a directory where you want this project folder to live, and do:
+Once that is done, you can enter the environment with:
 
-```console
-# make sure your virtual env is activated!!!
-git clone https://github.com/DHARPA-Project/kiara_plugin.core_types.git
-cd kiara_plugin.core_types
-pip install --extra-index-url https://pypi.fury.io/dharpa/ -U -e .[all_dev]
+```
+pixi shell
 ```
 
-#### Try it out
-
-After this is done, you should be able to run the included example module via:
+This will start a sub-shell with the virtual environment activated, and all dependencies of the plugin package installed. To confirm it works, you can run any `kiara` command:
 
-```console
-kiara run core_types_example text_1="xxx" text_2="yyy"
+```
+kiara --version
+# or
+kiara operation list
+# or
 ...
 ...
 ```
 
-### Re-activate the development environment
-
-The 'prepare' step from above only has to be done once. After that, to re-enable your virtual environment,
-you'll need to navigate to the directory again (wherever that is, in your case), and run the ``source`` command from before again:
+Once you are finished with your development session, you can exit the sub-shell as you would normally do in such cases:
 
-```console
-cd path/to/kiara_plugin.core_types
-source .venv/bin/activate  # if it isn't activated already, for example by the Anaconda navigator
-kiara --help  # or whatever, point is, kiara should be available for you now,
+```
+exit
 ```
 
-### ``make`` targets (Linux & Mac OS X)
+Alternatively, you can also run the `kiara` executable directly, it is located in `.pixi/env/bin/kiara`. So either adapt your `PATH` variable, or do something like:
 
-- ``init``: init development project (install project & dev dependencies into virtualenv, as well as pre-commit git hook)
-- ``update-dependencies``: update development dependencies (mainly the core ``kiara`` package from git)
-- ``flake``: run *flake8* tests
-- ``mypy``: run mypy tests
-- ``test``: run unit tests
-- ``docs``: create static documentation pages (under ``build/site``)
-- ``serve-docs``: serve documentation pages (incl. auto-reload) for getting direct feedback when working on documentation
-- ``clean``: clean build directories
+```
+.pixi/env/bin/kiara operation list
+```
 
-For details (and other, minor targets), check the ``Makefile``.
+In most cases it's recommended to use a pixi shell though.
 
 
-### Running tests
+### Using pre-defined development-related tasks
 
-``` console
-> make test
-# or
-> make coverage
-```
+The included `pixi.toml` file includes some useful tasks that help with development:
 
+- `pixi run pre-commit-check`: runs a set of checks against all files
+- `pixi run tests`: runs the unit tests
+- `pixi run mypy`: run mypy checks
 
 ## Copyright & license
 
 This project is MPL v2.0 licensed, for the license text please check the [LICENSE](/LICENSE) file in this repository.
```

### Comparing `kiara_plugin.core_types-0.5.0/docs/index.md` & `kiara_plugin_core_types-0.5.1rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_core_types-0.5.1rc1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/examples/pipelines/example_pipeline_core_types.yaml` & `kiara_plugin_core_types-0.5.1rc1/examples/pipelines/example_pipeline_core_types.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 pipeline_name: example_pipeline_core_types
 doc: Example pipeline for the core_types plugin.
 steps:
   - step_id: add_hello_string
-    module_type: example_proj.example
+    module_type: core_types.example
     module_config:
       separator: " "
       constants:
         text_1: "Hello"
       defaults:
         text_2: "World"
   - step_id: add_exclamation_mark
-    module_type: example_proj.example
+    module_type: core_types.example
     module_config:
       separator: ""
       constants:
         text_2: "!"
     input_links:
       text_1: add_hello_string.text
```

### Comparing `kiara_plugin.core_types-0.5.0/mkdocs.yml` & `kiara_plugin_core_types-0.5.1rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/pyproject.toml` & `kiara_plugin_core_types-0.5.1rc1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.0,<0.6.0",
+    "kiara==0.5.10rc10",
     "python-dateutil>=2.8.0",
 ]
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
@@ -238,9 +238,13 @@
 plugins = [
     "pydantic.mypy"
 ]
 
 
 # mypy per-module options:
 [[tool.mypy.overrides]]
-module = ["placholder.dummy.*"]
+module = [
+    "appdirs.*",
+    "pyarrow.*",
+    "ruamel.*"
+]
 ignore_missing_imports = true
```

### Comparing `kiara_plugin.core_types-0.5.0/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/scripts/documentation/gen_info_pages.py` & `kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/scripts/documentation/gen_module_doc.py` & `kiara_plugin_core_types-0.5.1rc1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/__init__.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/data_types/__init__.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,16 @@
     a schema for the items in the list.
     """
 
     _data_type_name: ClassVar[str] = "list"
 
     @classmethod
     def python_class(cls) -> Type:
-        return KiaraList
+        result: Type[KiaraList] = KiaraList  # make mypy happy
+        return result
 
     def _retrieve_characteristics(self) -> DataTypeCharacteristics:
         return DataTypeCharacteristics(is_scalar=False, is_json_serializable=True)
 
     def parse_python_obj(self, data: Any) -> KiaraList:
 
         python_cls = data.__class__
```

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/data_types/models.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/data_types/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,25 +81,26 @@
         from kiara.models.values.value import SerializationResult
 
         serialized = SerializationResult(**serialized_data)
         return serialized
 
     @classmethod
     def python_class(cls) -> Type[KiaraModel]:
-        return KiaraModel
+        result: Type[KiaraModel] = KiaraModel  # make mypy happy
+        return result
 
     @lru_cache(maxsize=1)
     def get_model_cls(self) -> Type[KiaraModel]:
 
         model_type_id = self.type_config.kiara_model_id
         assert model_type_id is not None
 
         model_registry = ModelRegistry.instance()
 
-        model_cls = model_registry.get_model_cls(
+        model_cls: Type[KiaraModel] = model_registry.get_model_cls(
             model_type_id, required_subclass=KiaraModel
         )
 
         return model_cls
 
     def parse_python_obj(self, data: Any) -> KiaraModel:
 
@@ -216,15 +217,15 @@
     def get_model_cls(self) -> Type[KiaraModel]:
 
         model_type_id = self.type_config.kiara_model_id
         assert model_type_id is not None
 
         model_registry = ModelRegistry.instance()
 
-        model_cls = model_registry.get_model_cls(
+        model_cls: Type[KiaraModel] = model_registry.get_model_cls(
             model_type_id, required_subclass=KiaraModel
         )
 
         return model_cls
 
     def parse_python_obj(self, data: Any) -> KiaraModelList[KiaraModel]:
 
@@ -247,15 +248,15 @@
                     model_instance = self.get_model_cls()(**_data)
                     result.append(model_instance)
                 except Exception as e:
                     raise KiaraException(
                         msg=f"Can't instantiate model of type '{self.type_config.kiara_model_id}' with data of type '{type(item)}': {e}"
                     )
 
-        instance: KiaraModelList[KiaraModel] = KiaraModelList[self.get_model_cls()].construct(  # type: ignore
+        instance: KiaraModelList[KiaraModel] = KiaraModelList[self.get_model_cls()](  # type: ignore
             list_items=result, kiara_model_id=self.type_config.kiara_model_id
         )
         return instance
 
     def _validate(self, value: Any) -> None:
 
         if not isinstance(value, KiaraModelList):
```

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/models.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/__init__.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/boolean.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/boolean.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/date.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/date.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/list.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/list.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/models.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/modules/string.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/modules/string.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/pipelines/logic/xor.json` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/pipelines/logic/xor.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin/core_types/renderers/lineage.py` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin/core_types/renderers/lineage.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.core_types-0.5.0/src/kiara_plugin.core_types.egg-info/SOURCES.txt` & `kiara_plugin_core_types-0.5.1rc1/src/kiara_plugin.core_types.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 Makefile
 README.md
 commitlint.config.js
 mkdocs.yml
+pixi.toml
 pyproject.toml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
 .github/workflows/build-darwin.yaml
 .github/workflows/build-linux.yaml
 .github/workflows/build-windows.yaml
 ci/conda/conda-pkg-patch.yaml
@@ -25,18 +26,21 @@
 docs/usage.md
 docs/stylesheets/extra.css
 examples/data/Readme.md
 examples/data/journals/JournalEdges1902.csv
 examples/data/journals/JournalNodes1902.csv
 examples/data/journals/Readme.md
 examples/jobs/Readme.md
+examples/jobs/check_date_in_range.yaml
+examples/jobs/check_date_in_range_string_inputs.yaml
 examples/jobs/logic_and_false.yaml
 examples/jobs/logic_and_true.yaml
 examples/jobs/logic_xor_false.yaml
 examples/jobs/logic_xor_true.yaml
+examples/jobs/parse_date_1.yaml
 examples/pipelines/Readme.md
 examples/pipelines/example_pipeline_core_types.yaml
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.core_types.egg-info/PKG-INFO
 src/kiara_plugin.core_types.egg-info/SOURCES.txt
@@ -63,12 +67,21 @@
 src/kiara_plugin/core_types/pipelines/logic/xor.json
 src/kiara_plugin/core_types/renderers/__init__.py
 src/kiara_plugin/core_types/renderers/lineage.py
 src/kiara_plugin/core_types/resources/.gitkeep
 tests/conftest.py
 tests/test_job_descs.py
 tests/test_kiara_modules_default.py
+tests/job_tests/check_date_in_range/outputs.yaml
+tests/job_tests/check_date_in_range_string_inputs/outputs.yaml
 tests/job_tests/logic_and_false/outputs.yaml
 tests/job_tests/logic_and_true/outputs.yaml
 tests/job_tests/logic_xor_false/outputs.yaml
 tests/job_tests/logic_xor_true/outputs.yaml
-tests/resources/.gitkeep
+tests/job_tests/parse_date_fail/outputs.py
+tests/job_tests/parse_date_fail/outputs.yaml
+tests/resources/.gitkeep
+tests/resources/jobs/.gitkeep
+tests/resources/jobs/init.yaml
+tests/resources/jobs/parse_date_fail.yaml
+tests/resources/pipelines/.gitkeep
+tests/resources/pipelines/init.yaml
```

### Comparing `kiara_plugin.core_types-0.5.0/tests/conftest.py` & `kiara_plugin_core_types-0.5.1rc1/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,53 +13,87 @@
 import os
 import tempfile
 import uuid
 from pathlib import Path
 
 import pytest
 
+from kiara.api import JobDesc, KiaraAPI
 from kiara.context import KiaraConfig
-from kiara.interfaces.python_api import KiaraAPI
 from kiara.interfaces.python_api.models.job import JobTest
-from kiara.utils.testing import get_tests_for_job, list_job_descs
+from kiara.utils.testing import get_init_job, get_tests_for_job, list_job_descs
 
 ROOT_DIR = os.path.abspath(os.path.join(os.path.dirname(__file__), ".."))
-JOBS_FOLDER = Path(os.path.join(ROOT_DIR, "examples", "jobs"))
+JOBS_FOLDERS = [
+    Path(os.path.join(ROOT_DIR, "tests", "resources", "jobs")),
+    Path(os.path.join(ROOT_DIR, "examples", "jobs")),
+]
 
 
 def create_temp_dir():
     session_id = str(uuid.uuid4())
     TEMP_DIR = Path(os.path.join(tempfile.gettempdir(), "kiara_tests"))
 
     instance_path = os.path.join(
         TEMP_DIR.resolve().absolute(), f"instance_{session_id}"
     )
     return instance_path
 
 
+def get_job_alias(job_desc: JobDesc) -> str:
+    return job_desc.job_alias
+
+
 @pytest.fixture
 def kiara_api() -> KiaraAPI:
 
     instance_path = create_temp_dir()
     kc = KiaraConfig.create_in_folder(instance_path)
     api = KiaraAPI(kc)
     return api
 
 
-@pytest.fixture(params=list_job_descs(JOBS_FOLDER))
-def example_job_test(request, kiara_api) -> JobTest:
+@pytest.fixture
+def kiara_api_init_example() -> KiaraAPI:
+    instance_path = create_temp_dir()
+    kc = KiaraConfig.create_in_folder(instance_path)
+    api = KiaraAPI(kc)
+
+    init_jobs = []
+    for jobs_folder in JOBS_FOLDERS:
+        init_job = get_init_job(jobs_folder)
+        if init_job is not None:
+            init_jobs.append(init_job)
+
+    if not init_jobs:
+        return api
+
+    for init_job in init_jobs:
+        results = api.run_job(init_job, comment="Init example job")
+
+        if not init_job.save:
+            continue
+
+        for field_name, alias_name in init_job.save.items():
+            api.store_value(results[field_name], alias_name)
+
+    return api
+
+
+@pytest.fixture(params=list_job_descs(JOBS_FOLDERS), ids=get_job_alias)
+def example_job_test(request, kiara_api_init_example) -> JobTest:
 
     job_tests_folder = Path(os.path.join(ROOT_DIR, "tests", "job_tests"))
 
     job_desc = request.param
     tests = get_tests_for_job(
         job_alias=job_desc.job_alias, job_tests_folder=job_tests_folder
     )
 
-    job_test = JobTest(kiara_api=kiara_api, job_desc=job_desc, tests=tests)
+    job_test = JobTest(kiara_api=kiara_api_init_example, job_desc=job_desc, tests=tests)
     return job_test
 
 
 @pytest.fixture
 def example_data_folder() -> Path:
     return Path(os.path.join(ROOT_DIR, "examples", "data"))
```

### Comparing `kiara_plugin.core_types-0.5.0/tests/test_job_descs.py` & `kiara_plugin_core_types-0.5.1rc1/tests/test_job_descs.py`

 * *Files identical despite different names*

