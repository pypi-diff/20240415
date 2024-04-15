# Comparing `tmp/trm_woodburn-0.0.4.tar.gz` & `tmp/trm_woodburn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.4.tar", last modified: Mon Apr 15 21:14:05 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.5.tar", last modified: Mon Apr 15 21:34:38 2024, max compression
```

## Comparing `trm_woodburn-0.0.4.tar` & `trm_woodburn-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.055902 trm_woodburn-0.0.4/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.4/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6951 2024-04-15 21:14:05.055853 trm_woodburn-0.0.4/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6472 2024-04-15 21:13:40.000000 trm_woodburn-0.0.4/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.4/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:14:05.056118 trm_woodburn-0.0.4/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.054068 trm_woodburn-0.0.4/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.054902 trm_woodburn-0.0.4/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.4/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19700 2024-04-15 19:37:21.000000 trm_woodburn-0.0.4/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.055686 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     6951 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.250509 trm_woodburn-0.0.5/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.5/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6965 2024-04-15 21:34:38.250453 trm_woodburn-0.0.5/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6486 2024-04-15 21:33:57.000000 trm_woodburn-0.0.5/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.5/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:34:38.250730 trm_woodburn-0.0.5/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.248693 trm_woodburn-0.0.5/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.249536 trm_woodburn-0.0.5/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.5/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19811 2024-04-15 21:32:23.000000 trm_woodburn-0.0.5/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:34:38.250281 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6965 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:34:38.000000 trm_woodburn-0.0.5/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.4/LICENSE.txt` & `trm_woodburn-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.4/PKG-INFO` & `trm_woodburn-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -68,15 +68,16 @@
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
 default to `20` rows and `60` columns.
 
 By default, this library will use Unicode symbols (specifically braille) for
 plotting. A good font to use for this is JuliaMono. However, if your font does
 not support the necessary Unicode symbols, you can tell the library to not use
-them by setting `trm.UNI` to `False` before calling the `trm.plot` function.
+them by setting `trm.config.uni` to `False` before calling the `trm.plot`
+function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
@@ -107,16 +108,17 @@
 
 ```python
 trm.heat(matrix)
 ```
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
-value. If `trm.UNI` is `True`, half-block characters from the Unicode table will
-be used. If it is `False`, two spaces per element of the matrix will be used.
+value. If `trm.config.uni` is `True`, half-block characters from the Unicode
+table will be used. If it is `False`, two spaces per element of the matrix will
+be used.
 
 | With Unicode      | Without Unicode     |
 | ----------------- | ------------------- |
 | ![][fig_heat_uni] | ![][fig_heat_ascii] |
 
 ## Tables
```

### Comparing `trm_woodburn-0.0.4/README.md` & `trm_woodburn-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,16 @@
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
 default to `20` rows and `60` columns.
 
 By default, this library will use Unicode symbols (specifically braille) for
 plotting. A good font to use for this is JuliaMono. However, if your font does
 not support the necessary Unicode symbols, you can tell the library to not use
-them by setting `trm.UNI` to `False` before calling the `trm.plot` function.
+them by setting `trm.config.uni` to `False` before calling the `trm.plot`
+function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
@@ -92,16 +93,17 @@
 
 ```python
 trm.heat(matrix)
 ```
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
-value. If `trm.UNI` is `True`, half-block characters from the Unicode table will
-be used. If it is `False`, two spaces per element of the matrix will be used.
+value. If `trm.config.uni` is `True`, half-block characters from the Unicode
+table will be used. If it is `False`, two spaces per element of the matrix will
+be used.
 
 | With Unicode      | Without Unicode     |
 | ----------------- | ------------------- |
 | ![][fig_heat_uni] | ![][fig_heat_ascii] |
 
 ## Tables
```

### Comparing `trm_woodburn-0.0.4/setup.cfg` & `trm_woodburn-0.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.4
+version = 0.0.5
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.4/src/trm/trm.py` & `trm_woodburn-0.0.5/src/trm/trm.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,26 +27,28 @@
 __status__ = "Development"
 
 import os
 import time
 import math
 import numpy as np
 
-UNI = True # flag to use unicode characters
-COLS = 60 # default column width
-ROWS = 20 # default row height
+
+class config:
+    uni = True # flag to use unicode characters
+    cols = 60 # default column width
+    rows = 20 # default row height
 
 
 def plot(x, y=None, label='', rows=1, cols=1):
     """
     Create a text-based plot of the path defined by (`x`, `y`) using characters.
     If the size of the terminal can be found, that will be used for sizing the
-    plot. Otherwise, the default dimensions (COLS, ROWS) will be used. Note that
-    this function does not plot connecting lines, only the points specified by
-    the (`x`, `y`) pairs.
+    plot. Otherwise, the default dimensions (config.cols, config.rows) will be
+    used. Note that this function does not plot connecting lines, only the
+    points specified by the (`x`, `y`) pairs.
 
     Parameters
     ----------
     x : (K,) or (J, K) np.ndarray
         Array of x-axis values or matrix of rows of x-axis values.
     y : (K,) or (J, K) np.ndarray, default None
         Array of y-axis values or matrix of rows of y-axis values. If `y` is not
@@ -63,31 +65,31 @@
     """
 
     # Get the terminal window size.
     try: # Try to get the true size.
         term_cols, term_rows = os.get_terminal_size()
         use_color = True
     except: # If getting terminal size fails, use default values.
-        term_cols = COLS
-        term_rows = ROWS
+        term_cols = config.cols
+        term_rows = config.rows
         use_color = False
     term_rows -= 1 # Account for the prompt line.
 
     # Convert a fractional canvas size to columns and rows.
     if cols <= 1:
         cols = max(round(term_cols * cols), 3)
     if rows <= 1:
         rows = max(round(term_rows * rows), 3)
 
     # Adjust for the bounding box and ensure integer type.
     rows = int(rows) - 2
     cols = int(cols) - 2
 
     # Define the sub-columns and sub-rows.
-    if UNI:
+    if config.uni:
         subcols = 2
         subrows = 4
     else:
         subcols = 1
         subrows = 3
 
     # If only `x` is provided, copy to `y`
@@ -184,15 +186,15 @@
         F = np.zeros((rows, cols), dtype=int)
         for j in range(J):
             F[v[j], u[j]] = color_list[j % 5]
     else:
         F = None
 
     # Convert the large matrix to a smaller matrix of character values.
-    C = matrix_to_braille(M) if UNI else matrix_to_ascii(M)
+    C = matrix_to_braille(M) if config.uni else matrix_to_ascii(M)
 
     # Draw the plot.
     draw_graph(C, ranges, label, F, row_zero)
 
 
 def draw_graph(C, left=None, right=None, F=None, row_zero=-1):
     """
@@ -205,15 +207,15 @@
     right : string, default None
         String to place on the right of the box.
     F : (I, J) int np.ndarray, default None
         Matrix of foreground 8-bit color values.
     """
 
     # Define the box drawing characters.
-    if UNI:
+    if config.uni:
         b = ["\u250C", "\u2500", "\u2510", "\u2502", "\u2502",
                 "\u251C", "\u2524", "\u2514", "\u2518"]
     else:
         b = [".", "-", ".", "|", "|", "+", "+", "'", "'"]
 
     # Replace zeros with spaces.
     C = np.where(C == 0, 0x20, C)
@@ -296,15 +298,15 @@
 def matrix_to_stars(M):
     I, J = M.shape
     C = 0x20*np.ones((I, 2*J + 1), dtype=int)
     C[:, 1:-1:2] += 0xA*M
     return C
 
 
-def bars(x, names=None, width=COLS, show_zero=True):
+def bars(x, names=None, width=config.cols, show_zero=True):
     # Get the name space.
     name_space = 0
     if names is not None:
         lens = [len(s) for s in names]
         name_space = max(lens)
 
     # Adjust the total width to make room for names.
@@ -341,15 +343,15 @@
     # Scale the matrix.
     m_min = np.min(matrix)
     m_max = np.max(matrix)
     M = np.round((matrix - m_min)/(m_max - m_min)*23).astype(int) + 232
     rows, cols = M.shape
 
     # Print the matrix.
-    if UNI:
+    if config.uni:
         for row in range(0, (rows - rows%2), 2):
             for col in range(cols):
                 print("\x1b[38;5;%dm\x1b[48;5;%dm\u2580" %
                         (M[row, col], M[row + 1, col]), end="")
             print("\x1b[39m\x1b[49m")
         if rows % 2 == 1:
             for col in range(cols):
@@ -550,15 +552,15 @@
 
 
 def sparsity(matrix, label=''):
     # Convert matrix to zeros and ones.
     M = (np.abs(matrix) > 1e-30).astype(int)
 
     # Convert the large matrix to a smaller matrix of character values.
-    C = matrix_to_braille(M) if UNI else matrix_to_stars(M)
+    C = matrix_to_braille(M) if config.uni else matrix_to_stars(M)
 
     # Create the shape string.
     shape_str = f"{matrix.shape[0]}x{matrix.shape[1]}"
 
     # Draw the plot.
     draw_graph(C, shape_str, label)
 
@@ -590,20 +592,20 @@
         displayed. If left as None, no time will be shown. When the progress bar
         completes, the total duration will be shown.
     width : int, default None
         Width of the full string, including the percent complete, the bar, and
         the clock. If not given, the width of the terminal window will be used.
     """
 
-    # Default the width to the terminal width or COLS.
+    # Default the width to the terminal width or config.cols.
     if width is None:
         try: # Try to get the true size.
             width, _ = os.get_terminal_size()
         except: # If getting terminal size fails, use default values.
-            width = COLS
+            width = config.cols
 
     # Get the ratio.
     ratio = (k + 1)/K
 
     # Get the clock string.
     if tic is not None:
         t_elapsed = time.perf_counter() - tic
```

### Comparing `trm_woodburn-0.0.4/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.5/src/trm_woodburn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -68,15 +68,16 @@
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
 default to `20` rows and `60` columns.
 
 By default, this library will use Unicode symbols (specifically braille) for
 plotting. A good font to use for this is JuliaMono. However, if your font does
 not support the necessary Unicode symbols, you can tell the library to not use
-them by setting `trm.UNI` to `False` before calling the `trm.plot` function.
+them by setting `trm.config.uni` to `False` before calling the `trm.plot`
+function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
@@ -107,16 +108,17 @@
 
 ```python
 trm.heat(matrix)
 ```
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
-value. If `trm.UNI` is `True`, half-block characters from the Unicode table will
-be used. If it is `False`, two spaces per element of the matrix will be used.
+value. If `trm.config.uni` is `True`, half-block characters from the Unicode
+table will be used. If it is `False`, two spaces per element of the matrix will
+be used.
 
 | With Unicode      | Without Unicode     |
 | ----------------- | ------------------- |
 | ![][fig_heat_uni] | ![][fig_heat_ascii] |
 
 ## Tables
```

