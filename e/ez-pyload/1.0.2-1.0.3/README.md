# Comparing `tmp/ez_pyload-1.0.2.tar.gz` & `tmp/ez_pyload-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_pyload-1.0.2.tar", max compression
+gzip compressed data, was "ez_pyload-1.0.3.tar", max compression
```

## Comparing `ez_pyload-1.0.2.tar` & `ez_pyload-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1356 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/README.md
--rw-r--r--   0        0        0       39 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/__init__.py
--rw-r--r--   0        0        0      613 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/__main__.py
--rw-r--r--   0        0        0     2852 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/download.py
--rw-r--r--   0        0        0     1125 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/patches.py
--rw-r--r--   0        0        0      451 2024-04-14 16:49:11.904468 ez_pyload-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ez_pyload-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1356 2024-04-14 20:48:34.689138 ez_pyload-1.0.3/README.md
+-rw-r--r--   0        0        0       39 2024-04-14 20:48:34.689138 ez_pyload-1.0.3/ez_pyload/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-14 20:48:34.689138 ez_pyload-1.0.3/ez_pyload/__main__.py
+-rw-r--r--   0        0        0     2976 2024-04-14 20:48:34.693138 ez_pyload-1.0.3/ez_pyload/download.py
+-rw-r--r--   0        0        0     1125 2024-04-14 20:48:34.693138 ez_pyload-1.0.3/ez_pyload/patches.py
+-rw-r--r--   0        0        0      451 2024-04-14 20:48:34.693138 ez_pyload-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ez_pyload-1.0.3/PKG-INFO
```

### Comparing `ez_pyload-1.0.2/README.md` & `ez_pyload-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ez_pyload-1.0.2/ez_pyload/__main__.py` & `ez_pyload-1.0.3/ez_pyload/__main__.py`

 * *Files identical despite different names*

### Comparing `ez_pyload-1.0.2/ez_pyload/download.py` & `ez_pyload-1.0.3/ez_pyload/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,24 +59,27 @@
         Path: Path to downloaded file/folder
     """
     download_dir = Path(download_dir)
     debug = loglevel == logging.DEBUG
     logger.setLevel(loglevel)
     tmp = "."
     with tempfile.TemporaryDirectory(".ez-pyload") as tmp:
-        pyload = Core(tmp, "tmpdir", "storage", debug)
-        is_dir = _download(pyload, url)
-        src_path = next((Path(tmp) / "data" / "storage" / "unknown").glob("*"))
-        name = src_path.name
-        dst_path = download_dir / name
-        # pyload messes with cwd again
-        os.chdir(cwd)
-        if is_dir:
-            shutil.copytree(src_path, dst_path)
-        else:
-            shutil.copy(src_path, dst_path)
-        # don't care about corrupting data,
-        # just need to release connections NOW
-        # so we can clean up tempdir
-        pyload.db.c.close()
-        pyload.db.conn.close()
-        return dst_path
+        try:
+            pyload = Core(tmp, "tmpdir", "storage", debug)
+            is_dir = _download(pyload, url)
+            src_path = next((Path(tmp) / "data" / "storage" / "unknown").glob("*"))
+            name = src_path.name
+            dst_path = download_dir / name
+            # pyload messes with cwd again
+            os.chdir(cwd)
+            if is_dir:
+                shutil.copytree(src_path, dst_path)
+            else:
+                shutil.copy(src_path, dst_path)
+            return dst_path
+        finally:
+            # don't care about corrupting data,
+            # just need to release connections NOW
+            # so we can clean up tempdir
+            pyload.db.c.close()
+            pyload.db.conn.close()
+            os.chdir(cwd)
```

### Comparing `ez_pyload-1.0.2/ez_pyload/patches.py` & `ez_pyload-1.0.3/ez_pyload/patches.py`

 * *Files identical despite different names*

### Comparing `ez_pyload-1.0.2/PKG-INFO` & `ez_pyload-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-pyload
-Version: 1.0.2
+Version: 1.0.3
 Summary: Wrapper for pyLoad to allow downloading files through Python (no webserver). Includes CLI
 License: MIT
 Author: 7x11x13
 Author-email: x7x11x13@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

