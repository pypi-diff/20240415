# Comparing `tmp/avania-0.1.1.tar.gz` & `tmp/avania-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.1.1.tar", last modified: Mon Apr 15 04:46:45 2024, max compression
+gzip compressed data, was "avania-0.1.2.tar", last modified: Mon Apr 15 07:02:44 2024, max compression
```

## Comparing `avania-0.1.1.tar` & `avania-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.395943 avania-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 04:46:35.000000 avania-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 04:46:45.395943 avania-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 04:46:35.000000 avania-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 04:46:35.000000 avania-0.1.1/avania/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/orm/driver/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/orm/driver/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 04:46:35.000000 avania-0.1.1/avania/orm/driver/mysql/mysqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/os/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/os/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/os/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania/sys/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 04:46:35.000000 avania-0.1.1/avania/sys/prompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 04:46:45.391944 avania-0.1.1/avania.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 04:46:45.000000 avania-0.1.1/avania.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 04:46:45.395943 avania-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 04:46:35.000000 avania-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:02:33.000000 avania-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:02:44.109703 avania-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:02:33.000000 avania-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.105703 avania-0.1.2/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:02:33.000000 avania-0.1.2/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.105703 avania-0.1.2/avania/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.105703 avania-0.1.2/avania/orm/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/orm/driver/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/mysqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/os/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/os/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/os/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/prompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:02:44.109703 avania-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:02:33.000000 avania-0.1.2/setup.py
```

### Comparing `avania-0.1.1/LICENSE` & `avania-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.1.1/PKG-INFO` & `avania-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.1/README.md` & `avania-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.1.1/avania/orm/driver/mysql/database.py` & `avania-0.1.2/avania/orm/driver/mysql/database.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.1/avania/orm/driver/mysql/mate.py` & `avania-0.1.2/avania/orm/driver/mysql/mate.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.1/avania/orm/driver/mysql/mysqli.py` & `avania-0.1.2/avania/orm/driver/mysql/mysqli.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.1/avania/sys/config/meta.py` & `avania-0.1.2/avania/sys/config/meta.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,56 @@
 class ConfigMetaClass(type):
     path = 'config'
+    template_base_path = '/'
+    template_path = '/sys/config/templates'
 
     def __new__(cls, name, bases, attrs):
+        cls.update_template_base_path()
         cls.check_folder()
         return type.__new__(cls, name, bases, attrs)
     
     @classmethod
+    def update_template_base_path(self):
+        from avania.sys.os import os
+        self.template_base_path = os.avania__path__()
+        return self
+
+    @classmethod
     def check_folder(self):
         from avania.sys.os import os
         if not os.listdir(self.path):
             self.create_folder()
         return self
     
     @classmethod
     def create_folder(self):
         from avania.sys.os import os
-        os.mkdir(self.path, inquirer=True, inquirer_message="Create config folder? [Y/n] ", verbose=True)
-        self.create_templates()
+        if os.mkdir(self.path, inquirer=True, inquirer_message="Create config folder? [Y/n] ", verbose=True):
+            self.create_templates()
         
 
     @classmethod
     def create_templates(self):
         from avania.sys.prompt import prompt
         # 询问是否创建模板文件
         # 如果create的为True
-        if prompt.prompt("Create template files? [Y/n] ", default=True):
+        if prompt.prompt("Create all template files? [Y/n] ", default=True):
             from avania.sys.os import os
             # 从avania/config/templates中复制所有文件到config文件夹
             for file in os.listdir('avania/sys/config/templates'):
                 # 创建文件
                 self.create_template(file.replace('.py', ''), inquirer=False)
         
     @classmethod
     def create_template(self, name, inquirer = True, verbose = True):
         from avania.sys.os import os
         from avania.sys.os.config import git_url
         from avania.sys.prompt import prompt
-        return os.cp(f'avania/sys/config/templates/{name}.py', f'config/{name}.py', verbose=verbose, inquirer=inquirer, inquirer_message=f'Create {name}.json? [Y/n] ',
-              success_message=f'Created {name}.json', fail_message=f'Failed to create {name}.json')
+        return os.cp(f'{self.template_base_path}{self.template_path}/{name}.py', f'config/{name}.py', verbose=verbose, inquirer=inquirer, inquirer_message=f'Create {name}.json? [Y/n] ',
+              success_message=f'Created {name}.py', fail_message=f'Failed to create {name}.py')
 
     @classmethod
     def get_file(self, name):
         from avania.sys.os import os
         result = os.read(f'{self.path}/{name}.py')
         if not result:
             if self.create_template(name):
```

### Comparing `avania-0.1.1/avania/sys/os/os.py` & `avania-0.1.2/avania/sys/os/os.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 prompt.print("Failed to create directory: %s" % path, "red")
             return False
 
     @classmethod
     def create_file(self, path, content):
         import os
         from avania.sys.prompt import prompt
-        prompt.print("eeee")
+        prompt.print("test")
 
     @classmethod
     def listdir(self, path, verbose=False, fail_message=None):
         if fail_message is None:
             fail_message = "Failed to list directory: %s" % path
         try:
             import os
@@ -91,8 +91,16 @@
                 return False
             with open(path) as f:
                 return f.read()
         except:
             from avania.sys.prompt import prompt
             if verbose:
                 prompt.print(fail_message, "red")
-            return False
+            return False
+        
+    @classmethod
+    def avania__path__(self):
+        try:
+            import os
+            return os.path.abspath(os.path.join(os.path.dirname(__file__), '../../..' + '/avania'))
+        except:
+            return f"./avania"
```

### Comparing `avania-0.1.1/avania/sys/prompt/prompt.py` & `avania-0.1.2/avania/sys/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.1/avania.egg-info/PKG-INFO` & `avania-0.1.2/avania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.1/avania.egg-info/SOURCES.txt` & `avania-0.1.2/avania.egg-info/SOURCES.txt`

 * *Files identical despite different names*

