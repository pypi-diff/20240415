# Comparing `tmp/matplotlib-inline-0.1.6.tar.gz` & `tmp/matplotlib_inline-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib-inline-0.1.6.tar", last modified: Thu Aug 18 03:47:05 2022, max compression
+gzip compressed data, was "matplotlib_inline-0.1.7.tar", last modified: Mon Apr 15 13:44:27 2024, max compression
```

## Comparing `matplotlib-inline-0.1.6.tar` & `matplotlib_inline-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 fperez   (33212) staff       (20)        0 2022-08-18 03:47:05.679935 matplotlib-inline-0.1.6/
--rw-r--r--   0 fperez   (33212) staff       (20)     1538 2022-08-16 20:04:52.000000 matplotlib-inline-0.1.6/LICENSE
--rw-r--r--   0 fperez   (33212) staff       (20)     2816 2022-08-18 03:47:05.679983 matplotlib-inline-0.1.6/PKG-INFO
--rw-r--r--   0 fperez   (33212) staff       (20)      892 2022-08-16 20:04:52.000000 matplotlib-inline-0.1.6/README.md
-drwxr-xr-x   0 fperez   (33212) staff       (20)        0 2022-08-18 03:47:05.678964 matplotlib-inline-0.1.6/matplotlib_inline/
--rw-r--r--   0 fperez   (33212) staff       (20)       75 2022-08-18 03:43:57.000000 matplotlib-inline-0.1.6/matplotlib_inline/__init__.py
--rw-r--r--   0 fperez   (33212) staff       (20)    11311 2022-08-18 03:09:32.000000 matplotlib-inline-0.1.6/matplotlib_inline/backend_inline.py
--rw-r--r--   0 fperez   (33212) staff       (20)     3911 2022-08-16 19:54:04.000000 matplotlib-inline-0.1.6/matplotlib_inline/config.py
-drwxr-xr-x   0 fperez   (33212) staff       (20)        0 2022-08-18 03:47:05.679832 matplotlib-inline-0.1.6/matplotlib_inline.egg-info/
--rw-r--r--   0 fperez   (33212) staff       (20)     2816 2022-08-18 03:47:05.000000 matplotlib-inline-0.1.6/matplotlib_inline.egg-info/PKG-INFO
--rw-r--r--   0 fperez   (33212) staff       (20)      334 2022-08-18 03:47:05.000000 matplotlib-inline-0.1.6/matplotlib_inline.egg-info/SOURCES.txt
--rw-r--r--   0 fperez   (33212) staff       (20)        1 2022-08-18 03:47:05.000000 matplotlib-inline-0.1.6/matplotlib_inline.egg-info/dependency_links.txt
--rw-r--r--   0 fperez   (33212) staff       (20)       10 2022-08-18 03:47:05.000000 matplotlib-inline-0.1.6/matplotlib_inline.egg-info/requires.txt
--rw-r--r--   0 fperez   (33212) staff       (20)       18 2022-08-18 03:47:05.000000 matplotlib-inline-0.1.6/matplotlib_inline.egg-info/top_level.txt
--rw-r--r--   0 fperez   (33212) staff       (20)     1060 2022-08-18 03:47:05.680220 matplotlib-inline-0.1.6/setup.cfg
--rw-r--r--   0 fperez   (33212) staff       (20)       38 2022-05-12 21:12:29.000000 matplotlib-inline-0.1.6/setup.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-04-15 13:44:27.718683 matplotlib_inline-0.1.7/
+-rw-r--r--   0 martin    (1000) martin    (1000)     1538 2024-04-15 13:37:56.000000 matplotlib_inline-0.1.7/LICENSE
+-rw-r--r--   0 martin    (1000) martin    (1000)     3873 2024-04-15 13:44:27.718683 matplotlib_inline-0.1.7/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      892 2024-04-15 13:37:56.000000 matplotlib_inline-0.1.7/README.md
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-04-15 13:44:27.717683 matplotlib_inline-0.1.7/matplotlib_inline/
+-rw-r--r--   0 martin    (1000) martin    (1000)       75 2024-04-15 13:39:33.000000 matplotlib_inline-0.1.7/matplotlib_inline/__init__.py
+-rw-r--r--   0 martin    (1000) martin    (1000)    11354 2024-04-15 13:37:56.000000 matplotlib_inline-0.1.7/matplotlib_inline/backend_inline.py
+-rw-r--r--   0 martin    (1000) martin    (1000)     3911 2024-04-15 13:37:56.000000 matplotlib_inline-0.1.7/matplotlib_inline/config.py
+drwxr-xr-x   0 martin    (1000) martin    (1000)        0 2024-04-15 13:44:27.718683 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/
+-rw-r--r--   0 martin    (1000) martin    (1000)     3873 2024-04-15 13:44:27.000000 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/PKG-INFO
+-rw-r--r--   0 martin    (1000) martin    (1000)      383 2024-04-15 13:44:27.000000 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/SOURCES.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)        1 2024-04-15 13:44:27.000000 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/dependency_links.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       63 2024-04-15 13:44:27.000000 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/entry_points.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       10 2024-04-15 13:44:27.000000 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/requires.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)       18 2024-04-15 13:44:27.000000 matplotlib_inline-0.1.7/matplotlib_inline.egg-info/top_level.txt
+-rw-r--r--   0 martin    (1000) martin    (1000)     1446 2024-04-15 13:37:56.000000 matplotlib_inline-0.1.7/pyproject.toml
+-rw-r--r--   0 martin    (1000) martin    (1000)       38 2024-04-15 13:44:27.718683 matplotlib_inline-0.1.7/setup.cfg
+-rw-r--r--   0 martin    (1000) martin    (1000)       92 2024-04-15 13:37:56.000000 matplotlib_inline-0.1.7/setup.py
```

### Comparing `matplotlib-inline-0.1.6/LICENSE` & `matplotlib_inline-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib-inline-0.1.6/README.md` & `matplotlib_inline-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib-inline-0.1.6/matplotlib_inline/backend_inline.py` & `matplotlib_inline-0.1.7/matplotlib_inline/backend_inline.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
     # done with access to the real shell object.
 
     cfg = InlineBackend.instance(parent=shell)
     cfg.shell = shell
     if cfg not in shell.configurables:
         shell.configurables.append(cfg)
 
-    if backend == 'module://matplotlib_inline.backend_inline':
+    if backend in ('inline', 'module://matplotlib_inline.backend_inline'):
         shell.events.register('post_execute', flush_figures)
 
         # Save rcParams that will be overwrittern
         shell._saved_rcParams = {}
         for k in cfg.rc:
             shell._saved_rcParams[k] = matplotlib.rcParams[k]
         # load inline_rc
@@ -207,15 +207,15 @@
 
 
 def _enable_matplotlib_integration():
     """Enable extra IPython matplotlib integration when we are loaded as the matplotlib backend."""
     from matplotlib import get_backend
     ip = get_ipython()
     backend = get_backend()
-    if ip and backend == 'module://%s' % __name__:
+    if ip and backend in ('inline', 'module://matplotlib_inline.backend_inline'):
         from IPython.core.pylabtools import activate_matplotlib
         try:
             activate_matplotlib(backend)
             configure_inline_support(ip, backend)
         except (ImportError, AttributeError):
             # bugs may cause a circular import on Python 2
             def configure_once(*args):
```

### Comparing `matplotlib-inline-0.1.6/matplotlib_inline/config.py` & `matplotlib_inline-0.1.7/matplotlib_inline/config.py`

 * *Files identical despite different names*

