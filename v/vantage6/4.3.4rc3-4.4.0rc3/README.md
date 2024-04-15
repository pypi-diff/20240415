# Comparing `tmp/vantage6-4.3.4rc3.tar.gz` & `tmp/vantage6-4.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-4.3.4rc3.tar", last modified: Mon Mar 25 11:02:00 2024, max compression
+gzip compressed data, was "vantage6-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:19 2024, max compression
```

## Comparing `vantage6-4.3.4rc3.tar` & `vantage6-4.4.0rc3.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.167181 vantage6-4.3.4rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:02:00.167181 vantage6-4.3.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.155181 vantage6-4.3.4rc3/tests_cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/tests_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/tests_cli/test_example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/tests_cli/test_node_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/tests_cli/test_server_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/tests_cli/test_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.151181 vantage6-4.3.4rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.155181 vantage6-4.3.4rc3/vantage6/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/__build__
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.155181 vantage6-4.3.4rc3/vantage6/cli/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algorithm/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algorithm/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.159181 vantage6-4.3.4rc3/vantage6/cli/algostore/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algostore/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algostore/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algostore/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algostore/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algostore/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/algostore/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.159181 vantage6-4.3.4rc3/vantage6/cli/common/
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/common/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/common/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/configuration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17022 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/configuration_wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.159181 vantage6-4.3.4rc3/vantage6/cli/context/
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/context/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/context/base_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/context/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/context/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.159181 vantage6-4.3.4rc3/vantage6/cli/dev/
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/dev/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/dev/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/dev/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/dev/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/node/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/node/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/create_private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/set_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    11986 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/node/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/rabbitmq/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/rabbitmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/rabbitmq/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/rabbitmq/queue_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/rabbitmq/rabbitmq.config
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/attach.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/server/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/import_.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/new.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     7650 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/start.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/stop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/template/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/template/node_config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/template/server_config.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/template/server_import_config.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.163181 vantage6-4.3.4rc3/vantage6/cli/test/common/
--rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/test/common/diagnostic_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/test/feature_tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/test/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-03-25 11:01:46.000000 vantage6-4.3.4rc3/vantage6/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:00.155181 vantage6-4.3.4rc3/vantage6.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-03-25 11:02:00.000000 vantage6-4.3.4rc3/vantage6.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-03-25 11:02:00.000000 vantage6-4.3.4rc3/vantage6.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:02:00.000000 vantage6-4.3.4rc3/vantage6.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-25 11:02:00.000000 vantage6-4.3.4rc3/vantage6.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-25 11:02:00.000000 vantage6-4.3.4rc3/vantage6.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 11:02:00.000000 vantage6-4.3.4rc3/vantage6.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/tests_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15937 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_node_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_server_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/tests_cli/test_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.047506 vantage6-4.4.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/vantage6/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/vantage6/cli/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algorithm/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algorithm/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/algostore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/algostore/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/common/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/common/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/configuration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/configuration_wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/base_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7409 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/context/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/dev/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/node/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.055506 vantage6-4.4.0rc3/vantage6/cli/node/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/create_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/set_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11893 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/node/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/queue_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/rabbitmq/rabbitmq.config
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/attach.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/import_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/stop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/template/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/template/node_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/template/server_config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/template/server_import_config.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.059506 vantage6-4.4.0rc3/vantage6/cli/test/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/test/common/diagnostic_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/test/feature_tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3802 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/test/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-15 13:15:06.000000 vantage6-4.4.0rc3/vantage6/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:19.051506 vantage6-4.4.0rc3/vantage6.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 13:15:19.000000 vantage6-4.4.0rc3/vantage6.egg-info/top_level.txt
```

### Comparing `vantage6-4.3.4rc3/PKG-INFO` & `vantage6-4.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.3.4rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6 Version: 4.4.0rc3 Summary: vantage6
 command line interface Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-4.3.4rc3/setup.py` & `vantage6-4.4.0rc3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/vantage6/vantage6",
     packages=find_namespace_packages(),
     python_requires=">=3.10",
     install_requires=[
         "click==8.1.3",
         "colorama==0.4.6",
-        "copier==8.3.0",
+        "copier==9.2.0",
         "docker==6.1.2",
         "ipython==8.10.0",
         "jinja2==3.1.3",
         "questionary==1.10.0",
         "rich==13.5.2",
         "schema==0.7.5",
         "SQLAlchemy==1.4.46",
```

### Comparing `vantage6-4.3.4rc3/tests_cli/test_node_cli.py` & `vantage6-4.4.0rc3/tests_cli/test_node_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
         # Check that error is produced
         self.assertEqual(result.output[:7], "[error]")
 
         # check for non zero exit-code
         self.assertNotEqual(result.exit_code, 0)
 
     @patch("docker.DockerClient.volumes")
-    @patch("vantage6.cli.node.start.pull_if_newer")
+    @patch("vantage6.cli.node.start.pull_image")
     @patch("vantage6.cli.common.decorator.get_context")
     @patch("docker.DockerClient.containers")
     @patch("vantage6.cli.node.start.check_docker_running", return_value=True)
     def test_start(self, check_docker, client, context, pull, volumes):
         # client.containers = MagicMock(name="docker.DockerClient.containers")
         client.list.return_value = []
         volume = MagicMock()
```

### Comparing `vantage6-4.3.4rc3/tests_cli/test_server_cli.py` & `vantage6-4.4.0rc3/tests_cli/test_server_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from vantage6.cli.server.attach import cli_server_attach
 
 
 class ServerCLITest(unittest.TestCase):
     @patch("vantage6.cli.server.start.NetworkManager")
     @patch("vantage6.cli.server.start.docker.types.Mount")
     @patch("os.makedirs")
-    @patch("vantage6.cli.common.start.pull_if_newer")
+    @patch("vantage6.cli.server.start.pull_image")
     @patch("vantage6.cli.common.decorator.get_context")
     @patch("vantage6.cli.server.start.docker.from_env")
     @patch("vantage6.cli.common.start.check_docker_running", return_value=True)
     def test_start(
         self,
         docker_check,
         containers,
@@ -87,17 +87,18 @@
 
         self.assertIsNone(result.exception)
         self.assertEqual(result.exit_code, 0)
 
     @patch("docker.DockerClient.containers")
     @patch("vantage6.cli.server.import_.print_log_worker")
     @patch("vantage6.cli.server.import_.click.Path")
+    @patch("vantage6.cli.server.import_.pull_image")
     @patch("vantage6.cli.server.import_.check_docker_running", return_value=True)
     @patch("vantage6.cli.common.decorator.get_context")
-    def test_import(self, context, docker_check, click_path, log, containers):
+    def test_import(self, context, docker_check, pull, click_path, log, containers):
         """Import entities without errors."""
         click_path.return_value = MagicMock()
 
         ctx = MagicMock()
         ctx.name = "some-name"
         context.return_value = ctx
```

### Comparing `vantage6-4.3.4rc3/tests_cli/test_wizard.py` & `vantage6-4.4.0rc3/tests_cli/test_wizard.py`

 * *Files 16% similar despite different names*

```diff
@@ -67,15 +67,23 @@
             for key in nesting:
                 self.assertIn(key, current_config)
                 current_config = current_config[key]
 
     def test_server_wizard(self):
         with patch(f"{module_path}.q") as q:
             q.prompt.side_effect = self.prompts
-            q.confirm.return_value.ask.side_effect = [True, True, True, True, True]
+            q.confirm.return_value.ask.side_effect = [
+                True,
+                True,
+                True,
+                True,
+                True,
+                True,
+                False,
+            ]
 
             config = server_configuration_questionaire("vantage6")
 
             keys = [
                 "description",
                 "ip",
                 "port",
@@ -83,14 +91,15 @@
                 "uri",
                 "allow_drop_all",
                 "jwt_secret_key",
                 "logging",
                 "vpn_server",
                 "rabbitmq",
                 "two_factor_auth",
+                "algorithm_stores",
             ]
 
             for key in keys:
                 self.assertIn(key, config)
 
     @patch(f"{module_path}.node_configuration_questionaire")
     @patch(f"{module_path}.server_configuration_questionaire")
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/_version.py` & `vantage6-4.4.0rc3/vantage6/cli/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 3, 4, "candidate", __build__, 0)
+version_info = (4, 4, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/algorithm/create.py` & `vantage6-4.4.0rc3/vantage6/cli/algorithm/create.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,10 +38,14 @@
 
     if not directory:
         default_dir = str(Path(os.getcwd()) / name)
         directory = q.text(
             "Directory to put the algorithm in:", default=default_dir
         ).ask()
 
-    run_copy(ALGORITHM_TEMPLATE_REPO, directory, data={"algorithm_name": name})
+    # Create the template. The `unsafe` flag is used to allow running a Python script
+    # after creating the template that cleans up some things.
+    run_copy(
+        ALGORITHM_TEMPLATE_REPO, directory, data={"algorithm_name": name}, unsafe=True
+    )
     info("Template created!")
     info(f"You can find your new algorithm in: {directory}")
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/algostore/attach.py` & `vantage6-4.4.0rc3/vantage6/cli/algostore/attach.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/algostore/files.py` & `vantage6-4.4.0rc3/vantage6/cli/algostore/files.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/algostore/new.py` & `vantage6-4.4.0rc3/vantage6/cli/algostore/new.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/algostore/start.py` & `vantage6-4.4.0rc3/vantage6/cli/algostore/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import click
 
 from vantage6.common import info
 from vantage6.common.globals import APPNAME, DEFAULT_ALGO_STORE_IMAGE, InstanceType
+from vantage6.common.docker.addons import pull_image
 from vantage6.cli.common.start import (
     attach_logs,
     check_for_start,
     get_image,
     mount_config_file,
     mount_database,
     mount_source,
-    pull_image,
 )
 from vantage6.cli.globals import AlgoStoreGlobals
 from vantage6.cli.context.algorithm_store import AlgorithmStoreContext
 from vantage6.cli.common.decorator import click_insert_context
 
 
 @click.command()
@@ -50,14 +50,15 @@
     Start the algorithm store server.
     """
     info("Starting algorithm store...")
     docker_client = check_for_start(ctx, InstanceType.ALGORITHM_STORE)
 
     image = get_image(image, ctx, "algorithm-store", DEFAULT_ALGO_STORE_IMAGE)
 
+    info("Pulling algorithm store image...")
     pull_image(docker_client, image)
 
     config_file = "/mnt/config.yaml"
     mounts = mount_config_file(ctx, config_file)
 
     src_mount = mount_source(mount_src)
     if src_mount:
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/algostore/stop.py` & `vantage6-4.4.0rc3/vantage6/cli/algostore/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/cli.py` & `vantage6-4.4.0rc3/vantage6/cli/cli.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/common/decorator.py` & `vantage6-4.4.0rc3/vantage6/cli/common/decorator.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/common/start.py` & `vantage6-4.4.0rc3/vantage6/cli/common/start.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from docker.models.containers import Container
 from colorama import Fore, Style
 from sqlalchemy.engine.url import make_url
 
 from vantage6.common import error, info, warning
 from vantage6.common.context import AppContext
 from vantage6.common.globals import InstanceType, APPNAME, DEFAULT_DOCKER_REGISTRY
-from vantage6.common.docker.addons import check_docker_running, pull_if_newer
+from vantage6.common.docker.addons import check_docker_running
 from vantage6.cli.context import AlgorithmStoreContext, ServerContext
 from vantage6.cli.common.utils import print_log_worker
 from vantage6.cli.utils import check_config_name_allowed
 from vantage6.cli.globals import ServerGlobals, AlgoStoreGlobals
 
 
 def check_for_start(ctx: AppContext, type_: InstanceType) -> DockerClient:
@@ -24,14 +24,19 @@
 
     Parameters
     ----------
     ctx : AppContext
         The context object
     type_ : InstanceType
         The type of instance to check for
+
+    Returns
+    -------
+    DockerClient
+        A Docker client instance
     """
     # will print an error if not
     check_docker_running()
 
     info("Finding Docker daemon.")
     docker_client = docker.from_env()
 
@@ -79,35 +84,14 @@
         if custom_images:
             image = custom_images.get(custom_image_key)
         if not image:
             image = f"{DEFAULT_DOCKER_REGISTRY}/{default_image}"
     return image
 
 
-def pull_image(docker_client: DockerClient, image: str) -> None:
-    """
-    Pull the image if it is not already available.
-
-    Parameters
-    ----------
-    docker : DockerClient
-        The docker client
-    image : str
-        The image name
-    """
-    info(f"Pulling latest image '{image}'.")
-    try:
-        pull_if_newer(docker_client.from_env(), image)
-    except Exception as e:
-        warning(" ... Getting latest server image failed:")
-        warning(f"     {e}")
-    else:
-        info(" ... success!")
-
-
 def mount_config_file(ctx: AppContext, config_file: str) -> list[docker.types.Mount]:
     """
     Mount the config file in the container.
 
     Parameters
     ----------
     ctx : AppContext
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/common/utils.py` & `vantage6-4.4.0rc3/vantage6/cli/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/configuration_manager.py` & `vantage6-4.4.0rc3/vantage6/cli/configuration_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         # TODO: remove `dict` validation from databases
         "databases": Or([Use(dict)], dict, None),
         "api_path": Use(str),
         "logging": LOGGING_VALIDATORS,
         "encryption": {"enabled": bool, Optional("private_key"): Use(str)},
         Optional("node_extra_env"): dict,
         Optional("node_extra_mounts"): [str],
+        Optional("node_extra_hosts"): dict,
     }
 
 
 class TestConfiguration(Configuration):
     VALIDATORS = {}
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/configuration_wizard.py` & `vantage6-4.4.0rc3/vantage6/cli/configuration_wizard.py`

 * *Files 2% similar despite different names*

```diff
@@ -367,14 +367,36 @@
             "Do you want to run RabbitMQ locally? (Use only for testing)"
         ).ask()
         config["rabbitmq"] = {
             "uri": rabbit_uri,
             "start_with_server": run_rabbit_locally,
         }
 
+    # add algorithm stores to this server
+    is_add_community_store = q.confirm(
+        "Do you want to make the algorithms from the community algorithm store "
+        "available to your users?"
+    ).ask()
+    algorithm_stores = []
+    if is_add_community_store:
+        algorithm_stores.append(
+            {"name": "Community store", "url": "https://store.cotopaxi.vantage6.ai"}
+        )
+    add_more_stores = q.confirm(
+        "Do you want to add more algorithm stores?", default=False
+    ).ask()
+    while add_more_stores:
+        store_name = q.text(message="Enter the name of the store:").ask()
+        store_url = q.text(message="Enter the URL of the store:").ask()
+        algorithm_stores.append({"name": store_name, "url": store_url})
+        add_more_stores = q.confirm(
+            "Do you want to add more algorithm stores?", default=False
+        ).ask()
+    config["algorithm_stores"] = algorithm_stores
+
     return config
 
 
 def algo_store_configuration_questionaire(instance_name: str) -> dict:
     """
     Questionary to generate a config file for the algorithm store server
     instance.
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/context/__init__.py` & `vantage6-4.4.0rc3/vantage6/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/context/algorithm_store.py` & `vantage6-4.4.0rc3/vantage6/cli/context/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/context/base_server.py` & `vantage6-4.4.0rc3/vantage6/cli/context/base_server.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/context/node.py` & `vantage6-4.4.0rc3/vantage6/cli/context/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/context/server.py` & `vantage6-4.4.0rc3/vantage6/cli/context/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/dev/create.py` & `vantage6-4.4.0rc3/vantage6/cli/dev/create.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/dev/remove.py` & `vantage6-4.4.0rc3/vantage6/cli/dev/remove.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/dev/start.py` & `vantage6-4.4.0rc3/vantage6/cli/dev/start.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/dev/stop.py` & `vantage6-4.4.0rc3/vantage6/cli/dev/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/globals.py` & `vantage6-4.4.0rc3/vantage6/cli/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/attach.py` & `vantage6-4.4.0rc3/vantage6/cli/node/attach.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/clean.py` & `vantage6-4.4.0rc3/vantage6/cli/node/clean.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/common/__init__.py` & `vantage6-4.4.0rc3/vantage6/cli/node/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/create_private_key.py` & `vantage6-4.4.0rc3/vantage6/cli/node/create_private_key.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/files.py` & `vantage6-4.4.0rc3/vantage6/cli/node/files.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/list.py` & `vantage6-4.4.0rc3/vantage6/cli/node/list.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/new.py` & `vantage6-4.4.0rc3/vantage6/cli/node/new.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/remove.py` & `vantage6-4.4.0rc3/vantage6/cli/node/remove.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/set_api_key.py` & `vantage6-4.4.0rc3/vantage6/cli/node/set_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/start.py` & `vantage6-4.4.0rc3/vantage6/cli/node/start.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 import click
 import docker
 
 from colorama import Fore, Style
 
 from vantage6.common import warning, error, info, debug, get_database_config
+from vantage6.common.docker.addons import pull_image
 from vantage6.common.globals import (
     APPNAME,
     DEFAULT_DOCKER_REGISTRY,
     DEFAULT_NODE_IMAGE,
     DEFAULT_NODE_IMAGE_WO_TAG,
     InstanceType,
 )
 from vantage6.common.docker.addons import (
-    pull_if_newer,
     remove_container_if_exists,
     check_docker_running,
 )
 
 from vantage6.cli.common.decorator import click_insert_context
 from vantage6.cli.context.node import NodeContext
 from vantage6.cli.common.utils import print_log_worker
@@ -131,25 +131,15 @@
 
         # fail safe, in case no custom image is specified and we can't get the
         # server version
         if not image:
             image = f"{DEFAULT_DOCKER_REGISTRY}/{DEFAULT_NODE_IMAGE}"
 
     info(f"Pulling latest node image '{image}'")
-    try:
-        # docker_client.images.pull(image)
-        pull_if_newer(docker.from_env(), image)
-
-    except Exception as e:
-        warning(" ... Getting latest node image failed:")
-        warning(f"     {e}")
-    else:
-        info(" ... success!")
-
-    info("Creating Docker data volume")
+    pull_image(docker_client, image)
 
     data_volume = docker_client.volumes.create(ctx.docker_volume_name)
     vpn_volume = docker_client.volumes.create(ctx.docker_vpn_volume_name)
     ssh_volume = docker_client.volumes.create(ctx.docker_ssh_volume_name)
     squid_volume = docker_client.volumes.create(ctx.docker_squid_volume_name)
 
     info("Creating file & folder mounts")
@@ -290,14 +280,17 @@
     if env_overwrites:
         error(
             "Cannot overwrite existing node environment variables: " f"{env_overwrites}"
         )
         exit(1)
     env.update(extra_env)
 
+    # Add extra hosts to the environment
+    extra_hosts = ctx.config.get("node_extra_hosts", {})
+
     remove_container_if_exists(
         docker_client=docker_client, name=ctx.docker_container_name
     )
 
     info("Running Docker container")
     container = docker_client.containers.run(
         image,
@@ -309,14 +302,15 @@
             "system": str(system_folders),
             "name": ctx.config_file_name,
         },
         environment=env,
         name=ctx.docker_container_name,
         auto_remove=not keep,
         tty=True,
+        extra_hosts=extra_hosts,
     )
 
     info("Node container was successfully started!")
 
     if attach:
         logs = container.attach(stream=True, logs=True)
         Thread(target=print_log_worker, args=(logs,), daemon=True).start()
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/stop.py` & `vantage6-4.4.0rc3/vantage6/cli/node/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/node/version.py` & `vantage6-4.4.0rc3/vantage6/cli/node/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/rabbitmq/__init__.py` & `vantage6-4.4.0rc3/vantage6/cli/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/rabbitmq/definitions.py` & `vantage6-4.4.0rc3/vantage6/cli/rabbitmq/definitions.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/rabbitmq/queue_manager.py` & `vantage6-4.4.0rc3/vantage6/cli/rabbitmq/queue_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/attach.py` & `vantage6-4.4.0rc3/vantage6/cli/server/attach.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/common/__init__.py` & `vantage6-4.4.0rc3/vantage6/cli/server/common/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/import_.py` & `vantage6-4.4.0rc3/vantage6/cli/server/import_.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import click
 import docker
 from sqlalchemy.engine.url import make_url
 from vantage6.cli.globals import ServerGlobals
 
 from vantage6.common import info, warning
-from vantage6.common.docker.addons import check_docker_running
+from vantage6.common.docker.addons import check_docker_running, pull_image
 from vantage6.common.globals import (
     APPNAME,
     DEFAULT_DOCKER_REGISTRY,
     DEFAULT_SERVER_IMAGE,
     InstanceType,
 )
 from vantage6.cli.context.server import ServerContext
@@ -73,21 +73,15 @@
 
     # pull latest Docker image
     if image is None:
         image = ctx.config.get(
             "image", f"{DEFAULT_DOCKER_REGISTRY}/{DEFAULT_SERVER_IMAGE}"
         )
     info(f"Pulling latest server image '{image}'.")
-    try:
-        docker_client.images.pull(image)
-    except Exception as e:
-        warning(" ... Getting latest node image failed:")
-        warning(f"     {e}")
-    else:
-        info(" ... success!")
+    pull_image(docker_client, image)
 
     info("Creating mounts")
     mounts = [
         docker.types.Mount("/mnt/config.yaml", str(ctx.config_file), type="bind"),
         docker.types.Mount("/mnt/import.yaml", str(file), type="bind"),
     ]
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/new.py` & `vantage6-4.4.0rc3/vantage6/cli/server/new.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/remove.py` & `vantage6-4.4.0rc3/vantage6/cli/server/remove.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/shell.py` & `vantage6-4.4.0rc3/vantage6/cli/server/shell.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/start.py` & `vantage6-4.4.0rc3/vantage6/cli/server/start.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import click
 import docker
 from docker.client import DockerClient
 
 from vantage6.common import info, warning, error
 from vantage6.common.docker.network_manager import NetworkManager
+from vantage6.common.docker.addons import pull_image
 from vantage6.common.globals import (
     APPNAME,
     DEFAULT_SERVER_IMAGE,
     DEFAULT_UI_IMAGE,
     InstanceType,
 )
 
@@ -18,15 +19,14 @@
 from vantage6.cli.common.decorator import click_insert_context
 from vantage6.cli.common.start import (
     attach_logs,
     check_for_start,
     get_image,
     mount_database,
     mount_source,
-    pull_image,
 )
 
 
 @click.command()
 @click.option("--ip", default=None, help="IP address to listen on")
 @click.option("-p", "--port", default=None, type=int, help="Port to listen on")
 @click.option("-i", "--image", default=None, help="Server Docker image to use")
@@ -86,14 +86,15 @@
     docker_client = check_for_start(ctx, InstanceType.SERVER)
 
     image = get_image(image, ctx, "server", DEFAULT_SERVER_IMAGE)
 
     # check that log directory exists - or create it
     ctx.log_dir.mkdir(parents=True, exist_ok=True)
 
+    info("Pulling server image...")
     pull_image(docker_client, image)
 
     info("Creating mounts")
     config_file = "/mnt/config.yaml"
     mounts = [
         docker.types.Mount(config_file, str(ctx.config_file), type="bind"),
         docker.types.Mount("/mnt/log/", str(ctx.log_dir), type="bind"),
```

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/stop.py` & `vantage6-4.4.0rc3/vantage6/cli/server/stop.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/server/version.py` & `vantage6-4.4.0rc3/vantage6/cli/server/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/template/node_config.j2` & `vantage6-4.4.0rc3/vantage6/cli/template/node_config.j2`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/template/server_import_config.j2` & `vantage6-4.4.0rc3/vantage6/cli/template/server_import_config.j2`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/test/common/diagnostic_runner.py` & `vantage6-4.4.0rc3/vantage6/cli/test/common/diagnostic_runner.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/test/feature_tester.py` & `vantage6-4.4.0rc3/vantage6/cli/test/feature_tester.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/test/integration_test.py` & `vantage6-4.4.0rc3/vantage6/cli/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6/cli/utils.py` & `vantage6-4.4.0rc3/vantage6/cli/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-4.3.4rc3/vantage6.egg-info/PKG-INFO` & `vantage6-4.4.0rc3/vantage6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: vantage6 command line interface
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6 Version: 4.3.4rc3 Summary: vantage6
+Metadata-Version: 2.1 Name: vantage6 Version: 4.4.0rc3 Summary: vantage6
 command line interface Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-4.3.4rc3/vantage6.egg-info/SOURCES.txt` & `vantage6-4.4.0rc3/vantage6.egg-info/SOURCES.txt`

 * *Files identical despite different names*

