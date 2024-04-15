# Comparing `tmp/tablemaster-1.2.0.tar.gz` & `tmp/tablemaster-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablemaster-1.2.0.tar", last modified: Wed Apr 10 06:00:54 2024, max compression
+gzip compressed data, was "tablemaster-1.2.1.tar", last modified: Mon Apr 15 07:00:28 2024, max compression
```

## Comparing `tablemaster-1.2.0.tar` & `tablemaster-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:54.241428 tablemaster-1.2.0/
--rw-rw-rw-   0        0        0    11558 2024-04-10 02:51:24.000000 tablemaster-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      468 2024-04-10 06:00:54.241428 tablemaster-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2692 2024-04-10 05:57:40.000000 tablemaster-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 06:00:54.241428 tablemaster-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      538 2024-04-10 05:46:29.000000 tablemaster-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:54.237437 tablemaster-1.2.0/tablemaster/
--rw-rw-rw-   0        0        0      671 2024-04-10 05:38:21.000000 tablemaster-1.2.0/tablemaster/__init__.py
--rw-rw-rw-   0        0        0     1749 2024-04-10 02:51:24.000000 tablemaster-1.2.0/tablemaster/feishu.py
--rw-rw-rw-   0        0        0     1170 2024-04-10 02:51:24.000000 tablemaster-1.2.0/tablemaster/gspread.py
--rw-rw-rw-   0        0        0     3427 2024-04-10 02:51:24.000000 tablemaster-1.2.0/tablemaster/local.py
--rw-rw-rw-   0        0        0     5913 2024-04-10 05:45:41.000000 tablemaster-1.2.0/tablemaster/mysql.py
--rw-rw-rw-   0        0        0      828 2024-04-10 02:51:24.000000 tablemaster-1.2.0/tablemaster/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-10 06:00:54.240426 tablemaster-1.2.0/tablemaster.egg-info/
--rw-rw-rw-   0        0        0      468 2024-04-10 06:00:54.000000 tablemaster-1.2.0/tablemaster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2024-04-10 06:00:54.000000 tablemaster-1.2.0/tablemaster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 06:00:54.000000 tablemaster-1.2.0/tablemaster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2024-04-10 06:00:54.000000 tablemaster-1.2.0/tablemaster.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 06:00:54.000000 tablemaster-1.2.0/tablemaster.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 07:00:28.285554 tablemaster-1.2.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-10 02:51:24.000000 tablemaster-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0      247 2024-04-15 07:00:28.284528 tablemaster-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2692 2024-04-10 05:57:40.000000 tablemaster-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-15 07:00:28.285554 tablemaster-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      538 2024-04-15 06:58:17.000000 tablemaster-1.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:00:28.280933 tablemaster-1.2.1/tablemaster/
+-rw-rw-rw-   0        0        0      671 2024-04-10 05:38:21.000000 tablemaster-1.2.1/tablemaster/__init__.py
+-rw-rw-rw-   0        0        0     1749 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/feishu.py
+-rw-rw-rw-   0        0        0     1170 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/gspread.py
+-rw-rw-rw-   0        0        0     3427 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/local.py
+-rw-rw-rw-   0        0        0     5913 2024-04-15 06:58:08.000000 tablemaster-1.2.1/tablemaster/mysql.py
+-rw-rw-rw-   0        0        0      828 2024-04-10 02:51:24.000000 tablemaster-1.2.1/tablemaster/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-15 07:00:28.284528 tablemaster-1.2.1/tablemaster.egg-info/
+-rw-rw-rw-   0        0        0      247 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 07:00:28.000000 tablemaster-1.2.1/tablemaster.egg-info/top_level.txt
```

### Comparing `tablemaster-1.2.0/LICENSE` & `tablemaster-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.0/README.md` & `tablemaster-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.0/setup.py` & `tablemaster-1.2.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tablemaster',
-    version='1.2.0',
+    version='1.2.1',
     packages=find_packages(),
     install_requires=[
         'PyMySQL',
         'SQLAlchemy',
         'pandas',
         'python-dateutil',
         'gspread',
```

### Comparing `tablemaster-1.2.0/tablemaster/__init__.py` & `tablemaster-1.2.1/tablemaster/__init__.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.0/tablemaster/feishu.py` & `tablemaster-1.2.1/tablemaster/feishu.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.0/tablemaster/gspread.py` & `tablemaster-1.2.1/tablemaster/gspread.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.0/tablemaster/local.py` & `tablemaster-1.2.1/tablemaster/local.py`

 * *Files identical despite different names*

### Comparing `tablemaster-1.2.0/tablemaster/mysql.py` & `tablemaster-1.2.1/tablemaster/mysql.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         except:
             print("table not found!")
 
     def delete_table(self):
         opt(f'DROP TABLE {self.table}', self)
         print(f'{self.table} deleted!')
 
-    def pal_del(self, clause):
+    def par_del(self, clause):
         del_clause = f"DELETE FROM {self.table} WHERE {clause}"
         opt(del_clause, self)
         print(f'records of table that {clause} are deleted!')
 
     def change_data_type(self, cols_name, data_type):
         change_clause = f'ALTER TABLE {self.table} MODIFY COLUMN {cols_name} {data_type}'
         opt(change_clause, self)
@@ -105,15 +105,15 @@
         except:
             print("table not found!")
 
     def delete_table(self):
         opt(f'DROP TABLE {self.table}', self)
         print(f'{self.table} deleted!')
 
-    def pal_del(self, clause):
+    def par_del(self, clause):
         del_clause = f"DELETE FROM {self.table} WHERE {clause}"
         opt(del_clause, self)
         print(f'records of table that {clause} are deleted!')
 
     def change_data_type(self, cols_name, data_type):
         change_clause = f'ALTER TABLE {self.table} MODIFY COLUMN {cols_name} {data_type}'
         opt(change_clause, self)
```

### Comparing `tablemaster-1.2.0/tablemaster/utils.py` & `tablemaster-1.2.1/tablemaster/utils.py`

 * *Files identical despite different names*

