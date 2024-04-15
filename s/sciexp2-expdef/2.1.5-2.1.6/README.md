# Comparing `tmp/sciexp2-expdef-2.1.5.tar.gz` & `tmp/sciexp2-expdef-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sciexp2-expdef-2.1.5.tar", last modified: Thu Apr 11 16:20:18 2024, max compression
+gzip compressed data, was "dist/sciexp2-expdef-2.1.6.tar", last modified: Mon Apr 15 15:57:13 2024, max compression
```

## Comparing `sciexp2-expdef-2.1.5.tar` & `sciexp2-expdef-2.1.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/.requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1682 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/system/
--rw-rw-rw-   0 root         (0) root         (0)     2356 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/system/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     9636 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/system/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4277 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/system/gridengine.py
--rw-rw-rw-   0 root         (0) root         (0)    53094 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/experiments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates/
--rwxrwxrwx   0 root         (0) root         (0)     5070 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates/gridengine.tpl
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates/gridengine.dsc
--rwxrwxrwx   0 root         (0) root         (0)     2687 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates/shell.tpl
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates/shell.dsc
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates/dacupc-gridengine.dsc
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11349 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/launcher.py
--rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/templates.py
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/expdef/env.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2/common/
--rw-rw-rw-   0 root         (0) root         (0)    14817 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/text.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16498 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    14779 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/progress.py
--rw-rw-rw-   0 root         (0) root         (0)     4835 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/pp.py
--rw-rw-rw-   0 root         (0) root         (0)    24868 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/sciexp2/common/instance.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-04-11 16:20:18.000000 sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)    12314 2024-04-11 16:19:59.000000 sciexp2-expdef-2.1.5/launcher
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/.requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/system/
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/system/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     9636 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/system/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4277 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/system/gridengine.py
+-rw-rw-rw-   0 root         (0) root         (0)    53894 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/experiments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates/
+-rwxrwxrwx   0 root         (0) root         (0)     5070 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates/gridengine.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates/gridengine.dsc
+-rwxrwxrwx   0 root         (0) root         (0)     2687 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates/shell.tpl
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates/shell.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates/dacupc-gridengine.dsc
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11349 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/launcher.py
+-rw-rw-rw-   0 root         (0) root         (0)    12015 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/templates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/expdef/env.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2/common/
+-rw-rw-rw-   0 root         (0) root         (0)    14817 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/text.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16498 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    14779 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/progress.py
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/pp.py
+-rw-rw-rw-   0 root         (0) root         (0)    24868 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/sciexp2/common/instance.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-15 15:57:12.000000 sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-15 15:57:13.000000 sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-15 15:57:12.000000 sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-15 15:57:12.000000 sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-15 15:57:12.000000 sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)    12314 2024-04-15 15:56:53.000000 sciexp2-expdef-2.1.6/launcher
```

### Comparing `sciexp2-expdef-2.1.5/PKG-INFO` & `sciexp2-expdef-2.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciexp2-expdef
-Version: 2.1.5
+Version: 2.1.6
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sciexp2-expdef-2.1.5/LICENSE` & `sciexp2-expdef-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/setup.py` & `sciexp2-expdef-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/README.md` & `sciexp2-expdef-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/system/shell.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/system/shell.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/system/__init__.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/system/__init__.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/system/gridengine.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/system/gridengine.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/experiments.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/experiments.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,59 +447,81 @@
 
 def _do_generate(experiments, template_from, template_to,
                  pre_exp_fun, post_exp_fun, parallel):
     out = os.path.abspath(utils.get_path(experiments.out))
     translate_from = text.Translator(template_from)
     translate_to = text.Translator(template_to)
 
-    done_first = {}
-    done_exp = {}
+    done_set_lock = threading.Lock()
+    done_set = {}
+    class done_state:
+        def __init__(self):
+            self.lock = threading.Lock()
+            self.is_first = True
+            self.is_second = False
+            self.first_exp = None
+        def set_first(self, exp):
+            with self.lock:
+                is_first = self.is_first
+                if is_first:
+                    self.is_first = False
+                    self.first_exp = exp
+                    is_second = True
+                else:
+                    is_second = False
+            return is_first, is_second
+    def get_done(path_from, path_to):
+        key = (path_from, path_to)
+        with done_set_lock:
+            if key not in done_set:
+                done_set[key] = done_state()
+            return done_set[key]
 
     with progress.get(len(experiments), msg="generating files...") as progr:
 
         def generate_with_progress(exp):
             with exp.auto_translate():
                 _WithExp._EXPERIMENT = exp
                 _WithExpTpl._EXPERIMENT = exp
 
                 path_from = utils.get_path(translate_from.translate(exp))
                 path_to = utils.get_path(translate_to.translate(exp))
                 path_to = os.path.join(out, path_to)
 
-                done_idx = path_from + "+" + path_to
-                if done_idx in done_first:
-                    if done_first[done_idx]:
-                        done_first[done_idx] = False
-                        progress.info(
-                            "Skipping already generated file: %s -> %s",
-                            path_from, path_to)
-                    progress.verbose(
-                        "Conflicting experiments during generation:\n%s\n%s",
-                        done_exp[done_idx], exp)
+                done = get_done(path_from, path_to)
+                is_first, is_second = done.set_first(exp)
+                if not is_first:
+                    msg = f"Skipping already generated file: {path_from} -> {path_to}"
+                    msg += "\n"
+                    msg += f"Source file template: {template_from}"
+                    msg += "\n"
+                    msg += f"Destination file template: {template_to}"
+                    msg += "\n"
+                    msg += f"Conflicting experiments:\n{done.first_exp}\n{exp}"
+                    if is_second:
+                        progress.info(msg)
+                    else:
+                        progress.verbose(msg)
                 else:
-                    done_first[done_idx] = True
-                    done_exp[done_idx] = exp
-
-                    progress.debug("Generating: %s -> %s", path_from, path_to)
+                    progress.debug(f"Generating: {path_from} -> {path_to}")
 
                     exp, contents_to = pre_exp_fun(exp, path_from, path_to)
 
                     utils.assert_dir(os.path.dirname(path_to))
                     if os.path.isfile(path_to):
                         with open(path_to, "r") as f:
                             contents_to_old = f.read()
                     else:
                         contents_to_old = ""
+                        utils.get_file(path_to, "w")
+                    shutil.copymode(path_from, path_to)
 
                     if contents_to != contents_to_old:
                         with open(path_to, "w") as f:
                             f.write(contents_to)
-                    elif not os.path.isfile(path_to):
-                        utils.get_file(path_to, "w")
-                    shutil.copymode(path_from, path_to)
 
                     post_exp_fun(exp, path_to)
 
             progr()
 
         max_workers = get_executor_workers(parallel)
         with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
```

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/templates/gridengine.tpl` & `sciexp2-expdef-2.1.6/sciexp2/expdef/templates/gridengine.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/templates/gridengine.dsc` & `sciexp2-expdef-2.1.6/sciexp2/expdef/templates/gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/templates/shell.tpl` & `sciexp2-expdef-2.1.6/sciexp2/expdef/templates/shell.tpl`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/templates/dacupc-gridengine.dsc` & `sciexp2-expdef-2.1.6/sciexp2/expdef/templates/dacupc-gridengine.dsc`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/launcher.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/launcher.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/templates.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/templates.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/expdef/env.py` & `sciexp2-expdef-2.1.6/sciexp2/expdef/env.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/common/text.py` & `sciexp2-expdef-2.1.6/sciexp2/common/text.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/common/utils.py` & `sciexp2-expdef-2.1.6/sciexp2/common/utils.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/common/progress.py` & `sciexp2-expdef-2.1.6/sciexp2/common/progress.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/common/filter.py` & `sciexp2-expdef-2.1.6/sciexp2/common/filter.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/common/pp.py` & `sciexp2-expdef-2.1.6/sciexp2/common/pp.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2/common/instance.py` & `sciexp2-expdef-2.1.6/sciexp2/common/instance.py`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/PKG-INFO` & `sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sciexp2-expdef
-Version: 2.1.5
+Version: 2.1.6
 Summary: Experiment definition framework for SciExp²
 Home-page: https://sciexp2-expdef.readthedocs.io/
 Author: Lluís Vilanova
 Author-email: llvilanovag@gmail.com
 License: GNU General Public License (GPL) version 3 or later
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `sciexp2-expdef-2.1.5/sciexp2_expdef.egg-info/SOURCES.txt` & `sciexp2-expdef-2.1.6/sciexp2_expdef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sciexp2-expdef-2.1.5/launcher` & `sciexp2-expdef-2.1.6/launcher`

 * *Files identical despite different names*

