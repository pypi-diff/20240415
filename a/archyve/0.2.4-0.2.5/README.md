# Comparing `tmp/archyve-0.2.4.tar.gz` & `tmp/archyve-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archyve-0.2.4.tar", max compression
+gzip compressed data, was "archyve-0.2.5.tar", max compression
```

## Comparing `archyve-0.2.4.tar` & `archyve-0.2.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     9665 2024-04-14 22:44:03.801273 archyve-0.2.4/archyve.py
--rw-r--r--   0        0        0      369 2024-04-14 22:44:35.725653 archyve-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1953 2024-04-14 22:23:51.671891 archyve-0.2.4/README.md
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 archyve-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     9665 2024-04-14 22:44:03.801273 archyve-0.2.5/archyve.py
+-rw-r--r--   0        0        0      369 2024-04-14 23:07:22.402536 archyve-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2331 2024-04-14 22:57:12.016031 archyve-0.2.5/README.md
+-rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 archyve-0.2.5/PKG-INFO
```

### Comparing `archyve-0.2.4/archyve.py` & `archyve-0.2.5/archyve.py`

 * *Files identical despite different names*

### Comparing `archyve-0.2.4/README.md` & `archyve-0.2.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Archive Manager
 
 Archive Manager is a Python tool designed to help users interact with and manage large archives of files efficiently. 
 Whether you need to sort files, find duplicates, perform equality checks, or remove unnecessary files, this tool 
 provides the necessary functionalities to streamline your file management tasks.
 
+Core concepts and explanation:
+- Archyves are wrappers for built in generators that enable the user to loop through directories revursively.
+- To represent each item that the archyve finds, we have Entry objects - these are wrappers for Path objects that enable some useful features like hashing, sorting etc.
+
 ## Features
 
 - **Sorting:** Organize your files based on various criteria such as file type, size, date modified, etc.
 - **Duplicate Finding:** Identify and manage duplicate files to free up storage space.
 - **Equality Checking:** Compare files to ensure they are identical or different.
 - **Removal Tools:** Safely remove unwanted files from your archives.
 
@@ -46,12 +50,15 @@
 2. Get a list of all non-text files recursively in a given directory:
    
    ```python
    from archyve import Archyve, EntryType
    
    # Create an archyve
    archyve: Archyve = Archyve(r"p1", r"p2")
+   
    # Filter the archyve entries on whatever you need
    archyve = archyve.filter(lambda e: not e.is_type(EntryType.TEXT))
+   
+   # Loop through the archyve and print the entries
    for entry in archyve:
       print(entry)
    ```
```

### Comparing `archyve-0.2.4/PKG-INFO` & `archyve-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archyve
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python toolkit for the mass management and analysis of files.
 Author: Alistair Kellaway
 Author-email: ali.kellaway139@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
@@ -12,14 +12,18 @@
 
 # Archive Manager
 
 Archive Manager is a Python tool designed to help users interact with and manage large archives of files efficiently. 
 Whether you need to sort files, find duplicates, perform equality checks, or remove unnecessary files, this tool 
 provides the necessary functionalities to streamline your file management tasks.
 
+Core concepts and explanation:
+- Archyves are wrappers for built in generators that enable the user to loop through directories revursively.
+- To represent each item that the archyve finds, we have Entry objects - these are wrappers for Path objects that enable some useful features like hashing, sorting etc.
+
 ## Features
 
 - **Sorting:** Organize your files based on various criteria such as file type, size, date modified, etc.
 - **Duplicate Finding:** Identify and manage duplicate files to free up storage space.
 - **Equality Checking:** Compare files to ensure they are identical or different.
 - **Removal Tools:** Safely remove unwanted files from your archives.
 
@@ -58,12 +62,15 @@
 2. Get a list of all non-text files recursively in a given directory:
    
    ```python
    from archyve import Archyve, EntryType
    
    # Create an archyve
    archyve: Archyve = Archyve(r"p1", r"p2")
+   
    # Filter the archyve entries on whatever you need
    archyve = archyve.filter(lambda e: not e.is_type(EntryType.TEXT))
+   
+   # Loop through the archyve and print the entries
    for entry in archyve:
       print(entry)
    ```
```

