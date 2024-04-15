# Comparing `tmp/avania-0.1.2.tar.gz` & `tmp/avania-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avania-0.1.2.tar", last modified: Mon Apr 15 07:02:44 2024, max compression
+gzip compressed data, was "avania-0.1.4.tar", last modified: Mon Apr 15 07:10:28 2024, max compression
```

## Comparing `avania-0.1.2.tar` & `avania-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:02:33.000000 avania-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:02:44.109703 avania-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:02:33.000000 avania-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.105703 avania-0.1.2/avania/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:02:33.000000 avania-0.1.2/avania/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.105703 avania-0.1.2/avania/orm/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.105703 avania-0.1.2/avania/orm/driver/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/orm/driver/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/mate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:02:33.000000 avania-0.1.2/avania/orm/driver/mysql/mysqli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/config/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/os/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/os/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/os/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania/sys/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:02:33.000000 avania-0.1.2/avania/sys/prompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:02:44.109703 avania-0.1.2/avania.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:02:44.000000 avania-0.1.2/avania.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:02:44.109703 avania-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:02:33.000000 avania-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.639489 avania-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-15 07:10:19.000000 avania-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:10:28.639489 avania-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-15 07:10:19.000000 avania-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-15 07:10:19.000000 avania-0.1.4/avania/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/orm/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/orm/driver/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/orm/driver/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/mate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 07:10:19.000000 avania-0.1.4/avania/orm/driver/mysql/mysqli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/sys/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/sys/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.635489 avania-0.1.4/avania/sys/os/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/os/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/os/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.639489 avania-0.1.4/avania/sys/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-15 07:10:19.000000 avania-0.1.4/avania/sys/prompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:10:28.639489 avania-0.1.4/avania.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 07:10:28.000000 avania-0.1.4/avania.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:10:28.639489 avania-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-15 07:10:19.000000 avania-0.1.4/setup.py
```

### Comparing `avania-0.1.2/LICENSE` & `avania-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/PKG-INFO` & `avania-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.2
+Version: 0.1.4
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.2/README.md` & `avania-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/avania/orm/driver/mysql/database.py` & `avania-0.1.4/avania/orm/driver/mysql/database.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/avania/orm/driver/mysql/mate.py` & `avania-0.1.4/avania/orm/driver/mysql/mate.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/avania/orm/driver/mysql/mysqli.py` & `avania-0.1.4/avania/orm/driver/mysql/mysqli.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/avania/sys/config/meta.py` & `avania-0.1.4/avania/sys/config/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     def create_templates(self):
         from avania.sys.prompt import prompt
         # 询问是否创建模板文件
         # 如果create的为True
         if prompt.prompt("Create all template files? [Y/n] ", default=True):
             from avania.sys.os import os
             # 从avania/config/templates中复制所有文件到config文件夹
-            for file in os.listdir('avania/sys/config/templates'):
+            for file in os.listdir(f'{self.template_base_path}{self.template_path}'):
                 # 创建文件
                 self.create_template(file.replace('.py', ''), inquirer=False)
         
     @classmethod
     def create_template(self, name, inquirer = True, verbose = True):
         from avania.sys.os import os
         from avania.sys.os.config import git_url
```

### Comparing `avania-0.1.2/avania/sys/os/os.py` & `avania-0.1.4/avania/sys/os/os.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/avania/sys/prompt/prompt.py` & `avania-0.1.4/avania/sys/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `avania-0.1.2/avania.egg-info/PKG-INFO` & `avania-0.1.4/avania.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avania
-Version: 0.1.2
+Version: 0.1.4
 Summary: Pays tribute to Laravel
 Author: Simon
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mysql-connector-python
 Requires-Dist: flask
```

### Comparing `avania-0.1.2/avania.egg-info/SOURCES.txt` & `avania-0.1.4/avania.egg-info/SOURCES.txt`

 * *Files identical despite different names*

