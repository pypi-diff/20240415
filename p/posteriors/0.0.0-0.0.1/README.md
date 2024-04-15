# Comparing `tmp/posteriors-0.0.0.tar.gz` & `tmp/posteriors-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "posteriors-0.0.0.tar", last modified: Mon Mar 25 19:15:15 2024, max compression
+gzip compressed data, was "posteriors-0.0.1.tar", last modified: Mon Apr 15 17:46:50 2024, max compression
```

## Comparing `posteriors-0.0.0.tar` & `posteriors-0.0.1.tar`

### file list

```diff
@@ -1,11 +1,23 @@
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-25 19:15:15.083260 posteriors-0.0.0/
--rw-r--r--   0 sam        (501) staff       (20)      127 2024-03-25 19:15:15.083093 posteriors-0.0.0/PKG-INFO
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-25 19:15:15.082294 posteriors-0.0.0/posteriors/
--rw-r--r--   0 sam        (501) staff       (20)        0 2024-03-25 19:05:30.000000 posteriors-0.0.0/posteriors/__init__.py
-drwxr-xr-x   0 sam        (501) staff       (20)        0 2024-03-25 19:15:15.082914 posteriors-0.0.0/posteriors.egg-info/
--rw-r--r--   0 sam        (501) staff       (20)      127 2024-03-25 19:15:15.000000 posteriors-0.0.0/posteriors.egg-info/PKG-INFO
--rw-r--r--   0 sam        (501) staff       (20)      173 2024-03-25 19:15:15.000000 posteriors-0.0.0/posteriors.egg-info/SOURCES.txt
--rw-r--r--   0 sam        (501) staff       (20)        1 2024-03-25 19:15:15.000000 posteriors-0.0.0/posteriors.egg-info/dependency_links.txt
--rw-r--r--   0 sam        (501) staff       (20)       11 2024-03-25 19:15:15.000000 posteriors-0.0.0/posteriors.egg-info/top_level.txt
--rw-r--r--   0 sam        (501) staff       (20)      150 2024-03-25 19:08:26.000000 posteriors-0.0.0/pyproject.toml
--rw-r--r--   0 sam        (501) staff       (20)       38 2024-03-25 19:15:15.083312 posteriors-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.392438 posteriors-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 17:46:46.000000 posteriors-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-15 17:46:50.392438 posteriors-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-04-15 17:46:46.000000 posteriors-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.388438 posteriors-0.0.1/posteriors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/torchopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22478 2024-04-15 17:46:46.000000 posteriors-0.0.1/posteriors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.392438 posteriors-0.0.1/posteriors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 17:46:50.000000 posteriors-0.0.1/posteriors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-15 17:46:46.000000 posteriors-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:46:50.392438 posteriors-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:46:50.392438 posteriors-0.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_torchopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16698 2024-04-15 17:46:46.000000 posteriors-0.0.1/tests/test_utils.py
```

