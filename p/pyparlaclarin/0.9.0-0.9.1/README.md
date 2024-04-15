# Comparing `tmp/pyparlaclarin-0.9.0.tar.gz` & `tmp/pyparlaclarin-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyparlaclarin-0.9.0.tar", max compression
+gzip compressed data, was "pyparlaclarin-0.9.1.tar", max compression
```

## Comparing `pyparlaclarin-0.9.0.tar` & `pyparlaclarin-0.9.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.9.0/README.md
--rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.9.0/pyparlaclarin/__init__.py
--rw-r--r--   0        0        0     4096 2024-02-09 10:06:54.385506 pyparlaclarin-0.9.0/pyparlaclarin/create.py
--rw-r--r--   0        0        0     5135 2024-03-28 12:07:25.490133 pyparlaclarin-0.9.0/pyparlaclarin/read.py
--rw-r--r--   0        0        0     5880 2023-05-05 12:59:39.989246 pyparlaclarin-0.9.0/pyparlaclarin/refine.py
--rw-r--r--   0        0        0      605 2024-03-28 12:13:19.413932 pyparlaclarin-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 pyparlaclarin-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2021-10-25 14:50:08.200629 pyparlaclarin-0.9.1/README.md
+-rw-r--r--   0        0        0       58 2021-10-25 14:50:08.220524 pyparlaclarin-0.9.1/pyparlaclarin/__init__.py
+-rw-r--r--   0        0        0     4096 2024-02-09 10:06:54.385506 pyparlaclarin-0.9.1/pyparlaclarin/create.py
+-rw-r--r--   0        0        0     5249 2024-04-15 13:03:28.618175 pyparlaclarin-0.9.1/pyparlaclarin/read.py
+-rw-r--r--   0        0        0     5880 2023-05-05 12:59:39.989246 pyparlaclarin-0.9.1/pyparlaclarin/refine.py
+-rw-r--r--   0        0        0      605 2024-04-15 13:05:38.856099 pyparlaclarin-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1597 1970-01-01 00:00:00.000000 pyparlaclarin-0.9.1/PKG-INFO
```

### Comparing `pyparlaclarin-0.9.0/README.md` & `pyparlaclarin-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.9.0/pyparlaclarin/create.py` & `pyparlaclarin-0.9.1/pyparlaclarin/create.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.9.0/pyparlaclarin/read.py` & `pyparlaclarin-0.9.1/pyparlaclarin/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,17 +122,19 @@
         for div in body.findall("{http://www.tei-c.org/ns/1.0}div"):
             for elem in div:
                 # Check if we enter the page the user requested
                 if page is not None:
                     if elem.tag == tei_ns + "pb":
                         correct_page = elem.attrib.get("n") == page
                 if output == "str":
-                    p = "\n".join(elem.itertext())
                     if page is None or correct_page:
-                        yield p
+                        for p in elem.itertext():
+                            p_text = " ".join(p.split())
+                            if p_text != "":
+                                yield p_text
                 elif output == "lxml":
                     if page is None or correct_page:
                         yield elem
 
 def get_dates(root):
     """
     Get dates of a Parla-Clarin file.
```

### Comparing `pyparlaclarin-0.9.0/pyparlaclarin/refine.py` & `pyparlaclarin-0.9.1/pyparlaclarin/refine.py`

 * *Files identical despite different names*

### Comparing `pyparlaclarin-0.9.0/pyproject.toml` & `pyparlaclarin-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyparlaclarin"
-version = "0.9.0"
+version = "0.9.1"
 description = "Read, create, and modify Parla-Clarin XML files"
 authors = ["ninpnin <vainoyrjanainen@icloud.com>"]
 repository = "https://github.com/welfare-state-analytics/pyparlaclarin"
 documentation = "https://welfare-state-analytics.github.io/pyparlaclarin/pyparlaclarin/"
 readme = "README.md"
 license = "MIT"
 packages = [
```

### Comparing `pyparlaclarin-0.9.0/PKG-INFO` & `pyparlaclarin-0.9.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyparlaclarin
-Version: 0.9.0
+Version: 0.9.1
 Summary: Read, create, and modify Parla-Clarin XML files
 Home-page: https://github.com/welfare-state-analytics/pyparlaclarin
 License: MIT
 Author: ninpnin
 Author-email: vainoyrjanainen@icloud.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

