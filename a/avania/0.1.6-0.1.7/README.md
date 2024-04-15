# Comparing `tmp/avania-0.1.6.tar.gz` & `tmp/avania-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.1.6.tar", last modified: Mon Apr 15 07:24:26 2024, max compression
+gzip compressed data, was "avania-0.1.7.tar", last modified: Mon Apr 15 07:43:24 2024, max compression
```

## Comparing `avania-0.1.6.tar` & `avania-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.562609 avania-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:24:16.000000 avania-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:24:26.562609 avania-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:24:16.000000 avania-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:24:16.000000 avania-0.1.6/avania/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/orm/driver/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/orm/driver/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:24:16.000000 avania-0.1.6/avania/orm/driver/mysql/mysqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/config/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/config/templates/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.558609 avania-0.1.6/avania/sys/os/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/os/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/os/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.562609 avania-0.1.6/avania/sys/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:24:16.000000 avania-0.1.6/avania/sys/prompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:24:26.562609 avania-0.1.6/avania.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:24:26.000000 avania-0.1.6/avania.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:24:26.562609 avania-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:24:16.000000 avania-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:43:14.000000 avania-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:43:24.582499 avania-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:43:14.000000 avania-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.578499 avania-0.1.7/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:43:14.000000 avania-0.1.7/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.578499 avania-0.1.7/avania/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:43:14.000000 avania-0.1.7/avania/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.578499 avania-0.1.7/avania/orm/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:43:14.000000 avania-0.1.7/avania/orm/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania/orm/driver/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:43:14.000000 avania-0.1.7/avania/orm/driver/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:43:14.000000 avania-0.1.7/avania/orm/driver/mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:43:14.000000 avania-0.1.7/avania/orm/driver/mysql/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:43:14.000000 avania-0.1.7/avania/orm/driver/mysql/mysqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania/sys/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania/sys/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania/sys/config/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/config/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/config/templates/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania/sys/os/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/os/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/os/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania/sys/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-15 07:43:14.000000 avania-0.1.7/avania/sys/prompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:43:24.582499 avania-0.1.7/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:43:24.000000 avania-0.1.7/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-15 07:43:24.000000 avania-0.1.7/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:43:24.000000 avania-0.1.7/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:43:24.000000 avania-0.1.7/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:43:24.000000 avania-0.1.7/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:43:24.582499 avania-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:43:14.000000 avania-0.1.7/setup.py
```

### Comparing `avania-0.1.6/LICENSE` & `avania-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.1.6/PKG-INFO` & `avania-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.6/README.md` & `avania-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.1.6/avania/orm/driver/mysql/database.py` & `avania-0.1.7/avania/orm/driver/mysql/database.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.6/avania/orm/driver/mysql/mate.py` & `avania-0.1.7/avania/orm/driver/mysql/mate.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.6/avania/orm/driver/mysql/mysqli.py` & `avania-0.1.7/avania/orm/driver/mysql/mysqli.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.6/avania/sys/config/meta.py` & `avania-0.1.7/avania/sys/config/meta.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,40 +29,42 @@
         if os.mkdir(self.path, inquirer=True, inquirer_message="Create config folder? [Y/n] ", verbose=True):
             self.create_templates()
         
 
     @classmethod
     def create_templates(self):
         from avania.sys.prompt import prompt
-        # 询问是否创建模板文件
-        # 如果create的为True
         if prompt.prompt("Create all template files? [Y/n] ", default=True):
             from avania.sys.os import os
             # 从avania/config/templates中复制所有文件到config文件夹
             for file in os.listdir(f'{self.template_base_path}{self.template_path}'):
-                # 创建文件
-                self.create_template(file.replace('.py', ''), inquirer=False)
+                # 如果不是__init__.py文件
+                if file != '__init__.py':
+                    # 创建文件
+                    self.create_template(file.replace('.py', ''), inquirer=False)
         
     @classmethod
     def create_template(self, name, inquirer = True, verbose = True):
         from avania.sys.os import os
         from avania.sys.os.config import git_url
         from avania.sys.prompt import prompt
-        if self.first and verbose:
-            verbose = False
-        return os.cp(f'{self.template_base_path}{self.template_path}/{name}.py', f'config/{name}.py', verbose=verbose, inquirer=inquirer, inquirer_message=f'Create {name}.json? [Y/n] ',
-              success_message=f'Created {name}.py', fail_message=f'Failed to create {name}.py')
+        if self.first and inquirer:
+            prompt.print(f'Failed to find {name}.py in config folder', 'red')
+            return False
+        return os.cp(f'{self.template_base_path}{self.template_path}/{name}.py', f'config/{name}.py', verbose=verbose, 
+                     inquirer=inquirer, inquirer_message=f'Create {name}.json? [Y/n] ',
+                     success_message=f'Created {name}.py', fail_message=f'Failed to create {name}.py')
 
     @classmethod
     def get_file(self, name):
         from avania.sys.os import os
         result = os.read(f'{self.path}/{name}.py')
         if not result:
             if self.create_template(name):
-                return self.get(name)
+                return self.get_file(name)
             else:
                 return None
         else:
             return result
 
     # 解析python文件的内容，返回一个JSON对象
     # 文件内容为xxx=xxx
```

### Comparing `avania-0.1.6/avania/sys/os/os.py` & `avania-0.1.7/avania/sys/os/os.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,25 @@
             if verbose:
                 prompt.print("Failed to check if path exists: %s" % path, "red")
             return False
         
     @classmethod
     def cp(self, copied_file, new_file, verbose=False, inquirer=False, inquirer_message=None, inquirer_color="blue",
            overwrite=False, success_message=None, fail_message=None):
+        from avania.sys.prompt import prompt
         if not self.exists(copied_file, verbose=verbose):
+            if verbose:
+                prompt.print("File %s does not exist" % copied_file, "red")
+                prompt.print_github()
             return False
         if success_message is None:
             success_message = "Copied %s to %s" % (copied_file, new_file)
         if fail_message is None:
             fail_message = "Failed to copy %s to %s" % (copied_file, new_file)
         if not overwrite and self.exists(new_file, verbose=verbose):
-            from avania.sys.prompt import prompt
             if verbose:
                 prompt.print("File %s already exists" % new_file, "yellow")
             return False
         if inquirer_message is None:
             inquirer_message = "Copy %s to %s? [Y/n] " % (copied_file, new_file)
         try:
             import os
```

### Comparing `avania-0.1.6/avania/sys/prompt/prompt.py` & `avania-0.1.7/avania/sys/prompt/prompt.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,12 @@
         if response == "":
             return default
         elif response.lower() in ["y", "yes"]:
             return True
         elif response.lower() in ["n", "no"]:
             return False
         else:
-            return prompt(message, default, color)
+            return prompt(message, default, color)
+        
+    @classmethod
+    def print_github(self):
+        prompt.print("Please visit https://github.com/StarLxa/avania-core for more information", "green")
```

### Comparing `avania-0.1.6/avania.egg-info/PKG-INFO` & `avania-0.1.7/avania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.6
+Version: 0.1.7
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.6/avania.egg-info/SOURCES.txt` & `avania-0.1.7/avania.egg-info/SOURCES.txt`

 * *Files identical despite different names*

