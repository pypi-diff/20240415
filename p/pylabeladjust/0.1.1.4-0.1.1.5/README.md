# Comparing `tmp/pylabeladjust-0.1.1.4.tar.gz` & `tmp/pylabeladjust-0.1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylabeladjust-0.1.1.4.tar", max compression
+gzip compressed data, was "pylabeladjust-0.1.1.5.tar", max compression
```

## Comparing `pylabeladjust-0.1.1.4.tar` & `pylabeladjust-0.1.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.4/LICENSE
--rw-r--r--   0        0        0     4068 2024-04-15 20:12:09.148350 pylabeladjust-0.1.1.4/README.md
--rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.4/pylabeladjust/__init__.py
--rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.4/pylabeladjust/core.py
--rw-r--r--   0        0        0      435 2024-04-15 20:11:57.734059 pylabeladjust-0.1.1.4/pyproject.toml
--rw-r--r--   0        0        0     4706 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 15:51:27.765165 pylabeladjust-0.1.1.5/LICENSE
+-rw-r--r--   0        0        0     4062 2024-04-15 20:16:05.213135 pylabeladjust-0.1.1.5/README.md
+-rw-r--r--   0        0        0       61 2024-04-15 12:28:42.751523 pylabeladjust-0.1.1.5/pylabeladjust/__init__.py
+-rw-r--r--   0        0        0    11855 2024-04-13 01:41:05.089290 pylabeladjust-0.1.1.5/pylabeladjust/core.py
+-rw-r--r--   0        0        0      435 2024-04-15 20:16:13.592486 pylabeladjust-0.1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     4700 1970-01-01 00:00:00.000000 pylabeladjust-0.1.1.5/PKG-INFO
```

### Comparing `pylabeladjust-0.1.1.4/LICENSE` & `pylabeladjust-0.1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.4/README.md` & `pylabeladjust-0.1.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylabeladjust
 
 `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python. It makes labels in matplotlib-plots not overlap by carefully pushing them apart, as illustrated by this video:
 
-<img src="https://raw.githubusercontent.com/jupyterlab/jupyterlab-git/v0.21.1/docs/figs/demo-0-10-0.gif" width="672" />
+<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/images/layout_process_texts.gif" width="672" />
 
 Pylabeladjust uses `pyqtree` in the background to be efficient. The setup of the `pylabeladjust`-plotting code takes inspiration from `adjust_text`. this package
 
 # When to use `pylabeladjust`
 
 `pylabeladjust` currently is meant for cases in which it is fine for your labels to move a little bit as in network-graphics or UMAP/t-SNE-plots, without any additional constraints. It should be able to handle cases where you have large numbers (1000+) of labels with a lot of overlap in reasonably small amounts of time. This makes it an alternative to `adjust_text` for this specific use-case, which in my experience struggles with many-abel/large overlap scenarios. If you need your labels to conform to more complicated constraints, like not overlapping particular points you might want to look into `adjust_text` and ... , which both can be very useful!
```

### Comparing `pylabeladjust-0.1.1.4/pylabeladjust/core.py` & `pylabeladjust-0.1.1.5/pylabeladjust/core.py`

 * *Files identical despite different names*

### Comparing `pylabeladjust-0.1.1.4/PKG-INFO` & `pylabeladjust-0.1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylabeladjust
-Version: 0.1.1.4
+Version: 0.1.1.5
 Summary: `pylabeladjust` is a port of Gephi's Label-Adjust algorithm to python.
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
 
-<img src="https://raw.githubusercontent.com/jupyterlab/jupyterlab-git/v0.21.1/docs/figs/demo-0-10-0.gif" width="672" />
+<img src="https://raw.githubusercontent.com/MNoichl/pylabeladjust/images/layout_process_texts.gif" width="672" />
 
 Pylabeladjust uses `pyqtree` in the background to be efficient. The setup of the `pylabeladjust`-plotting code takes inspiration from `adjust_text`. this package
 
 # When to use `pylabeladjust`
 
 `pylabeladjust` currently is meant for cases in which it is fine for your labels to move a little bit as in network-graphics or UMAP/t-SNE-plots, without any additional constraints. It should be able to handle cases where you have large numbers (1000+) of labels with a lot of overlap in reasonably small amounts of time. This makes it an alternative to `adjust_text` for this specific use-case, which in my experience struggles with many-abel/large overlap scenarios. If you need your labels to conform to more complicated constraints, like not overlapping particular points you might want to look into `adjust_text` and ... , which both can be very useful!
```

