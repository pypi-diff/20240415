# Comparing `tmp/yq-3.3.0.tar.gz` & `tmp/yq-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yq-3.3.0.tar", last modified: Sun Apr 14 05:26:43 2024, max compression
+gzip compressed data, was "yq-3.3.1.tar", last modified: Mon Apr 15 18:16:32 2024, max compression
```

## Comparing `yq-3.3.0.tar` & `yq-3.3.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.307416 yq-3.3.0/
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.289090 yq-3.3.0/.github/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:28:59.000000 yq-3.3.0/.github/FUNDING.yml
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.289672 yq-3.3.0/.github/workflows/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      945 2024-04-13 17:02:32.000000 yq-3.3.0/.github/workflows/ci.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      477 2023-10-23 21:28:59.000000 yq-3.3.0/.gitignore
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8032 2024-04-14 05:26:20.000000 yq-3.3.0/Changes.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10273 2023-10-23 21:28:59.000000 yq-3.3.0/LICENSE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2023-10-23 21:28:59.000000 yq-3.3.0/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      478 2023-10-23 21:28:59.000000 yq-3.3.0/Makefile
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8836 2024-04-14 05:26:43.306693 yq-3.3.0/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7582 2024-04-14 04:46:08.000000 yq-3.3.0/README.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      696 2023-10-23 21:29:01.000000 yq-3.3.0/SECURITY.md
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2542 2024-04-14 04:46:23.000000 yq-3.3.0/common.mk
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.294956 yq-3.3.0/docs/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:59.000000 yq-3.3.0/docs/changelog.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3515 2024-04-14 05:26:20.000000 yq-3.3.0/docs/cli-doc-tomlq.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3897 2024-04-14 05:26:20.000000 yq-3.3.0/docs/cli-doc-xq.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4503 2024-04-14 05:26:20.000000 yq-3.3.0/docs/cli-doc.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      806 2023-10-23 21:28:59.000000 yq-3.3.0/docs/conf.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      248 2023-10-23 21:28:59.000000 yq-3.3.0/docs/index.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:28:59.000000 yq-3.3.0/docs/toc.html
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      416 2024-04-14 04:46:08.000000 yq-3.3.0/pyproject.toml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-04-14 05:26:43.307499 yq-3.3.0/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1677 2024-04-14 05:25:14.000000 yq-3.3.0/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.297523 yq-3.3.0/test/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3468 2023-10-23 21:28:59.000000 yq-3.3.0/test/cfn.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      306 2023-10-23 21:28:59.000000 yq-3.3.0/test/doc.yml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-10-23 21:28:59.000000 yq-3.3.0/test/filter.jq
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    15883 2024-04-13 16:56:36.000000 yq-3.3.0/test/test.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.301291 yq-3.3.0/yq/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    13702 2024-04-14 05:11:44.000000 yq-3.3.0/yq/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:58.000000 yq-3.3.0/yq/__main__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3531 2023-10-23 21:28:58.000000 yq-3.3.0/yq/dumper.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8940 2024-04-14 05:11:03.000000 yq-3.3.0/yq/loader.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6212 2023-10-23 21:28:58.000000 yq-3.3.0/yq/parser.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-14 05:26:43.305657 yq-3.3.0/yq.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8836 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      555 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/entry_points.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      107 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        3 2024-04-14 05:26:43.000000 yq-3.3.0/yq.egg-info/top_level.txt
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.783069 yq-3.3.1/
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.767391 yq-3.3.1/.github/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       18 2023-10-23 21:28:59.000000 yq-3.3.1/.github/FUNDING.yml
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.767877 yq-3.3.1/.github/workflows/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      945 2024-04-15 18:14:25.000000 yq-3.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      477 2023-10-23 21:28:59.000000 yq-3.3.1/.gitignore
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8184 2024-04-15 18:16:07.000000 yq-3.3.1/Changes.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10273 2023-10-23 21:28:59.000000 yq-3.3.1/LICENSE
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       41 2023-10-23 21:28:59.000000 yq-3.3.1/MANIFEST.in
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      478 2023-10-23 21:28:59.000000 yq-3.3.1/Makefile
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8836 2024-04-15 18:16:32.782385 yq-3.3.1/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     7582 2024-04-15 18:14:25.000000 yq-3.3.1/README.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      696 2023-10-23 21:29:01.000000 yq-3.3.1/SECURITY.md
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2542 2024-04-15 18:14:25.000000 yq-3.3.1/common.mk
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.771795 yq-3.3.1/docs/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:59.000000 yq-3.3.1/docs/changelog.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3515 2024-04-15 18:16:07.000000 yq-3.3.1/docs/cli-doc-tomlq.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3897 2024-04-15 18:16:07.000000 yq-3.3.1/docs/cli-doc-xq.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4503 2024-04-15 18:16:07.000000 yq-3.3.1/docs/cli-doc.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      806 2023-10-23 21:28:59.000000 yq-3.3.1/docs/conf.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      248 2023-10-23 21:28:59.000000 yq-3.3.1/docs/index.rst
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-10-23 21:28:59.000000 yq-3.3.1/docs/toc.html
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      416 2024-04-15 18:14:25.000000 yq-3.3.1/pyproject.toml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       38 2024-04-15 18:16:32.783203 yq-3.3.1/setup.cfg
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1677 2024-04-15 18:16:02.000000 yq-3.3.1/setup.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.774527 yq-3.3.1/test/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3468 2023-10-23 21:28:59.000000 yq-3.3.1/test/cfn.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      306 2023-10-23 21:28:59.000000 yq-3.3.1/test/doc.yml
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-10-23 21:28:59.000000 yq-3.3.1/test/filter.jq
+-rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    15798 2024-04-15 18:15:39.000000 yq-3.3.1/test/test.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.777238 yq-3.3.1/yq/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    13702 2024-04-15 18:14:25.000000 yq-3.3.1/yq/__init__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       56 2023-10-23 21:28:58.000000 yq-3.3.1/yq/__main__.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3531 2023-10-23 21:28:58.000000 yq-3.3.1/yq/dumper.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8172 2024-04-15 18:15:39.000000 yq-3.3.1/yq/loader.py
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6212 2023-10-23 21:28:58.000000 yq-3.3.1/yq/parser.py
+drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2024-04-15 18:16:32.781039 yq-3.3.1/yq.egg-info/
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8836 2024-04-15 18:16:32.000000 yq-3.3.1/yq.egg-info/PKG-INFO
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      555 2024-04-15 18:16:32.000000 yq-3.3.1/yq.egg-info/SOURCES.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2024-04-15 18:16:32.000000 yq-3.3.1/yq.egg-info/dependency_links.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       63 2024-04-15 18:16:32.000000 yq-3.3.1/yq.egg-info/entry_points.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      107 2024-04-15 18:16:32.000000 yq-3.3.1/yq.egg-info/requires.txt
+-rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        3 2024-04-15 18:16:32.000000 yq-3.3.1/yq.egg-info/top_level.txt
```

### Comparing `yq-3.3.0/.github/workflows/ci.yml` & `yq-3.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/Changes.rst` & `yq-3.3.1/Changes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Changes for v3.3.1 (2024-04-15)
+===============================
+
+Revert “Do not interpret characters that cannot be parsed in octal as
+int (#176)”
+
 Changes for v3.3.0 (2024-04-13)
 ===============================
 
 -  tomlq: Use tomllib on Python 3.11 when not round-tripping
 
 -  xq: Support in-place XML editing
```

### Comparing `yq-3.3.0/LICENSE` & `yq-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/PKG-INFO` & `yq-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.3.0
+Version: 3.3.1
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `yq-3.3.0/README.rst` & `yq-3.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/SECURITY.md` & `yq-3.3.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/common.mk` & `yq-3.3.1/common.mk`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/docs/cli-doc-tomlq.txt` & `yq-3.3.1/docs/cli-doc-tomlq.txt`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/docs/cli-doc-xq.txt` & `yq-3.3.1/docs/cli-doc-xq.txt`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/docs/cli-doc.txt` & `yq-3.3.1/docs/cli-doc.txt`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/docs/conf.py` & `yq-3.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/setup.py` & `yq-3.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="yq",
-    version="3.3.0",
+    version="3.3.1",
     url="https://github.com/kislyuk/yq",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Command-line YAML/XML processor - jq wrapper for YAML/XML documents",
     long_description=open("README.rst").read(),
     python_requires=">=3.6",
```

### Comparing `yq-3.3.0/test/cfn.yml` & `yq-3.3.1/test/cfn.yml`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/test/test.py` & `yq-3.3.1/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,14 @@
         self.assertEqual(self.run_yq("+685_230", ["-y", "."]), "'+685_230'\n")
         self.assertEqual(self.run_yq("+685_230", ["-y", "--yml-out-ver=1.2", "."]), "+685_230\n...\n")
 
         self.assertEqual(self.run_yq("+12345", ["-y", "."]), "12345\n...\n")
 
     def test_yaml_1_1_octals(self):
         self.assertEqual(self.run_yq("on: -012345", ["-y", "."]), "'on': -5349\n")
-        self.assertEqual(self.run_yq("on: -012349", ["-y", "."]), "'on': -012349\n")
 
     @unittest.expectedFailure
     def test_yaml_1_2_octals(self):
         """YAML 1.2 octals not yet implemented"""
         self.assertEqual(self.run_yq("on: -012345", ["-y", "--yml-out-ver=1.2", "."]), "on: -12345\n")
```

### Comparing `yq-3.3.0/yq/__init__.py` & `yq-3.3.1/yq/__init__.py`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/yq/dumper.py` & `yq-3.3.1/yq/dumper.py`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/yq/loader.py` & `yq-3.3.1/yq/loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,41 +83,21 @@
         {
             "tag": "tag:yaml.org,2002:bool",
             "regexp": re.compile(r"^(?:|true|True|TRUE|false|False|FALSE)$", re.X),
             "start_chars": list("tTfF"),
         },
         {
             "tag": "tag:yaml.org,2002:int",
-            "regexp": re.compile(
-                r"""^(?:
-                # [-+]?0b[0-1_]+ # (base 2)
-                 [-+]?0[0-7]+ # (base 8)
-                |[-+]?0o[0-7]+ # (base 8)
-                |[-+]?(0|[1-9][0-9]*) # (base 10)
-                # |[-+]?0[0-7_]+ # (base 8)
-                # |[-+]?0o[0-7_]+ # (base 8)
-                # |[-+]?(0|[1-9][0-9_]*) # (base 10)
-                # |[-+]?0x[0-9a-fA-F_]+ # (base 16)
-                # |[-+]?[1-9][0-9_]*(:[0-5]?[0-9])+ # (base 60)
-                )$""",
-                re.X,
-            ),
+            "regexp": re.compile(r"^(?:|0o[0-7]+|[-+]?(?:[0-9]+)|0x[0-9a-fA-F]+)$", re.X),
             "start_chars": list("-+0123456789"),
         },
         {
             "tag": "tag:yaml.org,2002:float",
             "regexp": re.compile(
-                r"""^(?:
-                 [-+]?([0-9][0-9]*)?\.[0-9.]*([eE][-+][0-9]+)? (base 10)
-                |[-+]?[0-9][0-9]*(:[0-5]?[0-9])+\.[0-9]* (base 60)
-                # |[-+]?([0-9][0-9_]*)?\.[0-9.]*([eE][-+][0-9]+)? (base 10)
-                # |[-+]?[0-9][0-9_]*(:[0-5]?[0-9])+\.[0-9_]* (base 60)
-                |[-+]?\.(inf|Inf|INF) # (infinity)
-                |\.(nan|NaN|NAN) # (not a number)
-                )$""",
+                r"^(?:[-+]?(?:\.[0-9]+|[0-9]+(\.[0-9]*)?)(?:[eE][-+]?[0-9]+)?|[-+]?\.(?:inf|Inf|INF)|\.(?:nan|NaN|NAN))$",  # noqa
                 re.X,
             ),
             "start_chars": list("-+0123456789."),
         },
         {
             "tag": "tag:yaml.org,2002:null",
             "regexp": re.compile(r"^(?:~||null|Null|NULL)$", re.X),
```

### Comparing `yq-3.3.0/yq/parser.py` & `yq-3.3.1/yq/parser.py`

 * *Files identical despite different names*

### Comparing `yq-3.3.0/yq.egg-info/PKG-INFO` & `yq-3.3.1/yq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yq
-Version: 3.3.0
+Version: 3.3.1
 Summary: Command-line YAML/XML processor - jq wrapper for YAML/XML documents
 Home-page: https://github.com/kislyuk/yq
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `yq-3.3.0/yq.egg-info/SOURCES.txt` & `yq-3.3.1/yq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

