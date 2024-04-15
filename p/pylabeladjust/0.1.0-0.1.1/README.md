# Comparing `tmp/pylabeladjust-0.1.0.tar.gz` & `tmp/pylabeladjust-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabeladjust-0.1.0.tar", max compression
+gzip compressed data, was "pylabeladjust-0.1.1.tar", max compression
```

## Comparing `pylabeladjust-0.1.0.tar` & `pylabeladjust-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.0/LICENSE
--rw-r--r--   0        0        0     4006 2024-04-15 16:28:45.152677 pylabeladjust-0.1.0/README.md
--rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.0/pylabeladjust/__init__.py
--rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.0/pylabeladjust/core.py
--rw-r--r--   0        0        0      497 2024-04-15 15:46:10.539550 pylabeladjust-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4705 1970-01-01 00:00:00.000000 pylabeladjust-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4066 2024-04-15 19:37:51.092758 pylabeladjust-0.1.1/README.md
+-rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1/pylabeladjust/__init__.py
+-rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1/pylabeladjust/core.py
+-rw-r--r--   0        0        0      496 2024-04-15 19:40:34.976325 pylabeladjust-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4765 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1/PKG-INFO
```

### Comparing `pylabeladjust-0.1.0/LICENSE` & `pylabeladjust-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.0/README.md` & `pylabeladjust-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylabeladjust
 
 `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python. It makes labels in matplotlib-plots not overlap by carefully pushing them apart, as illustrated by this video:
 
-<img src="images/layout_process_texts.gif" width="672" />
+<img src="https://github.com/MNoichl/pylabeladjust/blob/main/images/layout_process_texts.gif?raw=true" width="672" />
 
 Pylabeladjust uses `pyqtree` in the background to be efficient. The setup of the `pylabeladjust`-plotting code takes inspiration from `adjust_text`. this package
 
 # When to use `pylabeladjust`
 
 `pylabeladjust` currently is meant for cases in which it is fine for your labels to move a little bit as in network-graphics or UMAP/t-SNE-plots, without any additional constraints. It should be able to handle cases where you have large numbers (1000+) of labels with a lot of overlap in reasonably small amounts of time. This makes it an alternative to `adjust_text` for this specific use-case, which in my experience struggles with many-abel/large overlap scenarios. If you need your labels to conform to more complicated constraints, like not overlapping particular points you might want to look into `adjust_text` and ... , which both can be very useful!
```

### Comparing `pylabeladjust-0.1.0/pylabeladjust/core.py` & `pylabeladjust-0.1.1/pylabeladjust/core.py`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.0/PKG-INFO` & `pylabeladjust-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylabeladjust
-Version: 0.1.0
+Version: 0.1.1
 Summary: `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python. It makes labels in matplotlib-plots not overlap by carefully p
 License: MIT
 Author: MNoichl
 Author-email: noichlmax@hotmail.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pylabeladjust
 
 `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python. It makes labels in matplotlib-plots not overlap by carefully pushing them apart, as illustrated by this video:
 
-<img src="images/layout_process_texts.gif" width="672" />
+<img src="https://github.com/MNoichl/pylabeladjust/blob/main/images/layout_process_texts.gif?raw=true" width="672" />
 
 Pylabeladjust uses `pyqtree` in the background to be efficient. The setup of the `pylabeladjust`-plotting code takes inspiration from `adjust_text`. this package
 
 # When to use `pylabeladjust`
 
 `pylabeladjust` currently is meant for cases in which it is fine for your labels to move a little bit as in network-graphics or UMAP/t-SNE-plots, without any additional constraints. It should be able to handle cases where you have large numbers (1000+) of labels with a lot of overlap in reasonably small amounts of time. This makes it an alternative to `adjust_text` for this specific use-case, which in my experience struggles with many-abel/large overlap scenarios. If you need your labels to conform to more complicated constraints, like not overlapping particular points you might want to look into `adjust_text` and ... , which both can be very useful!
```

