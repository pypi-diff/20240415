# Comparing `tmp/gloe-0.5.4.tar.gz` & `tmp/gloe-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gloe-0.5.4.tar", last modified: Fri Apr 12 18:07:15 2024, max compression
+gzip compressed data, was "gloe-0.5.5.tar", last modified: Mon Apr 15 20:24:08 2024, max compression
```

## Comparing `gloe-0.5.4.tar` & `gloe-0.5.5.tar`

### file list

```diff
@@ -1,86 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-12 18:07:10.000000 gloe-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-12 18:07:10.000000 gloe-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 18:07:10.000000 gloe-0.5.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 18:07:15.955186 gloe-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 18:07:10.000000 gloe-0.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.943186 gloe-0.5.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/_static/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/gloe-logo-small.png
--rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/gloe-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/assets/graph_example.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/_static/theme_customs.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.947187 gloe-0.5.4/docs/source/api-reference/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/gloe.collection.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/gloe.experimental.md
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/gloe.utils.md
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/api-reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/docutils.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/docs/source/getting-started/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/async-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/conditional-flows.md
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/ensurers.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/partial-transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/plotting.md
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/transformers.md
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/getting-started/utilities.md
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/limitations.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/docs/source/pygments/
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/pygments/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-12 18:07:10.000000 gloe-0.5.4/docs/source/theory.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/_composition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13681 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/base_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/collection/_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/collection/_mapover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/conditional/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/conditional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/conditional/_conditioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/ensurer/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/ensurer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/ensurer/_transformer_ensurer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.951187 gloe-0.5.4/gloe/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/gloe/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/experimental/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 18:07:10.000000 gloe-0.5.4/gloe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/gloe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 18:07:15.000000 gloe-0.5.4/gloe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-12 18:07:10.000000 gloe-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 18:07:15.955186 gloe-0.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 18:07:15.955186 gloe-0.5.4/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/conditioners.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/ensurers.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/lib/transformers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_async_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_conditioner_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_function_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_ensurer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 18:07:10.000000 gloe-0.5.4/tests/test_transformer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11334 2024-04-15 20:23:57.000000 gloe-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 20:23:57.000000 gloe-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-15 20:24:08.482239 gloe-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-15 20:23:57.000000 gloe-0.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.466239 gloe-0.5.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/_static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/gloe-logo-small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22309 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/gloe-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55575 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/assets/graph_example.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_static/theme_customs.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.470239 gloe-0.5.5/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/_templates/page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/docs/source/api-reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/gloe.collection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/gloe.experimental.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/gloe.utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/api-reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/docutils.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/docs/source/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/async-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/conditional-flows.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/ensurers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/partial-transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/plotting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6693 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/transformers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/getting-started/utilities.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/limitations.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/docs/source/pygments/
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/pygments/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-04-15 20:23:57.000000 gloe-0.5.5/docs/source/theory.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.474238 gloe-0.5.5/gloe/
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/_composition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/_transformer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/_typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5821 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13736 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/base_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/collection/_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/collection/_mapover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/conditional/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/conditional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/conditional/_conditioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/ensurer/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/ensurer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/ensurer/_transformer_ensurer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.478238 gloe-0.5.5/gloe/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/experimental/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6625 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-15 20:23:57.000000 gloe-0.5.5/gloe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/gloe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5727 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-15 20:24:08.000000 gloe-0.5.5/gloe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-15 20:23:57.000000 gloe-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:24:08.482239 gloe-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:24:08.482239 gloe-0.5.5/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/conditioners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/ensurers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/lib/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_async_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_conditioner_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_function_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9987 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_ensurer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-15 20:23:57.000000 gloe-0.5.5/tests/test_transformer_utils.py
```

### Comparing `gloe-0.5.4/LICENSE` & `gloe-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/PKG-INFO` & `gloe-0.5.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.4
-Summary: Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows.
+Version: 0.5.5
+Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions~=4.7.1
 Requires-Dist: schemdraw~=0.16
@@ -22,40 +25,36 @@
 ***
 
 <div align="center">
   <img src="https://github.com/ideos/gloe/raw/main/docs/source/_static/assets/gloe-logo.png"><br>
 </div>
 
 
-| | |
-| --- |-|
-| Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml)|
-| Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)|
-| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
+| |                                                                                                                                                                                                                                                             |
+| --- |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml) [![Coverage](https://codecov.io/github/ideos/gloe/coverage.svg?branch=main)](https://codecov.io/gh/ideos/gloe) |
+| Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe) [![Supported Python versions](https://img.shields.io/pypi/pyversions/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)              |
+| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE)                                                                                                                          | 
 
+**Documentation**: [gloe.ideos.com.br](https://gloe.ideos.com.br)
 
+# Write a Better Python Code
 
-Let Gloe help you
-===
-
-Gloe (pronounced /ɡloʊ/, like "glow") is a general purpose library made to help developers to create, maintain, document and test operational and data flows. It can be used in data science and machine learning pipelines as well in servers, scripts or wherever else one identifies a lack between the code and the understanding of logical business. Gloe was not thought to be used in the entire application even less replacing any existing library, it was built to be integrated with other tools and to be implemented where the code complexity can be bigger than the desired.
-
-## Documentation
-
-The official documentation is hosted on [gloe.ideos.com.br](https://gloe.ideos.com.br).
+Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code. It is particularly useful in data science and machine learning pipelines, as well as in servers and scripts, or any area where there is a gap between the code and the logical business understanding. Gloe is not intended to be used across an entire application or to replace existing libraries. Instead, it is built to integrate with other tools and to address areas where the code complexity may be higher than expected.
 
 ## Motivation
 
-Software development has a lot of patterns and good practices related to the code itself, like how to document, to test, to structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
+Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
-When a developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, the story can be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software will take a long time to understand the narrative and make it clear, or they might give up and leave it as is.
+When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
+### How Gloe Can Help Me?
 
-Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into concise steps with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
+Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
 
 ## Installing
```

### Comparing `gloe-0.5.4/README.md` & `gloe-0.5.5/docs/source/index.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,55 @@
-***
+% Gloe documentation master file, created by
+% sphinx-quickstart on Tue Dec 12 06:33:16 2023.
+% You can adapt this file completely to your liking, but it should at least
+% contain the root `toctree` directive.
 
-<div align="center">
-  <img src="https://github.com/ideos/gloe/raw/main/docs/source/_static/assets/gloe-logo.png"><br>
-</div>
+```{eval-rst} 
+:og:description: Gloe (pronounced like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 
+.. meta::
+  :description: Gloe (pronounced like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
+```
 
-| | |
-| --- |-|
-| Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml)|
-| Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)|
-| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
-
-
-
-Let Gloe help you
-===
-
-Gloe (pronounced /ɡloʊ/, like "glow") is a general purpose library made to help developers to create, maintain, document and test operational and data flows. It can be used in data science and machine learning pipelines as well in servers, scripts or wherever else one identifies a lack between the code and the understanding of logical business. Gloe was not thought to be used in the entire application even less replacing any existing library, it was built to be integrated with other tools and to be implemented where the code complexity can be bigger than the desired.
-
-## Documentation
+# Write a Better Python Code
 
-The official documentation is hosted on [gloe.ideos.com.br](https://gloe.ideos.com.br).
+Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code. It is particularly useful in data science and machine learning pipelines, as well as in servers and scripts, or any area where there is a gap between the code and the logical business understanding. Gloe is not intended to be used across an entire application or to replace existing libraries. Instead, it is built to integrate with other tools and to address areas where the code complexity may be higher than expected.
 
 ## Motivation
 
-Software development has a lot of patterns and good practices related to the code itself, like how to document, to test, to structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
+Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
-When a developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, the story can be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software will take a long time to understand the narrative and make it clear, or they might give up and leave it as is.
+When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
+### How Gloe Can Help Me?
 
-Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into concise steps with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
+Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
 
 ## Installing
 
 ```shell
 pip install gloe
 ```
 
-## License
+```{toctree}
+:caption: 'Contents'
+:maxdepth: 3
+:hidden:
+
+Introduction <self>
+theory
+getting-started/index
+limitations
+```
+
+```{toctree}
+:caption: 'Development'
+:maxdepth: 3
+:hidden:
 
-[Apache License Version 2.0](https://github.com/ideos/gloe/blob/main/LICENSE)
+api-reference/index
+```
```

### Comparing `gloe-0.5.4/docs/source/_static/assets/favicon.ico` & `gloe-0.5.5/docs/source/_static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/_static/assets/gloe-logo-small.png` & `gloe-0.5.5/docs/source/_static/assets/gloe-logo-small.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/_static/assets/gloe-logo.png` & `gloe-0.5.5/docs/source/_static/assets/gloe-logo.png`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/_static/assets/graph_example.jpeg` & `gloe-0.5.5/docs/source/_static/assets/graph_example.jpeg`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/api-reference/index.md` & `gloe-0.5.5/docs/source/api-reference/index.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/conf.py` & `gloe-0.5.5/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Configuration file for the Sphinx documentation builder.
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 import os
 import sys
+import pkg_resources
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 sys.path.insert(0, os.path.abspath("../.."))
 sys.path.insert(0, os.path.abspath("pygments"))
 
 project = "Gloe"
 copyright = "2023, Samir Braga"
 author = "Samir Braga"
-release = "0.4.3"
+version = pkg_resources.get_distribution("gloe").version
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx_toolbox.more_autodoc.variables",
     "sphinx.ext.autosectionlabel",
@@ -26,38 +27,44 @@
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     "sphinxext.opengraph",
     # "sphinx_autodoc_typehints",
     "myst_parser",
     "sphinx_copybutton",
+    "sphinx_sitemap",
 ]
 overloads_location = "bottom"
 napoleon_google_docstring = True
 autosectionlabel_prefix_document = True
 napoleon_use_rtype = False
 # intersphinx_mapping = {"httpx": ("https://www.python-httpx.org/", None)}
 ogp_social_cards = {
     "enable": True,
     "line_color": "#00afac",
     "image": "_static/assets/gloe-logo.png",
 }
 ogp_site_url = "https://gloe.ideos.com.br/"
 # ogp_image = "https://gloe.ideos.com.br/_static/assets/gloe-logo.png"
+html_baseurl = "https://gloe.ideos.com.br/"
+sitemap_locales = [None]
+sitemap_url_scheme = "{link}"
+html_extra_path = ["_static/robots.txt"]
+ogp_description_length = 160
 
 templates_path = ["_templates"]
 exclude_patterns = ["Thumbs.db", ".DS_Store"]
 autodoc_typehints = "description"
 autodoc_type_aliases = {
     "PreviousTransformer": "gloe.base_transformer.PreviousTransformer"
 }
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
-html_title = "Gloe"
+html_title = "Gloe - Write a Better Python Code"
 # html_logo = "assets/gloe-logo-small.png"
 html_theme = "furo"
 html_last_updated_fmt = ""
 # html_use_index = False  # Don't create index
 # html_domain_indices = False  # Don't need module indices
 # html_copy_source = False  # Don't need sources
 html_sidebars: dict[str, list[str]] = {
```

### Comparing `gloe-0.5.4/docs/source/getting-started/async-transformers.md` & `gloe-0.5.5/docs/source/getting-started/async-transformers.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 ```{admonition} API Reference
 :class: seealso
 - {func}`gloe.async_transformer`
 - {func}`gloe.partial_async_transformer`
 - {class}`gloe.AsyncTransformer`
 ```
 
-
-Transformer can be also created from [coroutines](https://docs.python.org/3/library/asyncio-task.html#coroutines), but, in this case, you need to use the `@async_transformer` decorator. For example, consider the bellow transformer that fetchs data from an external http server:
+Transformers can be also created from [coroutines](https://docs.python.org/3/library/asyncio-task.html#coroutines), but, in this case, you need to use the `@async_transformer` decorator. For example, consider the transformer below that fetches data from an external http server:
 
 ```python
 import httpx
 from gloe import async_transformer
 
 @async_transformer
 async def fetch_data(resource: str) -> httpx.Response:
     async with httpx.AsyncClient() as client:
         r = await client.get(f'{BASE_URL}/{resource}')
     return r
 ```
-The `@async_transformer` decorator converts the `fetch_data` function to an instance of the `AsyncTransformer` class.
+The `@async_transformer` decorator converts the `fetch_data` function into an instance of the `AsyncTransformer` class.
 
 To call this transformer, we need to use the `await` syntax, just like a normal coroutine:
 
 ```python
 await fetch_data('users')
 ```
 
@@ -39,35 +38,35 @@
 
 @transformer
 def extract_user_roles(user: User) -> list[Role]: ...
 
 get_user_roles = get_user_by_id >> extract_user_roles
 ```
 
-When a pipeline has at least one async transformer, the entire pipeline becomes async, so we must call it using the `await` statement as well:
+When a pipeline has at least one async transformer, the entire pipeline becomes async, so we must call it using the `await` statement:
 
 ```python
 await get_user_roles(user_id)
 ```
 
 Alternatively, we can start the pipeline with a sync transformer and append an async transformer to it:
 
 ```python
 @transformer
 def extract_user_id(request: Request) -> int: ...
 
 get_user = extract_user_id >> get_user_by_id
 ```
 
-Briefly, you can mix async and sync transformers together without care about its concurrent nature, just about the types as before.
+Briefly, you can mix async and sync transformers together without worrying about its concurrent nature, but it is still a transformer, so you'll still have to make sure the typing is correct.
 
 (partial-async-transformers)=
 ## Partial Async Transformers
 
-As well as in sync transformers, you can create [partial transformers](/getting-started/partial-transformers) with an async behavoir. It can be done using the `@partial_async_transformer`:
+Just like in sync transformers, you can create [partial transformers](/getting-started/partial-transformers) with an async behavior. It can be done using the `@partial_async_transformer`:
 
 ```python
 from gloe import partial_async_transformer
 
 @partial_async_transformer
 def get_users_by_role(role: str, page: int = 0, page_size: int = 10) -> Page[User]:
     "Get users with a specific role. The response is paginated."
```

### Comparing `gloe-0.5.4/docs/source/getting-started/conditional-flows.md` & `gloe-0.5.5/docs/source/getting-started/conditional-flows.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 )
 
 send_email_to_user = get_user_by_id >> send_email
 ```
 
 ## Chaining Many Conditions
 
-Suppose now we have to send another type of email to users with a "manager" role, we can adapt that flow to send this specific email to that users using the `.ElseIf` method:
+Suppose now we have to send another type of email to users with a "manager" role, we can adapt that flow to send this specific email to those users using the `.ElseIf` method:
 
 ```python
 from gloe.conditional import If
 
 send_email = (
     If(lambda user: "admin" in user.roles)
         .Then(fetch_admin_data >> send_admin_email)
@@ -65,28 +65,28 @@
 ```
 ```{tip}
 You can chain as many `ElseIf`'s as you want.
 ```
 
 ## Understanding the Types
 
-Assume the below transformers and conditions:
+Take the following transformers and conditions:
 
 ```python
 condition1: Callable[[In], bool]
 then_transformer1: Transformer[In, Out1]
 condition2: Callable[[In], bool]
 then_transformer2: Transformer[In, Out2]
 ...
 conditionN: Callable[[In], bool]
 then_transformerN: Transformer[In, OutN]
 else_transformer: Transformer[In, ElseOut]
 ```
 
-Lets chain the conditions:
+Now, let us chain the conditions:
 ```python
 chained_conditions = (
     If(condition1).Then(then_transformer1)
     .ElseIf(condition2).Then(then_transformer2)
     ...
     .ElseIf(conditionN).Then(then_transformerN)
     .Else(else_transformer)
@@ -94,12 +94,12 @@
 ```
 
 The type of `chained_conditions` is:
 ```python
 Transformer[In, Out1 | Out2 | ... | OutN | ElseOut]
 ```
 
-It means, the transformer after the `chained_conditions` must be able to deal with all possible output types of the cases.
+The transformer after the `chained_conditions` must be able to deal with all possible output types of the cases.
 
 ```{hint}
 If you are not familiar with the type annotation syntax used above, we strongly recommend you to read the [Mypy types documentation](https://mypy.readthedocs.io/en/stable/builtin_types.html).
 ```
```

### Comparing `gloe-0.5.4/docs/source/getting-started/ensurers.md` & `gloe-0.5.5/docs/source/getting-started/ensurers.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,76 +4,76 @@
 ```{admonition} API Reference
 :class: seealso
 - {func}`gloe.ensure`
 ```
 
 Although the type annotations are good enough to statically ensure a correct pipeline shape, on the other hand, there are some dynamic validations we may want to do on a transformer input and output during execution time. 
 
-For example, consider the same `filter_even` transformer and suppose we only want positive numbers as its input. One first option is to implement this logic inside the transformer code:
+For example, consider the same `filter_even` transformer and suppose we only want positive numbers as its input. One first option is implement this logic inside the transformer code:
 
 ```python
 @transformer
 def filter_even(numbers: list[int]) -> list[int]:
     non_positives = [num for num in numbers if num <= 0]
     if len(non_positives) > 0:
       raise Exception(f"The numbers {', '.join(non_positives)} are not positive.")
       
     return [num for num in numbers if num % 2 == 0]
 ```
 
-In the above example, we are assigning a new responsibility to the transformer: the input validation. However, in many cases, we could have a complex validation or even many validations, and it seems a good idea to split the processing and these validations in different places. To help in this scenario, Gloe provides the `@ensure` decorator:
+In the example above, we are assigning a new responsibility to the transformer: the input validation. However, in many cases, we could have many complex validations, and it may be a good idea to keep processes and validations in different places. To help in this scenario, Gloe provides the `@ensure` decorator:
 
 ```python
 def only_positive(numbers: list[int]):
   non_positives = [num for num in numbers if num <= 0]
   if len(non_positives) > 0:
     raise Exception(f"The numbers {', '.join(non_positives)} are not positive.")
 
 
 @ensure(incoming=[only_positive])
 @transformer
 def filter_even(numbers: list[int]) -> list[int]:
     return [num for num in numbers if num % 2 == 0]
 ```
 
-In this version we are validating the incoming data outside the transformer, what allow us to refactor the validation step without change the transformer internal logic. 
+In this version we are validating the incoming data outside the transformer, which allows us to refactor the validation step without changing the transformer internal logic. 
 
-The `@ensurer` decorator must be attached to a transformer and has the following parameters. All parameters receive a list of validators. A validator means just a normal function that perform a validation in the desired data and must throw an exception if the validation fails. The return of the validator is ignored.
+The `@ensure` decorator must be attached to a transformer and have the following parameters. All parameters receive a list of validators. A validator is a function that performs a validation in the desired data and must throw an exception if the validation fails. The return of the validator is ignored.
 
 - `incoming: list[Callable[[In], ...]]`: list of input validators. `In` type is the transformer incoming type.
 
 - `outcome: list[Callable[[Out], ...]]`: list of output validators. `Out` type is the transformer outcome type.
 
 - `changes: list[Callable[[In, Out], ...]]`: list of changes validators. A changes validator receives two parameters: the input and output data, which allow us to check if some kind of consistence is preserved after applying the transformation on the data. `In` and `Out` types are the transformer incoming type and outcome type, respectively.
 
 ## A complete example
 
-Suppose we have a Pandas dataframe of houses for sale, and we want to do an exploration of this data. This dataframe has many columns related to the houses' features (the city, for example) and a numeric column of "price". We want to find the cities with an average value of m² greater than a threshold (the implementations and pydocs will be omitted for simplicity):
+Suppose we have a Pandas dataframe of houses for sale, and we want to explore this data. This dataframe may have many columns related to the houses' features (the city, for example) and a numeric column of "price", for example. We want to find the cities with an average value of m² greater than a threshold (the implementations and pydocs will be omitted for simplicity):
 
 ```python
 @partial_transformer
 def cities_more_expensive_than(houses_df: pd.DataFrame, min_price: float) -> pd.DataFrame:
     ...
 ```
 
-One input validation we want to do is ensure that there is not NaN values in the price column:
+One input validation we may want to do is ensure that there is not NaN values in the price column:
 
 ```python
 def has_no_nan_prices(houses_df: pd.DataFrame):
     ...
 ```
 
-A possible output validation is checking that exists at least one city that satisfies our condition:
+Another possible output validation is checking that exists at least one city that satisfies our condition:
 
 ```python
 def is_non_empty(df: pd.DataFrame):
     ...
 ```
 
-By last, maybe we would like to be sure that the lowest price in the selected cities is greater than the average value of all houses.
+Lastly, maybe we would like to be sure that the lowest price in the selected cities is greater than the average value of all houses.
 
 ```python
 def lowest_price_gt_avg(houses_df: pd.DataFrame, city_prices_df: pd.DataFrame):
     ...
 ```
 
 Now we can add all these validations to our transformer:
@@ -85,9 +85,9 @@
     changes=[lowest_price_gt_avg]
 )
 @partial_transformer
 def cities_more_expensive_than(houses_df: pd.DataFrame, min_price: float) -> pd.DataFrame:
     ...
 ```
 ```{important}
-As you can see, the `@ensure` decorator works to partial transformers as well. In fact, you can use it with all types of transformers, including async transformers and partial async transformers.
+As you can see, the `@ensure` decorator works with partial transformers as well. In fact, you can use it with all types of transformers, including async transformers and partial async transformers.
 ```
```

### Comparing `gloe-0.5.4/docs/source/getting-started/partial-transformers.md` & `gloe-0.5.5/docs/source/getting-started/partial-transformers.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 (partial-transformers)=
 # Partial Transformers
 
+
 ```{admonition} API Reference
 :class: seealso
 - {func}`gloe.partial_transformer`
 ```
 
-The single parameter of a transformer represents the input data during the execution and this input will be the return of the previous transformer in the pipeline. Given that, doesn't make sense allow transformers to have multiple parameters, because functions can't return multiple things (only a tuple of multiple things). However, sometimes we need some accessory data to perform the desired transformation.
+The single parameter of a transformer represents the input data during the execution and this input will be the return of the previous transformer in the pipeline. That being said, it doesn't make sense to allow transformers to have multiple parameters, because functions can't return multiple things (only a tuple of multiple things). However, sometimes we need some accessory data to perform the desired transformation.
 
 For example, suppose we have a [Pandas](https://pandas.pydata.org/) dataframe of people with a numeric column "age". We want to filter people older than a specific age:
 
 ```python
 @transformer
 def filter_older_than_21(people_df: pd.DataFrame) -> pd.DataFrame:
     return people_df[people_df['age'] >= 21]
 ```
 
-But maybe we would want to make this age threshold flexible. The first idea is to resort to the use of classes:
+But maybe we want to make this age threshold flexible. The first idea is to resort to the use of classes:
 
 ```python
 class FilterOlderThan(Transformer[pd.DataFrame, pd.DataFrame]):
     def __init__(self, min_age: int):
         super().__init__() # don't forget that
         self.min_age = min_age
 
@@ -31,15 +32,15 @@
 Now we can create many transformers with different ages:
 
 ```python
 filter_older_than_21 = FilterOlderThan(min_age=21)
 filter_older_than_18 = FilterOlderThan(min_age=18)
 ```
 
-Gloe provide a much more easy way to implement this behavior using the `@partial_transformer` decorator. The same flexible transformer just created can be made using a functional approach:
+Gloe provides a much easier way to implement this behavior using the `@partial_transformer` decorator. We can then create the same transformer using a functional approach:
 
 ```python
 @partial_transformer
 def filter_older_than(people_df: pd.DataFrame, min_age: int) -> pd.DataFrame:
     return people_df[people_df['age'] >= min_age]
 ```
 
@@ -52,9 +53,9 @@
 
 In partial transformers, the first parameter is the input and all the remaining parameters are static and must be passed during the transformer instantiation. Another example:
 
 ```python
 pipeline = filter_man >> filter_older_than(min_age=21)
 ```
 ```{tip}
-When typing the partial transformer instantiation, the IDE will ignore the first argument during autocompletion.
+When typing the partial transformer instantiation, IDEs will ignore the first argument during autocompletion.
 ```
```

### Comparing `gloe-0.5.4/docs/source/getting-started/plotting.md` & `gloe-0.5.5/docs/source/getting-started/plotting.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/getting-started/transformers.md` & `gloe-0.5.5/docs/source/getting-started/transformers.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,39 +32,39 @@
 
 Every transformer (instance of the Transformer class) can be called just like a normal function:
 
 ```python
 filter_even([1, 2, 3, 4, 5, 6]) # returns [2, 4, 6]
 ```
 
-Another way to create a transformer is extending from the Transformer class. This is how implement the above example using a class instead of a function:
+Another way to create a transformer is extending from the Transformer class. This is how to implement the above example using a class instead of a function:
 
 ```python
 from gloe import Transformer
 
 class FilterEven(Transformer[list[int], list[int]]):
     """Filters out the even numbers from the input list."""
     
     def transform(self, numbers: list[int]) -> list[int]:
         return [num for num in numbers if num % 2 == 0]
 ```
 
-However, in this case, we need first to instantiate the `FilterEven` class and then use the instance as a transformer:
+However, in this case, we first need to instantiate the `FilterEven` class and then use the instance as a transformer:
 
 ```python
 filter_even = FilterEven()
 
 filter_even([1, 2, 3, 4, 5, 6]) # returns [2, 4, 6]
 ```
 
 This doesn't seem useful when comparing to the first example, but maybe you would like to split your code into methods of a class in some cases. In fact, we try to avoid using classes to implement transformers to keep its code and responsibility clean and short.
 
 ## Building a Pipeline
 
-The existence motivation of the transformers is composing many of them into an execution graph or pipeline. You can do that using the [right shift operator (>>)](https://docs.python.org/3/library/operator.html#operator.__rshift__). For example, consider the `filter_even` created above, we can create another transformer called `square`:
+You can create a pipeline by combining many transformers into an execution graph. You can do that by using the [right shift operator (>>)](https://docs.python.org/3/library/operator.html#operator.__rshift__). For example, consider the `filter_even` created above, we can create another transformer called `square`:
 
 ```python
 @transformer
 def square(numbers: list[int]) -> list[int]:
     return [num * num for num in numbers]
 ```
 
@@ -74,15 +74,15 @@
 pipeline = filter_even >> square
 ```
 ```{admonition} Naming things
 :class: seealso
 We call this **serial connection**
 ```
 
-By doing this, the `pipeline` variable becomes a transformer that executes the processing of the composed transformers sequentially. Of course, we can call it as well:
+By doing this, the `pipeline` variable becomes a transformer that executes the processing of the composed transformers sequentially. We can also call it as well:
 
 ```python
 pipeline([1, 2, 3, 4, 5, 6]) # returns [4, 16, 36]
 ```
 
 And you can continue appending transformers to the pipeline, even the ones already present there:
 
@@ -114,21 +114,21 @@
 send_promotion = get_users >> (
     filter_basic_subscription >> send_basic_subscription_promotion_email,
     filter_premium_subscription >> send_premium_subscription_promotion_email,
     filter_unsubscribed >> send_unsubscribed_promotion_email
 )
 ```
 
-This example makes clear how easy it is to understand and refactor the code when using Gloe to express the processing as a graph, with each node (transformer) having an atomic and well-defined responsibility.
+This example makes it clear how easy it is to understand and refactor the code when using Gloe to express the process as a graph, with each node (transformer) having an atomic and well-defined responsibility.
 
 ```{important}
-You can't assume any **order of execution** between the branches.
+You should not assume any **order of execution** between branches.
 ```
 
-The right shift operator can receive a transformer or a tuple of transformers as an argument. In the second case, the transformer returned will be as described bellow (pay attention at the types).
+The right shift operator can receive a transformer or a tuple of transformers as an argument. In the second case, the transformer returned will be as described bellow (pay attention to the types).
 
 Consider the following transformers:
 
 ```python
 begin: Transformer[In, Mid]
 branch1: Transformer[Mid, Out1]
 branch2: Transformer[Mid, Out2]
@@ -144,15 +144,15 @@
     ...,
     branchN
 )
 ```
 
 The return of each branch will compose a tuple following the respective order of branches.
 
-Of course, we can append a new transformer to the above graph, the only requirement is the incoming type of this new transformer must be `tuple[Out1, Out2, ..., OutN]`.
+Of course, we can append a new transformer to the above graph, the only requirement is for the incoming type of this new transformer to be `tuple[Out1, Out2, ..., OutN]`.
 
 ```python
 end: Transformer[tuple[Out1, Out2, ..., OutN], FinalOut]
 
 graph: Transformer[In, FinalOut] = begin >> (
     branch1,
     branch2,
```

### Comparing `gloe-0.5.4/docs/source/getting-started/utilities.md` & `gloe-0.5.5/docs/source/getting-started/utilities.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,57 +6,61 @@
 - {func}`gloe.utils.forward_incoming`
 - {data}`gloe.utils.forget`
 - {func}`gloe.utils.debug`
 ```
 
 ## forward
 
-The `forward` utility is quite useful when your flow starts with a divergent connection. For example:
+The `forward` utility is used when your flow starts with a divergent connection. For example:
 
 ```python
 from gloe.utils import forward
 
 send_emails = forward[list[User]]() >> (
     filter_basic_subscription >> send_basic_subscription_promotion_email,
     filter_premium_subscription >> send_premium_subscription_promotion_email,
     filter_unsubscribed >> send_unsubscribed_promotion_email
 )
 ```
 
-In this case, we have nothing to do before split the groups of users. So, when starting the pipeline with `forward` transformer, we are able to forward the incoming data to the next transformer directly.
+In this case, we have nothing to do before splitting the groups of users. So, when starting the pipeline with a `forward` transformer, we are able to forward the incoming data to the next transformer directly.
 ```{important}
 We have to explicitly define the incoming type of the forward transformer when it is used as the first step, because it is not known at the time of the definition.
 ```
 
 ## forward_incoming
 
-Suppose you need to extract some statistics of a Pandas DataFrame. However, you still need the use the original data in the next transformers. In that case, you can use `forward_incoming`, which receives a transformer as an argument. The output of the `forward_incoming` is a tuple with the output of the encapsulated transformer and its input.
+Suppose you need to extract some statistics from a Pandas DataFrame. However, you still need the use the original data in the next transformers. In that case, you can use `forward_incoming`, which receives a transformer as an argument. The output of the `forward_incoming` is a tuple with the output of the encapsulated transformer and its input.
 
 ```python
 get_data: Transformer[str, pd.DataFrame]
 extract_statistics: Transformer[pd.DataFrame, Statistics]
 process_statistics: Transformer[tuple[pd.DataFrame, Statistics], Result]
 
 process_data = get_data >> forward_incoming(extract_statistics) >> process_statistics 
 ```
 
-In the above example, both output of `get_data` and `extract_statistics` are passed as the input to `process_statistics`.
+In the example above, both `get_data` and `extract_statistics` outputs are passed on as the input to `process_statistics`.
 
 ## forget
 
 Converts any input data to `None`. Quite useful in addition with {ref}`conditional-flows`.
 
 ## debug
 
 It is quite useful when you want to see the flowing data at some points, for example:
 
 ```python
 from gloe.utils import debug
 
-send_emails = get_users >> filter_subscribed_users >> debug >> send_subscribed_email
+send_emails = get_users >> filter_subscribed_users >> debug() >> send_subscribed_email
 ```
 
 In this case, when calling `send_emails` in debugger mode, the processing will pause into the `debug` transformer. Then, we are able to see the output of the previous transformer (`filter_subscribed_users`) in the debug console.
 
-```{danger}
-You must not deploy a pipeline containing this transformer to a production environment.
+```{Important}
+This transformer is just a helper, you can keep adding breakpoints to any part of the transformers code as you are already used to.
+```
+
+```{Attention}
+The execution will stop only if a debugger is active. In general, this verification is valid only under a debug mode in IDE.
 ```
```

### Comparing `gloe-0.5.4/docs/source/limitations.md` & `gloe-0.5.5/docs/source/limitations.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/pygments/styles.py` & `gloe-0.5.5/docs/source/pygments/styles.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/docs/source/theory.md` & `gloe-0.5.5/docs/source/theory.md`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/gloe/__init__.py` & `gloe-0.5.5/gloe/__init__.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/gloe/_composition_utils.py` & `gloe-0.5.5/gloe/_composition_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from inspect import Signature
 from types import GenericAlias
 from typing import TypeVar, Any, cast
 
 from gloe.async_transformer import AsyncTransformer
 from gloe.base_transformer import BaseTransformer
 from gloe.transformers import Transformer
-from gloe._utils import _match_types, _specify_types, awaitify
+from gloe._typing_utils import _match_types, _specify_types
 from gloe.exceptions import UnsupportedTransformerArgException
 
 _In = TypeVar("_In")
 _Out = TypeVar("_Out")
 _NextOut = TypeVar("_NextOut")
 
 
@@ -21,18 +21,14 @@
     return isinstance(node, Transformer)
 
 
 def is_async_transformer(node):
     return isinstance(node, AsyncTransformer)
 
 
-def has_any_async_transformer(node: list):
-    return any(is_async_transformer(n) for n in node)
-
-
 def _resolve_new_merge_transformers(
     new_transformer: BaseTransformer, transformer2: BaseTransformer
 ):
     new_transformer.__class__.__name__ = transformer2.__class__.__name__
     new_transformer._label = transformer2.label
     new_transformer._children = transformer2.children
     new_transformer._invisible = transformer2.invisible
@@ -132,15 +128,15 @@
                 transformer1_out = transformer1(data)
                 transformed = await transformer2(transformer1_out)
                 return transformed
 
         new_transformer = NewTransformer4()
 
     else:
-        raise UnsupportedTransformerArgException(transformer2)
+        raise UnsupportedTransformerArgException(transformer2)  # pragma: no cover
 
     return _resolve_new_merge_transformers(new_transformer, transformer2)
 
 
 def _merge_diverging(
     incident_transformer,
     *receiving_transformers,
@@ -273,8 +269,8 @@
             unsupported_elem = [
                 elem for elem in next_node if not isinstance(elem, BaseTransformer)
             ]
             raise UnsupportedTransformerArgException(unsupported_elem[0])
         else:
             raise UnsupportedTransformerArgException(next_node)
     else:
-        raise UnsupportedTransformerArgException(next_node)
+        raise UnsupportedTransformerArgException(next_node)  # pragma: no cover
```

### Comparing `gloe-0.5.4/gloe/_utils.py` & `gloe-0.5.5/gloe/_typing_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,26 @@
-from functools import wraps
+import traceback
 from types import GenericAlias
 from typing import (
     TypeVar,
     get_origin,
-    TypeAlias,
-    TypedDict,
-    Generic,
-    Union,
     _GenericAlias,
-    ParamSpec,
-    Callable,
-    Awaitable,
 )  # type: ignore
 
 
-def _format_tuple(
-    tuple_annotation: tuple, generic_input_param, input_annotation
-) -> str:
+def _format_tuple(tuple_annotation: tuple, generic_input_param, input_annotation) -> str:
     formatted: list[str] = []
     for annotation in tuple_annotation:
         formatted.append(
             _format_return_annotation(annotation, generic_input_param, input_annotation)
         )
     return f"({', '.join(formatted)})"
 
 
-def _format_union(
-    tuple_annotation: tuple, generic_input_param, input_annotation
-) -> str:
+def _format_union(tuple_annotation: tuple, generic_input_param, input_annotation) -> str:
     formatted: list[str] = []
     for annotation in tuple_annotation:
         formatted.append(
             _format_return_annotation(annotation, generic_input_param, input_annotation)
         )
     return f"({' | '.join(formatted)})"
 
@@ -138,18 +127,7 @@
         return generic
 
     origin = get_origin(generic)
 
     args = tuple(_specify_types(arg, spec) for arg in generic_args)
 
     return GenericAlias(origin, args)
-
-
-_Args = ParamSpec("_Args")
-_R = TypeVar("_R")
-
-
-def awaitify(sync_func: Callable[_Args, _R]) -> Callable[_Args, Awaitable[_R]]:
-    async def async_func(*args, **kwargs):
-        return sync_func(*args, **kwargs)
-
-    return async_func
```

### Comparing `gloe-0.5.4/gloe/async_transformer.py` & `gloe-0.5.5/gloe/async_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import traceback
 import types
 import uuid
 from abc import abstractmethod, ABC
 from inspect import Signature
 from typing import TypeVar, overload, cast, Any, Callable, Awaitable
 
+from gloe._transformer_utils import catch_transformer_exception
 from gloe.base_transformer import (
     TransformerException,
     BaseTransformer,
     PreviousTransformer,
 )
 
 __all__ = ["AsyncTransformer"]
@@ -43,67 +44,37 @@
 
         Args:
             data: the incoming data passed to the transformer during the pipeline execution.
 
         Return:
             The outcome data, it means, the resulf of the transformation.
         """
-        pass
 
     def signature(self) -> Signature:
-        return self._signature(AsyncTransformer)
+        return self._signature(AsyncTransformer, "transform_async")
 
     def __repr__(self):
         return f"{self.input_annotation} -> ({type(self).__name__}) -> {self.output_annotation}"
 
     async def __call__(self, data: _In) -> _Out:
         transform_exception = None
 
         transformed: _Out | None = None
         try:
             transformed = await self.transform_async(data)
         except Exception as exception:
-            if type(exception.__cause__) == TransformerException:
-                transform_exception = exception.__cause__
-            else:
-                tb = traceback.extract_tb(exception.__traceback__)
-
-                # TODO: Make this filter condition stronger
-                transformer_frames = [
-                    frame
-                    for frame in tb
-                    if frame.name == self.__class__.__name__ or frame.name == "transform"
-                ]
-
-                if len(transformer_frames) == 1:
-                    transformer_frame = transformer_frames[0]
-                    exception_message = (
-                        f"\n  "
-                        f'File "{transformer_frame.filename}", line {transformer_frame.lineno}, '
-                        f'in transformer "{self.__class__.__name__}"\n  '
-                        f"  >> {transformer_frame.line}"
-                    )
-                else:
-                    exception_message = (
-                        f'An error occurred in transformer "{self.__class__.__name__}"'
-                    )
-
-                transform_exception = TransformerException(
-                    internal_exception=exception,
-                    raiser_transformer=self,
-                    message=exception_message,
-                )
+            transform_exception = catch_transformer_exception(exception, self)
 
         if transform_exception is not None:
             raise transform_exception.internal_exception
 
         if type(transformed) is not None:
             return cast(_Out, transformed)
 
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     def copy(
         self,
         transform: Callable[[BaseTransformer, _In], Awaitable[_Out]] | None = None,
         regenerate_instance_id: bool = False,
     ) -> "AsyncTransformer[_In, _Out]":
         copied = copy.copy(self)
@@ -209,9 +180,9 @@
             BaseTransformer[_Out, _Out7, Any],
         ],
     ) -> (
         "AsyncTransformer[_In, tuple[_NextOut, _Out2, _Out3, _Out4, _Out5, _Out6, _Out7]]"
     ):
         pass
 
-    def __rshift__(self, next_node):
+    def __rshift__(self, next_node):  # pragma: no cover
         pass
```

### Comparing `gloe-0.5.4/gloe/base_transformer.py` & `gloe-0.5.5/gloe/base_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     get_origin,
     TypeAlias,
     Type,
 )
 from uuid import UUID
 from itertools import groupby
 
-from gloe._utils import _format_return_annotation
+from gloe._typing_utils import _format_return_annotation
 
 __all__ = ["BaseTransformer", "TransformerException", "PreviousTransformer"]
 
 _In = TypeVar("_In")
 _Out = TypeVar("_Out")
 _NextOut = TypeVar("_NextOut")
 _Self = TypeVar("_Self", bound="BaseTransformer")
@@ -176,15 +176,15 @@
                 previous_transformer._set_previous(previous)
         elif isinstance(self.previous, BaseTransformer):
             self.previous._set_previous(previous)
 
     def signature(self) -> Signature:
         return self._signature(type(self))
 
-    def _signature(self, klass: Type) -> Signature:
+    def _signature(self, klass: Type, transform_method: str = "transform") -> Signature:
         orig_bases = getattr(self, "__orig_bases__", [])
         transformer_args = [
             get_args(base) for base in orig_bases if get_origin(base) == klass
         ]
         generic_args = [
             get_args(base) for base in orig_bases if get_origin(base) == Generic
         ]
@@ -201,15 +201,15 @@
             transformer_arg = transformer_args[0]
             specific_args = {
                 generic: specific
                 for generic, specific in zip(generic_arg, get_args(orig_class))
                 if generic in transformer_arg
             }
 
-        signature = inspect.signature(self.transform)
+        signature = inspect.signature(getattr(self, transform_method))
         new_return_annotation = specific_args.get(
             signature.return_annotation, signature.return_annotation
         )
         parameters = list(signature.parameters.values())
         if len(parameters) > 0:
             parameter = parameters[0]
             parameter = parameter.replace(
@@ -380,16 +380,15 @@
 
     def graph(self) -> DiGraph:
         net = nx.DiGraph()
         net.graph["splines"] = "ortho"
         self._dag(net)
         return net
 
-    # pragma: not covered
-    def export(self, path: str, with_edge_labels: bool = True):
+    def export(self, path: str, with_edge_labels: bool = True):  # pragma: no cover
         net = self.graph()
         boxed_nodes = [
             node
             for node in net.nodes.data()
             if "parent_id" in node[1] and "bounding_box" in node[1]
         ]
         if not with_edge_labels:
```

### Comparing `gloe-0.5.4/gloe/collection/_map.py` & `gloe-0.5.5/gloe/collection/_map.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/gloe/collection/_mapover.py` & `gloe-0.5.5/gloe/collection/_mapover.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/gloe/conditional/_conditioner.py` & `gloe-0.5.5/gloe/conditional/_conditioner.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/gloe/ensurer/_transformer_ensurer.py` & `gloe-0.5.5/gloe/ensurer/_transformer_ensurer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from abc import abstractmethod, ABC
 from types import FunctionType
 from typing import Any, Callable, Generic, ParamSpec, Sequence, TypeVar, cast, overload
 
+from gloe.exceptions import UnsupportedTransformerArgException
 from gloe.async_transformer import AsyncTransformer
-from gloe.functional import _PartialTransformer, _PartialAsyncTransformer
 from gloe.transformers import Transformer
 
 _T = TypeVar("_T")
 _S = TypeVar("_S")
 _U = TypeVar("_U")
 _P1 = ParamSpec("_P1")
 
@@ -18,34 +18,24 @@
     def validate_input(self, data: _T):
         """Perform a validation on incoming data before execute the transformer code"""
 
     @abstractmethod
     def validate_output(self, data: _T, output: _S):
         """Perform a validation on outcome data after execute the transformer code"""
 
-    def __call__(self, transformer: Transformer[_T, _S]) -> Transformer[_T, _S]:
-        def transform(this: Transformer, data: _T) -> _S:
-            self.validate_input(data)
-            output = transformer.transform(data)
-            self.validate_output(data, output)
-            return output
-
-        transformer_cp = transformer.copy(transform)
-        return transformer_cp
-
 
 def input_ensurer(func: Callable[[_T], Any]) -> TransformerEnsurer[_T, Any]:
     class LambdaEnsurer(TransformerEnsurer[_T, _S]):
         __doc__ = func.__doc__
         __annotations__ = cast(FunctionType, func).__annotations__
 
         def validate_input(self, data: _T):
             func(data)
 
-        def validate_output(self, data: _T, output: _S):
+        def validate_output(self, data: _T, output: _S):  # pragma: no cover
             pass
 
     return LambdaEnsurer()
 
 
 @overload
 def output_ensurer(func: Callable[[_T, _S], Any]) -> TransformerEnsurer[_T, _S]:
@@ -58,15 +48,15 @@
 
 
 def output_ensurer(func: Callable):
     class LambdaEnsurer(TransformerEnsurer):
         __doc__ = func.__doc__
         __annotations__ = cast(FunctionType, func).__annotations__
 
-        def validate_input(self, data):
+        def validate_input(self, data):  # pragma: no cover
             pass
 
         def validate_output(self, data, output):
             if len(inspect.signature(func).parameters) == 1:
                 func(output)
             else:
                 func(data, output)
@@ -76,60 +66,59 @@
 
 class _ensure_base:
     @overload
     def __call__(self, transformer: Transformer[_U, _S]) -> Transformer[_U, _S]:
         pass
 
     @overload
-    def __call__(
-        self, transformer_init: _PartialTransformer[_T, _P1, _U]
-    ) -> _PartialTransformer[_T, _P1, _U]:
+    def __call__(self, transformer: AsyncTransformer[_U, _S]) -> AsyncTransformer[_U, _S]:
         pass
 
     @overload
-    def __call__(self, transformer: AsyncTransformer[_U, _S]) -> AsyncTransformer[_U, _S]:
+    def __call__(
+        self, partial_transformer: Callable[_P1, Transformer[_T, _U]]
+    ) -> Callable[_P1, Transformer[_T, _U]]:
         pass
 
     @overload
     def __call__(
-        self, transformer_init: _PartialAsyncTransformer[_T, _P1, _U]
-    ) -> _PartialAsyncTransformer[_T, _P1, _U]:
+        self, partial_transformer: Callable[_P1, AsyncTransformer[_T, _U]]
+    ) -> Callable[_P1, AsyncTransformer[_T, _U]]:
         pass
 
     def __call__(self, arg):
         if isinstance(arg, Transformer):
             return self._generate_new_transformer(arg)
         if isinstance(arg, AsyncTransformer):
             return self._generate_new_async_transformer(arg)
-        if isinstance(arg, _PartialTransformer):
+        if callable(arg):
             transformer_init = arg
 
             def ensured_transformer_init(*args, **kwargs):
                 transformer = transformer_init(*args, **kwargs)
-                return self._generate_new_transformer(transformer)
+                if isinstance(transformer, Transformer):
+                    return self._generate_new_transformer(transformer)
+                if isinstance(transformer, AsyncTransformer):
+                    return self._generate_new_async_transformer(transformer)
 
-            return ensured_transformer_init
-        if isinstance(arg, _PartialAsyncTransformer):
-            async_transformer_init = arg
+                raise UnsupportedTransformerArgException(transformer)
 
-            def ensured_async_transformer_init(*args, **kwargs):
-                async_transformer = async_transformer_init(*args, **kwargs)
-                return self._generate_new_async_transformer(async_transformer)
+            return ensured_transformer_init
 
-            return ensured_async_transformer_init
+        raise UnsupportedTransformerArgException(arg)
 
     @abstractmethod
     def _generate_new_transformer(self, transformer: Transformer) -> Transformer:
-        pass
+        """Internally generates a new sync transformer"""
 
     @abstractmethod
     def _generate_new_async_transformer(
         self, transformer: AsyncTransformer
     ) -> AsyncTransformer:
-        pass
+        """Internally generates a new async transformer"""
 
 
 class _ensure_incoming(Generic[_T], _ensure_base):
     def __init__(self, incoming: Sequence[Callable[[_T], Any]]):
         self.input_ensurers_instances = [input_ensurer(ensurer) for ensurer in incoming]
 
     def _generate_new_transformer(self, transformer: Transformer) -> Transformer:
```

### Comparing `gloe-0.5.4/gloe/experimental/_bridge.py` & `gloe-0.5.5/gloe/experimental/_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/gloe/functional.py` & `gloe-0.5.5/gloe/functional.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,41 +26,17 @@
 S = TypeVar("S")
 S2 = TypeVar("S2")
 P1 = ParamSpec("P1")
 P2 = ParamSpec("P2")
 O = TypeVar("O")
 
 
-class _PartialTransformer(Generic[A, P1, S]):
-    def __init__(self, func: Callable[Concatenate[A, P1], S]):
-        self.func = func
-
-    def __call__(self, *args: P1.args, **kwargs: P1.kwargs) -> Transformer[A, S]:
-        func = self.func
-        func_signature = inspect.signature(func)
-
-        class LambdaTransformer(Transformer[A, S]):
-            __doc__ = func.__doc__
-            __annotations__ = cast(FunctionType, func).__annotations__
-
-            def signature(self) -> Signature:
-                return func_signature
-
-            def transform(self, data: A) -> S:
-                return func(data, *args, **kwargs)
-
-        lambda_transformer = LambdaTransformer()
-        lambda_transformer.__class__.__name__ = func.__name__
-        lambda_transformer._label = func.__name__
-        return lambda_transformer
-
-
 def partial_transformer(
     func: Callable[Concatenate[A, P1], S]
-) -> _PartialTransformer[A, P1, S]:
+) -> Callable[P1, Transformer[A, S]]:
     """
     This decorator let us create partial transformers, which are transformers that
     allow for partial application of their arguments. This capability is particularly
     useful for creating configurable transformer instances where some arguments are preset
     enhancing modularity and reusability in data processing pipelines.
 
     See Also:
@@ -85,49 +61,43 @@
     Args:
         func: A callable with one or more arguments. The first argument is of
             type :code:`A`. The subsequent arguments are retained for use during
             transformer instantiation. This callable returns a value of type
             :code:`S`.
 
     Returns:
-        An instance of the :code:`_PartialTransformer`, an internal class utilized within
-        Gloe that facilitates partial instantiation of transformers by the user.
-        The underlying mechanics of :code:`_PartialTransformer` are managed internally,
-        the user just needs to understand its usage.
+        A callable that receives the same arguments as :code:`func`, excluding the first
+        one and returns a transformer with incoming type being :code:`A` and with
+        :code:`S` as the outcome type.
     """
-    return _PartialTransformer(func)
-
-
-class _PartialAsyncTransformer(Generic[A, P1, S]):
-    def __init__(self, func: Callable[Concatenate[A, P1], Awaitable[S]]):
-        self.func = func
 
-    def __call__(self, *args: P1.args, **kwargs: P1.kwargs) -> AsyncTransformer[A, S]:
-        func = self.func
+    def partial(*args: P1.args, **kwargs: P1.kwargs) -> Transformer[A, S]:
         func_signature = inspect.signature(func)
 
-        class LambdaTransformer(AsyncTransformer[A, S]):
+        class LambdaTransformer(Transformer[A, S]):
             __doc__ = func.__doc__
             __annotations__ = cast(FunctionType, func).__annotations__
 
             def signature(self) -> Signature:
                 return func_signature
 
-            async def transform_async(self, data: A) -> S:
-                return await func(data, *args, **kwargs)
+            def transform(self, data: A) -> S:
+                return func(data, *args, **kwargs)
 
         lambda_transformer = LambdaTransformer()
         lambda_transformer.__class__.__name__ = func.__name__
         lambda_transformer._label = func.__name__
         return lambda_transformer
 
+    return partial
+
 
 def partial_async_transformer(
     func: Callable[Concatenate[A, P1], Awaitable[S]]
-) -> _PartialAsyncTransformer[A, P1, S]:
+) -> Callable[P1, AsyncTransformer[A, S]]:
     """
     This decorator enables the creation of partial asynchronous transformers, which are
     transformers capable of partial argument application. Such functionality is invaluable
     for crafting reusable asynchronous transformer instances where certain arguments are
     predetermined, enhancing both modularity and reusability within asynchronous data
     processing flows.
 
@@ -154,20 +124,38 @@
         func: A callable with one or more arguments, the first of which is of type `A`.
             Remaining arguments are preserved for later use during the instantiation of
             the transformer. This callable must asynchronously return a result of type
             `S`, indicating an operation that produces an output of type `S` upon
             completion.
 
     Returns:
-        An instance of the :code:`_PartialAsyncTransformer`, an internally managed class
-        within Gloe designed to facilitate the partial instantiation of asynchronous
-        transformers. Users are encouraged to understand its application, as the
-        underlying mechanics of :code:`_PartialAsyncTransformer` are handled internally.
+        A callable that receives the same arguments as :code:`func`, excluding the first
+        one and returns an async transformer with incoming type being :code:`A` and with
+        :code:`S` as the outcome type.
     """
-    return _PartialAsyncTransformer(func)
+
+    def partial(*args: P1.args, **kwargs: P1.kwargs) -> AsyncTransformer[A, S]:
+        func_signature = inspect.signature(func)
+
+        class LambdaTransformer(AsyncTransformer[A, S]):
+            __doc__ = func.__doc__
+            __annotations__ = cast(FunctionType, func).__annotations__
+
+            def signature(self) -> Signature:
+                return func_signature
+
+            async def transform_async(self, data: A) -> S:
+                return await func(data, *args, **kwargs)
+
+        lambda_transformer = LambdaTransformer()
+        lambda_transformer.__class__.__name__ = func.__name__
+        lambda_transformer._label = func.__name__
+        return lambda_transformer
+
+    return partial
 
 
 def transformer(func: Callable[[A], S]) -> Transformer[A, S]:
     """
     Convert a callable to an instance of the Transformer class.
 
     Example:
```

### Comparing `gloe-0.5.4/gloe/transformers.py` & `gloe-0.5.5/gloe/transformers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import traceback
 from abc import ABC, abstractmethod
 from inspect import Signature
 
 from typing import (
     TypeVar,
     overload,
     cast,
     Any,
     TypeAlias,
     Union,
 )
 
+from gloe._transformer_utils import catch_transformer_exception
 from gloe.base_transformer import BaseTransformer, TransformerException
 from gloe.async_transformer import AsyncTransformer
 
 __all__ = ["Transformer"]
 
 I = TypeVar("I")
 O = TypeVar("O")
@@ -110,52 +110,23 @@
     def __call__(self, data: I) -> O:
         transform_exception = None
 
         transformed: O | None = None
         try:
             transformed = self.transform(data)
         except Exception as exception:
-            if type(exception.__cause__) == TransformerException:
-                transform_exception = exception.__cause__
-            else:
-                tb = traceback.extract_tb(exception.__traceback__)
-
-                # TODO: Make this filter condition stronger
-                transformer_frames = [
-                    frame
-                    for frame in tb
-                    if frame.name == self.__class__.__name__ or frame.name == "transform"
-                ]
-
-                if len(transformer_frames) == 1:
-                    transformer_frame = transformer_frames[0]
-                    exception_message = (
-                        f"\n  "
-                        f'File "{transformer_frame.filename}", line {transformer_frame.lineno}, '
-                        f'in transformer "{self.__class__.__name__}"\n  '
-                        f"  >> {transformer_frame.line}"
-                    )
-                else:
-                    exception_message = (
-                        f'An error occurred in transformer "{self.__class__.__name__}"'
-                    )
-
-                transform_exception = TransformerException(
-                    internal_exception=exception,
-                    raiser_transformer=self,
-                    message=exception_message,
-                )
+            transform_exception = catch_transformer_exception(exception, self)
 
         if transform_exception is not None:
             raise transform_exception.internal_exception
 
         if type(transformed) is not None:
             return cast(O, transformed)
 
-        raise NotImplementedError
+        raise NotImplementedError  # pragma: no cover
 
     @overload
     def __rshift__(
         self,
         next_node: tuple["Tr[O, O1]", "Tr[O, O2]"],
     ) -> "Tr[I, tuple[O1, O2]]":
         pass
@@ -251,9 +222,9 @@
     @overload
     def __rshift__(
         self,
         next_node: AsyncNext7[O, O1, O2, O3, O4, O5, O6, O7],
     ) -> AsyncTransformer[I, tuple[O1, O2, O3, O4, O5, O6, O7]]:
         pass
 
-    def __rshift__(self, next_node):
+    def __rshift__(self, next_node):  # pragma: no cover
         pass
```

### Comparing `gloe-0.5.4/gloe.egg-info/PKG-INFO` & `gloe-0.5.5/gloe.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: gloe
-Version: 0.5.4
-Summary: Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows.
+Version: 0.5.5
+Summary: Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code.
 Author-email: Samir Braga <samirchavess@gmail.com>
 Project-URL: Homepage, https://gloe.ideos.com.br
 Project-URL: Documentation, https://gloe.ideos.com.br
 Project-URL: Issues, https://github.com/ideos/gloe/issues
 Project-URL: Repository, https://github.com/ideos/gloe
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: typing_extensions~=4.7.1
 Requires-Dist: schemdraw~=0.16
@@ -22,40 +25,36 @@
 ***
 
 <div align="center">
   <img src="https://github.com/ideos/gloe/raw/main/docs/source/_static/assets/gloe-logo.png"><br>
 </div>
 
 
-| | |
-| --- |-|
-| Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml)|
-| Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)|
-| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE) | 
+| |                                                                                                                                                                                                                                                             |
+| --- |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| Testing | [![CI - Test](https://github.com/ideos/gloe/actions/workflows/test.yml/badge.svg)](https://github.com/ideos/gloe/actions/workflows/test.yml) [![Coverage](https://codecov.io/github/ideos/gloe/coverage.svg?branch=main)](https://codecov.io/gh/ideos/gloe) |
+| Package | [![PyPI Latest Release](https://img.shields.io/pypi/v/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe) [![Supported Python versions](https://img.shields.io/pypi/pyversions/gloe.svg?color=%2334D058)](https://pypi.org/project/gloe)              |
+| Meta | [![License - Apache 2.0](https://img.shields.io/pypi/l/gloe.svg?color=%2304b367)](https://github.com/ideos/gloe/blob/main/LICENSE)                                                                                                                          | 
 
+**Documentation**: [gloe.ideos.com.br](https://gloe.ideos.com.br)
 
+# Write a Better Python Code
 
-Let Gloe help you
-===
-
-Gloe (pronounced /ɡloʊ/, like "glow") is a general purpose library made to help developers to create, maintain, document and test operational and data flows. It can be used in data science and machine learning pipelines as well in servers, scripts or wherever else one identifies a lack between the code and the understanding of logical business. Gloe was not thought to be used in the entire application even less replacing any existing library, it was built to be integrated with other tools and to be implemented where the code complexity can be bigger than the desired.
-
-## Documentation
-
-The official documentation is hosted on [gloe.ideos.com.br](https://gloe.ideos.com.br).
+Gloe (pronounced /ɡloʊ/, like "glow") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code. It is particularly useful in data science and machine learning pipelines, as well as in servers and scripts, or any area where there is a gap between the code and the logical business understanding. Gloe is not intended to be used across an entire application or to replace existing libraries. Instead, it is built to integrate with other tools and to address areas where the code complexity may be higher than expected.
 
 ## Motivation
 
-Software development has a lot of patterns and good practices related to the code itself, like how to document, to test, to structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
+Software development has lots of patterns and good practices related to the code itself, like how to document, test, structure and what programming paradigm to use. However, beyond all that, we believe that the key point of a successful software project is a good communication between everyone involved in the development. Of course, this communication is not necessarily restricted to meetings or text messages, it is present also in documentation artifacts and in a well-written code.
 
-When a developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, the story can be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software will take a long time to understand the narrative and make it clear, or they might give up and leave it as is.
+When developers write a code, they are telling a story to the next person who will read or/and refactor it. Depending on the code's quality, this story could be quite confusing, with no clear roles of the characters and a messy plot (sometimes with an undesired twist). The next person to maintain the software may take a long time to clearly understand the narrative and make it clear, or they will simply give up, leaving it as is.
 
 
+### How Gloe Can Help Me?
 
-Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into concise steps with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
+Gloe comes to turn this story coherent, logically organized and easy to follow. This is achieved by dividing the code into [concise steps](https://gloe.ideos.com.br/theory.html) with an unambiguous responsibility and explicit interface. Then, Gloe allows you to connect these steps, clarifying their collaboration and identifying necessary changes during refactoring. Thus, you can quickly understand the entire story being told and enhance it. Inspired by things like [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) and Free Monad (present in [Scala](https://typelevel.org/cats/datatypes/freemonad.html) and [Haskell](https://serokell.io/blog/introduction-to-free-monads)), Gloe implemented this approach using functional programming and strong typing concepts.
 
 ### Gloe is not a workflow orchestrator
 
 Currently, unlike platforms like [Air Flow](https://airflow.apache.org/) that include scheduler backends for task orchestration, Gloe's primary purpose is to aid in development. The graph structure, which will be discussed in subsequent sections, aims to make the code [more flat and hence readable](https://en.wikibooks.org/wiki/Computer_Programming/Coding_Style/Minimize_nesting). However, it is important to note that Gloe does not offer functionalities for executing tasks in a dedicated environment, nor does it directly contribute to execution speed or scalability improvements.
 
 ## Installing
```

### Comparing `gloe-0.5.4/gloe.egg-info/SOURCES.txt` & `gloe-0.5.5/gloe.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 MANIFEST.in
-Makefile
 README.md
 pyproject.toml
 docs/source/conf.py
 docs/source/docutils.conf
 docs/source/index.md
 docs/source/limitations.md
 docs/source/theory.md
+docs/source/_static/robots.txt
 docs/source/_static/theme_customs.css
 docs/source/_static/assets/favicon.ico
 docs/source/_static/assets/gloe-logo-small.png
 docs/source/_static/assets/gloe-logo.png
 docs/source/_static/assets/graph_example.jpeg
+docs/source/_templates/page.html
 docs/source/api-reference/gloe.collection.md
 docs/source/api-reference/gloe.experimental.md
 docs/source/api-reference/gloe.utils.md
 docs/source/api-reference/index.md
 docs/source/getting-started/async-transformers.md
 docs/source/getting-started/conditional-flows.md
 docs/source/getting-started/ensurers.md
@@ -24,15 +25,16 @@
 docs/source/getting-started/partial-transformers.md
 docs/source/getting-started/plotting.md
 docs/source/getting-started/transformers.md
 docs/source/getting-started/utilities.md
 docs/source/pygments/styles.py
 gloe/__init__.py
 gloe/_composition_utils.py
-gloe/_utils.py
+gloe/_transformer_utils.py
+gloe/_typing_utils.py
 gloe/async_transformer.py
 gloe/base_transformer.py
 gloe/functional.py
 gloe/py.typed
 gloe/transformers.py
 gloe/utils.py
 gloe.egg-info/PKG-INFO
```

### Comparing `gloe-0.5.4/pyproject.toml` & `gloe-0.5.5/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gloe"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="Samir Braga", email="samirchavess@gmail.com" },
 ]
-description = "Gloe is a general purpose library made to help developers to create, maintain, document and test operational and data flows."
+description = "Gloe (pronounced /ɡloʊ/, like \"glow\") is a general-purpose library made to help developers create, maintain, document, and test both operational and flow-oriented code."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'typing_extensions~=4.7.1',
     'schemdraw~=0.16',
     'setuptools~=61.2.0',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gloe-0.5.4/tests/lib/ensurers.py` & `gloe-0.5.5/tests/lib/ensurers.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/tests/lib/transformers.py` & `gloe-0.5.5/tests/lib/transformers.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,7 +88,12 @@
 
 @partial_transformer
 def repeat(content: str, n_times: int, linebreak: bool) -> str:
     repeated = content * n_times
     if linebreak:
         repeated += "\n"
     return repeated
+
+
+@transformer
+def identity(num: float) -> float:
+    return num
```

### Comparing `gloe-0.5.4/tests/test_conditioner_transformer.py` & `gloe-0.5.5/tests/test_conditioner_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/tests/test_function_transformer.py` & `gloe-0.5.5/tests/test_function_transformer.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/tests/test_transformer_bridge.py` & `gloe-0.5.5/tests/test_transformer_bridge.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/tests/test_transformer_collections.py` & `gloe-0.5.5/tests/test_transformer_collections.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/tests/test_transformer_graph.py` & `gloe-0.5.5/tests/test_transformer_graph.py`

 * *Files identical despite different names*

### Comparing `gloe-0.5.4/tests/test_transformer_types.py` & `gloe-0.5.5/tests/test_transformer_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import asyncio
 import os
 import unittest
-from collections.abc import Sequence
 from pathlib import Path
-from typing import Iterable, TypeVar, Any
-
+from typing import TypeVar
 from typing_extensions import assert_type
 
 from tests.lib.conditioners import if_not_zero, if_is_even
 from tests.lib.ensurers import is_even, same_value, same_value_int, is_greater_than_10
 from tests.lib.transformers import (
     square,
     square_root,
```

