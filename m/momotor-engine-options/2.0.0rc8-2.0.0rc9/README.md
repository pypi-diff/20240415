# Comparing `tmp/momotor-engine-options-2.0.0rc8.tar.gz` & `tmp/momotor-engine-options-2.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momotor-engine-options-2.0.0rc8.tar", last modified: Fri Jan 12 10:00:09 2024, max compression
+gzip compressed data, was "momotor-engine-options-2.0.0rc9.tar", last modified: Tue Jan 16 09:23:36 2024, max compression
```

## Comparing `momotor-engine-options-2.0.0rc8.tar` & `momotor-engine-options-2.0.0rc9.tar`

### file list

```diff
@@ -1,125 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/
--rw-rw-rw-   0 root         (0) root         (0)     1215 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     3251 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/.idea/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/.idea/inspectionProfiles/
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.idea/momotor.lib.engine-options.iml
--rw-rw-rw-   0 root         (0) root         (0)      238 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/.idea/workspace.xml
--rw-rw-rw-   0 root         (0) root         (0)    18559 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     2483 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      764 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     6988 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/_static/logo-text-negative.png
--rw-rw-rw-   0 root         (0) root         (0)     6887 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/_static/logo-text.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/docs/source/_templates/
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/_templates/projectlinks.html
--rw-rw-rw-   0 root         (0) root         (0)     4790 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/dependencies.rst
--rw-rw-rw-   0 root         (0) root         (0)      161 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/exceptions.rst
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      162 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/option.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/docs/source/options/
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/options/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/options/scheduler.rst
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/options/tools.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/docs/source/parser/
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/parser/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    30840 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/parser/syntax.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/providers.rst
--rw-rw-rw-   0 root         (0) root         (0)     6989 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/registry.rst
--rw-rw-rw-   0 root         (0) root         (0)    11586 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/result_query.rst
--rw-rw-rw-   0 root         (0) root         (0)      126 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/task_id.rst
--rw-rw-rw-   0 root         (0) root         (0)      618 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/docs/source/utilities.rst
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/publish-docs.sh
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/semver.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7428 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/convert.py
--rw-rw-rw-   0 root         (0) root         (0)     8331 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/doc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-12 09:59:28.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-12 09:59:28.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)    11572 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/preflight.py
--rw-rw-rw-   0 root         (0) root         (0)     8274 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     5570 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/tools/
--rw-rw-rw-   0 root         (0) root         (0)     6185 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       17 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/domain/tools/_domain.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/exception.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/filter_files.py
--rw-rw-rw-   0 root         (0) root         (0)    13199 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-12 09:59:28.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/consts.py
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/keyvalue.py
--rw-rw-rw-   0 root         (0) root         (0)     4024 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     2071 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)    24823 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8308 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/selector.py
--rw-rw-rw-   0 root         (0) root         (0)     1710 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/parser/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1055 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/providers.py
--rw-rw-rw-   0 root         (0) root         (0)     6463 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/result_query.py
--rw-rw-rw-   0 root         (0) root         (0)    15914 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/sphinx_ext.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/split.py
--rw-rw-rw-   0 root         (0) root         (0)     9149 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/task_id.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/tools/
--rw-rw-rw-   0 root         (0) root         (0)      919 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6210 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/tools/registry.py
--rw-rw-rw-   0 root         (0) root         (0)    12393 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/tools/tool.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/tools/types.py
--rw-rw-rw-   0 root         (0) root         (0)     6068 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/tools/version.py
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/types.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-12 10:00:05.000000 momotor-engine-options-2.0.0rc8/src/momotor/options/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2483 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3256 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      267 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     7508 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_option_definition.py
--rw-rw-rw-   0 root         (0) root         (0)     4365 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_parser_modifier.py
--rw-rw-rw-   0 root         (0) root         (0)     6167 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_parser_placeholders.py
--rw-rw-rw-   0 root         (0) root         (0)     9529 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_parser_reference.py
--rw-rw-rw-   0 root         (0) root         (0)     8543 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_parser_selector.py
--rw-rw-rw-   0 root         (0) root         (0)     8110 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_utils_dependencies.py
--rw-rw-rw-   0 root         (0) root         (0)     9006 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/test_utils_tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/nodefault/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/nodefault/1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/nodefault/2.1
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/nodefault/named
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/tool/
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/tool/1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/tool/2.1
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/tool/2.2
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/tool/_default
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/tool/envs
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/2.0/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/2.0/a
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/2.0/b
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-12 10:00:09.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/2.1/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/2.1/b
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/files/toolregistry.d/variant/2.1/c
--rw-rw-rw-   0 root         (0) root         (0)     3834 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/test_tool_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2995 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/test_tools_match.py
--rw-rw-rw-   0 root         (0) root         (0)     3221 2024-01-12 09:59:27.000000 momotor-engine-options-2.0.0rc8/tests/tools/test_tools_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     3251 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/.idea/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0 root         (0) root         (0)      174 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/momotor.lib.engine-options.iml
+-rw-rw-rw-   0 root         (0) root         (0)      238 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/.idea/workspace.xml
+-rw-rw-rw-   0 root         (0) root         (0)    18559 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     6988 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text-negative.png
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/_templates/
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/_templates/projectlinks.html
+-rw-rw-rw-   0 root         (0) root         (0)     4895 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/dependencies.rst
+-rw-rw-rw-   0 root         (0) root         (0)      161 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/exceptions.rst
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/option.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/options/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/options/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/options/scheduler.rst
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/options/tools.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/docs/source/parser/
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/parser/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    30840 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/parser/syntax.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/providers.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6989 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/registry.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11586 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/result_query.rst
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/task_id.rst
+-rw-rw-rw-   0 root         (0) root         (0)      618 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/docs/source/utilities.rst
+-rw-rw-rw-   0 root         (0) root         (0)      423 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/publish-docs.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/semver.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7428 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)     8331 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     1181 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/doc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)    11572 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/preflight.py
+-rw-rw-rw-   0 root         (0) root         (0)     8274 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4367 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     6185 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/_domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/exception.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/filter_files.py
+-rw-rw-rw-   0 root         (0) root         (0)    13301 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/consts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/keyvalue.py
+-rw-rw-rw-   0 root         (0) root         (0)     4024 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)    24823 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8308 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     1710 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/parser/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1055 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/providers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6463 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/result_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2555 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/fixextref.py
+-rw-rw-rw-   0 root         (0) root         (0)    15739 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/option.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/split.py
+-rw-rw-rw-   0 root         (0) root         (0)     9149 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/task_id.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/
+-rw-rw-rw-   0 root         (0) root         (0)      919 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6210 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    12393 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/tool.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     6068 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/tools/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/types.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-16 09:23:31.000000 momotor-engine-options-2.0.0rc9/src/momotor/options/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2483 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3338 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      267 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     7508 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_option_definition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4365 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_modifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     6167 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_placeholders.py
+-rw-rw-rw-   0 root         (0) root         (0)     9529 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_reference.py
+-rw-rw-rw-   0 root         (0) root         (0)     8543 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_parser_selector.py
+-rw-rw-rw-   0 root         (0) root         (0)     8110 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_utils_dependencies.py
+-rw-rw-rw-   0 root         (0) root         (0)     9006 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/test_utils_tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/2.1
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/nodefault/named
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/2.1
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/2.2
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/_default
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/tool/envs
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.0/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.0/a
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.0/b
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-16 09:23:36.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.1/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.1/b
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/files/toolregistry.d/variant/2.1/c
+-rw-rw-rw-   0 root         (0) root         (0)     3834 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/test_tool_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/test_tools_match.py
+-rw-rw-rw-   0 root         (0) root         (0)     3221 2024-01-16 09:22:54.000000 momotor-engine-options-2.0.0rc9/tests/tools/test_tools_options.py
```

### Comparing `momotor-engine-options-2.0.0rc8/.gitignore` & `momotor-engine-options-2.0.0rc9/.gitignore`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/.gitlab-ci.yml` & `momotor-engine-options-2.0.0rc9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/.idea/inspectionProfiles/Project_Default.xml` & `momotor-engine-options-2.0.0rc9/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/.idea/momotor.lib.engine-options.iml` & `momotor-engine-options-2.0.0rc9/.idea/momotor.lib.engine-options.iml`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/CHANGELOG.md` & `momotor-engine-options-2.0.0rc9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/PKG-INFO` & `momotor-engine-options-2.0.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: Momotor Engine Options Library
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
```

### Comparing `momotor-engine-options-2.0.0rc8/README.md` & `momotor-engine-options-2.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/Makefile` & `momotor-engine-options-2.0.0rc9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/make.bat` & `momotor-engine-options-2.0.0rc9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/_static/logo-text-negative.png` & `momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text-negative.png`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/_static/logo-text.png` & `momotor-engine-options-2.0.0rc9/docs/source/_static/logo-text.png`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/_templates/projectlinks.html` & `momotor-engine-options-2.0.0rc9/docs/source/_templates/projectlinks.html`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/conf.py` & `momotor-engine-options-2.0.0rc9/docs/source/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         loc = {}
         exec(version_file.readline(), {}, loc)
         return loc['__VERSION__'] + version_tag
 
 
 # -- Project information -----------------------------------------------------
 
+package_name = 'momotor-engine-options'
 project = 'Momotor Engine Options'
 copyright = '2021-%d, Eindhoven University of Technology' % datetime.datetime.now().year
 author = 'E.T.J. Scheffers'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
@@ -49,18 +50,19 @@
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
-    'momotor.options.sphinx_ext',
     'sphinx.ext.autodoc',
     'sphinx.ext.intersphinx',
     'sphinx_autodoc_typehints',
+    'momotor.options.sphinx.option',
+    'momotor.options.sphinx.fixextref',  # Must be listed after intersphinx
     'pytest_doctestplus.sphinx.doctestplus',
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # List of patterns, relative to source directory, that match files and
@@ -77,14 +79,15 @@
 
 # -- Options for autodoc -----------------------------------------------------
 
 autodoc_member_order = 'groupwise'
 
 # -- Options for intersphinx -------------------------------------------------
 
+
 def inventory(domain, name):
     # Try to collect intersphinx mapping from development environment first, then from online version
 
     local_project = None
     if domain == 'engine':
         local_project = os.path.join(project_dir, '..', name)
 
@@ -122,16 +125,16 @@
 html_theme_options = {
     "light_logo": "logo-text.png",
     "dark_logo": "logo-text-negative.png",
 }
 
 html_context = {
     'project_url': 'https://momotor.org/',
-    'pypi_url': 'https://pypi.org/project/momotor-engine-options/',
-    'repository_url': 'https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/',
+    'pypi_url': f'https://pypi.org/project/{package_name}/',
+    'repository_url': f'https://gitlab.tue.nl/momotor/engine-py3/{package_name}/',
 }
 
 html_sidebars = {
     "**": [
         "sidebar/brand.html",
         "sidebar/search.html",
         "sidebar/scroll-start.html",
@@ -147,8 +150,7 @@
 _PREAMBLE = r"""
 \DeclareUnicodeCharacter{2794}{$\rightarrow$}
 """
 
 latex_elements = {
     'preamble': _PREAMBLE,
 }
-
```

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/index.rst` & `momotor-engine-options-2.0.0rc9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/options/index.rst` & `momotor-engine-options-2.0.0rc9/docs/source/options/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/options/tools.rst` & `momotor-engine-options-2.0.0rc9/docs/source/options/tools.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/parser/index.rst` & `momotor-engine-options-2.0.0rc9/docs/source/parser/index.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/parser/syntax.rst` & `momotor-engine-options-2.0.0rc9/docs/source/parser/syntax.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/registry.rst` & `momotor-engine-options-2.0.0rc9/docs/source/registry.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/result_query.rst` & `momotor-engine-options-2.0.0rc9/docs/source/result_query.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/docs/source/utilities.rst` & `momotor-engine-options-2.0.0rc9/docs/source/utilities.rst`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/pyproject.toml` & `momotor-engine-options-2.0.0rc9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/convert.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/convert.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/dependencies.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/dependencies.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/doc.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/doc.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/preflight.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/preflight.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/tasks.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/domain/scheduler/tools.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/scheduler/tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import typing
-import warnings
 
 from momotor.bundles import RecipeBundle, ConfigBundle, ResultsBundle
 from momotor.options.doc import annotate_docstring
 from momotor.options.domain.tools import ToolOptionDefinition, TOOLS_DOMAIN
 from momotor.options.option import OptionDefinition, OptionNameDomain
 from momotor.options.parser.placeholders import replace_placeholders
 from momotor.options.providers import Providers
@@ -19,14 +18,17 @@
 TOOLS_OPTION_NAME = OptionNameDomain('tools', DOMAIN)
 
 #: The :momotor:option:`tools@scheduler` option defines the tools required for a step.
 TOOLS_OPTION = OptionDefinition(
     name=TOOLS_OPTION_NAME,
     type='string',
     doc=f"""\
+        .. role:: xml(code)
+           :language: xml
+   
         List of tools required for the step. Can only be provided by :xml:`<step>` nodes.
         
         Multiple tools can be provided by using multiple {TOOLS_OPTION_NAME} options, or using a single
         {TOOLS_OPTION_NAME} option with multiple tool names. Multiple tool names on a single option should 
         be space or comma separated.
         
         The list of tools should only contain tool names. Any detailed version requirements should
@@ -36,44 +38,23 @@
         this option is used to resolve a tool.
     """,
     multiple=True,
     location='step',
 )
 
 
-# deprecated interface. todo: remove in next major version
-@typing.overload
-def get_scheduler_tools_option(
-        recipe: RecipeBundle,
-        config: ConfigBundle | None,
-        step_id: str
-) -> "ToolRequirements":
-    ...
-
-
-# new interface
-@typing.overload
-def get_scheduler_tools_option(
-        recipe: RecipeBundle,
-        config: ConfigBundle | None,
-        results: ResultsBundle | None,
-        *, task_id: StepTaskId
-) -> "ToolRequirements":
-    ...
-
-
 @annotate_docstring(
     TOOLS_OPTION_NAME=TOOLS_OPTION_NAME,
     TOOLS_DOMAIN=TOOLS_DOMAIN,
 )
 def get_scheduler_tools_option(
         recipe: RecipeBundle,
         config: ConfigBundle | None,
-        results: ResultsBundle | None = None,
-        *, step_id: str = None, task_id: StepTaskId = None
+        results: ResultsBundle | None,
+        *, task_id: StepTaskId
 ) -> "ToolRequirements":
     """ Evaluate the tool requirements by parsing the :momotor:option:`{TOOLS_OPTION_NAME}` option
     for a single step in the given bundles.
 
     This gets the value of the :momotor:option:`{TOOLS_OPTION_NAME}` option for the step, and subsequently gets the
     specific tool version requirements (if any) from the options in the
     :py:ref:`{TOOLS_DOMAIN} domain <{TOOLS_DOMAIN} domain>`.
@@ -106,32 +87,17 @@
     is preferred, but if not available any ``anaconda3`` will do.
 
     For the format of the tool version requirements, see :py:ref:`tool registry`.
 
     :param recipe: The recipe bundle.
     :param config: The config bundle.
     :param results: The results bundle.
-    :param step_id: The step id.
     :param task_id: The task id.
     :return: The tool requirements for the requested step and task.
     """
-    if step_id is None and isinstance(results, str):
-        warnings.warn("get_scheduler_tools_option() called without positional argument 'result'", DeprecationWarning)
-        task_id = StepTaskId(step_id=results, task_number=None)
-        results = None
-    else:
-        results = typing.cast(typing.Optional[ResultsBundle], results)
-
-    if step_id is not None:
-        assert task_id is None, "provide `step_id` or `task_id`, not both"
-        warnings.warn("get_scheduler_tools_option() 'step_id' is deprecated, use 'task_id'", DeprecationWarning)
-        task_id = StepTaskId(step_id=step_id, task_number=None)
-
-    assert isinstance(task_id, StepTaskId), f'invalid type for `task_id`: {task_id!r}'
-
     requirement_providers = Providers(
         recipe=recipe,
         task_id=task_id
     )
 
     version_providers = Providers(
         recipe=recipe,
```

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/domain/tools/__init__.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/domain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/exception.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/exception.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/filter_files.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/filter_files.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/option.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/option.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,18 @@
         """ Return the short name of the option (i.e. without the domain if it is the default domain)
         """
         if self.domain == Option.DEFAULT_DOMAIN:
             return self.name
         else:
             return self.qualified_name()
 
-    def __eq__(self, other: "OptionNameDomain") -> bool:
+    def __eq__(self, other: typing.Any) -> bool:
+        if not isinstance(other, OptionNameDomain):
+            other = self.from_qualified_name(str(other))
+
         return self.domain == other.domain and self.name == other.name
 
     def __str__(self):
         return self.qualified_name()
 
 
 @dataclass(frozen=True)
```

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/consts.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/consts.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/keyvalue.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/keyvalue.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/modifier.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/modifier.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/placeholders.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/reference.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/reference.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/selector.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/selector.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/parser/tasks.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/parser/tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/providers.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/providers.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/result_query.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/result_query.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/sphinx_ext.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/sphinx/option.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,30 +6,27 @@
 
 from momotor.bundles.elements.options import Option
 from momotor.options import OptionDefinition, OptionNameDomain
 
 try:
     from docutils import nodes
     from docutils.nodes import make_id
-    from docutils.parsers.rst import Directive, directives
+    from docutils.parsers.rst import directives
     from docutils.parsers.rst.states import RSTState
     from docutils.statemachine import ViewList, StringList
-
     from sphinx import addnodes
     from sphinx.addnodes import desc_signature
     from sphinx.application import Sphinx
     from sphinx.directives import ObjectDescription
-    from sphinx.domains import Domain, ObjType, Index
-    from sphinx.domains.python import PyXRefRole, PyVariable, ObjectEntry
-    from sphinx.domains.std import StandardDomain
+    from sphinx.domains import Domain, ObjType
+    from sphinx.domains.python import PyVariable, ObjectEntry
     from sphinx.environment import BuildEnvironment
-    from sphinx.errors import ExtensionError
-    from sphinx.ext.autodoc import Documenter, AttributeDocumenter, DataDocumenter
+    from sphinx.ext.autodoc import DataDocumenter
     from sphinx.roles import XRefRole
-    from sphinx.util import import_object, nested_parse_with_titles, logging
+    from sphinx.util import nested_parse_with_titles, logging
     from sphinx.util.docfields import Field
     from sphinx.util.docstrings import prepare_docstring
     from sphinx.util.nodes import make_refnode
     from sphinx.util.typing import OptionSpec
 
 except ImportError:
     has_sphinx = False
@@ -396,15 +393,14 @@
 
             sourcename = self.get_sourcename()
             tab_width = self.directive.state.document.settings.tab_width
 
             for line in document_option_definition(self.object, tab_width):
                 self.add_line(line, sourcename)
 
-
     def setup(app: Sphinx) -> dict[str, typing.Any]:
         from importlib.metadata import version
 
         app.setup_extension('sphinx.ext.autodoc')
         app.add_autodocumenter(OptionDefinitionVariableDocumenter)
         app.add_domain(MomotorDomain)
```

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/split.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/split.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/task_id.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/task_id.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/tools/__init__.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/tools/registry.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/registry.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/tools/tool.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/tool.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/tools/version.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/tools/version.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor/options/types.py` & `momotor-engine-options-2.0.0rc9/src/momotor/options/types.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/PKG-INFO` & `momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momotor-engine-options
-Version: 2.0.0rc8
+Version: 2.0.0rc9
 Summary: Momotor Engine Options Library
 Author-email: Erik Scheffers <e.t.j.scheffers@tue.nl>
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Homepage, https://momotor.org
 Project-URL: Documentation, https://momotor.org/doc/engine/momotor-engine-options/
 Project-URL: Repository, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/
 Project-URL: Tracker, https://gitlab.tue.nl/momotor/engine-py3/momotor-engine-options/issues
```

### Comparing `momotor-engine-options-2.0.0rc8/src/momotor_engine_options.egg-info/SOURCES.txt` & `momotor-engine-options-2.0.0rc9/src/momotor_engine_options.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 src/momotor/options/dependencies.py
 src/momotor/options/doc.py
 src/momotor/options/exception.py
 src/momotor/options/filter_files.py
 src/momotor/options/option.py
 src/momotor/options/providers.py
 src/momotor/options/result_query.py
-src/momotor/options/sphinx_ext.py
 src/momotor/options/split.py
 src/momotor/options/task_id.py
 src/momotor/options/types.py
 src/momotor/options/version.py
 src/momotor/options/domain/__init__.py
 src/momotor/options/domain/scheduler/__init__.py
 src/momotor/options/domain/scheduler/_domain.py
@@ -58,14 +57,17 @@
 src/momotor/options/parser/consts.py
 src/momotor/options/parser/keyvalue.py
 src/momotor/options/parser/modifier.py
 src/momotor/options/parser/placeholders.py
 src/momotor/options/parser/reference.py
 src/momotor/options/parser/selector.py
 src/momotor/options/parser/tasks.py
+src/momotor/options/sphinx/__init__.py
+src/momotor/options/sphinx/fixextref.py
+src/momotor/options/sphinx/option.py
 src/momotor/options/tools/__init__.py
 src/momotor/options/tools/registry.py
 src/momotor/options/tools/tool.py
 src/momotor/options/tools/types.py
 src/momotor/options/tools/version.py
 src/momotor_engine_options.egg-info/PKG-INFO
 src/momotor_engine_options.egg-info/SOURCES.txt
```

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_option_definition.py` & `momotor-engine-options-2.0.0rc9/tests/test_option_definition.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_parser_modifier.py` & `momotor-engine-options-2.0.0rc9/tests/test_parser_modifier.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_parser_placeholders.py` & `momotor-engine-options-2.0.0rc9/tests/test_parser_placeholders.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_parser_reference.py` & `momotor-engine-options-2.0.0rc9/tests/test_parser_reference.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_parser_selector.py` & `momotor-engine-options-2.0.0rc9/tests/test_parser_selector.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_utils_dependencies.py` & `momotor-engine-options-2.0.0rc9/tests/test_utils_dependencies.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/test_utils_tasks.py` & `momotor-engine-options-2.0.0rc9/tests/test_utils_tasks.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/tools/test_tool_registry.py` & `momotor-engine-options-2.0.0rc9/tests/tools/test_tool_registry.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/tools/test_tools_match.py` & `momotor-engine-options-2.0.0rc9/tests/tools/test_tools_match.py`

 * *Files identical despite different names*

### Comparing `momotor-engine-options-2.0.0rc8/tests/tools/test_tools_options.py` & `momotor-engine-options-2.0.0rc9/tests/tools/test_tools_options.py`

 * *Files identical despite different names*

