# Comparing `tmp/cochleogram-0.8.3.tar.gz` & `tmp/cochleogram-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.8.3.tar", last modified: Tue Feb 27 21:31:08 2024, max compression
+gzip compressed data, was "cochleogram-0.8.4.tar", last modified: Mon Apr 15 18:02:43 2024, max compression
```

## Comparing `cochleogram-0.8.3.tar` & `cochleogram-0.8.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:31:08.118934 cochleogram-0.8.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:31:08.110934 cochleogram-0.8.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:31:08.114934 cochleogram-0.8.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-02-27 21:30:56.000000 cochleogram-0.8.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-02-27 21:30:56.000000 cochleogram-0.8.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-27 21:31:08.118934 cochleogram-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-27 21:30:56.000000 cochleogram-0.8.3/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:31:08.114934 cochleogram-0.8.3/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:31:08.118934 cochleogram-0.8.3/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/main-icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (127)    25893 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-02-27 21:30:56.000000 cochleogram-0.8.3/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 21:31:08.118934 cochleogram-0.8.3/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-27 21:31:08.000000 cochleogram-0.8.3/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-27 21:30:56.000000 cochleogram-0.8.3/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-27 21:30:56.000000 cochleogram-0.8.3/license
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-02-27 21:30:56.000000 cochleogram-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-02-27 21:30:56.000000 cochleogram-0.8.3/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 21:31:08.118934 cochleogram-0.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.990105 cochleogram-0.8.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.982105 cochleogram-0.8.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.986105 cochleogram-0.8.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-15 18:02:39.000000 cochleogram-0.8.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-15 18:02:39.000000 cochleogram-0.8.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-15 18:02:43.990105 cochleogram-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-15 18:02:39.000000 cochleogram-0.8.4/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.986105 cochleogram-0.8.4/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.990105 cochleogram-0.8.4/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/main-icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25893 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18597 2024-04-15 18:02:39.000000 cochleogram-0.8.4/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 18:02:43.990105 cochleogram-0.8.4/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9296 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 18:02:43.000000 cochleogram-0.8.4/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 18:02:39.000000 cochleogram-0.8.4/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-15 18:02:39.000000 cochleogram-0.8.4/license
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-15 18:02:39.000000 cochleogram-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-15 18:02:39.000000 cochleogram-0.8.4/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 18:02:43.990105 cochleogram-0.8.4/setup.cfg
```

### Comparing `cochleogram-0.8.3/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.8.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/.gitignore` & `cochleogram-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/PKG-INFO` & `cochleogram-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.8.3
+Version: 0.8.4
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: atom
 Requires-Dist: enaml[qt6-pyside]
```

### Comparing `cochleogram-0.8.3/cochleogram/config.py` & `cochleogram-0.8.4/cochleogram/config.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/gui.enaml` & `cochleogram-0.8.4/cochleogram/gui.enaml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/cells.png` & `cochleogram-0.8.4/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/exclude.png` & `cochleogram-0.8.4/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/main-icon.ico` & `cochleogram-0.8.4/cochleogram/icons/main-icon.ico`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/main-icon.png` & `cochleogram-0.8.4/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/make_icons.py` & `cochleogram-0.8.4/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/spiral.png` & `cochleogram-0.8.4/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/icons/tile.png` & `cochleogram-0.8.4/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/instructions.html` & `cochleogram-0.8.4/cochleogram/instructions.html`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/main.py` & `cochleogram-0.8.4/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/model.py` & `cochleogram-0.8.4/cochleogram/model.py`

 * *Files identical despite different names*

```diff
@@ -376,16 +376,17 @@
             'tiles': {t.source: t.get_state() for t in self.tiles},
             'copied_from': self.copied_from,
         })
         return state
 
     def set_state(self, state):
         super().set_state(state)
-        for tile in self.tiles:
-            tile.set_state(state['tiles'][tile.source])
+        if 'tiles' in state:
+            for tile in self.tiles:
+                tile.set_state(state['tiles'][tile.source])
 
 
 freq_fn = {
     'mouse': lambda d: (10**((1-d)*0.92) - 0.680) * 9.8,
 }
```

### Comparing `cochleogram-0.8.3/cochleogram/plot.py` & `cochleogram-0.8.4/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/presenter.py` & `cochleogram-0.8.4/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/readers.py` & `cochleogram-0.8.4/cochleogram/readers.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram/util.py` & `cochleogram-0.8.4/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.8.4/cochleogram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.8.3
+Version: 0.8.4
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Requires-Dist: atom
 Requires-Dist: enaml[qt6-pyside]
```

### Comparing `cochleogram-0.8.3/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.8.4/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/license` & `cochleogram-0.8.4/license`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/pyproject.toml` & `cochleogram-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.8.3/readme.rst` & `cochleogram-0.8.4/readme.rst`

 * *Files identical despite different names*

