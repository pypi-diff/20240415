# Comparing `tmp/pancho-1.0.2.tar.gz` & `tmp/pancho-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pancho-1.0.2.tar", max compression
+gzip compressed data, was "pancho-1.0.3.tar", max compression
```

## Comparing `pancho-1.0.2.tar` & `pancho-1.0.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    35149 2023-01-04 14:53:25.782768 pancho-1.0.2/LICENSE
--rw-r--r--   0        0        0      130 2024-04-02 15:23:42.891832 pancho-1.0.2/pancho/__init__.py
--rw-r--r--   0        0        0       36 2023-10-20 11:24:28.509021 pancho-1.0.2/pancho/definition/__init__.py
--rw-r--r--   0        0        0     2565 2024-04-12 13:04:05.932571 pancho-1.0.2/pancho/definition/contracts.py
--rw-r--r--   0        0        0     1520 2024-04-02 15:23:42.892185 pancho-1.0.2/pancho/definition/exceptions.py
--rw-r--r--   0        0        0      122 2024-04-02 15:23:42.892333 pancho-1.0.2/pancho/implementation/__init__.py
--rw-r--r--   0        0        0     1076 2024-04-02 15:23:42.892474 pancho-1.0.2/pancho/implementation/factory.py
--rw-r--r--   0        0        0     5573 2024-04-05 08:07:40.295161 pancho-1.0.2/pancho/implementation/processing.py
--rw-r--r--   0        0        0     7615 2024-04-05 16:44:15.824108 pancho-1.0.2/pancho/implementation/registry.py
--rw-r--r--   0        0        0      289 2024-04-13 13:17:46.721196 pancho-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 pancho-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-04 14:53:25.782768 pancho-1.0.3/LICENSE
+-rw-r--r--   0        0        0       39 2024-04-15 11:57:48.480093 pancho-1.0.3/README.md
+-rw-r--r--   0        0        0      130 2024-04-02 15:23:42.891832 pancho-1.0.3/pancho/__init__.py
+-rw-r--r--   0        0        0       36 2023-10-20 11:24:28.509021 pancho-1.0.3/pancho/definition/__init__.py
+-rw-r--r--   0        0        0     2565 2024-04-12 13:04:05.932571 pancho-1.0.3/pancho/definition/contracts.py
+-rw-r--r--   0        0        0     1520 2024-04-02 15:23:42.892185 pancho-1.0.3/pancho/definition/exceptions.py
+-rw-r--r--   0        0        0      122 2024-04-02 15:23:42.892333 pancho-1.0.3/pancho/implementation/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 15:23:42.892474 pancho-1.0.3/pancho/implementation/factory.py
+-rw-r--r--   0        0        0     5573 2024-04-05 08:07:40.295161 pancho-1.0.3/pancho/implementation/processing.py
+-rw-r--r--   0        0        0     7615 2024-04-05 16:44:15.824108 pancho-1.0.3/pancho/implementation/registry.py
+-rw-r--r--   0        0        0      358 2024-04-15 11:58:50.492711 pancho-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 pancho-1.0.3/PKG-INFO
```

### Comparing `pancho-1.0.2/LICENSE` & `pancho-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pancho-1.0.2/pancho/definition/contracts.py` & `pancho-1.0.3/pancho/definition/contracts.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.2/pancho/definition/exceptions.py` & `pancho-1.0.3/pancho/definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.2/pancho/implementation/factory.py` & `pancho-1.0.3/pancho/implementation/factory.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.2/pancho/implementation/processing.py` & `pancho-1.0.3/pancho/implementation/processing.py`

 * *Files identical despite different names*

### Comparing `pancho-1.0.2/pancho/implementation/registry.py` & `pancho-1.0.3/pancho/implementation/registry.py`

 * *Files identical despite different names*

