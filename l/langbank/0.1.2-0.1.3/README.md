# Comparing `tmp/langbank-0.1.2.tar.gz` & `tmp/langbank-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langbank-0.1.2.tar", last modified: Mon Apr 15 10:38:49 2024, max compression
+gzip compressed data, was "langbank-0.1.3.tar", last modified: Mon Apr 15 10:41:53 2024, max compression
```

## Comparing `langbank-0.1.2.tar` & `langbank-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.522431 langbank-0.1.2/
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1304 2024-04-15 10:38:49.522178 langbank-0.1.2/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1032 2024-04-15 09:49:18.000000 langbank-0.1.2/README.md
--rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-15 10:38:49.522469 langbank-0.1.2/setup.cfg
--rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-15 10:38:43.000000 langbank-0.1.2/setup.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.520524 langbank-0.1.2/src/
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.521153 langbank-0.1.2/src/langbank/
--rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1.2/src/langbank/__init__.py
--rw-r--r--   0 teddygonyea   (501) staff       (20)     4429 2024-04-15 10:15:02.000000 langbank-0.1.2/src/langbank/main.py
-drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:38:49.521991 langbank-0.1.2/src/langbank.egg-info/
--rw-r--r--   0 teddygonyea   (501) staff       (20)     1304 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/PKG-INFO
--rw-r--r--   0 teddygonyea   (501) staff       (20)      208 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/SOURCES.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/dependency_links.txt
--rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-15 10:38:49.000000 langbank-0.1.2/src/langbank.egg-info/top_level.txt
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.141145 langbank-0.1.3/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 10:41:53.140886 langbank-0.1.3/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      622 2024-04-15 10:40:40.000000 langbank-0.1.3/README.md
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       38 2024-04-15 10:41:53.141183 langbank-0.1.3/setup.cfg
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      492 2024-04-15 10:41:37.000000 langbank-0.1.3/setup.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.139183 langbank-0.1.3/src/
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.139875 langbank-0.1.3/src/langbank/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)       27 2024-04-14 12:25:24.000000 langbank-0.1.3/src/langbank/__init__.py
+-rw-r--r--   0 teddygonyea   (501) staff       (20)     4429 2024-04-15 10:15:02.000000 langbank-0.1.3/src/langbank/main.py
+drwxr-xr-x   0 teddygonyea   (501) staff       (20)        0 2024-04-15 10:41:53.140705 langbank-0.1.3/src/langbank.egg-info/
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      894 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/PKG-INFO
+-rw-r--r--   0 teddygonyea   (501) staff       (20)      208 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/SOURCES.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        1 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/dependency_links.txt
+-rw-r--r--   0 teddygonyea   (501) staff       (20)        9 2024-04-15 10:41:53.000000 langbank-0.1.3/src/langbank.egg-info/top_level.txt
```

### Comparing `langbank-0.1.2/src/langbank/main.py` & `langbank-0.1.3/src/langbank/main.py`

 * *Files identical despite different names*

