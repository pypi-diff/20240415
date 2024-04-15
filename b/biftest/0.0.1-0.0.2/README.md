# Comparing `tmp/biftest-0.0.1.tar.gz` & `tmp/biftest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biftest-0.0.1.tar", last modified: Fri Apr  5 00:44:39 2024, max compression
+gzip compressed data, was "biftest-0.0.2.tar", last modified: Mon Apr 15 11:56:19 2024, max compression
```

## Comparing `biftest-0.0.1.tar` & `biftest-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-05 00:44:39.499435 biftest-0.0.1/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-05 00:44:39.499320 biftest-0.0.1/PKG-INFO
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-05 00:44:39.498630 biftest-0.0.1/biftest/
--rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.1/biftest/__init__.py
--rw-r--r--   0 youngjin   (501) staff       (20)       39 2024-04-05 00:38:56.000000 biftest-0.0.1/biftest/hel.py
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-05 00:44:39.499131 biftest-0.0.1/biftest.egg-info/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-05 00:44:39.000000 biftest-0.0.1/biftest.egg-info/PKG-INFO
--rw-r--r--   0 youngjin   (501) staff       (20)      167 2024-04-05 00:44:39.000000 biftest-0.0.1/biftest.egg-info/SOURCES.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-05 00:44:39.000000 biftest-0.0.1/biftest.egg-info/dependency_links.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-05 00:44:39.000000 biftest-0.0.1/biftest.egg-info/top_level.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-05 00:44:39.499493 biftest-0.0.1/setup.cfg
--rw-r--r--   0 youngjin   (501) staff       (20)      111 2024-04-05 00:44:18.000000 biftest-0.0.1/setup.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-15 11:56:19.461657 biftest-0.0.2/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-15 11:56:19.461501 biftest-0.0.2/PKG-INFO
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-15 11:56:19.460695 biftest-0.0.2/biftest/
+-rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.2/biftest/__init__.py
+-rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.0.2/biftest/hel.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-15 11:56:19.461312 biftest-0.0.2/biftest.egg-info/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/PKG-INFO
+-rw-r--r--   0 youngjin   (501) staff       (20)      197 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/SOURCES.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/dependency_links.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       42 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/requires.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-15 11:56:19.000000 biftest-0.0.2/biftest.egg-info/top_level.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-15 11:56:19.461713 biftest-0.0.2/setup.cfg
+-rw-r--r--   0 youngjin   (501) staff       (20)      215 2024-04-15 11:55:36.000000 biftest-0.0.2/setup.py
```

