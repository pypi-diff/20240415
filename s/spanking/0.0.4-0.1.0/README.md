# Comparing `tmp/spanking-0.0.4.tar.gz` & `tmp/spanking-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanking-0.0.4.tar", last modified: Sun Apr 14 22:38:26 2024, max compression
+gzip compressed data, was "spanking-0.1.0.tar", last modified: Sun Apr 14 22:54:29 2024, max compression
```

## Comparing `spanking-0.0.4.tar` & `spanking-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:38:26.214398 spanking-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:38:16.000000 spanking-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-14 22:38:26.214398 spanking-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-14 22:38:16.000000 spanking-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:38:26.214398 spanking-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-14 22:38:16.000000 spanking-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:38:26.214398 spanking-0.0.4/spanking/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 22:38:16.000000 spanking-0.0.4/spanking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-14 22:38:16.000000 spanking-0.0.4/spanking/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 22:38:16.000000 spanking-0.0.4/spanking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:38:26.214398 spanking-0.0.4/spanking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:38:26.000000 spanking-0.0.4/spanking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:54:29.296356 spanking-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 22:54:20.000000 spanking-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-14 22:54:29.296356 spanking-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-14 22:54:20.000000 spanking-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 22:54:29.296356 spanking-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-14 22:54:20.000000 spanking-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:54:29.296356 spanking-0.1.0/spanking/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 22:54:20.000000 spanking-0.1.0/spanking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-14 22:54:20.000000 spanking-0.1.0/spanking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-14 22:54:20.000000 spanking-0.1.0/spanking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 22:54:29.296356 spanking-0.1.0/spanking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 22:54:29.000000 spanking-0.1.0/spanking.egg-info/top_level.txt
```

### Comparing `spanking-0.0.4/LICENSE` & `spanking-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spanking-0.0.4/PKG-INFO` & `spanking-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.0.4
+Version: 0.1.0
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `spanking-0.0.4/README.md` & `spanking-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spanking-0.0.4/setup.py` & `spanking-0.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `spanking-0.0.4/spanking/main.py` & `spanking-0.1.0/spanking/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         else:
             self.embeddings = jnp.concatenate((self.embeddings, new_embeddings), axis=0)
         self.texts.extend(texts)
 
     def delete_text(self, index):
         if 0 <= index < len(self.texts):
             self.texts.pop(index)
-            self.embeddings = self.embeddings.at[index].delete()
+            self.embeddings = jnp.delete(self.embeddings, index, axis=0)
         else:
             raise IndexError("Invalid index")
 
     def update_text(self, index, new_text):
         if 0 <= index < len(self.texts):
             self.texts[index] = new_text
             new_embedding = jnp.array(self.model.encode([new_text], normalize_embeddings=True)).squeeze()
```

### Comparing `spanking-0.0.4/spanking.egg-info/PKG-INFO` & `spanking-0.1.0/spanking.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.0.4
+Version: 0.1.0
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

