# Comparing `tmp/acceldata_sdk-3.2.0.tar.gz` & `tmp/acceldata_sdk-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acceldata_sdk-3.2.0.tar", last modified: Thu Mar 21 11:21:52 2024, max compression
+gzip compressed data, was "acceldata_sdk-3.3.0.tar", last modified: Mon Apr 15 09:07:02 2024, max compression
```

## Comparing `acceldata_sdk-3.2.0.tar` & `acceldata_sdk-3.3.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.346109 acceldata_sdk-3.2.0/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      110 2024-03-21 11:14:24.000000 acceldata_sdk-3.2.0/CHANGELOG.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/DATASOURCE_README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/LICENCE.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/MANIFEST.in
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23661 2024-03-21 11:21:52.345637 acceldata_sdk-3.2.0/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    18890 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/README.md
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/README.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.333734 acceldata_sdk-3.2.0/acceldata_sdk/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     7776 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/common.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2098 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      329 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/datetime_utils.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/errors.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.336089 acceldata_sdk-3.2.0/acceldata_sdk/events/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/events/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      903 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/events/generic_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/events/job_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      826 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/events/log_events.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1487 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/events/span_event.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/initialiser.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.340702 acceldata_sdk-3.2.0/acceldata_sdk/models/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/__init__.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     6106 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/assetType.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10021 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/connection.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3522 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/create_asset.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     8164 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/datasource.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10268 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/dqrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4599 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/job.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    24639 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/pipeline.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2015 2024-03-21 11:14:24.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/profile.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11785 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/reconcillationrule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/rule.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10102 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/ruleExecutionResult.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     2396 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/span.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    10582 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/span_context.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/models/tags.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15832 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    47793 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/acceldata_sdk/torch_http_client.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.345033 acceldata_sdk-3.2.0/acceldata_sdk.egg-info/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    23661 2024-03-21 11:21:52.000000 acceldata_sdk-3.2.0/acceldata_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1923 2024-03-21 11:21:52.000000 acceldata_sdk-3.2.0/acceldata_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-03-21 11:21:52.000000 acceldata_sdk-3.2.0/acceldata_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2024-03-21 11:21:52.000000 acceldata_sdk-3.2.0/acceldata_sdk.egg-info/requires.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2024-03-21 11:21:52.000000 acceldata_sdk-3.2.0/acceldata_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.340918 acceldata_sdk-3.2.0/docs/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.330081 acceldata_sdk-3.2.0/docs/_build/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.330166 acceldata_sdk-3.2.0/docs/_build/html/
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.342410 acceldata_sdk-3.2.0/docs/_build/html/_sources/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/modules.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/readme.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/readme_datasource.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/readme_pipeline.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/_build/html/_sources/torch_sdk.rst.txt
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/docs/conf.py
-drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-03-21 11:21:52.344181 acceldata_sdk-3.2.0/integration_tests/
--rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/integration_tests/test_constants.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     3765 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/integration_tests/test_ds_assets.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    11805 2024-03-21 11:14:17.000000 acceldata_sdk-3.2.0/integration_tests/test_external_integration_default_time.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    15535 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/integration_tests/test_external_integration_explicit_time.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/integration_tests/test_pipelines.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     4386 2024-02-22 04:32:27.000000 acceldata_sdk-3.2.0/integration_tests/test_policy.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)    26175 2024-03-21 11:14:17.000000 acceldata_sdk-3.2.0/integration_tests/test_torch_client.py
--rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-03-21 11:21:52.346186 acceldata_sdk-3.2.0/setup.cfg
--rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2024-03-21 11:14:24.000000 acceldata_sdk-3.2.0/setup.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.452101 acceldata_sdk-3.3.0/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       91 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/CHANGELOG.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3952 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/DATASOURCE_README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1082 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/LICENCE.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       31 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/MANIFEST.in
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23642 2024-04-15 09:07:02.451700 acceldata_sdk-3.3.0/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    18890 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/README.md
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      196 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/README.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.440179 acceldata_sdk-3.3.0/acceldata_sdk/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1227 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     7776 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/common.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2098 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      329 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/datetime_utils.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      172 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/errors.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.442022 acceldata_sdk-3.3.0/acceldata_sdk/events/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        0 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      903 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/generic_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1016 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/job_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      826 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/log_events.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1487 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/events/span_event.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      328 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/initialiser.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.446176 acceldata_sdk-3.3.0/acceldata_sdk/models/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      162 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/__init__.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     6106 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      664 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/assetType.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10021 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/connection.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3522 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/create_asset.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     8164 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/datasource.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10268 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/dqrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4599 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/job.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    24639 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/pipeline.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2015 2024-03-21 11:14:24.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/profile.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11785 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/reconcillationrule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     5929 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/rule.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10102 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/ruleExecutionResult.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     2396 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/span.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    10582 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/span_context.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3810 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/models/tags.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15832 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/acceldata_sdk/torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    48544 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/acceldata_sdk/torch_http_client.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.451055 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    23642 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1923 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)        1 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      117 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/requires.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       14 2024-04-15 09:07:02.000000 acceldata_sdk-3.3.0/acceldata_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.446411 acceldata_sdk-3.3.0/docs/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.435983 acceldata_sdk-3.3.0/docs/_build/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.436046 acceldata_sdk-3.3.0/docs/_build/html/
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.448592 acceldata_sdk-3.3.0/docs/_build/html/_sources/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      491 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       72 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/modules.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       54 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/readme.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       45 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/readme_datasource.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       34 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/readme_pipeline.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      921 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.events.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1731 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.models.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1070 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.rst.txt
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1946 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/docs/conf.py
+drwxr-xr-x   0 sangeetamishra   (502) staff       (20)        0 2024-04-15 09:07:02.450745 acceldata_sdk-3.3.0/integration_tests/
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)      887 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_constants.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     3765 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_ds_assets.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    11805 2024-03-21 11:14:17.000000 acceldata_sdk-3.3.0/integration_tests/test_external_integration_default_time.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    15535 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_external_integration_explicit_time.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4488 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_pipelines.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     4386 2024-02-22 04:32:27.000000 acceldata_sdk-3.3.0/integration_tests/test_policy.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)    27169 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/integration_tests/test_torch_client.py
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)       38 2024-04-15 09:07:02.452164 acceldata_sdk-3.3.0/setup.cfg
+-rw-r--r--   0 sangeetamishra   (502) staff       (20)     1238 2024-04-15 09:06:32.000000 acceldata_sdk-3.3.0/setup.py
```

### Comparing `acceldata_sdk-3.2.0/DATASOURCE_README.md` & `acceldata_sdk-3.3.0/DATASOURCE_README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/LICENCE.txt` & `acceldata_sdk-3.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/PKG-INFO` & `acceldata_sdk-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 3.2.0
+Version: 3.3.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -519,11 +519,11 @@
 # List all rules
 recon_rules = torch_client.list_all_policies(filter=filter)
 ```
 
 Version Log
 ==========
 
-3.2.0 (14/03/2024)
+3.3.0 (15/04/2024)
 -------------------
-- Implemented profile response handling fixes
+- Improved sample data api
```

### Comparing `acceldata_sdk-3.2.0/README.md` & `acceldata_sdk-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/client.py` & `acceldata_sdk-3.3.0/acceldata_sdk/client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/common.py` & `acceldata_sdk-3.3.0/acceldata_sdk/common.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/constants.py` & `acceldata_sdk-3.3.0/acceldata_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/events/generic_event.py` & `acceldata_sdk-3.3.0/acceldata_sdk/events/generic_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/events/job_events.py` & `acceldata_sdk-3.3.0/acceldata_sdk/events/job_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/events/log_events.py` & `acceldata_sdk-3.3.0/acceldata_sdk/events/log_events.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/events/span_event.py` & `acceldata_sdk-3.3.0/acceldata_sdk/events/span_event.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/asset.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/assetType.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/assetType.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/connection.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/connection.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/create_asset.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/create_asset.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/datasource.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/datasource.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/dqrule.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/dqrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/job.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/job.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/pipeline.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/profile.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/profile.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/reconcillationrule.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/reconcillationrule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/rule.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/rule.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/ruleExecutionResult.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/ruleExecutionResult.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/span.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/span.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/span_context.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/span_context.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/models/tags.py` & `acceldata_sdk-3.3.0/acceldata_sdk/models/tags.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/torch_client.py` & `acceldata_sdk-3.3.0/acceldata_sdk/torch_client.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk/torch_http_client.py` & `acceldata_sdk-3.3.0/acceldata_sdk/torch_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -736,20 +736,39 @@
             url=url,
             payload=payload
         )
         response['data']['client'] = self
         profile_response = Profile(**response['data'])
         return profile_response
 
-    def sample_data(self, id: int):
-        url = f'{self._catalog_api_base}/assets/{id}/sample'
-        response = self._get(
-            url=url
-        )
-        return response
+    def sample_data(self, asset_id: int):
+        url = f'{self._catalog_api_base}/assets/{asset_id}/sample/async'
+        response = self._post(url=url, as_json=True, payload={})
+
+
+        # This is a file/kafka based asset sampling
+        if response is not None and response.get('requestId') is not None:
+            request_id = response['requestId']
+            sample_data_result = self.get_sample_data_result(request_id)
+
+            while sample_data_result['jobExecutionStatus'] == 'IN_PROGRESS':
+                time.sleep(5)
+                sample_data_result = self.get_sample_data_result(request_id)
+
+            return sample_data_result
+        else:
+            return response
+
+
+    def get_sample_data_result(self, request_id: str):
+            url = f'{self._catalog_api_base}/assets/sample/result/{request_id}'
+            response = self._get(
+                url=url
+            )
+            return response
 
     def get_profile_request_details(self, asset_id: int, req_id: int):
         url = f'{self._catalog_api_base}/assets/{asset_id}/profile/{req_id}'
         response = self._get(
             url=url
         )
         return response
```

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk.egg-info/PKG-INFO` & `acceldata_sdk-3.3.0/acceldata_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acceldata_sdk
-Version: 3.2.0
+Version: 3.3.0
 Summary: Acceldata SDK.
 Home-page: 
 Author: acceldata
 Author-email: apisupport@acceldata.io
 License: MIT License
 Keywords: acceldata-sdk
 Classifier: Development Status :: 5 - Production/Stable
@@ -519,11 +519,11 @@
 # List all rules
 recon_rules = torch_client.list_all_policies(filter=filter)
 ```
 
 Version Log
 ==========
 
-3.2.0 (14/03/2024)
+3.3.0 (15/04/2024)
 -------------------
-- Implemented profile response handling fixes
+- Improved sample data api
```

### Comparing `acceldata_sdk-3.2.0/acceldata_sdk.egg-info/SOURCES.txt` & `acceldata_sdk-3.3.0/acceldata_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/docs/_build/html/_sources/torch_sdk.events.rst.txt` & `acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.events.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/docs/_build/html/_sources/torch_sdk.models.rst.txt` & `acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.models.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/docs/_build/html/_sources/torch_sdk.rst.txt` & `acceldata_sdk-3.3.0/docs/_build/html/_sources/torch_sdk.rst.txt`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/docs/conf.py` & `acceldata_sdk-3.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_constants.py` & `acceldata_sdk-3.3.0/integration_tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_ds_assets.py` & `acceldata_sdk-3.3.0/integration_tests/test_ds_assets.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_external_integration_default_time.py` & `acceldata_sdk-3.3.0/integration_tests/test_external_integration_default_time.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_external_integration_explicit_time.py` & `acceldata_sdk-3.3.0/integration_tests/test_external_integration_explicit_time.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_pipelines.py` & `acceldata_sdk-3.3.0/integration_tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_policy.py` & `acceldata_sdk-3.3.0/integration_tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `acceldata_sdk-3.2.0/integration_tests/test_torch_client.py` & `acceldata_sdk-3.3.0/integration_tests/test_torch_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,17 @@
 # Reconciliation Policy constants
 recon_policy_name = "Athena_automation_Hashed_Data_Equality_4_success"
 
 # Datasource name
 datasource_name = "Snowflake_stg"
 
 # Asset UID
-asset_uid = "Snowflake_stg.SNOWFLAKE_SAMPLE_DATA.TPCDS_SF100TCL.CATALOG_RETURNS"
+asset_uid_kafka = "Sample_Kafka.member_updates"
+asset_uid_file = "S3_Demo.trans_detail"
+asset_uid_table = "Snowflake_stg.SNOWFLAKE_SAMPLE_DATA.TPCDS_SF100TCL.CALL_CENTER"
 
 
 class TestTorchClientIntegration(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         # Set up common variables or configurations if needed
@@ -419,73 +421,88 @@
         status = datasource.get_crawler_status()
         pp.pprint(status)
         assert status is not None
 
     # Assets tests
     def test_get_asset_by_uid(self):
         pp.pprint("Validating test test_get_asset_by_uid")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         pp.pprint(asset)
         assert asset is not None
 
     def test_get_asset_by_id(self):
         pp.pprint("Validating test test_get_asset_by_id")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         asset_with_id = self.torch_client.get_asset(asset.id)
         pp.pprint(asset_with_id)
         assert asset_with_id is not None
 
     def test_get_asset_metadata(self):
         pp.pprint("Validating test test_get_asset_metadata")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         metadata_asset = asset.get_metadata()
         pp.pprint(metadata_asset)
         assert metadata_asset is not None
 
-    def test_get_asset_sample_data(self):
-        pp.pprint("Validating test test_get_asset_sample_data")
-        asset = self.torch_client.get_asset(asset_uid)
+    def test_get_asset_sample_data_table(self):
+        pp.pprint("Validating test test_get_asset_sample_data_table")
+        asset = self.torch_client.get_asset(asset_uid_table)
+        pp.pprint("Asset : {}".format(asset))
+        sample_data_asset = asset.sample_data()
+        pp.pprint(sample_data_asset)
+        assert sample_data_asset is not None
+
+    def test_get_asset_sample_data_file(self):
+        pp.pprint("Validating test test_get_asset_sample_data_file")
+        asset = self.torch_client.get_asset(asset_uid_file)
+        sample_data_asset = asset.sample_data()
+        pp.pprint(sample_data_asset)
+        assert sample_data_asset is not None
+
+    def test_get_asset_sample_data_kafka(self):
+        pp.pprint("Validating test test_get_asset_sample_data_kafka")
+        asset = self.torch_client.get_asset(asset_uid_kafka)
         sample_data_asset = asset.sample_data()
         pp.pprint(sample_data_asset)
         assert sample_data_asset is not None
 
     def test_get_asset_labels(self):
         pp.pprint("Validating test test_get_asset_labels")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         labels_asset = asset.get_labels()
         pp.pprint(labels_asset)
         assert labels_asset is not None
 
     def test_add_asset_labels(self):
         pp.pprint("Validating test test_add_asset_labels")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         asset.add_labels(labels=[AssetLabel('test12', 'shubh12'), AssetLabel('test22', 'shubh32')])
         labels_asset = asset.get_labels()
         pp.pprint(labels_asset)
         assert labels_asset is not None
 
     def test_add_asset_custom_metadata(self):
         pp.pprint("Validating test test_add_asset_custom_metadata")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         asset.add_custom_metadata(
             custom_metadata=[CustomAssetMetadata('testcm1', 'shubhcm1'), CustomAssetMetadata('testcm2', 'shubhcm2')])
         metadata_asset = asset.get_metadata()
         pp.pprint(metadata_asset)
         assert metadata_asset is not None
 
     def test_profile_status(self):
         pp.pprint("Validating test test_profile_status")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         latest_profile_status_asset = asset.get_latest_profile_status()
         pp.pprint(latest_profile_status_asset)
         assert latest_profile_status_asset is not None
 
     def test_cancel_profile(self):
         pp.pprint("Validating test test_cancel_profile")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         latest_profile_status_asset = asset.get_latest_profile_status()
         pp.pprint("Latest profile status")
         pp.pprint(latest_profile_status_asset)
         if latest_profile_status_asset.status != 'IN PROGRESS':
             pp.pprint("Triggering profiling start request")
             start_profile_asset = asset.start_profile(ProfilingType.FULL)
             pp.pprint(start_profile_asset)
@@ -495,31 +512,31 @@
                 pp.pprint("Cancelling profiling request")
                 cancel_res = start_profile_asset.cancel()
                 pp.pprint(profile_status)
                 assert cancel_res is not None
         else:
             pp.pprint("Profile execution request already in progress")
 
-
     def test_execute_profile(self):
         pp.pprint("Validating test test_execute_profile")
-        asset = self.torch_client.get_asset(asset_uid)
+        asset = self.torch_client.get_asset(asset_uid_table)
         latest_profile_status_asset = asset.get_latest_profile_status()
         pp.pprint("Latest profile status")
         pp.pprint(latest_profile_status_asset)
         if latest_profile_status_asset.status != 'IN PROGRESS':
             start_profile_asset = asset.start_profile(ProfilingType.FULL)
             pp.pprint(start_profile_asset)
             profile_status = start_profile_asset.get_status()
             pp.pprint("Current profiling result status")
             pp.pprint(profile_status)
             assert profile_status is not None
         else:
             pp.pprint("Profile execution request already in progress")
 
+
 if __name__ == '__main__':
     suite = unittest.TestSuite()
 
     # Pipeline Test cases
     suite.addTest(TestTorchClientIntegration('test_get_torch_version'))
     suite.addTest(TestTorchClientIntegration('test_get_supported_sdk_versions'))
     suite.addTest(TestTorchClientIntegration('test_create_pipeline'))
@@ -559,15 +576,17 @@
     suite.addTest(TestTorchClientIntegration('test_get_datasource_by_id'))
     suite.addTest(TestTorchClientIntegration('test_get_all_data_sources'))
     suite.addTest(TestTorchClientIntegration('test_get_ds_crawler_status'))
     suite.addTest(TestTorchClientIntegration('test_start_crawler'))
     suite.addTest(TestTorchClientIntegration('test_get_asset_by_uid'))
     suite.addTest(TestTorchClientIntegration('test_get_asset_by_id'))
     suite.addTest(TestTorchClientIntegration('test_get_asset_metadata'))
-    suite.addTest(TestTorchClientIntegration('test_get_asset_sample_data'))
+    suite.addTest(TestTorchClientIntegration('test_get_asset_sample_data_table'))
+    suite.addTest(TestTorchClientIntegration('test_get_asset_sample_data_file'))
+    suite.addTest(TestTorchClientIntegration('test_get_asset_sample_data_kafka'))
     suite.addTest(TestTorchClientIntegration('test_get_asset_labels'))
     suite.addTest(TestTorchClientIntegration('test_get_asset_labels'))
     suite.addTest(TestTorchClientIntegration('test_add_asset_labels'))
     suite.addTest(TestTorchClientIntegration('test_add_asset_custom_metadata'))
     suite.addTest(TestTorchClientIntegration('test_execute_profile'))
     suite.addTest(TestTorchClientIntegration('test_profile_status'))
     suite.addTest(TestTorchClientIntegration('test_cancel_profile'))
```

### Comparing `acceldata_sdk-3.2.0/setup.py` & `acceldata_sdk-3.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # except (IOError, ImportError):
 #     description = open('README.md').read()
 
 # Change MIN_TORCH_BACKEND_VERSION_SUPPORTED in constants as well if needed while updating version here
 
 setup(
     name='acceldata_sdk',
-    version='3.2.0',
+    version='3.3.0',
     description='Acceldata SDK.' + '\n\n' + open('README.txt').read(),
     long_description=open('README.md').read() + '\n\n' + open('DATASOURCE_README.md').read() + '\n\n'  + open('CHANGELOG.txt').read(),
     long_description_content_type="text/markdown",
     url='',
     author='acceldata',
     author_email='apisupport@acceldata.io',
     license='MIT License',
```

