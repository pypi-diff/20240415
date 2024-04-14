# Comparing `tmp/PokemonLibrary-1.0.0.tar.gz` & `tmp/PokemonLibrary-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PokemonLibrary-1.0.0.tar", last modified: Sun Apr 14 23:32:39 2024, max compression
+gzip compressed data, was "PokemonLibrary-1.0.1.tar", last modified: Sun Apr 14 23:47:00 2024, max compression
```

## Comparing `PokemonLibrary-1.0.0.tar` & `PokemonLibrary-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 23:32:39.197167 PokemonLibrary-1.0.0/
--rw-rw-rw-   0        0        0      188 2024-04-14 23:32:39.196172 PokemonLibrary-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 23:32:39.178614 PokemonLibrary-1.0.0/PokemonLibrary/
--rw-rw-rw-   0        0        0       41 2024-04-14 23:31:18.000000 PokemonLibrary-1.0.0/PokemonLibrary/__init__.py
--rw-rw-rw-   0        0        0      788 2024-04-14 21:58:23.000000 PokemonLibrary-1.0.0/PokemonLibrary/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-14 23:32:39.194193 PokemonLibrary-1.0.0/PokemonLibrary.egg-info/
--rw-rw-rw-   0        0        0      188 2024-04-14 23:32:39.000000 PokemonLibrary-1.0.0/PokemonLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-04-14 23:32:39.000000 PokemonLibrary-1.0.0/PokemonLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 23:32:39.000000 PokemonLibrary-1.0.0/PokemonLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-14 23:32:39.000000 PokemonLibrary-1.0.0/PokemonLibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 23:32:39.000000 PokemonLibrary-1.0.0/PokemonLibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 23:32:39.198166 PokemonLibrary-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      394 2024-04-14 23:30:53.000000 PokemonLibrary-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 23:47:00.641134 PokemonLibrary-1.0.1/
+-rw-rw-rw-   0        0        0      188 2024-04-14 23:47:00.640138 PokemonLibrary-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 23:47:00.620149 PokemonLibrary-1.0.1/PokemonLibrary/
+-rw-rw-rw-   0        0        0       41 2024-04-14 23:31:18.000000 PokemonLibrary-1.0.1/PokemonLibrary/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 PokemonLibrary-1.0.1/PokemonLibrary/pokemon.csv
+-rw-rw-rw-   0        0        0      788 2024-04-14 21:58:23.000000 PokemonLibrary-1.0.1/PokemonLibrary/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-14 23:47:00.637722 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 23:47:00.641134 PokemonLibrary-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      449 2024-04-14 23:46:01.000000 PokemonLibrary-1.0.1/setup.py
```

### Comparing `PokemonLibrary-1.0.0/PokemonLibrary/random_pokemon.py` & `PokemonLibrary-1.0.1/PokemonLibrary/random_pokemon.py`

 * *Files identical despite different names*

