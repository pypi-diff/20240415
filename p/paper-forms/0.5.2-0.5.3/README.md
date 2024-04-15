# Comparing `tmp/paper-forms-0.5.2.tar.gz` & `tmp/paper_forms-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-forms-0.5.2.tar", last modified: Thu Jan  4 12:35:43 2024, max compression
+gzip compressed data, was "paper_forms-0.5.3.tar", last modified: Mon Apr 15 08:16:34 2024, max compression
```

## Comparing `paper-forms-0.5.2.tar` & `paper_forms-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 12:35:43.302449 paper-forms-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-01-04 12:35:38.000000 paper-forms-0.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-04 12:35:38.000000 paper-forms-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-01-04 12:35:38.000000 paper-forms-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-01-04 12:35:38.000000 paper-forms-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-01-04 12:35:43.302449 paper-forms-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-01-04 12:35:38.000000 paper-forms-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 12:35:43.302449 paper-forms-0.5.2/paper_forms/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/composer.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 12:35:43.302449 paper-forms-0.5.2/paper_forms/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/templatetags/paper_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-01-04 12:35:38.000000 paper-forms-0.5.2/paper_forms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-04 12:35:43.302449 paper-forms-0.5.2/paper_forms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-01-04 12:35:43.000000 paper-forms-0.5.2/paper_forms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-04 12:35:43.000000 paper-forms-0.5.2/paper_forms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 12:35:43.000000 paper-forms-0.5.2/paper_forms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-04 12:35:43.000000 paper-forms-0.5.2/paper_forms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-04 12:35:43.000000 paper-forms-0.5.2/paper_forms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-04 12:35:43.000000 paper-forms-0.5.2/paper_forms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-04 12:35:43.306449 paper-forms-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-01-04 12:35:38.000000 paper-forms-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:16:34.720162 paper_forms-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-15 08:16:29.000000 paper_forms-0.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-15 08:16:29.000000 paper_forms-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-15 08:16:29.000000 paper_forms-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-15 08:16:29.000000 paper_forms-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-04-15 08:16:34.720162 paper_forms-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17376 2024-04-15 08:16:29.000000 paper_forms-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:16:34.720162 paper_forms-0.5.3/paper_forms/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/composer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:16:34.720162 paper_forms-0.5.3/paper_forms/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/templatetags/paper_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-15 08:16:29.000000 paper_forms-0.5.3/paper_forms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:16:34.720162 paper_forms-0.5.3/paper_forms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-04-15 08:16:34.000000 paper_forms-0.5.3/paper_forms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-15 08:16:34.000000 paper_forms-0.5.3/paper_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:16:34.000000 paper_forms-0.5.3/paper_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:16:34.000000 paper_forms-0.5.3/paper_forms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 08:16:34.000000 paper_forms-0.5.3/paper_forms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 08:16:34.000000 paper_forms-0.5.3/paper_forms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-15 08:16:34.724162 paper_forms-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-15 08:16:29.000000 paper_forms-0.5.3/setup.py
```

### Comparing `paper-forms-0.5.2/CHANGELOG.md` & `paper_forms-0.5.3/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change Log
 
+## [0.5.3](https://github.com/dldevinc/paper-forms/tree/v0.5.3) - 2024-05-15
+
+### Bug Fixes
+
+-   Classes specified in error_css_class and required_css_class are added to the field 
+    regardless of whether the context variable css_classes is overridden.
+
 ## [0.5.2](https://github.com/dldevinc/paper-forms/tree/v0.5.2) - 2024-01-04
 
 ### Features
 
 -   Now, widgets set through the `Composer.widgets` attribute receive the correct values 
     for `is_required` and `is_localized`. Additionally, attributes added by the 
     `forms.Field.build_attrs()` method are included.
```

### Comparing `paper-forms-0.5.2/CONTRIBUTING.md` & `paper_forms-0.5.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paper-forms-0.5.2/LICENSE` & `paper_forms-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-forms-0.5.2/PKG-INFO` & `paper_forms-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-forms
-Version: 0.5.2
+Version: 0.5.3
 Summary: A form templating app for Django
 Home-page: https://github.com/dldevinc/paper-forms
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
```

### Comparing `paper-forms-0.5.2/README.md` & `paper_forms-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `paper-forms-0.5.2/paper_forms/boundfield.py` & `paper_forms-0.5.3/paper_forms/boundfield.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,17 @@
             help_text = self.composer.get_help_text(self.name, widget)
             if help_text is None:
                 help_text = self.help_text
             context["help_text"] = help_text
 
         if "css_classes" not in context:
             extra_css_classes = self.composer.get_css_classes(self.name, widget)
-            context["css_classes"] = self.css_classes(extra_css_classes)
+        else:
+            extra_css_classes = context["css_classes"]
+        context["css_classes"] = self.css_classes(extra_css_classes)
 
         context["errors"] = self.errors
 
         return context
 
     def css_classes(self, extra_classes=None):
         if hasattr(extra_classes, "split"):
```

### Comparing `paper-forms-0.5.2/paper_forms/composer.py` & `paper_forms-0.5.3/paper_forms/composer.py`

 * *Files identical despite different names*

### Comparing `paper-forms-0.5.2/paper_forms/templatetags/paper_forms.py` & `paper_forms-0.5.3/paper_forms/templatetags/paper_forms.py`

 * *Files identical despite different names*

### Comparing `paper-forms-0.5.2/paper_forms.egg-info/PKG-INFO` & `paper_forms-0.5.3/paper_forms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-forms
-Version: 0.5.2
+Version: 0.5.3
 Summary: A form templating app for Django
 Home-page: https://github.com/dldevinc/paper-forms
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
```

### Comparing `paper-forms-0.5.2/setup.cfg` & `paper_forms-0.5.3/setup.cfg`

 * *Files identical despite different names*

