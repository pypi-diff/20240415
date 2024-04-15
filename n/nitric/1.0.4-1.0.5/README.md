# Comparing `tmp/nitric-1.0.4.tar.gz` & `tmp/nitric-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitric-1.0.4.tar", last modified: Fri Apr 12 03:52:40 2024, max compression
+gzip compressed data, was "nitric-1.0.5.tar", last modified: Mon Apr 15 05:53:09 2024, max compression
```

## Comparing `nitric-1.0.4.tar` & `nitric-1.0.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-12 03:52:40.776903 nitric-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-12 03:52:02.000000 nitric-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/bidi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/KeyValue/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/KeyValue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/KeyValue/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/KeyValue/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/apis/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/apis/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric/proto/deployments/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/deployments/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/http/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/http/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/http/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/kvstore/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/kvstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/kvstore/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/kvstore/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/queues/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/queues/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/queues/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/resources/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/schedules/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/schedules/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/secrets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/secrets/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/storage/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/topics/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/topics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/topics/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/topics/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/websockets/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/websockets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/proto/websockets/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/proto/websockets/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:02.000000 nitric-1.0.4/nitric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.776903 nitric-1.0.4/nitric/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/kv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/queues.py
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/topics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/resources/websockets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-12 03:52:36.000000 nitric-1.0.4/nitric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 03:52:40.772903 nitric-1.0.4/nitric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 03:52:40.000000 nitric-1.0.4/nitric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 03:52:02.000000 nitric-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 03:52:40.776903 nitric-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-12 03:52:02.000000 nitric-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.087648 nitric-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-15 05:53:09.087648 nitric-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-15 05:52:28.000000 nitric-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.079649 nitric-1.0.5/nitric/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/bidi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.079649 nitric-1.0.5/nitric/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12018 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/KeyValue/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/KeyValue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/KeyValue/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/KeyValue/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/apis/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/apis/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/deployments/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    14719 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/deployments/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/http/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/http/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/http/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/kvstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/kvstore/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/kvstore/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/queues/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/queues/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7708 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/queues/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/resources/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/schedules/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/schedules/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/secrets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5425 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/secrets/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16834 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/storage/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/topics/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/topics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/topics/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/topics/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/websockets/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/websockets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.083649 nitric-1.0.5/nitric/proto/websockets/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/proto/websockets/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 05:52:28.000000 nitric-1.0.5/nitric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.087648 nitric-1.0.5/nitric/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/kv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7866 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7737 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/topics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9451 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/resources/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-15 05:53:04.000000 nitric-1.0.5/nitric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 05:53:09.079649 nitric-1.0.5/nitric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-04-15 05:53:09.000000 nitric-1.0.5/nitric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-15 05:53:09.000000 nitric-1.0.5/nitric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 05:53:09.000000 nitric-1.0.5/nitric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-15 05:53:09.000000 nitric-1.0.5/nitric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 05:53:09.000000 nitric-1.0.5/nitric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 05:52:28.000000 nitric-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 05:53:09.087648 nitric-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-15 05:52:28.000000 nitric-1.0.5/setup.py
```

### Comparing `nitric-1.0.4/PKG-INFO` & `nitric-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.4
+Version: 1.0.5
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.4 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.5 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.4/README.md` & `nitric-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/__init__.py` & `nitric-1.0.5/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/application.py` & `nitric-1.0.5/nitric/application.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/bidi.py` & `nitric-1.0.5/nitric/bidi.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/config/__init__.py` & `nitric-1.0.5/nitric/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/context.py` & `nitric-1.0.5/nitric/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 from opentelemetry import propagate
 
 from nitric.proto.schedules.v1 import ServerMessage as ScheduleServerMessage
 from nitric.proto.topics.v1 import ClientMessage as TopicClientMessage
 from nitric.proto.topics.v1 import MessageResponse as TopicResponse
 from nitric.proto.topics.v1 import ServerMessage as TopicServerMessage
+from nitric.utils import dict_from_struct
 
 Record = Dict[str, Union[str, List[str]]]
 PROPAGATOR = propagate.get_global_textmap()
 
 
 class HttpMethod(Enum):
     """Valid query expression operators."""
@@ -169,15 +170,15 @@
         self.res = response if response else MessageResponse()
 
     @staticmethod
     def _from_request(msg: TopicServerMessage) -> MessageContext:
         """Construct a new EventContext from a Topic trigger from the Nitric Membrane."""
         return MessageContext(
             request=MessageRequest(
-                data=msg.message_request.message.struct_payload.to_dict(),
+                data=dict_from_struct(msg.message_request.message.struct_payload),
                 topic=msg.message_request.topic_name,
             )
         )
 
     def to_response(self) -> TopicClientMessage:
         """Construct a EventContext for the Nitric Membrane from this context object."""
         return TopicClientMessage(message_response=TopicResponse(success=self.res.success))
```

### Comparing `nitric-1.0.4/nitric/exception.py` & `nitric-1.0.5/nitric/exception.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/KeyValue/__init__.py` & `nitric-1.0.5/nitric/proto/KeyValue/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/KeyValue/v1/__init__.py` & `nitric-1.0.5/nitric/proto/KeyValue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/__init__.py` & `nitric-1.0.5/nitric/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/apis/__init__.py` & `nitric-1.0.5/nitric/proto/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/apis/v1/__init__.py` & `nitric-1.0.5/nitric/proto/apis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/deployments/__init__.py` & `nitric-1.0.5/nitric/proto/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/deployments/v1/__init__.py` & `nitric-1.0.5/nitric/proto/deployments/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/http/__init__.py` & `nitric-1.0.5/nitric/proto/http/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/http/v1/__init__.py` & `nitric-1.0.5/nitric/proto/http/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/kvstore/__init__.py` & `nitric-1.0.5/nitric/proto/kvstore/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/kvstore/v1/__init__.py` & `nitric-1.0.5/nitric/proto/kvstore/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/queues/__init__.py` & `nitric-1.0.5/nitric/proto/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/queues/v1/__init__.py` & `nitric-1.0.5/nitric/proto/queues/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/resources/__init__.py` & `nitric-1.0.5/nitric/proto/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/resources/v1/__init__.py` & `nitric-1.0.5/nitric/proto/resources/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/schedules/__init__.py` & `nitric-1.0.5/nitric/proto/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/schedules/v1/__init__.py` & `nitric-1.0.5/nitric/proto/schedules/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/secrets/__init__.py` & `nitric-1.0.5/nitric/proto/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/secrets/v1/__init__.py` & `nitric-1.0.5/nitric/proto/secrets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/storage/__init__.py` & `nitric-1.0.5/nitric/proto/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/storage/v1/__init__.py` & `nitric-1.0.5/nitric/proto/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/topics/__init__.py` & `nitric-1.0.5/nitric/proto/topics/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/topics/v1/__init__.py` & `nitric-1.0.5/nitric/proto/topics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/websockets/__init__.py` & `nitric-1.0.5/nitric/proto/websockets/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/proto/websockets/v1/__init__.py` & `nitric-1.0.5/nitric/proto/websockets/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/__init__.py` & `nitric-1.0.5/nitric/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/apis.py` & `nitric-1.0.5/nitric/resources/apis.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/buckets.py` & `nitric-1.0.5/nitric/resources/buckets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/kv.py` & `nitric-1.0.5/nitric/resources/kv.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/queues.py` & `nitric-1.0.5/nitric/resources/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/resource.py` & `nitric-1.0.5/nitric/resources/resource.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/schedules.py` & `nitric-1.0.5/nitric/resources/schedules.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/secrets.py` & `nitric-1.0.5/nitric/resources/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/resources/topics.py` & `nitric-1.0.5/nitric/resources/topics.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from nitric.proto.resources.v1 import Action, ResourceDeclareRequest, ResourceIdentifier, ResourceType
 from nitric.proto.topics.v1 import ClientMessage, TopicMessage
 from nitric.proto.topics.v1 import MessageRequest as ProtoMessageRequest
 from nitric.proto.topics.v1 import MessageResponse as ProtoMessageResponse
 from nitric.proto.topics.v1 import RegistrationRequest, SubscriberStub
 from nitric.proto.topics.v1 import TopicPublishRequest, TopicsStub
 from nitric.resources.resource import SecureResource
-from nitric.utils import new_default_channel, struct_from_dict
+from nitric.utils import dict_from_struct, new_default_channel, struct_from_dict
 
 TopicPermission = Literal["publish"]
 
 
 class TopicRef:
     """A reference to a deployed topic, used to interact with the topic at runtime."""
 
@@ -127,15 +127,15 @@
 
         return decorator
 
 
 def _message_context_from_proto(msg: ProtoMessageRequest) -> MessageContext:
     return MessageContext(
         request=MessageRequest(
-            data=msg.message.struct_payload.to_dict(),
+            data=dict_from_struct(msg.message.struct_payload),
             topic=msg.topic_name,
         )
     )
 
 
 class Subscriber(FunctionServer):
     """A handler for topic messages."""
```

### Comparing `nitric-1.0.4/nitric/resources/websockets.py` & `nitric-1.0.5/nitric/resources/websockets.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric/utils.py` & `nitric-1.0.5/nitric/utils.py`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/nitric.egg-info/PKG-INFO` & `nitric-1.0.5/nitric.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 1.0.4
+Version: 1.0.5
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 1.0.4 Summary: The Nitric SDK for
+Metadata-Version: 2.1 Name: nitric Version: 1.0.5 Summary: The Nitric SDK for
 Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent Requires-Python: >=3.11
 Description-Content-Type: text/markdown Provides-Extra: dev
                                  _[_N_i_t_r_i_c_ _L_o_g_o_]
                ********** BBuuiilldd _nn_ii_tt_rr_ii_cc aapppplliiccaattiioonnss wwiitthh PPyytthhoonn **********
            _[_B_u_i_l_d_ _S_t_a_t_u_s_]_[_C_o_d_e_c_o_v_]_[_V_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_/_w_e_e_k_]_[_D_i_s_c_o_r_d_]
```

### Comparing `nitric-1.0.4/nitric.egg-info/SOURCES.txt` & `nitric-1.0.5/nitric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitric-1.0.4/setup.py` & `nitric-1.0.5/setup.py`

 * *Files identical despite different names*

