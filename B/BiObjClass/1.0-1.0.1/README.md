# Comparing `tmp/BiObjClass-1.0.tar.gz` & `tmp/BiObjClass-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BiObjClass-1.0.tar", last modified: Mon Apr 15 18:03:04 2024, max compression
+gzip compressed data, was "BiObjClass-1.0.1.tar", last modified: Mon Apr 15 19:34:22 2024, max compression
```

## Comparing `BiObjClass-1.0.tar` & `BiObjClass-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-15 18:03:04.299177 BiObjClass-1.0/
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-15 18:03:04.299177 BiObjClass-1.0/BiObjClass/
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       22 2024-02-28 17:56:40.000000 BiObjClass-1.0/BiObjClass/__init__.py
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    13380 2024-04-15 18:00:25.000000 BiObjClass-1.0/BiObjClass/wrapper.py
-drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-15 18:03:04.299177 BiObjClass-1.0/BiObjClass.egg-info/
--rw-r--r--   0 tiago     (1000) tiago     (1000)     4119 2024-04-15 18:03:03.000000 BiObjClass-1.0/BiObjClass.egg-info/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)      240 2024-04-15 18:03:03.000000 BiObjClass-1.0/BiObjClass.egg-info/SOURCES.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-15 18:03:03.000000 BiObjClass-1.0/BiObjClass.egg-info/dependency_links.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)        7 2024-04-15 18:03:03.000000 BiObjClass-1.0/BiObjClass.egg-info/requires.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       11 2024-04-15 18:03:03.000000 BiObjClass-1.0/BiObjClass.egg-info/top_level.txt
--rw-rw-r--   0 tiago     (1000) tiago     (1000)    35148 2024-02-28 18:01:36.000000 BiObjClass-1.0/LICENSE
--rw-r--r--   0 tiago     (1000) tiago     (1000)     4119 2024-04-15 18:03:04.299177 BiObjClass-1.0/PKG-INFO
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     3334 2024-04-15 17:59:13.000000 BiObjClass-1.0/README.md
--rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-15 18:03:04.299177 BiObjClass-1.0/setup.cfg
--rw-rw-r--   0 tiago     (1000) tiago     (1000)     1373 2024-03-09 20:35:46.000000 BiObjClass-1.0/setup.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-15 19:34:22.136646 BiObjClass-1.0.1/
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-15 19:34:22.104645 BiObjClass-1.0.1/BiObjClass/
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       22 2024-02-28 17:56:40.000000 BiObjClass-1.0.1/BiObjClass/__init__.py
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    12820 2024-04-15 19:31:07.000000 BiObjClass-1.0.1/BiObjClass/wrapper.py
+drwxrwxr-x   0 tiago     (1000) tiago     (1000)        0 2024-04-15 19:34:22.112645 BiObjClass-1.0.1/BiObjClass.egg-info/
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     4060 2024-04-15 19:34:22.000000 BiObjClass-1.0.1/BiObjClass.egg-info/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)      240 2024-04-15 19:34:22.000000 BiObjClass-1.0.1/BiObjClass.egg-info/SOURCES.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        1 2024-04-15 19:34:22.000000 BiObjClass-1.0.1/BiObjClass.egg-info/dependency_links.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)        7 2024-04-15 19:34:22.000000 BiObjClass-1.0.1/BiObjClass.egg-info/requires.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       11 2024-04-15 19:34:22.000000 BiObjClass-1.0.1/BiObjClass.egg-info/top_level.txt
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)    35148 2024-02-28 18:01:36.000000 BiObjClass-1.0.1/LICENSE
+-rw-r--r--   0 tiago     (1000) tiago     (1000)     4060 2024-04-15 19:34:22.112645 BiObjClass-1.0.1/PKG-INFO
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     3335 2024-04-15 17:56:35.000000 BiObjClass-1.0.1/README.md
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)       38 2024-04-15 19:34:22.136646 BiObjClass-1.0.1/setup.cfg
+-rw-rw-r--   0 tiago     (1000) tiago     (1000)     1309 2024-04-15 19:34:15.000000 BiObjClass-1.0.1/setup.py
```

### Comparing `BiObjClass-1.0/BiObjClass/wrapper.py` & `BiObjClass-1.0.1/BiObjClass/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -265,42 +265,16 @@
             if n == 0:
                 A[i][j] = G[i][j]
             else:
                 A[i][j] = G[i][j]
 
 
         # Variável para calcular o maior valor na linha
-        max = max(A[0])
+        max = max(A[i])
 
         for j in range(n):
             # Caso A[i][j] == 0 então A[i][j] recebe o maior valor da linha multiplicado por 10
             if A[i][j] == 0:
                 A[i][j] = max*10
         #A.sort()
 
-
-
-#R_file = input("Informe o nome do arquivo R: ")
-#T_file = input("Informe o nome do arquivo T: ")
-#
-#R = []
-#T = []
-#
-#
-#has_header_input = input("Os arquivos têm cabeçalho? (S para Sim, N para Não): ").upper()
-#has_header = has_header_input == 'S'
-#
-#names = []
-#
-#
-#
-#
-#A = bilex(R_file, T_file, has_header)
-#tam = len(A)
-#
-#
-## Exibir a matriz A
-#with open('out.txt', 'w') as output_file:
-#    for i in range(0, tam):
-#        name = names[i]
-#        formatted_row = [float(value) for value in A[i]]
-#        print(f'{name: <30}{formatted_row}', file=output_file)
+    return A
```

### Comparing `BiObjClass-1.0/BiObjClass.egg-info/PKG-INFO` & `BiObjClass-1.0.1/BiObjClass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: BiObjClass
-Version: 1.0
+Version: 1.0.1
 Summary: Bi-objective Lexicographical Classification
 Author: Tiago Costa Soares, Pedro Augusto Mendes, Iago Augusto de Carvalho
 Author-email: tiagocsoares22@gmail.com, pedroaugusto.mendes035@gmail.com, iago.carvalho@unifal-mg.edu.brZ
-Keywords: classification,bi-objetive,lexicographical,ranking,csv,bilex,par10
+Keywords: classification,bi-objetive,lexicographical,ranking,csv
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: csvkit
 
 
 # BiObjClass
```

### Comparing `BiObjClass-1.0/LICENSE` & `BiObjClass-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BiObjClass-1.0/PKG-INFO` & `BiObjClass-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: BiObjClass
-Version: 1.0
+Version: 1.0.1
 Summary: Bi-objective Lexicographical Classification
 Author: Tiago Costa Soares, Pedro Augusto Mendes, Iago Augusto de Carvalho
 Author-email: tiagocsoares22@gmail.com, pedroaugusto.mendes035@gmail.com, iago.carvalho@unifal-mg.edu.brZ
-Keywords: classification,bi-objetive,lexicographical,ranking,csv,bilex,par10
+Keywords: classification,bi-objetive,lexicographical,ranking,csv
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: csvkit
 
 
 # BiObjClass
```

### Comparing `BiObjClass-1.0/README.md` & `BiObjClass-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -68,8 +68,8 @@
 'Replace 'G.csv' with your file name'
 
 This approach is recommended for files that have a header line. By assigning true to has_header, the function will no longer apply the classification to the first line of the files.
 
 
 ## License
 
-This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.
+This project is licensed under the GNU General Public License v3.0 - see the LICENSE file for details.
```

### Comparing `BiObjClass-1.0/setup.py` & `BiObjClass-1.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'Bi-objective Lexicographical Classification'
 LONG_DESCRIPTION = ('A package that allows building a matrix with the Bi-objective Lexicographical Classification '
                     'of different algorithms.')
 
 # Setting up
 setup(
     name="BiObjClass",
@@ -20,18 +20,17 @@
     author="Tiago Costa Soares, Pedro Augusto Mendes, Iago Augusto de Carvalho",
     author_email="tiagocsoares22@gmail.com, pedroaugusto.mendes035@gmail.com, iago.carvalho@unifal-mg.edu.brZ",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=['csvkit'],
-    keywords=['classification', 'bi-objetive', 'lexicographical', 'ranking', "csv", "bilex", "par10"],
+    keywords=['classification', 'bi-objetive', 'lexicographical', 'ranking', "csv"],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3",
         "Operating System :: POSIX :: Linux",
-        "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

