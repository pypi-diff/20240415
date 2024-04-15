# Comparing `tmp/dune_rivals-0.4.1.tar.gz` & `tmp/dune_rivals-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dune_rivals-0.4.1.tar", last modified: Sun Apr 14 16:05:09 2024, max compression
+gzip compressed data, was "dune_rivals-0.4.2.tar", last modified: Mon Apr 15 21:49:23 2024, max compression
```

## Comparing `dune_rivals-0.4.1.tar` & `dune_rivals-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-14 16:05:09.963288 dune_rivals-0.4.1/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-14 16:05:09.962726 dune_rivals-0.4.1/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.4.1/README.md
-drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-14 16:05:09.962319 dune_rivals-0.4.1/dune_rivals.egg-info/
--rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-14 16:05:09.000000 dune_rivals-0.4.1/dune_rivals.egg-info/PKG-INFO
--rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-14 16:05:09.000000 dune_rivals-0.4.1/dune_rivals.egg-info/SOURCES.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-14 16:05:09.000000 dune_rivals-0.4.1/dune_rivals.egg-info/dependency_links.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-14 16:05:09.000000 dune_rivals-0.4.1/dune_rivals.egg-info/top_level.txt
--rw-r--r--   0 matthewrusso   (501) staff       (20)    23794 2024-04-14 16:04:27.000000 dune_rivals-0.4.1/dune_rivals.py
--rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-14 16:04:57.000000 dune_rivals-0.4.1/pyproject.toml
--rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-14 16:05:09.963388 dune_rivals-0.4.1/setup.cfg
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-15 21:49:23.641442 dune_rivals-0.4.2/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-15 21:49:23.641004 dune_rivals-0.4.2/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        0 2024-04-11 16:36:06.000000 dune_rivals-0.4.2/README.md
+drwxr-xr-x   0 matthewrusso   (501) staff       (20)        0 2024-04-15 21:49:23.640364 dune_rivals-0.4.2/dune_rivals.egg-info/
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      436 2024-04-15 21:49:23.000000 dune_rivals-0.4.2/dune_rivals.egg-info/PKG-INFO
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      179 2024-04-15 21:49:23.000000 dune_rivals-0.4.2/dune_rivals.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)        1 2024-04-15 21:49:23.000000 dune_rivals-0.4.2/dune_rivals.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       12 2024-04-15 21:49:23.000000 dune_rivals-0.4.2/dune_rivals.egg-info/top_level.txt
+-rw-r--r--   0 matthewrusso   (501) staff       (20)    24154 2024-04-15 21:48:48.000000 dune_rivals-0.4.2/dune_rivals.py
+-rw-r--r--   0 matthewrusso   (501) staff       (20)      503 2024-04-15 21:49:15.000000 dune_rivals-0.4.2/pyproject.toml
+-rw-r--r--   0 matthewrusso   (501) staff       (20)       38 2024-04-15 21:49:23.641537 dune_rivals-0.4.2/setup.cfg
```

### Comparing `dune_rivals-0.4.1/dune_rivals.py` & `dune_rivals-0.4.2/dune_rivals.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,22 @@
         self.j = np.random.randint(0, MAP_DIM - 1)
         self.gamestate = ray.get_actor("GameState")
         self.spice_loc_map = None
         self.spice_file_map = None
         self.order_map = None
         self.name = None
 
+    def _set_fields(self, spice_loc_map: np.ndarray, spice_file_map: np.ndarray, order_map: dict) -> None:
+        """
+        This is technically not necessary but it will save a lot of people issues with a race condition.
+        """
+        self.spice_loc_map = spice_loc_map
+        self.spice_file_map = spice_file_map
+        self.order_map = order_map
+
     def _destroy_spice_field(self) -> bool:
         """
         DO NOT MODIFY
 
         (Contributes to) destroy(ing) the spice field at location: (self.i, self.j)
 
         Recall that order_map[(i, j)] returns the order in which your Fedaykin must
```

