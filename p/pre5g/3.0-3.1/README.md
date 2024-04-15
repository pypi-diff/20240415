# Comparing `tmp/pre5g-3.0.tar.gz` & `tmp/pre5g-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-3.0.tar", last modified: Mon Apr 15 10:03:19 2024, max compression
+gzip compressed data, was "dist/pre5g-3.1.tar", last modified: Mon Apr 15 11:14:53 2024, max compression
```

## Comparing `pre5g-3.0.tar` & `pre5g-3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 10:03:19.247064 pre5g-3.0/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.0/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 10:03:19.246064 pre5g-3.0/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.0/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 10:03:19.238064 pre5g-3.0/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.0/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.0/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.0/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-3.0/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1020 2024-04-08 09:31:08.000000 pre5g-3.0/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.0/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.0/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.0/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 10:03:19.246064 pre5g-3.0/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-15 10:03:19.247064 pre5g-3.0/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-15 10:03:05.000000 pre5g-3.0/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 11:14:53.944171 pre5g-3.1/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.1/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 11:14:53.944171 pre5g-3.1/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.1/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 11:14:53.933171 pre5g-3.1/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.1/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.1/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.1/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-3.1/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1267 2024-04-15 11:14:41.000000 pre5g-3.1/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.1/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.1/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.1/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 11:14:53.943171 pre5g-3.1/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 11:14:53.000000 pre5g-3.1/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-15 11:14:53.000000 pre5g-3.1/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-15 11:14:53.000000 pre5g-3.1/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-15 11:14:53.000000 pre5g-3.1/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-15 11:14:53.945171 pre5g-3.1/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-15 11:14:47.000000 pre5g-3.1/setup.py
```

### Comparing `pre5g-3.0/LICENSE` & `pre5g-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/__init__.py` & `pre5g-3.1/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/labelen.py` & `pre5g-3.1/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/normalization.py` & `pre5g-3.1/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/nullvalue.py` & `pre5g-3.1/pre5g/nullvalue.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/onehoten.py` & `pre5g-3.1/pre5g/onehoten.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 import pandas as pd
 
-
 def one_hot_encoding_selected(data, columns):
     """
     Perform one-hot encoding on selected columns while retaining numeric values.
 
     Parameters:
     data (DataFrame): The input DataFrame.
     columns (list): List of column names to one-hot encode.
 
     Returns:
-    list: List of lists with one-hot encoded columns.
+    list: List of lists with one-hot encoded columns, including column names.
     """
     # Copy the original DataFrame
     encoded_data = data.copy()
     
+    # Initialize a list to store the column names in the output
+    column_names = []
+    
     # Iterate through selected columns
     for column in columns:
         # Check if column exists and is categorical
         if column in data.columns and data[column].dtype == 'object':
             # Perform one-hot encoding
             encoded_column = pd.get_dummies(data[column], prefix=column)
+            # Store the names of the one-hot encoded columns
+            column_names.extend(encoded_column.columns)
             # Drop original column and concatenate one-hot encoded columns
             encoded_data = pd.concat([encoded_data.drop(column, axis=1), encoded_column], axis=1)
     
     # Convert DataFrame to list of lists
     encoded_list = encoded_data.values.tolist()
     
-    return encoded_list
-
+    return [column_names] + encoded_list
```

### Comparing `pre5g-3.0/pre5g/robustscaler.py` & `pre5g-3.1/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/standardization.py` & `pre5g-3.1/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/pre5g/winsorization.py` & `pre5g-3.1/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-3.0/setup.py` & `pre5g-3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='3.0',
+    version='3.1',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

