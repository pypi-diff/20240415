# Comparing `tmp/schubmult-1.3.3.tar.gz` & `tmp/schubmult-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schubmult-1.3.3.tar", last modified: Sat Apr 13 16:40:11 2024, max compression
+gzip compressed data, was "schubmult-1.3.4.tar", last modified: Mon Apr 15 14:05:56 2024, max compression
```

## Comparing `schubmult-1.3.3.tar` & `schubmult-1.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.919000 schubmult-1.3.3/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.3/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)     5231 2024-04-13 16:40:11.868000 schubmult-1.3.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4849 2024-04-13 16:38:44.000000 schubmult-1.3.3/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:09.299000 schubmult-1.3.3/schubmult/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.3/schubmult/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    16003 2024-04-12 18:48:00.000000 schubmult-1.3.3/schubmult/perm_lib.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:10.072000 schubmult-1.3.3/schubmult/schubmult_double/
--rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.3/schubmult/schubmult_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.3/schubmult/schubmult_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.3/schubmult/schubmult_double/schubmult_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:10.412000 schubmult-1.3.3/schubmult/schubmult_py/
--rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.3/schubmult/schubmult_py/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.3/schubmult/schubmult_py/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.3/schubmult/schubmult_py/schubmult_py.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:10.759000 schubmult-1.3.3/schubmult/schubmult_q/
--rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.3/schubmult/schubmult_q/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.3/schubmult/schubmult_q/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     9008 2024-04-08 20:08:59.000000 schubmult-1.3.3/schubmult/schubmult_q/schubmult_q.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.082000 schubmult-1.3.3/schubmult/schubmult_q_double/
--rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.3/schubmult/schubmult_q_double/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.3/schubmult/schubmult_q_double/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     3042 2024-04-12 20:25:54.000000 schubmult-1.3.3/schubmult/schubmult_q_double/schubmult_q_double.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.421000 schubmult-1.3.3/schubmult/schubmult_q_yz/
--rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.3/schubmult/schubmult_q_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.3/schubmult/schubmult_q_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)     5865 2024-04-12 18:47:48.000000 schubmult-1.3.3/schubmult/schubmult_q_yz/schubmult_q_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:11.802000 schubmult-1.3.3/schubmult/schubmult_yz/
--rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.3/schubmult/schubmult_yz/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.3/schubmult/schubmult_yz/__main__.py
--rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.3/schubmult/schubmult_yz/schubmult_yz.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-13 16:40:09.745000 schubmult-1.3.3/schubmult.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     5231 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      978 2024-04-13 16:40:08.000000 schubmult-1.3.3/schubmult.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)      353 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/entry_points.txt
--rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-13 16:40:07.000000 schubmult-1.3.3/schubmult.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-13 16:40:11.904000 schubmult-1.3.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1243 2024-04-12 18:51:29.000000 schubmult-1.3.3/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:56.285000 schubmult-1.3.4/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2023-09-24 17:08:26.000000 schubmult-1.3.4/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-15 14:05:56.236000 schubmult-1.3.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4853 2024-04-15 14:05:16.000000 schubmult-1.3.4/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:54.059000 schubmult-1.3.4/schubmult/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-09-24 17:08:26.000000 schubmult-1.3.4/schubmult/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    16003 2024-04-12 18:48:00.000000 schubmult-1.3.4/schubmult/perm_lib.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:54.734000 schubmult-1.3.4/schubmult/schubmult_double/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2023-09-25 01:39:08.000000 schubmult-1.3.4/schubmult/schubmult_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       97 2023-09-26 17:55:50.000000 schubmult-1.3.4/schubmult/schubmult_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4773 2024-04-10 12:45:13.000000 schubmult-1.3.4/schubmult/schubmult_double/schubmult_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.025000 schubmult-1.3.4/schubmult/schubmult_py/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2023-09-25 01:39:03.000000 schubmult-1.3.4/schubmult/schubmult_py/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       94 2023-09-26 17:55:38.000000 schubmult-1.3.4/schubmult/schubmult_py/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4373 2024-04-10 12:45:06.000000 schubmult-1.3.4/schubmult/schubmult_py/schubmult_py.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.307000 schubmult-1.3.4/schubmult/schubmult_q/
+-rwxrwxrwx   0 root         (0) root         (0)       36 2024-04-03 15:35:41.000000 schubmult-1.3.4/schubmult/schubmult_q/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       92 2024-04-03 15:28:43.000000 schubmult-1.3.4/schubmult/schubmult_q/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9008 2024-04-08 20:08:59.000000 schubmult-1.3.4/schubmult/schubmult_q/schubmult_q.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.590000 schubmult-1.3.4/schubmult/schubmult_q_double/
+-rwxrwxrwx   0 root         (0) root         (0)       33 2024-04-12 18:50:20.000000 schubmult-1.3.4/schubmult/schubmult_q_double/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       99 2024-04-12 18:49:31.000000 schubmult-1.3.4/schubmult/schubmult_q_double/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     3215 2024-04-15 14:01:00.000000 schubmult-1.3.4/schubmult/schubmult_q_double/schubmult_q_double.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:55.879000 schubmult-1.3.4/schubmult/schubmult_q_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       29 2024-04-12 18:49:56.000000 schubmult-1.3.4/schubmult/schubmult_q_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       95 2024-04-12 18:49:43.000000 schubmult-1.3.4/schubmult/schubmult_q_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5854 2024-04-15 13:59:54.000000 schubmult-1.3.4/schubmult/schubmult_q_yz/schubmult_q_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:56.171000 schubmult-1.3.4/schubmult/schubmult_yz/
+-rwxrwxrwx   0 root         (0) root         (0)       27 2023-09-25 01:38:28.000000 schubmult-1.3.4/schubmult/schubmult_yz/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       93 2023-09-26 17:55:32.000000 schubmult-1.3.4/schubmult/schubmult_yz/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)    42460 2024-04-12 14:57:13.000000 schubmult-1.3.4/schubmult/schubmult_yz/schubmult_yz.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 14:05:54.472000 schubmult-1.3.4/schubmult.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     5235 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      978 2024-04-15 14:05:53.000000 schubmult-1.3.4/schubmult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)      353 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/entry_points.txt
+-rwxrwxrwx   0 root         (0) root         (0)       83 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       10 2024-04-15 14:05:52.000000 schubmult-1.3.4/schubmult.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2024-04-15 14:05:56.272000 schubmult-1.3.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1243 2024-04-15 14:05:23.000000 schubmult-1.3.4/setup.py
```

### Comparing `schubmult-1.3.3/LICENSE` & `schubmult-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/PKG-INFO` & `schubmult-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.3
+Version: 1.3.4
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
 schubmult_yz -code 0 1 1 2 - 1 0 2 3 --display-positive
 schubmult_q -code 4 0 2 1 - 4 0 1 1
 schubmult_q_double -code 4 0 2 1 - 4 0 1 1
-schubmult_q_yz 5 4 0 2 1 - 1 3 --display-positive
+schubmult_q_yz -code 4 0 2 1 - 1 3 --display-positive
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4 --display-positive
```

### Comparing `schubmult-1.3.3/README.md` & `schubmult-1.3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
 schubmult_yz -code 0 1 1 2 - 1 0 2 3 --display-positive
 schubmult_q -code 4 0 2 1 - 4 0 1 1
 schubmult_q_double -code 4 0 2 1 - 4 0 1 1
-schubmult_q_yz 5 4 0 2 1 - 1 3 --display-positive
+schubmult_q_yz -code 4 0 2 1 - 1 3 --display-positive
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4 --display-positive
```

### Comparing `schubmult-1.3.3/schubmult/perm_lib.py` & `schubmult-1.3.4/schubmult/perm_lib.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/schubmult/schubmult_double/schubmult_double.py` & `schubmult-1.3.4/schubmult/schubmult_double/schubmult_double.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/schubmult/schubmult_py/schubmult_py.py` & `schubmult-1.3.4/schubmult/schubmult_py/schubmult_py.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/schubmult/schubmult_q/schubmult_q.py` & `schubmult-1.3.4/schubmult/schubmult_q/schubmult_q.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/schubmult/schubmult_q_double/schubmult_q_double.py` & `schubmult-1.3.4/schubmult/schubmult_q_double/schubmult_q_double.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,17 +37,14 @@
 		check = True
 		msg = False
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
-				if s == "-coprod":
-					coprod = True
-					continue
 				if s == "-nocheck":
 					check = False
 					continue
 				if s == "--display-positive":
 					display_positive = True
 					continue
 				if s == "--optimizer-message":
@@ -56,25 +53,28 @@
 				if s == "--version":
 					print(f"Python version {sys.version}")
 					exit(0)
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "--usage":
-					print("Usage: schubmult_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
-					print("Alternative usage: schubmult_yz <-code> <--display-positive> -coprod perm - indexlist")
+					print("**** schubmult_q_double ****")
+					print("Purpose: Compute equivariant Gromov-Witten invariants, structure constants of quantum double Schubert polynomials")
+					print("Usage: schubmult_q_double <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
+					#print("Alternative usage: schubmult_yz <-code> <--display-positive> -coprod perm - indexlist")
 					exit(0)
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
-			print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
-			print("Alternative usage: schubmult_yz <-code> <--display-positive> <--optimizer-message> -coprod perm - indexlist")
+			print("**** schubmult_q_double ****")
+			print("Purpose: Compute equivariant Gromov-Witten invariants, structure constants of quantum double Schubert polynomials")
+			print("Usage: schubmult_q_double <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
 			exit(1)
 				
 		perms += [curperm]
 		
 		
 		if ascode:
 			for i in range(len(perms)):
```

### Comparing `schubmult-1.3.3/schubmult/schubmult_q_yz/schubmult_q_yz.py` & `schubmult-1.3.4/schubmult/schubmult_q_yz/schubmult_q_yz.py`

 * *Files 12% similar despite different names*

```diff
@@ -108,17 +108,14 @@
 		check = True
 		msg = False
 		try:
 			for s in sys.argv[1:]:
 				if s == "-np" or s == "--no-print":
 					pr = False
 					continue
-				if s == "-coprod":
-					coprod = True
-					continue
 				if s == "-nocheck":
 					check = False
 					continue
 				if s == "--display-positive":
 					display_positive = True
 					continue
 				if s == "--optimizer-message":
@@ -127,25 +124,27 @@
 				if s == "--version":
 					print(f"Python version {sys.version}")
 					exit(0)
 				if s == "-code":
 					ascode = True
 					continue
 				if s == "--usage":
-					print("Usage: schubmult_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
-					print("Alternative usage: schubmult_yz <-code> <--display-positive> -coprod perm - indexlist")
+					print("**** schubmult_q_yz ****")
+					print("Purpose: Compute Molev-Sagan coefficients of quantum double Schubert polynomials")
+					print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
 					exit(0)
 				if s == "-":
 					perms += [curperm]
 					curperm = []
 					continue
 				curperm += [int(s)]
 		except Exception:
+			print("**** schubmult_q_yz ****")
+			print("Purpose: Compute Molev-Sagan coefficients of quantum double Schubert polynomials")
 			print("Usage: schubmult_q_yz <-np|--no-print> <-code> <--display-positive> <--optimizer-message> perm1 - perm2 < - perm3 .. >")
-			print("Alternative usage: schubmult_yz <-code> <--display-positive> <--optimizer-message> -coprod perm - indexlist")
 			exit(1)
 				
 		perms += [curperm]
 		
 		
 		if ascode:
 			for i in range(len(perms)):
```

### Comparing `schubmult-1.3.3/schubmult/schubmult_yz/schubmult_yz.py` & `schubmult-1.3.4/schubmult/schubmult_yz/schubmult_yz.py`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/schubmult.egg-info/PKG-INFO` & `schubmult-1.3.4/schubmult.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schubmult
-Version: 1.3.3
+Version: 1.3.4
 Summary: Computing Littlewood-Richardson coefficients of Schubert polynomials
 Home-page: https://github.com/matthematics/schubmult
 Author: Matt Samuel
 Author-email: schubmult@gmail.com
 License: GNU
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -30,15 +30,15 @@
 
 ```
 schubmult_py -code 0 0 1 5 6 2 3 4 - 5 6 0 0 0 0 1 2 3 4
 schubmult_double -code 0 1 1 2 - 1 0 2 3
 schubmult_yz -code 0 1 1 2 - 1 0 2 3 --display-positive
 schubmult_q -code 4 0 2 1 - 4 0 1 1
 schubmult_q_double -code 4 0 2 1 - 4 0 1 1
-schubmult_q_yz 5 4 0 2 1 - 1 3 --display-positive
+schubmult_q_yz -code 4 0 2 1 - 1 3 --display-positive
 ```
 
 For coproducts:
 ```
 schubmult_py -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_double -coprod 1 3 5 7 2 4 6 - 2 4
 schubmult_yz -coprod 1 3 5 7 2 4 6 - 2 4 --display-positive
```

### Comparing `schubmult-1.3.3/schubmult.egg-info/SOURCES.txt` & `schubmult-1.3.4/schubmult.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schubmult-1.3.3/setup.py` & `schubmult-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="schubmult",
-    version="1.3.3",
+    version="1.3.4",
     description="Computing Littlewood-Richardson coefficients of Schubert polynomials",
 	long_description=long_description,
 	long_description_content_type='text/markdown',
     url="https://github.com/matthematics/schubmult",
     author="Matt Samuel",
     author_email="schubmult@gmail.com",
     license="GNU",
```

