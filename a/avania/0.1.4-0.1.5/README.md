# Comparing `tmp/avania-0.1.4.tar.gz` & `tmp/avania-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.1.4.tar", last modified: Mon Apr 15 07:10:28 2024, max compression
+gzip compressed data, was "avania-0.1.5.tar", last modified: Mon Apr 15 07:19:34 2024, max compression
```

## Comparing `avania-0.1.4.tar` & `avania-0.1.5.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.639489 avania-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:10:19.000000 avania-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:10:28.639489 avania-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:10:19.000000 avania-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:10:19.000000 avania-0.1.4/avania/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/orm/driver/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/orm/driver/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/mysqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/sys/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/sys/config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/sys/os/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/os/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/os/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.639489 avania-0.1.4/avania/sys/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/prompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.639489 avania-0.1.4/avania.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:10:28.639489 avania-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:10:19.000000 avania-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:19:26.000000 avania-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:19:34.697524 avania-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:19:26.000000 avania-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.693524 avania-0.1.5/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:19:26.000000 avania-0.1.5/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.693524 avania-0.1.5/avania/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.693524 avania-0.1.5/avania/orm/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/orm/driver/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/mysqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/config/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/templates/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/os/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/os/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/os/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/prompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:19:34.697524 avania-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:19:26.000000 avania-0.1.5/setup.py
```

### Comparing `avania-0.1.4/LICENSE` & `avania-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.1.4/PKG-INFO` & `avania-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.4/README.md` & `avania-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.1.4/avania/orm/driver/mysql/database.py` & `avania-0.1.5/avania/orm/driver/mysql/database.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.4/avania/orm/driver/mysql/mate.py` & `avania-0.1.5/avania/orm/driver/mysql/mate.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.4/avania/orm/driver/mysql/mysqli.py` & `avania-0.1.5/avania/orm/driver/mysql/mysqli.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.4/avania/sys/config/meta.py` & `avania-0.1.5/avania/sys/config/meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         from avania.sys.os import os
         self.template_base_path = os.avania__path__()
         return self
 
     @classmethod
     def check_folder(self):
         from avania.sys.os import os
-        if not os.listdir(self.path):
+        if not os.hasdir(self.path):
             self.create_folder()
         return self
     
     @classmethod
     def create_folder(self):
         from avania.sys.os import os
         if os.mkdir(self.path, inquirer=True, inquirer_message="Create config folder? [Y/n] ", verbose=True):
```

### Comparing `avania-0.1.4/avania/sys/os/os.py` & `avania-0.1.5/avania/sys/os/os.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,26 @@
                 prompt.print("Failed to create directory: %s" % path, "red")
             return False
 
     @classmethod
     def create_file(self, path, content):
         import os
         from avania.sys.prompt import prompt
-        prompt.print("test")
+        prompt.print("test")     
+
+    @classmethod
+    def hasdir(self, path, verbose=False):
+        try:
+            import os
+            return os.path.isdir(path)
+        except:
+            from avania.sys.prompt import prompt
+            if verbose:
+                prompt.print("Failed to check if path is directory: %s" % path, color="red")
+            return False
 
     @classmethod
     def listdir(self, path, verbose=False, fail_message=None):
         if fail_message is None:
             fail_message = "Failed to list directory: %s" % path
         try:
             import os
```

### Comparing `avania-0.1.4/avania/sys/prompt/prompt.py` & `avania-0.1.5/avania/sys/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.4/avania.egg-info/PKG-INFO` & `avania-0.1.5/avania.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.4/avania.egg-info/SOURCES.txt` & `avania-0.1.5/avania.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,14 @@
 avania/orm/driver/mysql/database.py
 avania/orm/driver/mysql/mate.py
 avania/orm/driver/mysql/mysqli.py
 avania/sys/__init__.py
 avania/sys/config/__init__.py
 avania/sys/config/config.py
 avania/sys/config/meta.py
+avania/sys/config/templates/__init__.py
+avania/sys/config/templates/database.py
 avania/sys/os/__init__.py
 avania/sys/os/config.py
 avania/sys/os/os.py
 avania/sys/prompt/__init__.py
 avania/sys/prompt/prompt.py
```

