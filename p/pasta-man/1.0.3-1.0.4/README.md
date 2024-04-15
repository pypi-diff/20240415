# Comparing `tmp/pasta_man-1.0.3.tar.gz` & `tmp/pasta_man-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.3.tar", last modified: Mon Apr 15 18:17:15 2024, max compression
+gzip compressed data, was "pasta_man-1.0.4.tar", last modified: Mon Apr 15 21:32:35 2024, max compression
```

## Comparing `pasta_man-1.0.3.tar` & `pasta_man-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.888887 pasta_man-1.0.3/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.3/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6508 2024-04-15 18:17:15.888438 pasta_man-1.0.3/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     4032 2024-04-15 18:16:25.000000 pasta_man-1.0.3/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1420 2024-04-15 09:34:52.000000 pasta_man-1.0.3/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 18:17:15.888945 pasta_man-1.0.3/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.877930 pasta_man-1.0.3/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.882841 pasta_man-1.0.3/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/__main__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/exceptions.py
--rw-r--r--   0 d33pster   (501) staff       (20)    11416 2024-04-15 17:27:12.000000 pasta_man-1.0.3/src/pasta_man/gui.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     3450 2024-04-15 17:30:19.000000 pasta_man-1.0.3/src/pasta_man/pasta_man.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/targets.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.887091 pasta_man-1.0.3/src/pasta_man/utilities/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 17:26:23.000000 pasta_man-1.0.3/src/pasta_man/utilities/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/utilities/helptext.py
--rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-15 18:13:03.000000 pasta_man-1.0.3/src/pasta_man/utilities/pasta_menu.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.887860 pasta_man-1.0.3/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6508 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      547 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.508106 pasta_man-1.0.4/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.4/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     7268 2024-04-15 21:32:35.507680 pasta_man-1.0.4/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     4792 2024-04-15 21:32:13.000000 pasta_man-1.0.4/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1506 2024-04-15 21:32:13.000000 pasta_man-1.0.4/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 21:32:35.508166 pasta_man-1.0.4/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.492694 pasta_man-1.0.4/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.498241 pasta_man-1.0.4/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.4/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.4/src/pasta_man/__main__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.502904 pasta_man-1.0.4/src/pasta_man/architectures/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/architectures/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11479 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/architectures/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9911 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/architectures/targets.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.4/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.4/src/pasta_man/exceptions.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     3508 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/pasta_man.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.504975 pasta_man-1.0.4/src/pasta_man/self_launch_thread/
+-rw-r--r--   0 d33pster   (501) staff       (20)      191 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/self_launch_thread/Launch.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      362 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/self_launch_thread/Launcher.py
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:13.000000 pasta_man-1.0.4/src/pasta_man/self_launch_thread/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.506387 pasta_man-1.0.4/src/pasta_man/utilities/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 18:18:11.000000 pasta_man-1.0.4/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 18:18:11.000000 pasta_man-1.0.4/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-15 18:18:11.000000 pasta_man-1.0.4/src/pasta_man/utilities/pasta_menu.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 21:32:35.507084 pasta_man-1.0.4/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     7268 2024-04-15 21:32:35.000000 pasta_man-1.0.4/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      748 2024-04-15 21:32:35.000000 pasta_man-1.0.4/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 21:32:35.000000 pasta_man-1.0.4/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)      139 2024-04-15 21:32:35.000000 pasta_man-1.0.4/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-15 21:32:35.000000 pasta_man-1.0.4/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 21:32:35.000000 pasta_man-1.0.4/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0.3/LICENSE` & `pasta_man-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.3/PKG-INFO` & `pasta_man-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.3
+Version: 1.0.4
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -91,17 +91,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar 
+Themes can be changed using the MenuBar -
 
-<!-- <img src="images/MenuBar.png"> -->
+<img src="images/MenuBar.png">
+
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -129,17 +131,37 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.3
+pip install pasta-man==1.0.4
 ```
 
+## README before [#Usage](#usage)
+
+After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man==1.0.4` -> `pasta-man` and `pasta-man-launcher`.
+
+- `pasta-man` Command
+
+    - This command will launch `pasta-man` as a separate and independent process.
+    
+    - The terminal will be usable after `pasta-man` command is run.
+    
+    - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
+
+- `pasta-man-launcher` Command
+    
+    - This will launch `pasta-man` in the terminal.
+
+    - The terminal wont be available until this process is running.
+
+    - All outputs will be logged in `stdin` (in the terminal screen)
+
 ## Usage
 
 - To run `Pasta-Man`, run the following in the terminal/CMD.
 
     ```bash
     pasta-man
     ```
```

### Comparing `pasta_man-1.0.3/README.md` & `pasta_man-1.0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,17 +40,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar 
+Themes can be changed using the MenuBar -
 
-<!-- <img src="images/MenuBar.png"> -->
+<img src="images/MenuBar.png">
+
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -78,17 +80,37 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.3
+pip install pasta-man==1.0.4
 ```
 
+## README before [#Usage](#usage)
+
+After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man==1.0.4` -> `pasta-man` and `pasta-man-launcher`.
+
+- `pasta-man` Command
+
+    - This command will launch `pasta-man` as a separate and independent process.
+    
+    - The terminal will be usable after `pasta-man` command is run.
+    
+    - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
+
+- `pasta-man-launcher` Command
+    
+    - This will launch `pasta-man` in the terminal.
+
+    - The terminal wont be available until this process is running.
+
+    - All outputs will be logged in `stdin` (in the terminal screen)
+
 ## Usage
 
 - To run `Pasta-Man`, run the following in the terminal/CMD.
 
     ```bash
     pasta-man
     ```
```

### Comparing `pasta_man-1.0.3/pyproject.toml` & `pasta_man-1.0.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0.3"
+version = "1.0.4"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -27,13 +27,14 @@
 ]
 maintainers = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
 dependencies = ['cryptography', 'pandas', 'termcolor', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes']
 
 [project.scripts]
-pasta-man = "pasta_man.pasta_man:main"
+pasta-man-launcher = "pasta_man.self_launch_thread.Launch:drumroll"
+pasta-man = "pasta_man.self_launch_thread.Launcher:main"
 
 [project.urls]
 GitHub = 'https://github.com/d33pster/pasta-man'
 Issues = 'https://github.com/d33pster/pasta-man/issues'
 Documentation = 'https://d33pster.github.io/pasta-man/'
```

### Comparing `pasta_man-1.0.3/src/pasta_man/encryption.py` & `pasta_man-1.0.4/src/pasta_man/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.3/src/pasta_man/gui.py` & `pasta_man-1.0.4/src/pasta_man/architectures/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # This is the pmanager class file
 #
 
 # import project specific modules
-from pasta_man.targets import targets
+import sys
+from pasta_man.architectures.targets import targets
 from pasta_man.encryption import Encryption
 from pasta_man.utilities.pasta_menu import __menu__
 
 # import libs
 from tkinter import *
 from tkinter import ttk, simpledialog, messagebox
 from os.path import join as jPath
@@ -172,30 +173,32 @@
         
         # reinit the _makeFetch_ to refresh newly added Entries
         for widget in self.gettab.winfo_children():
             widget.destroy()
         
         self._makeFetch_()
     
-    def decryptthread(self, masterpassword: str):
-        denc = Encryption("pastaman".encode('ascii'), masterpassword.encode('ascii'))
-        denc.unlock()
-        self.den = denc.__unencryptedstring__
     
     def copyToClipboard(self):
         
         # prepare alleged pass
         allegedpass = simpledialog.askstring("Master Password", "Enter Master Password to copy password to clipboard: ")
         
         # get masterpass
         with open(jPath(str(Path.home()), '.pastaman', '.m'), 'rb') as m:
             masterpassword = m.read() # this is encrypted
         
+        def decryptthread(masterpassword: str):
+            denc = Encryption("pastaman".encode('ascii'), masterpassword.encode('ascii'))
+            denc.unlock()
+            self.den = denc.__unencryptedstring__
+            sys.exit(0)
         
-        t1 = threading.Thread(target=self.decryptthread, args=(masterpassword.decode('ascii'),))
+        
+        t1 = threading.Thread(target=decryptthread, args=(masterpassword.decode('ascii'),))
         t1.start()
         t1.join()
         
         
         if allegedpass == self.den.decode('ascii'):
             t = threading.Thread(target=self.arch.decrypt, args=(self.arch.__searchresult__['password'],))
             t.start()
```

### Comparing `pasta_man-1.0.3/src/pasta_man/pasta_man.py` & `pasta_man-1.0.4/src/pasta_man/pasta_man.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 # version info
-__version__ = "1.0"
+__version__ = "1.0.4"
 
 # import project specific modules
-from pasta_man.gui import pmanager
+from pasta_man.architectures.gui import pmanager
 from pasta_man.encryption import Encryption
 from pasta_man.exceptions import NoneTypeVariable, OptError
 from pasta_man.utilities.helptext import helptext
 
 # import libs
 from tkinter import *
 from tkinter import simpledialog
@@ -21,20 +21,22 @@
 import threading
 
 def locker(masterpassword: str):
     global encb
     enc = Encryption("pastaman".encode('ascii'), masterpassword.encode('ascii'))
     enc.lock()
     encb = enc.__encryptedstring__
+    sys.exit(0)
 
 def unlocker(encpassword: str):
     global dencb
     denc = Encryption("pastaman".encode("ascii"), encpassword.encode('ascii'))
     denc.unlock()
     dencb = denc.__unencryptedstring__
+    sys.exit(0)
 
 def checkmfile(home = str(Path.home())) -> bytes:
     # --> find out if master password is defined -> .m file
     if not there(jPath(home, '.pastaman', '.m')):
         # ask dialog
         masterpassword = simpledialog.askstring("User Input", "Enter Master Password: ")
         # check if it is empty or non
@@ -104,11 +106,11 @@
     
     rootwindow.mainloop()
 
 if __name__=="__main__":
     encb:bytes = ''.encode('ascii')
     dencb:bytes = ''.encode('ascii')
     try:
-        main()
+        sys.exit(main())
     except KeyboardInterrupt:
         print("\n"+colored("KEYBOARD INTERRUPT", 'red'))
         sys.exit(1)
```

### Comparing `pasta_man-1.0.3/src/pasta_man/targets.py` & `pasta_man-1.0.4/src/pasta_man/architectures/targets.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from base64 import urlsafe_b64encode
 from pathlib import Path
 from os import makedirs
 from os.path import join as jPath, exists as there
 from datetime import datetime
 # from tabulate import tabulate
 import pandas as pd
+import sys
 from re import match
 
 #
 # The format to save the persistent passwords file ==>
 # key:value|key:value|...\n
 #
 #
@@ -100,14 +101,16 @@
             content = self.fernet.encrypt(content)
             
             with open(jPath(home, ".pastaman", '.passwords'), 'wb') as pfile:
                 pfile.write(content)
             
             content = None
         
+        sys.exit(0)
+        
     
     def add(self, target:str, targettype: str, username: str, password:bytes):
         """Add data in collection.
 
         Args:
             target (str): target is the place where this data is valid.
             targettype (str): example -> link, app, etc.
@@ -156,14 +159,16 @@
         newcontent = self.fernet.encrypt(newcontent.encode('ascii'))
         
         # write it
         with open(jPath(str(Path.home()), '.pastaman', '.passwords'), 'wb') as pfile:
             pfile.write(newcontent)
         
         newcontent = None
+        
+        sys.exit(0)
     
     def remove(self, target:str, username: str):
         """remove an entry from the collection of all entries.
 
         Args:
             target (str): target name.
             username (str): username.
@@ -237,27 +242,30 @@
             raise InvalidKeyword(f'{keywordtype} cannot be set as keywordtype.')
         
         self.__searchresult__ = None
         
         for dictionary in self.data:
             if searchkeyword in dictionary[keywordtype]:
                 self.__searchresult__ = dictionary
+        
+        sys.exit(0)
 
     def targets(self):
         ts:list[str] = []
         added = []
         for dictionary in self.data:
             if dictionary['target-type']!="init" and dictionary['target-type'] not in added:
                 ts.append(dictionary['target-type'])
                 added.append(dictionary['target-type'])
         
         self.__target_types__ = ts
     
     def decrypt(self, password: bytes):
         self._dec_ = self.fernet.decrypt(password).decode('ascii')
+        sys.exit(0)
     
     def export(self, exporttype: str = "csv") -> None:
         """General purpose Export. Excludes timestamp.
 
         Args:
             exporttype (str, optional): specify export type. Valid -> ['csv', 'xlsx']. Defaults to "csv".
         """
```

### Comparing `pasta_man-1.0.3/src/pasta_man/utilities/helptext.py` & `pasta_man-1.0.4/src/pasta_man/utilities/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.3/src/pasta_man/utilities/pasta_menu.py` & `pasta_man-1.0.4/src/pasta_man/utilities/pasta_menu.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.3/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.4/src/pasta_man.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.3
+Version: 1.0.4
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -91,17 +91,19 @@
 
 ### Faster than basic tkinter apps
 `Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
 
 ### Themes
 User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
 
-Themes can be changed using the MenuBar 
+Themes can be changed using the MenuBar -
 
-<!-- <img src="images/MenuBar.png"> -->
+<img src="images/MenuBar.png">
+
+###### <p align='center'>MenuBar Screenshot<p>
 
 #### Currently Supported Themes
 
 - Adapta
 - Arc
 - Aquativo
 - Black
@@ -129,17 +131,37 @@
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man==1.0.3
+pip install pasta-man==1.0.4
 ```
 
+## README before [#Usage](#usage)
+
+After update _v1.0.4_, `pasta-man` launches as a separate process. There are two commands that gets installed with `pip install pasta-man==1.0.4` -> `pasta-man` and `pasta-man-launcher`.
+
+- `pasta-man` Command
+
+    - This command will launch `pasta-man` as a separate and independent process.
+    
+    - The terminal will be usable after `pasta-man` command is run.
+    
+    - The output logs will be stored in -> `HOME/.pastaman/.log` in Linux and MacOS.
+
+- `pasta-man-launcher` Command
+    
+    - This will launch `pasta-man` in the terminal.
+
+    - The terminal wont be available until this process is running.
+
+    - All outputs will be logged in `stdin` (in the terminal screen)
+
 ## Usage
 
 - To run `Pasta-Man`, run the following in the terminal/CMD.
 
     ```bash
     pasta-man
     ```
```

### Comparing `pasta_man-1.0.3/src/pasta_man.egg-info/SOURCES.txt` & `pasta_man-1.0.4/src/pasta_man.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 LICENSE
 README.md
 pyproject.toml
 src/pasta_man/__init__.py
 src/pasta_man/__main__.py
 src/pasta_man/encryption.py
 src/pasta_man/exceptions.py
-src/pasta_man/gui.py
 src/pasta_man/pasta_man.py
-src/pasta_man/targets.py
 src/pasta_man.egg-info/PKG-INFO
 src/pasta_man.egg-info/SOURCES.txt
 src/pasta_man.egg-info/dependency_links.txt
 src/pasta_man.egg-info/entry_points.txt
 src/pasta_man.egg-info/requires.txt
 src/pasta_man.egg-info/top_level.txt
+src/pasta_man/architectures/__init__.py
+src/pasta_man/architectures/gui.py
+src/pasta_man/architectures/targets.py
+src/pasta_man/self_launch_thread/Launch.py
+src/pasta_man/self_launch_thread/Launcher.py
+src/pasta_man/self_launch_thread/__init__.py
 src/pasta_man/utilities/__init__.py
 src/pasta_man/utilities/helptext.py
 src/pasta_man/utilities/pasta_menu.py
```

