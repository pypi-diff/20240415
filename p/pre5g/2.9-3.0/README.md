# Comparing `tmp/pre5g-2.9.tar.gz` & `tmp/pre5g-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-2.9.tar", last modified: Mon Apr 15 07:23:45 2024, max compression
+gzip compressed data, was "dist/pre5g-3.0.tar", last modified: Mon Apr 15 10:03:19 2024, max compression
```

## Comparing `pre5g-2.9.tar` & `pre5g-3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:23:45.111624 pre5g-2.9/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-2.9/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 07:23:45.111624 pre5g-2.9/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-2.9/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:23:45.110624 pre5g-2.9/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-2.9/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-2.9/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-2.9/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-2.9/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1020 2024-04-08 09:31:08.000000 pre5g-2.9/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2697 2024-04-08 07:59:01.000000 pre5g-2.9/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-2.9/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-2.9/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:23:45.111624 pre5g-2.9/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-15 07:23:45.111624 pre5g-2.9/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-15 07:23:41.000000 pre5g-2.9/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 10:03:19.247064 pre5g-3.0/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-3.0/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 10:03:19.246064 pre5g-3.0/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-3.0/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 10:03:19.238064 pre5g-3.0/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-3.0/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-3.0/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-3.0/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-3.0/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1020 2024-04-08 09:31:08.000000 pre5g-3.0/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3355 2024-04-15 10:02:56.000000 pre5g-3.0/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-3.0/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-3.0/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 10:03:19.246064 pre5g-3.0/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-15 10:03:19.000000 pre5g-3.0/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-15 10:03:19.247064 pre5g-3.0/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-15 10:03:05.000000 pre5g-3.0/setup.py
```

### Comparing `pre5g-2.9/LICENSE` & `pre5g-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/__init__.py` & `pre5g-3.0/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/labelen.py` & `pre5g-3.0/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/normalization.py` & `pre5g-3.0/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/nullvalue.py` & `pre5g-3.0/pre5g/nullvalue.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/onehoten.py` & `pre5g-3.0/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/robustscaler.py` & `pre5g-3.0/pre5g/robustscaler.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,19 +40,31 @@
     """
     # Initialize lists to store median and IQR for each selected column
     column_medians = []
     column_iqrs = []
 
     # Calculate median and IQR for each selected column
     for col_index in selected_columns:
-        # Extract column values, excluding non-numeric values
+        # Extract column values, excluding non-numeric and string values
         column_values = [row[col_index] for row in data if isinstance(row[col_index], (int, float))]
-        column_medians.append(np.median(column_values))
-        q3, q1 = np.percentile(column_values, [75 ,25])
-        column_iqrs.append(q3 - q1)
+        if column_values:
+            column_medians.append(np.median(column_values))
+            
+            # Filter out string values before calculating percentiles
+            numeric_values = [val for val in column_values if not isinstance(val, str)]
+            if numeric_values:
+                q3, q1 = np.percentile(numeric_values, [75 ,25])
+                column_iqrs.append(q3 - q1)
+            else:
+                # Handle the case when there are no numeric values in the column
+                column_iqrs.append(0)  # Set IQR to 0 or any other value
+        else:
+            # Handle the case when the column has no numeric values
+            column_medians.append(0)  # Set median to 0 or any other value
+            column_iqrs.append(0)  # Set IQR to 0 or any other value
 
     # Apply Robust Scaling to each selected column
     scaled_data = []
     for row in data:
         scaled_row = []
         for i, val in enumerate(row):
             if i in selected_columns:
```

### Comparing `pre5g-2.9/pre5g/standardization.py` & `pre5g-3.0/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/pre5g/winsorization.py` & `pre5g-3.0/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.9/setup.py` & `pre5g-3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='2.9',
+    version='3.0',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
```

