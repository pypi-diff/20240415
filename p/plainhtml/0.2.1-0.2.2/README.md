# Comparing `tmp/plainhtml-0.2.1.tar.gz` & `tmp/plainhtml-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plainhtml-0.2.1.tar", max compression
+gzip compressed data, was "plainhtml-0.2.2.tar", max compression
```

## Comparing `plainhtml-0.2.1.tar` & `plainhtml-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1079 2024-02-09 09:58:06.785599 plainhtml-0.2.1/LICENSE
--rw-r--r--   0        0        0      235 2024-02-09 09:58:06.785599 plainhtml-0.2.1/README.md
--rw-r--r--   0        0        0       86 2024-02-09 14:34:54.138023 plainhtml-0.2.1/plainhtml/__init__.py
--rw-r--r--   0        0        0      330 2024-02-09 09:58:06.785599 plainhtml-0.2.1/plainhtml/core.py
--rw-r--r--   0        0        0     3930 2024-02-09 10:03:48.278222 plainhtml-0.2.1/plainhtml/parser.py
--rw-r--r--   0        0        0     1935 2024-02-09 09:59:33.025731 plainhtml-0.2.1/plainhtml/utils.py
--rw-r--r--   0        0        0      457 2024-02-09 14:34:59.361990 plainhtml-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 plainhtml-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2024-02-09 09:58:06.785599 plainhtml-0.2.2/LICENSE
+-rw-r--r--   0        0        0      235 2024-02-09 09:58:06.785599 plainhtml-0.2.2/README.md
+-rw-r--r--   0        0        0       86 2024-02-09 14:34:54.138023 plainhtml-0.2.2/plainhtml/__init__.py
+-rw-r--r--   0        0        0      330 2024-02-09 09:58:06.785599 plainhtml-0.2.2/plainhtml/core.py
+-rw-r--r--   0        0        0     3930 2024-02-09 10:03:48.278222 plainhtml-0.2.2/plainhtml/parser.py
+-rw-r--r--   0        0        0     1935 2024-02-09 09:59:33.025731 plainhtml-0.2.2/plainhtml/utils.py
+-rw-r--r--   0        0        0      496 2024-04-15 12:19:35.030505 plainhtml-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 plainhtml-0.2.2/PKG-INFO
```

### Comparing `plainhtml-0.2.1/LICENSE` & `plainhtml-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plainhtml-0.2.1/plainhtml/parser.py` & `plainhtml-0.2.2/plainhtml/parser.py`

 * *Files identical despite different names*

### Comparing `plainhtml-0.2.1/plainhtml/utils.py` & `plainhtml-0.2.2/plainhtml/utils.py`

 * *Files identical despite different names*

### Comparing `plainhtml-0.2.1/PKG-INFO` & `plainhtml-0.2.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: plainhtml
-Version: 0.2.1
+Version: 0.2.2
 Summary: Extract plain text from HTML
 Author: Severin Simmler
 Author-email: s.simmler@snapaddy.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: lxml (>=5.1.0,<6.0.0)
+Requires-Dist: lxml[html-clean] (>=5.1.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # Extract plain text from HTML
 
 ## Installation
 
 ```
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: plainhtml Version: 0.2.1 Summary: Extract plain
+Metadata-Version: 2.1 Name: plainhtml Version: 0.2.2 Summary: Extract plain
 text from HTML Author: Severin Simmler Author-email: s.simmler@snapaddy.com
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: lxml (>=5.1.0,<6.0.0) Description-Content-Type: text/markdown #
-Extract plain text from HTML ## Installation ``` $ pip install plainhtml ``` ##
-Example ```python >>> import plainhtml >>> html = "
+Requires-Dist: lxml[html-clean] (>=5.1.0,<6.0.0) Description-Content-Type:
+text/markdown # Extract plain text from HTML ## Installation ``` $ pip install
+plainhtml ``` ## Example ```python >>> import plainhtml >>> html = "
 foo
 bar
 " >>> plainhtml.extract_text(html) 'foo\n\nbar' ```
```

