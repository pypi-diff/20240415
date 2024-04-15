# Comparing `tmp/repelsec-0.3.tar.gz` & `tmp/repelsec-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repelsec-0.3.tar", last modified: Sat Apr  6 17:16:37 2024, max compression
+gzip compressed data, was "repelsec-0.4.tar", last modified: Mon Apr 15 17:12:10 2024, max compression
```

## Comparing `repelsec-0.3.tar` & `repelsec-0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 17:16:37.230501 repelsec-0.3/
--rw-rw-rw-   0        0        0     1090 2024-04-05 16:11:12.000000 repelsec-0.3/LICENSE
--rw-rw-rw-   0        0        0     3308 2024-04-06 17:16:37.229438 repelsec-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2905 2024-04-06 17:14:32.000000 repelsec-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-06 17:16:37.205447 repelsec-0.3/repelsec/
--rw-rw-rw-   0        0        0        0 2024-04-05 16:11:12.000000 repelsec-0.3/repelsec/__init__.py
--rw-rw-rw-   0        0        0    24446 2024-04-06 16:56:51.000000 repelsec-0.3/repelsec/cwe_vulnerabilities.py
--rw-rw-rw-   0        0        0     4300 2024-04-06 15:25:47.000000 repelsec-0.3/repelsec/functions.py
--rw-rw-rw-   0        0        0     4382 2024-04-05 16:11:12.000000 repelsec-0.3/repelsec/generate_pdf.py
--rw-rw-rw-   0        0        0    18907 2024-04-06 14:52:29.000000 repelsec-0.3/repelsec/main.py
--rw-rw-rw-   0        0        0    13581 2024-04-06 16:49:37.000000 repelsec-0.3/repelsec/tests.py
-drwxrwxrwx   0        0        0        0 2024-04-06 17:16:37.226466 repelsec-0.3/repelsec.egg-info/
--rw-rw-rw-   0        0        0     3308 2024-04-06 17:16:37.000000 repelsec-0.3/repelsec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-04-06 17:16:37.000000 repelsec-0.3/repelsec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 17:16:37.000000 repelsec-0.3/repelsec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-06 17:16:37.000000 repelsec-0.3/repelsec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      138 2024-04-06 17:16:37.000000 repelsec-0.3/repelsec.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 17:16:37.000000 repelsec-0.3/repelsec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 17:16:37.230501 repelsec-0.3/setup.cfg
--rw-rw-rw-   0        0        0      622 2024-04-06 17:15:41.000000 repelsec-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:12:10.698493 repelsec-0.4/
+-rw-rw-rw-   0        0        0     1090 2024-04-05 16:11:12.000000 repelsec-0.4/LICENSE
+-rw-rw-rw-   0        0        0     3351 2024-04-15 17:12:10.697483 repelsec-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2948 2024-04-15 17:00:41.000000 repelsec-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 17:12:10.675707 repelsec-0.4/repelsec/
+-rw-rw-rw-   0        0        0        0 2024-04-05 16:11:12.000000 repelsec-0.4/repelsec/__init__.py
+-rw-rw-rw-   0        0        0    24455 2024-04-11 17:12:38.000000 repelsec-0.4/repelsec/cwe_vulnerabilities.py
+-rw-rw-rw-   0        0        0     4300 2024-04-06 15:25:47.000000 repelsec-0.4/repelsec/functions.py
+-rw-rw-rw-   0        0        0     6167 2024-04-12 15:04:11.000000 repelsec-0.4/repelsec/generate_pdf.py
+-rw-rw-rw-   0        0        0    19229 2024-04-15 17:10:54.000000 repelsec-0.4/repelsec/main.py
+-rw-rw-rw-   0        0        0    13581 2024-04-06 16:49:37.000000 repelsec-0.4/repelsec/unit_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-15 17:12:10.695761 repelsec-0.4/repelsec.egg-info/
+-rw-rw-rw-   0        0        0     3351 2024-04-15 17:12:10.000000 repelsec-0.4/repelsec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-15 17:12:10.000000 repelsec-0.4/repelsec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 17:12:10.000000 repelsec-0.4/repelsec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-15 17:12:10.000000 repelsec-0.4/repelsec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      138 2024-04-15 17:12:10.000000 repelsec-0.4/repelsec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-15 17:12:10.000000 repelsec-0.4/repelsec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 17:12:10.698493 repelsec-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      622 2024-04-15 17:10:13.000000 repelsec-0.4/setup.py
```

### Comparing `repelsec-0.3/LICENSE` & `repelsec-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `repelsec-0.3/PKG-INFO` & `repelsec-0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repelsec
-Version: 0.3
+Version: 0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nvdlib~=0.7.5
 Requires-Dist: xmltodict~=0.13.0
 Requires-Dist: pandas~=2.1.1
 Requires-Dist: argparse~=1.4.0
 Requires-Dist: setuptools~=69.0.2
@@ -23,15 +23,17 @@
   potential CWE vulnerabilities.
 - Software composition analysis (SCA) that identifies any outdated dependencies within the pom.xml file and their
   associated
   CVE vulnerabilities.
 
 ## Installation
 
-If your system has Python installed, open your preferred terminal and enter the following command.
+If your system has Python installed, open your preferred terminal or IDE and enter the following command.
+
+`python -m pip install repelsec`
 
 `pip install repelsec`
 
 To keep this tool up to date, run the following command on a scheduled basis.
 
 `pip install repelsec --upgrade`
```

### Comparing `repelsec-0.3/README.md` & `repelsec-0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,17 @@
   potential CWE vulnerabilities.
 - Software composition analysis (SCA) that identifies any outdated dependencies within the pom.xml file and their
   associated
   CVE vulnerabilities.
 
 ## Installation
 
-If your system has Python installed, open your preferred terminal and enter the following command.
+If your system has Python installed, open your preferred terminal or IDE and enter the following command.
+
+`python -m pip install repelsec`
 
 `pip install repelsec`
 
 To keep this tool up to date, run the following command on a scheduled basis.
 
 `pip install repelsec --upgrade`
```

### Comparing `repelsec-0.3/repelsec/cwe_vulnerabilities.py` & `repelsec-0.4/repelsec/cwe_vulnerabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from functions import is_strong_token
+from repelsec.functions import is_strong_token
 
 
 # MITRE CWE Classes:
 
 # CWE-89: Improper Neutralization of Special Elements used in an SQL Command ('SQL Injection')
 # CWE-111: Direct Use of Unsafe JNI
 # CWE-190: Integer Overflow or Wraparound
```

### Comparing `repelsec-0.3/repelsec/functions.py` & `repelsec-0.4/repelsec/functions.py`

 * *Files identical despite different names*

### Comparing `repelsec-0.3/repelsec/main.py` & `repelsec-0.4/repelsec/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Imports
 import json
 import os
 from argparse import ArgumentParser, Namespace
 from datetime import datetime
+from time import time
 
 import nvdlib
 import pandas as pd
 import requests.exceptions
 import xmltodict
 
 from repelsec import cwe_vulnerabilities
@@ -33,25 +34,27 @@
                         type=lambda x: sec.is_valid_path(parser, x))
 
     # Define custom type args
     args: Namespace = parser.parse_args()
 
     # Set output path for result exports
     if args.output_path is None:
-        # output_path = os.getcwd()
-        output_path = os.path.join(os.getcwd(), "repelsec/results")  # For TESTING
+        output_path = os.getcwd()
+        # output_path = os.path.join(os.getcwd(), "repelsec/results")  # For TESTING
     else:
         output_path = args.output_path
 
     # Define filename from path provided
     filename = os.path.basename(args.filename)
 
     # SCA SCAN
     if "pom.xml" in filename:
 
+        start_time = time()
+
         # Open supplied file
         with open(args.filename, "r") as f:
             file = f.read()
 
         # Convert pom.xml file to Python Dictionary and assign its attributes to variables
         pom_dict = xmltodict.parse(file)
         parent = pom_dict["project"]["parent"]
@@ -215,24 +218,29 @@
                 f.write(f"Security Score - {scan_score}\n")
                 f.write("\n")
 
         # If pdf argument is enabled, print SCA results to a PDF file
         if args.pdf:
             pdf = PDF()
             pdf_path = os.path.join(output_path, "sca.pdf")
-            pdf.create_pdf("SCA", sca_dict_list)
+            pdf.create_pdf("SCA", sca_dict_list, scan_score)
             pdf.output(pdf_path, 'F')
 
             if args.password:
                 encrypted_path = os.path.join(output_path, "e_sca.pdf")
                 sec.add_pdf_password(pdf_path, encrypted_path, args.password)
 
+        end_time = time()
+        print(f"SCA Scan time {round((end_time - start_time), 4)} Seconds")
+
     # SAST Scan
     elif ".java" in filename or ".jsp" in filename:
 
+        start_time = time()
+
         # Define initial Scan Result and Score
         scan_score = 100
         scan_result = "Pass"
 
         # Open supplied file
         # with open(args.filename, "r") as f:
         #    lines = f.read.splitlines()
@@ -371,13 +379,16 @@
                 f.write(f"Scan Score - {scan_score}\n")
                 f.write("\n")
 
         # If pdf argument is enabled, print SCA results to a PDF file
         if args.pdf:
             pdf = PDF()
             pdf_path = os.path.join(output_path, "sast.pdf")
-            pdf.create_pdf("SAST", sast_dict_list)
+            pdf.create_pdf("SAST", sast_dict_list, scan_score)
             pdf.output(pdf_path, 'F')
 
             if args.password:
                 encrypted_path = os.path.join(output_path, "e_sast.pdf")
                 sec.add_pdf_password(pdf_path, encrypted_path, args.password)
+
+        end_time = time()
+        print(f"SAST Scan time {round((end_time - start_time), 4)} Seconds")
```

### Comparing `repelsec-0.3/repelsec/tests.py` & `repelsec-0.4/repelsec/unit_tests.py`

 * *Files identical despite different names*

### Comparing `repelsec-0.3/repelsec.egg-info/PKG-INFO` & `repelsec-0.4/repelsec.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repelsec
-Version: 0.3
+Version: 0.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nvdlib~=0.7.5
 Requires-Dist: xmltodict~=0.13.0
 Requires-Dist: pandas~=2.1.1
 Requires-Dist: argparse~=1.4.0
 Requires-Dist: setuptools~=69.0.2
@@ -23,15 +23,17 @@
   potential CWE vulnerabilities.
 - Software composition analysis (SCA) that identifies any outdated dependencies within the pom.xml file and their
   associated
   CVE vulnerabilities.
 
 ## Installation
 
-If your system has Python installed, open your preferred terminal and enter the following command.
+If your system has Python installed, open your preferred terminal or IDE and enter the following command.
+
+`python -m pip install repelsec`
 
 `pip install repelsec`
 
 To keep this tool up to date, run the following command on a scheduled basis.
 
 `pip install repelsec --upgrade`
```

### Comparing `repelsec-0.3/setup.py` & `repelsec-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="repelsec",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     include_package_data=True,
     install_requires=read_requirements(),
     entry_points='''
     [console_scripts]
     repelsec=repelsec.main:main
     ''',
```

