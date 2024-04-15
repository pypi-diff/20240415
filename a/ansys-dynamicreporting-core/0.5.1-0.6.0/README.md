# Comparing `tmp/ansys-dynamicreporting-core-0.5.1.tar.gz` & `tmp/ansys_dynamicreporting_core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-dynamicreporting-core-0.5.1.tar", last modified: Thu Jan 18 09:55:40 2024, max compression
+gzip compressed data, was "ansys_dynamicreporting_core-0.6.0.tar", last modified: Mon Apr 15 16:29:32 2024, max compression
```

## Comparing `ansys-dynamicreporting-core-0.5.1.tar` & `ansys_dynamicreporting_core-0.6.0.tar`

### file list

```diff
@@ -1,176 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.074143 ansys-dynamicreporting-core-0.5.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.030143 ansys-dynamicreporting-core-0.5.1/.ci/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.ci/pull_adr_image.sh
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.030143 ansys-dynamicreporting-core-0.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.030143 ansys-dynamicreporting-core-0.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.github/workflows/ci_cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.github/workflows/nightly-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.github/workflows/nightly.yml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-01-18 09:55:40.074143 ansys-dynamicreporting-core-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.030143 ansys-dynamicreporting-core-0.5.1/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/adr_utils.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/all_scrap_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/all_test_prop.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13813 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/pyadritem.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/read_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/codegen/rename_whl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.030143 ansys-dynamicreporting-core-0.5.1/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/.vale.ini
--rwxr-xr-x   0 runner    (1001) docker     (127)      970 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.030143 ansys-dynamicreporting-core-0.5.1/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/_static/
--rwxr-xr-x   0 runner    (1001) docker     (127)    43416 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_complete_report_0.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    33601 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_create_db_0.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     9619 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_create_db_1.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     7820 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_create_db_2.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    67994 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_connect_0.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    67994 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_connect_1.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60479 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_connect_3.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    46192 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_two_simulation_same_db_0.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    45542 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_two_simulation_same_db_1.png
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)   103592 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/all_items.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     9105 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/bar_plot.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    31953 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/default_thumb.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     9047 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/heatmap.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    60188 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/img_item.PNG
--rwxr-xr-x   0 runner    (1001) docker     (127)    21115 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/line_plot.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    28445 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/parallel_coord.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    13051 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/pie_plot.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6081 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/sankey.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8025 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/simpletable.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/text_img.PNG
--rwxr-xr-x   0 runner    (1001) docker     (127)     5131 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_static/text_img_after.PNG
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/class_documentation.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4630 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4185 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/00-create_db.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3862 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/01-connect.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7070 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/02-plottype.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      239 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/25-intermediate/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2961 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/25-intermediate/00-tagging.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3792 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/25-intermediate/01-queries.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/25-intermediate/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/50-advanced/
--rwxr-xr-x   0 runner    (1001) docker     (127)    15801 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/50-advanced/00-complete_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7536 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/50-advanced/01-two_simulation_same_db.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/50-advanced/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.038143 ansys-dynamicreporting-core-0.5.1/doc/source/gettingstarted/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5815 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/gettingstarted/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.042143 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11275 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/DataItemObject.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     3220 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/DatasetandSessionObjects.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    13142 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/GettingStarted.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    13430 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/ServerObject.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    58204 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/TemplateObjects.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)      637 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.042143 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/
--rwxr-xr-x   0 runner    (1001) docker     (127)    27314 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem293.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    28599 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem294.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    14492 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem304.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    49403 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem305.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    35137 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem306.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    27128 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem307.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    44203 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem308.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    94550 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem309.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    70692 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem310.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    15728 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem311.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    44941 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem312.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     8196 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem313.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.046143 ansys-dynamicreporting-core-0.5.1/doc/source/userguide/
--rwxr-xr-x   0 runner    (1001) docker     (127)     7177 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/source/userguide/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.046143 ansys-dynamicreporting-core-0.5.1/doc/styles/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/styles/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.026143 ansys-dynamicreporting-core-0.5.1/doc/styles/Vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.046143 ansys-dynamicreporting-core-0.5.1/doc/styles/Vocab/ANSYS/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 09:55:40.074143 ansys-dynamicreporting-core-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.026143 ansys-dynamicreporting-core-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.026143 ansys-dynamicreporting-core-0.5.1/src/ansys/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.026143 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.046143 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20962 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    39395 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/docker_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.050143 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/extremely_ugly_hacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/filelock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/geofile_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    25732 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_download_html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_download_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)   119749 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_objects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    71214 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_remote_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    29810 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.070143 ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-01-18 09:55:40.000000 ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-18 09:55:39.000000 ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/test_cleanup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.054143 ansys-dynamicreporting-core-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3413 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.058143 ansys-dynamicreporting-core-0.5.1/tests/test_data/
--rwxr-xr-x   0 runner    (1001) docker     (127)    42741 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/aa_00_0_alpha1.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    56961 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/aa_00_0_u.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    42648 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/aa_00_1_alpha1.png
--rwxr-xr-x   0 runner    (1001) docker     (127)   248887 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/ami.evsn
--rwxr-xr-x   0 runner    (1001) docker     (127)    94256 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/dam_break.ens
--rwxr-xr-x   0 runner    (1001) docker     (127)   368036 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/dam_break.mp4
--rwxr-xr-x   0 runner    (1001) docker     (127)   502602 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/flow2d.csf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.058143 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/
--rwxr-xr-x   0 runner    (1001) docker     (127)   413696 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/db.sqlite3
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.058143 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/media/
--rwxr-xr-x   0 runner    (1001) docker     (127)    44739 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/media/73a1885c-089d-11ed-9389-747827182a82_image.png
--rwxr-xr-x   0 runner    (1001) docker     (127)    46908 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/media/810b9cba-089e-11ed-812e-747827182a82_image.png
--rwxr-xr-x   0 runner    (1001) docker     (127)        9 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/media/csf_conversion_version
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/view_report.nexdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 09:55:40.058143 ansys-dynamicreporting-core-0.5.1/tests/test_data/scenes/
--rwxr-xr-x   0 runner    (1001) docker     (127)    67100 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/scenes/proxy.png
--rwxr-xr-x   0 runner    (1001) docker     (127)  8331248 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/scenes/scene.avz
--rwxr-xr-x   0 runner    (1001) docker     (127)   218737 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_data/viewer_test.scdoc
--rwxr-xr-x   0 runner    (1001) docker     (127)     2585 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_download_html.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_encoders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3412 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_filelock.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3741 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_geofile_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1337 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_hacks.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10087 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_item.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3814 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    55683 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_report_objects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13113 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_report_remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6298 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_report_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    11189 2024-01-18 09:55:16.000000 ansys-dynamicreporting-core-0.5.1/tests/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.759607 ansys_dynamicreporting_core-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.719607 ansys_dynamicreporting_core-0.6.0/.ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.ci/pull_adr_image.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.719607 ansys_dynamicreporting_core-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.719607 ansys_dynamicreporting_core-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.github/workflows/ci_cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.github/workflows/nightly-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.github/workflows/nightly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-15 16:29:32.759607 ansys_dynamicreporting_core-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.723607 ansys_dynamicreporting_core-0.6.0/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/adr_utils.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/all_scrap_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20340 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/all_test_prop.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/pyadritem.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/read_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/codegen/rename_whl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.723607 ansys_dynamicreporting_core-0.6.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/.vale.ini
+-rwxr-xr-x   0 runner    (1001) docker     (127)      970 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.723607 ansys_dynamicreporting_core-0.6.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.727607 ansys_dynamicreporting_core-0.6.0/doc/source/_static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43416 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_complete_report_0.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    33601 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_create_db_0.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9619 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_create_db_1.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7820 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_create_db_2.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67994 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_connect_0.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67994 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_connect_1.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60479 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_connect_3.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46192 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_two_simulation_same_db_0.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45542 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_two_simulation_same_db_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)   103592 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/all_items.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9105 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/bar_plot.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31953 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/default_thumb.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9047 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/heatmap.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60188 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/img_item.PNG
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21115 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/line_plot.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28445 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/parallel_coord.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13051 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/pie_plot.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6081 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/sankey.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8025 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/simpletable.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4064 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/text_img.PNG
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5131 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_static/text_img_after.PNG
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.727607 ansys_dynamicreporting_core-0.6.0/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/class_documentation.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4630 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.727607 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.731607 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4185 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/00-create_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3862 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/01-connect.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7070 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/02-plottype.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      239 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.731607 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/25-intermediate/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2961 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/25-intermediate/00-tagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3792 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/25-intermediate/01-queries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      237 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/25-intermediate/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.731607 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/50-advanced/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15801 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/50-advanced/00-complete_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7536 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/50-advanced/01-two_simulation_same_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      211 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/50-advanced/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       77 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.731607 ansys_dynamicreporting_core-0.6.0/doc/source/gettingstarted/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5815 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/gettingstarted/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.731607 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11275 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/DataItemObject.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3220 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/DatasetandSessionObjects.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13142 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/GettingStarted.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13430 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/ServerObject.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58204 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/TemplateObjects.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)      637 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.735607 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27314 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem293.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28599 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem294.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14492 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem304.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    49403 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem305.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35137 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem306.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27128 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem307.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44203 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem308.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    94550 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem309.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    70692 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem310.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15728 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem311.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44941 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem312.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8196 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem313.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.735607 ansys_dynamicreporting_core-0.6.0/doc/source/userguide/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7177 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/source/userguide/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.735607 ansys_dynamicreporting_core-0.6.0/doc/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/styles/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.715607 ansys_dynamicreporting_core-0.6.0/doc/styles/Vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.735607 ansys_dynamicreporting_core-0.6.0/doc/styles/Vocab/ANSYS/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 16:29:32.759607 ansys_dynamicreporting_core-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.715607 ansys_dynamicreporting_core-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.715607 ansys_dynamicreporting_core-0.6.0/src/ansys/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.715607 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.735607 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    41698 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14301 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/docker_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.739607 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/extremely_ugly_hacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14907 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9945 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/geofile_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25732 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_download_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_download_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119749 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_objects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    71081 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_remote_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29810 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.755607 ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10763 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 16:29:32.000000 ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/test_cleanup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.743607 ansys_dynamicreporting_core-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3413 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.743607 ansys_dynamicreporting_core-0.6.0/tests/test_data/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42741 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/aa_00_0_alpha1.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56961 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/aa_00_0_u.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42648 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/aa_00_1_alpha1.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)   248887 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/ami.evsn
+-rwxr-xr-x   0 runner    (1001) docker     (127)    94256 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/dam_break.ens
+-rwxr-xr-x   0 runner    (1001) docker     (127)   368036 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/dam_break.mp4
+-rwxr-xr-x   0 runner    (1001) docker     (127)   502602 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/flow2d.csf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.747607 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   413696 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/db.sqlite3
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.747607 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/media/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44739 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/media/73a1885c-089d-11ed-9389-747827182a82_image.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    46908 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/media/810b9cba-089e-11ed-812e-747827182a82_image.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)        9 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/media/csf_conversion_version
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/view_report.nexdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 16:29:32.747607 ansys_dynamicreporting_core-0.6.0/tests/test_data/scenes/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    67100 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/scenes/proxy.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)  8331248 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/scenes/scene.avz
+-rwxr-xr-x   0 runner    (1001) docker     (127)   218737 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_data/viewer_test.scdoc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2585 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_download_html.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1088 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_encoders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3412 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_filelock.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3741 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_geofile_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1337 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_hacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10087 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_item.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3814 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55683 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_report_objects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13113 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_report_remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6298 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_report_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11189 2024-04-15 16:29:20.000000 ansys_dynamicreporting_core-0.6.0/tests/test_service.py
```

### Comparing `ansys-dynamicreporting-core-0.5.1/.flake8` & `ansys_dynamicreporting_core-0.6.0/.flake8`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/.github/workflows/ci_cd.yml` & `ansys_dynamicreporting_core-0.6.0/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/.github/workflows/nightly-docs.yml` & `ansys_dynamicreporting_core-0.6.0/.github/workflows/nightly-docs.yml`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/.github/workflows/nightly.yml` & `ansys_dynamicreporting_core-0.6.0/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/.gitignore` & `ansys_dynamicreporting_core-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/.pre-commit-config.yaml` & `ansys_dynamicreporting_core-0.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/CONTRIBUTING.rst` & `ansys_dynamicreporting_core-0.6.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/CONTRIBUTORS.md` & `ansys_dynamicreporting_core-0.6.0/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/LICENSE` & `ansys_dynamicreporting_core-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/Makefile` & `ansys_dynamicreporting_core-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/PKG-INFO` & `ansys_dynamicreporting_core-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-dynamicreporting-core
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python interface to Ansys Dynamic Reporting
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>, Ansys ADR Team <nexus@ansys.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansys/pydynamicreporting
 Project-URL: documentation, https://dynamicreporting.docs.pyansys.com/
 Project-URL: changelog, https://github.com/ansys/pydynamicreporting/blob/main/CHANGELOG.rst
@@ -25,15 +25,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: build>=0.8.0
 Requires-Dist: django>=3.2.10
 Requires-Dist: filelock>=3.7.1
-Requires-Dist: numpy>=1.18.0
+Requires-Dist: numpy<2,>=1.18.0
 Requires-Dist: packaging>=21.0
 Requires-Dist: docker>=6.1.0
 Requires-Dist: pypng>=0.20220715.0
 Requires-Dist: python-dateutil>=2.8.0
 Requires-Dist: pytz>=2021.3
 Requires-Dist: requests>=2.28.2
 Requires-Dist: twine>=4.0.1
```

### Comparing `ansys-dynamicreporting-core-0.5.1/README.rst` & `ansys_dynamicreporting_core-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/codegen/adr_utils.txt` & `ansys_dynamicreporting_core-0.6.0/codegen/adr_utils.txt`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/codegen/all_scrap_prop.py` & `ansys_dynamicreporting_core-0.6.0/codegen/all_scrap_prop.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/codegen/all_test_prop.xml` & `ansys_dynamicreporting_core-0.6.0/codegen/all_test_prop.xml`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/codegen/build_info.py` & `ansys_dynamicreporting_core-0.6.0/codegen/build_info.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/codegen/pyadritem.txt` & `ansys_dynamicreporting_core-0.6.0/codegen/pyadritem.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,400 +1,402 @@
-"""Item module.
-
-Module to create ``Item`` instances.
-
-Any object from an Ansys Dynamic Reporting database can be represented
-as an ``Item`` instance. This class allows for easy creation and manipulation
-of such objects.
-
-Examples
---------
-::
-
-    import ansys.dynamicreporting.core as adr
-    adr_service = Service()
-    ret = adr_service.connect()
-    my_img = adr_service.create_item()
-    my_img.item_image = 'Image_to_push_on_report'
-
-"""
-import os.path
-import requests
-import sys
-from typing import Optional
-
-from .adr_utils import in_ipynb, table_attr, type_maps
-import webbrowser
-
-try:
-    from IPython.display import IFrame
-except ImportError:
-    pass
-
-
-# Generate the items for the ADR database
-class Item:
-
-    """Provides for creating an object that represents an Ansys Dynamic Reporting item.
-
-    Create an instance of this class for each item in the database that you want to
-    interact with. When the object is created, no type is set. The type, determined the
-    first time that you set the ``item_*`` attribute, cannot be changed.
-
-    This code creates an instance with the object ``my_txt`` as a text item:
-
-    >>> my_txt = adr_service.create_item()
-    >>> my_txt.item_text = '<h1>The test</h1>This is a text item'
-
-
-    The type of the item created in the preceding code cannot be changed. However,
-    the attributes describing the object can be reset at any time. These hanges are
-    automatically propagated into the database. The attributes described in the
-    following "Parameters" section can be used to control the rendering of these objects.
-
-    .. note::
-       These attributes mirror the generic data item attributes described in
-       `Data Items`_ in the documentation for Ansys Dynamic Reporting.
-
-    .. _Data Items: https://nexusdemo.ensight.com/docs/html/Nexus.html?DataItems.html
-
-    Parameters
-    ----------
-    service : ansys.dynamicreporting.core.Service, optional
-        Ansys Dynamic Reporting object that provides the connection to the database
-        that the item is to interact with. The default is ``None``.
-    obj_name : str, optional
-        Name of the item object in the database. The default is ``default``.
-    source : str, optional
-        Name of the source for the item in the database. The default is ``"ADR"``.
-
-
-    Examples
-    --------
-    Initialize the ``Service`` class inside an Ansys Dynamic Reporting service and
-    create an object as a text item::
-
-        import ansys.dynamicreporting.core as adr
-        adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-        adr_service.connect(url='http://localhost:8010')
-        my_txt = adr_service.create_item()
-        my_txt.item_text = '<h1>The test</h1>This is a text item'
-
-    """
-
-    def __init__(self, service: 'ADR' = None, obj_name: Optional[str] = "default",
-                 source: Optional[str] = "ADR") -> None:
-        self.item = None
-        self.serverobj = service.serverobj
-        self._url = None
-        self.logger = service.logger
-        self.source = source
-        self.obj_name = str(obj_name)
-        self.type = None
-        self.item_text = ""
-        """Text (HTML and LaTeX formatting)"""
-        self.item_image = None
-        """Image object (Image and PNG binary files)"""
-        self.item_scene = None
-        """3D scene (AVZ, PLY, SCDOC, GLB, and STL files)"""
-        # Attributes for the table items
-        self.table_attr = table_attr
-        self.item_table = None
-        """Table values (Must be in a numpy array)"""
-        self.table_dict = {}
-        self.item = self.serverobj.create_item(name=self.obj_name, source=self.source)
-
-    @property
-    def url(self):
-        """URL corresponding to the item"""
-        if self.serverobj.get_URL() is not None and self.item.guid is not None:
-            self._url = self.serverobj.get_URL() + "/reports/report_display/?usemenus=off&query=A%7Ci_guid%7C%eq%7C"
-            self._url += str(self.item.guid)
-        else:
-            self._url = None
-        return self._url
-
-    def __pushonly__(self):
-        """
-        Push self to the server - with server existence check
-        """
-        ret = 0
-        if self._url is None:
-            _ = self.url
-        if self.serverobj is not None:
-            ret = self.serverobj.put_objects([self.item])
-        else:
-            self.logger.error("No connection to service established")
-        return ret
-
-    def __push__(self, value):
-        if self.type == "text":
-            self.item.set_payload_html(value)
-        elif self.type == "image":
-            # If the image is passed as a file, first open it. Otherwise, directly
-            # pass it as a payload value
-            if os.path.exists(value):
-                with open(value, "rb") as fb:
-                    img = fb.read()
-            else:
-                img = value
-            self.item.set_payload_image(img)
-        elif self.type == "scene":
-            self.item.set_payload_scene(value)
-        elif self.type == "table":
-            self.item.set_payload_table(self.table_dict)
-        elif self.type == "animation":
-            self.item.set_payload_animation(value)
-        elif self.type == "file":
-            self.item.set_payload_file(value)
-        elif self.type == "tree":
-            self.item.set_payload_tree(value)
-        _ = self.__pushonly__()
-
-    def __setattr__(self, name, value, only_set=False):
-        # If only_set is set to True, then skip the push methods. This is needed when using the
-        # setattr to create Item objs that correspond to what is in the database, but
-        # not to actually push changes to the database items - for example, when querying it
-        if name == "item":
-            super().__setattr__(name, value)
-            return 0
-        if self.item is None:
-            super().__setattr__(name, value)
-            return 0
-        if name in type_maps:
-            if self.type is None:
-                self.type = type_maps[name]
-            if self.type != type_maps[name]:
-                self.logger.error(f"Can not set {name} on an item of type: {self.type}")
-                return -1
-            if name == "item_table":
-                self.table_dict["array"] = value
-            if only_set is False:
-                self.__push__(value)
-        if name in self.table_attr:
-            if self.type == "table":
-                if value is not None:
-                    self.table_dict[name] = value
-                    if "array" in self.table_dict.keys():
-                        if only_set is False:
-                            self.__push__(value)
-        super().__setattr__(name, value)
-        return 0
-
-    def __copyattrs__(self, dataitem=None):
-        """
-        Copy the attributes from a data Item into the current Item
-        This is useful in the query method when creating a Item that corresponds to an existing
-        DataItem
-
-        Parameters
-        ----------
-        dataitem : utils.report_objects.ItemREST
-            ADR item to copy from. Default: None
-        """
-        if dataitem is None:
-            return
-        if dataitem.type == "table":
-            for t_attr in self.table_attr:
-                self.__setattr__(t_attr, dataitem.payloaddata.get(t_attr, None), only_set=True)
-
-    def visualize(self, new_tab: Optional[bool] = False) -> None:
-        """Render this item only.
-
-        Parameters
-        ----------
-        new_tab : bool, optional
-            Whether to render the item in a new tab if the current environment is a Jupyter
-            notebook. The default is ``False``, in which case the item is rendered in the
-            current location. If the environment is not a Jupyter notebook, the item is
-            always rendered in a new tab.
-
-        Returns
-        -------
-        Item
-            Rendered item.
-
-        Examples
-        --------
-        Create a text item and render it in a new tab::
-
-            import ansys.dynamicreporting.core as adr
-            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-            ret = adr_service.connect(url='http://localhost:8010')
-            my_txt = adr_service.create_item()
-            my_txt.item_text = '<h1>The test</h1>This is a text item'
-            my_txt.visualize(new_tab = True)
-
-
-        """
-        if in_ipynb() and not new_tab:
-            iframe = self.get_iframe()
-            if iframe is not None:
-                display(iframe)
-            else: # pragma: no cover
-                self.logger.error("Could not generate an IFrame")
-        else:
-            if self._url is None: # pragma: no cover
-                self.logger.error("Could not obtain a url")
-            else:
-                webbrowser.open_new(self._url)
-
-    def get_iframe(self, width=0, height=0):
-        """Get the iframe object corresponding to the item.
-
-        Parameters
-        ----------
-        width : int, optional
-            Width of the iframe object. The default is ``min(Item width * 1,1, 1000)``.
-            For example, if the item width is ``0``, the default is ``1000``.
-        height : int, optional
-            Height of the iframe object. The default is ``min(Item height, fixed height)``,
-            where the fixed height is ``800`` for an item scene and ``400`` otherwise.
-
-        Returns
-        -------
-        iframe
-            iframe object corresponding to the item. If no iframe can be generated,
-            ``None`` is returned.
-
-        Examples
-        --------
-        ::
-
-            import ansys.dynamicreporting.core as adr
-            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-            ret = adr_service.connect(url='http://localhost:8010')
-            my_txt = adr_service.create_item()
-            my_txt.item_text = '<h1>The test</h1>This is a text item'
-            item_iframe = my_txt.get_iframe()
-
-        """
-        if 'IPython.display' in sys.modules:
-            if width == 0:
-                if self.item.width == 0:
-                    width = 1000
-                else:
-                    width = min(self.item.width * 1.1, 1000)
-            if height == 0:
-                if self.type == "scene":
-                    height = 800
-                else:
-                    height = 400
-                if self.item.height > 0:
-                    height = min(self.item.height * 1.1, height)
-            iframe = IFrame(src=self._url, width=width, height=height)
-        else:
-            iframe = None
-        return iframe
-
-    def set_tags(self, tagstring: str = '') -> bool:
-        """Set tags on the item.
-
-        Parameters
-        ----------
-        tagstring : str, optional
-            Tags to set on the item. Separate multiple tags with a space. The
-            tag syntax is ``tagname=value``.
-
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-
-        Examples
-        --------
-        ::
-
-            import ansys.dynamicreporting.core as adr
-            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-            ret = adr_service.connect()
-            my_txt = adr_service.create_item()
-            my_txt.item_text = '<h1>The test</h1>This is a text item'
-            my_txt.set_tags("tagone=1 tagtwo=two")
-
-        """
-        self.item.set_tags(tagstring)
-        ret = self.__pushonly__()
-        return ret == requests.codes.ok
-
-    def get_tags(self) -> str:
-        """Get the tags on the item.
-
-        Returns
-        -------
-        str
-            Tags on the item.
-
-        Examples
-        --------
-        ::
-
-            import ansys.dynamicreporting.core as adr
-            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-            ret = adr_service.connect()
-            item_list = adr_service.query()
-            first_item = item_list[0]
-            all_tags = first_item.get_tags()
-
-        """
-        tags = self.item.get_tags()
-        return tags
-
-    def add_tag(self, tag: str = '', value: str = '') -> bool:
-        """Add a tag to the item.
-
-        Parameters
-        ----------
-        tag : str, optional
-            Tag name. The default is ``""``.
-        value str : str, optional
-            Tag value.  The default is ``""``.
-
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-
-        Examples
-        --------
-        ::
-
-            import ansys.dynamicreporting.core as adr
-            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-            ret = adr_service.connect()
-            my_txt = adr_service.create_item()
-            my_txt.item_text = '<h1>The test</h1>This is a text item'
-            my_txt.add_tag(tag='tagone', value='one')
-
-        """
-        self.item.add_tag(tag=tag, value=value)
-        ret = self.__pushonly__()
-        return ret == requests.codes.ok
-
-    def rem_tag(self, tag: str = '') -> bool:
-        """Remove a tag on the item.
-
-        Parameters
-        ----------
-        tag : str, optional
-            Tag to remove. The default is ``""``.
-
-        Returns
-        -------
-        bool
-            ``True`` when successful, ``False`` when failed.
-
-        Examples
-        --------
-        ::
-
-            import ansys.dynamicreporting.core as adr
-            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
-            ret = adr_service.connect()
-            item_list = adr_service.query()
-            first_item = item_list[0]
-            all_tags = first_item.rem_tags(tag='tagone')
-
-        """
-        self.item.rem_tag(tag=tag)
-        ret = self.__pushonly__()
-        return ret == requests.codes.ok
+"""Item module.
+
+Module to create ``Item`` instances.
+
+Any object from an Ansys Dynamic Reporting database can be represented
+as an ``Item`` instance. This class allows for easy creation and manipulation
+of such objects.
+
+Examples
+--------
+::
+
+    import ansys.dynamicreporting.core as adr
+    adr_service = Service()
+    ret = adr_service.connect()
+    my_img = adr_service.create_item()
+    my_img.item_image = 'Image_to_push_on_report'
+
+"""
+import os.path
+import requests
+import sys
+from typing import Optional
+
+from .adr_utils import in_ipynb, table_attr, type_maps
+import webbrowser
+
+try:
+    from IPython.display import IFrame
+except ImportError:
+    pass
+
+
+# Generate the items for the ADR database
+class Item:
+
+    """Provides for creating an object that represents an Ansys Dynamic Reporting item.
+
+    Create an instance of this class for each item in the database that you want to
+    interact with. When the object is created, no type is set. The type, determined the
+    first time that you set the ``item_*`` attribute, cannot be changed.
+
+    This code creates an instance with the object ``my_txt`` as a text item:
+
+    >>> my_txt = adr_service.create_item()
+    >>> my_txt.item_text = '<h1>The test</h1>This is a text item'
+
+
+    The type of the item created in the preceding code cannot be changed. However,
+    the attributes describing the object can be reset at any time. These hanges are
+    automatically propagated into the database. The attributes described in the
+    following "Parameters" section can be used to control the rendering of these objects.
+
+    .. note::
+       These attributes mirror the generic data item attributes described in
+       `Data Items`_ in the documentation for Ansys Dynamic Reporting.
+
+    .. _Data Items: https://nexusdemo.ensight.com/docs/html/Nexus.html?DataItems.html
+
+    Parameters
+    ----------
+    service : ansys.dynamicreporting.core.Service, optional
+        Ansys Dynamic Reporting object that provides the connection to the database
+        that the item is to interact with. The default is ``None``.
+    obj_name : str, optional
+        Name of the item object in the database. The default is ``default``.
+    source : str, optional
+        Name of the source for the item in the database. The default is ``"ADR"``.
+
+
+    Examples
+    --------
+    Initialize the ``Service`` class inside an Ansys Dynamic Reporting service and
+    create an object as a text item::
+
+        import ansys.dynamicreporting.core as adr
+        adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+        adr_service.connect(url='http://localhost:8010')
+        my_txt = adr_service.create_item()
+        my_txt.item_text = '<h1>The test</h1>This is a text item'
+
+    """
+
+    def __init__(self, service: 'ADR' = None, obj_name: Optional[str] = "default",
+                 source: Optional[str] = "ADR") -> None:
+        self.item = None
+        self.serverobj = service.serverobj
+        self._url = None
+        self.logger = service.logger
+        self.source = source
+        self.obj_name = str(obj_name)
+        self.type = None
+        self.item_text = ""
+        """Text (HTML and LaTeX formatting)"""
+        self.item_image = None
+        """Image object (Image and PNG binary files)"""
+        self.item_scene = None
+        """3D scene (AVZ, PLY, SCDOC, GLB, and STL files)"""
+        self.item_animation = None
+        """Animation file (MP4/H.264 format files)"""
+        # Attributes for the table items
+        self.table_attr = table_attr
+        self.item_table = None
+        """Table values (Must be in a numpy array)"""
+        self.table_dict = {}
+        self.item = self.serverobj.create_item(name=self.obj_name, source=self.source)
+
+    @property
+    def url(self):
+        """URL corresponding to the item"""
+        if self.serverobj.get_URL() is not None and self.item.guid is not None:
+            self._url = self.serverobj.get_URL() + "/reports/report_display/?usemenus=off&query=A%7Ci_guid%7C%eq%7C"
+            self._url += str(self.item.guid)
+        else:
+            self._url = None
+        return self._url
+
+    def __pushonly__(self):
+        """
+        Push self to the server - with server existence check
+        """
+        ret = 0
+        if self._url is None:
+            _ = self.url
+        if self.serverobj is not None:
+            ret = self.serverobj.put_objects([self.item])
+        else:
+            self.logger.error("No connection to service established")
+        return ret
+
+    def __push__(self, value):
+        if self.type == "text":
+            self.item.set_payload_html(value)
+        elif self.type == "image":
+            # If the image is passed as a file, first open it. Otherwise, directly
+            # pass it as a payload value
+            if os.path.exists(value):
+                with open(value, "rb") as fb:
+                    img = fb.read()
+            else:
+                img = value
+            self.item.set_payload_image(img)
+        elif self.type == "scene":
+            self.item.set_payload_scene(value)
+        elif self.type == "table":
+            self.item.set_payload_table(self.table_dict)
+        elif self.type == "animation":
+            self.item.set_payload_animation(value)
+        elif self.type == "file":
+            self.item.set_payload_file(value)
+        elif self.type == "tree":
+            self.item.set_payload_tree(value)
+        _ = self.__pushonly__()
+
+    def __setattr__(self, name, value, only_set=False):
+        # If only_set is set to True, then skip the push methods. This is needed when using the
+        # setattr to create Item objs that correspond to what is in the database, but
+        # not to actually push changes to the database items - for example, when querying it
+        if name == "item":
+            super().__setattr__(name, value)
+            return 0
+        if self.item is None:
+            super().__setattr__(name, value)
+            return 0
+        if name in type_maps:
+            if self.type is None:
+                self.type = type_maps[name]
+            if self.type != type_maps[name]:
+                self.logger.error(f"Can not set {name} on an item of type: {self.type}")
+                return -1
+            if name == "item_table":
+                self.table_dict["array"] = value
+            if only_set is False:
+                self.__push__(value)
+        if name in self.table_attr:
+            if self.type == "table":
+                if value is not None:
+                    self.table_dict[name] = value
+                    if "array" in self.table_dict.keys():
+                        if only_set is False:
+                            self.__push__(value)
+        super().__setattr__(name, value)
+        return 0
+
+    def __copyattrs__(self, dataitem=None):
+        """
+        Copy the attributes from a data Item into the current Item
+        This is useful in the query method when creating a Item that corresponds to an existing
+        DataItem
+
+        Parameters
+        ----------
+        dataitem : utils.report_objects.ItemREST
+            ADR item to copy from. Default: None
+        """
+        if dataitem is None:
+            return
+        if dataitem.type == "table":
+            for t_attr in self.table_attr:
+                self.__setattr__(t_attr, dataitem.payloaddata.get(t_attr, None), only_set=True)
+
+    def visualize(self, new_tab: Optional[bool] = False) -> None:
+        """Render this item only.
+
+        Parameters
+        ----------
+        new_tab : bool, optional
+            Whether to render the item in a new tab if the current environment is a Jupyter
+            notebook. The default is ``False``, in which case the item is rendered in the
+            current location. If the environment is not a Jupyter notebook, the item is
+            always rendered in a new tab.
+
+        Returns
+        -------
+        Item
+            Rendered item.
+
+        Examples
+        --------
+        Create a text item and render it in a new tab::
+
+            import ansys.dynamicreporting.core as adr
+            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+            ret = adr_service.connect(url='http://localhost:8010')
+            my_txt = adr_service.create_item()
+            my_txt.item_text = '<h1>The test</h1>This is a text item'
+            my_txt.visualize(new_tab = True)
+
+
+        """
+        if in_ipynb() and not new_tab:
+            iframe = self.get_iframe()
+            if iframe is not None:
+                display(iframe)
+            else: # pragma: no cover
+                self.logger.error("Could not generate an IFrame")
+        else:
+            if self._url is None: # pragma: no cover
+                self.logger.error("Could not obtain a url")
+            else:
+                webbrowser.open_new(self._url)
+
+    def get_iframe(self, width=0, height=0):
+        """Get the iframe object corresponding to the item.
+
+        Parameters
+        ----------
+        width : int, optional
+            Width of the iframe object. The default is ``min(Item width * 1,1, 1000)``.
+            For example, if the item width is ``0``, the default is ``1000``.
+        height : int, optional
+            Height of the iframe object. The default is ``min(Item height, fixed height)``,
+            where the fixed height is ``800`` for an item scene and ``400`` otherwise.
+
+        Returns
+        -------
+        iframe
+            iframe object corresponding to the item. If no iframe can be generated,
+            ``None`` is returned.
+
+        Examples
+        --------
+        ::
+
+            import ansys.dynamicreporting.core as adr
+            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+            ret = adr_service.connect(url='http://localhost:8010')
+            my_txt = adr_service.create_item()
+            my_txt.item_text = '<h1>The test</h1>This is a text item'
+            item_iframe = my_txt.get_iframe()
+
+        """
+        if 'IPython.display' in sys.modules:
+            if width == 0:
+                if self.item.width == 0:
+                    width = 1000
+                else:
+                    width = min(self.item.width * 1.1, 1000)
+            if height == 0:
+                if self.type == "scene":
+                    height = 800
+                else:
+                    height = 400
+                if self.item.height > 0:
+                    height = min(self.item.height * 1.1, height)
+            iframe = IFrame(src=self._url, width=width, height=height)
+        else:
+            iframe = None
+        return iframe
+
+    def set_tags(self, tagstring: str = '') -> bool:
+        """Set tags on the item.
+
+        Parameters
+        ----------
+        tagstring : str, optional
+            Tags to set on the item. Separate multiple tags with a space. The
+            tag syntax is ``tagname=value``.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        Examples
+        --------
+        ::
+
+            import ansys.dynamicreporting.core as adr
+            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+            ret = adr_service.connect()
+            my_txt = adr_service.create_item()
+            my_txt.item_text = '<h1>The test</h1>This is a text item'
+            my_txt.set_tags("tagone=1 tagtwo=two")
+
+        """
+        self.item.set_tags(tagstring)
+        ret = self.__pushonly__()
+        return ret == requests.codes.ok
+
+    def get_tags(self) -> str:
+        """Get the tags on the item.
+
+        Returns
+        -------
+        str
+            Tags on the item.
+
+        Examples
+        --------
+        ::
+
+            import ansys.dynamicreporting.core as adr
+            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+            ret = adr_service.connect()
+            item_list = adr_service.query()
+            first_item = item_list[0]
+            all_tags = first_item.get_tags()
+
+        """
+        tags = self.item.get_tags()
+        return tags
+
+    def add_tag(self, tag: str = '', value: str = '') -> bool:
+        """Add a tag to the item.
+
+        Parameters
+        ----------
+        tag : str, optional
+            Tag name. The default is ``""``.
+        value str : str, optional
+            Tag value.  The default is ``""``.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        Examples
+        --------
+        ::
+
+            import ansys.dynamicreporting.core as adr
+            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+            ret = adr_service.connect()
+            my_txt = adr_service.create_item()
+            my_txt.item_text = '<h1>The test</h1>This is a text item'
+            my_txt.add_tag(tag='tagone', value='one')
+
+        """
+        self.item.add_tag(tag=tag, value=value)
+        ret = self.__pushonly__()
+        return ret == requests.codes.ok
+
+    def rem_tag(self, tag: str = '') -> bool:
+        """Remove a tag on the item.
+
+        Parameters
+        ----------
+        tag : str, optional
+            Tag to remove. The default is ``""``.
+
+        Returns
+        -------
+        bool
+            ``True`` when successful, ``False`` when failed.
+
+        Examples
+        --------
+        ::
+
+            import ansys.dynamicreporting.core as adr
+            adr_service = adr.Service(ansys_installation = r'C:\\Program Files\\ANSYS Inc\\v232')
+            ret = adr_service.connect()
+            item_list = adr_service.query()
+            first_item = item_list[0]
+            all_tags = first_item.rem_tags(tag='tagone')
+
+        """
+        self.item.rem_tag(tag=tag)
+        ret = self.__pushonly__()
+        return ret == requests.codes.ok
```

### Comparing `ansys-dynamicreporting-core-0.5.1/codegen/read_prop.py` & `ansys_dynamicreporting_core-0.6.0/codegen/read_prop.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/.vale.ini` & `ansys_dynamicreporting_core-0.6.0/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/Makefile` & `ansys_dynamicreporting_core-0.6.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/make.bat` & `ansys_dynamicreporting_core-0.6.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_complete_report_0.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_complete_report_0.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_create_db_0.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_create_db_0.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_create_db_1.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_create_db_1.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/00_create_db_2.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/00_create_db_2.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_connect_0.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_connect_0.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_connect_1.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_connect_1.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_connect_3.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_connect_3.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_two_simulation_same_db_0.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_two_simulation_same_db_0.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/01_two_simulation_same_db_1.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/01_two_simulation_same_db_1.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/all_items.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/all_items.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/bar_plot.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/bar_plot.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/default_thumb.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/default_thumb.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/heatmap.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/heatmap.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/img_item.PNG` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/img_item.PNG`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/line_plot.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/line_plot.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/parallel_coord.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/parallel_coord.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/pie_plot.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/pie_plot.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/sankey.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/sankey.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/simpletable.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/simpletable.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/text_img.PNG` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/text_img.PNG`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/_static/text_img_after.PNG` & `ansys_dynamicreporting_core-0.6.0/doc/source/_static/text_img_after.PNG`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/class_documentation.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/class_documentation.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/conf.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/contributing.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/00-create_db.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/00-create_db.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/01-connect.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/01-connect.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/00-basic/02-plottype.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/00-basic/02-plottype.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/25-intermediate/00-tagging.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/25-intermediate/00-tagging.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/25-intermediate/01-queries.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/25-intermediate/01-queries.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/50-advanced/00-complete_report.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/50-advanced/00-complete_report.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/examples_source/50-advanced/01-two_simulation_same_db.py` & `ansys_dynamicreporting_core-0.6.0/doc/source/examples_source/50-advanced/01-two_simulation_same_db.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/gettingstarted/index.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/gettingstarted/index.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/index.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/DataItemObject.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/DataItemObject.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/DatasetandSessionObjects.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/DatasetandSessionObjects.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/GettingStarted.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/GettingStarted.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/ServerObject.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/ServerObject.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/TemplateObjects.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/TemplateObjects.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/index.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/index.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem293.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem293.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem294.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem294.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem304.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem304.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem305.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem305.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem306.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem306.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem307.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem307.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem308.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem308.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem309.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem309.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem310.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem310.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem311.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem311.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem312.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem312.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/lowlevelapi/lib/NewItem313.png` & `ansys_dynamicreporting_core-0.6.0/doc/source/lowlevelapi/lib/NewItem313.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/doc/source/userguide/index.rst` & `ansys_dynamicreporting_core-0.6.0/doc/source/userguide/index.rst`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/pyproject.toml` & `ansys_dynamicreporting_core-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools>=45.0",
     "setuptools-scm",
     "wheel>=0.37.0",
 ]
 
 [project]
 name = "ansys-dynamicreporting-core"
-version = "0.5.1"
+version = "0.6.0"
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
 maintainers = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
     {name = "Ansys ADR Team", email = "nexus@ansys.com"},
 ]
@@ -33,15 +33,15 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "build>=0.8.0",
     "django>=3.2.10",
     "filelock>=3.7.1",
-    "numpy>=1.18.0",
+    "numpy>=1.18.0,<2",
     "packaging>=21.0",
     "docker>=6.1.0",
     "pypng>=0.20220715.0",
     "python-dateutil>=2.8.0",
     "pytz>=2021.3",
     "requests>=2.28.2",
     "twine>=4.0.1",
```

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/__init__.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_item.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,16 @@
         self.type = None
         self.item_text = ""
         """Text (HTML and LaTeX formatting)"""
         self.item_image = None
         """Image object (Image and PNG binary files)"""
         self.item_scene = None
         """3D scene (AVZ, PLY, SCDOC, GLB, and STL files)"""
+        self.item_animation = None
+        """Animation file (MP4/H.264 format files)"""
         # Attributes for the table items
         self.table_attr = table_attr
         self.item_table = None
         """Table values (Must be in a numpy array)"""
         self.table_dict = {}
         self.format = None
         """Number format
```

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_report.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_report.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_service.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     ret = adr_service.connect()
     my_img = adr_service.create_item()
     my_img.item_image = 'Image_to_push_on_report'
     adr_service.visualize_report()
 """
 
 import atexit
+import glob
 import os
 import re
 import shutil
 import tempfile
 import time
 from typing import Optional
 
@@ -121,22 +122,22 @@
     ) -> None:
         """
         Initialize an Ansys Dynamic Reporting object.
 
         Parameters
         ----------
         ansys_installation : str, optional
-            Locatation of the Ansys installation, including the version directory.
+            Location of the Ansys installation, including the version directory.
             For example, r'C:\\Program Files\\ANSYS Inc\\v232'. The default is
             ``None``. This parameter is needed only if the Service instance is
             to launch a dynamic Reporting service. It is not needed if connecting
             to an existing service. If there is no local Ansys installation and
             a Docker image is to be used instead, enter ``"docker"``.
         docker_image : str, optional
-            Location of the Docker image for Ansys Dynamic Reporting. The defaults
+            Location of the Docker image for Ansys Dynamic Reporting. The default
             is ghcr.io/ansys-internal/nexus. This parameter is used only if the
             value for the ``ansys_installation`` parameter is set to ``"docker"``.
             Default:
         data_directory: str, optional
             Directory where Docker is to store temporary copy of files. The
             default is ``None``, in which case ``TMP_DIR`` is used. This parameter
             is used only if the value for the ``ansys_installation`` parameter
@@ -216,47 +217,93 @@
                     db_directory=self._db_directory,
                     port=self._port,
                 )
             except Exception as e:  # pragma: no cover
                 self.logger.error(f"Error starting the Docker Container.\n{str(e)}\n")
                 raise e
 
-        elif ansys_installation:  # pragma: no cover
-            # verify path
-            if not os.path.isdir(ansys_installation):
-                raise InvalidAnsysPath(ansys_installation)
-
-        if ansys_installation != "docker" and ansys_installation is not None:  # pragma: no cover
-            # Not using docker
-            # Backward compatibility: if the path passed is only up to the version directory,
-            # append the CEI directory
-            if ansys_installation.endswith("CEI") is False:
-                ansys_installation = os.path.join(ansys_installation, "CEI")
-                self._ansys_installation = ansys_installation
-                # verify new path
-                if not os.path.isdir(ansys_installation):
-                    # Option for local development build
-                    if os.environ.get("CEIDEVROOTDOS") is not None:
-                        self._ansys_installation = os.environ.get("CEIDEVROOTDOS")
-                    else:
-                        raise InvalidAnsysPath(ansys_installation)
-            if self._ansys_version is None:
-                # try to get version from install path
-                matches = re.search(r".*v([0-9]{3}).*", self._ansys_installation)
-                if matches is None:
-                    # Option for local development build
-                    if os.environ.get("ANSYS_REL_INT_I") is not None:
-                        self._ansys_version = int(os.environ.get("ANSYS_REL_INT_I"))
+        else:  # pragma: no cover
+            # Not using docker. Make a list of directory names to consider:
+            # 1) any passed ansys_installation directory
+            # 2) any passed ansys_installation directory with 'CEI' dir appended
+            # 3) the 'enve.home()' directory (if enve will load)
+            # 4) the latest ansys installation via AWP_ROOTxyz environmental variable
+            # 5) CEIDEVROOTDOS environmental variable
+            #
+            dirs_to_check = []
+            if ansys_installation:
+                dirs_to_check.append(ansys_installation)
+                dirs_to_check.append(os.path.join(ansys_installation, "CEI"))
+
+            # if we are running from a distro "EnSight" cpython, enve might be there
+            try:
+                import enve
+
+                dirs_to_check.append(enve.home())
+            except ModuleNotFoundError:
+                pass
+
+            # Find via AWP_ROOTxyz envvar...  Most recent version installed
+            env_name = "AWP_ROOT000"
+            for name in os.environ.keys():
+                if name.startswith("AWP_ROOT"):
+                    env_name = max(env_name, name)
+            if env_name in os.environ:
+                # add AWP_ROOT{max}/CEI to the list of directories to search
+                dirs_to_check.append(os.path.join(os.environ[env_name], "CEI"))
+
+            # Option for local development build
+            if os.environ.get("CEIDEVROOTDOS") is not None:
+                dirs_to_check.append(os.environ.get("CEIDEVROOTDOS"))
+
+            # Check all the potential local directories for the distro
+            # bin/cpython should be in the server distro
+            found = False
+            for install_dir in dirs_to_check:
+                cpython_name = os.path.join(install_dir, "bin", "cpython")
+                if os.path.isfile(cpython_name):
+                    self._ansys_installation = install_dir
+                    found = True
+                    break
+
+            # Should we raise an exception here?  If no ansys_installation was
+            # passed, then no but the user can only connect to existing servers
+            # as per docs.  If ansys_installation was passed, then there is an
+            # exception if the passed value is not the root of the installation.
+            # Basically, the passed install path was illegal.
+            if ansys_installation:
+                if not self._ansys_installation.startswith(ansys_installation):
+                    raise InvalidAnsysPath(ansys_installation)
+            if not found:
+                self._ansys_installation = None
+            else:
+                # populate the version number
+                if self._ansys_version is None:
+                    # An ansys distro include a v??? directory name.  This is the fallback.
+                    matches = re.search(r".*v([0-9]{3}).*", self._ansys_installation)
+                    # Try to get version from install path bin\cei_python??? name
+                    # Build the cpython path glob name:
+                    cpython_glob = os.path.join(
+                        self._ansys_installation, "bin", "cpython[0-9][0-9][0-9]"
+                    )
+                    cpython_name = glob.glob(cpython_glob)
+                    # is the file there (it should be...)
+                    if len(cpython_name):
+                        matches = re.search(r".*cpython([0-9]{3})", cpython_name[0])
+                    if matches is None:
+                        # Option for local development build
+                        if "ANSYS_REL_INT_I" in os.environ:
+                            self._ansys_version = int(os.environ.get("ANSYS_REL_INT_I"))
+                        else:
+                            raise AnsysVersionAbsentError
                     else:
-                        raise AnsysVersionAbsentError
-                else:
-                    try:
-                        self._ansys_version = int(matches.group(1))
-                    except IndexError:
-                        raise AnsysVersionAbsentError
+                        try:
+                            self._ansys_version = int(matches.group(1))
+                        except IndexError:
+                            raise AnsysVersionAbsentError
 
     @property
     def session_guid(self):
         """GUID of the session associated with the service."""
         if self._session_guid == "":
             self.logger.error("No session attached to this instance.")
             raise MissingSession
```

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/adr_utils.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/adr_utils.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/docker_support.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/docker_support.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/exceptions.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/encoders.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/exceptions.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/extremely_ugly_hacks.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/extremely_ugly_hacks.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/filelock.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/filelock.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/geofile_processing.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/geofile_processing.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_download_html.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_download_html.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_download_pdf.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_download_pdf.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_objects.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_objects.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_remote_server.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_remote_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1075,17 +1075,14 @@
                 group = Group.objects.create(name="nexus")
                 for p in Permission.objects.all():
                     group.permissions.add(p)
                 # and the nexus user
                 group.user_set.add(user)
                 group.save()
                 os.makedirs(os.path.join(db_dir, "media"))
-                from ansys.nexus.core.geofile_processing import do_geometry_update_check
-
-                do_geometry_update_check()
             except Exception:
                 error = True
             if parent and has_qt:
                 QtWidgets.QApplication.restoreOverrideCursor()
             # Unset the environmental vars...
             os.environ.pop("CEI_NEXUS_SECRET_KEY")
             os.environ.pop("CEI_NEXUS_LOCAL_DB_DIR")
```

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys/dynamicreporting/core/utils/report_utils.py` & `ansys_dynamicreporting_core-0.6.0/src/ansys/dynamicreporting/core/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/PKG-INFO` & `ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-dynamicreporting-core
-Version: 0.5.1
+Version: 0.6.0
 Summary: Python interface to Ansys Dynamic Reporting
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>, Ansys ADR Team <nexus@ansys.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansys/pydynamicreporting
 Project-URL: documentation, https://dynamicreporting.docs.pyansys.com/
 Project-URL: changelog, https://github.com/ansys/pydynamicreporting/blob/main/CHANGELOG.rst
@@ -25,15 +25,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS
 Requires-Dist: build>=0.8.0
 Requires-Dist: django>=3.2.10
 Requires-Dist: filelock>=3.7.1
-Requires-Dist: numpy>=1.18.0
+Requires-Dist: numpy<2,>=1.18.0
 Requires-Dist: packaging>=21.0
 Requires-Dist: docker>=6.1.0
 Requires-Dist: pypng>=0.20220715.0
 Requires-Dist: python-dateutil>=2.8.0
 Requires-Dist: pytz>=2021.3
 Requires-Dist: requests>=2.28.2
 Requires-Dist: twine>=4.0.1
```

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/SOURCES.txt` & `ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/src/ansys_dynamicreporting_core.egg-info/requires.txt` & `ansys_dynamicreporting_core-0.6.0/src/ansys_dynamicreporting_core.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 build>=0.8.0
 django>=3.2.10
 filelock>=3.7.1
-numpy>=1.18.0
+numpy<2,>=1.18.0
 packaging>=21.0
 docker>=6.1.0
 pypng>=0.20220715.0
 python-dateutil>=2.8.0
 pytz>=2021.3
 requests>=2.28.2
 twine>=4.0.1
```

### Comparing `ansys-dynamicreporting-core-0.5.1/test_cleanup.py` & `ansys_dynamicreporting_core-0.6.0/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/conftest.py` & `ansys_dynamicreporting_core-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/aa_00_0_alpha1.png` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/aa_00_0_alpha1.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/aa_00_0_u.png` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/aa_00_0_u.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/aa_00_1_alpha1.png` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/aa_00_1_alpha1.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/ami.evsn` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/ami.evsn`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/dam_break.ens` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/dam_break.ens`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/dam_break.mp4` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/dam_break.mp4`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/flow2d.csf` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/flow2d.csf`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/db.sqlite3` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/db.sqlite3`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/media/73a1885c-089d-11ed-9389-747827182a82_image.png` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/media/73a1885c-089d-11ed-9389-747827182a82_image.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/query_db/media/810b9cba-089e-11ed-812e-747827182a82_image.png` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/query_db/media/810b9cba-089e-11ed-812e-747827182a82_image.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/scenes/proxy.png` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/scenes/proxy.png`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/scenes/scene.avz` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/scenes/scene.avz`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_data/viewer_test.scdoc` & `ansys_dynamicreporting_core-0.6.0/tests/test_data/viewer_test.scdoc`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_download_html.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_download_html.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_encoders.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_filelock.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_geofile_processing.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_geofile_processing.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_hacks.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_hacks.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_item.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_report.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_report_objects.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_report_objects.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_report_remote_server.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_report_remote_server.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_report_utils.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_report_utils.py`

 * *Files identical despite different names*

### Comparing `ansys-dynamicreporting-core-0.5.1/tests/test_service.py` & `ansys_dynamicreporting_core-0.6.0/tests/test_service.py`

 * *Files identical despite different names*

