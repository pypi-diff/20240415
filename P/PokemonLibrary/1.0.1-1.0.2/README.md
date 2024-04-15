# Comparing `tmp/PokemonLibrary-1.0.1.tar.gz` & `tmp/PokemonLibrary-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PokemonLibrary-1.0.1.tar", last modified: Sun Apr 14 23:47:00 2024, max compression
+gzip compressed data, was "PokemonLibrary-1.0.2.tar", last modified: Mon Apr 15 00:00:39 2024, max compression
```

## Comparing `PokemonLibrary-1.0.1.tar` & `PokemonLibrary-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 23:47:00.641134 PokemonLibrary-1.0.1/
--rw-rw-rw-   0        0        0      188 2024-04-14 23:47:00.640138 PokemonLibrary-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 23:47:00.620149 PokemonLibrary-1.0.1/PokemonLibrary/
--rw-rw-rw-   0        0        0       41 2024-04-14 23:31:18.000000 PokemonLibrary-1.0.1/PokemonLibrary/__init__.py
--rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 PokemonLibrary-1.0.1/PokemonLibrary/pokemon.csv
--rw-rw-rw-   0        0        0      788 2024-04-14 21:58:23.000000 PokemonLibrary-1.0.1/PokemonLibrary/random_pokemon.py
-drwxrwxrwx   0        0        0        0 2024-04-14 23:47:00.637722 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/
--rw-rw-rw-   0        0        0      188 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-14 23:47:00.000000 PokemonLibrary-1.0.1/PokemonLibrary.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 23:47:00.641134 PokemonLibrary-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      449 2024-04-14 23:46:01.000000 PokemonLibrary-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:00:39.161582 PokemonLibrary-1.0.2/
+-rw-rw-rw-   0        0        0      188 2024-04-15 00:00:39.160591 PokemonLibrary-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 00:00:39.143045 PokemonLibrary-1.0.2/PokemonLibrary/
+-rw-rw-rw-   0        0        0       41 2024-04-14 23:31:18.000000 PokemonLibrary-1.0.2/PokemonLibrary/__init__.py
+-rw-rw-rw-   0        0        0    44028 2016-09-21 12:51:28.000000 PokemonLibrary-1.0.2/PokemonLibrary/pokemon.csv
+-rw-rw-rw-   0        0        0      794 2024-04-15 00:00:13.000000 PokemonLibrary-1.0.2/PokemonLibrary/random_pokemon.py
+drwxrwxrwx   0        0        0        0 2024-04-15 00:00:39.156626 PokemonLibrary-1.0.2/PokemonLibrary.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-04-15 00:00:39.000000 PokemonLibrary-1.0.2/PokemonLibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-04-15 00:00:39.000000 PokemonLibrary-1.0.2/PokemonLibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 00:00:39.000000 PokemonLibrary-1.0.2/PokemonLibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 00:00:39.000000 PokemonLibrary-1.0.2/PokemonLibrary.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-15 00:00:39.000000 PokemonLibrary-1.0.2/PokemonLibrary.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 00:00:39.161582 PokemonLibrary-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      449 2024-04-15 00:00:23.000000 PokemonLibrary-1.0.2/setup.py
```

### Comparing `PokemonLibrary-1.0.1/PokemonLibrary/pokemon.csv` & `PokemonLibrary-1.0.2/PokemonLibrary/pokemon.csv`

 * *Files identical despite different names*

### Comparing `PokemonLibrary-1.0.1/PokemonLibrary/random_pokemon.py` & `PokemonLibrary-1.0.2/PokemonLibrary/random_pokemon.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 class RandomPokemon:
     FILE_PATH = "pokemon.csv"
 
     def __init__(self):
-        self._file = pd.read_csv(RandomPokemon.FILE_PATH)
+        self._file = pd.read_csv(self.FILE_PATH)
         self._pokemon = None
         self._number = None
         self._name = None
         self._type1 = None
 
     def generateRandomPokemon(self):
         self._pokemon = self._file.sample() #Toma una fila aleatoria del archivo
@@ -24,7 +24,8 @@
 
     def getName(self):
         return self._name
 
     def getType1(self):
         return self._type1
 
+RandomPokemon()
```

