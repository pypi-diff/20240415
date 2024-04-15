# Comparing `tmp/L7N-0.5.tar.gz` & `tmp/L7N-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "L7N-0.5.tar", last modified: Thu Apr 11 12:43:26 2024, max compression
+gzip compressed data, was "L7N-1.1.tar", last modified: Mon Apr 15 00:12:44 2024, max compression
```

## Comparing `L7N-0.5.tar` & `L7N-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 12:43:26.440308 L7N-0.5/
-drwxrwxrwx   0        0        0        0 2024-04-11 12:43:26.347315 L7N-0.5/L7N/
--rw-rw-rw-   0        0        0     4389 2024-04-11 12:30:12.000000 L7N-0.5/L7N/L7N.py
--rw-rw-rw-   0        0        0       33 2024-04-11 12:26:54.000000 L7N-0.5/L7N/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 12:43:26.394316 L7N-0.5/L7N.egg-info/
--rw-rw-rw-   0        0        0      297 2024-04-11 12:43:25.000000 L7N-0.5/L7N.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2024-04-11 12:43:25.000000 L7N-0.5/L7N.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 12:43:25.000000 L7N-0.5/L7N.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-11 12:43:25.000000 L7N-0.5/L7N.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2023-11-19 12:48:39.000000 L7N-0.5/LICENSE.txt
--rw-rw-rw-   0        0        0      297 2024-04-11 12:43:26.440308 L7N-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-11 12:43:26.453314 L7N-0.5/setup.cfg
--rw-rw-rw-   0        0        0      378 2024-04-11 12:42:51.000000 L7N-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:12:44.231148 L7N-1.1/
+drwxrwxrwx   0        0        0        0 2024-04-15 00:12:44.181151 L7N-1.1/L7N/
+-rw-rw-rw-   0        0        0    15946 2024-04-15 00:06:03.000000 L7N-1.1/L7N/L7N.py
+-rw-rw-rw-   0        0        0      180 2024-04-15 00:04:00.000000 L7N-1.1/L7N/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:12:44.224147 L7N-1.1/L7N.egg-info/
+-rw-rw-rw-   0        0        0      289 2024-04-15 00:12:42.000000 L7N-1.1/L7N.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2024-04-15 00:12:42.000000 L7N-1.1/L7N.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:12:42.000000 L7N-1.1/L7N.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-15 00:12:42.000000 L7N-1.1/L7N.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2023-11-19 12:48:38.000000 L7N-1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      289 2024-04-15 00:12:44.232149 L7N-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:12:44.237146 L7N-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      370 2024-04-12 18:14:14.000000 L7N-1.1/setup.py
```

