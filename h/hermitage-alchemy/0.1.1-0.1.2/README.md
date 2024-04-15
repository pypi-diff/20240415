# Comparing `tmp/hermitage_alchemy-0.1.1.tar.gz` & `tmp/hermitage_alchemy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hermitage_alchemy-0.1.1.tar", max compression
+gzip compressed data, was "hermitage_alchemy-0.1.2.tar", max compression
```

## Comparing `hermitage_alchemy-0.1.1.tar` & `hermitage_alchemy-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2024-01-29 14:07:08.657002 hermitage_alchemy-0.1.1/README.md
--rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.1/hermitage_alchemy/__init__.py
--rw-r--r--   0        0        0    10395 2024-04-13 13:59:52.794872 hermitage_alchemy-0.1.1/hermitage_alchemy/assembling.py
--rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.1.1/hermitage_alchemy/bootstraping.py
--rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.1/hermitage_alchemy/configuration.py
--rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.1/hermitage_alchemy/definition/__init__.py
--rw-r--r--   0        0        0     2762 2024-04-13 13:56:13.202035 hermitage_alchemy-0.1.1/hermitage_alchemy/definition/contracts.py
--rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.1/hermitage_alchemy/definition/exceptions.py
--rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.1/hermitage_alchemy/execution/__init__.py
--rw-r--r--   0        0        0     6217 2024-04-13 13:58:57.410241 hermitage_alchemy-0.1.1/hermitage_alchemy/execution/fetching.py
--rw-r--r--   0        0        0     3929 2024-04-13 13:58:57.403359 hermitage_alchemy-0.1.1/hermitage_alchemy/execution/storing.py
--rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/__init__.py
--rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/generic.py
--rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/total.py
--rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/upsert.py
--rw-r--r--   0        0        0      416 2024-04-13 14:00:48.255293 hermitage_alchemy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      482 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      120 2024-04-15 11:40:18.155284 hermitage_alchemy-0.1.2/README.md
+-rw-r--r--   0        0        0      609 2024-04-02 15:23:42.890138 hermitage_alchemy-0.1.2/hermitage_alchemy/__init__.py
+-rw-r--r--   0        0        0    10395 2024-04-13 13:59:52.794872 hermitage_alchemy-0.1.2/hermitage_alchemy/assembling.py
+-rw-r--r--   0        0        0      826 2024-04-13 14:00:09.650913 hermitage_alchemy-0.1.2/hermitage_alchemy/bootstraping.py
+-rw-r--r--   0        0        0     6903 2024-04-02 15:23:42.890449 hermitage_alchemy-0.1.2/hermitage_alchemy/configuration.py
+-rw-r--r--   0        0        0        0 2024-04-02 15:23:42.890486 hermitage_alchemy-0.1.2/hermitage_alchemy/definition/__init__.py
+-rw-r--r--   0        0        0     2762 2024-04-13 13:56:13.202035 hermitage_alchemy-0.1.2/hermitage_alchemy/definition/contracts.py
+-rw-r--r--   0        0        0      660 2024-04-02 15:23:42.890980 hermitage_alchemy-0.1.2/hermitage_alchemy/definition/exceptions.py
+-rw-r--r--   0        0        0        1 2024-04-02 15:23:42.891065 hermitage_alchemy-0.1.2/hermitage_alchemy/execution/__init__.py
+-rw-r--r--   0        0        0     6217 2024-04-13 13:58:57.410241 hermitage_alchemy-0.1.2/hermitage_alchemy/execution/fetching.py
+-rw-r--r--   0        0        0     3929 2024-04-13 13:58:57.403359 hermitage_alchemy-0.1.2/hermitage_alchemy/execution/storing.py
+-rw-r--r--   0        0        0       97 2024-04-02 15:23:42.891391 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-02 15:23:42.891483 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/generic.py
+-rw-r--r--   0        0        0     1163 2024-04-02 15:23:42.891584 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/total.py
+-rw-r--r--   0        0        0      907 2024-04-11 15:13:54.800420 hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/upsert.py
+-rw-r--r--   0        0        0      416 2024-04-15 11:39:16.867361 hermitage_alchemy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 hermitage_alchemy-0.1.2/PKG-INFO
```

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/__init__.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/assembling.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/assembling.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/bootstraping.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/bootstraping.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/configuration.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/configuration.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/definition/contracts.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/definition/exceptions.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/execution/fetching.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/execution/fetching.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/execution/storing.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/execution/storing.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/total.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/total.py`

 * *Files identical despite different names*

### Comparing `hermitage_alchemy-0.1.1/hermitage_alchemy/plugins/upsert.py` & `hermitage_alchemy-0.1.2/hermitage_alchemy/plugins/upsert.py`

 * *Files identical despite different names*

