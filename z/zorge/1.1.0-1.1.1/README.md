# Comparing `tmp/zorge-1.1.0.tar.gz` & `tmp/zorge-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zorge-1.1.0.tar", max compression
+gzip compressed data, was "zorge-1.1.1.tar", max compression
```

## Comparing `zorge-1.1.0.tar` & `zorge-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    35149 2023-01-04 14:56:28.854602 zorge-1.1.0/LICENSE
--rw-r--r--   0        0        0      286 2024-04-13 14:07:59.244876 zorge-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-02-19 15:31:10.223460 zorge-1.1.0/zorge/.DS_Store
--rw-r--r--   0        0        0      130 2024-04-11 07:57:07.720615 zorge-1.1.0/zorge/__init__.py
--rw-r--r--   0        0        0      188 2024-04-11 07:57:07.720731 zorge-1.1.0/zorge/contracts/__init__.py
--rw-r--r--   0        0        0      534 2024-04-11 07:57:07.720842 zorge-1.1.0/zorge/contracts/domain.py
--rw-r--r--   0        0        0     1309 2024-04-11 07:57:07.720917 zorge-1.1.0/zorge/contracts/internal.py
--rw-r--r--   0        0        0       87 2024-04-11 07:57:07.720992 zorge-1.1.0/zorge/exceptions/__init__.py
--rw-r--r--   0        0        0      494 2024-04-11 07:57:07.721065 zorge-1.1.0/zorge/exceptions/di.py
--rw-r--r--   0        0        0        1 2024-04-11 07:57:07.721285 zorge-1.1.0/zorge/implementation/__init__.py
--rw-r--r--   0        0        0     6888 2024-04-11 07:57:07.721589 zorge-1.1.0/zorge/implementation/container.py
--rw-r--r--   0        0        0     4647 2024-04-11 07:57:07.721881 zorge-1.1.0/zorge/implementation/resolver.py
--rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 zorge-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-04 14:56:28.854602 zorge-1.1.1/LICENSE
+-rw-r--r--   0        0        0       66 2024-04-15 11:44:41.305549 zorge-1.1.1/README.md
+-rw-r--r--   0        0        0      367 2024-04-15 11:44:50.975041 zorge-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-02-19 15:31:10.223460 zorge-1.1.1/zorge/.DS_Store
+-rw-r--r--   0        0        0      130 2024-04-11 07:57:07.720615 zorge-1.1.1/zorge/__init__.py
+-rw-r--r--   0        0        0      188 2024-04-11 07:57:07.720731 zorge-1.1.1/zorge/contracts/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-11 07:57:07.720842 zorge-1.1.1/zorge/contracts/domain.py
+-rw-r--r--   0        0        0     1309 2024-04-11 07:57:07.720917 zorge-1.1.1/zorge/contracts/internal.py
+-rw-r--r--   0        0        0       87 2024-04-11 07:57:07.720992 zorge-1.1.1/zorge/exceptions/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-11 07:57:07.721065 zorge-1.1.1/zorge/exceptions/di.py
+-rw-r--r--   0        0        0        1 2024-04-11 07:57:07.721285 zorge-1.1.1/zorge/implementation/__init__.py
+-rw-r--r--   0        0        0     6888 2024-04-11 07:57:07.721589 zorge-1.1.1/zorge/implementation/container.py
+-rw-r--r--   0        0        0     4647 2024-04-11 07:57:07.721881 zorge-1.1.1/zorge/implementation/resolver.py
+-rw-r--r--   0        0        0      551 1970-01-01 00:00:00.000000 zorge-1.1.1/PKG-INFO
```

### Comparing `zorge-1.1.0/LICENSE` & `zorge-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zorge-1.1.0/zorge/.DS_Store` & `zorge-1.1.1/zorge/.DS_Store`

 * *Files identical despite different names*

### Comparing `zorge-1.1.0/zorge/contracts/domain.py` & `zorge-1.1.1/zorge/contracts/domain.py`

 * *Files identical despite different names*

### Comparing `zorge-1.1.0/zorge/contracts/internal.py` & `zorge-1.1.1/zorge/contracts/internal.py`

 * *Files identical despite different names*

### Comparing `zorge-1.1.0/zorge/implementation/container.py` & `zorge-1.1.1/zorge/implementation/container.py`

 * *Files identical despite different names*

### Comparing `zorge-1.1.0/zorge/implementation/resolver.py` & `zorge-1.1.1/zorge/implementation/resolver.py`

 * *Files identical despite different names*

