# Comparing `tmp/ObjectToString-0.2.67.tar.gz` & `tmp/ObjectToString-0.2.68.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ObjectToString-0.2.67.tar", last modified: Mon Apr  8 15:31:24 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "ObjectToString-0.2.68.tar", last modified: Mon Apr 15 15:53:40 2024, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `ObjectToString-0.2.67.tar` & `ObjectToString-0.2.68.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.67/
--rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.67/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.67/objecttostring/
-drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.67/ObjectToString.egg-info/
--rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.67/ObjectToString.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.67/ObjectToString.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.67/ObjectToString.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.67/ObjectToString.egg-info/top_level.txt
--rwxrwxrwx   0        0        0  3709952 2024-04-08 15:15:22.000000 ObjectToString-0.2.67/objecttostring/pdslib.cp312-win_amd64.pyd
--rwxrwxrwx   0        0        0     4368 2024-02-22 15:49:50.000000 ObjectToString-0.2.67/objecttostring/test1.py
--rwxrwxrwx   0        0        0      100 2024-04-08 15:31:10.000000 ObjectToString-0.2.67/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.67/setup.cfg
--rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.67/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-03 09:43:44.000000 ObjectToString-0.2.68/
+-rw-rw-rw-   0        0        0       59 2023-09-03 09:39:02.000000 ObjectToString-0.2.68/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.68/objecttostring/
+drwxrwxrwx   0        0        0        0 2023-09-06 15:34:56.000000 ObjectToString-0.2.68/ObjectToString.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-09-06 15:34:55.000000 ObjectToString-0.2.68/ObjectToString.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       99 2023-09-06 15:34:55.000000 ObjectToString-0.2.68/ObjectToString.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2023-09-06 15:34:55.000000 ObjectToString-0.2.68/ObjectToString.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       15 2023-09-06 15:34:55.000000 ObjectToString-0.2.68/ObjectToString.egg-info/top_level.txt
+-rwxrwxrwx   0        0        0  3709952 2024-04-15 15:40:09.000000 ObjectToString-0.2.68/objecttostring/pdslib.cp312-win_amd64.pyd
+-rwxrwxrwx   0        0        0    90112 2024-04-15 15:34:42.000000 ObjectToString-0.2.68/objecttostring/python.exe
+-rwxrwxrwx   0        0        0    56320 2024-04-15 15:34:26.000000 ObjectToString-0.2.68/objecttostring/python3.dll
+-rwxrwxrwx   0        0        0  8850432 2024-04-15 15:34:42.000000 ObjectToString-0.2.68/objecttostring/python312.dll
+-rwxrwxrwx   0        0        0      100 2024-04-15 15:53:29.000000 ObjectToString-0.2.68/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-09-06 15:34:56.000000 ObjectToString-0.2.68/setup.cfg
+-rw-rw-rw-   0        0        0      234 2023-09-03 09:43:44.000000 ObjectToString-0.2.68/setup.py
```
