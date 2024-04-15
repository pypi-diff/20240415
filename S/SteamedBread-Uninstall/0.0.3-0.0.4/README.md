# Comparing `tmp/SteamedBread-Uninstall-0.0.3.tar.gz` & `tmp/SteamedBread-Uninstall-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SteamedBread-Uninstall-0.0.3.tar", last modified: Sun Mar 31 16:09:59 2024, max compression
+gzip compressed data, was "SteamedBread-Uninstall-0.0.4.tar", last modified: Mon Apr 15 15:19:18 2024, max compression
```

## Comparing `SteamedBread-Uninstall-0.0.3.tar` & `SteamedBread-Uninstall-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 chocolate   (501) staff       (20)        0 2024-03-31 16:09:59.850300 SteamedBread-Uninstall-0.0.3/
--rw-r--r--   0 chocolate   (501) staff       (20)    11357 2024-03-26 15:15:45.000000 SteamedBread-Uninstall-0.0.3/LICENSE
--rw-r--r--   0 chocolate   (501) staff       (20)      794 2024-03-31 16:09:59.850172 SteamedBread-Uninstall-0.0.3/PKG-INFO
--rw-r--r--   0 chocolate   (501) staff       (20)      449 2024-03-26 16:02:49.000000 SteamedBread-Uninstall-0.0.3/README.md
-drwxr-xr-x   0 chocolate   (501) staff       (20)        0 2024-03-31 16:09:59.849664 SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/
--rw-r--r--   0 chocolate   (501) staff       (20)      794 2024-03-31 16:09:59.000000 SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/PKG-INFO
--rw-r--r--   0 chocolate   (501) staff       (20)      328 2024-03-31 16:09:59.000000 SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/SOURCES.txt
--rw-r--r--   0 chocolate   (501) staff       (20)        1 2024-03-31 16:09:59.000000 SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/dependency_links.txt
--rw-r--r--   0 chocolate   (501) staff       (20)       80 2024-03-31 16:09:59.000000 SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/entry_points.txt
--rw-r--r--   0 chocolate   (501) staff       (20)       19 2024-03-31 16:09:59.000000 SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/top_level.txt
-drwxr-xr-x   0 chocolate   (501) staff       (20)        0 2024-03-31 16:09:59.849862 SteamedBread-Uninstall-0.0.3/_CleanPackageTools/
--rw-r--r--   0 chocolate   (501) staff       (20)     4909 2024-03-31 16:07:46.000000 SteamedBread-Uninstall-0.0.3/_CleanPackageTools/CleanDependence.py
--rw-r--r--   0 chocolate   (501) staff       (20)      152 2024-03-26 15:35:53.000000 SteamedBread-Uninstall-0.0.3/_CleanPackageTools/__init__.py
--rw-r--r--   0 chocolate   (501) staff       (20)       38 2024-03-31 16:09:59.850348 SteamedBread-Uninstall-0.0.3/setup.cfg
--rw-r--r--   0 chocolate   (501) staff       (20)      865 2024-03-31 15:55:06.000000 SteamedBread-Uninstall-0.0.3/setup.py
+drwxr-xr-x   0 chocolate   (501) staff       (20)        0 2024-04-15 15:19:18.165683 SteamedBread-Uninstall-0.0.4/
+-rw-r--r--   0 chocolate   (501) staff       (20)    11357 2024-03-26 15:15:45.000000 SteamedBread-Uninstall-0.0.4/LICENSE
+-rw-r--r--   0 chocolate   (501) staff       (20)      794 2024-04-15 15:19:18.165581 SteamedBread-Uninstall-0.0.4/PKG-INFO
+-rw-r--r--   0 chocolate   (501) staff       (20)      449 2024-03-26 16:02:49.000000 SteamedBread-Uninstall-0.0.4/README.md
+drwxr-xr-x   0 chocolate   (501) staff       (20)        0 2024-04-15 15:19:18.165158 SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/
+-rw-r--r--   0 chocolate   (501) staff       (20)      794 2024-04-15 15:19:18.000000 SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/PKG-INFO
+-rw-r--r--   0 chocolate   (501) staff       (20)      328 2024-04-15 15:19:18.000000 SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/SOURCES.txt
+-rw-r--r--   0 chocolate   (501) staff       (20)        1 2024-04-15 15:19:18.000000 SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/dependency_links.txt
+-rw-r--r--   0 chocolate   (501) staff       (20)       80 2024-04-15 15:19:18.000000 SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/entry_points.txt
+-rw-r--r--   0 chocolate   (501) staff       (20)       19 2024-04-15 15:19:18.000000 SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/top_level.txt
+drwxr-xr-x   0 chocolate   (501) staff       (20)        0 2024-04-15 15:19:18.165345 SteamedBread-Uninstall-0.0.4/_CleanPackageTools/
+-rw-r--r--   0 chocolate   (501) staff       (20)     4934 2024-04-15 15:18:45.000000 SteamedBread-Uninstall-0.0.4/_CleanPackageTools/CleanDependence.py
+-rw-r--r--   0 chocolate   (501) staff       (20)      152 2024-03-26 15:35:53.000000 SteamedBread-Uninstall-0.0.4/_CleanPackageTools/__init__.py
+-rw-r--r--   0 chocolate   (501) staff       (20)       38 2024-04-15 15:19:18.165717 SteamedBread-Uninstall-0.0.4/setup.cfg
+-rw-r--r--   0 chocolate   (501) staff       (20)      865 2024-03-31 15:55:06.000000 SteamedBread-Uninstall-0.0.4/setup.py
```

### Comparing `SteamedBread-Uninstall-0.0.3/LICENSE` & `SteamedBread-Uninstall-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SteamedBread-Uninstall-0.0.3/PKG-INFO` & `SteamedBread-Uninstall-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SteamedBread-Uninstall
-Version: 0.0.3
+Version: 0.0.4
 Summary: 馒头的三方库管理器
 Home-page: https://github.com/neihanshenshou/SteamedBreadPackageManager
 Author: 馒头
 Author-email: neihanshenshou@163.com
 License: Apache License 2.0
 Platform: MacOS、Window
 Description-Content-Type: text/markdown
```

### Comparing `SteamedBread-Uninstall-0.0.3/SteamedBread_Uninstall.egg-info/PKG-INFO` & `SteamedBread-Uninstall-0.0.4/SteamedBread_Uninstall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SteamedBread-Uninstall
-Version: 0.0.3
+Version: 0.0.4
 Summary: 馒头的三方库管理器
 Home-page: https://github.com/neihanshenshou/SteamedBreadPackageManager
 Author: 馒头
 Author-email: neihanshenshou@163.com
 License: Apache License 2.0
 Platform: MacOS、Window
 Description-Content-Type: text/markdown
```

### Comparing `SteamedBread-Uninstall-0.0.3/_CleanPackageTools/CleanDependence.py` & `SteamedBread-Uninstall-0.0.4/_CleanPackageTools/CleanDependence.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,33 +8,32 @@
 
 import optparse
 import subprocess
 import sys
 
 from pkg_resources import working_set, get_distribution, VersionConflict, DistributionNotFound
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 # 不允许卸载
-WHITELIST = ["pip", "pip3", "setuptools"]
+WHITELIST = ["pip", "pip3", "setuptools", "SteamedBread-Uninstall"]
 
 
 def auto_remove(names, yes=False):
     dead = list_dead(names)
     names = [d.project_name for d in dead]
     print(f"你要卸载的三方库及其子依赖: {names}")
     if dead and (yes or confirm("Uninstall (Y/N) or (y/n)? ")):
         remove_dists(dead)
 
 
 def list_dead(names):
     start = set()
     for name in names:
         try:
-
             start.add(get_distribution(name))
         except DistributionNotFound:
             print("未在pip 模块下找到 %s , 跳过" % name, file=sys.stderr)
         except VersionConflict:
             print("%s is not the currently installed version, skipping" % name, file=sys.stderr)
     graph = get_graph()
     dead = exclude_whitelist(find_all_dead(graph, start))
```

### Comparing `SteamedBread-Uninstall-0.0.3/setup.py` & `SteamedBread-Uninstall-0.0.4/setup.py`

 * *Files identical despite different names*

