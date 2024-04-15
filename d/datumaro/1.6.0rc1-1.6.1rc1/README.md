# Comparing `tmp/datumaro-1.6.0rc1.tar.gz` & `tmp/datumaro-1.6.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.6.0rc1.tar", last modified: Fri Jan 12 02:42:38 2024, max compression
+gzip compressed data, was "datumaro-1.6.1rc1.tar", last modified: Mon Apr 15 10:06:35 2024, max compression
```

## Comparing `datumaro-1.6.0rc1.tar` & `datumaro-1.6.1rc1.tar`

### file list

```diff
@@ -1,395 +1,396 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)   391964 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/requirements-default.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.764831 datumaro-1.6.0rc1/rust/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/rust/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/coco_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/datum_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/json_section_page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/page_mapper.rs
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/page_maps.rs
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/rust/src/utils.rs
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.756832 datumaro-1.6.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.768831 datumaro-1.6.0rc1/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.772832 datumaro-1.6.0rc1/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     9340 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.772832 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.772832 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.776831 datumaro-1.6.0rc1/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.780831 datumaro-1.6.0rc1/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.780831 datumaro-1.6.0rc1/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.780831 datumaro-1.6.0rc1/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (127)    34942 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    25024 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/contexts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/contexts/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (127)    34020 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    25867 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12351 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18272 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14443 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (127)    15442 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    41283 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.784832 datumaro-1.6.0rc1/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    14069 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (127)    89834 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    23625 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.788832 datumaro-1.6.0rc1/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.788832 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.788832 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/configurable_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.792832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (127)     8693 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17705 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (127)    12457 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)    21483 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24679 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.796832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19062 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12137 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (127)     8357 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13499 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.800832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (127)    15150 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mmdet.py
--rw-r--r--   0 runner    (1001) docker     (127)     9234 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     5151 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    38738 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.804832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9098 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    15663 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.808832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13949 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/framework_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.812832 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    49095 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.816832 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.820832 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    49413 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.820832 datumaro-1.6.0rc1/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12679 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/import_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12034 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/multi_procs_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8494 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-12 02:42:30.000000 datumaro-1.6.0rc1/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-12 02:42:38.824832 datumaro-1.6.0rc1/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7752 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-12 02:42:38.000000 datumaro-1.6.0rc1/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.620596 datumaro-1.6.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)   393113 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-15 10:06:35.620596 datumaro-1.6.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/requirements-default.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.556596 datumaro-1.6.1rc1/rust/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.560596 datumaro-1.6.1rc1/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6711 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/coco_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/datum_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/json_section_page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/page_mapper.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/page_maps.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/rust/src/utils.rs
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:06:35.620596 datumaro-1.6.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.548596 datumaro-1.6.1rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.560596 datumaro-1.6.1rc1/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.560596 datumaro-1.6.1rc1/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.560596 datumaro-1.6.1rc1/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.564596 datumaro-1.6.1rc1/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10170 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.564596 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.564596 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5924 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.568596 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8383 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.568596 datumaro-1.6.1rc1/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.568596 datumaro-1.6.1rc1/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2553 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.568596 datumaro-1.6.1rc1/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.572596 datumaro-1.6.1rc1/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13546 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8957 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36472 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34148 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7574 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26104 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9843 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14785 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19922 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14541 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19999 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)    15576 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8271 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41468 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.576596 datumaro-1.6.1rc1/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24403 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14387 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89550 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.580596 datumaro-1.6.1rc1/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.580596 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.580596 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15491 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/anchor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37755 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/configurable_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.588596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8831 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.588596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.588596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.588596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17865 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.592596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10889 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.592596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24813 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33535 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6915 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.592596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21501 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.592596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18239 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19062 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.596596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11209 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.596596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6297 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.596596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12539 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4261 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8073 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/imagenet_txt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.596596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kaggle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kaggle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kaggle/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.596596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11401 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.600596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17906 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15274 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.600596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11577 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6603 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11120 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.600596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.600596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38893 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.600596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10251 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.604596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6062 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.604596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7215 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.604596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6671 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.604596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15800 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.604596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16675 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31405 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10734 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.608596 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14467 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/framework_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.608596 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.608596 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16787 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.608596 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.612596 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.612596 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7810 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.612596 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8109 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.612596 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.612596 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51884 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32124 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.612596 datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.616596 datumaro-1.6.1rc1/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50015 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45116 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.616596 datumaro-1.6.1rc1/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13348 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/import_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14465 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/multi_procs_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8833 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4702 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 10:06:31.000000 datumaro-1.6.1rc1/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:06:35.620596 datumaro-1.6.1rc1/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 10:06:35.000000 datumaro-1.6.1rc1/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.6.0rc1/3rd-party.txt` & `datumaro-1.6.1rc1/3rd-party.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7295,10 +7295,22 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 -------------------------------------------------------------
+imagesize_py
 
+MIT
+
+Copyright © 2016 Yoshiki Shibukawa
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+-------------------------------------------------------------
 
 * Other names and brands may be claimed as the property of others.
```

### Comparing `datumaro-1.6.0rc1/LICENSE` & `datumaro-1.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/PKG-INFO` & `datumaro-1.6.1rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.0rc1
+Version: 1.6.1rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: defusedxml>=0.7.0
 Requires-Dist: h5py>=2.10.0
-Requires-Dist: lxml>=4.4.1
+Requires-Dist: imagesize>=1.4.1
+Requires-Dist: lxml==5.2.0
 Requires-Dist: matplotlib>=3.3.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: nibabel>=3.2.1
-Requires-Dist: numpy>=1.17.3
-Requires-Dist: orjson>=3.6.6
-Requires-Dist: Pillow>=6.1.0
+Requires-Dist: numpy<2,>=1.23.4
+Requires-Dist: orjson==3.10.0
+Requires-Dist: Pillow==10.3.0
 Requires-Dist: ruamel.yaml>=0.17.0
 Requires-Dist: shapely>=1.7
 Requires-Dist: typing_extensions>=3.7.4.3
 Requires-Dist: tqdm
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
-Requires-Dist: PyYAML>=5.3.1
+Requires-Dist: PyYAML==6.0.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
-Requires-Dist: pandas>=1.1.5
-Requires-Dist: openvino>=2023.2.0
+Requires-Dist: pandas~=1.4.0
+Requires-Dist: openvino<2024.0.0,>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
-Requires-Dist: protobuf<4
+Requires-Dist: protobuf
 Requires-Dist: tabulate
 Requires-Dist: ovmsclient
 Requires-Dist: tritonclient[all]
 Requires-Dist: scikit-learn
 Requires-Dist: json-stream
 Requires-Dist: opencv-python
 Provides-Extra: tf
@@ -51,15 +52,15 @@
 Requires-Dist: tensorflow-datasets<4.9.3; extra == "tfds"
 Provides-Extra: tf-gpu
 Requires-Dist: tensorflow-gpu; extra == "tf-gpu"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: torchvision; extra == "torch"
 Provides-Extra: default
-Requires-Dist: dvc==3.30.1; extra == "default"
+Requires-Dist: dvc==3.49.0; extra == "default"
 Requires-Dist: fsspec<=2022.11.0; python_version < "3.8" and extra == "default"
 Requires-Dist: GitPython!=3.1.25,>=3.1.18; extra == "default"
 Requires-Dist: openvino-telemetry>=2022.1.0; extra == "default"
 Requires-Dist: openvino-dev>=2023.2.0; extra == "default"
 
 # Dataset Management Framework (Datumaro)
```

### Comparing `datumaro-1.6.0rc1/README.md` & `datumaro-1.6.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/pyproject.toml` & `datumaro-1.6.1rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "src/datumaro/__main__.py",
     "src/datumaro/version.py",
     "tests/*",
 ]
 
 [tool.cibuildwheel]
 # reference docs - https://cibuildwheel.readthedocs.io/en/stable/options/#build-skip
-build = "cp38-*_x86_64 cp39-*_x86_64 cp310-*_x86_64 cp311-*_x86_64 cp38-*_amd64 cp39-*_amd64 cp310-*_amd64 cp311-*_amd64"
+build = "cp39-*_x86_64 cp310-*_x86_64 cp311-*_x86_64 cp39-*_amd64 cp310-*_amd64 cp311-*_amd64"
 skip = "*macos*"
 
 [tool.cibuildwheel.linux]
 before-all = [
     "curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs -o rustup-init.sh",
     "sh ./rustup-init.sh -y --default-toolchain stable --profile minimal"
 ]
@@ -59,15 +59,15 @@
 # don't fail on the code that can be found
 ignore_errors = true
 
 skip_empty = true
 
 [tool.black]
 line-length = 100
-target-version = ['py38']
+target-version = ['py310']
 
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F"]
 
 # Need to review all ignore items below
 ignore = [
@@ -114,15 +114,15 @@
 # Same as Black.
 line-length = 120
 
 # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 # minimum target version
-target-version = "py38"
+target-version = "py39"
 
 # ignore-init-module-imports = true
 
 [tool.ruff.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
```

### Comparing `datumaro-1.6.0rc1/requirements-core.txt` & `datumaro-1.6.1rc1/requirements-core.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 attrs>=21.3.0
 defusedxml>=0.7.0
 h5py>=2.10.0
-lxml>=4.4.1
+imagesize>=1.4.1
+lxml==5.2.0
 matplotlib>=3.3.1
 networkx>=2.6
 nibabel>=3.2.1
-numpy>=1.17.3
-orjson>=3.6.6
-Pillow>=6.1.0
+numpy<2,>=1.23.4
+orjson==3.10.0
+Pillow==10.3.0
 ruamel.yaml>=0.17.0
 shapely>=1.7
 typing_extensions>=3.7.4.3
 tqdm
 
 pycocotools>=2.0.4; platform_system != "Windows" or python_version >= '3.9'
 
 pycocotools-windows; platform_system == "Windows" and python_version < '3.9'
-PyYAML>=5.3.1
+PyYAML==6.0.1
 
 # 2.3 has an unlisted dependency on PyTorch, which we don't need
 tensorboardX>=1.8,!=2.3
 
 # Builtin plugin dependencies
 
 # NDR
 scipy
 
 # Image generator
 requests
 
 # Sampler
-pandas>=1.1.5
+pandas~=1.4.0
 
 # OpenVINO
-openvino>=2023.2.0
+openvino>=2023.2.0,<2024.0.0 # Accuracy checker is deprecated >=2024.0.0
 tokenizers
 
 # Encryption
 cryptography>= 38.03
 
 # Shift analyzer
 pyemd
 
 # apache arrow
 pyarrow
 
 # ava data format
-protobuf<4
+protobuf
 
 # Comparator
 tabulate
 
 # Model inference launcher from the dedicated inference server
 ovmsclient
 tritonclient[all]
```

### Comparing `datumaro-1.6.0rc1/rust/src/coco_page_mapper.rs` & `datumaro-1.6.1rc1/rust/src/coco_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/rust/src/datum_page_mapper.rs` & `datumaro-1.6.1rc1/rust/src/datum_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/rust/src/json_section_page_mapper.rs` & `datumaro-1.6.1rc1/rust/src/json_section_page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/rust/src/lib.rs` & `datumaro-1.6.1rc1/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/rust/src/page_mapper.rs` & `datumaro-1.6.1rc1/rust/src/page_mapper.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/rust/src/page_maps.rs` & `datumaro-1.6.1rc1/rust/src/page_maps.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/rust/src/utils.rs` & `datumaro-1.6.1rc1/rust/src/utils.rs`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/setup.py` & `datumaro-1.6.1rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src", include=["datumaro*"]),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     install_requires=CORE_REQUIREMENTS,
     extras_require={
         "tf": ["tensorflow"],
         "tfds": ["tensorflow-datasets<4.9.3"],
         "tf-gpu": ["tensorflow-gpu"],
         "torch": ["torch", "torchvision"],
         "default": DEFAULT_REQUIREMENTS,
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,24 +47,24 @@
     CategoriesInfo,
     DatasetBase,
     DatasetItem,
     IDataset,
     SubsetBase,
 )
 from .components.dataset_item_storage import ItemStatus
-from .components.environment import Environment, PluginRegistry
+from .components.environment import Environment
 from .components.exporter import Exporter, ExportErrorPolicy, FailingExportErrorPolicy
 from .components.hl_ops import HLOps
 from .components.importer import FailingImportErrorPolicy, Importer, ImportErrorPolicy
 from .components.launcher import Launcher
 from .components.media import Image, MediaElement, Video, VideoFrame
-from .components.media_manager import MediaManager
 from .components.progress_reporting import (
     NullProgressReporter,
     ProgressReporter,
     SimpleProgressReporter,
     TQDMProgressReporter,
 )
+from .components.registry import PluginRegistry
 from .components.transformer import ItemTransform, ModelTransform, Transform
 from .components.validator import Validator
 from .components.visualizer import Visualizer
 from .version import __version__
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/capi/pybind.cpp` & `datumaro-1.6.1rc1/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/__main__.py` & `datumaro-1.6.1rc1/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/compare.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/convert.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             )
             return 2
 
         fmt = matches[0]
         log.info(f"Source dataset format detected as {fmt}")
 
     if fmt == args.output_format:
-        log.error("The source data format and the output data format is same as {fmt}.")
+        log.error(f"The source data format and the output data format is same as {fmt}.")
         return 3
 
     source = osp.abspath(args.source)
 
     dst_dir = args.dst_dir
     if dst_dir:
         if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/download.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/explain.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/explain.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         See explanations at: https://arxiv.org/pdf/1806.07421.pdf
         """,
         formatter_class=MultilineFormatter,
     )
     rise_parser.add_argument(
         "-s",
         "--max-samples",
-        default=None,
+        default=100,
         type=int,
         help="Number of algorithm iterations (default: mask size ^ 2)",
     )
     rise_parser.add_argument(
         "--mw",
         "--mask-width",
         dest="mask_width",
@@ -199,21 +199,17 @@
     if str(args.algorithm).lower() != "rise":
         raise CliException("Explanation algorithm except for rise is not yet implemented.")
 
     from datumaro.components.algorithms.rise import RISE
 
     rise = RISE(
         model,
-        max_samples=args.max_samples,
-        mask_width=args.mask_width,
-        mask_height=args.mask_height,
+        num_masks=args.max_samples,
+        mask_size=args.mask_width,
         prob=args.prob,
-        iou_thresh=args.iou_thresh,
-        nms_thresh=args.nms_iou_thresh,
-        det_conf_thresh=args.det_conf_thresh,
         batch_size=args.batch_size,
     )
 
     if args.target and is_image(args.target):
         image_path = args.target
         image = load_image(image_path)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/explore.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/explore.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
-import os.path as osp
 import shutil
 import uuid
 
 from datumaro.components.algorithms.hash_key_inference.explorer import Explorer
 from datumaro.components.algorithms.hash_key_inference.hashkey_util import (
     check_and_convert_to_list,
     match_query_subset,
@@ -85,14 +84,21 @@
         "-s",
         "--save",
         action="store_true",
         default=False,
         help="Save explorer result files on explore_result folder",
     )
     parser.add_argument(
+        "-o",
+        "--output-dir",
+        dest="dst_dir",
+        default=None,
+        help="Directory to save explore results " "(default: generate automatically)",
+    )
+    parser.add_argument(
         "--stage",
         type=str_to_bool,
         default=True,
         help="""
             Include this action as a project build step.
             If true, this operation will be saved in the project
             build tree, allowing to reproduce the resulting dataset later.
@@ -108,14 +114,15 @@
 
 def get_sensitive_args():
     return {
         explore_command: [
             "target",
             "topk",
             "project_dir",
+            "dst_dir",
         ]
     }
 
 
 @scoped
 def explore_command(args):
     project = None
@@ -126,30 +133,28 @@
             raise
 
     if args.target:
         targets = [args.target]
     else:
         targets = list(project.working_tree.sources)
 
-    source_datasets = []
-    for target in targets:
-        target_dataset, _ = parse_full_revpath(target, project)
-        source_datasets.append(target_dataset)
+    source_datasets = [parse_full_revpath(target, project)[0] for target in targets]
 
     explorer_args = {"save_hashkey": True}
-    build_tree = project.working_tree.clone()
-    for target in targets:
-        build_tree.build_targets.add_explore_stage(target, params=explorer_args)
+    if project:
+        build_tree = project.working_tree.clone()
+        for target in targets:
+            build_tree.build_targets.add_explore_stage(target, params=explorer_args)
 
     explorer = Explorer(*source_datasets)
     for dataset in source_datasets:
         dst_dir = dataset.data_path
         dataset.save(dst_dir, save_media=True, save_hashkey_meta=True)
 
-    if args.stage:
+    if args.stage and project:
         project.working_tree.config.update(build_tree.config)
         project.working_tree.save()
 
     if args.query_img_path:
         querys = check_and_convert_to_list(args.query_img_path)
         query_datasetitems = []
         for query_ in querys:
@@ -175,18 +180,18 @@
     log.info(f"Most similar {args.topk} results of query in dataset")
     for result in results:
         path = getattr(result.media, "path", None)
         result_path_list.append(path)
         log.info(f"id: {result.id} | subset: {result.subset} | path : {path}")
 
     if args.save:
-        saved_result_path = osp.join(args.project_dir, "explore_result")
-        if osp.exists(saved_result_path):
+        saved_result_path = args.dst_dir or os.path.join(args.project_dir, "explore_result")
+        if os.path.exists(saved_result_path):
             shutil.rmtree(saved_result_path)
         os.makedirs(saved_result_path)
         for result in results:
-            saved_subset_path = osp.join(saved_result_path, result.subset)
-            if not osp.exists(saved_subset_path):
+            saved_subset_path = os.path.join(saved_result_path, result.subset)
+            if not os.path.exists(saved_subset_path):
                 os.makedirs(saved_subset_path)
-            shutil.copyfile(path, osp.join(saved_subset_path, result.id + ".jpg"))
+            shutil.copyfile(path, os.path.join(saved_subset_path, result.id + ".jpg"))
 
     return 0
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/filter.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/generate.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/info.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/merge.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/patch.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/prune.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/prune.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
+import os.path as osp
 
 from datumaro.components.algorithms.hash_key_inference.prune import Prune
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.project import load_project, parse_full_revpath
@@ -41,15 +42,21 @@
         |s|s%(prog)s -m query_clust -h img -r 0.5|
         - Prune dataset based on entropy with clustering in image hash and ratio 50%:|n
         |s|s%(prog)s -m entropy -h img -r 0.5|
         """,
         formatter_class=MultilineFormatter,
     )
 
-    parser.add_argument("target", nargs="?", help="Target dataset revpath (default: project)")
+    parser.add_argument(
+        "target",
+        nargs="?",
+        default="project",
+        metavar="revpath",
+        help="Target dataset revpath (default: project)",
+    )
     parser.add_argument("-m", "--method", dest="method", help="Method to apply to the dataset")
     parser.add_argument(
         "-r", "--ratio", type=float, dest="ratio", help="How much to remain dataset after pruning"
     )
     parser.add_argument(
         "--hash-type",
         type=str,
@@ -106,16 +113,16 @@
             raise
 
     targets = [args.target] if args.target else list(project.working_tree.sources)
 
     source_dataset = [parse_full_revpath(target, project)[0] for target in targets][0]
 
     prune = Prune(source_dataset, cluster_method=args.method, hash_type=args.hash_type)
-
-    source_dataset.save(source_dataset.data_path, save_media=True, save_hashkey_meta=True)
-
     result = prune.get_pruned(args.ratio)
 
     dst_dir = args.dst_dir or source_dataset.data_path
+    dst_dir = (
+        dst_dir if dst_dir else osp.join(args.project_dir, list(project.working_tree.sources)[0])
+    )
     result.save(dst_dir, save_media=True)
 
     log.info("Results have been saved to '%s'" % dst_dir)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/stats.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
         help="Get project statistics",
         description="""
-        Outputs various project statistics like image mean and std,
+        Outputs various project statistics like image mean and std (RGB),
         annotations count etc.|n
         |n
         Target dataset is specified by a revpath. The full syntax is:|n
         - Dataset paths:|n
         |s|s- <dataset path>[ :<format> ]|n
         - Revision paths:|n
         |s|s- <project path> [ @<rev> ] [ :<target> ]|n
@@ -50,15 +50,15 @@
         "target", default="project", nargs="?", help="Target dataset revpath (default: project)"
     )
     parser.add_argument("-s", "--subset", help="Compute stats only for a specific subset")
     parser.add_argument(
         "--image-stats",
         type=str_to_bool,
         default=True,
-        help="Compute image mean and std (default: %(default)s)",
+        help="Compute image mean and std (RGB) (default: %(default)s)",
     )
     parser.add_argument(
         "--ann-stats",
         type=str_to_bool,
         default=True,
         help="Compute annotation statistics (default: %(default)s)",
     )
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/transform.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/commands/validate.py` & `datumaro-1.6.1rc1/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/contexts/model.py` & `datumaro-1.6.1rc1/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/contexts/source.py` & `datumaro-1.6.1rc1/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/contexts/util.py` & `datumaro-1.6.1rc1/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/util/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/util/compare.py` & `datumaro-1.6.1rc1/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/cli/util/project.py` & `datumaro-1.6.1rc1/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/abstracts/merger.py` & `datumaro-1.6.1rc1/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.6.1rc1/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.6.1rc1/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.6.1rc1/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/annotation.py` & `datumaro-1.6.1rc1/src/datumaro/components/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2021-2022 Intel Corporation
+# Copyright (C) 2021-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 from enum import IntEnum
 from functools import partial
@@ -366,31 +366,66 @@
     @property
     def image(self) -> BinaryMaskImage:
         image = self._image
         if callable(image):
             image = image()
         return image
 
-    def as_class_mask(self, label_id: Optional[int] = None) -> IndexMaskImage:
-        """
-        Produces a class index mask. Mask label id can be changed.
+    def as_class_mask(
+        self,
+        label_id: Optional[int] = None,
+        ignore_index: int = 0,
+        dtype: Optional[np.dtype] = None,
+    ) -> IndexMaskImage:
+        """Produces a class index mask based on the binary mask.
+
+        Args:
+            label_id: Scalar value to represent the class index of the mask.
+                If not specified, `self.label` will be used. Defaults to None.
+            ignore_index: Scalar value to fill in the zeros in the binary mask.
+                Defaults to 0.
+            dtype: Data type for the resulting mask. If not specified,
+                it will be inferred from the provided `label_id` to hold its value.
+                For example, if `label_id=255`, the inferred dtype will be `np.uint8`.
+                Defaults to None.
+
+        Returns:
+            IndexMaskImage: Class index mask generated from the binary mask.
         """
         if label_id is None:
             label_id = self.label
         from datumaro.util.mask_tools import make_index_mask
 
-        return make_index_mask(self.image, label_id)
+        return make_index_mask(self.image, index=label_id, ignore_index=ignore_index, dtype=dtype)
 
-    def as_instance_mask(self, instance_id: int) -> IndexMaskImage:
-        """
-        Produces a instance index mask.
+    def as_instance_mask(
+        self,
+        instance_id: int,
+        ignore_index: int = 0,
+        dtype: Optional[np.dtype] = None,
+    ) -> IndexMaskImage:
+        """Produces an instance index mask based on the binary mask.
+
+        Args:
+            instance_id: Scalar value to represent the instance id.
+            ignore_index: Scalar value to fill in the zeros in the binary mask.
+                Defaults to 0.
+            dtype: Data type for the resulting mask. If not specified,
+                it will be inferred from the provided `label_id` to hold its value.
+                For example, if `label_id=255`, the inferred dtype will be `np.uint8`.
+                Defaults to None.
+
+        Returns:
+            IndexMaskImage: Instance index mask generated from the binary mask.
         """
         from datumaro.util.mask_tools import make_index_mask
 
-        return make_index_mask(self.image, instance_id)
+        return make_index_mask(
+            self.image, index=instance_id, ignore_index=ignore_index, dtype=dtype
+        )
 
     def get_area(self) -> int:
         return np.count_nonzero(self.image)
 
     def get_bbox(self) -> Tuple[int, int, int, int]:
         """
         Computes the bounding box of the mask.
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/annotations/matcher.py` & `datumaro-1.6.1rc1/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/annotations/merger.py` & `datumaro-1.6.1rc1/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/cli_plugin.py` & `datumaro-1.6.1rc1/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/comparator.py` & `datumaro-1.6.1rc1/src/datumaro/components/comparator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2023-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
 from textwrap import wrap
@@ -517,35 +517,35 @@
         subset_names = first_subsets.copy()
         subset_names.extend(item for item in second_subsets if item not in first_subsets)
 
         for subset_name in subset_names:
             first_subset_data = first_image_stats["subsets"].get(subset_name, {})
             second_subset_data = second_image_stats["subsets"].get(subset_name, {})
             mean_str_first = (
-                ", ".join(f"{val:6.2f}" for val in first_subset_data.get("image mean", []))
-                if "image mean" in first_subset_data
+                ", ".join(f"{val:6.2f}" for val in first_subset_data.get("image mean (RGB)", []))
+                if "image mean (RGB)" in first_subset_data
                 else ""
             )
             std_str_first = (
-                ", ".join(f"{val:6.2f}" for val in first_subset_data.get("image std", []))
+                ", ".join(f"{val:6.2f}" for val in first_subset_data.get("image std (RGB)", []))
                 if "image std" in first_subset_data
                 else ""
             )
             mean_str_second = (
-                ", ".join(f"{val:6.2f}" for val in second_subset_data.get("image mean", []))
-                if "image mean" in second_subset_data
+                ", ".join(f"{val:6.2f}" for val in second_subset_data.get("image mean (RGB)", []))
+                if "image mean (RGB)" in second_subset_data
                 else ""
             )
             std_str_second = (
                 ", ".join(f"{val:6.2f}" for val in second_subset_data.get("image std", []))
-                if "image std" in second_subset_data
+                if "image std (RGB)" in second_subset_data
                 else ""
             )
-            rows.append([f"{subset_name} - Image Mean", mean_str_first, mean_str_second])
-            rows.append([f"{subset_name} - Image Std", std_str_first, std_str_second])
+            rows.append([f"{subset_name} - Image Mean (RGB)", mean_str_first, mean_str_second])
+            rows.append([f"{subset_name} - Image Std (RGB)", std_str_first, std_str_second])
 
         first_labels = sorted(list(first_ann_stats["annotations"]["labels"]["distribution"].keys()))
         second_labels = sorted(
             list(second_ann_stats["annotations"]["labels"]["distribution"].keys())
         )
 
         label_names = first_labels.copy()
@@ -600,35 +600,44 @@
         ]
 
         table = self._create_table(headers, rows)
         data_dict = self._create_dict(rows)
 
         return table, data_dict
 
-    def compare_datasets(self, first: Dataset, second: Dataset) -> Tuple[str, str, str, Dict]:
+    def compare_datasets(
+        self, first: Dataset, second: Dataset, mode: str = "all"
+    ) -> Tuple[str, str, str, Dict]:
         """Compares two datasets and generates comparison reports.
 
         Args:
             first: The first dataset to compare.
             second: The second dataset to compare.
 
         Returns:
             A tuple containing high-level table, mid-level table, low-level table, and a
             dictionary representation of the comparison.
         """
         first_info = self._analyze_dataset(first)
         second_info = self._analyze_dataset(second)
 
-        high_level_table, high_level_dict = self._create_high_level_comparison_table(
-            first_info, second_info
-        )
-        mid_level_table, mid_level_dict = self._create_mid_level_comparison_table(
-            first_info, second_info
-        )
-        low_level_table, low_level_dict = self._create_low_level_comparison_table(first, second)
+        high_level_table, high_level_dict = None, {}
+        mid_level_table, mid_level_dict = None, {}
+        low_level_table, low_level_dict = None, {}
+
+        if mode in ["high", "all"]:
+            high_level_table, high_level_dict = self._create_high_level_comparison_table(
+                first_info, second_info
+            )
+        if mode in ["mid", "all"]:
+            mid_level_table, mid_level_dict = self._create_mid_level_comparison_table(
+                first_info, second_info
+            )
+        if mode in ["low", "all"]:
+            low_level_table, low_level_dict = self._create_low_level_comparison_table(first, second)
 
         comparison_dict = dict(
             high_level=high_level_dict, mid_level=mid_level_dict, low_level=low_level_dict
         )
 
         print(f"High-level comparison:\n{high_level_table}\n")
         print(f"Mid-level comparison:\n{mid_level_table}\n")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/config.py` & `datumaro-1.6.1rc1/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/config_model.py` & `datumaro-1.6.1rc1/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/contexts/importer.py` & `datumaro-1.6.1rc1/src/datumaro/components/contexts/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/crypter.py` & `datumaro-1.6.1rc1/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/dataset.py` & `datumaro-1.6.1rc1/src/datumaro/components/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from datumaro.components.dataset_item_storage import DatasetItemStorageDatasetView
 from datumaro.components.dataset_storage import DatasetPatch, DatasetStorage, StreamDatasetStorage
 from datumaro.components.environment import DEFAULT_ENVIRONMENT, Environment
 from datumaro.components.errors import (
     DatasetImportError,
     MultipleFormatsMatchError,
     NoMatchingFormatsError,
+    StreamedItemError,
     UnknownFormatError,
 )
 from datumaro.components.exporter import ExportContext, Exporter, ExportErrorPolicy, _ExportFail
 from datumaro.components.filter import (
     UserFunctionAnnotationsFilter,
     UserFunctionDatasetFilter,
     XPathAnnotationsFilter,
@@ -436,25 +437,24 @@
                 applied to items or annotations
             remove_empty: When filtering annotations, allows to
                 exclude empty items from the resulting dataset
 
         Returns: self
 
         Example:
-            - (`filter_annotations=True`) This is an example of filtering
+            - (`filter_annotations=False`) This is an example of filtering
                 dataset items with images larger than 1024 pixels::
 
                 from datumaro.components.media import Image
 
                 def filter_func(item: DatasetItem) -> bool:
                     h, w = item.media_as(Image).size
                     return h > 1024 or w > 1024
 
-                filtered = UserFunctionDatasetFilter(
-                    extractor=dataset, filter_func=filter_func)
+                filtered = dataset.filter(filter_func=filter_func, filter_annotations=False)
                 # No items with an image height or width greater than 1024
                 filtered_items = [item for item in filtered]
 
             - (`filter_annotations=True`) This is an example of removing bounding boxes
                 sized greater than 50% of the image size::
 
                 from datumaro.components.media import Image
@@ -468,16 +468,15 @@
                     h, w = item.media_as(Image).size
                     image_size = h * w
                     bbox_size = ann.h * ann.w
 
                     # Accept Bboxes smaller than 50% of the image size
                     return bbox_size < 0.5 * image_size
 
-                filtered = UserFunctionAnnotationsFilter(
-                    extractor=dataset, filter_func=filter_func)
+                filtered = dataset.filter(filter_func=filter_func, filter_annotations=True)
                 # No bounding boxes with a size greater than 50% of their image
                 filtered_items = [item for item in filtered]
         """
         ...
 
     def filter(
         self,
@@ -928,14 +927,19 @@
         """Create a deep copy of this dataset.
 
         Returns:
             A cloned instance of the `Dataset`.
         """
         return deepcopy(self)
 
+    def __getitem__(self, idx: int) -> DatasetItem:
+        if not self._data.is_stream:
+            return self._data[idx]
+        raise StreamedItemError()
+
 
 class StreamDataset(Dataset):
     _stream = True
 
     def __init__(
         self,
         source: Optional[IDataset] = None,
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/dataset_base.py` & `datumaro-1.6.1rc1/src/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.6.1rc1/src/datumaro/components/dataset_item_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     removed = auto()
 
 
 class DatasetItemStorage:
     def __init__(self):
         self.data = {}  # { subset_name: { id: DatasetItem } }
         self._traversal_order = {}  # maintain the order of elements
+        self._order = []  # allow indexing
 
     def __iter__(self) -> Iterator[DatasetItem]:
         for item in self._traversal_order.values():
             yield item
 
     def __len__(self) -> int:
         return len(self._traversal_order)
@@ -36,14 +37,16 @@
         # Subsets might contain removed items, so this may differ from __len__
         return all(len(s) == 0 for s in self.data.values())
 
     def put(self, item: DatasetItem) -> bool:
         subset = self.data.setdefault(item.subset, {})
         is_new = subset.get(item.id) is None
         self._traversal_order[(item.id, item.subset)] = item
+        if is_new:
+            self._order.append((item.id, item.subset))
         subset[item.id] = item
         return is_new
 
     def get(
         self, id: Union[str, DatasetItem], subset: Optional[str] = None, dummy: Any = None
     ) -> Optional[DatasetItem]:
         if isinstance(id, DatasetItem):
@@ -63,14 +66,15 @@
 
         subset_data = self.data.setdefault(subset, {})
         is_removed = subset_data.get(id) is not None
         subset_data[id] = None
         if is_removed:
             # TODO : investigate why "del subset_data[id]" cannot replace "subset_data[id] = None".
             self._traversal_order.pop((id, subset))
+            self._order.remove((id, subset))
         return is_removed
 
     def __contains__(self, x: Union[DatasetItem, Tuple[str, str]]) -> bool:
         if not isinstance(x, tuple):
             x = [x]
         dummy = 0
         return self.get(*x, dummy=dummy) is not dummy
@@ -95,17 +99,23 @@
             for ann in item.annotations:
                 annotations_by_type[ann.type.name]["count"] += 1
         return sum(t["count"] for t in annotations_by_type.values())
 
     def __copy__(self):
         copied = DatasetItemStorage()
         copied._traversal_order = copy(self._traversal_order)
+        copied._order = copy(self._order)
         copied.data = copy(self.data)
         return copied
 
+    def __getitem__(self, idx: int) -> DatasetItem:
+        _id, subset = self._order[idx]
+        item = self.data[subset][_id]
+        return item
+
 
 class DatasetItemStorageDatasetView(IDataset):
     class Subset(IDataset):
         def __init__(self, parent: "DatasetItemStorageDatasetView", name: str):
             super().__init__()
             self.parent = parent
             self.name = name
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/dataset_storage.py` & `datumaro-1.6.1rc1/src/datumaro/components/dataset_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,14 +553,21 @@
                 )
                 continue
 
             safe_transforms += [transform]
 
         self._transforms = safe_transforms
 
+    def __getitem__(self, idx: int) -> DatasetItem:
+        try:
+            return self._storage[idx]
+        except IndexError:  # Data storage should be initialized
+            self.init_cache()
+            return self._storage[idx]
+
 
 class StreamSubset(IDataset):
     def __init__(self, source: IDataset, subset: str) -> None:
         if not source.is_stream:
             raise ValueError("source should be a stream.")
         self._source = source
         self._subset = subset
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/errors.py` & `datumaro-1.6.1rc1/src/datumaro/components/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,7 +747,13 @@
         return (
             f"Annotation '{self.ann_id}' in the "
             f"item has a value of '{self.prop}' that "
             "is too far from the attribute average. (mean of "
             f"'{self.attr_name}' = '{self.attr_value}' for the "
             f"'{self.label_name}' label: {self.mean}, got '{self.val}')."
         )
+
+
+@define(auto_exc=False)
+class StreamedItemError(DatasetError):
+    def __str__(self):
+        return "__getitem__ is disabled for StreamDataset. Use Dataset instead."
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/extractor_tfds.py` & `datumaro-1.6.1rc1/src/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/filter.py` & `datumaro-1.6.1rc1/src/datumaro/components/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2023 Intel Corporation
+# Copyright (C) 2019-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 import logging as log
 from typing import TYPE_CHECKING, Callable, Optional
 
@@ -11,14 +11,15 @@
 
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
     Bbox,
     Caption,
     Ellipse,
+    HashKey,
     Label,
     Mask,
     Points,
     Polygon,
     PolyLine,
 )
 from datumaro.components.media import Image
@@ -253,14 +254,17 @@
             return cls.encode_polyline_object(o, categories)
         if isinstance(o, Polygon):
             return cls.encode_polygon_object(o, categories)
         if isinstance(o, Caption):
             return cls.encode_caption_object(o)
         if isinstance(o, Ellipse):
             return cls.encode_ellipse_object(o, categories)
+        if isinstance(o, HashKey):
+            return cls.encode_annotation_base(o)
+
         raise NotImplementedError("Unexpected annotation object passed: %s" % o)
 
     @staticmethod
     def to_string(encoded_item: ET.ElementBase) -> str:
         return ET.tostring(encoded_item, encoding="unicode", pretty_print=True)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/format_detection.py` & `datumaro-1.6.1rc1/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/generator.py` & `datumaro-1.6.1rc1/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/components/hl_ops/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,25 +186,28 @@
             remove_empty: When filtering annotations, allows to
                 exclude empty items from the resulting dataset
 
         Returns: a wrapper around the input dataset, which is computed lazily
             during iteration
 
         Example:
-            - (`filter_annotations=True`) This is an example of filtering
+            - (`filter_annotations=False`) This is an example of filtering
                 dataset items with images larger than 1024 pixels::
 
                 from datumaro.components.media import Image
 
                 def filter_func(item: DatasetItem) -> bool:
                     h, w = item.media_as(Image).size
                     return h > 1024 or w > 1024
 
-                filtered = UserFunctionDatasetFilter(
-                    extractor=dataset, filter_func=filter_func)
+                filtered = HLOps.filter(
+                    dataset=dataset,
+                    filter_func=filter_func,
+                    filter_annotations=False,
+                )
                 # No items with an image height or width greater than 1024
                 filtered_items = [item for item in filtered]
 
             - (`filter_annotations=True`) This is an example of removing bounding boxes
                 sized greater than 50% of the image size::
 
                 from datumaro.components.media import Image
@@ -218,16 +221,19 @@
                     h, w = item.media_as(Image).size
                     image_size = h * w
                     bbox_size = ann.h * ann.w
 
                     # Accept Bboxes smaller than 50% of the image size
                     return bbox_size < 0.5 * image_size
 
-                filtered = UserFunctionAnnotationsFilter(
-                    extractor=dataset, filter_func=filter_func)
+                filtered = HLOps.filter(
+                    dataset=dataset,
+                    filter_func=filter_func,
+                    filter_annotations=True,
+                )
                 # No bounding boxes with a size greater than 50% of their image
                 filtered_items = [item for item in filtered]
         """
 
     def filter(
         dataset: IDataset,
         expr_or_filter_func: Union[
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/importer.py` & `datumaro-1.6.1rc1/src/datumaro/components/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,18 @@
     ) -> FormatDetectionConfidence:
         if not cls.find_sources_with_params(context.root_path):
             context.fail("specific requirement information unavailable")
 
         return cls.DETECT_CONFIDENCE
 
     @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        raise NotImplementedError()
+
+    @classmethod
     def find_sources(cls, path: str) -> List[Dict]:
         raise NotImplementedError()
 
     @classmethod
     def find_sources_with_params(cls, path: str, **extra_params) -> List[Dict]:
         return cls.find_sources(path)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/launcher.py` & `datumaro-1.6.1rc1/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/lazy_plugin.py` & `datumaro-1.6.1rc1/src/datumaro/components/lazy_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 from abc import ABC, abstractclassmethod
 from importlib import import_module
 from importlib.util import find_spec
-from typing import List, Optional, Sequence, Type, Union
+from typing import Dict, List, Optional, Sequence, Type, Union
 
 from datumaro.components.dataset_base import DatasetBase
 from datumaro.components.errors import DatumaroError
 from datumaro.components.exporter import Exporter
 from datumaro.components.generator import DatasetGenerator
 from datumaro.components.importer import Importer
 from datumaro.components.launcher import Launcher
@@ -53,25 +53,27 @@
 
 
 def get_lazy_plugin(
     import_path: str,
     plugin_name: str,
     plugin_type: str,
     extra_deps: List[str] = [],
+    metadata: Dict = {},
 ) -> Optional[LazyPlugin]:
     for extra_dep in extra_deps:
         spec = find_spec(extra_dep)
         if spec is None:
             log.debug(f"Cannot import extra dep={extra_dep} for plugin_name={plugin_name}.")
             return None
 
     plugin_type_cls = STR_TO_PLUGIN_TYPES[plugin_type]
 
     class LazyPluginImpl(LazyPlugin, plugin_type_cls):
         NAME = plugin_name
+        METADATA = metadata
 
         @classmethod
         def get_plugin_cls(cls) -> PLUGIN_TYPES:
             splits = import_path.split(".")
             module_name = ".".join(splits[:-1])
             class_name = splits[-1]
             module = import_module(module_name)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/media.py` & `datumaro-1.6.1rc1/src/datumaro/components/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from __future__ import annotations
 
 import errno
 import io
 import os
 import os.path as osp
 import shutil
-import weakref
 from copy import deepcopy
 from enum import IntEnum
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
@@ -25,14 +24,15 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import cv2
+import imagesize
 import numpy as np
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.errors import DatumaroError, MediaShapeError
 from datumaro.util.definitions import BboxIntCoords
 from datumaro.util.image import (
     _image_loading_errors,
@@ -326,14 +326,27 @@
 
         if self._size is None and data is not None:
             if not 2 <= data.ndim <= 3:
                 raise MediaShapeError("An image should have 2 (gray) or 3 (bgra) dims.")
             self._size = tuple(map(int, data.shape[:2]))
         return data
 
+    @property
+    def size(self) -> Optional[Tuple[int, int]]:
+        """Returns (H, W)"""
+
+        if self._size is None:
+            try:
+                width, height = imagesize.get(self.path)
+                assert width != -1 and height != -1
+                self._size = (height, width)
+            except Exception:
+                _ = super().size
+        return self._size
+
     def save(
         self,
         fp: Union[str, io.IOBase],
         ext: Optional[str] = None,
         crypter: Crypter = NULL_CRYPTER,
     ):
         cur_path = osp.abspath(self.path) if self.path else None
@@ -585,18 +598,14 @@
         #   can be invalid or inaccurate due to variable frame rate
         #   or fractional values rounded up. Relying on the value will give
         #   errors during requesting frames.
         # https://stackoverflow.com/a/47796468
         self._frame_count = None
         self._length = None
 
-        from .media_manager import MediaManager
-
-        MediaManager.get_instance().push(weakref.ref(self), self)
-
     def close(self):
         self._iterator = None
 
         if self._reader is not None:
             self._reader.release()
             self._reader = None
 
@@ -967,16 +976,14 @@
 
     @property
     def roi(self) -> BboxIntCoords:
         return self._roi
 
     def _get_roi_data(self, data: np.ndarray) -> np.ndarray:
         x, y, w, h = self._roi
-        if isinstance(data, np.ndarray):
-            data = data.astype(np.float32)
         return data[y : y + h, x : x + w]
 
     def save(
         self,
         fp: Union[str, io.IOBase],
         ext: Optional[str] = None,
         crypter: Crypter = NULL_CRYPTER,
@@ -1003,15 +1010,15 @@
         **kwargs,
     ) -> None:
         super().__init__(path, roi, *args, **kwargs)
         self.__data = lazy_image(self.path, crypter=self._crypter)
 
     @property
     def data(self) -> Optional[np.ndarray]:
-        """Image data in BGRA HWC [0; 255] (float) format"""
+        """Image data in BGRA HWC [0; 255] (uint8) format"""
         if not self.has_data:
             return None
         data = self.__data()
         return self._get_roi_data(data)
 
 
 class RoIImageFromData(FromDataMixin, RoIImage):
@@ -1026,15 +1033,15 @@
         *args,
         **kwargs,
     ) -> None:
         super().__init__(data, roi, *args, **kwargs)
 
     @property
     def data(self) -> Optional[np.ndarray]:
-        """Image data in BGRA HWC [0; 255] (float) format"""
+        """Image data in BGRA HWC [0; 255] (uint8) format"""
         data = super().data
         if data is None:
             return None
         if isinstance(data, bytes):
             data = decode_image(data)
         return self._get_roi_data(data)
 
@@ -1047,15 +1054,15 @@
         *args,
         **kwargs,
     ) -> None:
         super().__init__(data, roi, *args, **kwargs)
 
     @property
     def data(self) -> Optional[np.ndarray]:
-        """Image data in BGRA HWC [0; 255] (float) format"""
+        """Image data in BGRA HWC [0; 255] (uint8) format"""
         data = super().data
         if data is None:
             return None
         return self._get_roi_data(data)
 
 
 ImageWithRoI = Tuple[Image, BboxIntCoords]
@@ -1112,15 +1119,15 @@
         save_image(fp, data, ext=new_ext, crypter=crypter)
 
 
 class MosaicImageFromImageRoIPairs(MosaicImageFromData):
     def __init__(self, data: List[ImageWithRoI], size: Tuple[int, int]) -> None:
         def _get_mosaic_img() -> np.ndarray:
             h, w = self.size
-            mosaic_img = np.zeros(shape=(h, w, 3), dtype=np.float32)
+            mosaic_img = np.zeros(shape=(h, w, 3), dtype=np.uint8)
             for img, roi in data:
                 assert isinstance(img, Image), "MosaicImage can only take a list of Images."
                 x, y, w, h = roi
                 mosaic_img[y : y + h, x : x + w] = img.data
             return mosaic_img
 
         super().__init__(data=_get_mosaic_img, size=size)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/merge/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/merge/base.py` & `datumaro-1.6.1rc1/src/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.6.1rc1/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/merge/extractor_merger.py` & `datumaro-1.6.1rc1/src/datumaro/components/merge/extractor_merger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from typing import Optional, Sequence, TypeVar
+from collections import defaultdict
+from typing import Dict, Iterator, List, Optional, Sequence, TypeVar
 
 from datumaro.components.contexts.importer import _ImportFail
-from datumaro.components.dataset_base import DatasetBase, SubsetBase
+from datumaro.components.dataset_base import (
+    CategoriesInfo,
+    DatasetBase,
+    DatasetInfo,
+    DatasetItem,
+    SubsetBase,
+)
 
 T = TypeVar("T")
 
 
 def check_identicalness(seq: Sequence[T], raise_error_on_empty: bool = True) -> Optional[T]:
     if len(seq) == 0 and raise_error_on_empty:
         raise _ImportFail("It should not be empty.")
@@ -32,35 +39,42 @@
         if len(sources) == 0:
             raise _ImportFail("It should not be empty.")
 
         self._infos = check_identicalness([s.infos() for s in sources])
         self._categories = check_identicalness([s.categories() for s in sources])
         self._media_type = check_identicalness([s.media_type() for s in sources])
         self._is_stream = check_identicalness([s.is_stream for s in sources])
-        self._subsets = {s.subset: s for s in sources}
 
-    def infos(self):
+        self._subsets: Dict[str, List[SubsetBase]] = defaultdict(list)
+        for source in sources:
+            self._subsets[source.subset] += [source]
+
+    def infos(self) -> DatasetInfo:
         return self._infos
 
-    def categories(self):
+    def categories(self) -> CategoriesInfo:
         return self._categories
 
-    def __iter__(self):
-        for subset in self._subsets.values():
-            yield from subset
-
-    def __len__(self):
-        return sum(len(subset) for subset in self._subsets.values())
-
-    def get(self, id: str, subset: Optional[str] = None):
-        if subset is None:
-            for s in self._subsets.values():
-                item = s.get(id)
-                if item is not None:
+    def __iter__(self) -> Iterator[DatasetItem]:
+        for sources in self._subsets.values():
+            for source in sources:
+                yield from source
+
+    def __len__(self) -> int:
+        return sum(len(source) for sources in self._subsets.values() for source in sources)
+
+    def get(self, id: str, subset: Optional[str] = None) -> Optional[DatasetItem]:
+        if subset is not None and (sources := self._subsets.get(subset, [])):
+            for source in sources:
+                if item := source.get(id, subset):
+                    return item
+
+        for sources in self._subsets.values():
+            for source in sources:
+                if item := source.get(id=id, subset=source.subset):
                     return item
 
-        s = self._subsets[subset]
-        return s.get(id, subset)
+        return None
 
     @property
     def is_stream(self) -> bool:
         return self._is_stream
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.6.1rc1/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/merge/union_merge.py` & `datumaro-1.6.1rc1/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/operations.py` & `datumaro-1.6.1rc1/src/datumaro/components/operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import cv2
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset_base import CategoriesInfo, DatasetItem, IDataset
 from datumaro.components.errors import DatumaroError
 from datumaro.components.media import Image
+from datumaro.util.image import IMAGE_BACKEND, ImageColorChannel, decode_image_context
 
 
 def mean_std(dataset: IDataset):
     counter = _MeanStdCounter()
 
     for item in dataset:
         counter.accumulate(item)
@@ -160,24 +161,29 @@
         )
 
     stats = deepcopy(IMAGE_STATS_SCHEMA)
 
     stats_counter = _MeanStdCounter()
     unique_counter = _ItemMatcher()
 
-    for item in dataset:
-        if not isinstance(item.media, Image):
-            warnings.warn(
-                f"item (id: {item.id}, subset: {item.subset})"
-                f" has media_type, {item.media} but only Image media_type is allowed."
-            )
-            continue
+    # NOTE: Force image color channel to RGB
+    with decode_image_context(
+        image_backend=IMAGE_BACKEND.get(),
+        image_color_channel=ImageColorChannel.COLOR_RGB,
+    ):
+        for item in dataset:
+            if not isinstance(item.media, Image):
+                warnings.warn(
+                    f"item (id: {item.id}, subset: {item.subset})"
+                    f" has media_type, {item.media} but only Image media_type is allowed."
+                )
+                continue
 
-        stats_counter.accumulate(item)
-        unique_counter.process_item(item)
+            stats_counter.accumulate(item)
+            unique_counter.process_item(item)
 
     def _extractor_stats(subset_name):
         sub_counter = _MeanStdCounter()
         sub_counter._stats = {
             k: v
             for k, v in stats_counter._stats.items()
             if subset_name and k[1] == subset_name or not subset_name
@@ -190,23 +196,23 @@
         }
 
         if available:
             mean, std = sub_counter.get_result()
 
             stats.update(
                 {
-                    "image mean": [float(v) for v in mean[::-1]],
-                    "image std": [float(v) for v in std[::-1]],
+                    "image mean (RGB)": [float(v) for v in mean],
+                    "image std (RGB)": [float(v) for v in std],
                 }
             )
         else:
             stats.update(
                 {
-                    "image mean": "n/a",
-                    "image std": "n/a",
+                    "image mean (RGB)": "n/a",
+                    "image std (RGB)": "n/a",
                 }
             )
         return stats
 
     for subset_name in dataset.subsets():
         stats["subsets"][subset_name] = _extractor_stats(subset_name)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/progress_reporting.py` & `datumaro-1.6.1rc1/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/project.py` & `datumaro-1.6.1rc1/src/datumaro/components/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,14 @@
     UnknownStageError,
     UnknownTargetError,
     UnsavedChangesError,
     VcsAlreadyExists,
     VcsError,
 )
 from datumaro.components.launcher import Launcher
-from datumaro.components.media_manager import MediaManager
 from datumaro.util import find, parse_json_file, parse_str_enum_value
 from datumaro.util.log_utils import catch_logs, logging_disabled
 from datumaro.util.os_util import (
     copytree,
     generate_next_name,
     is_subpath,
     make_file_name,
@@ -1808,16 +1807,14 @@
 
         project = Project(path)
         project._init_vcs()
 
         return project
 
     def close(self):
-        MediaManager.get_instance().clear()
-
         if self._dvc:
             self._dvc.close()
             self._dvc = None
 
         if self._git:
             self._git.close()
             self._git = None
@@ -2008,16 +2005,14 @@
 
         return tempfile.TemporaryDirectory(suffix=suffix, dir=project_tmp_dir)
 
     def remove_cache_obj(self, ref: Union[Revision, ObjectId]):
         if self.readonly:
             raise ReadonlyProjectError()
 
-        MediaManager.get_instance().clear()
-
         obj_type, obj_hash = self._parse_ref(ref)
 
         if self._is_cached(obj_hash):
             rmtree(self.cache_path(obj_hash))
 
         if obj_type == self._ObjectIdKind.tree:
             # Revision metadata is cheap enough and needed to materialize
@@ -2360,16 +2355,14 @@
 
         if self.readonly:
             raise ReadonlyProjectError()
 
         if name not in self.working_tree.sources and not force:
             raise UnknownSourceError(name)
 
-        MediaManager.get_instance().clear()
-
         self.working_tree.sources.remove(name)
 
         data_dir = self.source_data_dir(name)
         if not keep_data:
             if osp.isdir(data_dir):
                 rmtree(data_dir)
 
@@ -2498,16 +2491,14 @@
         elif sources is None:
             sources = {}
         else:
             sources = set(sources)
 
         rev = rev or "HEAD"
 
-        MediaManager.get_instance().clear()
-
         if sources:
             rev_tree = self.get_rev(rev)
 
             # Check targets
             for s in sources:
                 if s not in rev_tree.sources:
                     raise UnknownSourceError(s)
@@ -2710,14 +2701,12 @@
     def remove_model(self, name: str):
         if self.readonly:
             raise ReadonlyProjectError()
 
         if name not in self.models:
             raise KeyError("Unknown model '%s'" % name)
 
-        MediaManager.get_instance().clear()
-
         self._config.models.remove(name)
 
         data_dir = self.model_data_dir(name)
         if osp.isdir(data_dir):
             rmtree(data_dir)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/shift_analyzer.py` & `datumaro-1.6.1rc1/src/datumaro/components/shift_analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # ruff: noqa: E501
 
-import itertools
 from collections import defaultdict
 from typing import TYPE_CHECKING, Dict, List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import FeatureVector
 from datumaro.components.dataset import IDataset
@@ -75,16 +74,17 @@
         self.model = model
         self._batch_size = 1
 
     def get_activation_stats(self, dataset: IDataset) -> RunningStats1D:
         running_stats = RunningStats1D()
 
         for batch in take_by(dataset, self._batch_size):
-            features = self.model.launch(batch)
-            running_stats.add(list(itertools.chain(*features)))
+            outputs = self.model.launch(batch)[0]
+            features = [outputs[-1]]  # extracted feature vector of googlenet-v4
+            running_stats.add(features)
 
         return running_stats
 
 
 class FeatureAccumulatorByLabel(FeatureAccumulator):
     def __init__(self, model):
         super().__init__(model)
@@ -95,18 +95,19 @@
         for batch in take_by(dataset, self._batch_size):
             inputs, targets = [], []
             for item in batch:
                 for ann in item.annotations:
                     inputs.append(np.atleast_3d(item.media.data))
                     targets.append(ann.label)
 
-            features = self.model.launch(batch)
+            outputs = self.model.launch(batch)[0]
+            features = [outputs[-1]]  # extracted feature vector of googlenet-v4
 
-            for feat, target in zip(features, targets):
-                running_stats[target].add(feat)
+            for target in targets:
+                running_stats[target].add(features)
 
         return running_stats
 
 
 class ShiftAnalyzer:
     def __init__(self) -> None:
         """
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/transformer.py` & `datumaro-1.6.1rc1/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/validator.py` & `datumaro-1.6.1rc1/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/components/visualizer.py` & `datumaro-1.6.1rc1/src/datumaro/components/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
 import logging as log
 import math
 import random
@@ -184,14 +184,16 @@
             return self._draw_cuboid_3d(ann, label_categories, fig, ax, context)
         if ann.type == AnnotationType.super_resolution_annotation:
             return self._draw_super_resolution_annotation(ann, label_categories, fig, ax, context)
         if ann.type == AnnotationType.depth_annotation:
             return self._draw_depth_annotation(ann, label_categories, fig, ax, context)
         if ann.type == AnnotationType.ellipse:
             return self._draw_ellipse(ann, label_categories, fig, ax, context)
+        if ann.type == AnnotationType.hash_key:
+            return None
 
         # warning instead of raising an error for unsupported annotation types.
         log.warning(f"Ignore unknown ann.type={ann.type}")
 
     def _get_color(self, ann: Annotation) -> str:
         color = self.color_cycles[ann.label % len(self.color_cycles)]
         return color
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/configurable_validator.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/configurable_validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 import re
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, CompiledMask, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
@@ -165,23 +165,29 @@
         mask = load_image(path)
         _, instance_mask = np.unique(mask[:, :, 0], return_inverse=True)
         instance_mask = instance_mask.reshape(mask[:, :, 0].shape)
         return instance_mask
 
 
 class Ade20k2017Importer(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file("*/**/*_atr.txt")
+        context.require_file(f"*/**/*_atr{cls._ANNO_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         for i in range(5):
             for i in glob.iglob(osp.join(path, *("*" * i))):
                 if osp.splitext(i)[1].lower() in IMAGE_EXTENSIONS:
                     return [
                         {
                             "url": path,
                             "format": Ade20k2017Base.NAME,
                         }
                     ]
         return []
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 import re
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
@@ -213,17 +213,19 @@
     def _load_class_mask(path):
         mask = load_image(path)
         mask = ((mask[:, :, 2] / 10).astype(np.int32) << 8) + mask[:, :, 1].astype(np.int32)
         return mask
 
 
 class Ade20k2020Importer(Importer):
+    _ANNO_EXT = ".json"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_path = context.require_file("*/**/*.json")
+        annot_path = context.require_file(f"*/**/*{cls._ANNO_EXT}")
 
         with context.probe_text_file(
             annot_path,
             'must be a JSON object with an "annotation" key',
         ):
             fpath = osp.join(context.root_path, annot_path)
             page_mapper = JsonSectionPageMapper(fpath)
@@ -240,7 +242,11 @@
                     return [
                         {
                             "url": path,
                             "format": Ade20k2020Base.NAME,
                         }
                     ]
         return []
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 
 from .format import DatumaroArrow
 
 __all__ = ["ArrowImporter"]
 
 
 class ArrowImporter(Importer):
+    _FORMAT_EXT = ".arrow"
+
     @classmethod
     def detect(
         cls,
         context: FormatDetectionContext,
     ) -> Optional[FormatDetectionConfidence]:
         if context.root_path.endswith(".arrow"):
             cls._verify_datumaro_arrow_format(context.root_path)
@@ -41,15 +43,15 @@
                 cls._verify_datumaro_arrow_format(path)
                 return True
             except DatasetImportError:
                 return False
 
         return cls._find_sources_recursive(
             path=path,
-            ext=".arrow",
+            ext=cls._FORMAT_EXT,
             extractor_name=cls.NAME,
             file_filter=_filter,
             max_depth=0,
         )
 
     @classmethod
     def find_sources_with_params(cls, path: str, **extra_params) -> List[Dict]:
@@ -67,7 +69,11 @@
     def _verify_datumaro_arrow_format(file: str) -> None:
         with pa.memory_map(file, "r") as mm_file:
             with pa.ipc.open_file(mm_file) as reader:
                 schema = reader.schema
         DatumaroArrow.check_signature(schema.metadata.get(b"signature", b"").decode())
         DatumaroArrow.check_version(schema.metadata.get(b"version", b"").decode())
         DatumaroArrow.check_schema(schema)
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import csv
 import errno
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import google.protobuf.text_format as text_format
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
@@ -153,32 +153,38 @@
                     )
                 )
 
         return items.values()
 
 
 class AvaImporter(Importer):
+    _ANNO_EXT = "csv"
+
     @classmethod
     def find_sources(cls, path):
         ann_files = find_files(
-            osp.join(path, AvaPath.ANNOTATION_DIR), exts="csv", recursive=True, max_depth=1
+            osp.join(path, AvaPath.ANNOTATION_DIR), exts=cls._ANNO_EXT, recursive=True, max_depth=1
         )
 
         sources = []
         for ann_file in ann_files:
             if AvaPath.ANNOTATION_PREFIX in ann_file:
                 sources.append({"url": ann_file, "format": AvaBase.NAME})
 
         return sources
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> FormatDetectionConfidence:
         super().detect(context)
         return FormatDetectionConfidence.MEDIUM
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [f".{cls._ANNO_EXT}"]
+
 
 class AvaExporter(Exporter):
     DEFAULT_IMAGE_EXT = AvaPath.IMAGE_EXT
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/brats.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import glob
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import nibabel as nib
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
@@ -103,7 +103,11 @@
         with context.require_any():
             with context.alternative():
                 context.require_file(f"*/*{BratsPath.DATA_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, "", "brats", filename=f"{BratsPath.IMAGES_DIR}*")
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(BratsPath.DATA_EXT)[-1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
@@ -109,7 +109,11 @@
         context.require_file(BratsNumpyPath.IDS_FILE)
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(
             path, "", "brats_numpy", filename=BratsNumpyPath.IDS_FILE
         )
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(BratsNumpyPath.IDS_FILE)[1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/camvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import glob
 import logging as log
 import os
 import os.path as osp
 from collections import OrderedDict
 from enum import Enum, auto
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
@@ -242,17 +242,21 @@
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
 
 class CamvidImporter(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_path = context.require_file("*.txt", exclude_fnames=CamvidPath.LABELMAP_FILE)
+        annot_path = context.require_file(
+            f"*{cls._ANNO_EXT}", exclude_fnames=CamvidPath.LABELMAP_FILE
+        )
 
         with context.probe_text_file(
             annot_path,
             "must be a CamVid-like annotation file",
         ) as f:
             for line in f:
                 _, mask_path = _parse_annotation_line(line)
@@ -270,14 +274,18 @@
         return cls._find_sources_recursive(
             path,
             ".txt",
             "camvid",
             file_filter=lambda p: osp.basename(p) != CamvidPath.LABELMAP_FILE,
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class LabelmapType(Enum):
     camvid = auto()
     source = auto()
 
 
 class CamvidExporter(Exporter):
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Label,
     LabelCategories,
     Points,
@@ -269,7 +269,11 @@
             root_dir = osp.dirname(anno_dir)
             img_dir = osp.join(root_dir, cls.PATH_CLS.IMAGES_DIR)
             if not osp.exists(img_dir):
                 raise DatasetImportError(f"Cannot find {cls.NAME}'s images directory at {img_dir}")
             source["url"] = root_dir
 
         return sources
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(cls.PATH_CLS.LABELS_FILE)[1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cifar.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,18 @@
 
         sources = []
         sources += _find(path, CifarPath.META_10_FILE)
         sources += _find(path, CifarPath.META_100_FILE)
 
         return sources
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list({osp.splitext(p)[1] for p in (CifarPath.META_10_FILE, CifarPath.META_100_FILE)})
+
 
 class CifarExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 from collections import OrderedDict
 from enum import Enum, auto
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
@@ -261,55 +261,57 @@
         mask_suffix = CityscapesPath.LABEL_TRAIN_IDS_SUFFIX
         if not masks:
             masks = glob.glob(
                 osp.join(self._gt_anns_dir, "**", f"*{CityscapesPath.GT_INSTANCE_MASK_SUFFIX}"),
                 recursive=True,
             )
             mask_suffix = CityscapesPath.GT_INSTANCE_MASK_SUFFIX
+
+        self._categories = self._load_categories(
+            self._path, use_train_label_map=mask_suffix is CityscapesPath.LABEL_TRAIN_IDS_SUFFIX
+        )
+
+        label_ids = []
+        for label_cat in self._categories[AnnotationType.label]:
+            label_id, _ = self._categories[AnnotationType.label].find(label_cat.name)
+            if label_id:
+                label_ids.append(label_id)
+
         for mask_path in masks:
             item_id = self._get_id_from_mask_path(mask_path, mask_suffix)
 
             anns = []
             instances_mask = load_image(mask_path, dtype=np.int32)
-            segm_ids = np.unique(instances_mask)
-            for segm_id in segm_ids:
-                # either is_crowd or ann_id should be set
-                if segm_id < 1000:
-                    label_id = segm_id
-                    is_crowd = True
-                    ann_id = None
-                else:
-                    label_id = segm_id // 1000
-                    is_crowd = False
-                    ann_id = segm_id % 1000
+            mask_id = 1
+            for label_id in label_ids:
+                if label_id not in instances_mask:
+                    continue
+                binary_mask = self._lazy_extract_mask(instances_mask, label_id)
                 anns.append(
                     Mask(
-                        image=self._lazy_extract_mask(instances_mask, segm_id),
+                        id=mask_id,
+                        image=binary_mask,
                         label=label_id,
-                        id=ann_id,
-                        attributes={"is_crowd": is_crowd},
                     )
                 )
+                mask_id += 1
 
             image = image_path_by_id.pop(item_id, None)
             if image:
                 image = Image.from_file(path=image)
 
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=image, annotations=anns
             )
 
         for item_id, path in image_path_by_id.items():
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, media=Image.from_file(path=path)
             )
 
-        self._categories = self._load_categories(
-            self._path, use_train_label_map=mask_suffix is CityscapesPath.LABEL_TRAIN_IDS_SUFFIX
-        )
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
 
@@ -348,14 +350,26 @@
                 "cityscapes",
                 dirname=osp.join(CityscapesPath.IMGS_FINE_DIR, CityscapesPath.ORIGINAL_IMAGE_DIR),
                 max_depth=1,
             )
 
         return sources
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list(
+            {
+                osp.splitext(p)[1]
+                for p in (
+                    CityscapesPath.GT_INSTANCE_MASK_SUFFIX,
+                    CityscapesPath.LABEL_TRAIN_IDS_SUFFIX,
+                )
+            }
+        )
+
 
 class LabelmapType(Enum):
     cityscapes = auto()
     source = auto()
 
 
 class CityscapesExporter(Exporter):
@@ -425,16 +439,16 @@
 
                 # If a label can distinguish between instances,
                 # make id an instance id. Otherwise use label id.
                 compiled_mask = CompiledMask.from_instance_masks(
                     masks,
                     instance_ids=[
                         self._label_id_mapping(m.label)
-                        if m.attributes.get("is_crowd", False)
-                        else self._label_id_mapping(m.label) * 1000 + (m.id or (i + 1))
+                        # if m.attributes.get("is_crowd", False)
+                        # else self._label_id_mapping(m.label) * 1000 + (m.id or (i + 1))
                         for i, m in enumerate(masks)
                     ],
                     instance_labels=[self._label_id_mapping(m.label) for m in masks],
                 )
 
                 mask_name = item.id + "_" + CityscapesPath.GT_FINE_DIR
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2022 Intel Corporation
+# Copyright (C) 2019-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import logging as log
 import os.path as osp
 from inspect import isclass
@@ -501,15 +501,20 @@
                         label=label_id,
                         id=ann_id,
                         attributes=attributes,
                         group=group,
                     )
                 )
 
-            segmentation = self._parse_field(ann, "segmentation", (list, dict))
+            try:
+                segmentation = self._parse_field(ann, "segmentation", (list, dict))
+            except MissingFieldError as e:
+                log.warn(str(e))
+                segmentation = None
+
             if segmentation and segmentation != [[]]:
                 rle = None
 
                 if isinstance(segmentation, list):
                     if not self._merge_instance_polygons:
                         # polygon - a single object can consist of multiple parts
                         for polygon_points in segmentation:
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/extractor_merger.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,10 +81,10 @@
 
         grouped_by_subset = defaultdict(list)
 
         for s in sources:
             grouped_by_subset[s.subset] += [s]
 
         self._subsets = {
-            subset: COCOTaskMergedBase(sources, subset)
+            subset: [COCOTaskMergedBase(sources, subset)]
             for subset, sources in grouped_by_subset.items()
         }
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
 from glob import glob
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME
 from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 from datumaro.components.merge.extractor_merger import ExtractorMerger
 from datumaro.plugins.data_formats.coco.base import (
@@ -33,14 +33,15 @@
         CocoTask.captions: CocoCaptionsBase,
         CocoTask.labels: CocoLabelsBase,
         CocoTask.image_info: CocoImageInfoBase,
         CocoTask.panoptic: CocoPanopticBase,
         CocoTask.stuff: CocoStuffBase,
     }
     _IMPORTER_TYPE = CocoImporterType.default
+    _ANNO_EXT = ".json"
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument(
             "--keep-original-category-ids",
             action="store_true",
@@ -61,15 +62,15 @@
         # for the single-task formats.
         if len(cls._TASKS) == 1:
             context.raise_unsupported()
 
         with context.require_any():
             for task in cls._TASKS.keys():
                 with context.alternative():
-                    context.require_file(f"annotations/{task.name}_*.json")
+                    context.require_file(f"annotations/{task.name}_*{cls._ANNO_EXT}")
 
     def __call__(self, path, stream: bool = False, **extra_params):
         subsets = self.find_sources(path)
 
         if len(subsets) == 0:
             raise DatasetNotFoundError(path, self.NAME)
 
@@ -154,14 +155,18 @@
                 ann_type.name + "_", maxsplit=1
             )
             subset_name = parts[1] if len(parts) == 2 else DEFAULT_SUBSET_NAME
             subsets.setdefault(subset_name, {})[ann_type] = subset_path
 
         return subsets
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
     @property
     def can_stream(self) -> bool:
         return True
 
     def get_extractor_merger(self) -> Optional[ExtractorMerger]:
         return COCOExtractorMerger
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/coco/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import glob
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask, MaskCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer, with_subset_dirs
@@ -159,14 +159,18 @@
 
         return FormatDetectionConfidence.MEDIUM
 
     @classmethod
     def find_sources(cls, path):
         return [{"url": path, "format": "common_semantic_segmentation"}]
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(DATASET_META_FILE)[1]]
+
 
 @with_subset_dirs
 class CommonSemanticSegmentationWithSubsetDirsImporter(CommonSemanticSegmentationImporter):
     """It supports the following subset sub-directory structure for CommonSemanticSegmentation.
 
     .. code-block::
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import SuperResolutionAnnotation
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
@@ -76,15 +76,25 @@
 
             items[item_id].annotations = [SuperResolutionAnnotation(Image.from_file(path=hr_image))]
 
         return items
 
 
 class CommonSuperResolutionImporter(Importer):
+    _FORMAT_EXT = ".jpg"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file(osp.join(CommonSuperResolutionPath.HR_IMAGES_DIR, "**", "*"))
-        context.require_file(osp.join(CommonSuperResolutionPath.LR_IMAGES_DIR, "**", "*"))
+        context.require_file(
+            osp.join(CommonSuperResolutionPath.HR_IMAGES_DIR, "**", f"*{cls._FORMAT_EXT}")
+        )
+        context.require_file(
+            osp.join(CommonSuperResolutionPath.LR_IMAGES_DIR, "**", f"*{cls._FORMAT_EXT}")
+        )
 
     @classmethod
     def find_sources(cls, path):
         return [{"url": path, "format": "common_super_resolution"}]
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from collections import OrderedDict
 from copy import deepcopy
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
@@ -388,17 +388,19 @@
                 annotations=item_desc.get("annotations"),
                 attributes={"frame": int(frame_id)},
             )
         return parsed
 
 
 class CvatImporter(Importer):
+    _ANNO_EXT = ".xml"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_file = context.require_file("*.xml")
+        annot_file = context.require_file(f"*{cls._ANNO_EXT}")
 
         with context.probe_text_file(
             annot_file,
             'must be an XML file with an "annotations" root element',
         ) as f:
             _, root_elem = next(ElementTree.iterparse(f, events=("start",)))
             if root_elem.tag != "annotations":
@@ -429,7 +431,11 @@
                 sources += [source]
             else:
                 raise DatasetImportError(
                     "CVAT XML file should have a <meta> -> <task> or <meta> -> <project> subtree."
                 )
 
         return sources
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,13 +40,17 @@
         return cls._find_sources_recursive(
             path,
             cls.PATH_CLS.ANNOTATION_EXT,
             cls.NAME,
             dirname=cls.PATH_CLS.ANNOTATIONS_DIR,
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls.PATH_CLS.ANNOTATION_EXT]
+
     @property
     def can_stream(self) -> bool:
         return True
 
     def get_extractor_merger(self) -> Type[ExtractorMerger]:
         return ExtractorMerger
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # SPDX-License-Identifier: MIT
 
 import csv
 import errno
 import glob
 import logging as log
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import Bbox, Caption, Mask, MaskCategories, Polygon
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
@@ -280,17 +280,19 @@
 class IcdarTextSegmentationBase(_IcdarBase):
     def __init__(self, path, **kwargs):
         kwargs["task"] = IcdarTask.text_segmentation
         super().__init__(path, **kwargs)
 
 
 class IcdarWordRecognitionImporter(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_path = context.require_file("*/gt.txt")
+        annot_path = context.require_file(f"*/gt{cls._ANNO_EXT}")
 
         with context.probe_text_file(
             annot_path,
             "must be a ICDAR-like annotation file",
         ) as f:
             reader = csv.reader(f, doublequote=False, escapechar="\\", skipinitialspace=True)
             fields = next(reader)
@@ -299,28 +301,44 @@
             if osp.splitext(fields[0])[1] not in IMAGE_EXTENSIONS:
                 raise Exception
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".txt", "icdar_word_recognition")
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class IcdarTextLocalizationImporter(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file("**/gt_*.txt")
+        context.require_file(f"**/gt_*{cls._ANNO_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, "", "icdar_text_localization")
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class IcdarTextSegmentationImporter(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        gt_txt_path = context.require_file("**/*_GT.txt")
+        gt_txt_path = context.require_file(f"**/*_GT{cls._ANNO_EXT}")
         gt_bmp_path = osp.splitext(gt_txt_path)[0] + ".bmp"
         context.require_file(glob.escape(gt_bmp_path))
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, "", "icdar_text_segmentation")
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
-from datumaro.util.image import find_images
+from datumaro.util.image import IMAGE_EXTENSIONS, find_images
 
 
 class ImageDirImporter(Importer):
     """
     Reads images from a directory as a dataset.
     """
 
@@ -33,14 +33,18 @@
 
     @classmethod
     def find_sources(cls, path):
         if not osp.isdir(path):
             return []
         return [{"url": path, "format": ImageDirBase.NAME}]
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list(IMAGE_EXTENSIONS)
+
 
 class ImageDirBase(SubsetBase):
     def __init__(
         self,
         url: str,
         *,
         subset: Optional[str] = None,
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
 from enum import Enum
-from typing import Optional
+from typing import List, Optional
 from zipfile import ZIP_BZIP2, ZIP_DEFLATED, ZIP_LZMA, ZIP_STORED, ZipFile
 
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.exporter import Exporter
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import parse_str_enum_value
@@ -47,17 +47,23 @@
                 if extension.lower() not in IMAGE_EXTENSIONS:
                     continue
                 image = Image.from_bytes(data=zf.read(path.filename))
                 self._items.append(DatasetItem(id=item_id, media=image, subset=self._subset))
 
 
 class ImageZipImporter(Importer):
+    _FORMAT_EXT = ".zip"
+
     @classmethod
     def find_sources(cls, path):
-        return cls._find_sources_recursive(path, ".zip", "image_zip")
+        return cls._find_sources_recursive(path, cls._FORMAT_EXT, "image_zip")
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
 
 
 class ImageZipExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
     @staticmethod
     def _get_compression_method(s):
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # SPDX-License-Identifier: MIT
 
 import errno
 import logging as log
 import os
 import os.path as osp
 import warnings
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer, with_subset_dirs
 from datumaro.components.media import Image
 from datumaro.util.definitions import SUBSET_NAME_BLACKLIST
-from datumaro.util.image import find_images
+from datumaro.util.image import IMAGE_EXTENSIONS, find_images
 
 
 class ImagenetPath:
     IMAGE_DIR_NO_LABEL = "no_label"
     SEP_TOKEN = ":"
 
 
@@ -124,14 +124,18 @@
         # Images should be in root/label_dir/*.img and root/*.img is not allowed.
         # => max_depth=1, min_depth=1
         for _ in find_images(path, recursive=True, max_depth=1, min_depth=1):
             return [{"url": path, "format": ImagenetBase.NAME}]
 
         return []
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list(IMAGE_EXTENSIONS)
+
 
 @with_subset_dirs
 class ImagenetWithSubsetDirsImporter(ImagenetImporter):
     """TorchVision ImageFolder style importer.
     For example, it imports the following directory structure.
 
     .. code-block::
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
 from enum import Enum, auto
-from typing import Iterable, Optional, Sequence, Tuple, Union
+from typing import Iterable, List, Optional, Sequence, Tuple, Union
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
@@ -135,17 +135,21 @@
                     annotations=anno,
                 )
 
         return items
 
 
 class ImagenetTxtImporter(Importer, CliPlugin):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_path = context.require_file("*.txt", exclude_fnames=ImagenetTxtPath.LABELS_FILE)
+        annot_path = context.require_file(
+            f"*{cls._ANNO_EXT}", exclude_fnames=ImagenetTxtPath.LABELS_FILE
+        )
 
         with context.probe_text_file(
             annot_path,
             "must be an ImageNet-like annotation file",
         ) as f:
             for line in f:
                 _, _, label_ids = _parse_annotation_line(line)
@@ -185,14 +189,18 @@
                 return osp.basename(p) != labels_file_name
 
         else:
             file_filter = None
 
         return cls._find_sources_recursive(path, ".txt", "imagenet_txt", file_filter=file_filter)
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class ImagenetTxtExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".jpg"
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kaggle/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,427 +1,422 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import os
+from __future__ import annotations
+
 import os.path as osp
-import warnings
-from typing import Dict, Optional, Type, TypeVar, Union
+from collections import OrderedDict
+from typing import Dict, Iterator, List, Optional, Type, TypeVar, Union
+
+import yaml
 
-import numpy as np
-import pandas as pd
-from defusedxml import ElementTree
-
-from datumaro.components.annotation import (
-    AnnotationType,
-    Bbox,
-    Label,
-    LabelCategories,
-    Mask,
-    MaskCategories,
+from datumaro.components.annotation import Annotation, AnnotationType, Bbox, LabelCategories
+from datumaro.components.dataset_base import CategoriesInfo, DatasetBase, DatasetItem, SubsetBase
+from datumaro.components.errors import (
+    DatasetImportError,
+    InvalidAnnotationError,
+    UndeclaredLabelError,
 )
-from datumaro.components.dataset import DatasetItem
-from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetBase, SubsetBase
-from datumaro.components.errors import InvalidAnnotationError, InvalidFieldError, MissingFieldError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, ImageFromFile
-from datumaro.util.image import IMAGE_EXTENSIONS, load_image
-
-T = TypeVar("T")
-
-
-class KaggleImageCsvBase(DatasetBase):
-    def __init__(
-        self,
-        path: str,
-        ann_file: str,
-        columns: Dict[str, str],
-        *,
-        subset: Optional[str] = DEFAULT_SUBSET_NAME,
-        ctx: Optional[ImportContext] = None,
-    ):
-        super().__init__(ctx=ctx)
-
-        self._subset = subset
-
-        self._path = path
-        self._columns = columns
-
-        self._items, label_cat = self._load_items(ann_file, columns)
-        self._categories = {AnnotationType.label: label_cat}
-
-    def _load_items(self, ann_file: str, columns: Dict[str, Union[str, list]]):
-        df = pd.read_csv(ann_file, header=None, on_bad_lines="skip")
-
-        indices = {}
-        for key, field in columns.items():
-            if key == "bbox":
-                indices[key] = []
-                for v in field:
-                    indices[key].append(list(df.iloc[0]).index(v))
-            else:
-                indices[key] = list(df.iloc[0]).index(field)
-
-        label_cat = LabelCategories()
-        items = []
-        for ind, row in df.iterrows():
-            if ind == 0:
-                continue
-            data_info = list(row)
+from datumaro.util.image import (
+    DEFAULT_IMAGE_META_FILE_NAME,
+    IMAGE_EXTENSIONS,
+    ImageMeta,
+    load_image_meta_file,
+)
+from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
+from datumaro.util.os_util import extract_subset_name_from_parent, find_files, split_path
 
-            media_name = data_info[indices["media"]]
-            id = osp.splitext(media_name)[0]
+from .format import YoloLoosePath, YoloPath, YoloUltralyticsPath
 
-            if not media_name.lower().endswith(tuple(IMAGE_EXTENSIONS)):
-                for ext in IMAGE_EXTENSIONS:
-                    media_path = osp.join(self._path, media_name + ext)
-                    if osp.exists(media_path):
-                        break
-            else:
-                media_path = osp.join(self._path, media_name)
+T = TypeVar("T")
 
-            if not osp.exists(media_path):
-                warnings.warn(
-                    f"'{media_path}' is not existed in the directory, "
-                    f"so we skip to create an dataset item according to {row}."
-                )
-                continue
+__all__ = ["YoloStrictBase", "YoloLooseBase", "YoloUltralyticsBase"]
 
-            annotations = []
-            if "label" in indices:
-                label_name = str(data_info[indices["label"]])
-                label, cat = label_cat.find(label_name)
-
-                if not cat:
-                    label_cat.add(label_name)
-                    label, _ = label_cat.find(label_name)
-
-                annotations.append(Label(label=label))
-
-            items.append(
-                DatasetItem(
-                    id=id,
-                    subset=self._subset,
-                    media=Image.from_file(path=media_path),
-                    annotations=annotations,
-                )
-            )
 
-        return items, label_cat
+def localize_path(path: str) -> str:
+    """
+    Removes the "data/" prefix from the path
+    """
 
-    def categories(self):
-        return self._categories
+    path = osp.normpath(path.strip()).replace("\\", "/")
+    default_base = "data/"
+    if path.startswith(default_base):
+        path = path[len(default_base) :]
+    return path
 
-    def __iter__(self):
-        yield from self._items
 
-
-class KaggleImageTxtBase(DatasetBase):
+# TODO: Need to clean this dirty structure (SubsetBase has _Subset).
+class _Subset(DatasetBase):
     def __init__(
         self,
+        subset_name: str,
         path: str,
-        ann_file: str,
-        columns: Dict[str, int],
-        *,
-        subset: Optional[str] = DEFAULT_SUBSET_NAME,
-        ctx: Optional[ImportContext] = None,
+        items: OrderedDict[str, str],
+        categories: CategoriesInfo,
+        image_info: ImageMeta,
     ):
-        super().__init__(ctx=ctx)
-
-        self._subset = subset
-
+        super().__init__()
+        self._subset_name = subset_name
         self._path = path
-        self._columns = columns
-
-        self._items, label_cat = self._load_items(ann_file, columns)
-        self._categories = {AnnotationType.label: label_cat}
-
-    def _load_items(self, ann_file: str, columns: Dict[str, Union[int, list]]):
-        label_cat = LabelCategories()
+        self._items = items
+        self._categories = categories
+        self._image_info = image_info
+
+    def __iter__(self) -> Iterator[DatasetItem]:
+        for item_id in self._items:
+            item = self._get(item_id)
+            if item is not None:
+                yield item
 
-        item_ids = []
-        items = []
-        with open(ann_file, "r", encoding="utf-8") as f:
-            for line in f:
-                line = line.split()
-                media_name = line[columns["media"]]
-                item_id = osp.splitext(media_name)[0]
-
-                if item_id in item_ids:
-                    warnings.warn(
-                        f"There is duplicated '{id}' in {ann_file}, "
-                        f"so we skip to create an dataset item according to {line}."
-                    )
-                    continue
-
-                if not media_name.lower().endswith(tuple(IMAGE_EXTENSIONS)):
-                    for ext in IMAGE_EXTENSIONS:
-                        media_path = osp.join(self._path, media_name + ext)
-                        if osp.exists(media_path):
-                            break
-                else:
-                    media_path = osp.join(self._path, media_name)
-
-                if not osp.exists(media_path):
-                    warnings.warn(
-                        f"'{media_path}' is not existed in the directory, "
-                        f"so we skip to create an dataset item according to {line}."
-                    )
-                    continue
-
-                annotations = []
-                if "label" in columns:
-                    label_name = str(line[columns["label"]])
-                    label, cat = label_cat.find(label_name)
-
-                    if not cat:
-                        label_cat.add(label_name)
-                        label, _ = label_cat.find(label_name)
-
-                    annotations.append(Label(label=label))
-
-                item_ids.append(item_id)
-                items.append(
-                    DatasetItem(
-                        id=item_id,
-                        subset=self._subset,
-                        media=Image.from_file(path=media_path),
-                        annotations=annotations,
-                    )
-                )
-
-        return items, label_cat
+    def __len__(self):
+        return len(self._items)
 
     def categories(self):
-        return self._categories
+        return self._parent.categories()
 
-    def __iter__(self):
-        yield from self._items
+    def _get(self, item_id: str) -> Optional[DatasetItem]:
+        item = self._items.get(item_id)
 
+        if not isinstance(item, str):
+            return None
 
-class KaggleImageMaskBase(DatasetBase):
-    def __init__(
-        self,
-        path: str,
-        mask_path: str,
-        labelmap_file: Optional[str] = None,
-        *,
-        subset: Optional[str] = DEFAULT_SUBSET_NAME,
-        ctx: Optional[ImportContext] = None,
-    ):
-        super().__init__(ctx=ctx)
+        try:
+            image_size = self._image_info.get(item_id)
+            image = Image.from_file(path=osp.join(self._path, item), size=image_size)
 
-        self._subset = subset
+            anno_path = osp.splitext(image.path)[0] + ".txt"
+            annotations = self._parse_annotations(
+                anno_path,
+                image,
+                label_categories=self._categories[AnnotationType.label],
+            )
 
-        self._path = path
-        self._mask_path = mask_path
+            item = DatasetItem(
+                id=item_id, subset=self._subset_name, media=image, annotations=annotations
+            )
+            return item
+        except (UndeclaredLabelError, InvalidAnnotationError) as e:
+            self._ctx.error_policy.report_annotation_error(e, item_id=(item_id, self._subset_name))
+        except Exception as e:
+            self._ctx.error_policy.report_item_error(e, item_id=(item_id, self._subset_name))
 
-        self._categories = self._load_categories(labelmap_file)
-        self._items = self._load_items()
+        return None
 
-    def _load_categories(self, label_map_file: Optional[str]):
-        label_map = dict()
-        if not label_map_file:
-            label_map["background"] = (0, 0, 0)
-            label_map["object"] = (255, 255, 255)
-        else:
-            df = pd.read_csv(label_map_file)
-            for _, row in df.iterrows():
-                name = row[0]
-                color = tuple([int(c) for c in row[1:]])
-                label_map[name] = color
+    @classmethod
+    def _parse_annotations(
+        cls,
+        anno_path: str,
+        image: ImageFromFile,
+        *,
+        label_categories: LabelCategories,
+    ) -> List[Annotation]:
+        lines = []
+        with open(anno_path, "r", encoding="utf-8") as f:
+            for line in f:
+                line = line.strip()
+                if line:
+                    lines.append(line)
 
-        label_categories = LabelCategories()
-        for label in label_map:
-            label_categories.add(label)
+        annotations = []
 
-        categories = {}
-        categories[AnnotationType.label] = label_categories
+        if lines:
+            # Use image info as late as possible to avoid unnecessary image loading
+            if image.size is None:
+                raise DatasetImportError(f"Can't find image info for '{localize_path(image.path)}'")
+            image_height, image_width = image.size
 
-        colormap = {}
-        for label_name, label_color in label_map.items():
-            label_id = label_categories.find(label_name)[0]
-            colormap[label_id] = label_color
-
-        categories[AnnotationType.mask] = MaskCategories(colormap)
-
-        return categories
-
-    def _load_items(self):
-        def _lazy_extract_mask(mask, c):
-            return lambda: mask == c
-
-        items = []
-        for media_name in os.listdir(self._path):
-            id = osp.splitext(media_name)[0]
-
-            anns = []
-            for mask_name in os.listdir(self._mask_path):
-                if id in mask_name:
-                    instances_mask = load_image(
-                        osp.join(self._mask_path, mask_name), dtype=np.int32
-                    )
-                    label_ids = np.unique(instances_mask)
-                    for label_id in label_ids:
-                        anns.append(
-                            Mask(
-                                image=_lazy_extract_mask(instances_mask, label_id),
-                                label=label_id,
-                            )
-                        )
-
-            items.append(
-                DatasetItem(
-                    id=id,
-                    subset=self._subset,
-                    media=Image.from_file(path=osp.join(self._path, media_name)),
-                    annotations=anns,
+        for idx, line in enumerate(lines):
+            parts = line.split()
+            if len(parts) != 5:
+                raise InvalidAnnotationError(
+                    f"Unexpected field count {len(parts)} in the bbox description. "
+                    "Expected 5 fields (label, xc, yc, w, h)."
                 )
-            )
-
-        return items
+            label_id, xc, yc, w, h = parts
 
-    def categories(self):
-        return self._categories
+            label_id = cls._parse_field(label_id, int, "bbox label id")
+            if label_id not in label_categories:
+                raise UndeclaredLabelError(str(label_id))
+
+            w = cls._parse_field(w, float, "bbox width")
+            h = cls._parse_field(h, float, "bbox height")
+            x = cls._parse_field(xc, float, "bbox center x") - w * 0.5
+            y = cls._parse_field(yc, float, "bbox center y") - h * 0.5
+            annotations.append(
+                Bbox(
+                    x * image_width,
+                    y * image_height,
+                    w * image_width,
+                    h * image_height,
+                    label=label_id,
+                    id=idx,
+                    group=idx,
+                )
+            )
 
-    def __iter__(self):
-        yield from self._items
+        return annotations
 
+    @classmethod
+    def _parse_field(cls, value: str, desired_type: Type[T], field_name: str) -> T:
+        try:
+            return desired_type(value)
+        except Exception as e:
+            raise InvalidAnnotationError(
+                f"Can't parse {field_name} from '{value}'. Expected {desired_type}"
+            ) from e
 
-class KaggleVocBase(SubsetBase):
-    ann_extensions = ".xml"
 
+class YoloStrictBase(SubsetBase):
     def __init__(
         self,
-        path: str,
-        ann_path: str,
+        config_path: str,
+        image_info: Union[None, str, ImageMeta] = None,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
-    ):
+        **kwargs,
+    ) -> None:
         super().__init__(subset=subset, ctx=ctx)
 
-        self._label_cat = LabelCategories()
-        self._items = []
-        self._size = None
+        if not osp.isfile(config_path):
+            raise DatasetImportError(f"Can't read dataset descriptor file '{config_path}'")
 
-        for img_filename in os.listdir(path):
-            if not img_filename.lower().endswith(tuple(IMAGE_EXTENSIONS)):
-                continue
-            item_id = os.path.splitext(img_filename)[0]
+        rootpath = osp.dirname(config_path)
+        self._path = rootpath
 
-            img_file = os.path.join(path, img_filename)
-            ann_file = os.path.join(ann_path, item_id + self.ann_extensions)
+        self._image_info = self.parse_image_info(rootpath, image_info)
 
-            annotations = (
-                self._parse_annotations(img_file, ann_file) if os.path.isfile(ann_file) else []
-            )
+        config = YoloPath._parse_config(config_path)
 
-            media = Image.from_file(path=img_file, size=self._size)
+        names_path = config.get("names")
+        if not names_path:
+            raise InvalidAnnotationError("Failed to parse names file path from config")
 
-            self._items.append(
-                DatasetItem(
-                    id=item_id,
-                    subset=self._subset,
-                    media=media,
-                    annotations=annotations,
-                )
+        self._categories = {
+            AnnotationType.label: self._load_categories(
+                osp.join(self._path, localize_path(names_path))
             )
-        self._categories = {AnnotationType.label: self._label_cat}
+        }
 
-    def _parse_annotations(self, img_file: str, ann_file: str):
-        root_elem = ElementTree.parse(ann_file).getroot()
-        if root_elem.tag != "annotation":
-            raise MissingFieldError("annotation")
-
-        height = self._parse_field(root_elem, "size/height", int, required=False)
-        width = self._parse_field(root_elem, "size/width", int, required=False)
-        if height and width:
-            self._size = (height, width)
+        # The original format is like this:
+        #
+        # classes = 2
+        # train  = data/train.txt
+        # valid  = data/test.txt
+        # names = data/obj.names
+        # backup = backup/
+        #
+        # To support more subset names, we disallow subsets
+        # called 'classes', 'names' and 'backup'.
+        subsets = {k: v for k, v in config.items() if k not in YoloPath.RESERVED_CONFIG_KEYS}
+        self._subsets: Dict[str, self._Subset] = {}
 
-        annotations = []
-        for obj_id, object_elem in enumerate(root_elem.iterfind("object")):
-            label_name = self._parse_field(object_elem, "name", str, required=True)
+        for subset_name, list_path in subsets.items():
+            if subset_name != subset:
+                continue
 
-            bbox_elem = object_elem.find("bndbox")
-            if not bbox_elem:
-                raise MissingFieldError("bndbox")
-
-            xmin = self._parse_field(bbox_elem, "xmin", float)
-            xmax = self._parse_field(bbox_elem, "xmax", float)
-            ymin = self._parse_field(bbox_elem, "ymin", float)
-            ymax = self._parse_field(bbox_elem, "ymax", float)
+            list_path = osp.join(self._path, localize_path(list_path))
+            if not osp.isfile(list_path):
+                raise InvalidAnnotationError(f"Can't find '{subset_name}' subset list file")
+
+            with open(list_path, "r", encoding="utf-8") as f:
+                items = OrderedDict(
+                    (self.name_from_path(p), localize_path(p)) for p in f if p.strip()
+                )
 
-            self._label_cat.add(label_name)
-            label_id, _ = self._label_cat.find(label_name)
-            annotations.append(
-                Bbox(id=obj_id, label=label_id, x=xmin, y=ymin, w=xmax - xmin, h=ymax - ymin)
+            subset = _Subset(
+                subset_name=subset_name,
+                path=self._path,
+                items=items,
+                categories=self._categories,
+                image_info=self._image_info,
             )
+            self._subsets[subset_name] = subset
 
-        return annotations
+    @staticmethod
+    def parse_image_info(
+        rootpath: str, image_info: Optional[Union[str, ImageMeta]] = None
+    ) -> ImageMeta:
+        assert image_info is None or isinstance(image_info, (str, dict))
+        if image_info is None:
+            image_info = osp.join(rootpath, DEFAULT_IMAGE_META_FILE_NAME)
+            if not osp.isfile(image_info):
+                image_info = {}
+        if isinstance(image_info, str):
+            image_info = load_image_meta_file(image_info)
+
+        return image_info
+
+    @classmethod
+    def name_from_path(cls, path: str) -> str:
+        """
+        Obtains <image name> from the path like [data/]<subset>_obj/<image_name>.ext
+
+        <image name> can be <a/b/c/filename>, so it is
+        more involved than just calling "basename()".
+        """
+
+        path = localize_path(path)
+
+        parts = split_path(path)
+        if 1 < len(parts) and not osp.isabs(path):
+            path = osp.join(*parts[1:])  # pylint: disable=no-value-for-parameter
+
+        return osp.splitext(path)[0]
 
     @staticmethod
-    def _parse_field(root, xpath: str, cls: Type[T] = str, required: bool = True) -> Optional[T]:
-        elem = root.find(xpath)
-        if elem is None:
-            if required:
-                raise MissingFieldError(xpath)
-            else:
-                return None
+    def _load_categories(names_path):
+        if has_meta_file(osp.dirname(names_path)):
+            return LabelCategories.from_iterable(parse_meta_file(osp.dirname(names_path)).keys())
 
-        if cls is str:
-            return elem.text
+        label_categories = LabelCategories()
 
-        try:
-            return cls(elem.text)
-        except Exception as e:
-            raise InvalidFieldError(xpath) from e
+        with open(names_path, "r", encoding="utf-8") as f:
+            for label in f:
+                label = label.strip()
+                if label:
+                    label_categories.add(label)
+
+        return label_categories
+
+    def __iter__(self) -> Iterator[DatasetItem]:
+        subsets = self._subsets
+        pbars = self._ctx.progress_reporter.split(len(subsets))
+        for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
+            for item in pbar.iter(subset, desc=f"Importing '{subset_name}'"):
+                yield item
+
+    def __len__(self):
+        return sum(len(s) for s in self._subsets.values())
+
+    def get_subset(self, name):
+        return self._subsets[name]
+
+    @property
+    def is_stream(self) -> bool:
+        return True
 
 
-class KaggleYoloBase(KaggleVocBase, SubsetBase):
-    ann_extensions = ".txt"
+class YoloLooseBase(SubsetBase):
+    META_FILE = YoloLoosePath.NAMES_FILE
 
     def __init__(
         self,
-        path: str,
-        ann_path: str,
+        config_path: str,
+        image_info: Union[None, str, ImageMeta] = None,
+        urls: Optional[List[str]] = None,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
-    ):
-        super().__init__(path=path, ann_path=ann_path, subset=subset, ctx=ctx)
+    ) -> None:
+        super().__init__(subset=subset, ctx=ctx)
 
-    def _parse_annotations(self, img_file: str, ann_file: str):
-        image = ImageFromFile(path=img_file)
-        image_height, image_width = image.size
+        if not osp.isdir(config_path):
+            raise DatasetImportError(f"{config_path} should be a directory.")
 
-        lines = []
-        with open(ann_file, "r", encoding="utf-8") as f:
-            for line in f:
-                line = line.strip()
-                if line:
-                    lines.append(line)
+        if not urls:
+            raise DatasetImportError(
+                f"`urls` should be specified for {self.__class__.__name__}, "
+                f"if you want to import a dataset with using this {self.__class__.__name__} directly. "
+                "In most case, it happens by giving an incorrect format name to the import interface. "
+                "Please consider to import your dataset with this format name, 'yolo', "
+                "such as `Dataset.import_from(..., format='yolo')`."
+            )
 
-        annotations = []
-        for obj_id, line in enumerate(lines):
-            parts = line.split()
-            if len(parts) != 5:
-                raise InvalidAnnotationError(
-                    f"Unexpected field count {len(parts)} in the bbox description. "
-                    "Expected 5 fields (label, xc, yc, w, h)."
+        rootpath = self._get_rootpath(config_path)
+
+        self._image_info = YoloStrictBase.parse_image_info(rootpath, image_info)
+
+        # Init label categories
+        label_categories = self._load_categories(osp.join(rootpath, self.META_FILE))
+        self._categories = {AnnotationType.label: label_categories}
+
+        self._urls = urls
+        self._img_files = self._load_img_files(rootpath)
+
+    def __iter__(self) -> Iterator[DatasetItem]:
+        label_categories = self._categories.get(AnnotationType.label)
+        if label_categories is None:
+            raise DatasetImportError("label_categories should be not None.")
+
+        pbar = self._ctx.progress_reporter
+        for url in pbar.iter(self._urls, desc=f"Importing '{self._subset}'"):
+            try:
+                fname = self._get_fname(url)
+                img = Image.from_file(path=self._img_files[fname])
+                anns = self._parse_annotations(
+                    url,
+                    img,
+                    label_categories=label_categories,
                 )
-            label_name, xc, yc, w, h = parts
-            xc = float(xc)
-            yc = float(yc)
-            w = float(w)
-            h = float(h)
-            x = (xc - w * 0.5) * image_width
-            y = (yc - h * 0.5) * image_height
-            w *= image_width
-            h *= image_height
+                yield DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
+            except Exception as e:
+                self._ctx.error_policy.report_item_error(e, item_id=(fname, self._subset))
+
+    def __len__(self) -> int:
+        return len(self._urls)
+
+    def _get_rootpath(self, config_path: str) -> str:
+        return config_path
+
+    def _load_categories(self, names_path: str) -> LabelCategories:
+        return YoloStrictBase._load_categories(names_path)
+
+    def _get_fname(self, fpath: str) -> str:
+        return osp.splitext(osp.basename(fpath))[0]
+
+    def _load_img_files(self, rootpath: str) -> Dict[str, str]:
+        return {
+            self._get_fname(img_file): img_file
+            for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
+            if extract_subset_name_from_parent(img_file, rootpath) == self._subset
+        }
+
+    def _parse_annotations(
+        self, anno_path: str, image: ImageFromFile, label_categories: LabelCategories
+    ) -> List[Annotation]:
+        return _Subset._parse_annotations(
+            anno_path=anno_path, image=image, label_categories=label_categories
+        )
+
+    def _parse_field(self, value: str, desired_type: Type[T], field_name: str) -> T:
+        return _Subset._parse_field(value=value, desired_type=desired_type, field_name=field_name)
+
+    @property
+    def is_stream(self) -> bool:
+        return True
 
-            self._label_cat.add(label_name)
-            label_id, _ = self._label_cat.find(label_name)
 
-            annotations.append(Bbox(id=obj_id, label=label_id, x=x, y=y, w=w, h=h))
+class YoloUltralyticsBase(YoloLooseBase):
+    META_FILE = YoloUltralyticsPath.META_FILE
 
-        return annotations
+    def __init__(
+        self,
+        config_path: str,
+        image_info: Union[None, str, ImageMeta] = None,
+        urls: Optional[List[str]] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(config_path, image_info, urls, **kwargs)
+
+    def _load_categories(self, names_path: str) -> LabelCategories:
+        if has_meta_file(osp.dirname(names_path)):
+            return LabelCategories.from_iterable(parse_meta_file(osp.dirname(names_path)).keys())
+
+        label_categories = LabelCategories()
+
+        with open(names_path, "r") as fp:
+            loaded = yaml.safe_load(fp.read())
+            if isinstance(loaded["names"], list):
+                label_names = loaded["names"]
+            elif isinstance(loaded["names"], dict):
+                label_names = list(loaded["names"].values())
+            else:
+                raise DatasetImportError(f"Can't read dataset category file '{names_path}'")
+
+        for label_name in label_names:
+            label_categories.add(label_name)
+
+        return label_categories
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import csv
 import errno
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Video
 from datumaro.plugins.data_formats.video import VIDEO_EXTENSIONS
@@ -130,19 +130,21 @@
                     item_desc["annotations"]["segment"][1],
                     item_desc["subset"],
                 )
             )
 
 
 class KineticsImporter(Importer):
+    _ANNO_EXTS = [".json", ".csv"]
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         with context.require_any():
             with context.alternative():
-                ann_file = context.require_file("*.json")
+                ann_file = context.require_file(f"*{cls._ANNO_EXTS[0]}")
 
                 with context.probe_text_file(
                     ann_file,
                     "JSON file must contain an youtube 'url' key",
                 ) as f:
                     fpath = osp.join(context.root_path, ann_file)
                     page_mapper = JsonSectionPageMapper(fpath)
@@ -155,22 +157,26 @@
                     contents = parse_json(f.read(size))
                     if not isinstance(contents, dict):
                         raise Exception
                     if "youtube" not in contents.get("url", ""):
                         raise Exception
 
             with context.alternative():
-                ann_file = context.require_file("*.csv")
+                ann_file = context.require_file(f"*{cls._ANNO_EXTS[1]}")
 
                 with context.probe_text_file(
                     ann_file,
                     "CSV file must contain 'youtube_id' in header",
                 ) as f:
                     header = f.readline()
                     if "youtube_id" not in header.split(","):
                         raise Exception
 
     @classmethod
     def find_sources(cls, path):
         if find_files(path, ["csv", "json"]):
             return [{"url": path, "format": KineticsBase.NAME}]
         return []
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return cls._ANNO_EXTS
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (C) 2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
 from glob import glob
+from typing import List
 
 from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 
 from .format import KittiPath, KittiTask
 
@@ -80,28 +81,43 @@
     ) -> FormatDetectionConfidence:
         sub_importers = [KittiDetectionImporter, KittiSegmentationImporter]
         with context.require_any():
             for importer_cls in sub_importers:
                 with context.alternative():
                     importer_cls.detect(context)
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        sub_importers = [KittiDetectionImporter, KittiSegmentationImporter]
+        return list({ext for importer in sub_importers for ext in importer.get_file_extensions()})
+
 
 class KittiDetectionImporter(KittiImporter):
     _TASK = KittiTask.detection
     _TASKS = {_TASK: KittiImporter._TASKS[_TASK]}
+    _ANNO_EXT = ".txt"
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> FormatDetectionConfidence:
         # left color camera label files
-        context.require_file("**/label_2/*.txt")
+        context.require_file(f"**/label_2/*{cls._ANNO_EXT}")
         return cls.DETECT_CONFIDENCE
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class KittiSegmentationImporter(KittiImporter):
     _TASK = KittiTask.segmentation
     _TASKS = {_TASK: KittiImporter._TASKS[_TASK]}
+    _FORMAT_EXT = ".png"
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> FormatDetectionConfidence:
         # instance segmentation masks
-        context.require_file("**/instance/*.png")
+        context.require_file(f"**/instance/*{cls._FORMAT_EXT}")
         return cls.DETECT_CONFIDENCE
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from defusedxml import ElementTree as ET
 
 from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
@@ -275,17 +275,19 @@
                 attributes={"frame": int(frame_id)},
             )
 
         return items
 
 
 class KittiRawImporter(Importer):
+    _ANNO_EXT = ".xml"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_file = context.require_file("*.xml")
+        annot_file = context.require_file(f"*{cls._ANNO_EXT}")
 
         with context.probe_text_file(
             annot_file,
             "must be a KITTI-like annotation file",
         ) as f:
             parser = ET.iterparse(f, events=("start",))
 
@@ -296,7 +298,11 @@
             _, elem = next(parser)
             if elem.tag != "tracklets":
                 raise Exception
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".xml", "kitti_raw")
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/labelme.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 import logging as log
 import os
 import os.path as osp
 from collections import defaultdict
 from glob import glob, iglob
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask, Polygon
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import MediaTypeError
@@ -291,17 +291,19 @@
         return self._categories
 
     def __iter__(self):
         yield from self._items
 
 
 class LabelMeImporter(Importer):
+    _ANNO_EXT = ".xml"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        annot_paths = context.require_files("**/*.xml")
+        annot_paths = context.require_files(f"**/*{cls._ANNO_EXT}")
 
         for annot_path in annot_paths:
             with context.probe_text_file(
                 annot_path,
                 "must be a LabelMe annotation file",
             ) as f:
                 elem_parents = []
@@ -348,14 +350,18 @@
                     "format": LabelMeBase.NAME,
                 }
             )
         except StopIteration:
             pass
         return subsets
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class LabelMeExporter(Exporter):
     DEFAULT_IMAGE_EXT = LabelMePath.IMAGE_EXT
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/lfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
 import re
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories, Points
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
@@ -231,14 +231,18 @@
     @classmethod
     def find_sources(cls, path):
         base, ext = osp.splitext(LfwPath.PAIRS_FILE)
         return cls._find_sources_recursive(
             path, ext, "lfw", filename=base, dirname=LfwPath.ANNOTATION_DIR
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(LfwPath.PAIRS_FILE)[1]]
+
 
 class LfwExporter(Exporter):
     DEFAULT_IMAGE_EXT = LfwPath.IMAGE_EXT
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import glob
 import logging as log
 import os.path as osp
+from typing import List
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME
 from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.importer import Importer
 from datumaro.util import str_to_bool
 
 from .base import MapillaryVistasInstancesBase, MapillaryVistasPanopticBase
@@ -109,14 +110,18 @@
 
             for ann_path in glob.glob(osp.join(path, "*", suffix)):
                 subset = osp.dirname(osp.dirname(osp.relpath(ann_path, path)))
                 subsets.setdefault(subset, {})[task] = osp.join(path, subset)
 
         return subsets
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [".jpg", ".png", ".json"]
+
 
 class MapillaryVistasInstancesImporter(MapillaryVistasImporter):
     _TASK = MapillaryVistasTask.instances
     _TASKS = {_TASK: MapillaryVistasImporter._TASKS[_TASK]}
 
 
 class MapillaryVistasPanopticImporter(MapillaryVistasImporter):
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/market1501.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
 import re
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
@@ -114,14 +114,18 @@
     def find_sources(cls, path):
         for dirname in os.listdir(path):
             if dirname.startswith(
                 (Market1501Path.BBOX_DIR, Market1501Path.QUERY_DIR, Market1501Path.LIST_PREFIX)
             ):
                 return [{"url": path, "format": Market1501Base.NAME}]
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [".jpg"]
+
 
 class Market1501Exporter(Exporter):
     DEFAULT_IMAGE_EXT = Market1501Path.IMAGE_EXT
 
     def _make_dir_name(self, item):
         dirname = Market1501Path.BBOX_DIR + item.subset
         query = item.attributes.get("query")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mars.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 # SPDX-License-Identifier: MIT
 
 import fnmatch
 import glob
 import logging as log
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset import DatasetItem
 from datumaro.components.dataset_base import DatasetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 
 
 class MarsPath:
     SUBSET_DIR_PATTERN = "bbox_*"
     IMAGE_DIR_PATTERNS = ["[0-9]" * 4, "00-1"]
-    IMAGE_NAME_POSTFIX = "C[0-9]" + "T" + "[0-9]" * 4 + "F" + "[0-9]" * 3 + ".*"
+    IMAGE_NAME_POSTFIX = "C[0-9]" + "T" + "[0-9]" * 4 + "F" + "[0-9]" * 3 + ".jpg"
 
 
 class MarsBase(DatasetBase):
     def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         assert osp.isdir(path), path
         super().__init__(ctx=ctx)
 
@@ -137,7 +137,11 @@
 
         for pattern in patterns:
             try:
                 next(glob.iglob(pattern))
                 return [{"url": path, "format": "mars"}]
             except StopIteration:
                 continue
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(MarsPath.IMAGE_NAME_POSTFIX)[1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mmdet.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mmdet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mnist.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import gzip
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
@@ -122,24 +122,30 @@
                 i = meta[i][0]
 
             items[i] = DatasetItem(id=i, subset=self._subset, media=image, annotations=annotations)
         return items
 
 
 class MnistImporter(Importer):
+    _FORMAT_EXT = ".gz"
+
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(
             path,
-            ".gz",
+            cls._FORMAT_EXT,
             "mnist",
             file_filter=lambda p: 1 < len(osp.basename(p).split("-"))
             and osp.basename(p).split("-")[1] == "labels",
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
+
 
 class MnistExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
@@ -112,21 +112,29 @@
 
             items[i] = DatasetItem(id=i, subset=self._subset, media=image, annotations=item_anno)
         return items
 
 
 class MnistCsvImporter(Importer):
     DETECT_CONFIDENCE = FormatDetectionConfidence.MEDIUM
+    _ANNO_EXT = ".csv"
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(
-            path, ".csv", "mnist_csv", file_filter=lambda p: osp.basename(p).find("mnist_") != -1
+            path,
+            cls._ANNO_EXT,
+            "mnist_csv",
+            file_filter=lambda p: osp.basename(p).find("mnist_") != -1,
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class MnistCsvExporter(Exporter):
     DEFAULT_IMAGE_EXT = ".png"
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mot.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,24 +223,34 @@
             "imwidth",
             "imheight",
             "imext",
         }, seq_info
 
 
 class MotSeqImporter(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file("gt/gt.txt")
+        context.require_file(f"gt/gt{cls._ANNO_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(
-            path, ".txt", "mot_seq", dirname="gt", filename=osp.splitext(MotPath.GT_FILENAME)[0]
+            path,
+            cls._ANNO_EXT,
+            "mot_seq",
+            dirname="gt",
+            filename=osp.splitext(MotPath.GT_FILENAME)[0],
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class MotSeqGtExporter(Exporter):
     DEFAULT_IMAGE_EXT = MotPath.IMAGE_EXT
 
     def _apply_impl(self):
         extractor = self._extractor
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mots.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Implements MOTS format https://www.vision.rwth-aachen.de/page/mots
 
 import logging as log
 import os
 import os.path as osp
 from enum import Enum
 from glob import iglob
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
@@ -145,14 +145,18 @@
             for p in os.listdir(path):
                 detected = MotsPngExtractor.detect_dataset(osp.join(path, p))
                 for s in detected:
                     s.setdefault("options", {})["subset"] = p
                 subsets.extend(detected)
         return subsets
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [".png", ".txt"]
+
 
 class MotsPngExporter(Exporter):
     DEFAULT_IMAGE_EXT = MotsPath.IMAGE_EXT
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     LabelCategories,
@@ -169,7 +169,11 @@
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".json", "mpii_json")
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         context.require_file(MpiiJsonPath.ANNOTATION_FILE)
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(MpiiJsonPath.ANNOTATION_FILE)[1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import scipy.io as spio
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     LabelCategories,
@@ -138,14 +138,20 @@
                 annotations=annotations,
             )
 
         return items
 
 
 class MpiiImporter(Importer):
+    _FORMAT_EXT = ".mat"
+
     @classmethod
     def find_sources(cls, path):
-        return cls._find_sources_recursive(path, ".mat", "mpii")
+        return cls._find_sources_recursive(path, cls._FORMAT_EXT, "mpii")
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file("*.mat")
+        context.require_file(f"*{cls._FORMAT_EXT}")
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from glob import glob
+from typing import List
 
 from datumaro.components.format_detection import FormatDetectionConfidence
 from datumaro.components.importer import Importer
 
 from .format import MvtecPath, MvtecTask
 
 
@@ -36,14 +37,18 @@
                             "format": extractor_type,
                             "options": dict({"merge_policy": "union"}),
                         }
                     )
 
         return sources
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [".png"]
+
 
 class MvtecClassificationImporter(MvtecImporter):
     DETECT_CONFIDENCE = FormatDetectionConfidence.MEDIUM
     _TASK = MvtecTask.classification
     _TASKS = {_TASK: MvtecImporter._TASKS[_TASK]}
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import glob
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 import h5py
 import numpy as np
 
 from datumaro.components.annotation import DepthAnnotation
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
@@ -48,14 +48,20 @@
                 annotations=[DepthAnnotation(image=Image.from_numpy(data=depth))],
             )
 
         return items
 
 
 class NyuDepthV2Importer(Importer):
+    _FORMAT_EXT = ".h5"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file("*.h5")
+        context.require_file(f"*{cls._FORMAT_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         return [{"url": path, "format": "nyu_depth_v2"}]
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/open_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import itertools
 import json
 import logging as log
 import os
 import os.path as osp
 import re
 import types
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 import cv2
 import numpy as np
 from attr import attrs
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
@@ -614,14 +614,18 @@
         for pattern in cls.POSSIBLE_ANNOTATION_PATTERNS:
             if glob.glob(osp.join(glob.escape(path), OpenImagesPath.ANNOTATIONS_DIR, pattern)):
                 return [{"url": path, "format": OpenImagesBase.NAME}]
             elif glob.glob(osp.join(glob.escape(path), pattern)):
                 return [{"url": path, "format": OpenImagesBase.NAME}]
         return []
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list({osp.splitext(p)[1] for p in cls.POSSIBLE_ANNOTATION_PATTERNS})
+
 
 class _LazyCsvDictWriter:
     """
     For annotation files, we only learn that the file is required after
     we find at least one occurrence of the corresponding annotation type.
     However, it's convenient to create the writer ahead of time, so that
     it can be used in a `with` statement.
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/base_tfrecord.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import re
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.lazy_plugin import extra_deps
 from datumaro.plugins.data_formats.tf_detection_api.base import TfDetectionApiBase
 from datumaro.plugins.data_formats.tf_detection_api.format import TfrecordImporterType
 from datumaro.util.tf_util import has_feature
 from datumaro.util.tf_util import import_tf as _import_tf
 
 tf = _import_tf()
 
 
 @extra_deps("tensorflow")
 class RoboflowTfrecordImporter(Importer):
+    _ANNO_EXT = ".tfrecord"
+
     @classmethod
     def find_sources(cls, path):
         sources = cls._find_sources_recursive(
             path=path,
-            ext=".tfrecord",
+            ext=cls._ANNO_EXT,
             extractor_name="roboflow_tfrecord",
         )
         if len(sources) == 0:
             return []
 
         undesired_feature = {
             "image/source_id": tf.io.FixedLenFeature([], tf.string),
@@ -48,14 +50,18 @@
                 },
             }
             for subset, url in subsets.items()
         ]
 
         return sources
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class RoboflowTfrecordBase(TfDetectionApiBase):
     def __init__(
         self,
         path: str,
         *,
         subset: Optional[str] = None,
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,18 @@
             subset_name = osp.basename(osp.dirname(subset_path))
             sources.append(
                 {"url": subset_path, "format": cls.FORMAT, "options": {"subset": subset_name}}
             )
 
         return sources
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(cls.ANN_FILE_NAME)[1]]
+
     @property
     def can_stream(self) -> bool:
         return True
 
     def get_extractor_merger(self) -> Type[ExtractorMerger]:
         return ExtractorMerger
 
@@ -128,14 +132,18 @@
                 },
             }
             for subset, url in subsets.items()
         ]
 
         return sources
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls.FORMAT_EXT]
+
 
 class RoboflowYoloImporter(RoboflowVocImporter):
     FORMAT = "roboflow_yolo"
     FORMAT_EXT = ".txt"
     ANN_DIR_NAME = "labels/"
 
     @classmethod
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 from datumaro.rust_api import JsonSectionPageMapper
 from datumaro.util import parse_json
 
 
 class SegmentAnythingImporter(Importer):
     _N_JSON_TO_TEST = 10
     _MAX_ANNOTATION_SECTION_BYTES = 100 * 1024 * 1024  # 100 MiB
+    _ANNO_EXT = ".json"
 
     @classmethod
     def detect(
         cls,
         context: FormatDetectionContext,
     ) -> Optional[FormatDetectionConfidence]:
         # test maximum 10 annotation files only
         ctr = 0
-        for file in context.require_files_iter("*.json"):
+        for file in context.require_files_iter(f"*{cls._ANNO_EXT}"):
             ctr += 1
             with context.probe_text_file(
                 file, "Annotation format is not Segmentat-Anything format", is_binary_file=True
             ) as f:
                 fpath = os.path.join(context.root_path, file)
                 page_mapper = JsonSectionPageMapper(fpath)
                 sections = page_mapper.sections()
@@ -63,7 +64,11 @@
                 break
 
     @classmethod
     def find_sources(cls, path) -> List[Dict]:
         if not os.path.isdir(path):
             return []
         return [{"url": path, "format": cls.NAME}]
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
 from glob import iglob
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import InvalidFieldError, UndeclaredLabelError
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image, PointCloud
 from datumaro.util import parse_json_file
@@ -183,11 +183,16 @@
             )
 
         return parsed
 
 
 class SuperviselyPointCloudImporter(Importer):
     NAME = "sly_pointcloud"
+    _ANNO_EXT = ".json"
 
     @classmethod
     def find_sources(cls, path):
-        return cls._find_sources_recursive(path, ".json", "sly_pointcloud", filename="meta")
+        return cls._find_sources_recursive(path, cls._ANNO_EXT, "sly_pointcloud", filename="meta")
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (C) 2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
+from typing import List
 
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 
 from .format import SynthiaAlPath, SynthiaFormatType, SynthiaRandPath, SynthiaSfPath
 
 
@@ -22,14 +23,18 @@
 
         return FormatDetectionConfidence.MEDIUM
 
     @classmethod
     def find_sources(cls, path):
         return [{"url": path, "format": cls.FORMAT}]
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [".png"]
+
 
 class SynthiaRandImporter(_SynthiaImporter):
     FORMAT = SynthiaFormatType.synthia_rand.name
     META_FOLDERS = SynthiaRandPath.meta_folders()
 
 
 class SynthiaSfImporter(_SynthiaImporter):
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tabular.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tabular.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,18 @@
             if ext in TABULAR_EXTENSIONS:
                 return [{"url": path, "format": TabularDataBase.NAME}]
         else:
             for _ in find_files(path, TABULAR_EXTENSIONS):  # find 1 depth only.
                 return [{"url": path, "format": TabularDataBase.NAME}]
         return []
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list({f".{ext}" for ext in TABULAR_EXTENSIONS})
+
 
 class TabularDataExporter(Exporter):
     """
     Export a tabular dataset.
     This will save each subset into a '.csv' file regardless of 'save_media' value
     """
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
 import re
 from collections import OrderedDict
-from typing import Optional
+from typing import List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.lazy_plugin import extra_deps
@@ -196,19 +196,21 @@
             )
 
         return dataset_items, dataset_labels
 
 
 @extra_deps("tensorflow")
 class TfDetectionApiImporter(Importer):
+    _FORMAT_EXT = ".tfrecord"
+
     @classmethod
     def find_sources(cls, path):
         sources = cls._find_sources_recursive(
             path=path,
-            ext=".tfrecord",
+            ext=cls._FORMAT_EXT,
             extractor_name="tf_detection_api",
         )
         if len(sources) == 0:
             return []
 
         desired_feature = {
             "image/source_id": tf.io.FixedLenFeature([], tf.string),
@@ -225,7 +227,11 @@
                 "url": url,
                 "format": "tf_detection_api",
             }
             for _, url in subsets.items()
         ]
 
         return sources
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import csv
 import errno
 import os
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Points
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import (
     AnnotationExportError,
     DatasetImportError,
     InvalidAnnotationError,
@@ -194,20 +194,22 @@
                             label=label,
                         )
                     )
         return items
 
 
 class VggFace2Importer(Importer):
+    _ANNO_EXT = ".csv"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         with context.require_any():
             for prefix in (VggFace2Path.BBOXES_FILE, VggFace2Path.LANDMARKS_FILE):
                 with context.alternative():
-                    context.require_file(f"{VggFace2Path.ANNOTATION_DIR}/{prefix}*.csv")
+                    context.require_file(f"{VggFace2Path.ANNOTATION_DIR}/{prefix}*{cls._ANNO_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         if osp.isdir(path):
             annotation_dir = osp.join(path, VggFace2Path.ANNOTATION_DIR)
             if osp.isdir(annotation_dir):
                 return [
@@ -225,14 +227,18 @@
                     {
                         "url": path,
                         "format": VggFace2Base.NAME,
                     }
                 ]
         return []
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class VggFace2Exporter(Exporter):
     DEFAULT_IMAGE_EXT = VggFace2Path.IMAGE_EXT
 
     def _apply_impl(self):
         def _get_name_id(item_parts, label_name):
             if 1 < len(item_parts) and item_parts[0] == label_name:
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
-from typing import Optional, Tuple
+from typing import List, Optional, Tuple
 
 import cv2
 import numpy as np
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
@@ -93,14 +93,18 @@
 
     @classmethod
     def find_sources(cls, path):
         if not osp.isfile(path):
             return []
         return [{"url": path, "format": VideoFramesBase.NAME}]
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list({f".{ext}" for ext in VIDEO_EXTENSIONS})
+
 
 class VideoFramesBase(DatasetBase):
     def __init__(
         self,
         url: str,
         *,
         name_pattern: str = "%06d",
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
-from typing import Optional, Type
+from typing import List, Optional, Type
 
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import Importer
 from datumaro.components.merge.extractor_merger import ExtractorMerger
 
 from .format import VocPath, VocTask
 
@@ -18,27 +18,30 @@
         VocTask.voc_classification: ("voc_classification", "Main"),
         VocTask.voc_detection: ("voc_detection", "Main"),
         VocTask.voc_segmentation: ("voc_segmentation", "Segmentation"),
         VocTask.voc_instance_segmentation: ("voc_instance_segmentation", "Segmentation"),
         VocTask.voc_layout: ("voc_layout", "Layout"),
         VocTask.voc_action: ("voc_action", "Action"),
     }
+    ANNO_EXT = ".txt"
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         # The `voc` format is inherently ambiguous with `voc_classification`,
         # `voc_detection`, etc. To remove the ambiguity (and thus make it
         # possible to use autodetection with the VOC datasets), disable
         # autodetection for the single-task formats.
 
         with context.require_any():
             task_dirs = {task_dir for _, task_dir in cls._TASKS.values()}
             for task_dir in sorted(task_dirs):
                 with context.alternative():
-                    context.require_file(osp.join(VocPath.SUBSETS_DIR, task_dir, "*.txt"))
+                    context.require_file(
+                        osp.join(VocPath.SUBSETS_DIR, task_dir, f"*{cls.ANNO_EXT}")
+                    )
 
     @classmethod
     def find_sources(cls, path):
         subsets = []
 
         # find root path for the dataset and use it for all tasks
         root_path = None
@@ -68,14 +71,18 @@
     @property
     def can_stream(self) -> bool:
         return True
 
     def get_extractor_merger(self) -> Optional[Type[ExtractorMerger]]:
         return ExtractorMerger
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls.ANNO_EXT]
+
 
 class VocImporter(_VocImporter):
     _TASK = VocTask.voc
     _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
 
 
 class VocClassificationImporter(_VocImporter):
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import csv
 import errno
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
@@ -87,7 +87,11 @@
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".csv", "vott_csv")
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         context.require_file("*" + VottCsvPath.ANNO_FILE_SUFFIX)
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(VottCsvPath.ANNO_FILE_SUFFIX)[1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os.path as osp
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import parse_json_file
@@ -109,7 +109,11 @@
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(path, ".json", "vott_json")
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         context.require_file("*" + VottJsonPath.ANNO_FILE_SUFFIX)
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [osp.splitext(VottJsonPath.ANNO_FILE_SUFFIX)[1]]
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/widerface.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import os
 import os.path as osp
 import re
-from typing import Optional
+from typing import List, Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import ImportContext, Importer
@@ -167,24 +167,30 @@
                         )
                     )
 
         return items
 
 
 class WiderFaceImporter(Importer):
+    _ANNO_EXT = ".txt"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file(f"{WiderFacePath.ANNOTATIONS_DIR}/*.txt")
+        context.require_file(f"{WiderFacePath.ANNOTATIONS_DIR}/*{cls._ANNO_EXT}")
 
     @classmethod
     def find_sources(cls, path):
         return cls._find_sources_recursive(
-            path, ".txt", "wider_face", dirname=WiderFacePath.ANNOTATIONS_DIR
+            path, cls._ANNO_EXT, "wider_face", dirname=WiderFacePath.ANNOTATIONS_DIR
         )
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._ANNO_EXT]
+
 
 class WiderFaceExporter(Exporter):
     DEFAULT_IMAGE_EXT = WiderFacePath.IMAGE_EXT
 
     def _apply_impl(self):
         if self._extractor.media_type() and not issubclass(self._extractor.media_type(), Image):
             raise MediaTypeError("Media type is not an image")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/kaggle/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,413 +1,524 @@
-# Copyright (C) 2019-2023 Intel Corporation
+# Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from __future__ import annotations
-
+import os
 import os.path as osp
-from collections import OrderedDict
-from typing import Dict, Iterator, List, Optional, Type, TypeVar, Union
-
-import yaml
-
-from datumaro.components.annotation import Annotation, AnnotationType, Bbox, LabelCategories
-from datumaro.components.dataset_base import CategoriesInfo, DatasetBase, DatasetItem, SubsetBase
-from datumaro.components.errors import (
-    DatasetImportError,
-    InvalidAnnotationError,
-    UndeclaredLabelError,
+import re
+import warnings
+from typing import Dict, Optional, Type, TypeVar, Union
+
+import numpy as np
+import pandas as pd
+from defusedxml import ElementTree
+
+from datumaro.components.annotation import (
+    AnnotationType,
+    Bbox,
+    Label,
+    LabelCategories,
+    Mask,
+    MaskCategories,
 )
+from datumaro.components.dataset import DatasetItem
+from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetBase, SubsetBase
+from datumaro.components.errors import InvalidAnnotationError, InvalidFieldError, MissingFieldError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, ImageFromFile
-from datumaro.util.image import (
-    DEFAULT_IMAGE_META_FILE_NAME,
-    IMAGE_EXTENSIONS,
-    ImageMeta,
-    load_image_meta_file,
-)
-from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
-from datumaro.util.os_util import extract_subset_name_from_parent, find_files, split_path
-
-from .format import YoloLoosePath, YoloPath, YoloUltralyticsPath
+from datumaro.plugins.data_formats.coco.base import CocoInstancesBase
+from datumaro.plugins.data_formats.coco.format import CocoTask
+from datumaro.plugins.data_formats.coco.page_mapper import COCOPageMapper
+from datumaro.util import parse_json_file
+from datumaro.util.image import IMAGE_EXTENSIONS, load_image
 
 T = TypeVar("T")
 
-__all__ = ["YoloStrictBase", "YoloLooseBase", "YoloUltralyticsBase"]
 
+class KaggleImageCsvBase(DatasetBase):
+    def __init__(
+        self,
+        path: str,
+        ann_file: str,
+        columns: Dict[str, str],
+        *,
+        subset: Optional[str] = DEFAULT_SUBSET_NAME,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(ctx=ctx)
+
+        self._subset = subset
+        self._path = path
+
+        if "media" not in columns:
+            raise MissingFieldError("media")
+
+        self._label_cat = LabelCategories()
+        self._items = self._load_items(ann_file, columns)
+        self._categories = {AnnotationType.label: self._label_cat}
+
+    def _get_media_path(self, media_name: str):
+        media_path = osp.join(self._path, media_name)
+        if osp.exists(media_path):
+            return media_path
+
+        for ext in IMAGE_EXTENSIONS:
+            media_path_with_ext = media_path + ext
+            if osp.exists(media_path_with_ext):
+                return media_path_with_ext
 
-def localize_path(path: str) -> str:
-    """
-    Removes the "data/" prefix from the path
-    """
+        return None
+
+    def _parse_bbox_coords(self, bbox_str):
+        coords = re.findall(r"[-+]?\d*\.\d+|\d+", bbox_str)
+        if len(coords) != 4:
+            raise ValueError("Bounding box coordinates must have exactly 4 values.")
+
+        # expected to output [x1, y1, x2, y2]
+        return [float(coord.strip()) for coord in coords]
+
+    def _load_annotations(self, datas: list, indices: Dict[str, int], bbox_flag: bool):
+        if "label" in indices:
+            label_name = str(datas[indices["label"]])
+            label, cat = self._label_cat.find(label_name)
+            if not cat:
+                self._label_cat.add(label_name)
+                label, _ = self._label_cat.find(label_name)
+        else:
+            _, cat = self._label_cat.find("object")
+            if not cat:
+                self._label_cat.add("object")
+            label = 0
+
+        if "label" in indices and not bbox_flag:
+            return Label(label=label)
+        if bbox_flag:
+            if "bbox" in indices:
+                coords = self._parse_bbox_coords(datas[indices["bbox"]])
+                return Bbox(
+                    label=label,
+                    x=coords[0],
+                    y=coords[1],
+                    w=coords[2] - coords[0],
+                    h=coords[3] - coords[1],
+                )
+            if "width" in indices and "height" in indices:
+                return Bbox(
+                    label=label,
+                    x=float(datas[indices["x1"]]),
+                    y=float(datas[indices["y1"]]),
+                    w=float(datas[indices["width"]]),
+                    h=float(datas[indices["height"]]),
+                )
+            if "x2" in indices and "y2" in indices:
+                return Bbox(
+                    label=label,
+                    x=float(datas[indices["x1"]]),
+                    y=float(datas[indices["y1"]]),
+                    w=float(datas[indices["x2"]]) - float(datas[indices["x1"]]),
+                    h=float(datas[indices["y2"]]) - float(datas[indices["y1"]]),
+                )
+
+    def _load_items(self, ann_file: str, columns: Dict[str, Union[str, list]]):
+        df = pd.read_csv(ann_file, header=None, on_bad_lines="skip")
+        df_fields = list(df.iloc[0])
+
+        indices = {"media": df_fields.index(columns["media"])}
+        if "label" in columns:
+            indices.update({"label": df_fields.index(columns["label"])})
+
+        bbox_flag = False
+        bbox_index = columns.get("bbox")
+        if bbox_index:
+            bbox_flag = True
+            bbox_indices = {"x1", "x2", "y1", "y2", "width", "height"}
+            if isinstance(bbox_index, str):
+                indices["bbox"] = df_fields.index(bbox_index)
+            elif isinstance(bbox_index, dict):
+                indices.update(
+                    {
+                        key: df_fields.index(bbox_index[key])
+                        for key in bbox_indices
+                        if bbox_index.get(key)
+                    }
+                )
+            if not (
+                {"x1", "x2", "y1", "y2"} <= bbox_indices
+                or {"x1", "y1", "width", "height"} <= bbox_indices
+            ):
+                warnings.warn("Insufficient box coordinate is given for importing bounding boxes.")
+                bbox_flag = False
+
+        items = dict()
+        for _, row in df.iloc[1:].iterrows():  # Skip header row
+            data_info = list(row)
+
+            media_name = data_info[indices["media"]]
+            item_id = osp.splitext(media_name)[0]
+
+            media_path = self._get_media_path(media_name)
+            if not osp.exists(media_path):
+                warnings.warn(
+                    f"'{media_path}' is not existed in the directory, "
+                    f"so we skip to create an dataset item according to {row}."
+                )
+                continue
+
+            ann = self._load_annotations(data_info, indices, bbox_flag)
+            if item_id in items:
+                items[item_id].annotations.append(ann)
+            else:
+                items[item_id] = DatasetItem(
+                    id=item_id,
+                    subset=self._subset,
+                    media=Image.from_file(path=media_path),
+                    annotations=[ann],
+                )
+        return items.values()
+
+    def categories(self):
+        return self._categories
 
-    path = osp.normpath(path.strip()).replace("\\", "/")
-    default_base = "data/"
-    if path.startswith(default_base):
-        path = path[len(default_base) :]
-    return path
+    def __iter__(self):
+        yield from self._items
 
 
-# TODO: Need to clean this dirty structure (SubsetBase has _Subset).
-class _Subset(DatasetBase):
+class KaggleImageTxtBase(KaggleImageCsvBase):
     def __init__(
         self,
-        subset_name: str,
         path: str,
-        items: OrderedDict[str, str],
-        categories: CategoriesInfo,
-        image_info: ImageMeta,
+        ann_file: str,
+        columns: Dict[str, int],
+        *,
+        subset: Optional[str] = DEFAULT_SUBSET_NAME,
+        ctx: Optional[ImportContext] = None,
     ):
-        super().__init__()
-        self._subset_name = subset_name
-        self._path = path
-        self._items = items
-        self._categories = categories
-        self._image_info = image_info
-
-    def __iter__(self) -> Iterator[DatasetItem]:
-        for item_id in self._items:
-            item = self._get(item_id)
-            if item is not None:
-                yield item
+        super().__init__(path=path, ann_file=ann_file, columns=columns, subset=subset, ctx=ctx)
 
-    def __len__(self):
-        return len(self._items)
+    def _load_items(self, ann_file: str, columns: Dict[str, Union[int, Dict]]):
+        bbox_flag = False
+        if "bbox" in columns:
+            bbox_flag = True
+            bbox_columns = columns.pop("bbox")
+            if isinstance(bbox_columns, dict):
+                if not (
+                    all(item in bbox_columns for item in ["x1", "x2", "y1", "y2"])
+                    or all(item in bbox_columns for item in ["x1", "y1", "width", "height"])
+                ):
+                    warnings.warn(
+                        "Insufficient box coordinate is given for importing bounding boxes."
+                    )
+                    bbox_flag = False
+                columns.update(bbox_columns)
 
-    def categories(self):
-        return self._parent.categories()
+        items = dict()
+        with open(ann_file, "r", encoding="utf-8") as f:
+            for line in f:
+                line = re.split(r"\s|,", line)
 
-    def _get(self, item_id: str) -> Optional[DatasetItem]:
-        item = self._items.get(item_id)
+                media_name = line[columns["media"]]
+                item_id = osp.splitext(media_name)[0]
 
-        if not isinstance(item, str):
-            return None
+                media_path = self._get_media_path(media_name)
+                if not osp.exists(media_path):
+                    warnings.warn(
+                        f"'{media_path}' is not existed in the directory, "
+                        f"so we skip to create an dataset item according to {line}."
+                    )
+                    continue
+
+                ann = self._load_annotations(line, columns, bbox_flag)
+                if item_id in items:
+                    items[item_id].annotations.append(ann)
+                else:
+                    items[item_id] = DatasetItem(
+                        id=item_id,
+                        subset=self._subset,
+                        media=Image.from_file(path=media_path),
+                        annotations=[ann],
+                    )
 
-        try:
-            image_size = self._image_info.get(item_id)
-            image = Image.from_file(path=osp.join(self._path, item), size=image_size)
+        return items.values()
 
-            anno_path = osp.splitext(image.path)[0] + ".txt"
-            annotations = self._parse_annotations(
-                anno_path,
-                image,
-                label_categories=self._categories[AnnotationType.label],
-            )
 
-            item = DatasetItem(
-                id=item_id, subset=self._subset_name, media=image, annotations=annotations
-            )
-            return item
-        except (UndeclaredLabelError, InvalidAnnotationError) as e:
-            self._ctx.error_policy.report_annotation_error(e, item_id=(item_id, self._subset_name))
-        except Exception as e:
-            self._ctx.error_policy.report_item_error(e, item_id=(item_id, self._subset_name))
+class KaggleImageMaskBase(DatasetBase):
+    def __init__(
+        self,
+        path: str,
+        mask_path: str,
+        labelmap_file: Optional[str] = None,
+        *,
+        subset: Optional[str] = DEFAULT_SUBSET_NAME,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(ctx=ctx)
 
-        return None
+        self._subset = subset
 
-    @classmethod
-    def _parse_annotations(
-        cls,
-        anno_path: str,
-        image: ImageFromFile,
-        *,
-        label_categories: LabelCategories,
-    ) -> List[Annotation]:
-        lines = []
-        with open(anno_path, "r", encoding="utf-8") as f:
-            for line in f:
-                line = line.strip()
-                if line:
-                    lines.append(line)
+        self._path = path
+        self._mask_path = mask_path
 
-        annotations = []
+        self._label_ids = []
+        self._categories = self._load_categories(labelmap_file)
+        self._items = self._load_items()
+
+    def _load_categories(self, label_map_file: Optional[str]):
+        label_map = dict()
+        if not label_map_file:
+            label_map["background"] = (0, 0, 0)
+            label_map["object"] = (255, 255, 255)
+        else:
+            df = pd.read_csv(label_map_file)
+            for _, row in df.iterrows():
+                name = row[0]
+                color = tuple([int(c) for c in row[1:]])
+                label_map[name] = color
 
-        if lines:
-            # Use image info as late as possible to avoid unnecessary image loading
-            if image.size is None:
-                raise DatasetImportError(f"Can't find image info for '{localize_path(image.path)}'")
-            image_height, image_width = image.size
+        label_categories = LabelCategories()
+        for label in label_map:
+            label_categories.add(label)
 
-        for idx, line in enumerate(lines):
-            parts = line.split()
-            if len(parts) != 5:
-                raise InvalidAnnotationError(
-                    f"Unexpected field count {len(parts)} in the bbox description. "
-                    "Expected 5 fields (label, xc, yc, w, h)."
-                )
-            label_id, xc, yc, w, h = parts
+        categories = {}
+        categories[AnnotationType.label] = label_categories
 
-            label_id = cls._parse_field(label_id, int, "bbox label id")
-            if label_id not in label_categories:
-                raise UndeclaredLabelError(str(label_id))
-
-            w = cls._parse_field(w, float, "bbox width")
-            h = cls._parse_field(h, float, "bbox height")
-            x = cls._parse_field(xc, float, "bbox center x") - w * 0.5
-            y = cls._parse_field(yc, float, "bbox center y") - h * 0.5
-            annotations.append(
-                Bbox(
-                    x * image_width,
-                    y * image_height,
-                    w * image_width,
-                    h * image_height,
-                    label=label_id,
-                    id=idx,
-                    group=idx,
+        colormap = {}
+        for label_name, label_color in label_map.items():
+            label_id = label_categories.find(label_name)[0]
+            colormap[label_id] = label_color
+            self._label_ids.append(label_id)
+
+        categories[AnnotationType.mask] = MaskCategories(colormap)
+
+        return categories
+
+    def _load_items(self):
+        def _lazy_extract_mask(mask, c):
+            return lambda: mask == c
+
+        items = []
+        for media_name in sorted(os.listdir(self._path)):
+            id = osp.splitext(media_name)[0]
+
+            anns = []
+            for mask_name in os.listdir(self._mask_path):
+                if id in mask_name:
+                    instances_mask = load_image(
+                        osp.join(self._mask_path, mask_name), dtype=np.int32
+                    )
+                    # label_ids = np.unique(instances_mask)
+                    for label_id in self._label_ids:
+                        anns.append(
+                            Mask(
+                                image=_lazy_extract_mask(instances_mask, label_id),
+                                label=label_id,
+                            )
+                        )
+
+            items.append(
+                DatasetItem(
+                    id=id,
+                    subset=self._subset,
+                    media=Image.from_file(path=osp.join(self._path, media_name)),
+                    annotations=anns,
                 )
             )
 
-        return annotations
+        return items
 
-    @classmethod
-    def _parse_field(cls, value: str, desired_type: Type[T], field_name: str) -> T:
-        try:
-            return desired_type(value)
-        except Exception as e:
-            raise InvalidAnnotationError(
-                f"Can't parse {field_name} from '{value}'. Expected {desired_type}"
-            ) from e
+    def categories(self):
+        return self._categories
+
+    def __iter__(self):
+        yield from self._items
 
 
-class YoloStrictBase(SubsetBase):
+class KaggleVocBase(SubsetBase):
+    ann_extensions = ".xml"
+
     def __init__(
         self,
-        config_path: str,
-        image_info: Union[None, str, ImageMeta] = None,
+        path: str,
+        ann_path: str,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
-        **kwargs,
-    ) -> None:
+    ):
         super().__init__(subset=subset, ctx=ctx)
 
-        if not osp.isfile(config_path):
-            raise DatasetImportError(f"Can't read dataset descriptor file '{config_path}'")
+        self._label_cat = LabelCategories()
+        self._items = []
+        self._size = None
 
-        rootpath = osp.dirname(config_path)
-        self._path = rootpath
+        for img_filename in sorted(os.listdir(path)):
+            if not img_filename.lower().endswith(tuple(IMAGE_EXTENSIONS)):
+                continue
+            item_id = osp.splitext(img_filename)[0]
 
-        self._image_info = self.parse_image_info(rootpath, image_info)
+            img_file = osp.join(path, img_filename)
+            ann_file = osp.join(ann_path, item_id + self.ann_extensions)
 
-        config = YoloPath._parse_config(config_path)
+            annotations = (
+                self._parse_annotations(img_file, ann_file) if osp.isfile(ann_file) else []
+            )
 
-        names_path = config.get("names")
-        if not names_path:
-            raise InvalidAnnotationError("Failed to parse names file path from config")
+            media = Image.from_file(path=img_file, size=self._size)
 
-        self._categories = {
-            AnnotationType.label: self._load_categories(
-                osp.join(self._path, localize_path(names_path))
+            self._items.append(
+                DatasetItem(
+                    id=item_id,
+                    subset=self._subset,
+                    media=media,
+                    annotations=annotations,
+                )
             )
-        }
+        self._categories = {AnnotationType.label: self._label_cat}
 
-        # The original format is like this:
-        #
-        # classes = 2
-        # train  = data/train.txt
-        # valid  = data/test.txt
-        # names = data/obj.names
-        # backup = backup/
-        #
-        # To support more subset names, we disallow subsets
-        # called 'classes', 'names' and 'backup'.
-        subsets = {k: v for k, v in config.items() if k not in YoloPath.RESERVED_CONFIG_KEYS}
-        self._subsets: Dict[str, self._Subset] = {}
+    def _parse_annotations(self, img_file: str, ann_file: str):
+        root_elem = ElementTree.parse(ann_file).getroot()
+        if root_elem.tag != "annotation":
+            raise MissingFieldError("annotation")
+
+        height = self._parse_field(root_elem, "size/height", int, required=False)
+        width = self._parse_field(root_elem, "size/width", int, required=False)
+        if height and width:
+            self._size = (height, width)
 
-        for subset_name, list_path in subsets.items():
-            if subset_name != subset:
-                continue
+        annotations = []
+        for obj_id, object_elem in enumerate(root_elem.iterfind("object")):
+            label_name = self._parse_field(object_elem, "name", str, required=True)
 
-            list_path = osp.join(self._path, localize_path(list_path))
-            if not osp.isfile(list_path):
-                raise InvalidAnnotationError(f"Can't find '{subset_name}' subset list file")
-
-            with open(list_path, "r", encoding="utf-8") as f:
-                items = OrderedDict(
-                    (self.name_from_path(p), localize_path(p)) for p in f if p.strip()
-                )
+            bbox_elem = object_elem.find("bndbox")
+            if not bbox_elem:
+                raise MissingFieldError("bndbox")
+
+            xmin = self._parse_field(bbox_elem, "xmin", float)
+            xmax = self._parse_field(bbox_elem, "xmax", float)
+            ymin = self._parse_field(bbox_elem, "ymin", float)
+            ymax = self._parse_field(bbox_elem, "ymax", float)
+
+            label_id, cat = self._label_cat.find(label_name)
+            if not cat:
+                self._label_cat.add(label_name)
+                label_id, _ = self._label_cat.find(label_name)
 
-            subset = _Subset(
-                subset_name=subset_name,
-                path=self._path,
-                items=items,
-                categories=self._categories,
-                image_info=self._image_info,
+            annotations.append(
+                Bbox(id=obj_id, label=label_id, x=xmin, y=ymin, w=xmax - xmin, h=ymax - ymin)
             )
-            self._subsets[subset_name] = subset
 
-    @staticmethod
-    def parse_image_info(
-        rootpath: str, image_info: Optional[Union[str, ImageMeta]] = None
-    ) -> ImageMeta:
-        assert image_info is None or isinstance(image_info, (str, dict))
-        if image_info is None:
-            image_info = osp.join(rootpath, DEFAULT_IMAGE_META_FILE_NAME)
-            if not osp.isfile(image_info):
-                image_info = {}
-        if isinstance(image_info, str):
-            image_info = load_image_meta_file(image_info)
-
-        return image_info
-
-    @classmethod
-    def name_from_path(cls, path: str) -> str:
-        """
-        Obtains <image name> from the path like [data/]<subset>_obj/<image_name>.ext
-
-        <image name> can be <a/b/c/filename>, so it is
-        more involved than just calling "basename()".
-        """
-
-        path = localize_path(path)
-
-        parts = split_path(path)
-        if 1 < len(parts) and not osp.isabs(path):
-            path = osp.join(*parts[1:])  # pylint: disable=no-value-for-parameter
-
-        return osp.splitext(path)[0]
+        return annotations
 
     @staticmethod
-    def _load_categories(names_path):
-        if has_meta_file(osp.dirname(names_path)):
-            return LabelCategories.from_iterable(parse_meta_file(osp.dirname(names_path)).keys())
+    def _parse_field(root, xpath: str, cls: Type[T] = str, required: bool = True) -> Optional[T]:
+        elem = root.find(xpath)
+        if elem is None:
+            if required:
+                raise MissingFieldError(xpath)
+            else:
+                return None
 
-        label_categories = LabelCategories()
+        if cls is str:
+            return elem.text
 
-        with open(names_path, "r", encoding="utf-8") as f:
-            for label in f:
-                label = label.strip()
-                if label:
-                    label_categories.add(label)
-
-        return label_categories
-
-    def __iter__(self) -> Iterator[DatasetItem]:
-        subsets = self._subsets
-        pbars = self._ctx.progress_reporter.split(len(subsets))
-        for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
-            for item in pbar.iter(subset, desc=f"Importing '{subset_name}'"):
-                yield item
-
-    def __len__(self):
-        return sum(len(s) for s in self._subsets.values())
-
-    def get_subset(self, name):
-        return self._subsets[name]
-
-    @property
-    def is_stream(self) -> bool:
-        return True
+        try:
+            return cls(elem.text)
+        except Exception as e:
+            raise InvalidFieldError(xpath) from e
 
 
-class YoloLooseBase(SubsetBase):
-    META_FILE = YoloLoosePath.NAMES_FILE
+class KaggleYoloBase(KaggleVocBase, SubsetBase):
+    ann_extensions = ".txt"
 
     def __init__(
         self,
-        config_path: str,
-        image_info: Union[None, str, ImageMeta] = None,
-        urls: Optional[List[str]] = None,
+        path: str,
+        ann_path: str,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
-    ) -> None:
-        super().__init__(subset=subset, ctx=ctx)
-
-        if not osp.isdir(config_path):
-            raise DatasetImportError(f"{config_path} should be a directory.")
+    ):
+        super().__init__(path=path, ann_path=ann_path, subset=subset, ctx=ctx)
 
-        rootpath = self._get_rootpath(config_path)
+    def _parse_annotations(self, img_file: str, ann_file: str):
+        image = ImageFromFile(path=img_file)
+        image_height, image_width = image.size
 
-        self._image_info = YoloStrictBase.parse_image_info(rootpath, image_info)
+        lines = []
+        with open(ann_file, "r", encoding="utf-8") as f:
+            for line in f:
+                line = line.strip()
+                if line:
+                    lines.append(line)
 
-        # Init label categories
-        label_categories = self._load_categories(osp.join(rootpath, self.META_FILE))
-        self._categories = {AnnotationType.label: label_categories}
-
-        self._urls = urls
-        self._img_files = self._load_img_files(rootpath)
-
-    def __iter__(self) -> Iterator[DatasetItem]:
-        label_categories = self._categories.get(AnnotationType.label)
-        if label_categories is None:
-            raise DatasetImportError("label_categories should be not None.")
-
-        pbar = self._ctx.progress_reporter
-        for url in pbar.iter(self._urls, desc=f"Importing '{self._subset}'"):
-            try:
-                fname = self._get_fname(url)
-                img = Image.from_file(path=self._img_files[fname])
-                anns = self._parse_annotations(
-                    url,
-                    img,
-                    label_categories=label_categories,
+        annotations = []
+        for obj_id, line in enumerate(lines):
+            parts = line.split()
+            if len(parts) != 5:
+                raise InvalidAnnotationError(
+                    f"Unexpected field count {len(parts)} in the bbox description. "
+                    "Expected 5 fields (label, xc, yc, w, h)."
                 )
-                yield DatasetItem(id=fname, subset=self._subset, media=img, annotations=anns)
-            except Exception as e:
-                self._ctx.error_policy.report_item_error(e, item_id=(fname, self._subset))
-
-    def __len__(self) -> int:
-        return len(self._urls)
-
-    def _get_rootpath(self, config_path: str) -> str:
-        return config_path
-
-    def _load_categories(self, names_path: str) -> LabelCategories:
-        return YoloStrictBase._load_categories(names_path)
-
-    def _get_fname(self, fpath: str) -> str:
-        return osp.splitext(osp.basename(fpath))[0]
-
-    def _load_img_files(self, rootpath: str) -> Dict[str, str]:
-        return {
-            self._get_fname(img_file): img_file
-            for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
-            if extract_subset_name_from_parent(img_file, rootpath) == self._subset
-        }
-
-    def _parse_annotations(
-        self, anno_path: str, image: ImageFromFile, label_categories: LabelCategories
-    ) -> List[Annotation]:
-        return _Subset._parse_annotations(
-            anno_path=anno_path, image=image, label_categories=label_categories
-        )
-
-    def _parse_field(self, value: str, desired_type: Type[T], field_name: str) -> T:
-        return _Subset._parse_field(value=value, desired_type=desired_type, field_name=field_name)
-
-    @property
-    def is_stream(self) -> bool:
-        return True
+            label_name, xc, yc, w, h = parts
+            xc = float(xc)
+            yc = float(yc)
+            w = float(w)
+            h = float(h)
+            x = (xc - w * 0.5) * image_width
+            y = (yc - h * 0.5) * image_height
+            w *= image_width
+            h *= image_height
+
+            label_id, cat = self._label_cat.find(label_name)
+            if not cat:
+                self._label_cat.add(label_name)
+                label_id, _ = self._label_cat.find(label_name)
+            label_id, _ = self._label_cat.find(label_name)
 
+            annotations.append(Bbox(id=obj_id, label=label_id, x=x, y=y, w=w, h=h))
+
+        return annotations
 
-class YoloUltralyticsBase(YoloLooseBase):
-    META_FILE = YoloUltralyticsPath.META_FILE
 
+class KaggleCocoBase(CocoInstancesBase, SubsetBase):
     def __init__(
         self,
-        config_path: str,
-        image_info: Union[None, str, ImageMeta] = None,
-        urls: Optional[List[str]] = None,
-        **kwargs,
-    ) -> None:
-        super().__init__(config_path, image_info, urls, **kwargs)
-
-    def _load_categories(self, names_path: str) -> LabelCategories:
-        if has_meta_file(osp.dirname(names_path)):
-            return LabelCategories.from_iterable(parse_meta_file(osp.dirname(names_path)).keys())
+        path: str,
+        ann_file: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+        stream: bool = False,
+    ):
+        SubsetBase.__init__(self, subset=subset, ctx=ctx)
 
-        label_categories = LabelCategories()
+        self._rootpath = path
+        self._images_dir = path
+        self._path = ann_file
+        self._task = CocoTask.instances
+        self._merge_instance_polygons = False
 
-        with open(names_path, "r") as fp:
-            loaded = yaml.safe_load(fp.read())
-            if isinstance(loaded["names"], list):
-                label_names = loaded["names"]
-            elif isinstance(loaded["names"], dict):
-                label_names = list(loaded["names"].values())
-            else:
-                raise DatasetImportError(f"Can't read dataset category file '{names_path}'")
+        keep_original_category_ids = False
+
+        self._stream = stream
+        if not stream:
+            self._page_mapper = None  # No use in case of stream = False
 
-        for label_name in label_names:
-            label_categories.add(label_name)
+            json_data = parse_json_file(ann_file)
+
+            self._load_categories(
+                json_data,
+                keep_original_ids=keep_original_category_ids,
+            )
+
+            self._items = self._load_items(json_data)
+
+            del json_data
+        else:
+            self._page_mapper = COCOPageMapper(ann_file)
+
+            categories_data = self._page_mapper.stream_parse_categories_data()
+
+            self._load_categories(
+                {"categories": categories_data},
+                keep_original_ids=keep_original_category_ids,
+            )
 
-        return label_categories
+            self._length = None
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,35 +13,42 @@
 from datumaro.components.merge.extractor_merger import ExtractorMerger
 from datumaro.util.os_util import extract_subset_name_from_parent
 
 from .format import YoloFormatType, YoloLoosePath, YoloPath, YoloUltralyticsPath
 
 
 class _YoloStrictImporter(Importer):
+    _FORMAT_EXT = ".data"
+
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
-        context.require_file("obj.data")
+        context.require_file(f"obj{cls._FORMAT_EXT}")
 
     @classmethod
-    def find_sources(cls, path: str) -> List[Dict]:
-        found = cls._find_sources_recursive(path, ".data", YoloFormatType.yolo_strict.name)
-        if len(found) == 0:
-            return []
+    def find_sources(cls, path: str) -> List[Dict[str, Any]]:
+        sources = cls._find_sources_recursive(path, ".data", YoloFormatType.yolo_strict.name)
 
-        config_path = found[0]["url"]
-        config = YoloPath._parse_config(config_path)
-        subsets = [k for k in config if k not in YoloPath.RESERVED_CONFIG_KEYS]
-        return [
-            {
-                "url": config_path,
-                "format": YoloFormatType.yolo_strict.name,
-                "options": {"subset": subset},
-            }
-            for subset in subsets
-        ]
+        def _extract_subset_wise_sources(source) -> List[Dict[str, Any]]:
+            config_path = source["url"]
+            config = YoloPath._parse_config(config_path)
+            subsets = [k for k in config if k not in YoloPath.RESERVED_CONFIG_KEYS]
+            return [
+                {
+                    "url": config_path,
+                    "format": YoloFormatType.yolo_strict.name,
+                    "options": {"subset": subset},
+                }
+                for subset in subsets
+            ]
+
+        return sum([_extract_subset_wise_sources(source) for source in sources], [])
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [cls._FORMAT_EXT]
 
 
 class _YoloLooseImporter(Importer):
     META_FILE = YoloLoosePath.NAMES_FILE
     FORMAT = YoloFormatType.yolo_loose.name
 
     @classmethod
@@ -122,47 +129,60 @@
         ]
         return sources
 
     @classmethod
     def find_sources(cls, path: str) -> List[Dict[str, Any]]:
         # Check obj.names first
         filename, ext = osp.splitext(cls.META_FILE)
-        sources = cls._find_sources_recursive(
+        obj_names_files = cls._find_sources_recursive(
             path,
             ext=ext,
             extractor_name="",
             dirname="",
             filename=filename,
             max_depth=1,
             recursive=False,
         )
-        if len(sources) == 0:
+        if len(obj_names_files) == 0:
             return []
 
-        # TODO: From Python >= 3.8, we can use
-        # "if (sources := cls._find_strict(path)): return sources"
-        sources = cls._find_loose(path, "[Aa]nnotations")
-        if sources:
-            return sources
-
-        sources = cls._find_loose(path, "[Ll]abels")
-        if sources:
-            return sources
+        sources = []
 
-        return []
+        for obj_names_file in obj_names_files:
+            base_path = osp.dirname(obj_names_file["url"])
+            if found := cls._find_loose(base_path, "[Aa]nnotations"):
+                sources += found
+
+            if found := cls._find_loose(path, "[Ll]abels"):
+                sources += found
+
+        return sources
 
     @property
     def can_stream(self) -> bool:
         return True
 
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return [".txt"]
+
 
 class _YoloUltralyticsImporter(_YoloLooseImporter):
     META_FILE = YoloUltralyticsPath.META_FILE
     FORMAT = YoloFormatType.yolo_ultralytics.name
 
+    @classmethod
+    def _check_ann_file_impl(cls, fp: TextIOWrapper) -> bool:
+        try:
+            return _YoloLooseImporter._check_ann_file_impl(fp)
+        except DatasetImportError as e:
+            if e.args[0] == "Empty file is not allowed.":
+                return True
+            raise
+
 
 class YoloImporter(Importer):
     SUB_IMPORTERS: Dict[YoloFormatType, Importer] = {
         YoloFormatType.yolo_strict: _YoloStrictImporter,
         YoloFormatType.yolo_loose: _YoloLooseImporter,
         YoloFormatType.yolo_ultralytics: _YoloUltralyticsImporter,
     }
@@ -175,17 +195,24 @@
                     return importer_cls.detect(context)
 
         context.fail("Any yolo format is not detected.")
 
     @classmethod
     def find_sources(cls, path: str) -> List[Dict[str, Any]]:
         for importer_cls in cls.SUB_IMPORTERS.values():
-            # TODO: From Python >= 3.8, we can use
-            # "if (sources := importer_cls.find_sources(path)): return sources"
-            sources = importer_cls.find_sources(path)
-            if sources:
+            if sources := importer_cls.find_sources(path):
                 return sources
 
         return []
 
     def get_extractor_merger(self) -> Optional[Type[ExtractorMerger]]:
         return ExtractorMerger
+
+    @classmethod
+    def get_file_extensions(cls) -> List[str]:
+        return list(
+            {
+                ext
+                for importer in cls.SUB_IMPORTERS.values()
+                for ext in importer.get_file_extensions()
+            }
+        )
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/explorer.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/framework_converter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/framework_converter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/ndr.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,14 +204,22 @@
         if output_layers:
             log.info(f"Add additional output layers {output_layers} to the model outputs.")
             self._network.add_outputs(output_layers)
 
         self._check_model_support(self._network, self._device)
         self._load_executable_net()
 
+    @property
+    def inputs(self):
+        return self._network.inputs
+
+    @property
+    def outputs(self):
+        return self._network.outputs
+
     def _check_model_support(self, net, device):
         not_supported_layers = set(
             name for name, dev in self._core.query_model(net, device).items() if not dev
         )
         if len(not_supported_layers) != 0:
             log.error(
                 "The following layers are not supported "
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     std = (255 * np.array([0.229, 0.224, 0.225])).reshape(1, 1, 3)
 
     def preprocess(self, inp: DatasetItem) -> Tuple[LauncherInputType, PrepInfo]:
         img = inp.media_as(Image).data
         img = cv2.resize(img, (224, 224))
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         img = (img - self.mean) / self.std
+        if len(img.shape) == 3 and img.shape[2] in {3, 4}:
+            img = np.transpose(img, (2, 0, 1))
         return img, None
 
     def postprocess(self, pred: ModelPred, info: PrepInfo) -> List[Annotation]:
         feature_vector = pred.get("output")
         if feature_vector is None:
             raise DatumaroError('"output" key should exist in the model prediction.')
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,36 +8,47 @@
 
 from datumaro.components.abstracts import IModelInterpreter
 from datumaro.components.abstracts.model_interpreter import LauncherInputType, ModelPred, PrepInfo
 from datumaro.components.annotation import (
     Annotation,
     AnnotationType,
     FeatureVector,
+    Label,
     LabelCategories,
 )
 from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import DatumaroError
 from datumaro.components.media import Image
 
 
 class GooglenetV4TfModelInterpreter(IModelInterpreter):
+    LOGIT_KEY = "InceptionV4/Logits/Predictions"
     FEAT_KEY = "InceptionV4/Logits/PreLogitsFlatten/flatten_1/Reshape:0"
 
     def preprocess(self, inp: DatasetItem) -> Tuple[LauncherInputType, PrepInfo]:
         img = inp.media_as(Image).data
         img = cv2.resize(img, (299, 299))
         img = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
         return img, None
 
     def postprocess(self, pred: ModelPred, info: PrepInfo) -> List[Annotation]:
+        logit = pred.get(self.LOGIT_KEY)
+        if logit is None:
+            raise DatumaroError(f'"{self.LOGIT_KEY}" key should exist in the model prediction.')
+
         feature_vector = pred.get(self.FEAT_KEY)
         if feature_vector is None:
             raise DatumaroError(f'"{self.FEAT_KEY}" key should exist in the model prediction.')
 
-        return [FeatureVector(feature_vector)]
+        outputs = [
+            Label(label=label, attributes={"score": score}) for label, score in enumerate(logit)
+        ]
+        outputs += [FeatureVector(feature_vector)]
+
+        return outputs  # [FeatureVector(logit), FeatureVector(feature_vector)]
 
     def get_categories(self):
         # output categories - label map etc.
 
         label_categories = LabelCategories()
 
         with open("samples/imagenet.class", "r", encoding="utf-8") as file:
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/automatic_mask_gen.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/bbox_to_inst_mask.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_amg.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_decoder_for_bbox.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sam_transforms/interpreters/sam_encoder.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/specs.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/specs.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
 
 def get_lazy_plugins():
     return [
         plugin
         for plugin in [
             get_lazy_plugin(
-                spec["import_path"], spec["plugin_name"], spec["plugin_type"], spec["extra_deps"]
+                spec["import_path"],
+                spec["plugin_name"],
+                spec["plugin_type"],
+                spec.get("extra_deps", []),
+                spec.get("metadata", {}),
             )
             for spec in parse_json_file(str(_SPECS_JSON_PATH))
         ]
         if plugin is not None
     ]
 
 
@@ -35,22 +39,26 @@
     def _enroll_to_plugin_specs(plugins, plugin_type):
         global plugin_specs
 
         for _, plugin in plugins.items():
             mod = plugin.__module__
             class_name = plugin.__name__
             plugin_name = plugin.NAME
-            plugin_specs += [
-                {
-                    "import_path": f"{mod}.{class_name}",
-                    "plugin_name": plugin_name,
-                    "plugin_type": plugin_type,
-                    "extra_deps": get_extra_deps(plugin),
-                }
-            ]
+            extra_deps = get_extra_deps(plugin)
+            plugin_spec = {
+                "import_path": f"{mod}.{class_name}",
+                "plugin_name": plugin_name,
+                "plugin_type": plugin_type,
+            }
+            if extra_deps:
+                plugin_spec["extra_deps"] = extra_deps
+            # Setting metadata for importers
+            if hasattr(plugin, "get_file_extensions"):
+                plugin_spec["metadata"] = {"file_extensions": sorted(plugin.get_file_extensions())}
+            plugin_specs.append(plugin_spec)
 
     _enroll_to_plugin_specs(env.extractors, "DatasetBase")
     _enroll_to_plugin_specs(env.importers, "Importer")
     _enroll_to_plugin_specs(env.launchers, "Launcher")
     _enroll_to_plugin_specs(env.exporters, "Exporter")
     _enroll_to_plugin_specs(env.generators, "DatasetGenerator")
     _enroll_to_plugin_specs(env.transforms, "Transform")
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/splitter.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/tiling/util.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/transforms.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1065,14 +1065,24 @@
             rescaled_mask = cv2.resize(
                 mask.image.astype(np.float32), new_size[::-1], interpolation=cv2.INTER_NEAREST
             )
             return rescaled_mask.astype(np.uint8)
 
         return _resize_image
 
+    @staticmethod
+    def _lazy_resize_rlemask(mask, new_size):
+        def _resize_image():
+            # Can use only NEAREST for masks,
+            # because we can't have interpolated values
+            rescaled_mask = cv2.resize(mask.image, new_size[::-1], interpolation=cv2.INTER_NEAREST)
+            return mask_utils.encode(np.asfortranarray(rescaled_mask.astype(np.uint8)))
+
+        return _resize_image
+
     def transform_item(self, item):
         if not isinstance(item.media, Image):
             raise DatumaroError(
                 "Item %s: image info is required for this " "transform" % (item.id,)
             )
 
         h, w = item.media.size
@@ -1102,14 +1112,17 @@
                         points=[
                             p
                             for t in ((x * xscale, y * yscale) for x, y in take_by(ann.points, 2))
                             for p in t
                         ]
                     )
                 )
+            elif isinstance(ann, RleMask):
+                rescaled_mask = self._lazy_resize_rlemask(ann, new_size)
+                resized_annotations.append(ann.wrap(rle=rescaled_mask))
             elif isinstance(ann, Mask):
                 rescaled_mask = self._lazy_resize_mask(ann, new_size)
                 resized_annotations.append(ann.wrap(image=rescaled_mask))
             elif isinstance(ann, (Caption, Label)):
                 resized_annotations.append(ann)
             else:
                 assert False, f"Unexpected annotation type {type(ann)}"
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/plugins/validators.py` & `datumaro-1.6.1rc1/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/__init__.py` & `datumaro-1.6.1rc1/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/annotation_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/attrs_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/definitions.py` & `datumaro-1.6.1rc1/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/file_utils.py` & `datumaro-1.6.1rc1/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/image.py` & `datumaro-1.6.1rc1/src/datumaro/util/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# Copyright (C) 2019-2023 Intel Corporation
+# Copyright (C) 2019-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 from __future__ import annotations
 
-import importlib
 import os
 import os.path as osp
 import shlex
 import weakref
 from contextlib import contextmanager
 from contextvars import ContextVar
 from enum import Enum, auto
@@ -22,109 +21,138 @@
 try:
     # Introduced in 1.20
     from numpy.typing import DTypeLike
 except ImportError:
     DTypeLike = Any
 
 
-class _IMAGE_BACKENDS(Enum):
+class ImageBackend(Enum):
     cv2 = auto()
     PIL = auto()
 
 
-_IMAGE_BACKEND: ContextVar[_IMAGE_BACKENDS] = ContextVar("_IMAGE_BACKENDS")
+IMAGE_BACKEND: ContextVar[ImageBackend] = ContextVar("IMAGE_BACKEND")
 _image_loading_errors = (FileNotFoundError,)
 try:
-    importlib.import_module("cv2")
-    _IMAGE_BACKEND.set(_IMAGE_BACKENDS.cv2)
+    import cv2
+
+    IMAGE_BACKEND.set(ImageBackend.cv2)
 except ModuleNotFoundError:
     import PIL
 
-    _IMAGE_BACKEND.set(_IMAGE_BACKENDS.PIL)
+    IMAGE_BACKEND.set(ImageBackend.PIL)
     _image_loading_errors = (*_image_loading_errors, PIL.UnidentifiedImageError)
 
 from datumaro.util.image_cache import ImageCache
 from datumaro.util.os_util import find_files
 
 if TYPE_CHECKING:
     from PIL.Image import Image as PILImage
 
 
-class ImageColorScale(Enum):
-    """Image color scale
+class ImageColorChannel(Enum):
+    """Image color channel
 
-    - UNCHANGED: Use the original image's scale (default)
-    - COLOR: Use 3 channels (it can ignore the alpha channel or convert the gray scale image to BGR)
+    - UNCHANGED: Use the original image's channel (default)
+    - COLOR_BGR: Use BGR 3 channels (it can ignore the alpha channel or convert the gray scale image)
+    - COLOR_RGB: Use RGB 3 channels (it can ignore the alpha channel or convert the gray scale image)
     """
 
     UNCHANGED = 0
-    COLOR = 1
+    COLOR_BGR = 1
+    COLOR_RGB = 2
 
-    def convert_cv2(self, img: np.ndarray) -> np.ndarray:
-        import cv2
+    def decode_by_cv2(self, image_bytes: bytes) -> np.ndarray:
+        """Convert image color channel for OpenCV image (np.ndarray)."""
+        image_buffer = np.frombuffer(image_bytes, dtype=np.uint8)
+
+        if self == ImageColorChannel.UNCHANGED:
+            return cv2.imdecode(image_buffer, cv2.IMREAD_UNCHANGED)
+
+        img = cv2.imdecode(image_buffer, cv2.IMREAD_COLOR)
+
+        if self == ImageColorChannel.COLOR_BGR:
+            return img
+
+        if self == ImageColorChannel.COLOR_RGB:
+            return cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
+
+        raise ValueError
+
+    def decode_by_pil(self, image_bytes: bytes) -> PILImage:
+        """Convert image color channel for PIL Image."""
+        from PIL import Image
 
-        if self == ImageColorScale.COLOR:
-            return cv2.imdecode(img, cv2.IMREAD_COLOR)
+        img = Image.open(BytesIO(image_bytes))
 
-        return cv2.imdecode(img, cv2.IMREAD_UNCHANGED)
+        if self == ImageColorChannel.UNCHANGED:
+            return img
 
-    def convert_pil(self, img: PILImage) -> PILImage:
-        if self == ImageColorScale.COLOR:
+        if self == ImageColorChannel.COLOR_BGR:
+            return Image.fromarray(np.flip(np.asarray(img.convert("RGB")), -1))
+
+        if self == ImageColorChannel.COLOR_RGB:
             return img.convert("RGB")
 
-        return img
+        raise ValueError
 
 
-IMAGE_COLOR_SCALE: ContextVar[ImageColorScale] = ContextVar(
-    "IMAGE_COLOR_SCALE", default=ImageColorScale.UNCHANGED
+IMAGE_COLOR_CHANNEL: ContextVar[ImageColorChannel] = ContextVar(
+    "IMAGE_COLOR_CHANNEL", default=ImageColorChannel.UNCHANGED
 )
 
 
 @contextmanager
-def decode_image_context(color_scale: ImageColorScale):
-    """Change Datumaro image decoding color scale.
+def decode_image_context(image_backend: ImageBackend, image_color_channel: ImageColorChannel):
+    """Change Datumaro image color channel while decoding.
 
     For model training, it is recommended to use this context manager
     to load images in the BGR 3-channel format. For example,
 
     .. code-block:: python
 
         import datumaro as dm
-        with decode_image_context(ImageColorScale.COLOR):
+        with decode_image_context(image_backend=ImageBackend.cv2, image_color_channel=ImageColorScale.COLOR):
             item: dm.DatasetItem
             img_data = item.media_as(dm.Image).data
             assert img_data.shape[-1] == 3  # It should be a 3-channel image
     """
-    curr_ctx = IMAGE_COLOR_SCALE.get()
-    IMAGE_COLOR_SCALE.set(color_scale)
+
+    curr_ctx = (IMAGE_BACKEND.get(), IMAGE_COLOR_CHANNEL.get())
+
+    IMAGE_BACKEND.set(image_backend)
+    IMAGE_COLOR_CHANNEL.set(image_color_channel)
+
     yield
-    IMAGE_COLOR_SCALE.set(curr_ctx)
+
+    IMAGE_BACKEND.set(curr_ctx[0])
+    IMAGE_COLOR_CHANNEL.set(curr_ctx[1])
 
 
 def load_image(path: str, dtype: DTypeLike = np.uint8, crypter: Crypter = NULL_CRYPTER):
     """
     Reads an image in the HWC Grayscale/BGR(A) [0; 255] format (default dtype is uint8).
     """
 
-    if _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.cv2:
+    if IMAGE_BACKEND.get() == ImageBackend.cv2:
         # cv2.imread does not support paths that are not representable
         # in the locale encoding on Windows, so we read the image bytes
         # ourselves.
 
         with open(path, "rb") as f:
             image_bytes = crypter.decrypt(f.read())
 
         return decode_image(image_bytes, dtype=dtype)
-    elif _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.PIL:
+    elif IMAGE_BACKEND.get() == ImageBackend.PIL:
         with open(path, "rb") as f:
             image_bytes = crypter.decrypt(f.read())
 
         return decode_image(image_bytes, dtype=dtype)
 
-    raise NotImplementedError(_IMAGE_BACKEND)
+    raise NotImplementedError(IMAGE_BACKEND)
 
 
 def copyto_image(
     src: Union[str, IOBase], dst: Union[str, IOBase], src_crypter: Crypter, dst_crypter: Crypter
 ) -> None:
     if src_crypter == dst_crypter and src == dst:
         return
@@ -171,30 +199,30 @@
 
     if not kwargs:
         kwargs = {}
 
     # NOTE: OpenCV documentation says "If the image format is not supported,
     # the image will be converted to 8-bit unsigned and saved that way".
     # Conversion from np.int32 to np.uint8 is not working properly
-    backend = _IMAGE_BACKEND.get()
+    backend = IMAGE_BACKEND.get()
     if dtype == np.int32:
-        backend = _IMAGE_BACKENDS.PIL
-    if backend == _IMAGE_BACKENDS.cv2:
+        backend = ImageBackend.PIL
+    if backend == ImageBackend.cv2:
         # cv2.imwrite does not support paths that are not representable
         # in the locale encoding on Windows, so we write the image bytes
         # ourselves.
 
         image_bytes = encode_image(image, ext, dtype=dtype, **kwargs)
 
         if isinstance(dst, str):
             with open(dst, "wb") as f:
                 f.write(crypter.encrypt(image_bytes))
         else:
             dst.write(crypter.encrypt(image_bytes))
-    elif backend == _IMAGE_BACKENDS.PIL:
+    elif backend == ImageBackend.PIL:
         from PIL import Image
 
         if ext.startswith("."):
             ext = ext[1:]
 
         if not crypter.is_null_crypter:
             raise DatumaroError("PIL backend should have crypter=NullCrypter.")
@@ -213,15 +241,15 @@
         raise NotImplementedError()
 
 
 def encode_image(image: np.ndarray, ext: str, dtype: DTypeLike = np.uint8, **kwargs) -> bytes:
     if not kwargs:
         kwargs = {}
 
-    if _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.cv2:
+    if IMAGE_BACKEND.get() == ImageBackend.cv2:
         import cv2
 
         params = []
 
         if not ext.startswith("."):
             ext = "." + ext
 
@@ -229,15 +257,15 @@
             params = [int(cv2.IMWRITE_JPEG_QUALITY), kwargs.get("jpeg_quality", 75)]
 
         image = image.astype(dtype)
         success, result = cv2.imencode(ext, image, params=params)
         if not success:
             raise Exception("Failed to encode image to '%s' format" % (ext))
         return result.tobytes()
-    elif _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.PIL:
+    elif IMAGE_BACKEND.get() == ImageBackend.PIL:
         from PIL import Image
 
         if ext.startswith("."):
             ext = ext[1:]
 
         params = {}
         params["quality"] = kwargs.get("jpeg_quality")
@@ -252,29 +280,22 @@
             image.save(buffer, format=ext, **params)
             return buffer.getvalue()
     else:
         raise NotImplementedError()
 
 
 def decode_image(image_bytes: bytes, dtype: DTypeLike = np.uint8) -> np.ndarray:
-    ctx_color_scale = IMAGE_COLOR_SCALE.get()
+    ctx_color_scale = IMAGE_COLOR_CHANNEL.get()
 
-    if _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.cv2:
-        image = np.frombuffer(image_bytes, dtype=np.uint8)
-        image = ctx_color_scale.convert_cv2(image)
+    if IMAGE_BACKEND.get() == ImageBackend.cv2:
+        image = ctx_color_scale.decode_by_cv2(image_bytes)
         image = image.astype(dtype)
-    elif _IMAGE_BACKEND.get() == _IMAGE_BACKENDS.PIL:
-        from PIL import Image
-
-        image = Image.open(BytesIO(image_bytes))
-        image = ctx_color_scale.convert_pil(image)
+    elif IMAGE_BACKEND.get() == ImageBackend.PIL:
+        image = ctx_color_scale.decode_by_pil(image_bytes)
         image = np.asarray(image, dtype=dtype)
-        if len(image.shape) == 3 and image.shape[2] in {3, 4}:
-            image = np.array(image)  # Release read-only
-            image[:, :, :3] = image[:, :, 2::-1]  # RGB to BGR
     else:
         raise NotImplementedError()
 
     assert len(image.shape) in {2, 3}
     if len(image.shape) == 3:
         assert image.shape[2] in {3, 4}
     return image
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/image_cache.py` & `datumaro-1.6.1rc1/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/log_utils.py` & `datumaro-1.6.1rc1/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/mask_tools.py` & `datumaro-1.6.1rc1/src/datumaro/util/mask_tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright (C) 2019-2021 Intel Corporation
+# Copyright (C) 2019-2024 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-
+import logging as log
 from functools import partial
 from itertools import chain
-from typing import Dict, Tuple
+from typing import Dict, Optional, Tuple
 
 import numpy as np
 from pycocotools import mask as pycocotools_mask
 
 from datumaro._capi import encode
 from datumaro.util.image import lazy_image, load_image
 
@@ -120,16 +120,80 @@
     # mask: HW(C) [0; max_index] mask
     """
     check_is_mask(mask)
 
     return np.array([map_fn(c) for c in range(256)], dtype=np.uint8)[mask]
 
 
-def make_index_mask(binary_mask, index, dtype=None):
-    return binary_mask * np.array([index], dtype=dtype or np.min_scalar_type(index))
+def make_index_mask(
+    binary_mask: np.ndarray,
+    index: int,
+    ignore_index: int = 0,
+    dtype: Optional[np.dtype] = None,
+):
+    """Create an index mask from a binary mask by filling a given index value.
+
+    Args:
+        binary_mask: Binary mask to create an index mask.
+        index: Scalar value to fill the ones in the binary mask.
+        ignore_index: Scalar value to fill in the zeros in the binary mask.
+            Defaults to 0.
+        dtype: Data type for the resulting mask. If not specified,
+                it will be inferred from the provided `index` to hold its value.
+                For example, if `index=255`, the inferred dtype will be `np.uint8`.
+                Defaults to None.
+
+    Returns:
+        np.ndarray: Index mask created from the binary mask.
+
+    Raises:
+        ValueError: If dtype is not specified and incompatible scalar types are used for index
+            and ignore_index.
+
+    Examples:
+        >>> binary_mask = np.eye(2, dtype=np.bool_)
+        >>> index_mask = make_index_mask(binary_mask, index=10, ignore_index=255, dtype=np.uint8)
+        >>> print(index_mask)
+        array([[ 10, 255],
+               [255,  10]], dtype=uint8)
+    """
+    if dtype is None:
+        dtype = np.min_scalar_type(index)
+        if dtype != np.min_scalar_type(ignore_index):
+            msg = (
+                "Given dtype is None, "
+                "but inferred dtypes from the given index and ignore_index are different each other. "
+                "Please mannually set dtype"
+            )
+            raise ValueError(msg, index, ignore_index)
+
+    flipped_zero_np_scalar = ~np.full(tuple(), fill_value=0, dtype=dtype)
+
+    # NOTE: This dispatching rule is required for a performance boost
+    if ignore_index == flipped_zero_np_scalar:
+        flipped_index = ~np.full(tuple(), fill_value=index, dtype=dtype)
+        return ~(binary_mask * flipped_index)
+    elif index < ignore_index:
+        diff = ignore_index - index
+        mask = ~binary_mask * np.full(tuple(), fill_value=diff, dtype=dtype)
+        mask += index
+        return mask
+    elif index > ignore_index:
+        diff = index - ignore_index
+        mask = binary_mask * np.full(tuple(), fill_value=diff, dtype=dtype)
+        mask += ignore_index
+        return mask
+
+    # index == ignore_index
+    msg = (
+        "index == ignore_index. "
+        f"It will create an index mask filling with a single value, index={index}"
+    )
+    log.warning(msg)
+    return np.full_like(binary_mask, fill_value=index, dtype=dtype)
 
 
 def make_binary_mask(mask):
     if mask.dtype.kind == "b":
         return mask
     return mask.astype(bool)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/meta_file_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/multi_procs_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/multi_procs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/os_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/os_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Copyright (C) 2020-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import glob
 import importlib
 import os
 import os.path as osp
 import re
 import shutil
 import subprocess  # nosec B404
 import sys
 import unicodedata
 from contextlib import ExitStack, contextmanager, redirect_stderr, redirect_stdout
 from io import StringIO
-from typing import Iterable, Iterator, Optional, Union
+from typing import Iterable, Iterator, List, Optional, Set, Union
 
 try:
     # Declare functions to remove files and directories.
     #
     # Use rmtree from GitPython to avoid the problem with removal of
     # readonly files on Windows, which Git uses extensively
     # It double checks if a file cannot be removed because of readonly flag
@@ -63,15 +64,15 @@
 def walk(path, max_depth: Optional[int] = None, min_depth: Optional[int] = None):
     if max_depth is None:
         max_depth = DEFAULT_MAX_DEPTH
     if min_depth is None:
         min_depth = DEFAULT_MIN_DEPTH
 
     baselevel = path.count(osp.sep)
-    for dirpath, dirnames, filenames in os.walk(path, topdown=True):
+    for dirpath, dirnames, filenames in os.walk(path, topdown=True, followlinks=True):
         curlevel = dirpath.count(osp.sep)
         if baselevel + min_depth > curlevel:
             continue
 
         if baselevel + max_depth <= curlevel:
             dirnames.clear()  # topdown=True allows to modify the list
 
@@ -299,7 +300,15 @@
     relpath, _ = osp.split(relpath)
     relpath, subdir_name = osp.split(relpath)
 
     if relpath == "":
         return DEFAULT_SUBSET_NAME
 
     return subdir_name
+
+
+def get_all_file_extensions(path: str, ignore_dirs: Set[str]) -> List[str]:
+    extensions = set()
+    for p in glob.iglob(osp.join(path, "**", "*.*"), recursive=True):
+        if ignore_dirs.isdisjoint(p.split(os.sep)):
+            extensions.add(osp.splitext(p)[1])
+    return list(extensions)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/pickle_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/scope.py` & `datumaro-1.6.1rc1/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/telemetry_stub.py` & `datumaro-1.6.1rc1/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/telemetry_utils.py` & `datumaro-1.6.1rc1/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro/util/tf_util.py` & `datumaro-1.6.1rc1/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.6.0rc1/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.6.1rc1/src/datumaro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.6.0rc1
+Version: 1.6.1rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: attrs>=21.3.0
 Requires-Dist: defusedxml>=0.7.0
 Requires-Dist: h5py>=2.10.0
-Requires-Dist: lxml>=4.4.1
+Requires-Dist: imagesize>=1.4.1
+Requires-Dist: lxml==5.2.0
 Requires-Dist: matplotlib>=3.3.1
 Requires-Dist: networkx>=2.6
 Requires-Dist: nibabel>=3.2.1
-Requires-Dist: numpy>=1.17.3
-Requires-Dist: orjson>=3.6.6
-Requires-Dist: Pillow>=6.1.0
+Requires-Dist: numpy<2,>=1.23.4
+Requires-Dist: orjson==3.10.0
+Requires-Dist: Pillow==10.3.0
 Requires-Dist: ruamel.yaml>=0.17.0
 Requires-Dist: shapely>=1.7
 Requires-Dist: typing_extensions>=3.7.4.3
 Requires-Dist: tqdm
 Requires-Dist: pycocotools>=2.0.4; platform_system != "Windows" or python_version >= "3.9"
 Requires-Dist: pycocotools-windows; platform_system == "Windows" and python_version < "3.9"
-Requires-Dist: PyYAML>=5.3.1
+Requires-Dist: PyYAML==6.0.1
 Requires-Dist: tensorboardX!=2.3,>=1.8
 Requires-Dist: scipy
 Requires-Dist: requests
-Requires-Dist: pandas>=1.1.5
-Requires-Dist: openvino>=2023.2.0
+Requires-Dist: pandas~=1.4.0
+Requires-Dist: openvino<2024.0.0,>=2023.2.0
 Requires-Dist: tokenizers
 Requires-Dist: cryptography>=38.03
 Requires-Dist: pyemd
 Requires-Dist: pyarrow
-Requires-Dist: protobuf<4
+Requires-Dist: protobuf
 Requires-Dist: tabulate
 Requires-Dist: ovmsclient
 Requires-Dist: tritonclient[all]
 Requires-Dist: scikit-learn
 Requires-Dist: json-stream
 Requires-Dist: opencv-python
 Provides-Extra: tf
@@ -51,15 +52,15 @@
 Requires-Dist: tensorflow-datasets<4.9.3; extra == "tfds"
 Provides-Extra: tf-gpu
 Requires-Dist: tensorflow-gpu; extra == "tf-gpu"
 Provides-Extra: torch
 Requires-Dist: torch; extra == "torch"
 Requires-Dist: torchvision; extra == "torch"
 Provides-Extra: default
-Requires-Dist: dvc==3.30.1; extra == "default"
+Requires-Dist: dvc==3.49.0; extra == "default"
 Requires-Dist: fsspec<=2022.11.0; python_version < "3.8" and extra == "default"
 Requires-Dist: GitPython!=3.1.25,>=3.1.18; extra == "default"
 Requires-Dist: openvino-telemetry>=2022.1.0; extra == "default"
 Requires-Dist: openvino-dev>=2023.2.0; extra == "default"
 
 # Dataset Management Framework (Datumaro)
```

### Comparing `datumaro-1.6.0rc1/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.6.1rc1/src/datumaro.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -87,18 +87,18 @@
 src/datumaro/components/filter.py
 src/datumaro/components/format_detection.py
 src/datumaro/components/generator.py
 src/datumaro/components/importer.py
 src/datumaro/components/launcher.py
 src/datumaro/components/lazy_plugin.py
 src/datumaro/components/media.py
-src/datumaro/components/media_manager.py
 src/datumaro/components/operations.py
 src/datumaro/components/progress_reporting.py
 src/datumaro/components/project.py
+src/datumaro/components/registry.py
 src/datumaro/components/shift_analyzer.py
 src/datumaro/components/transformer.py
 src/datumaro/components/validator.py
 src/datumaro/components/visualizer.py
 src/datumaro/components/abstracts/__init__.py
 src/datumaro/components/abstracts/merger.py
 src/datumaro/components/abstracts/model_interpreter.py
@@ -120,14 +120,15 @@
 src/datumaro/components/merge/__init__.py
 src/datumaro/components/merge/base.py
 src/datumaro/components/merge/exact_merge.py
 src/datumaro/components/merge/extractor_merger.py
 src/datumaro/components/merge/intersect_merge.py
 src/datumaro/components/merge/union_merge.py
 src/datumaro/plugins/__init__.py
+src/datumaro/plugins/anchor_generator.py
 src/datumaro/plugins/configurable_validator.py
 src/datumaro/plugins/explorer.py
 src/datumaro/plugins/framework_converter.py
 src/datumaro/plugins/missing_annotation_detection.py
 src/datumaro/plugins/ndr.py
 src/datumaro/plugins/specs.json
 src/datumaro/plugins/specs.py
```

### Comparing `datumaro-1.6.0rc1/src/datumaro.egg-info/requires.txt` & `datumaro-1.6.1rc1/src/datumaro.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 attrs>=21.3.0
 defusedxml>=0.7.0
 h5py>=2.10.0
-lxml>=4.4.1
+imagesize>=1.4.1
+lxml==5.2.0
 matplotlib>=3.3.1
 networkx>=2.6
 nibabel>=3.2.1
-numpy>=1.17.3
-orjson>=3.6.6
-Pillow>=6.1.0
+numpy<2,>=1.23.4
+orjson==3.10.0
+Pillow==10.3.0
 ruamel.yaml>=0.17.0
 shapely>=1.7
 typing_extensions>=3.7.4.3
 tqdm
-PyYAML>=5.3.1
+PyYAML==6.0.1
 tensorboardX!=2.3,>=1.8
 scipy
 requests
-pandas>=1.1.5
-openvino>=2023.2.0
+pandas~=1.4.0
+openvino<2024.0.0,>=2023.2.0
 tokenizers
 cryptography>=38.03
 pyemd
 pyarrow
-protobuf<4
+protobuf
 tabulate
 ovmsclient
 tritonclient[all]
 scikit-learn
 json-stream
 opencv-python
 
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
 
 [default]
-dvc==3.30.1
+dvc==3.49.0
 GitPython!=3.1.25,>=3.1.18
 openvino-telemetry>=2022.1.0
 openvino-dev>=2023.2.0
 
 [default:python_version < "3.8"]
 fsspec<=2022.11.0
```

