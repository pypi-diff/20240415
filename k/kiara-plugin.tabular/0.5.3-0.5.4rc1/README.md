# Comparing `tmp/kiara_plugin.tabular-0.5.3.tar.gz` & `tmp/kiara_plugin_tabular-0.5.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.tabular-0.5.3.tar", last modified: Fri Dec 29 11:37:54 2023, max compression
+gzip compressed data, was "kiara_plugin_tabular-0.5.4rc1.tar", last modified: Mon Apr 15 14:10:11 2024, max compression
```

## Comparing `kiara_plugin.tabular-0.5.3.tar` & `kiara_plugin_tabular-0.5.4rc1.tar`

### file list

```diff
@@ -1,161 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.781557 kiara_plugin.tabular-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      815 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      342 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2023-12-29 11:37:54.781557 kiara_plugin.tabular-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)    33121 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.765557 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.769557 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16793 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18280 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18481 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18620 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18698 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18540 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.769557 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/
--rw-r--r--   0 runner    (1001) docker     (127)    19397 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20647 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20650 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21017 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20982 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.769557 kiara_plugin.tabular-0.5.3/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/assemble_tables_1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/assemble_tables_2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/assemble_tables_3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/corpus_onboarding_small.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/create_table_from_file.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/create_tables_from_file_bundle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/import_journal_nodes_table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/pick_column_from_tables.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/jobs/pick_table_from_tables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.769557 kiara_plugin.tabular-0.5.3/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/pipelines/corpus_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/pipelines/database_from_csv_files.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/pipelines/init.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/examples/pipelines/tables_from_csv_files.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/pixi.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.769557 kiara_plugin.tabular-0.5.3/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-29 11:37:54.781557 kiara_plugin.tabular-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.757557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     6860 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/array/
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/array/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/db/
--rw-r--r--   0 runner    (1001) docker     (127)    21619 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/table/
--rw-r--r--   0 runner    (1001) docker     (127)    25406 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/table/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.773557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/tables/
--rw-r--r--   0 runner    (1001) docker     (127)    16968 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      124 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      641 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    17114 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/utils/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2023-12-29 11:37:54.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2023-12-29 11:37:54.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-29 11:37:54.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-12-29 11:37:54.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-12-29 11:37:54.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-29 11:37:54.000000 kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.761557 kiara_plugin.tabular-0.5.3/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/assemble_tables_1/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/assemble_tables_1/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/assemble_tables_2/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/assemble_tables_2/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/assemble_tables_3/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/assemble_tables_3/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/corpus_onboarding_small/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/corpus_onboarding_small/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/create_table_from_file/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/create_table_from_file/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/create_tables_from_file_bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/create_tables_from_file_bundle/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/create_tables_from_file_bundle/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/import_journal_nodes_table/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/import_journal_nodes_table/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/pick_column_from_tables/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/pick_column_from_tables/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/job_tests/pick_table_from_tables/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/job_tests/pick_table_from_tables/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:54.777557 kiara_plugin.tabular-0.5.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2023-12-29 11:37:45.000000 kiara_plugin.tabular-0.5.3/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.706406 kiara_plugin_tabular-0.5.4rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.706406 kiara_plugin_tabular-0.5.4rc1/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.714406 kiara_plugin_tabular-0.5.4rc1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    33121 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.706406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/
+-rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16793 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18280 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18481 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18620 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18698 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18540 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.718406 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/
+-rw-r--r--   0 runner    (1001) docker     (127)    19397 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20647 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20650 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21017 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20982 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/assemble_tables_1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/assemble_tables_2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/assemble_tables_3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/corpus_onboarding_small.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/create_table_from_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/create_tables_from_file_bundle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/import_journal_nodes_table.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/pick_column_from_tables.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/jobs/pick_table_from_tables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/corpus_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/database_from_csv_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/import.table.from.local_folder_path_ignore_errors.json
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/init.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/examples/pipelines/tables_from_csv_files.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/pixi.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.722406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6860 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/array/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/db/
+-rw-r--r--   0 runner    (1001) docker     (127)    21619 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/
+-rw-r--r--   0 runner    (1001) docker     (127)    26251 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/tables/
+-rw-r--r--   0 runner    (1001) docker     (127)    16968 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    17114 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5170 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-15 14:10:11.000000 kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.710406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.726406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_1/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_1/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_2/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_2/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_3/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/assemble_tables_3/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/corpus_onboarding_small/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/corpus_onboarding_small/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_table_from_file/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_table_from_file/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/import_journal_nodes_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/import_journal_nodes_table/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_column_from_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_column_from_tables/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_table_from_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/job_tests/pick_table_from_tables/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/resources/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/resources/jobs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:11.730406 kiara_plugin_tabular-0.5.4rc1/tests/resources/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/resources/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-04-15 14:10:06.000000 kiara_plugin_tabular-0.5.4rc1/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.tabular-0.5.3/.cruft.json` & `kiara_plugin_tabular-0.5.4rc1/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'61841496d46e8ce4f79da1126443524bde03f977'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "96e37df1692a56068082857a41318dc7d17f1643",
+    "commit": "61841496d46e8ce4f79da1126443524bde03f977",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.tabular-0.5.3/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin_tabular-0.5.4rc1/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/.github/workflows/build-darwin.yaml` & `kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-darwin.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   test-darwin:
     name: pytest on darwin
     runs-on: macos-11
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.tabular
```

### Comparing `kiara_plugin.tabular-0.5.3/.github/workflows/build-linux.yaml` & `kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-linux.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 #      - uses: wagoid/commitlint-github-action@v4
 
   test-linux:
     name: pytest on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.tabular
@@ -51,15 +51,15 @@
           parallel-finished: true
 
   mypy-linux:
     name: mypy check on linux
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.tabular
```

### Comparing `kiara_plugin.tabular-0.5.3/.github/workflows/build-windows.yaml` & `kiara_plugin_tabular-0.5.4rc1/.github/workflows/build-windows.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 jobs:
   test-windows:
     name: pytest on windows
     runs-on: windows-latest
     strategy:
       matrix:
-        python_version: ["3.8", "3.9", "3.10", "3.11"]
+        python_version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
     steps:
       - name: "Set up Python ${{ matrix.python_version }}"
         uses: actions/setup-python@v4
         with:
           python-version: "${{ matrix.python_version }}"
       - uses: actions/checkout@v3
       - name: install kiara_plugin.tabular
```

### Comparing `kiara_plugin.tabular-0.5.3/.gitignore` & `kiara_plugin_tabular-0.5.4rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/.pre-commit-config.yaml` & `kiara_plugin_tabular-0.5.4rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/LICENSE` & `kiara_plugin_tabular-0.5.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/Makefile` & `kiara_plugin_tabular-0.5.4rc1/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/PKG-INFO` & `kiara_plugin_tabular-0.5.4rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.tabular
-Version: 0.5.3
+Version: 0.5.4rc1
 Summary: kiara data-types and modules for working with tables and databases.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.tabular
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Keywords: kiara
@@ -19,28 +19,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.9
-Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.0
-Requires-Dist: duckdb<0.10.0,>=0.9.0
+Requires-Dist: kiara<0.6.0,>=0.5.10rc10
+Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1rc1
+Requires-Dist: duckdb<0.11.0,>=0.10.0
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: polars>=0.18.0
 Requires-Dist: pyarrow>=12.0.0
 Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: sqlalchemy-utc>=0.10.0
 Requires-Dist: sqlalchemy-utils>=0.38.0
 Requires-Dist: sqlite-utils==3.30
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
-Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
+Requires-Dist: kiara[dev_testing]==0.5.10rc10; extra == "dev-testing"
 Requires-Dist: pandas-stubs; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
 Provides-Extra: dev-all
 Requires-Dist: kiara[dev_all]; extra == "dev-all"
 Provides-Extra: streamlit
 Requires-Dist: kiara_plugin.streamlit; extra == "streamlit"
```

### Comparing `kiara_plugin.tabular-0.5.3/README.md` & `kiara_plugin_tabular-0.5.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/docs/index.md` & `kiara_plugin_tabular-0.5.4rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin_tabular-0.5.4rc1/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-04-25_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-05_ed-4_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Ragione/sn84037024_1917-05-16_ed-3_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-07_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-14_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-1_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt` & `kiara_plugin_tabular-0.5.4rc1/examples/data/text_corpus/data/La_Rassegna/sn84037025_1917-04-21_ed-2_seq-1_ocr.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/jobs/init.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/jobs/init.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/pipelines/corpus_onboarding.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/corpus_onboarding.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/pipelines/database_from_csv_files.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/database_from_csv_files.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/pipelines/init.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/init.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/examples/pipelines/tables_from_csv_files.yaml` & `kiara_plugin_tabular-0.5.4rc1/examples/pipelines/tables_from_csv_files.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/mkdocs.yml` & `kiara_plugin_tabular-0.5.4rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/pixi.toml` & `kiara_plugin_tabular-0.5.4rc1/pixi.toml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/pyproject.toml` & `kiara_plugin_tabular-0.5.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "kiara>=0.5.9,<0.6.0",
-    "kiara_plugin.core_types>=0.5.0,<0.6.0",
-    "duckdb>=0.9.0,<0.10.0",
+    "kiara>=0.5.10rc10,<0.6.0",
+    "kiara_plugin.core_types>=0.5.1rc1,<0.6.0",
+    "duckdb>=0.10.0,<0.11.0",
     "pandas>=1.4.0",
     "polars>=0.18.0",
     "pyarrow>=12.0.0",
     "sqlalchemy>=2.0.0",
     "sqlalchemy-utc>=0.10.0",
     "sqlalchemy-utils>=0.38.0",
     "sqlite-utils==3.30",
@@ -61,15 +61,15 @@
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
 dev_testing = [
-    "kiara[dev_testing]",
+    "kiara[dev_testing]==0.5.10rc10",
     "pandas-stubs"
 ]
 dev_utils = [
     "kiara[dev_utils]",
 ]
 dev_all = [
     "kiara[dev_all]"
```

### Comparing `kiara_plugin.tabular-0.5.3/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/scripts/documentation/gen_info_pages.py` & `kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/scripts/documentation/gen_module_doc.py` & `kiara_plugin_tabular-0.5.4rc1/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/array.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     """Utility methdo to stora an array to a file."""
 
     import pyarrow as pa
     from pyarrow import ChunkedArray
 
     schema = pa.schema([pa.field(column_name, array_obj.type)])
 
+    os.makedirs(os.path.dirname(file_name), exist_ok=True)
+
     # TODO: support non-single chunk columns
     with pa.OSFile(file_name, "wb") as sink:
         with pa.ipc.new_file(sink, schema=schema) as writer:
             if isinstance(array_obj, ChunkedArray):
                 for chunk in array_obj.chunks:
                     batch = pa.record_batch([chunk], schema=schema)
                     writer.write(batch)
```

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/db.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/db.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/table.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/table.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/data_types/tables.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/data_types/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             for column_name in arrow_table.column_names:
                 if not column_name:
                     raise Exception(
                         f"column name for table '{table_id}' is empty. This is not allowed."
                     )
 
                 column: pa.Array = arrow_table.column(column_name)
-                file_name = os.path.join(temp_f, column_name)
+                file_name = os.path.join(temp_f, table_id, column_name)
                 store_array(
                     array_obj=column, file_name=file_name, column_name=column_name
                 )
                 chunk_map[f"{table_id}{TABLE_COLUMN_SPLIT_MARKER}{column_name}"] = {
                     "type": "file",
                     "file": file_name,
                     "codec": "raw",
```

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/defaults.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/array.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/array.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/db.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/db.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/table.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/table.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/models/tables.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/models/tables.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/array/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/array/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/db/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/db/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/table/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 # -*- coding: utf-8 -*-
 import os
-from typing import Any, Dict, Iterable, List, Mapping, Type, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Mapping,
+    Type,
+    Union,
+)
 
 from pydantic import BaseModel, Field
 
 from kiara.exceptions import KiaraProcessingException
 from kiara.models.filesystem import (
     FILE_BUNDLE_IMPORT_AVAILABLE_COLUMNS,
     KiaraFile,
@@ -27,14 +37,17 @@
 from kiara_plugin.tabular.defaults import (
     RESERVED_SQL_KEYWORDS,
     TABLE_SCHEMA_CHUNKS_NAME,
 )
 from kiara_plugin.tabular.models.array import KiaraArray
 from kiara_plugin.tabular.models.table import KiaraTable
 
+if TYPE_CHECKING:
+    from multiformats.varint import BytesLike
+
 EMPTY_COLUMN_NAME_MARKER = "__no_column_name__"
 
 
 class CreateTableModuleConfig(CreateFromModuleConfig):
 
     ignore_errors: bool = Field(
         description="Whether to ignore convert errors and omit the failed items.",
@@ -223,16 +236,20 @@
     def to__python_object(self, data: SerializedData, **config: Any):
 
         import pyarrow as pa
 
         columns = {}
 
         table_schema_chunks = data.get_serialized_data(TABLE_SCHEMA_CHUNKS_NAME)
-        chunks_generator = table_schema_chunks.get_chunks(as_files=False)
-        schema_chunk = next(chunks_generator)  # type: ignore
+        chunks_generator: Generator[
+            "BytesLike", None, None
+        ] = table_schema_chunks.get_chunks(
+            as_files=False
+        )  # type: ignore
+        schema_chunk = next(chunks_generator)
         schema = pa.ipc.read_schema(pa.py_buffer(schema_chunk))
 
         for column_name in data.get_keys():
 
             if column_name == TABLE_SCHEMA_CHUNKS_NAME:
                 continue
 
@@ -365,14 +382,34 @@
 
     Column names of the resulting table can be controlled by the 'column_map' configuration, which takes the
     desired column name as key, and a field-name in the following format as value:
     - '[inputs_schema key]' for inputs of type 'array'
     - '[inputs_schema_key].orig_column_name' for inputs of type 'table'
     """
 
+    # @classmethod
+    # def retrieve_included_operations(cls):
+    #
+    #     return {
+    #         "table.add_column": {
+    #             "module_config": {
+    #                 "inputs_schema": {
+    #                     "table": {
+    #                         "type": "table",
+    #                         "doc": "The table to add the column to.",
+    #                     },
+    #                     "column": {
+    #                         "type": "array",
+    #                         "doc": "The column to add.",
+    #                     }
+    #                 }
+    #             }
+    #         }
+    #     }
+
     _module_type_name = "table.merge"
     _config_cls = MergeTableConfig
 
     def create_inputs_schema(
         self,
     ) -> ValueMapSchema:
```

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/table/filters.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/table/filters.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/modules/tables/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/modules/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.yaml` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.yaml` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.yaml` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.yaml` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/utils/__init__.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin/tabular/utils/tables.py` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin/tabular/utils/tables.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/PKG-INFO` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.tabular
-Version: 0.5.3
+Version: 0.5.4rc1
 Summary: kiara data-types and modules for working with tables and databases.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.tabular
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.tabular
 Keywords: kiara
@@ -19,28 +19,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
-Requires-Dist: kiara<0.6.0,>=0.5.9
-Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.0
-Requires-Dist: duckdb<0.10.0,>=0.9.0
+Requires-Dist: kiara<0.6.0,>=0.5.10rc10
+Requires-Dist: kiara_plugin.core_types<0.6.0,>=0.5.1rc1
+Requires-Dist: duckdb<0.11.0,>=0.10.0
 Requires-Dist: pandas>=1.4.0
 Requires-Dist: polars>=0.18.0
 Requires-Dist: pyarrow>=12.0.0
 Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: sqlalchemy-utc>=0.10.0
 Requires-Dist: sqlalchemy-utils>=0.38.0
 Requires-Dist: sqlite-utils==3.30
 Provides-Extra: dev-documentation
 Requires-Dist: kiara[dev_documentation]; extra == "dev-documentation"
 Provides-Extra: dev-testing
-Requires-Dist: kiara[dev_testing]; extra == "dev-testing"
+Requires-Dist: kiara[dev_testing]==0.5.10rc10; extra == "dev-testing"
 Requires-Dist: pandas-stubs; extra == "dev-testing"
 Provides-Extra: dev-utils
 Requires-Dist: kiara[dev_utils]; extra == "dev-utils"
 Provides-Extra: dev-all
 Requires-Dist: kiara[dev_all]; extra == "dev-all"
 Provides-Extra: streamlit
 Requires-Dist: kiara_plugin.streamlit; extra == "streamlit"
```

### Comparing `kiara_plugin.tabular-0.5.3/src/kiara_plugin.tabular.egg-info/SOURCES.txt` & `kiara_plugin_tabular-0.5.4rc1/src/kiara_plugin.tabular.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 examples/jobs/import_journal_nodes_table.yaml
 examples/jobs/init.yaml
 examples/jobs/pick_column_from_tables.yaml
 examples/jobs/pick_table_from_tables.yaml
 examples/pipelines/Readme.md
 examples/pipelines/corpus_onboarding.yaml
 examples/pipelines/database_from_csv_files.yaml
+examples/pipelines/import.table.from.local_folder_path_ignore_errors.json
 examples/pipelines/init.yaml
 examples/pipelines/tables_from_csv_files.yaml
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.tabular.egg-info/PKG-INFO
 src/kiara_plugin.tabular.egg-info/SOURCES.txt
@@ -87,18 +88,18 @@
 src/kiara_plugin/tabular/modules/array/__init__.py
 src/kiara_plugin/tabular/modules/db/__init__.py
 src/kiara_plugin/tabular/modules/table/__init__.py
 src/kiara_plugin/tabular/modules/table/filters.py
 src/kiara_plugin/tabular/modules/tables/__init__.py
 src/kiara_plugin/tabular/pipelines/.gitkeep
 src/kiara_plugin/tabular/pipelines/__init__.py
-src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.yaml
-src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.yaml
-src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.yaml
-src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.yaml
+src/kiara_plugin/tabular/pipelines/extract_date_array.from.table.json
+src/kiara_plugin/tabular/pipelines/import.database.from.local_file_path.json
+src/kiara_plugin/tabular/pipelines/import.table.from.local_file_path.json
+src/kiara_plugin/tabular/pipelines/import.table.from.local_folder_path.json
 src/kiara_plugin/tabular/resources/.gitkeep
 src/kiara_plugin/tabular/utils/__init__.py
 src/kiara_plugin/tabular/utils/tables.py
 tests/conftest.py
 tests/test_job_descs.py
 tests/test_kiara_modules_default.py
 tests/job_tests/assemble_tables_1/outputs.yaml
@@ -107,8 +108,10 @@
 tests/job_tests/corpus_onboarding_small/outputs.yaml
 tests/job_tests/create_table_from_file/outputs.yaml
 tests/job_tests/create_tables_from_file_bundle/outputs.py
 tests/job_tests/create_tables_from_file_bundle/outputs.yaml
 tests/job_tests/import_journal_nodes_table/outputs.yaml
 tests/job_tests/pick_column_from_tables/outputs.yaml
 tests/job_tests/pick_table_from_tables/outputs.yaml
-tests/resources/.gitkeep
+tests/resources/.gitkeep
+tests/resources/jobs/.gitkeep
+tests/resources/pipelines/.gitkeep
```

### Comparing `kiara_plugin.tabular-0.5.3/tests/conftest.py` & `kiara_plugin_tabular-0.5.4rc1/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 import os
 import tempfile
 import uuid
 from pathlib import Path
 
 import pytest
 
+from kiara.api import JobDesc, KiaraAPI
 from kiara.context import KiaraConfig
-from kiara.interfaces.python_api import KiaraAPI
-from kiara.interfaces.python_api.models.job import JobDesc, JobTest
+from kiara.interfaces.python_api.models.job import JobTest
 from kiara.utils.testing import get_init_job, get_tests_for_job, list_job_descs
 
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
@@ -50,30 +53,36 @@
 
 @pytest.fixture
 def kiara_api_init_example() -> KiaraAPI:
     instance_path = create_temp_dir()
     kc = KiaraConfig.create_in_folder(instance_path)
     api = KiaraAPI(kc)
 
-    init_job = get_init_job(JOBS_FOLDER)
-    if init_job is None:
+    init_jobs = []
+    for jobs_folder in JOBS_FOLDERS:
+        init_job = get_init_job(jobs_folder)
+        if init_job is not None:
+            init_jobs.append(init_job)
+
+    if not init_jobs:
         return api
 
-    results = api.run_job(init_job)
+    for init_job in init_jobs:
+        results = api.run_job(init_job, comment="Init example job")
 
-    if not init_job.save:
-        return api
+        if not init_job.save:
+            continue
 
-    for field_name, alias_name in init_job.save.items():
-        api.store_value(results[field_name], alias_name)
+        for field_name, alias_name in init_job.save.items():
+            api.store_value(results[field_name], alias_name)
 
     return api
 
 
-@pytest.fixture(params=list_job_descs(JOBS_FOLDER), ids=get_job_alias)
+@pytest.fixture(params=list_job_descs(JOBS_FOLDERS), ids=get_job_alias)
 def example_job_test(request, kiara_api_init_example) -> JobTest:
 
     job_tests_folder = Path(os.path.join(ROOT_DIR, "tests", "job_tests"))
 
     job_desc = request.param
 
     tests = get_tests_for_job(
```

### Comparing `kiara_plugin.tabular-0.5.3/tests/job_tests/create_tables_from_file_bundle/outputs.py` & `kiara_plugin_tabular-0.5.4rc1/tests/job_tests/create_tables_from_file_bundle/outputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.tabular-0.5.3/tests/test_job_descs.py` & `kiara_plugin_tabular-0.5.4rc1/tests/test_job_descs.py`

 * *Files identical despite different names*

