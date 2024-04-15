# Comparing `tmp/sphinx_issues-4.0.0.tar.gz` & `tmp/sphinx_issues-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_issues-4.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_issues-4.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_issues-4.0.0.tar` & `sphinx_issues-4.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      382 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1052 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/LICENSE
--rw-r--r--   0        0        0     1442 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/NOTICE
--rw-r--r--   0        0        0     6820 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/README.rst
--rw-r--r--   0        0        0     1499 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/pyproject.toml
--rw-r--r--   0        0        0    12966 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/src/sphinx_issues/__init__.py
--rw-r--r--   0        0        0        0 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/tests/source/_static/.gitkeep
--rw-r--r--   0        0        0     2328 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/tests/source/conf.py
--rw-r--r--   0        0        0      141 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/tests/source/examples.rst
--rw-r--r--   0        0        0      140 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/tests/source/index.rst
--rw-r--r--   0        0        0    11532 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/tests/test_sphinx_issues.py
--rw-r--r--   0        0        0      340 2024-01-19 14:15:43.489468 sphinx_issues-4.0.0/tox.ini
--rw-r--r--   0        0        0     7960 1970-01-01 00:00:00.000000 sphinx_issues-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      382 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/LICENSE
+-rw-r--r--   0        0        0     1442 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/NOTICE
+-rw-r--r--   0        0        0     7199 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/README.rst
+-rw-r--r--   0        0        0     1499 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0    13598 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/src/sphinx_issues/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/tests/source/_static/.gitkeep
+-rw-r--r--   0        0        0     2328 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/tests/source/conf.py
+-rw-r--r--   0        0        0      141 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/tests/source/examples.rst
+-rw-r--r--   0        0        0      140 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/tests/source/index.rst
+-rw-r--r--   0        0        0    11723 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/tests/test_sphinx_issues.py
+-rw-r--r--   0        0        0      340 2024-04-15 03:03:45.371402 sphinx_issues-4.1.0/tox.ini
+-rw-r--r--   0        0        0     8339 1970-01-01 00:00:00.000000 sphinx_issues-4.1.0/PKG-INFO
```

### Comparing `sphinx_issues-4.0.0/LICENSE` & `sphinx_issues-4.1.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2024 Steven Loria
+Copyright Steven Loria and contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sphinx_issues-4.0.0/NOTICE` & `sphinx_issues-4.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `sphinx_issues-4.0.0/README.rst` & `sphinx_issues-4.1.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -131,28 +131,40 @@
 
 Use the ``:cwe:`` role to link to CWEs on https://cwe.mitre.org.
 
 .. code-block:: rst
 
     :cwe:`CWE-787` - The software writes data past the end, or...
 
+Use the ``:pypi:`` role to link to PyPI on https://pypi.org.
+
+.. code-block:: rst
+
+    :pypi:`sphinx-issues` - A Sphinx extension for linking to your project's issue tracker.
+
 Credits
 *******
 
 Credit goes to Jeff Forcier for his work on the `releases <https://github.com/bitprophet/releases>`_ extension, which is a full-featured solution for generating changelogs. I just needed a quick way to reference GitHub issues in my docs, so I yoinked the bits that I needed.
 
 License
 *******
 
 MIT licensed. See the bundled `LICENSE <https://github.com/sloria/sphinx-issues/blob/master/LICENSE>`_ file for more details.
 
 
 Changelog
 *********
 
+4.1.0 (2024-04-14)
+------------------
+
+- Add `:pypi:` role for linking to PyPI projects (`#144 <https://github.com/sloria/sphinx-issues/issues/144>`_).
+  Thanks @shenxianpeng for the suggestion and PR.
+
 4.0.0 (2024-01-19)
 ------------------
 
 - Default to linking GH Sponsors for the :user: role (`#129 <https://github.com/sloria/sphinx-issues/issues/129>`_).
   Thanks @webknjaz for the suggestion.
 - Support Python 3.8-3.12. Older versions are no longer supported.
 - *Backwards-incompatible*: Remove ``__version__``, ``__author__``, and ``__license__`` attributes.
```

### Comparing `sphinx_issues-4.0.0/pyproject.toml` & `sphinx_issues-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sphinx-issues"
-version = "4.0.0"
+version = "4.1.0"
 description = "A Sphinx extension for linking to your project's issue tracker"
 readme = "README.rst"
 license = { file = "LICENSE" }
 authors = [{ name = "Steven Loria", email = "sloria1@gmail.com" }]
 classifiers = [
   "Framework :: Sphinx :: Extension",
   "Intended Audience :: Developers",
```

### Comparing `sphinx_issues-4.0.0/src/sphinx_issues/__init__.py` & `sphinx_issues-4.1.0/src/sphinx_issues/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A Sphinx extension for linking to your project's issue tracker."""
+
 import importlib.metadata
 import re
 from typing import Callable, Optional, Tuple
 
 from docutils import nodes, utils
 from sphinx.config import Config
 from sphinx.util.nodes import split_explicit_title
@@ -181,14 +182,34 @@
     number = target[4:]
     ref = f"https://cwe.mitre.org/data/definitions/{number}.html"
     text = title if has_explicit_title else target
     link = nodes.reference(text=text, refuri=ref, **options)
     return [link], []
 
 
+def pypi_role(name, rawtext, text, lineno, inliner, options=None, content=None):
+    """Sphinx role for linking to a PyPI on https://pypi.org/.
+
+    Examples: ::
+
+        :pypi:`sphinx-issues`
+
+    """
+    options = options or {}
+    content = content or []
+    has_explicit_title, title, target = split_explicit_title(text)
+
+    target = utils.unescape(target).strip()
+    title = utils.unescape(title).strip()
+    ref = f"https://pypi.org/project/{target}"
+    text = title if has_explicit_title else target
+    link = nodes.reference(text=text, refuri=ref, **options)
+    return [link], []
+
+
 class IssueRole:
     # Symbols used to separate and issue/pull request/merge request etc
     # i.e
     #   - group/project#2323 for issues
     #   - group/project!1234 for merge requests (in gitlab)
     #   - group/project@adbc1234 for commits
     ELEMENT_SEPARATORS = "#@!"
@@ -379,12 +400,13 @@
     app.add_config_value("issues_user_prefix", default="@", rebuild="html", types=[str])
     app.add_role("issue", issue_role)
     app.add_role("pr", pr_role)
     app.add_role("user", user_role)
     app.add_role("commit", commit_role)
     app.add_role("cve", cve_role)
     app.add_role("cwe", cwe_role)
+    app.add_role("pypi", pypi_role)
     return {
         "version": importlib.metadata.version("sphinx-issues"),
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `sphinx_issues-4.0.0/tests/source/conf.py` & `sphinx_issues-4.1.0/tests/source/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx_issues-4.0.0/tests/test_sphinx_issues.py` & `sphinx_issues-4.1.0/tests/test_sphinx_issues.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 from sphinx_issues import (
     commit_role,
     cve_role,
     cwe_role,
     issue_role,
     pr_role,
+    pypi_role,
     user_role,
 )
 from sphinx_issues import setup as issues_setup
 
 BASE_DIR = Path(__file__).parent.absolute()
 
 
@@ -105,14 +106,21 @@
             cwe_role,
             "cve",
             "CWE-787",
             "CWE-787",
             "https://cwe.mitre.org/data/definitions/787.html",
         ),
         (
+            pypi_role,
+            "pypi",
+            "sphinx-issues",
+            "sphinx-issues",
+            "https://pypi.org/project/sphinx-issues",
+        ),
+        (
             commit_role,
             "commit",
             "123abc456def",
             "@123abc4",
             "https://github.com/marshmallow-code/marshmallow/commit/123abc456def",
         ),
         # External issue
```

### Comparing `sphinx_issues-4.0.0/PKG-INFO` & `sphinx_issues-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-issues
-Version: 4.0.0
+Version: 4.1.0
 Summary: A Sphinx extension for linking to your project's issue tracker
 Keywords: sphinx,issues,github
 Author-email: Steven Loria <sloria1@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Intended Audience :: Developers
@@ -159,28 +159,40 @@
 
 Use the ``:cwe:`` role to link to CWEs on https://cwe.mitre.org.
 
 .. code-block:: rst
 
     :cwe:`CWE-787` - The software writes data past the end, or...
 
+Use the ``:pypi:`` role to link to PyPI on https://pypi.org.
+
+.. code-block:: rst
+
+    :pypi:`sphinx-issues` - A Sphinx extension for linking to your project's issue tracker.
+
 Credits
 *******
 
 Credit goes to Jeff Forcier for his work on the `releases <https://github.com/bitprophet/releases>`_ extension, which is a full-featured solution for generating changelogs. I just needed a quick way to reference GitHub issues in my docs, so I yoinked the bits that I needed.
 
 License
 *******
 
 MIT licensed. See the bundled `LICENSE <https://github.com/sloria/sphinx-issues/blob/master/LICENSE>`_ file for more details.
 
 
 Changelog
 *********
 
+4.1.0 (2024-04-14)
+------------------
+
+- Add `:pypi:` role for linking to PyPI projects (`#144 <https://github.com/sloria/sphinx-issues/issues/144>`_).
+  Thanks @shenxianpeng for the suggestion and PR.
+
 4.0.0 (2024-01-19)
 ------------------
 
 - Default to linking GH Sponsors for the :user: role (`#129 <https://github.com/sloria/sphinx-issues/issues/129>`_).
   Thanks @webknjaz for the suggestion.
 - Support Python 3.8-3.12. Older versions are no longer supported.
 - *Backwards-incompatible*: Remove ``__version__``, ``__author__``, and ``__license__`` attributes.
```

