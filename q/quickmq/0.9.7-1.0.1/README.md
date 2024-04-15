# Comparing `tmp/QuickMQ-0.9.7.tar.gz` & `tmp/quickmq-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuickMQ-0.9.7.tar", last modified: Wed Mar  6 17:44:48 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `QuickMQ-0.9.7.tar` & `quickmq-1.0.1.tar`

### file list

```diff
@@ -1,28 +1,18 @@
-drwxr-xr-x   0 mdrex     (1000) mdrex     (1000)        0 2024-03-06 17:44:48.169846 QuickMQ-0.9.7/
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     1071 2023-12-20 15:12:42.000000 QuickMQ-0.9.7/LICENSE
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     5424 2024-03-06 17:44:48.169846 QuickMQ-0.9.7/PKG-INFO
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     3485 2024-02-12 18:26:53.000000 QuickMQ-0.9.7/README.md
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     2501 2024-02-12 18:26:53.000000 QuickMQ-0.9.7/pyproject.toml
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)       38 2024-03-06 17:44:48.169846 QuickMQ-0.9.7/setup.cfg
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      128 2023-12-20 15:12:42.000000 QuickMQ-0.9.7/setup.py
-drwxr-xr-x   0 mdrex     (1000) mdrex     (1000)        0 2024-03-06 17:44:48.159846 QuickMQ-0.9.7/src/
-drwxr-xr-x   0 mdrex     (1000) mdrex     (1000)        0 2024-03-06 17:44:48.169846 QuickMQ-0.9.7/src/QuickMQ.egg-info/
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     5424 2024-03-06 17:44:48.000000 QuickMQ-0.9.7/src/QuickMQ.egg-info/PKG-INFO
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      519 2024-03-06 17:44:48.000000 QuickMQ-0.9.7/src/QuickMQ.egg-info/SOURCES.txt
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)        1 2024-03-06 17:44:48.000000 QuickMQ-0.9.7/src/QuickMQ.egg-info/dependency_links.txt
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)       50 2024-03-06 17:44:48.000000 QuickMQ-0.9.7/src/QuickMQ.egg-info/entry_points.txt
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)       79 2024-03-06 17:44:48.000000 QuickMQ-0.9.7/src/QuickMQ.egg-info/requires.txt
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)        8 2024-03-06 17:44:48.000000 QuickMQ-0.9.7/src/QuickMQ.egg-info/top_level.txt
-drwxr-xr-x   0 mdrex     (1000) mdrex     (1000)        0 2024-03-06 17:44:48.169846 QuickMQ-0.9.7/src/quickmq/
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      465 2024-03-06 17:44:25.000000 QuickMQ-0.9.7/src/quickmq/__init__.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     4673 2023-12-30 00:56:55.000000 QuickMQ-0.9.7/src/quickmq/__main__.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     9268 2024-03-06 17:38:47.000000 QuickMQ-0.9.7/src/quickmq/abstracts.py
-drwxr-xr-x   0 mdrex     (1000) mdrex     (1000)        0 2024-03-06 17:44:48.169846 QuickMQ-0.9.7/src/quickmq/adapters/
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      120 2023-12-20 15:26:05.000000 QuickMQ-0.9.7/src/quickmq/adapters/__init__.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     6029 2024-02-23 18:41:35.000000 QuickMQ-0.9.7/src/quickmq/adapters/pika.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      911 2023-12-26 22:33:51.000000 QuickMQ-0.9.7/src/quickmq/api.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     6436 2024-03-01 17:19:35.000000 QuickMQ-0.9.7/src/quickmq/client.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)     4106 2024-01-02 19:43:34.000000 QuickMQ-0.9.7/src/quickmq/config.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      575 2024-02-21 18:44:39.000000 QuickMQ-0.9.7/src/quickmq/exceptions.py
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)        0 2023-12-20 15:12:42.000000 QuickMQ-0.9.7/src/quickmq/py.typed
--rw-r--r--   0 mdrex     (1000) mdrex     (1000)      522 2024-03-06 17:39:19.000000 QuickMQ-0.9.7/src/quickmq/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.1/CONTRIBUTING
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 quickmq-1.0.1/requirements-dev.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 quickmq-1.0.1/requirements.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 quickmq-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 quickmq-1.0.1/docs/reqs-and-specs.md
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/__about__.py
+-rw-r--r--   0        0        0    10736 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/__init__.py
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/_defs.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/_utils.py
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 quickmq-1.0.1/src/ssec_amqp/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_api.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_client.py
+-rw-r--r--   0        0        0     3641 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_exchange.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 quickmq-1.0.1/tests/test_utils.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 quickmq-1.0.1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 quickmq-1.0.1/README.md
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 quickmq-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 quickmq-1.0.1/PKG-INFO
```

