# Comparing `tmp/avania-0.1.5.tar.gz` & `tmp/avania-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.1.5.tar", last modified: Mon Apr 15 07:19:34 2024, max compression
+gzip compressed data, was "avania-0.1.6.tar", last modified: Mon Apr 15 07:24:26 2024, max compression
```

## Comparing `avania-0.1.5.tar` & `avania-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:19:26.000000 avania-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:19:34.697524 avania-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:19:26.000000 avania-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.693524 avania-0.1.5/avania/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:19:26.000000 avania-0.1.5/avania/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.693524 avania-0.1.5/avania/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.693524 avania-0.1.5/avania/orm/driver/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/orm/driver/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:19:26.000000 avania-0.1.5/avania/orm/driver/mysql/mysqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/config/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/config/templates/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/os/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/os/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/os/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania/sys/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:19:26.000000 avania-0.1.5/avania/sys/prompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:19:34.697524 avania-0.1.5/avania.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:19:34.000000 avania-0.1.5/avania.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:19:34.697524 avania-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:19:26.000000 avania-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.562609 avania-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:24:16.000000 avania-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:24:26.562609 avania-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:24:16.000000 avania-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:24:16.000000 avania-0.1.6/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/orm/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/orm/driver/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/mysqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/config/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/templates/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/os/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/os/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/os/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.562609 avania-0.1.6/avania/sys/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/prompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.562609 avania-0.1.6/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:24:26.562609 avania-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:24:16.000000 avania-0.1.6/setup.py
```

### Comparing `avania-0.1.5/LICENSE` & `avania-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/PKG-INFO` & `avania-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.5/README.md` & `avania-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/avania/orm/driver/mysql/database.py` & `avania-0.1.6/avania/orm/driver/mysql/database.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/avania/orm/driver/mysql/mate.py` & `avania-0.1.6/avania/orm/driver/mysql/mate.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/avania/orm/driver/mysql/mysqli.py` & `avania-0.1.6/avania/orm/driver/mysql/mysqli.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/avania/sys/config/meta.py` & `avania-0.1.6/avania/sys/config/meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 class ConfigMetaClass(type):
     path = 'config'
     template_base_path = '/'
     template_path = '/sys/config/templates'
+    first = False
 
     def __new__(cls, name, bases, attrs):
         cls.update_template_base_path()
         cls.check_folder()
         return type.__new__(cls, name, bases, attrs)
     
     @classmethod
@@ -14,14 +15,15 @@
         self.template_base_path = os.avania__path__()
         return self
 
     @classmethod
     def check_folder(self):
         from avania.sys.os import os
         if not os.hasdir(self.path):
+            self.first = True
             self.create_folder()
         return self
     
     @classmethod
     def create_folder(self):
         from avania.sys.os import os
         if os.mkdir(self.path, inquirer=True, inquirer_message="Create config folder? [Y/n] ", verbose=True):
@@ -41,14 +43,16 @@
                 self.create_template(file.replace('.py', ''), inquirer=False)
         
     @classmethod
     def create_template(self, name, inquirer = True, verbose = True):
         from avania.sys.os import os
         from avania.sys.os.config import git_url
         from avania.sys.prompt import prompt
+        if self.first and verbose:
+            verbose = False
         return os.cp(f'{self.template_base_path}{self.template_path}/{name}.py', f'config/{name}.py', verbose=verbose, inquirer=inquirer, inquirer_message=f'Create {name}.json? [Y/n] ',
               success_message=f'Created {name}.py', fail_message=f'Failed to create {name}.py')
 
     @classmethod
     def get_file(self, name):
         from avania.sys.os import os
         result = os.read(f'{self.path}/{name}.py')
```

### Comparing `avania-0.1.5/avania/sys/os/os.py` & `avania-0.1.6/avania/sys/os/os.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/avania/sys/prompt/prompt.py` & `avania-0.1.6/avania/sys/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.5/avania.egg-info/PKG-INFO` & `avania-0.1.6/avania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.5
+Version: 0.1.6
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.5/avania.egg-info/SOURCES.txt` & `avania-0.1.6/avania.egg-info/SOURCES.txt`

 * *Files identical despite different names*

