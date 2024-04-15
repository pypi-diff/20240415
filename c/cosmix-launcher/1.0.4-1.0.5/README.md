# Comparing `tmp/cosmix_launcher-1.0.4.tar.gz` & `tmp/cosmix_launcher-1.0.5.tar.gz`

## Comparing `cosmix_launcher-1.0.4.tar` & `cosmix_launcher-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/cosmix.bat
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/license.txt
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/requirements.txt
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/scripts/publish.sh
--rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/scripts/test.sh
--rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/__main__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/config.py
--rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/instance.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/logger.py
--rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/maven.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/mod.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/net.py
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/paths.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/src/cosmix/api/versions.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/.gitignore
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/readme.md
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/cosmix.bat
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/license.txt
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/requirements.txt
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/scripts/publish.sh
+-rwxr-xr-x   0        0        0      343 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/scripts/test.sh
+-rw-r--r--   0        0        0     5117 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/__main__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/config.py
+-rw-r--r--   0        0        0     5516 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/instance.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/logger.py
+-rw-r--r--   0        0        0     2564 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/maven.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/mod.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/net.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/paths.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/src/cosmix/api/versions.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/.gitignore
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/readme.md
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 cosmix_launcher-1.0.5/PKG-INFO
```

### Comparing `cosmix_launcher-1.0.4/license.txt` & `cosmix_launcher-1.0.5/license.txt`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/__main__.py` & `cosmix_launcher-1.0.5/src/cosmix/__main__.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/config.py` & `cosmix_launcher-1.0.5/src/cosmix/api/config.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/instance.py` & `cosmix_launcher-1.0.5/src/cosmix/api/instance.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,26 +11,20 @@
 import java_manifest
 import shutil
 
 
 __all__ = (
     "VALID_INSTANCE_NAME",
     "COSMIC_ARCHIVE_RAW_URL",
-    "COSMIC_QUILT_ARGS",
     "Instance",
 )
 
 
 VALID_INSTANCE_NAME = re.compile(r"[a-zA-Z0-9_-]*")
 COSMIC_ARCHIVE_RAW_URL = "https://raw.githubusercontent.com/CRModders/CosmicArchive/main"
-COSMIC_QUILT_ARGS = [
-    "-classpath",
-    f".{os.path.sep}deps{os.path.sep}*",
-    "org.quiltmc.loader.impl.launch.knot.KnotClient"
-]
 
 
 class Instance:
     def __init__(
         self,
         instance_name: str,
         cosmic_reach_version: str,
@@ -47,23 +41,30 @@
 
     def is_modded(self) -> bool:
         return self.quilt_version is not None
 
     def path_to(self, path: str) -> str:
         return os.path.join(self.path, path)
 
+    def get_classpath(self) -> str:
+        path = self.path_to("deps")
+        return ":".join([os.path.join(path, dep) for dep in os.listdir(path)])
+
     def launch(self, launch_args: Optional[list[str]] = None):
         os.chdir(self.path)
 
         args = ["java"]
         if not self.is_modded():
             args.extend(["-jar", paths.path_to_cr(self.version)])
         else:
-            args.append("-Dloader.gameJarPath=" + paths.path_to_cr(self.version))
-            args.extend(COSMIC_QUILT_ARGS)
+            args.extend([
+                "-Dloader.gameJarPath=" + paths.path_to_cr(self.version),
+                "-classpath", self.get_classpath(),
+                "org.quiltmc.loader.impl.launch.knot.KnotClient"
+            ])
         args.extend(self.args)
         args.extend(launch_args)
 
         logger.info(f"Launching \"{self.display_name}\" ({self.name}) with args {args} in folder {self.path}")
         os.execvp("java", args)
 
     def download(self, is_updating: bool = False):
```

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/logger.py` & `cosmix_launcher-1.0.5/src/cosmix/api/logger.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/maven.py` & `cosmix_launcher-1.0.5/src/cosmix/api/maven.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/mod.py` & `cosmix_launcher-1.0.5/src/cosmix/api/mod.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/net.py` & `cosmix_launcher-1.0.5/src/cosmix/api/net.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/src/cosmix/api/versions.py` & `cosmix_launcher-1.0.5/src/cosmix/api/versions.py`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/pyproject.toml` & `cosmix_launcher-1.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cosmix-launcher"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     { name = "EmmaTheMartian", email="emmathemartian@gmail.com" },
 ]
 description = "A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt"
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `cosmix_launcher-1.0.4/readme.md` & `cosmix_launcher-1.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `cosmix_launcher-1.0.4/PKG-INFO` & `cosmix_launcher-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cosmix-launcher
-Version: 1.0.4
+Version: 1.0.5
 Summary: A dead simple CLI-based launcher for Cosmic Reach and Cosmic Quilt
 Project-URL: Homepage, https://codeberg.org/EmmaTheMartian/cosmix
 Project-URL: Issues, https://codeberg.org/EmmaTheMartian/cosmix/issues
 Author-email: EmmaTheMartian <emmathemartian@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

