# Comparing `tmp/pycpio-0.8.4.tar.gz` & `tmp/pycpio-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycpio-0.8.4.tar", last modified: Wed Jan 17 19:10:06 2024, max compression
+gzip compressed data, was "pycpio-0.9.2.tar", last modified: Mon Apr 15 01:11:07 2024, max compression
```

## Comparing `pycpio-0.8.4.tar` & `pycpio-0.9.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/
--rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-11-26 02:38:37.000000 pycpio-0.8.4/LICENSE
--rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-01-17 19:10:06.990193 pycpio-0.8.4/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      687 2024-01-17 19:08:30.000000 pycpio-0.8.4/pyproject.toml
--rw-r--r--   0 desu      (1000) desu      (1000)       84 2023-11-25 18:42:57.000000 pycpio-0.8.4/readme.md
--rw-r--r--   0 desu      (1000) desu      (1000)       38 2024-01-17 19:10:06.990193 pycpio-0.8.4/setup.cfg
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.988193 pycpio-0.8.4/src/
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.989193 pycpio-0.8.4/src/pycpio/
--rw-r--r--   0 desu      (1000) desu      (1000)       49 2023-11-26 16:53:57.000000 pycpio-0.8.4/src/pycpio/__init__.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/src/pycpio/cpio/
--rw-r--r--   0 desu      (1000) desu      (1000)      172 2023-12-02 22:27:03.000000 pycpio-0.8.4/src/pycpio/cpio/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     4902 2024-01-11 19:47:06.000000 pycpio-0.8.4/src/pycpio/cpio/archive.py
--rw-r--r--   0 desu      (1000) desu      (1000)      843 2023-12-03 02:12:07.000000 pycpio-0.8.4/src/pycpio/cpio/chardev.py
--rw-r--r--   0 desu      (1000) desu      (1000)      447 2023-11-27 04:09:12.000000 pycpio-0.8.4/src/pycpio/cpio/common.py
--rw-r--r--   0 desu      (1000) desu      (1000)     6586 2024-01-11 19:38:25.000000 pycpio-0.8.4/src/pycpio/cpio/data.py
--rw-r--r--   0 desu      (1000) desu      (1000)      624 2023-12-03 02:30:33.000000 pycpio-0.8.4/src/pycpio/cpio/dir.py
--rw-r--r--   0 desu      (1000) desu      (1000)      814 2023-11-28 01:13:44.000000 pycpio-0.8.4/src/pycpio/cpio/file.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1285 2023-12-19 03:06:17.000000 pycpio-0.8.4/src/pycpio/cpio/symlink.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/src/pycpio/header/
--rw-r--r--   0 desu      (1000) desu      (1000)      228 2023-11-27 19:50:55.000000 pycpio-0.8.4/src/pycpio/header/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     7950 2024-01-11 19:38:14.000000 pycpio-0.8.4/src/pycpio/header/cpioheader.py
--rw-r--r--   0 desu      (1000) desu      (1000)      701 2023-11-27 22:10:56.000000 pycpio-0.8.4/src/pycpio/header/header_funcs.py
--rw-r--r--   0 desu      (1000) desu      (1000)      411 2023-11-27 22:28:21.000000 pycpio-0.8.4/src/pycpio/header/headers.py
--rwxr-xr-x   0 desu      (1000) desu      (1000)     3267 2024-01-17 19:08:21.000000 pycpio-0.8.4/src/pycpio/main.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/src/pycpio/masks/
--rw-r--r--   0 desu      (1000) desu      (1000)      277 2023-11-27 19:37:46.000000 pycpio-0.8.4/src/pycpio/masks/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1378 2023-12-03 01:03:25.000000 pycpio-0.8.4/src/pycpio/masks/modes.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1499 2023-11-27 18:36:51.000000 pycpio-0.8.4/src/pycpio/masks/permissions.py
--rw-r--r--   0 desu      (1000) desu      (1000)     3659 2024-01-11 19:47:25.000000 pycpio-0.8.4/src/pycpio/pycpio.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/src/pycpio/reader/
--rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:23.000000 pycpio-0.8.4/src/pycpio/reader/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     3700 2024-01-11 19:46:36.000000 pycpio-0.8.4/src/pycpio/reader/reader.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/src/pycpio/writer/
--rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:07.000000 pycpio-0.8.4/src/pycpio/writer/__init__.py
--rw-r--r--   0 desu      (1000) desu      (1000)     1584 2024-01-11 19:46:06.000000 pycpio-0.8.4/src/pycpio/writer/writer.py
-drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-01-17 19:10:06.990193 pycpio-0.8.4/src/pycpio.egg-info/
--rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-01-17 19:10:06.000000 pycpio-0.8.4/src/pycpio.egg-info/PKG-INFO
--rw-r--r--   0 desu      (1000) desu      (1000)      835 2024-01-17 19:10:06.000000 pycpio-0.8.4/src/pycpio.egg-info/SOURCES.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        1 2024-01-17 19:10:06.000000 pycpio-0.8.4/src/pycpio.egg-info/dependency_links.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       44 2024-01-17 19:10:06.000000 pycpio-0.8.4/src/pycpio.egg-info/entry_points.txt
--rw-r--r--   0 desu      (1000) desu      (1000)       14 2024-01-17 19:10:06.000000 pycpio-0.8.4/src/pycpio.egg-info/requires.txt
--rw-r--r--   0 desu      (1000) desu      (1000)        7 2024-01-17 19:10:06.000000 pycpio-0.8.4/src/pycpio.egg-info/top_level.txt
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.958554 pycpio-0.9.2/
+-rw-r--r--   0 desu      (1000) desu      (1000)    18092 2023-11-26 02:38:37.000000 pycpio-0.9.2/LICENSE
+-rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-04-15 01:11:07.958554 pycpio-0.9.2/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      687 2024-04-15 01:03:04.000000 pycpio-0.9.2/pyproject.toml
+-rw-r--r--   0 desu      (1000) desu      (1000)       84 2023-11-25 18:42:57.000000 pycpio-0.9.2/readme.md
+-rw-r--r--   0 desu      (1000) desu      (1000)       38 2024-04-15 01:11:07.958554 pycpio-0.9.2/setup.cfg
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.953554 pycpio-0.9.2/src/
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.954554 pycpio-0.9.2/src/pycpio/
+-rw-r--r--   0 desu      (1000) desu      (1000)       49 2023-11-26 16:53:57.000000 pycpio-0.9.2/src/pycpio/__init__.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.956554 pycpio-0.9.2/src/pycpio/cpio/
+-rw-r--r--   0 desu      (1000) desu      (1000)      172 2023-12-02 22:27:03.000000 pycpio-0.9.2/src/pycpio/cpio/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     4902 2024-01-11 19:47:06.000000 pycpio-0.9.2/src/pycpio/cpio/archive.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      843 2023-12-03 02:12:07.000000 pycpio-0.9.2/src/pycpio/cpio/chardev.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      447 2023-11-27 04:09:12.000000 pycpio-0.9.2/src/pycpio/cpio/common.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     6611 2024-03-24 23:10:29.000000 pycpio-0.9.2/src/pycpio/cpio/data.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      624 2023-12-03 02:30:33.000000 pycpio-0.9.2/src/pycpio/cpio/dir.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      814 2023-11-28 01:13:44.000000 pycpio-0.9.2/src/pycpio/cpio/file.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1285 2023-12-19 03:06:17.000000 pycpio-0.9.2/src/pycpio/cpio/symlink.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.957554 pycpio-0.9.2/src/pycpio/header/
+-rw-r--r--   0 desu      (1000) desu      (1000)      228 2023-11-27 19:50:55.000000 pycpio-0.9.2/src/pycpio/header/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     7950 2024-03-24 23:35:31.000000 pycpio-0.9.2/src/pycpio/header/cpioheader.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      701 2023-11-27 22:10:56.000000 pycpio-0.9.2/src/pycpio/header/header_funcs.py
+-rw-r--r--   0 desu      (1000) desu      (1000)      411 2023-11-27 22:28:21.000000 pycpio-0.9.2/src/pycpio/header/headers.py
+-rwxr-xr-x   0 desu      (1000) desu      (1000)     3257 2024-04-15 01:04:10.000000 pycpio-0.9.2/src/pycpio/main.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.957554 pycpio-0.9.2/src/pycpio/masks/
+-rw-r--r--   0 desu      (1000) desu      (1000)      277 2023-11-27 19:37:46.000000 pycpio-0.9.2/src/pycpio/masks/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1378 2024-03-24 23:37:22.000000 pycpio-0.9.2/src/pycpio/masks/modes.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1499 2023-11-27 18:36:51.000000 pycpio-0.9.2/src/pycpio/masks/permissions.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     3704 2024-01-20 23:48:13.000000 pycpio-0.9.2/src/pycpio/pycpio.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.957554 pycpio-0.9.2/src/pycpio/reader/
+-rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:23.000000 pycpio-0.9.2/src/pycpio/reader/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     3700 2024-01-11 19:46:36.000000 pycpio-0.9.2/src/pycpio/reader/reader.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.958554 pycpio-0.9.2/src/pycpio/writer/
+-rw-r--r--   0 desu      (1000) desu      (1000)       57 2023-11-27 19:34:07.000000 pycpio-0.9.2/src/pycpio/writer/__init__.py
+-rw-r--r--   0 desu      (1000) desu      (1000)     1584 2024-03-24 22:50:18.000000 pycpio-0.9.2/src/pycpio/writer/writer.py
+drwxr-xr-x   0 desu      (1000) desu      (1000)        0 2024-04-15 01:11:07.958554 pycpio-0.9.2/src/pycpio.egg-info/
+-rw-r--r--   0 desu      (1000) desu      (1000)      648 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/PKG-INFO
+-rw-r--r--   0 desu      (1000) desu      (1000)      835 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/SOURCES.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        1 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/dependency_links.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       44 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/entry_points.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)       14 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/requires.txt
+-rw-r--r--   0 desu      (1000) desu      (1000)        7 2024-04-15 01:11:07.000000 pycpio-0.9.2/src/pycpio.egg-info/top_level.txt
```

### Comparing `pycpio-0.8.4/LICENSE` & `pycpio-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/PKG-INFO` & `pycpio-0.9.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pycpio
-Version: 0.8.4
+Version: 0.9.2
 Summary: A Python library for reading and writing cpio archives.
 Author-email: Desultory <dev@pyl.onl>
 Project-URL: Homepage, https://github.com/desultory/pycpio
 Project-URL: Issues, https://github.com/desultory/pycpio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zenlib>=1.6.4
+Requires-Dist: zenlib>=1.7.3
 
 # pycpio
 
 A library for working with CPIO files using python
 
 In active development
```

### Comparing `pycpio-0.8.4/pyproject.toml` & `pycpio-0.9.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycpio"
-version = "0.8.4"
+version = "0.9.2"
 authors = [
   { name="Desultory", email="dev@pyl.onl" },
 ]
 description = "A Python library for reading and writing cpio archives."
 readme = "readme.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
     "Operating System :: OS Independent",
 ]
-dependencies = ["zenlib >= 1.6.4"]
+dependencies = ["zenlib >= 1.7.3"]
 
 [project.scripts]
 pycpio = "pycpio.main:main"
 
 [project.urls]
 Homepage = "https://github.com/desultory/pycpio"
 Issues = "https://github.com/desultory/pycpio/issues"
```

### Comparing `pycpio-0.8.4/src/pycpio/cpio/archive.py` & `pycpio-0.9.2/src/pycpio/cpio/archive.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/cpio/chardev.py` & `pycpio-0.9.2/src/pycpio/cpio/chardev.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/cpio/data.py` & `pycpio-0.9.2/src/pycpio/cpio/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     self.hash is the sha256 hash of the data.
     """
     @staticmethod
     def from_dir(path: Path, parent=None, relative=None, *args, **kwargs):
         """
         Returns a list of CPIOData objects from a directory
 
-        If the path is a symlink, it will be resolved and the resolved path will be used.
+        Resolves the path and checks if it is a directory.
 
         If relative is set, the name will be relative to that path.
         The path will be unaltered, since it is used for header stats and data.
         """
         path = Path(path).resolve()
         if not path.is_dir():
             raise ValueError("Path is not a directory: %s" % path)
@@ -50,15 +50,15 @@
                 child_path = child
 
             if relative:
                 kwargs['name'] = str(child_path.relative_to(relative))
             else:
                 kwargs['name'] = str(child_path)
 
-            if child.is_dir():
+            if child.is_dir() and not child.is_symlink():
                 data.extend(CPIOData.from_dir(path=child_path, parent=parent, relative=relative, *args, **kwargs))
             else:
                 data.append(CPIOData.from_path(path=child_path, relative=relative, *args, **kwargs))
         return data
 
     @staticmethod
     def from_path(path: Path, relative=None, *args, **kwargs):
@@ -177,15 +177,15 @@
                 from hashlib import sha256
                 self.hash = sha256(value).hexdigest()
             self.header.filesize = len(value)
 
     def __init__(self, data: bytes, header, *args, **kwargs):
         self.header = header
         self.hash = None
-        self.data = data
+        self.data = data if data is not None else b''
 
     def __str__(self):
         return f"\n{self.header}\nSHA256: {self.hash}\n{self.__class__.__name__}"
 
     def __bytes__(self):
         """ Convert the data to bytes """
         return bytes(self.header) + self.data
```

### Comparing `pycpio-0.8.4/src/pycpio/cpio/dir.py` & `pycpio-0.9.2/src/pycpio/cpio/dir.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/cpio/file.py` & `pycpio-0.9.2/src/pycpio/cpio/file.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/cpio/symlink.py` & `pycpio-0.9.2/src/pycpio/cpio/symlink.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/header/cpioheader.py` & `pycpio-0.9.2/src/pycpio/header/cpioheader.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/header/header_funcs.py` & `pycpio-0.9.2/src/pycpio/header/header_funcs.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/masks/modes.py` & `pycpio-0.9.2/src/pycpio/masks/modes.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,18 @@
     raise ValueError(f"Invalid mode: {mode}")
 
 
 def mode_bytes_from_path(file_path: Path) -> CPIOModes:
     """
     Gets the mode type bytes from the given path.
     """
-    if file_path.is_dir():
-        return CPIOModes.Dir.value
-    elif file_path.is_symlink():
+    if file_path.is_symlink():
         return CPIOModes.Symlink.value
+    elif file_path.is_dir():
+        return CPIOModes.Dir.value
     elif file_path.is_block_device():
         return CPIOModes.BlkDev.value
     elif file_path.is_char_device():
         return CPIOModes.CharDev.value
     elif file_path.is_fifo():
         return CPIOModes.FIFO.value
     elif file_path.is_file():
```

### Comparing `pycpio-0.8.4/src/pycpio/masks/permissions.py` & `pycpio-0.9.2/src/pycpio/masks/permissions.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/pycpio.py` & `pycpio-0.9.2/src/pycpio/pycpio.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self.structure = structure
         self.overrides = {}
         self.entries = CPIOArchive(self.structure, logger=self.logger, _log_init=False)
 
         for attr in self.structure:
             if value := kwargs.pop(attr, None):
                 self.logger.info("[%s] Setting override: %s" % (attr, value))
+                self.overrides[attr] = value
 
     def append_cpio(self, path: Path, name: str = None, *args, **kwargs):
         """ Appends a file or directory to the CPIO archive. """
         kwargs.update({'path': path, 'structure': self.structure, 'overrides': self.overrides,
                        'logger': self.logger, '_log_init': False})
         if name:
             kwargs['name'] = name
```

### Comparing `pycpio-0.8.4/src/pycpio/reader/reader.py` & `pycpio-0.9.2/src/pycpio/reader/reader.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio/writer/writer.py` & `pycpio-0.9.2/src/pycpio/writer/writer.py`

 * *Files identical despite different names*

### Comparing `pycpio-0.8.4/src/pycpio.egg-info/PKG-INFO` & `pycpio-0.9.2/src/pycpio.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: pycpio
-Version: 0.8.4
+Version: 0.9.2
 Summary: A Python library for reading and writing cpio archives.
 Author-email: Desultory <dev@pyl.onl>
 Project-URL: Homepage, https://github.com/desultory/pycpio
 Project-URL: Issues, https://github.com/desultory/pycpio/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: zenlib>=1.6.4
+Requires-Dist: zenlib>=1.7.3
 
 # pycpio
 
 A library for working with CPIO files using python
 
 In active development
```

### Comparing `pycpio-0.8.4/src/pycpio.egg-info/SOURCES.txt` & `pycpio-0.9.2/src/pycpio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

