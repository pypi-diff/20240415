# Comparing `tmp/pre5g-2.0.tar.gz` & `tmp/pre5g-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pre5g-2.0.tar", last modified: Mon Apr 15 07:16:28 2024, max compression
+gzip compressed data, was "dist/pre5g-2.9.tar", last modified: Mon Apr 15 07:23:45 2024, max compression
```

## Comparing `pre5g-2.0.tar` & `pre5g-2.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:16:28.298479 pre5g-2.0/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-2.0/LICENSE
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 07:16:28.297479 pre5g-2.0/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-2.0/README.md
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:16:28.289479 pre5g-2.0/pre5g/
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-2.0/pre5g/__init__.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-2.0/pre5g/labelen.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-2.0/pre5g/normalization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-2.0/pre5g/nullvalue.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     1020 2024-04-08 09:31:08.000000 pre5g-2.0/pre5g/onehoten.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2697 2024-04-08 07:59:01.000000 pre5g-2.0/pre5g/robustscaler.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-2.0/pre5g/standardization.py
--rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 05:26:00.000000 pre5g-2.0/pre5g/winsorization.py
-drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:16:28.297479 pre5g-2.0/pre5g.egg-info/
--rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 07:16:28.000000 pre5g-2.0/pre5g.egg-info/PKG-INFO
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-15 07:16:28.000000 pre5g-2.0/pre5g.egg-info/SOURCES.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-15 07:16:28.000000 pre5g-2.0/pre5g.egg-info/dependency_links.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-15 07:16:28.000000 pre5g-2.0/pre5g.egg-info/top_level.txt
--rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-15 07:16:28.298479 pre5g-2.0/setup.cfg
--rw-rw-r--   0 trainee   (1003) trainee   (1003)      601 2024-04-15 07:16:21.000000 pre5g-2.0/setup.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:23:45.111624 pre5g-2.9/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1063 2024-03-26 07:38:31.000000 pre5g-2.9/LICENSE
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 07:23:45.111624 pre5g-2.9/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       82 2024-03-26 07:39:06.000000 pre5g-2.9/README.md
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:23:45.110624 pre5g-2.9/pre5g/
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1137 2024-04-04 11:14:45.000000 pre5g-2.9/pre5g/__init__.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1042 2024-04-08 06:54:23.000000 pre5g-2.9/pre5g/labelen.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2707 2024-04-01 11:33:46.000000 pre5g-2.9/pre5g/normalization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     4306 2024-04-08 09:30:56.000000 pre5g-2.9/pre5g/nullvalue.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     1020 2024-04-08 09:31:08.000000 pre5g-2.9/pre5g/onehoten.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2697 2024-04-08 07:59:01.000000 pre5g-2.9/pre5g/robustscaler.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     3124 2024-04-01 11:39:06.000000 pre5g-2.9/pre5g/standardization.py
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)     2422 2024-04-15 07:20:59.000000 pre5g-2.9/pre5g/winsorization.py
+drwxrwxr-x   0 trainee   (1003) trainee   (1003)        0 2024-04-15 07:23:45.111624 pre5g-2.9/pre5g.egg-info/
+-rw-r--r--   0 trainee   (1003) trainee   (1003)      491 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/PKG-INFO
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      307 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/SOURCES.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        1 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/dependency_links.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)        6 2024-04-15 07:23:45.000000 pre5g-2.9/pre5g.egg-info/top_level.txt
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)       38 2024-04-15 07:23:45.111624 pre5g-2.9/setup.cfg
+-rw-rw-r--   0 trainee   (1003) trainee   (1003)      600 2024-04-15 07:23:41.000000 pre5g-2.9/setup.py
```

### Comparing `pre5g-2.0/LICENSE` & `pre5g-2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/__init__.py` & `pre5g-2.9/pre5g/__init__.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/labelen.py` & `pre5g-2.9/pre5g/labelen.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/normalization.py` & `pre5g-2.9/pre5g/normalization.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/nullvalue.py` & `pre5g-2.9/pre5g/nullvalue.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/onehoten.py` & `pre5g-2.9/pre5g/onehoten.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/robustscaler.py` & `pre5g-2.9/pre5g/robustscaler.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/standardization.py` & `pre5g-2.9/pre5g/standardization.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/pre5g/winsorization.py` & `pre5g-2.9/pre5g/winsorization.py`

 * *Files identical despite different names*

### Comparing `pre5g-2.0/setup.py` & `pre5g-2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pre5g',
-    version='2.0',
+    version='2.9',
     packages=find_packages(),
     description='An preprocessing package',
     author='SnehaM',
     author_email='1js20cs161@gmail.com',
     license='MIT',
     keywords=['example', 'package'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.6',
     ],
-)
+)
```

