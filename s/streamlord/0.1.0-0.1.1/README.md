# Comparing `tmp/streamlord-0.1.0.tar.gz` & `tmp/streamlord-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlord-0.1.0.tar", max compression
+gzip compressed data, was "streamlord-0.1.1.tar", max compression
```

## Comparing `streamlord-0.1.0.tar` & `streamlord-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       17 2024-04-13 13:40:05.904405 streamlord-0.1.0/README.md
--rw-r--r--   0        0        0      305 2024-04-13 14:04:09.776804 streamlord-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       81 2024-04-02 15:23:42.893017 streamlord-0.1.0/streamlord/__init__.py
--rw-r--r--   0        0        0       30 2024-04-02 15:23:42.893115 streamlord-0.1.0/streamlord/collectors/__init__.py
--rw-r--r--   0        0        0      144 2024-04-02 15:23:42.893228 streamlord-0.1.0/streamlord/collectors/navigation.py
--rw-r--r--   0        0        0       24 2024-04-02 15:23:42.893330 streamlord-0.1.0/streamlord/definitions/__init__.py
--rw-r--r--   0        0        0       90 2024-04-02 15:23:42.893418 streamlord-0.1.0/streamlord/definitions/contracts.py
--rw-r--r--   0        0        0      152 2024-04-02 15:23:42.893517 streamlord-0.1.0/streamlord/mappers/__init__.py
--rw-r--r--   0        0        0      832 2024-04-02 15:23:42.893612 streamlord-0.1.0/streamlord/mappers/destroyer.py
--rw-r--r--   0        0        0      729 2024-04-02 15:23:42.893704 streamlord-0.1.0/streamlord/mappers/digger.py
--rw-r--r--   0        0        0     1289 2024-04-02 15:23:42.893800 streamlord-0.1.0/streamlord/mappers/injector.py
--rw-r--r--   0        0        0     1622 2024-04-02 15:23:42.893901 streamlord-0.1.0/streamlord/mappers/squeezer.py
--rw-r--r--   0        0        0     1318 2024-04-05 08:07:40.295775 streamlord-0.1.0/streamlord/mappers/stamper.py
--rw-r--r--   0        0        0      809 2024-04-02 15:23:42.894091 streamlord-0.1.0/streamlord/pipeline.py
--rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 streamlord-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       59 2024-04-15 11:50:57.981205 streamlord-0.1.1/README.md
+-rw-r--r--   0        0        0      357 2024-04-15 11:51:23.283987 streamlord-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-04-02 15:23:42.893017 streamlord-0.1.1/streamlord/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-02 15:23:42.893115 streamlord-0.1.1/streamlord/collectors/__init__.py
+-rw-r--r--   0        0        0      144 2024-04-02 15:23:42.893228 streamlord-0.1.1/streamlord/collectors/navigation.py
+-rw-r--r--   0        0        0       24 2024-04-02 15:23:42.893330 streamlord-0.1.1/streamlord/definitions/__init__.py
+-rw-r--r--   0        0        0       90 2024-04-02 15:23:42.893418 streamlord-0.1.1/streamlord/definitions/contracts.py
+-rw-r--r--   0        0        0      152 2024-04-02 15:23:42.893517 streamlord-0.1.1/streamlord/mappers/__init__.py
+-rw-r--r--   0        0        0      832 2024-04-02 15:23:42.893612 streamlord-0.1.1/streamlord/mappers/destroyer.py
+-rw-r--r--   0        0        0      729 2024-04-02 15:23:42.893704 streamlord-0.1.1/streamlord/mappers/digger.py
+-rw-r--r--   0        0        0     1289 2024-04-02 15:23:42.893800 streamlord-0.1.1/streamlord/mappers/injector.py
+-rw-r--r--   0        0        0     1622 2024-04-02 15:23:42.893901 streamlord-0.1.1/streamlord/mappers/squeezer.py
+-rw-r--r--   0        0        0     1318 2024-04-05 08:07:40.295775 streamlord-0.1.1/streamlord/mappers/stamper.py
+-rw-r--r--   0        0        0      809 2024-04-02 15:23:42.894091 streamlord-0.1.1/streamlord/pipeline.py
+-rw-r--r--   0        0        0      547 1970-01-01 00:00:00.000000 streamlord-0.1.1/PKG-INFO
```

### Comparing `streamlord-0.1.0/streamlord/mappers/destroyer.py` & `streamlord-0.1.1/streamlord/mappers/destroyer.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.1.0/streamlord/mappers/digger.py` & `streamlord-0.1.1/streamlord/mappers/digger.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.1.0/streamlord/mappers/injector.py` & `streamlord-0.1.1/streamlord/mappers/injector.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.1.0/streamlord/mappers/squeezer.py` & `streamlord-0.1.1/streamlord/mappers/squeezer.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.1.0/streamlord/mappers/stamper.py` & `streamlord-0.1.1/streamlord/mappers/stamper.py`

 * *Files identical despite different names*

### Comparing `streamlord-0.1.0/streamlord/pipeline.py` & `streamlord-0.1.1/streamlord/pipeline.py`

 * *Files identical despite different names*

