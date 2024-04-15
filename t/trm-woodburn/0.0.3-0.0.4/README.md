# Comparing `tmp/trm_woodburn-0.0.3.tar.gz` & `tmp/trm_woodburn-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trm_woodburn-0.0.3.tar", last modified: Mon Apr 15 19:39:02 2024, max compression
+gzip compressed data, was "trm_woodburn-0.0.4.tar", last modified: Mon Apr 15 21:14:05 2024, max compression
```

## Comparing `trm_woodburn-0.0.3.tar` & `trm_woodburn-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.920315 trm_woodburn-0.0.3/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.3/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:39:02.920260 trm_woodburn-0.0.3/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5046 2024-04-15 19:17:04.000000 trm_woodburn-0.0.3/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.3/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 19:39:02.920531 trm_woodburn-0.0.3/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.918654 trm_woodburn-0.0.3/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.919343 trm_woodburn-0.0.3/src/trm/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.3/src/trm/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19700 2024-04-15 19:37:21.000000 trm_woodburn-0.0.3/src/trm/trm.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 19:39:02.920089 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     5525 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 19:39:02.000000 trm_woodburn-0.0.3/src/trm_woodburn.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.055902 trm_woodburn-0.0.4/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1054 2024-04-15 16:11:57.000000 trm_woodburn-0.0.4/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6951 2024-04-15 21:14:05.055853 trm_woodburn-0.0.4/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6472 2024-04-15 21:13:40.000000 trm_woodburn-0.0.4/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 trm_woodburn-0.0.4/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      601 2024-04-15 21:14:05.056118 trm_woodburn-0.0.4/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.054068 trm_woodburn-0.0.4/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.054902 trm_woodburn-0.0.4/src/trm/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2024-04-15 19:15:58.000000 trm_woodburn-0.0.4/src/trm/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    19700 2024-04-15 19:37:21.000000 trm_woodburn-0.0.4/src/trm/trm.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-04-15 21:14:05.055686 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     6951 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      280 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-04-15 21:14:05.000000 trm_woodburn-0.0.4/src/trm_woodburn.egg-info/top_level.txt
```

### Comparing `trm_woodburn-0.0.3/LICENSE.txt` & `trm_woodburn-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.3/PKG-INFO` & `trm_woodburn-0.0.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,8 @@
-Metadata-Version: 2.1
-Name: trm-woodburn
-Version: 0.0.3
-Summary: A library for pretty printing to the terminal
-Home-page: https://gitlab.com/davidwoodburn/trm
-Author: David Woodburn
-Author-email: david.woodburn@icloud.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: numpy
-
-# Console Information Explorer
+# Terminal Utilities
 
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
@@ -31,15 +16,15 @@
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do you work in the
 terminal the better.
 
 ## Plots
 
 ```python
-trm.plot(x, y=None, label='', cols=1, rows=1)
+trm.plot(x, y=None, label='', rows=1, cols=1)
 ```
 
 The plot function will render all the data points defined by `x` and `y` to the
 terminal. The inputs `x` and `y` can be vectors or matrices. If they are
 matrices, each row is treated as a separate curve.
 
 The shapes of `x` and `y` do not have to be the same, but they must be
@@ -56,75 +41,105 @@
 (0:99, -1.5:1.5)
 ```
 
 means that `x` ranges from `0` to `99` and `y` ranges from `-1.5` to `1.5`.
 
 If a `label` is given, this will be printed in the bottom right of the plot box.
 
-The `cols` and `rows` parameters let you specify the number of terminal text
-columns and rows to use for the plot, respectively. For each of these, if the
+The `rows` and `cols` parameters let you specify the number of terminal text
+rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
-to use. For example, if `cols` is `0.5`, then half the number of columns of the
+to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
-default to `60` columns and `20` rows.
+default to `20` rows and `60` columns.
 
-By default, this library will use unicode symbols (specifically braille) for
+By default, this library will use Unicode symbols (specifically braille) for
 plotting. A good font to use for this is JuliaMono. However, if your font does
-not support the necessary unicode symbols, you can tell the library to not use
+not support the necessary Unicode symbols, you can tell the library to not use
 them by setting `trm.UNI` to `False` before calling the `trm.plot` function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![][fig_plot_1] | ![][fig_plot_5] |
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
 values. The `labels` input is a list of strings corresponding to the labels to
 print before the bar of each value in `x`. The `width` input is the total width
 of characters including the labels.
 
+```
+ apples |=========                                         |
+oranges |=========================================         |
+bananas |==================================================|
+  pears |====================                              |
+ grapes |============================                      |
+```
+
 ## Heat maps
 
 ```python
 trm.heat(matrix)
 ```
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
-value. If `trm.UNI` is `True`, half-block characters from the unicode table will
+value. If `trm.UNI` is `True`, half-block characters from the Unicode table will
 be used. If it is `False`, two spaces per element of the matrix will be used.
 
+| With Unicode      | Without Unicode     |
+| ----------------- | ------------------- |
+| ![][fig_heat_uni] | ![][fig_heat_ascii] |
+
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
 inputs are lists of header and left-most column labels, respectively, to print
 around the `matrix`.
 
+```
+           |      Set 1       Set 2       Set 3
+---------- | ----------  ----------  ----------
+    apples | 0.65802165  0.20015677  0.51074794
+   bananas | 0.42184098  0.46774988  0.39589918
+     pears | 0.79159879  0.89324181  0.57347394
+   oranges | 0.25932644  0.29973433  0.90646047
+    grapes |  0.2751687  0.40117769  0.58233234
+```
+
 ## Sparsity
 
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
+| With Unicode          | Without Unicode         |
+| --------------------- | ----------------------- |
+| ![][fig_sparsity_uni] | ![][fig_sparsity_ascii] |
+
 ## Progress bars
 
 ```python
 trm.progress(k, K, tic=None, width=None)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
@@ -133,7 +148,20 @@
 one-page function. The `k` input is the counter of whatever for loop the
 progress bar is reporting on. The `K` input is one greater than the largest
 possible value of `k`, as in `for k in range(K):`. If `tic` is provided, the
 estimated time remaining to complete the process based on the initial time
 stored in `tic` will be displayed. When the process is completed, the total
 elapsed time since `tic` will be displayed. If `width` is not provided, the full
 width of the current terminal window will be used.
+
+```
+ 44% [/////////////////////----------------------------] -00:00:02.1
+```
+
+
+[fig_heat_uni]: figures/fig_heat_uni.png
+[fig_heat_ascii]: figures/fig_heat_ascii.png
+[fig_plot]: figures/fig_plot.png
+[fig_plot_1]: figures/fig_plot_1.png
+[fig_plot_5]: figures/fig_plot_5.png
+[fig_sparsity_uni]: figures/fig_sparsity_uni.png
+[fig_sparsity_ascii]: figures/fig_sparsity_ascii.png
```

### Comparing `trm_woodburn-0.0.3/setup.cfg` & `trm_woodburn-0.0.4/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trm-woodburn
-version = 0.0.3
+version = 0.0.4
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for pretty printing to the terminal
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/trm
 classifiers =
```

### Comparing `trm_woodburn-0.0.3/src/trm/trm.py` & `trm_woodburn-0.0.4/src/trm/trm.py`

 * *Files identical despite different names*

### Comparing `trm_woodburn-0.0.3/src/trm_woodburn.egg-info/PKG-INFO` & `trm_woodburn-0.0.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: trm-woodburn
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for pretty printing to the terminal
 Home-page: https://gitlab.com/davidwoodburn/trm
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 
-# Console Information Explorer
+# Terminal Utilities
 
 This library provides several functions for nicely printing data to the
 terminal. MatPlotLib is a very nice library, but it can be a bit tedious at
 times when all you want is something quick and dirty.
 
 -   Every separate plot needs to be introduced with a `plt.figure()` statement.
 -   Large sets of data can be slow to render.
@@ -31,15 +31,15 @@
 These are all excuses to use this library. But, the biggest reason to use this
 library is that the terminal is cool, and the more you can do you work in the
 terminal the better.
 
 ## Plots
 
 ```python
-trm.plot(x, y=None, label='', cols=1, rows=1)
+trm.plot(x, y=None, label='', rows=1, cols=1)
 ```
 
 The plot function will render all the data points defined by `x` and `y` to the
 terminal. The inputs `x` and `y` can be vectors or matrices. If they are
 matrices, each row is treated as a separate curve.
 
 The shapes of `x` and `y` do not have to be the same, but they must be
@@ -56,75 +56,105 @@
 (0:99, -1.5:1.5)
 ```
 
 means that `x` ranges from `0` to `99` and `y` ranges from `-1.5` to `1.5`.
 
 If a `label` is given, this will be printed in the bottom right of the plot box.
 
-The `cols` and `rows` parameters let you specify the number of terminal text
-columns and rows to use for the plot, respectively. For each of these, if the
+The `rows` and `cols` parameters let you specify the number of terminal text
+rows and columns to use for the plot, respectively. For each of these, if the
 value is less than or equal to 1, it represents a portion of the available space
-to use. For example, if `cols` is `0.5`, then half the number of columns of the
+to use. For example, if `rows` is `0.5`, then half the number of rows of the
 current terminal window will be used for the plot. If the value is greater than
 1, it represents the absolute number of columns or rows to use. Also, if the
 size of the current terminal cannot be obtained, the available space will
-default to `60` columns and `20` rows.
+default to `20` rows and `60` columns.
 
-By default, this library will use unicode symbols (specifically braille) for
+By default, this library will use Unicode symbols (specifically braille) for
 plotting. A good font to use for this is JuliaMono. However, if your font does
-not support the necessary unicode symbols, you can tell the library to not use
+not support the necessary Unicode symbols, you can tell the library to not use
 them by setting `trm.UNI` to `False` before calling the `trm.plot` function.
 
 If only one curve is being plotted, the characters will be written in whatever
 the default font color is set to in your terminal. If more than one curve is
 plotted, color will be used. The color map is blue, green, yellow, red, and
 magenta. If you have more than 5 curves (This is just a terminal-based plot; why
 would you do that?), then the colors will recyle.
 
+| Single curve    | Multiple curves |
+| --------------- | --------------- |
+| ![][fig_plot_1] | ![][fig_plot_5] |
+
 ## Bars
 
 ```python
 trm.bars(x, labels=None, width=COLS, show_zero=True)
 ```
 
 It can be convenient to plot a simple bar graph. The `x` input is the vector of
 values. The `labels` input is a list of strings corresponding to the labels to
 print before the bar of each value in `x`. The `width` input is the total width
 of characters including the labels.
 
+```
+ apples |=========                                         |
+oranges |=========================================         |
+bananas |==================================================|
+  pears |====================                              |
+ grapes |============================                      |
+```
+
 ## Heat maps
 
 ```python
 trm.heat(matrix)
 ```
 
 The `heat` function will generate a heat map of the `matrix` input using 24
 shades of gray. Black is used for the lowest value and white for the highest
-value. If `trm.UNI` is `True`, half-block characters from the unicode table will
+value. If `trm.UNI` is `True`, half-block characters from the Unicode table will
 be used. If it is `False`, two spaces per element of the matrix will be used.
 
+| With Unicode      | Without Unicode     |
+| ----------------- | ------------------- |
+| ![][fig_heat_uni] | ![][fig_heat_ascii] |
+
 ## Tables
 
 ```python
 trm.table(matrix, head=None, left=None, width=10, sep='  ')
 ```
 
 You can print a nicely spaced table of the `matrix` data. The `head` and `left`
 inputs are lists of header and left-most column labels, respectively, to print
 around the `matrix`.
 
+```
+           |      Set 1       Set 2       Set 3
+---------- | ----------  ----------  ----------
+    apples | 0.65802165  0.20015677  0.51074794
+   bananas | 0.42184098  0.46774988  0.39589918
+     pears | 0.79159879  0.89324181  0.57347394
+   oranges | 0.25932644  0.29973433  0.90646047
+    grapes |  0.2751687  0.40117769  0.58233234
+```
+
 ## Sparsity
 
 ```python
 trm.sparsity(matrix, label='')
 ```
 
 If all you want to see is the sparsity of a matrix, use this function. The
 `label` input will be placed in the bottom-right corner of the render.
 
+| With Unicode          | Without Unicode         |
+| --------------------- | ----------------------- |
+| ![][fig_sparsity_uni] | ![][fig_sparsity_ascii] |
+
 ## Progress bars
 
 ```python
 trm.progress(k, K, tic=None, width=None)
 ```
 
 There are many progress bar libraries available for Python. But, many of them
@@ -133,7 +163,20 @@
 one-page function. The `k` input is the counter of whatever for loop the
 progress bar is reporting on. The `K` input is one greater than the largest
 possible value of `k`, as in `for k in range(K):`. If `tic` is provided, the
 estimated time remaining to complete the process based on the initial time
 stored in `tic` will be displayed. When the process is completed, the total
 elapsed time since `tic` will be displayed. If `width` is not provided, the full
 width of the current terminal window will be used.
+
+```
+ 44% [/////////////////////----------------------------] -00:00:02.1
+```
+
+
+[fig_heat_uni]: figures/fig_heat_uni.png
+[fig_heat_ascii]: figures/fig_heat_ascii.png
+[fig_plot]: figures/fig_plot.png
+[fig_plot_1]: figures/fig_plot_1.png
+[fig_plot_5]: figures/fig_plot_5.png
+[fig_sparsity_uni]: figures/fig_sparsity_uni.png
+[fig_sparsity_ascii]: figures/fig_sparsity_ascii.png
```

