# Comparing `tmp/pasta_man-1.0.tar.gz` & `tmp/pasta_man-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.tar", last modified: Mon Apr 15 00:50:29 2024, max compression
+gzip compressed data, was "pasta_man-1.0.1.tar", last modified: Mon Apr 15 01:31:51 2024, max compression
```

## Comparing `pasta_man-1.0.tar` & `pasta_man-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 00:50:29.826995 pasta_man-1.0/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-14 16:40:49.000000 pasta_man-1.0/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     5458 2024-04-15 00:50:29.826550 pasta_man-1.0/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3009 2024-04-15 00:47:58.000000 pasta_man-1.0/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1405 2024-04-15 00:49:36.000000 pasta_man-1.0/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 00:50:29.827071 pasta_man-1.0/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 00:50:29.815337 pasta_man-1.0/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 00:50:29.821913 pasta_man-1.0/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-14 16:41:38.000000 pasta_man-1.0/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 00:20:33.000000 pasta_man-1.0/src/pasta_man/__main__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-14 22:21:36.000000 pasta_man-1.0/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-14 23:07:56.000000 pasta_man-1.0/src/pasta_man/exceptions.py
--rw-r--r--   0 d33pster   (501) staff       (20)     8929 2024-04-15 00:20:45.000000 pasta_man-1.0/src/pasta_man/gui.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-14 23:15:05.000000 pasta_man-1.0/src/pasta_man/helptext.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     3623 2024-04-15 00:21:19.000000 pasta_man-1.0/src/pasta_man/pasta_man.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 00:21:27.000000 pasta_man-1.0/src/pasta_man/targets.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 00:50:29.825904 pasta_man-1.0/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     5458 2024-04-15 00:50:29.000000 pasta_man-1.0/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      463 2024-04-15 00:50:29.000000 pasta_man-1.0/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 00:50:29.000000 pasta_man-1.0/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 00:50:29.000000 pasta_man-1.0/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       59 2024-04-15 00:50:29.000000 pasta_man-1.0/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 00:50:29.000000 pasta_man-1.0/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.518836 pasta_man-1.0.1/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.1/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     5460 2024-04-15 01:31:51.518396 pasta_man-1.0.1/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3009 2024-04-15 01:10:20.000000 pasta_man-1.0.1/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1407 2024-04-15 01:31:37.000000 pasta_man-1.0.1/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 01:31:51.518900 pasta_man-1.0.1/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.507884 pasta_man-1.0.1/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.513940 pasta_man-1.0.1/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/__main__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/exceptions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9961 2024-04-15 01:31:37.000000 pasta_man-1.0.1/src/pasta_man/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/helptext.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     3623 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/pasta_man.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/targets.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.517806 pasta_man-1.0.1/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     5460 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      463 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       59 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0/LICENSE` & `pasta_man-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0/PKG-INFO` & `pasta_man-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0
+Version: 1.0.1
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

### Comparing `pasta_man-1.0/README.md` & `pasta_man-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0/pyproject.toml` & `pasta_man-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0"
+version = "1.0.1"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pasta_man-1.0/src/pasta_man/encryption.py` & `pasta_man-1.0.1/src/pasta_man/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0/src/pasta_man/gui.py` & `pasta_man-1.0.1/src/pasta_man/gui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 #
 # This is the pmanager class file
 #
 
 # import project specific modules
 from pasta_man.targets import targets
+from pasta_man.encryption import Encryption
 
 # import libs
 from tkinter import *
-from tkinter import ttk
+from tkinter import ttk, simpledialog, messagebox
+from os.path import join as jPath
+from pathlib import Path
 import pyperclip
 import threading
 
 class pmanager:
     def __init__(self, master:Tk, masterpassword: bytes):
         self.parent = master
         self.parent.title('Pasta-Man')
@@ -129,23 +132,44 @@
         
         # reinit the _makeFetch_ to refresh newly added Entries
         for widget in self.gettab.winfo_children():
             widget.destroy()
         
         self._makeFetch_()
     
-    def copyToClipboard(self):
+    def decryptthread(self, masterpassword: str):
+        denc = Encryption("pastaman".encode('ascii'), masterpassword.encode('ascii'))
+        denc.unlock()
+        self.den = denc.__unencryptedstring__
     
-        t = threading.Thread(target=self.arch.decrypt, args=(self.arch.__searchresult__['password'],))
-        t.start()
-        t.join()
-        
-        pyperclip.copy(self.arch._dec_)
-        spam = pyperclip.paste()
-        self.arch._dec_ = None
+    def copyToClipboard(self):
+        
+        # prepare alleged pass
+        allegedpass = simpledialog.askstring("Master Password", "Enter Master Password to copy password to clipboard: ")
+        
+        # get masterpass
+        with open(jPath(str(Path.home()), '.pastaman', '.m'), 'rb') as m:
+            masterpassword = m.read() # this is encrypted
+        
+        
+        t1 = threading.Thread(target=self.decryptthread, args=(masterpassword.decode('ascii'),))
+        t1.start()
+        t1.join()
+        
+        
+        if allegedpass == self.den.decode('ascii'):
+            t = threading.Thread(target=self.arch.decrypt, args=(self.arch.__searchresult__['password'],))
+            t.start()
+            t.join()
+            
+            pyperclip.copy(self.arch._dec_)
+            spam = pyperclip.paste()
+            self.arch._dec_ = None
+        else:
+            messagebox.showwarning("Wrong Master Password", "The master password entered by you is wrong!")
         
     def _makeAdd_(self):
         # -> create enclosing frame under Add
         self.AEF = ttk.Frame(self.addtab)
         self.AEF.pack(expand=True, fill=BOTH)
         
         # -> create target label and input
```

### Comparing `pasta_man-1.0/src/pasta_man/helptext.py` & `pasta_man-1.0.1/src/pasta_man/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0/src/pasta_man/pasta_man.py` & `pasta_man-1.0.1/src/pasta_man/pasta_man.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0/src/pasta_man/targets.py` & `pasta_man-1.0.1/src/pasta_man/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.1/src/pasta_man.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0
+Version: 1.0.1
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

