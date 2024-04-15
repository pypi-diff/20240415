# Comparing `tmp/vantage6-server-4.3.4rc3.tar.gz` & `tmp/vantage6-server-4.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-server-4.3.4rc3.tar", last modified: Mon Mar 25 11:02:01 2024, max compression
+gzip compressed data, was "vantage6-server-4.4.0rc3.tar", last modified: Mon Apr 15 13:15:20 2024, max compression
```

## Comparing `vantage6-server-4.3.4rc3.tar` & `vantage6-server-4.4.0rc3.tar`

### file list

```diff
@@ -1,95 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.371178 vantage6-server-4.3.4rc3/tests_server/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/tests_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/tests_server/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)   174680 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/tests_server/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.367178 vantage6-server-4.3.4rc3/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.371178 vantage6-server-4.3.4rc3/vantage6/server/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    26798 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.371178 vantage6-server-4.3.4rc3/vantage6/server/_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.371178 vantage6-server-4.3.4rc3/vantage6/server/_data/dev/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/dev/fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/dev/node_a.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/dev/node_b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/dev/server.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/example_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/unittest_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_data/unittest_fixtures.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.371178 vantage6-server-4.3.4rc3/vantage6/server/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/cli/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.371178 vantage6-server-4.3.4rc3/vantage6/server/controller/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/controller/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/default_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/mail_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.375178 vantage6-server-4.3.4rc3/vantage6/server/model/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/algorithm_port.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/authenticatable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.375178 vantage6-server-4.3.4rc3/vantage6/server/model/common/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/node_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/role_rule_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/study.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/task_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/vantage6/server/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30457 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/collaboration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/vantage6/server/resource/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/common/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/common/input_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/common/output_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/common/swagger_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10460 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/node.py
--rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/study.py
--rw-r--r--   0 runner    (1001) docker     (127)    40615 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/vantage6/server/resource/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/ui/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/resource/websocket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-25 11:01:46.000000 vantage6-server-4.3.4rc3/vantage6/server/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 11:02:01.379178 vantage6-server-4.3.4rc3/vantage6_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-03-25 11:02:01.000000 vantage6-server-4.3.4rc3/vantage6_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-25 11:02:01.000000 vantage6-server-4.3.4rc3/vantage6_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 11:02:01.000000 vantage6-server-4.3.4rc3/vantage6_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-25 11:02:01.000000 vantage6-server-4.3.4rc3/vantage6_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-25 11:02:01.000000 vantage6-server-4.3.4rc3/vantage6_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-25 11:02:01.000000 vantage6-server-4.3.4rc3/vantage6_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.287515 vantage6-server-4.4.0rc3/tests_server/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/tests_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/tests_server/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174647 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/tests_server/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.287515 vantage6-server-4.4.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    29881 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/dev/server.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/example_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_fixtures.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/algo_store_communication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.291516 vantage6-server-4.4.0rc3/vantage6/server/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/cli/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.295516 vantage6-server-4.4.0rc3/vantage6/server/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/controller/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/default_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/mail_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.295516 vantage6-server-4.4.0rc3/vantage6/server/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/authenticatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13648 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.295516 vantage6-server-4.4.0rc3/vantage6/server/model/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/node_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/role_rule_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/task_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8841 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18080 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.299516 vantage6-server-4.4.0rc3/vantage6/server/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     7806 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22084 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31301 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/collaboration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.299516 vantage6-server-4.4.0rc3/vantage6/server/resource/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/input_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/output_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/common/swagger_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21884 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15089 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12973 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29127 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23751 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28647 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40748 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14260 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/vantage6/server/resource/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/ui/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30045 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19457 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/resource/websocket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15348 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-15 13:15:06.000000 vantage6-server-4.4.0rc3/vantage6/server/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:15:20.303516 vantage6-server-4.4.0rc3/vantage6_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 13:15:20.000000 vantage6-server-4.4.0rc3/vantage6_server.egg-info/top_level.txt
```

### Comparing `vantage6-server-4.3.4rc3/PKG-INFO` & `vantage6-server-4.4.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.3.4rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.0rc3 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-server-4.3.4rc3/setup.py` & `vantage6-server-4.4.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/tests_server/test_models.py` & `vantage6-server-4.4.0rc3/tests_server/test_models.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/tests_server/test_resources.py` & `vantage6-server-4.4.0rc3/tests_server/test_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -3458,15 +3458,15 @@
         res.save()
 
         headers = self.login_container(collaboration=col, organization=org, task=task)
         results = self.app.get(f"/api/run?task_id={task.id}", headers=headers)
         self.assertEqual(results.status_code, HTTPStatus.OK)
 
     @patch(
-        "vantage6.server.resource.algorithm_store.AlgorithmStores._request_algo_store",
+        "vantage6.server.algo_store_communication.request_algo_store",
         return_value=("success", HTTPStatus.CREATED),
     )
     def test_create_algorithm_store_record(self, _request_algo_store):
         """Test creating an algorithm store record"""
         # initialize resources
         org = Organization()
         col = Collaboration(organizations=[org])
@@ -3644,15 +3644,15 @@
 
         # cleanup
         org.delete()
         col.delete()
         algo_store.delete()
 
     @patch(
-        "vantage6.server.resource.algorithm_store.AlgorithmStore._request_algo_store",
+        "vantage6.server.resource.algorithm_store.request_algo_store",
     )
     def test_delete_algorithm_store(self, request_algo_store):
         """Test deleting algorithm store records"""
         mock_response = MagicMock()
         mock_response.json.return_value = [{"id": "1"}]
         request_algo_store.return_value = (mock_response, HTTPStatus.OK)
```

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/__init__.py` & `vantage6-server-4.4.0rc3/vantage6/server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from gevent import monkey
 
 # This is a workaround for readthedocs
 if not os.environ.get("READTHEDOCS"):
     # flake8: noqa: E402 (ignore import error)
     monkey.patch_all()
 
+# pylint: disable=wrong-import-position, wrong-import-order
 import importlib
 import logging
 import uuid
 import json
 import time
 import datetime as dt
 import traceback
@@ -43,14 +44,15 @@
 from flask_principal import Principal, Identity, identity_changed
 from flask_socketio import SocketIO
 from threading import Thread
 from pathlib import Path
 
 from vantage6.common import logger_name
 from vantage6.common.globals import PING_INTERVAL_SECONDS
+from vantage6.backend.common.globals import HOST_URI_ENV
 from vantage6.server import db
 from vantage6.cli.context.server import ServerContext
 from vantage6.server.model.base import DatabaseSessionManager, Database
 from vantage6.server.resource.common.output_schema import HATEOASModelSchema
 from vantage6.server.permission import RuleNeed, PermissionManager
 from vantage6.server.globals import (
     APPNAME,
@@ -64,15 +66,18 @@
     SERVER_MODULE_NAME,
 )
 from vantage6.server.resource.common.swagger_templates import swagger_template
 from vantage6.server._version import __version__
 from vantage6.server.mail_service import MailService
 from vantage6.server.websockets import DefaultSocketNamespace
 from vantage6.server.default_roles import get_default_roles, DefaultRole
-
+from vantage6.server.algo_store_communication import (
+    post_algorithm_store,
+    get_server_url,
+)
 
 module_name = logger_name(__name__)
 log = logging.getLogger(module_name)
 
 
 class ServerApp:
     """
@@ -131,14 +136,23 @@
         self.permissions = PermissionManager()
 
         # Api - REST JSON-rpc
         self.api = Api(self.app)
         self.configure_api()
         self.load_resources()
 
+        # couple any algoritm stores to the server if defined in config. This should be
+        # done after the resources are loaded to ensure that rules are set up
+        self.couple_algorithm_stores()
+
+        # set environment variable for dev environment
+        host_uri = self.ctx.config.get("dev", {}).get("host_uri")
+        if host_uri:
+            os.environ[HOST_URI_ENV] = host_uri
+
         # set the server version
         self.__version__ = __version__
 
         # set up socket ping/pong
         log.debug("Starting thread to set node status")
         t = Thread(target=self.__node_status_worker, daemon=True)
         t.start()
@@ -707,14 +721,70 @@
                     if node.last_seen < before_wait:
                         node.status = "offline"
                         node.save()
             except Exception:
                 log.exception("Node-status thread had an exception")
                 time.sleep(PING_INTERVAL_SECONDS)
 
+    def couple_algorithm_stores(self) -> None:
+        """Couple algorithm stores to the server.
+
+        Checks if default algorithm stores are defined in the configuration and if so,
+        couples them to the server.
+        """
+        algorithm_stores = self.ctx.config.get("algorithm_stores", [])
+        server_url = get_server_url(self.ctx.config)
+        if algorithm_stores and not server_url:
+            log.warning(
+                "Algorithm stores are defined in the configuration, but the server "
+                "url is not. Skipping coupling of algorithm stores."
+            )
+            return
+        if algorithm_stores:
+            # TODO in the future it may change that not just any algorithm store can
+            # be added to this server - in that case show a useful error below
+            # (automated coupling is not possible for such cases I think?)
+
+            # couple the stores
+            for store in algorithm_stores:
+                if not (name := store.get("name")):
+                    log.warning("Algorithm store has no name, skipping coupling")
+                    continue
+                elif not (url := store.get("url")):
+                    log.warning(
+                        "Algorithm store %s has no url, skipping coupling", name
+                    )
+                    continue
+                store = db.AlgorithmStore.get_by_url(url)
+                if not store:
+                    response, status = post_algorithm_store(
+                        {
+                            "name": name,
+                            "algorithm_store_url": url,
+                            "server_url": server_url,
+                            "force": True,
+                        },
+                        self.ctx.config,
+                    )
+                    if status == HTTPStatus.CREATED:
+                        log.info(
+                            "Algorithm store '%s' at %s has been coupled to the server",
+                            name,
+                            url,
+                        )
+                    else:
+                        log.error(
+                            "Failed to couple algorithm store '%s' at %s to the server:"
+                            " %s",
+                            name,
+                            url,
+                            response["msg"],
+                        )
+                # else: store already exists, no need to couple it again
+
 
 def run_server(config: str, system_folders: bool = True) -> ServerApp:
     """
     Run a vantage6 server.
 
     Parameters
     ----------
```

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/dev/fixtures.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/dev/node_a.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_a.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/dev/node_b.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/node_b.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/dev/server.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/dev/server.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/example_fixtures.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/example_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/unittest_config.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_config.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_data/unittest_fixtures.yaml` & `vantage6-server-4.4.0rc3/vantage6/server/_data/unittest_fixtures.yaml`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/_version.py` & `vantage6-server-4.4.0rc3/vantage6/server/_version.py`

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

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/cli/server.py` & `vantage6-server-4.4.0rc3/vantage6/server/cli/server.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/context.py` & `vantage6-server-4.4.0rc3/vantage6/server/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/controller/fixture.py` & `vantage6-server-4.4.0rc3/vantage6/server/controller/fixture.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/db.py` & `vantage6-server-4.4.0rc3/vantage6/server/db.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/default_roles.py` & `vantage6-server-4.4.0rc3/vantage6/server/default_roles.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/globals.py` & `vantage6-server-4.4.0rc3/vantage6/server/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/mail_service.py` & `vantage6-server-4.4.0rc3/vantage6/server/mail_service.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/__init__.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/algorithm_port.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/algorithm_store.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/authenticatable.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/authenticatable.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/base.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/base.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/collaboration.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/common/utils.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/common/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/member.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/member.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/node.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/node_config.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/node_config.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/organization.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/permission.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/role.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/rule.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/run.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/study.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/task.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/task.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/task_database.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/task_database.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/model/user.py` & `vantage6-server-4.4.0rc3/vantage6/server/model/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/permission.py` & `vantage6-server-4.4.0rc3/vantage6/server/permission.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/__init__.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/algorithm_store.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/algorithm_store.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 import logging
 
-import requests
-from flask import Response, request, g
-from flask_restful import Api
 from http import HTTPStatus
+from flask import request, g
+from flask_restful import Api
 from sqlalchemy import or_
 
 from vantage6.server import db
 from vantage6.backend.common.resource.pagination import Pagination
 from vantage6.server.resource.common.input_schema import AlgorithmStoreInputSchema
 from vantage6.server.permission import RuleCollection, Operation as P
 from vantage6.server.resource.common.output_schema import AlgorithmStoreSchema
 from vantage6.server.resource import with_user, ServicesResources
+from vantage6.server.algo_store_communication import (
+    post_algorithm_store,
+    get_server_url,
+    request_algo_store,
+)
 
 
 module_name = __name__.split(".")[-1]
 log = logging.getLogger(module_name)
 
 
 def setup(api: Api, api_base: str, services: dict) -> None:
@@ -60,183 +64,28 @@
 class AlgorithmStoreBase(ServicesResources):
     """Base class for algorithm store resources."""
 
     def __init__(self, socketio, mail, api, permissions, config):
         super().__init__(socketio, mail, api, permissions, config)
         self.r_col: RuleCollection = getattr(self.permissions, "collaboration")
 
-    def _request_algo_store(
-        self,
-        algo_store_url: str,
-        server_url: str,
-        endpoint: str,
-        method: str,
-        force: bool = False,
-    ) -> tuple[dict | Response, HTTPStatus]:
-        """
-        Whitelist this vantage6 server url for the algorithm store.
-
-        Parameters
-        ----------
-        algo_store_url : str
-            URL to the algorithm store
-        server_url : str
-            URL to this vantage6 server. This is used to whitelist this server
-            at the algorithm store.
-        endpoint : str
-            Endpoint to use at the algorithm store.
-        method : str
-            HTTP method to use.
-        force : bool
-            If True, the algorithm store will be added even if the algorithm
-            store url is insecure (i.e. localhost)
-
-        Returns
-        -------
-        tuple[dict | Response, HTTPStatus]
-            The response of the algorithm store and the HTTP status. If the
-            algorithm store is not reachable, a dict with an error message is
-            returned instead of the response.
-        """
-        # TODO this is not pretty, but it works for now. This should change
-        # when we have a separate auth service
-        is_localhost_algo_store = self._contains_localhost(algo_store_url)
-        try:
-            response = self._execute_algo_store_request(
-                algo_store_url, server_url, endpoint, method, force
-            )
-        except requests.exceptions.ConnectionError as exc:
-            if not is_localhost_algo_store:
-                log.warning("Request to algorithm store failed")
-                log.exception(exc)
-            response = None
-
-        if not response and is_localhost_algo_store:
-            # try again with the docker host ip
-            algo_store_url = algo_store_url.replace(
-                "localhost", "host.docker.internal"
-            ).replace("127.0.0.1", "host.docker.internal")
-            try:
-                response = self._execute_algo_store_request(
-                    algo_store_url, server_url, endpoint, method, force
-                )
-            except requests.exceptions.ConnectionError as exc:
-                log.warning("Request to algorithm store failed")
-                log.exception(exc)
-                response = None
-
-        if response is None:
-            return {
-                "msg": "Algorithm store cannot be reached. Make sure that "
-                "it is online and that you have not included /api at the "
-                "end of the algorithm store URL"
-            }, HTTPStatus.BAD_REQUEST
-        elif response.status_code not in [HTTPStatus.CREATED, HTTPStatus.OK]:
-            try:
-                msg = (
-                    f"Algorithm store error: {response.json()['msg']}, HTTP status: "
-                    f"{response.status_code}"
-                )
-            except KeyError:
-                msg = (
-                    "Communication to algorithm store failed. HTTP status: "
-                    f"{response.status_code}"
-                )
-            return {"msg": msg}, HTTPStatus.BAD_REQUEST
-        # else: server has been registered at algorithm store, proceed
-        return response, response.status_code
-
-    @staticmethod
-    def _contains_localhost(url: str) -> bool:
-        """Check if the url refers to localhost address"""
-        return url.startswith("http://localhost") or url.startswith("http://127.0.0.1")
-
-    # TODO this function and above should be moved to some kind of client lib
     @staticmethod
-    def _execute_algo_store_request(
-        algo_store_url: str, server_url: str, endpoint: str, method: str, force: bool
-    ) -> requests.Response:
+    def get_authorization_headers_from_request() -> dict:
         """
-        Send a request to the algorithm store to whitelist this vantage6 server
-        url for the algorithm store.
-
-        Parameters
-        ----------
-        algo_store_url : str
-            URL to the algorithm store
-        server_url : str
-            URL to this vantage6 server. This is used to whitelist this server
-            at the algorithm store.
-        endpoint : str
-            Endpoint to use at the algorithm store.
-        method : str
-            HTTP method to use. Choose "post" for adding the server url and
-            "delete" for removing it.
-        force : bool
-            If True, the algorithm store will be added even if the algorithm
-            store url is insecure (i.e. localhost)
+        Get the authorization headers from the request.
 
         Returns
         -------
-        requests.Response | None
-            Response from the algorithm store. If the algorithm store is not
-            reachable, None is returned
+        dict
+            The authorization headers
         """
-        if server_url.endswith("/"):
-            server_url = server_url[:-1]
-        if algo_store_url.endswith("/"):
-            algo_store_url = algo_store_url[:-1]
-
-        param_dict = {"url": server_url}
-        if force:
-            param_dict["force"] = True
-
-        # set headers
-        headers = {"server_url": server_url}
         current_headers = request.headers
         if "Authorization" in current_headers:
-            headers["Authorization"] = current_headers["Authorization"]
-
-        params = None
-        json = None
-        if method == "get":
-            request_function = requests.get
-            params = param_dict
-        elif method == "post":
-            request_function = requests.post
-            json = param_dict
-        elif method == "delete":
-            request_function = requests.delete
-            params = param_dict
-        else:
-            raise ValueError(f"Method {method} not supported")
-
-        return request_function(
-            f"{algo_store_url}/api/{endpoint}",
-            params=params,
-            json=json,
-            headers=headers,
-        )
-
-    def _get_server_url(self, server_url_from_request: str | None) -> str:
-        """ "
-        Get the server url from the server configuration, or from the request
-        data if it is not present in the configuration.
-
-        Parameters
-        ----------
-        server_url_from_request : str | None
-            Server url from the request data.
-
-        Returns
-        -------
-        str | None
-            The server url
-        """
-        return self.config.get("server_url", server_url_from_request)
+            return {"Authorization": current_headers["Authorization"]}
+        return {}
 
 
 class AlgorithmStores(AlgorithmStoreBase):
     """Resource for /algorithm"""
 
     @with_user
     def get(self):
@@ -452,83 +301,22 @@
                 "for all collaborations!"
             }, HTTPStatus.UNAUTHORIZED
         elif not self.r_col.can_for_col(P.EDIT, collaboration_id):
             return {
                 "msg": "You lack the permission to do that!"
             }, HTTPStatus.UNAUTHORIZED
 
-        # check if algorithm store is already available for the collaboration
-        algorithm_store_url = data["algorithm_store_url"]
-        if algorithm_store_url.endswith("/"):
-            algorithm_store_url = algorithm_store_url[:-1]
-        existing_algorithm_stores = db.AlgorithmStore.get_by_url(algorithm_store_url)
-        records_to_delete = []
-        if existing_algorithm_stores:
-            collabs_with_algo_store = [
-                a.collaboration_id for a in existing_algorithm_stores
-            ]
-            if None in collabs_with_algo_store:
-                return {
-                    "msg": "Algorithm store is already available for all "
-                    "collaborations"
-                }, HTTPStatus.BAD_REQUEST
-            if collaboration_id in collabs_with_algo_store:
-                return {
-                    "msg": "Algorithm store is already available for this "
-                    "collaboration"
-                }, HTTPStatus.BAD_REQUEST
-            if not collaboration_id:
-                # algorithm store is currently available for some
-                # collaborations, but now it will be available for all of them.
-                # Remove the records that only make it available to some
-                # collaborations (this prevents duplicates)
-                records_to_delete = existing_algorithm_stores
-
-        # raise a warning if the algorithm store url is insecure (i.e.
-        # localhost)
-        force = data.get("force", False)
-        if not force and (
-            "localhost" in algorithm_store_url or "127.0.0.1" in algorithm_store_url
-        ):
-            return {
-                "msg": "Algorithm store url is insecure: localhost services "
-                "may be run on any computer. Add it anyway by setting the "
-                "'force' flag to true, but only do so for development servers!"
-            }, HTTPStatus.BAD_REQUEST
-
-        server_url = self._get_server_url(data.get("server_url"))
-        if not server_url:
-            return {
-                "msg": "The 'server_url' key is required in the server "
-                "configuration, or as a parameter. Please add it or ask your "
-                "server administrator to specify it in the server configuration."
-            }, HTTPStatus.BAD_REQUEST
-
-        # whitelist this vantage6 server url for the algorithm store
-        response, status = self._request_algo_store(
-            algorithm_store_url,
-            server_url,
-            endpoint="vantage6-server",
-            method="post",
-            force=force,
+        response, status = post_algorithm_store(
+            request.get_json(),
+            self.config,
         )
         if status != HTTPStatus.CREATED:
             return response, status
-
-        # delete and create records
-        for record in records_to_delete:
-            record.delete()
-        algorithm_store = db.AlgorithmStore(
-            name=data["name"],
-            url=algorithm_store_url,
-            collaboration_id=collaboration_id,
-        )
-        algorithm_store.save()
-
-        return algorithm_store_schema.dump(algorithm_store), HTTPStatus.CREATED
+        else:
+            return algorithm_store_schema.dump(response), status
 
 
 class AlgorithmStore(AlgorithmStoreBase):
     """Resource for /algorithm/<id>"""
 
     @with_user
     def get(self, id):
@@ -775,25 +563,26 @@
 
         # Delete the whitelisting of this server at the algorithm store.
         # First check if algostore is not used by other collaborations
         other_algorithm_stores = db.AlgorithmStore.get_by_url(algorithm_store.url)
         if len(other_algorithm_stores) == 1:
             # only this algorithm store uses this url, so delete the
             # whitelisting
-            server_url = self._get_server_url(request.args.get("server_url"))
+            server_url = get_server_url(self.config, request.args.get("server_url"))
             if not server_url:
                 return {
                     "msg": "The 'server_url' query parameter is required"
                 }, HTTPStatus.BAD_REQUEST
             # get the ID of the whitelisted server, then delete it
-            response, status = self._request_algo_store(
+            response, status = request_algo_store(
                 algorithm_store.url,
                 server_url,
                 endpoint="vantage6-server",
                 method="get",
+                headers=self.get_authorization_headers_from_request(),
             )
             if status != HTTPStatus.OK:
                 return response, status
             result = response.json()
             if len(result) > 1:
                 msg = (
                     "More than one whitelisted server found with url "
@@ -806,19 +595,20 @@
                     "No whitelisted server found with url "
                     f"{server_url}. This should not happen!"
                 )
                 log.warning(msg)
             # remove all linked servers with the given url
             for server in result:
                 server_id = server["id"]
-                response, status = self._request_algo_store(
+                response, status = request_algo_store(
                     algorithm_store.url,
                     server_url,
                     endpoint=f"vantage6-server/{server_id}",
                     method="delete",
+                    headers=self.get_authorization_headers_from_request(),
                 )
             if status != HTTPStatus.OK:
                 return response, status
 
         # finally delete the algorithm store record itself
         algorithm_store.delete()
         return {"msg": f"Algorithm store id={id} successfully deleted"}, HTTPStatus.OK
```

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/collaboration.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/collaboration.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/common/auth_helper.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/common/auth_helper.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/common/input_schema.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/common/input_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/common/output_schema.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/common/output_schema.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/common/swagger_templates.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/common/swagger_templates.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/event.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,16 @@
         namespace="/tasks",
         room=f"collaboration_{task.collaboration_id}",
     )
 
     # set tasks and subtasks status to killed
     def set_killed(task: db.Task):
         for run in task.runs:
+            if has_task_finished(run.status):
+                continue  # don't overwrite status if run is already finished
             run.status = TaskStatus.KILLED
             run.finished_at = dt.datetime.now()
             run.save()
 
     set_killed(task)
     for subtask in task.children:
         set_killed(subtask)
```

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/health.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/health.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/node.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/organization.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/organization.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/port.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/port.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/recover.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/recover.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/role.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/role.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/rule.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/run.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/run.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/stats.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/stats.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/study.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/task.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,14 +547,18 @@
         """
         Create new task and algorithm runs. Send the task to the nodes.
 
         Parameters
         ----------
         data : dict
             Task data
+        socketio : SocketIO
+            SocketIO server instance
+        rules : RuleCollection
+            Rule collection instance
         """
         # validate request body
         errors = task_input_schema.validate(data)
         if errors:
             return {
                 "msg": "Request body is incorrect",
                 "errors": errors,
```

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/token.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/token.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/ui/column.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/ui/column.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/user.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/user.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/version.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/version.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/vpn.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/vpn.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/resource/websocket_test.py` & `vantage6-server-4.4.0rc3/vantage6/server/resource/websocket_test.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/utils.py` & `vantage6-server-4.4.0rc3/vantage6/server/utils.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6/server/websockets.py` & `vantage6-server-4.4.0rc3/vantage6/server/websockets.py`

 * *Files identical despite different names*

### Comparing `vantage6-server-4.3.4rc3/vantage6_server.egg-info/PKG-INFO` & `vantage6-server-4.4.0rc3/vantage6_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-server
-Version: 4.3.4rc3
+Version: 4.4.0rc3
 Summary: Vantage6 server
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-server Version: 4.3.4rc3 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-server Version: 4.4.0rc3 Summary: Vantage6
 server Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-server-4.3.4rc3/vantage6_server.egg-info/SOURCES.txt` & `vantage6-server-4.4.0rc3/vantage6_server.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 setup.py
 tests_server/__init__.py
 tests_server/test_models.py
 tests_server/test_resources.py
 vantage6/server/__build__
 vantage6/server/__init__.py
 vantage6/server/_version.py
+vantage6/server/algo_store_communication.py
 vantage6/server/context.py
 vantage6/server/db.py
 vantage6/server/default_roles.py
 vantage6/server/exceptions.py
 vantage6/server/globals.py
 vantage6/server/mail_service.py
 vantage6/server/permission.py
```

