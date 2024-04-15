# Comparing `tmp/pgml-1.0.1.tar.gz` & `tmp/pgml-1.0.2.tar.gz`

## Comparing `pgml-1.0.1.tar` & `pgml-1.0.2.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0      501       20      344 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-macros/Cargo.toml
--rw-r--r--   0      501       20     2919 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-macros/src/common.rs
--rw-r--r--   0      501       20    20250 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-macros/src/javascript.rs
--rw-r--r--   0      501       20     1444 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-macros/src/lib.rs
--rw-r--r--   0      501       20    19297 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-macros/src/python.rs
--rw-r--r--   0      501       20     8035 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-macros/src/types.rs
--rw-r--r--   0      501       20      117 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/Cargo.toml
--rw-r--r--   0      501       20      166 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-traits/Cargo.toml
--rw-r--r--   0      501       20     7447 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-traits/src/javascript/mod.rs
--rw-r--r--   0      501       20       37 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-traits/src/lib.rs
--rw-r--r--   0      501       20     2448 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge-traits/src/python/mod.rs
--rw-r--r--   0      501       20      292 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge/Cargo.toml
--rw-r--r--   0      501       20       93 2024-03-27 22:50:53.000000 pgml-1.0.1/rust-bridge/rust-bridge/src/lib.rs
--rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 pgml-1.0.1/pgml/Cargo.toml
--rw-r--r--   0      501       20      240 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/.cargo/config.toml
--rw-r--r--   0      501       20     3171 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/.gitignore
--rw-r--r--   0      501       20      491 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/README.md
--rw-r--r--   0      501       20     2381 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/build.rs
--rw-r--r--   0      501       20       21 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/.npmignore
--rw-r--r--   0      501       20     9605 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/README.md
--rw-r--r--   0      501       20     1371 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/build.js
--rw-r--r--   0      501       20     1598 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/README.md
--rw-r--r--   0      501       20     1614 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/extractive_question_answering.js
--rw-r--r--   0      501       20      983 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/package-lock.json
--rw-r--r--   0      501       20      282 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/package.json
--rw-r--r--   0      501       20     1260 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/question_answering.js
--rw-r--r--   0      501       20     1549 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/question_answering_instructor.js
--rw-r--r--   0      501       20     1229 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/semantic_search.js
--rw-r--r--   0      501       20     1625 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/summarizing_question_answering.js
--rw-r--r--   0      501       20      844 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/webpack/README.md
--rw-r--r--   0      501       20    52794 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/webpack/package-lock.json
--rw-r--r--   0      501       20      409 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/webpack/package.json
--rw-r--r--   0      501       20      249 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/webpack/src/get_classification.js
--rw-r--r--   0      501       20      580 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/webpack/src/index.js
--rw-r--r--   0      501       20      353 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/examples/webpack/webpack.config.js
--rw-r--r--   0      501       20      874 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/index.js
--rw-r--r--   0      501       20     1400 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/package-lock.json
--rw-r--r--   0      501       20      757 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/package.json
--rw-r--r--   0      501       20      163 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/tests/jest.config.js
--rw-r--r--   0      501       20   132336 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/tests/package-lock.json
--rw-r--r--   0      501       20      302 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/tests/package.json
--rw-r--r--   0      501       20    12331 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/tests/tsconfig.json
--rw-r--r--   0      501       20    10267 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript/tests/typescript-tests/test.ts
--rwxr-xr-x   0      501       20       77 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript-cli/index.js
--rw-r--r--   0      501       20      621 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript-cli/package-lock.json
--rw-r--r--   0      501       20      549 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/javascript-cli/package.json
--rw-r--r--   0      501       20   221092 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/poetry.lock
--rw-r--r--   0      501       20    12145 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/README.md
--rw-r--r--   0      501       20     2151 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/README.md
--rw-r--r--   0      501       20     2063 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/extractive_question_answering.py
--rw-r--r--   0      501       20     1552 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/question_answering.py
--rw-r--r--   0      501       20     2088 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/question_answering_instructor.py
--rw-r--r--   0      501       20     2897 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/rag_question_answering.py
--rw-r--r--   0      501       20      597 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/requirements.txt
--rw-r--r--   0      501       20     1609 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/semantic_search.py
--rw-r--r--   0      501       20     2095 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/summarizing_question_answering.py
--rw-r--r--   0      501       20     2012 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/examples/table_question_answering.py
--rwxr-xr-x   0      501       20      251 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/manual-build-deploy.sh
--rw-r--r--   0      501       20      101 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/pgml/__init__.py
--rw-r--r--   0      501       20       92 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/pgml/__main__.py
--rw-r--r--   0      501       20     5041 2024-03-27 22:56:03.000000 pgml-1.0.1/pgml/python/pgml/pgml.pyi
--rw-r--r--   0      501       20     2926 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/tests/stress_test.py
--rw-r--r--   0      501       20    12137 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/python/tests/test.py
--rw-r--r--   0      501       20     3444 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/builtins.rs
--rw-r--r--   0      501       20    11058 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/cli.rs
--rw-r--r--   0      501       20    52044 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/collection.rs
--rw-r--r--   0      501       20    15602 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/filter_builder.rs
--rw-r--r--   0      501       20     8855 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/languages/javascript.rs
--rw-r--r--   0      501       20       95 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/languages/mod.rs
--rw-r--r--   0      501       20     6688 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/languages/python.rs
--rw-r--r--   0      501       20    65478 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/lib.rs
--rw-r--r--   0      501       20     2855 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/migrations/mod.rs
--rw-r--r--   0      501       20     2981 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/migrations/pgml--0.9.1--0.9.2.rs
--rw-r--r--   0      501       20      353 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/migrations/pgml--0.9.2--1.0.0.rs
--rw-r--r--   0      501       20     4772 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/model.rs
--rw-r--r--   0      501       20     1936 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/models.rs
--rw-r--r--   0      501       20    17200 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/open_source_ai.rs
--rw-r--r--   0      501       20     3240 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/order_by_builder.rs
--rw-r--r--   0      501       20    34091 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/pipeline.rs
--rw-r--r--   0      501       20    11559 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/queries.rs
--rw-r--r--   0      501       20     3046 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/query_builder.rs
--rw-r--r--   0      501       20     2784 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/query_runner.rs
--rw-r--r--   0      501       20     6569 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/remote_embeddings.rs
--rw-r--r--   0      501       20    23304 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/search_query_builder.rs
--rw-r--r--   0      501       20     4766 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/single_field_pipeline.rs
--rw-r--r--   0      501       20     3388 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/splitter.rs
--rw-r--r--   0      501       20      406 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/sql/fdw.sql
--rw-r--r--   0      501       20      174 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/sql/fdw_drop.sql
--rw-r--r--   0      501       20    10994 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/transformer_pipeline.rs
--rw-r--r--   0      501       20     4034 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/types.rs
--rw-r--r--   0      501       20     4675 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/utils.rs
--rw-r--r--   0      501       20     8992 2024-03-27 22:50:53.000000 pgml-1.0.1/pgml/src/vector_search_query_builder.rs
--rw-r--r--   0      501       20    79837 2024-03-27 22:54:41.000000 pgml-1.0.1/pgml/Cargo.lock
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pgml-1.0.1/pyproject.toml
--rw-r--r--   0      501       20      101 2024-03-27 22:50:53.000000 pgml-1.0.1/python/pgml/__init__.py
--rw-r--r--   0      501       20     5041 2024-03-27 22:56:03.000000 pgml-1.0.1/python/pgml/pgml.pyi
--rw-r--r--   0      501       20       92 2024-03-27 22:50:53.000000 pgml-1.0.1/python/pgml/__main__.py
--rw-r--r--   0      501       20    12145 2024-03-27 22:50:53.000000 pgml-1.0.1/python/README.md
--rw-r--r--   0        0        0    13009 1970-01-01 00:00:00.000000 pgml-1.0.1/PKG-INFO
+-rw-r--r--   0      501       20      292 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge/Cargo.toml
+-rw-r--r--   0      501       20       93 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge/src/lib.rs
+-rw-r--r--   0      501       20      117 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/Cargo.toml
+-rw-r--r--   0      501       20      166 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-traits/Cargo.toml
+-rw-r--r--   0      501       20     7447 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-traits/src/javascript/mod.rs
+-rw-r--r--   0      501       20       37 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-traits/src/lib.rs
+-rw-r--r--   0      501       20     2448 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-traits/src/python/mod.rs
+-rw-r--r--   0      501       20      344 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-macros/Cargo.toml
+-rw-r--r--   0      501       20     2919 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-macros/src/common.rs
+-rw-r--r--   0      501       20    20250 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-macros/src/javascript.rs
+-rw-r--r--   0      501       20     1444 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-macros/src/lib.rs
+-rw-r--r--   0      501       20    19297 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-macros/src/python.rs
+-rw-r--r--   0      501       20     8035 2024-04-15 19:00:27.000000 pgml-1.0.2/rust-bridge/rust-bridge-macros/src/types.rs
+-rw-r--r--   0        0        0     1945 1970-01-01 00:00:00.000000 pgml-1.0.2/pgml/Cargo.toml
+-rw-r--r--   0      501       20      240 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/.cargo/config.toml
+-rw-r--r--   0      501       20     3171 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/.gitignore
+-rw-r--r--   0      501       20      491 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/README.md
+-rw-r--r--   0      501       20     2381 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/build.rs
+-rw-r--r--   0      501       20       21 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/.npmignore
+-rw-r--r--   0      501       20     9605 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/README.md
+-rw-r--r--   0      501       20     1371 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/build.js
+-rw-r--r--   0      501       20     1598 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/README.md
+-rw-r--r--   0      501       20     1614 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/extractive_question_answering.js
+-rw-r--r--   0      501       20      983 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/package-lock.json
+-rw-r--r--   0      501       20      282 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/package.json
+-rw-r--r--   0      501       20     1260 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/question_answering.js
+-rw-r--r--   0      501       20     1549 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/question_answering_instructor.js
+-rw-r--r--   0      501       20     1229 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/semantic_search.js
+-rw-r--r--   0      501       20     1625 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/summarizing_question_answering.js
+-rw-r--r--   0      501       20      844 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/webpack/README.md
+-rw-r--r--   0      501       20    52794 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/webpack/package-lock.json
+-rw-r--r--   0      501       20      409 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/webpack/package.json
+-rw-r--r--   0      501       20      249 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/webpack/src/get_classification.js
+-rw-r--r--   0      501       20      580 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/webpack/src/index.js
+-rw-r--r--   0      501       20      353 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/examples/webpack/webpack.config.js
+-rw-r--r--   0      501       20      874 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/index.js
+-rw-r--r--   0      501       20     1400 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/package-lock.json
+-rw-r--r--   0      501       20      757 2024-04-15 20:41:32.000000 pgml-1.0.2/pgml/javascript/package.json
+-rw-r--r--   0      501       20      163 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/tests/jest.config.js
+-rw-r--r--   0      501       20   132336 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/tests/package-lock.json
+-rw-r--r--   0      501       20      302 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/tests/package.json
+-rw-r--r--   0      501       20    12331 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/tests/tsconfig.json
+-rw-r--r--   0      501       20    10267 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript/tests/typescript-tests/test.ts
+-rwxr-xr-x   0      501       20       77 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript-cli/index.js
+-rw-r--r--   0      501       20      621 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript-cli/package-lock.json
+-rw-r--r--   0      501       20      549 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/javascript-cli/package.json
+-rw-r--r--   0      501       20   221092 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/poetry.lock
+-rw-r--r--   0      501       20    12145 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/README.md
+-rw-r--r--   0      501       20     2151 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/README.md
+-rw-r--r--   0      501       20     2063 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/extractive_question_answering.py
+-rw-r--r--   0      501       20     1552 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/question_answering.py
+-rw-r--r--   0      501       20     2088 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/question_answering_instructor.py
+-rw-r--r--   0      501       20     2897 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/rag_question_answering.py
+-rw-r--r--   0      501       20      597 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/requirements.txt
+-rw-r--r--   0      501       20     1609 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/semantic_search.py
+-rw-r--r--   0      501       20     2095 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/summarizing_question_answering.py
+-rw-r--r--   0      501       20     2012 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/examples/table_question_answering.py
+-rwxr-xr-x   0      501       20      251 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/manual-build-deploy.sh
+-rw-r--r--   0      501       20      101 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/pgml/__init__.py
+-rw-r--r--   0      501       20       92 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/pgml/__main__.py
+-rw-r--r--   0      501       20     5041 2024-04-15 20:44:36.000000 pgml-1.0.2/pgml/python/pgml/pgml.pyi
+-rw-r--r--   0      501       20     2926 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/tests/stress_test.py
+-rw-r--r--   0      501       20    12137 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/python/tests/test.py
+-rw-r--r--   0      501       20     3444 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/builtins.rs
+-rw-r--r--   0      501       20    11058 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/cli.rs
+-rw-r--r--   0      501       20    52044 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/collection.rs
+-rw-r--r--   0      501       20    15602 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/filter_builder.rs
+-rw-r--r--   0      501       20     8855 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/languages/javascript.rs
+-rw-r--r--   0      501       20       95 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/languages/mod.rs
+-rw-r--r--   0      501       20     6688 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/languages/python.rs
+-rw-r--r--   0      501       20    65478 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/lib.rs
+-rw-r--r--   0      501       20     2855 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/migrations/mod.rs
+-rw-r--r--   0      501       20     2981 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/migrations/pgml--0.9.1--0.9.2.rs
+-rw-r--r--   0      501       20      353 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/migrations/pgml--0.9.2--1.0.0.rs
+-rw-r--r--   0      501       20     4772 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/model.rs
+-rw-r--r--   0      501       20     1936 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/models.rs
+-rw-r--r--   0      501       20    17200 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/open_source_ai.rs
+-rw-r--r--   0      501       20     3240 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/order_by_builder.rs
+-rw-r--r--   0      501       20    34091 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/pipeline.rs
+-rw-r--r--   0      501       20    11559 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/queries.rs
+-rw-r--r--   0      501       20     3046 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/query_builder.rs
+-rw-r--r--   0      501       20     2784 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/query_runner.rs
+-rw-r--r--   0      501       20     6569 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/remote_embeddings.rs
+-rw-r--r--   0      501       20    23304 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/search_query_builder.rs
+-rw-r--r--   0      501       20     4766 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/single_field_pipeline.rs
+-rw-r--r--   0      501       20     3388 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/splitter.rs
+-rw-r--r--   0      501       20      406 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/sql/fdw.sql
+-rw-r--r--   0      501       20      174 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/sql/fdw_drop.sql
+-rw-r--r--   0      501       20     9029 2024-04-15 20:41:32.000000 pgml-1.0.2/pgml/src/transformer_pipeline.rs
+-rw-r--r--   0      501       20     3994 2024-04-15 20:41:32.000000 pgml-1.0.2/pgml/src/types.rs
+-rw-r--r--   0      501       20     4675 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/utils.rs
+-rw-r--r--   0      501       20     8992 2024-04-15 19:00:27.000000 pgml-1.0.2/pgml/src/vector_search_query_builder.rs
+-rw-r--r--   0      501       20    79837 2024-04-15 20:43:23.000000 pgml-1.0.2/pgml/Cargo.lock
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 pgml-1.0.2/pyproject.toml
+-rw-r--r--   0      501       20      101 2024-04-15 19:00:27.000000 pgml-1.0.2/python/pgml/__init__.py
+-rw-r--r--   0      501       20     5041 2024-04-15 20:44:36.000000 pgml-1.0.2/python/pgml/pgml.pyi
+-rw-r--r--   0      501       20       92 2024-04-15 19:00:27.000000 pgml-1.0.2/python/pgml/__main__.py
+-rw-r--r--   0      501       20    12145 2024-04-15 19:00:27.000000 pgml-1.0.2/python/README.md
+-rw-r--r--   0        0        0    13009 1970-01-01 00:00:00.000000 pgml-1.0.2/PKG-INFO
```

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-macros/src/common.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-macros/src/common.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-macros/src/javascript.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-macros/src/javascript.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-macros/src/lib.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-macros/src/python.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-macros/src/python.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-macros/src/types.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-macros/src/types.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-traits/src/javascript/mod.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-traits/src/javascript/mod.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/rust-bridge/rust-bridge-traits/src/python/mod.rs` & `pgml-1.0.2/rust-bridge/rust-bridge-traits/src/python/mod.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/Cargo.toml` & `pgml-1.0.2/pgml/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pgml"
-version = "1.0.1"
+version = "1.0.2"
 edition = "2021"
 authors = ["PosgresML <team@postgresml.org>"]
 homepage = "https://postgresml.org/"
 repository = ""
 license = "MIT"
 keywords = ["postgres", "machine learning", "vector databases", "embeddings"]
```

### Comparing `pgml-1.0.1/pgml/.gitignore` & `pgml-1.0.2/pgml/.gitignore`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/build.rs` & `pgml-1.0.2/pgml/build.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/README.md` & `pgml-1.0.2/pgml/javascript/README.md`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/build.js` & `pgml-1.0.2/pgml/javascript/build.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/README.md` & `pgml-1.0.2/pgml/javascript/examples/README.md`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/extractive_question_answering.js` & `pgml-1.0.2/pgml/javascript/examples/extractive_question_answering.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/package-lock.json` & `pgml-1.0.2/pgml/javascript/examples/package-lock.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/question_answering.js` & `pgml-1.0.2/pgml/javascript/examples/question_answering.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/question_answering_instructor.js` & `pgml-1.0.2/pgml/javascript/examples/question_answering_instructor.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/semantic_search.js` & `pgml-1.0.2/pgml/javascript/examples/semantic_search.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/summarizing_question_answering.js` & `pgml-1.0.2/pgml/javascript/examples/summarizing_question_answering.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/webpack/README.md` & `pgml-1.0.2/pgml/javascript/examples/webpack/README.md`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/webpack/package-lock.json` & `pgml-1.0.2/pgml/javascript/examples/webpack/package-lock.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/examples/webpack/src/index.js` & `pgml-1.0.2/pgml/javascript/examples/webpack/src/index.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/index.js` & `pgml-1.0.2/pgml/javascript/index.js`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/package-lock.json` & `pgml-1.0.2/pgml/javascript/package-lock.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/package.json` & `pgml-1.0.2/pgml/javascript/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.0.2'"}*

```diff
@@ -25,9 +25,9 @@
         "type": "git",
         "url": "https://github.com/postgresml/postgresml"
     },
     "scripts": {
         "build": "node build.js",
         "build-release": "node build.js --release"
     },
-    "version": "1.0.1"
+    "version": "1.0.2"
 }
```

### Comparing `pgml-1.0.1/pgml/javascript/tests/package-lock.json` & `pgml-1.0.2/pgml/javascript/tests/package-lock.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/tests/tsconfig.json` & `pgml-1.0.2/pgml/javascript/tests/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript/tests/typescript-tests/test.ts` & `pgml-1.0.2/pgml/javascript/tests/typescript-tests/test.ts`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript-cli/package-lock.json` & `pgml-1.0.2/pgml/javascript-cli/package-lock.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/javascript-cli/package.json` & `pgml-1.0.2/pgml/javascript-cli/package.json`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/poetry.lock` & `pgml-1.0.2/pgml/poetry.lock`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/README.md` & `pgml-1.0.2/pgml/python/README.md`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/README.md` & `pgml-1.0.2/pgml/python/examples/README.md`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/extractive_question_answering.py` & `pgml-1.0.2/pgml/python/examples/extractive_question_answering.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/question_answering.py` & `pgml-1.0.2/pgml/python/examples/question_answering.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/question_answering_instructor.py` & `pgml-1.0.2/pgml/python/examples/question_answering_instructor.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/rag_question_answering.py` & `pgml-1.0.2/pgml/python/examples/rag_question_answering.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/requirements.txt` & `pgml-1.0.2/pgml/python/examples/requirements.txt`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/semantic_search.py` & `pgml-1.0.2/pgml/python/examples/semantic_search.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/summarizing_question_answering.py` & `pgml-1.0.2/pgml/python/examples/summarizing_question_answering.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/examples/table_question_answering.py` & `pgml-1.0.2/pgml/python/examples/table_question_answering.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/pgml/pgml.pyi` & `pgml-1.0.2/pgml/python/pgml/pgml.pyi`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/tests/stress_test.py` & `pgml-1.0.2/pgml/python/tests/stress_test.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/python/tests/test.py` & `pgml-1.0.2/pgml/python/tests/test.py`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/builtins.rs` & `pgml-1.0.2/pgml/src/builtins.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/cli.rs` & `pgml-1.0.2/pgml/src/cli.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/collection.rs` & `pgml-1.0.2/pgml/src/collection.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/filter_builder.rs` & `pgml-1.0.2/pgml/src/filter_builder.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/languages/javascript.rs` & `pgml-1.0.2/pgml/src/languages/javascript.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/languages/python.rs` & `pgml-1.0.2/pgml/src/languages/python.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/lib.rs` & `pgml-1.0.2/pgml/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/migrations/mod.rs` & `pgml-1.0.2/pgml/src/migrations/mod.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/migrations/pgml--0.9.1--0.9.2.rs` & `pgml-1.0.2/pgml/src/migrations/pgml--0.9.1--0.9.2.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/model.rs` & `pgml-1.0.2/pgml/src/model.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/models.rs` & `pgml-1.0.2/pgml/src/models.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/open_source_ai.rs` & `pgml-1.0.2/pgml/src/open_source_ai.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/order_by_builder.rs` & `pgml-1.0.2/pgml/src/order_by_builder.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/pipeline.rs` & `pgml-1.0.2/pgml/src/pipeline.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/queries.rs` & `pgml-1.0.2/pgml/src/queries.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/query_builder.rs` & `pgml-1.0.2/pgml/src/query_builder.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/query_runner.rs` & `pgml-1.0.2/pgml/src/query_runner.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/remote_embeddings.rs` & `pgml-1.0.2/pgml/src/remote_embeddings.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/search_query_builder.rs` & `pgml-1.0.2/pgml/src/search_query_builder.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/single_field_pipeline.rs` & `pgml-1.0.2/pgml/src/single_field_pipeline.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/splitter.rs` & `pgml-1.0.2/pgml/src/splitter.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/transformer_pipeline.rs` & `pgml-1.0.2/pgml/src/transformer_pipeline.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 use anyhow::Context;
-use futures::Stream;
 use rust_bridge::{alias, alias_methods};
-use sqlx::{postgres::PgRow, Row};
-use sqlx::{Postgres, Transaction};
-use std::collections::VecDeque;
-use std::future::Future;
-use std::pin::Pin;
-use std::task::Poll;
+use sqlx::Row;
 use tracing::instrument;
 
 /// Provides access to builtin database methods
 #[derive(alias, Debug, Clone)]
 pub struct TransformerPipeline {
     task: Json,
     database_url: Option<String>,
@@ -18,107 +12,14 @@
 
 use crate::types::GeneralJsonAsyncIterator;
 use crate::{get_or_initialize_pool, types::Json};
 
 #[cfg(feature = "python")]
 use crate::types::{GeneralJsonAsyncIteratorPython, JsonPython};
 
-#[allow(clippy::type_complexity)]
-struct TransformerStream {
-    transaction: Option<Transaction<'static, Postgres>>,
-    future: Option<Pin<Box<dyn Future<Output = Result<Vec<PgRow>, sqlx::Error>> + Send + 'static>>>,
-    commit: Option<Pin<Box<dyn Future<Output = Result<(), sqlx::Error>> + Send + 'static>>>,
-    done: bool,
-    query: String,
-    db_batch_size: i32,
-    results: VecDeque<PgRow>,
-}
-
-impl std::fmt::Debug for TransformerStream {
-    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
-        f.debug_struct("TransformerStream").finish()
-    }
-}
-
-impl TransformerStream {
-    fn new(transaction: Transaction<'static, Postgres>, db_batch_size: i32) -> Self {
-        let query = format!("FETCH {} FROM c", db_batch_size);
-        Self {
-            transaction: Some(transaction),
-            future: None,
-            commit: None,
-            done: false,
-            query,
-            db_batch_size,
-            results: VecDeque::new(),
-        }
-    }
-}
-
-impl Stream for TransformerStream {
-    type Item = anyhow::Result<Json>;
-
-    fn poll_next(
-        mut self: Pin<&mut Self>,
-        cx: &mut std::task::Context<'_>,
-    ) -> Poll<Option<Self::Item>> {
-        if self.done {
-            if let Some(c) = self.commit.as_mut() {
-                if c.as_mut().poll(cx).is_ready() {
-                    self.commit = None;
-                }
-            }
-        } else {
-            if self.future.is_none() {
-                unsafe {
-                    let s = self.as_mut().get_unchecked_mut();
-                    let s: *mut Self = s;
-                    let s = Box::leak(Box::from_raw(s));
-                    s.future = Some(Box::pin(
-                        sqlx::query(&s.query).fetch_all(&mut **s.transaction.as_mut().unwrap()),
-                    ));
-                }
-            }
-
-            if let Poll::Ready(o) = self.as_mut().future.as_mut().unwrap().as_mut().poll(cx) {
-                let rows = o?;
-                if rows.len() < self.db_batch_size as usize {
-                    self.done = true;
-                    unsafe {
-                        let s = self.as_mut().get_unchecked_mut();
-                        let transaction = std::mem::take(&mut s.transaction).unwrap();
-                        s.commit = Some(Box::pin(transaction.commit()));
-                    }
-                } else {
-                    unsafe {
-                        let s = self.as_mut().get_unchecked_mut();
-                        let s: *mut Self = s;
-                        let s = Box::leak(Box::from_raw(s));
-                        s.future = Some(Box::pin(
-                            sqlx::query(&s.query).fetch_all(&mut **s.transaction.as_mut().unwrap()),
-                        ));
-                    }
-                }
-                for r in rows.into_iter() {
-                    self.results.push_back(r)
-                }
-            }
-        }
-
-        if !self.results.is_empty() {
-            let r = self.results.pop_front().unwrap();
-            Poll::Ready(Some(Ok(r.get::<Json, _>(0))))
-        } else if self.done {
-            Poll::Ready(None)
-        } else {
-            Poll::Pending
-        }
-    }
-}
-
 #[alias_methods(new, transform, transform_stream)]
 impl TransformerPipeline {
     /// Creates a new [TransformerPipeline]
     ///
     /// # Arguments
     /// * `task` - The task to run
     /// * `model` - The model to use
@@ -196,15 +97,15 @@
         &self,
         input: Json,
         args: Option<Json>,
         batch_size: Option<i32>,
     ) -> anyhow::Result<GeneralJsonAsyncIterator> {
         let pool = get_or_initialize_pool(&self.database_url).await?;
         let args = args.unwrap_or_default();
-        let batch_size = batch_size.unwrap_or(10);
+        let batch_size = batch_size.unwrap_or(1);
 
         let mut transaction = pool.begin().await?;
         // We set the task in the new constructor so we can unwrap here
         if self.task["task"].as_str().unwrap() == "conversational" {
             let inputs = input
                 .as_array()
                 .context("`input` to transformer_stream must be an array of objects")?
@@ -230,18 +131,45 @@
             .bind(&self.task)
             .bind(input)
             .bind(&args)
             .execute(&mut *transaction)
             .await?;
         }
 
-        Ok(GeneralJsonAsyncIterator(Box::pin(TransformerStream::new(
-            transaction,
-            batch_size,
-        ))))
+        let s = futures::stream::try_unfold(transaction, move |mut transaction| async move {
+            let query = format!("FETCH {} FROM c", batch_size);
+            let mut res: Vec<Json> = sqlx::query_scalar(&query)
+                .fetch_all(&mut *transaction)
+                .await?;
+            if !res.is_empty() {
+                if batch_size > 1 {
+                    let res: Vec<String> = res
+                        .into_iter()
+                        .map(|v| {
+                            v.0.as_array()
+                                .context("internal SDK error - cannot parse db value as array. Please post a new github issue")
+                                .map(|v| {
+                                    v[0].as_str()
+                                        .context(
+                                            "internal SDK error - cannot parse db value as string. Please post a new github issue",
+                                        )
+                                        .map(|v| v.to_owned())
+                                })
+                        })
+                        .collect::<anyhow::Result<anyhow::Result<Vec<String>>>>()??;
+                    Ok(Some((serde_json::json!(res).into(), transaction)))
+                } else {
+                    Ok(Some((std::mem::take(&mut res[0]), transaction)))
+                }
+            } else {
+                transaction.commit().await?;
+                Ok(None)
+            }
+        });
+        Ok(GeneralJsonAsyncIterator(Box::pin(s)))
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use crate::internal_init_logger;
@@ -301,15 +229,15 @@
             None,
         );
         let mut stream = t
             .transform_stream(
                 serde_json::json!("AI is going to").into(),
                 Some(
                     serde_json::json!({
-                        "max_new_tokens": 10
+                        "max_new_tokens": 30
                     })
                     .into(),
                 ),
                 None,
             )
             .await?;
         while let Some(o) = stream.next().await {
```

### Comparing `pgml-1.0.1/pgml/src/types.rs` & `pgml-1.0.2/pgml/src/types.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use anyhow::Context;
-use futures::{Stream, StreamExt};
+use futures::{stream::BoxStream, Stream, StreamExt};
 use itertools::Itertools;
 use rust_bridge::alias_manual;
 use sea_query::Iden;
 use serde::{Deserialize, Serialize};
 use std::ops::{Deref, DerefMut};
 
 /// A wrapper around `serde_json::Value`
@@ -119,19 +119,17 @@
         self.split('.')
             .map(|s| SIden::String(s.to_string()))
             .collect_tuple()
             .expect("Malformed table name in IntoTableNameAndSchema")
     }
 }
 
-/// A wrapper around `std::pin::Pin<Box<dyn Stream<Item = anyhow::Result<Json>> + Send>>`
+/// A wrapper around `BoxStream<'static, anyhow::Result<Json>>`
 #[derive(alias_manual)]
-pub struct GeneralJsonAsyncIterator(
-    pub std::pin::Pin<Box<dyn Stream<Item = anyhow::Result<Json>> + Send>>,
-);
+pub struct GeneralJsonAsyncIterator(pub BoxStream<'static, anyhow::Result<Json>>);
 
 impl Stream for GeneralJsonAsyncIterator {
     type Item = anyhow::Result<Json>;
 
     fn poll_next(
         mut self: std::pin::Pin<&mut Self>,
         cx: &mut std::task::Context<'_>,
```

### Comparing `pgml-1.0.1/pgml/src/utils.rs` & `pgml-1.0.2/pgml/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/src/vector_search_query_builder.rs` & `pgml-1.0.2/pgml/src/vector_search_query_builder.rs`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/pgml/Cargo.lock` & `pgml-1.0.2/pgml/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1527,15 +1527,15 @@
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pgml"
-version = "1.0.1"
+version = "1.0.2"
 dependencies = [
  "anyhow",
  "async-trait",
  "chrono",
  "clap",
  "colored",
  "ctrlc",
```

### Comparing `pgml-1.0.1/pyproject.toml` & `pgml-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0", "patchelf"]
 build-backend = "maturin"
 
 [project]
 name = "pgml"
 requires-python = ">=3.7"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python SDK is designed to facilitate the development of scalable vector search applications on PostgreSQL databases."
 authors = [
   {name = "PostgresML",  email = "team@postgresml.org"},
 ]
 readme = "./python/README.md"
 keywords = ["postgres","machine learning","vector databases","embeddings"]
 classifiers = [
```

### Comparing `pgml-1.0.1/python/pgml/pgml.pyi` & `pgml-1.0.2/python/pgml/pgml.pyi`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/python/README.md` & `pgml-1.0.2/python/README.md`

 * *Files identical despite different names*

### Comparing `pgml-1.0.1/PKG-INFO` & `pgml-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pgml
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python SDK is designed to facilitate the development of scalable vector search applications on PostgreSQL databases.
 Keywords: postgres,machine learning,vector databases,embeddings
 Home-Page: https://postgresml.org/
 Author: PosgresML <team@postgresml.org>
```

