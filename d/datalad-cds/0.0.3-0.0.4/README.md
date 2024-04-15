# Comparing `tmp/datalad-cds-0.0.3.tar.gz` & `tmp/datalad_cds-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad-cds-0.0.3.tar", last modified: Wed Apr 10 13:42:36 2024, max compression
+gzip compressed data, was "datalad_cds-0.0.4.tar", last modified: Mon Apr 15 09:51:47 2024, max compression
```

## Comparing `datalad-cds-0.0.3.tar` & `datalad_cds-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.968902 datalad-cds-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-10 13:42:36.968902 datalad-cds-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.960902 datalad-cds-0.0.3/_datalad_buildsupport/
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/_datalad_buildsupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/_datalad_buildsupport/formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/_datalad_buildsupport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.964902 datalad-cds-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.964902 datalad-cds-0.0.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.964902 datalad-cds-0.0.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/source/_static/datalad_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.960902 datalad-cds-0.0.3/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.964902 datalad-cds-0.0.3/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/source/cli_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/docs/source/python_reference.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-10 13:42:36.968902 datalad-cds-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.960902 datalad-cds-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.964902 datalad-cds-0.0.3/src/datalad_cds/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/src/datalad_cds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-10 13:42:36.968902 datalad-cds-0.0.3/src/datalad_cds/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3653 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/src/datalad_cds/cds_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/src/datalad_cds/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/src/datalad_cds/download_cds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/src/datalad_cds/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.968902 datalad-cds-0.0.3/src/datalad_cds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-10 13:42:36.000000 datalad-cds-0.0.3/src/datalad_cds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-10 13:42:36.000000 datalad-cds-0.0.3/src/datalad_cds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:42:36.000000 datalad-cds-0.0.3/src/datalad_cds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-10 13:42:36.000000 datalad-cds-0.0.3/src/datalad_cds.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 13:42:36.000000 datalad-cds-0.0.3/src/datalad_cds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-10 13:42:36.000000 datalad-cds-0.0.3/src/datalad_cds.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:36.968902 datalad-cds-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/tests/test_cds_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/tests/test_download_cds.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/tests/test_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-10 13:42:33.000000 datalad-cds-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.417657 datalad_cds-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-15 09:51:47.417657 datalad_cds-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3432 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.413657 datalad_cds-0.0.4/_datalad_buildsupport/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/_datalad_buildsupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10698 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/_datalad_buildsupport/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/_datalad_buildsupport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.413657 datalad_cds-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.413657 datalad_cds-0.0.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.413657 datalad_cds-0.0.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/source/_static/datalad_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.409657 datalad_cds-0.0.4/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.413657 datalad_cds-0.0.4/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/source/cli_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/docs/source/python_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 09:51:47.417657 datalad_cds-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.409657 datalad_cds-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.413657 datalad_cds-0.0.4/src/datalad_cds/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/src/datalad_cds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 09:51:47.417657 datalad_cds-0.0.4/src/datalad_cds/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/src/datalad_cds/cds_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/src/datalad_cds/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/src/datalad_cds/download_cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/src/datalad_cds/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.417657 datalad_cds-0.0.4/src/datalad_cds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-15 09:51:47.000000 datalad_cds-0.0.4/src/datalad_cds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-15 09:51:47.000000 datalad_cds-0.0.4/src/datalad_cds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:51:47.000000 datalad_cds-0.0.4/src/datalad_cds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 09:51:47.000000 datalad_cds-0.0.4/src/datalad_cds.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-15 09:51:47.000000 datalad_cds-0.0.4/src/datalad_cds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 09:51:47.000000 datalad_cds-0.0.4/src/datalad_cds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:47.417657 datalad_cds-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/tests/test_cds_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/tests/test_download_cds.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/tests/test_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-15 09:51:43.000000 datalad_cds-0.0.4/versioneer.py
```

### Comparing `datalad-cds-0.0.3/LICENSE` & `datalad_cds-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/PKG-INFO` & `datalad_cds-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-cds
-Version: 0.0.3
+Version: 0.0.4
 Summary: DataLad extension for downloading from the Copernicus Climate Data Store
 Author: Matthias Riße
 Author-email: The DataLad Team and Contributors <team@datalad.org>, Benedikt Bulich <b.bulich@fz-juelich.de>, Daniel Klauß <daniel.klauss@alumni.fh-aachen.de>, Laurens Jan van Haaren <l.van.haaren@fz-juelich.de>, Matthias Riße <m.risse@fz-juelich.de>
 Maintainer-email: Matthias Riße <m.risse@fz-juelich.de>
 License: # Main Copyright/License
         
         DataLad, including all examples, code snippets and attached
```

### Comparing `datalad-cds-0.0.3/README.md` & `datalad_cds-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/_datalad_buildsupport/__init__.py` & `datalad_cds-0.0.4/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/_datalad_buildsupport/formatters.py` & `datalad_cds-0.0.4/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/_datalad_buildsupport/setup.py` & `datalad_cds-0.0.4/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/docs/Makefile` & `datalad_cds-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/docs/README.md` & `datalad_cds-0.0.4/docs/README.md`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/docs/source/_static/datalad_logo.png` & `datalad_cds-0.0.4/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/docs/source/conf.py` & `datalad_cds-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/docs/source/index.rst` & `datalad_cds-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/pyproject.toml` & `datalad_cds-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/src/datalad_cds/__init__.py` & `datalad_cds-0.0.4/src/datalad_cds/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/src/datalad_cds/cds_remote.py` & `datalad_cds-0.0.4/src/datalad_cds/cds_remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,16 +91,16 @@
             raise RemoteError(exceptions)
 
     def whereis(self, key: str) -> str:
         url = self.annex.geturls(key, "cds:")[0]
         return datalad_cds.spec.Spec.from_url(url).to_json()
 
     def checkpresent(self, key: str) -> bool:
-        # We just assume that we can always handle the key
-        return True
+        urls = self.annex.geturls(key, "cds:")
+        return len(urls) > 0
 
     def claimurl(self, url: str) -> bool:
         return url.startswith("cds:")
 
     def checkurl(self, url: str) -> bool:
         return url.startswith("cds:")
```

### Comparing `datalad-cds-0.0.3/src/datalad_cds/download_cds.py` & `datalad_cds-0.0.4/src/datalad_cds/download_cds.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             raise TypeError("spec could not be parsed")
         ds = require_dataset(dataset, check_installed=True)
         ensure_special_remote_exists_and_is_enabled(ds.repo, "cds")
         pathobj = ds.pathobj / path
         url = parsed_spec.to_url()
         options = []
         if lazy:
-            options.append("--relaxed")
+            options.append("--fast")
         ds.repo.add_url_to_file(pathobj, url, options=options)
         if save:
             msg = (
                 message
                 if message is not None
                 else "[DATALAD] Download from Climate Data Store"
             )
```

### Comparing `datalad-cds-0.0.3/src/datalad_cds/spec.py` & `datalad_cds-0.0.4/src/datalad_cds/spec.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/src/datalad_cds.egg-info/PKG-INFO` & `datalad_cds-0.0.4/src/datalad_cds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-cds
-Version: 0.0.3
+Version: 0.0.4
 Summary: DataLad extension for downloading from the Copernicus Climate Data Store
 Author: Matthias Riße
 Author-email: The DataLad Team and Contributors <team@datalad.org>, Benedikt Bulich <b.bulich@fz-juelich.de>, Daniel Klauß <daniel.klauss@alumni.fh-aachen.de>, Laurens Jan van Haaren <l.van.haaren@fz-juelich.de>, Matthias Riße <m.risse@fz-juelich.de>
 Maintainer-email: Matthias Riße <m.risse@fz-juelich.de>
 License: # Main Copyright/License
         
         DataLad, including all examples, code snippets and attached
```

### Comparing `datalad-cds-0.0.3/src/datalad_cds.egg-info/SOURCES.txt` & `datalad_cds-0.0.4/src/datalad_cds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/tests/conftest.py` & `datalad_cds-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/tests/test_cds_remote.py` & `datalad_cds-0.0.4/tests/test_cds_remote.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/tests/test_download_cds.py` & `datalad_cds-0.0.4/tests/test_download_cds.py`

 * *Files identical despite different names*

### Comparing `datalad-cds-0.0.3/versioneer.py` & `datalad_cds-0.0.4/versioneer.py`

 * *Files identical despite different names*

