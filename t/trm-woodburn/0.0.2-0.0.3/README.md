# Comparing `tmp/trm_woodburn-0.0.2.tar.gz` & `tmp/trm_woodburn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.2.tar", last modified: Mon Apr 15 19:34:36 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.3.tar", last modified: Mon Apr 15 19:39:02 2024, max compression
```

## Comparing `trm_woodburn-0.0.2.tar` & `trm_woodburn-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.928838 trm_woodburn-0.0.2/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.2/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:34:36.928781 trm_woodburn-0.0.2/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5046 2024-04-15 19:17:04.000000 trm_woodburn-0.0.2/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.2/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 19:34:36.929054 trm_woodburn-0.0.2/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.927184 trm_woodburn-0.0.2/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.927856 trm_woodburn-0.0.2/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.2/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19631 2024-04-15 19:32:30.000000 trm_woodburn-0.0.2/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.928607 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.920315 trm_woodburn-0.0.3/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.3/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:39:02.920260 trm_woodburn-0.0.3/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5046 2024-04-15 19:17:04.000000 trm_woodburn-0.0.3/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.3/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 19:39:02.920531 trm_woodburn-0.0.3/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.918654 trm_woodburn-0.0.3/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.919343 trm_woodburn-0.0.3/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.3/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19700 2024-04-15 19:37:21.000000 trm_woodburn-0.0.3/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.920089 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.2/LICENSE.txt` & `trm_woodburn-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.2/PKG-INFO` & `trm_woodburn-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trm_woodburn-0.0.2/README.md` & `trm_woodburn-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.2/setup.cfg` & `trm_woodburn-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.2
+version = 0.0.3
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.2/src/trm/trm.py` & `trm_woodburn-0.0.3/src/trm/trm.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,19 @@
         Desired number of columns if greater than 1 or fraction of existing
         columns if less than 1.
     """
 
     # Get the terminal window size.
     try: # Try to get the true size.
         term_cols, term_rows = os.get_terminal_size()
+        use_color = True
     except: # If getting terminal size fails, use default values.
         term_cols = COLS
         term_rows = ROWS
+        use_color = False
     term_rows -= 1 # Account for the prompt line.
 
     # Convert a fractional canvas size to columns and rows.
     if cols <= 1:
         cols = max(round(term_cols * cols), 3)
     if rows <= 1:
         rows = max(round(term_rows * rows), 3)
@@ -171,15 +173,15 @@
     # Map locations to a large matrix.
     M = np.zeros((subrows*rows, subcols*cols), dtype=int)
     X = np.round(X_jk).astype(int)
     Y = np.round(Y_jk).astype(int)
     M[Y, X] = 1 # Puts a 1 wherever the curve coordinates are.
 
     # Scale the data to dots.
-    if J > 1:
+    if (J > 1) and (use_color):
         color_list = [39, 40, 220, 208, 201]
         u = X//subcols
         v = Y//subrows
         F = np.zeros((rows, cols), dtype=int)
         for j in range(J):
             F[v[j], u[j]] = color_list[j % 5]
     else:
```

### Comparing `trm_woodburn-0.0.2/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.3/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

