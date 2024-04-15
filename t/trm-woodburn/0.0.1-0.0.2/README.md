# Comparing `tmp/trm_woodburn-0.0.1.tar.gz` & `tmp/trm_woodburn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.1.tar", last modified: Mon Apr 15 19:17:27 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.2.tar", last modified: Mon Apr 15 19:34:36 2024, max compression
```

## Comparing `trm_woodburn-0.0.1.tar` & `trm_woodburn-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:17:27.535541 trm_woodburn-0.0.1/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.1/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:17:27.535480 trm_woodburn-0.0.1/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5046 2024-04-15 19:17:04.000000 trm_woodburn-0.0.1/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.1/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 19:17:27.535762 trm_woodburn-0.0.1/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:17:27.533909 trm_woodburn-0.0.1/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:17:27.534587 trm_woodburn-0.0.1/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.1/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19631 2024-04-15 17:08:23.000000 trm_woodburn-0.0.1/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:17:27.535312 trm_woodburn-0.0.1/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:17:27.000000 trm_woodburn-0.0.1/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 19:17:27.000000 trm_woodburn-0.0.1/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 19:17:27.000000 trm_woodburn-0.0.1/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 19:17:27.000000 trm_woodburn-0.0.1/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 19:17:27.000000 trm_woodburn-0.0.1/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.928838 trm_woodburn-0.0.2/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.2/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:34:36.928781 trm_woodburn-0.0.2/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5046 2024-04-15 19:17:04.000000 trm_woodburn-0.0.2/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.2/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 19:34:36.929054 trm_woodburn-0.0.2/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.927184 trm_woodburn-0.0.2/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.927856 trm_woodburn-0.0.2/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.2/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19631 2024-04-15 19:32:30.000000 trm_woodburn-0.0.2/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:34:36.928607 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 19:34:36.000000 trm_woodburn-0.0.2/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.1/LICENSE.txt` & `trm_woodburn-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.1/PKG-INFO` & `trm_woodburn-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trm_woodburn-0.0.1/README.md` & `trm_woodburn-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.1/setup.cfg` & `trm_woodburn-0.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.1
+version = 0.0.2
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.1/src/trm/trm.py` & `trm_woodburn-0.0.2/src/trm/trm.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import numpy as np
 
 UNI = True # flag to use unicode characters
 COLS = 60 # default column width
 ROWS = 20 # default row height
 
 
-def plot(x, y=None, label='', cols=1, rows=1):
+def plot(x, y=None, label='', rows=1, cols=1):
     """
     Create a text-based plot of the path defined by (`x`, `y`) using characters.
     If the size of the terminal can be found, that will be used for sizing the
     plot. Otherwise, the default dimensions (COLS, ROWS) will be used. Note that
     this function does not plot connecting lines, only the points specified by
     the (`x`, `y`) pairs.
 
@@ -50,20 +50,20 @@
         Array of x-axis values or matrix of rows of x-axis values.
     y : (K,) or (J, K) np.ndarray, default None
         Array of y-axis values or matrix of rows of y-axis values. If `y` is not
         provided, `x` will be used as the `y` array and `x` will be defined to
         be an array of indices.
     label : str, default ''
         Text to place at top of the plot, centered in the border.
-    cols : int, default 1
-        Desired number of columns if greater than 1 or fraction of existing
-        columns if less than 1.
     rows : int, default 1
         Desired number of rows if greater than 1 or fraction of existing rows if
         less than 1.
+    cols : int, default 1
+        Desired number of columns if greater than 1 or fraction of existing
+        columns if less than 1.
     """
 
     # Get the terminal window size.
     try: # Try to get the true size.
         term_cols, term_rows = os.get_terminal_size()
     except: # If getting terminal size fails, use default values.
         term_cols = COLS
@@ -610,15 +610,15 @@
         else:
             t_remaining = t_elapsed*(1.0 - ratio)/ratio
             clk_str = " -" + time_str(t_remaining)
     else:
         clk_str = ""
 
     # Build the progress bar.
-    N = width - 7 - len(clk_str) # maximum length of bar within the brackets
+    N = width - 8 - len(clk_str) # maximum length of bar within the brackets
     if k + 1 == K:
         print(f"\r100% [{'/'*N}]{clk_str}", flush=True)
     elif (K < N) or (k % int(K/N) == 0):
         bar_len = int(N*ratio)
         print(f"\r{int(100*ratio):3d}% "
             + f"[{'/'*bar_len}{'-'*(N - bar_len)}]{clk_str}",
             end="", flush=True)
```

### Comparing `trm_woodburn-0.0.1/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.2/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

