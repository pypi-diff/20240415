# Comparing `tmp/pasta_man-1.0.1.tar.gz` & `tmp/pasta_man-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.1.tar", last modified: Mon Apr 15 01:31:51 2024, max compression
+gzip compressed data, was "pasta_man-1.0.2.tar", last modified: Mon Apr 15 08:53:45 2024, max compression
```

## Comparing `pasta_man-1.0.1.tar` & `pasta_man-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.518836 pasta_man-1.0.1/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.1/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     5460 2024-04-15 01:31:51.518396 pasta_man-1.0.1/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3009 2024-04-15 01:10:20.000000 pasta_man-1.0.1/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1407 2024-04-15 01:31:37.000000 pasta_man-1.0.1/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 01:31:51.518900 pasta_man-1.0.1/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.507884 pasta_man-1.0.1/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.513940 pasta_man-1.0.1/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/__main__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/exceptions.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9961 2024-04-15 01:31:37.000000 pasta_man-1.0.1/src/pasta_man/gui.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/helptext.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     3623 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/pasta_man.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 01:10:20.000000 pasta_man-1.0.1/src/pasta_man/targets.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 01:31:51.517806 pasta_man-1.0.1/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     5460 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      463 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       59 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 01:31:51.000000 pasta_man-1.0.1/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.186797 pasta_man-1.0.2/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.2/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     5763 2024-04-15 08:53:45.186317 pasta_man-1.0.2/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3312 2024-04-15 08:21:04.000000 pasta_man-1.0.2/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1407 2024-04-15 01:32:28.000000 pasta_man-1.0.2/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 08:53:45.186864 pasta_man-1.0.2/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.176022 pasta_man-1.0.2/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.182072 pasta_man-1.0.2/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/__main__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/exceptions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    10798 2024-04-15 08:51:18.000000 pasta_man-1.0.2/src/pasta_man/gui.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/helptext.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     3623 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/pasta_man.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/targets.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.185654 pasta_man-1.0.2/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     5763 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      463 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       59 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0.1/LICENSE` & `pasta_man-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.1/PKG-INFO` & `pasta_man-1.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.1
+Version: 1.0.2
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -44,14 +44,20 @@
 Requires-Dist: cryptography
 Requires-Dist: pandas
 Requires-Dist: termcolor
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 
+![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
+![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
+
+
 # Overview
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
 
 ## Motivation
  - In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
  - The repeated use of single password in multiple accounts may lead to data breach or loss of data.
  - Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
@@ -79,15 +85,15 @@
 `For Example:`<br>
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
 ## Dependencies
-- Python >= v3.9+
+- Python>=3.9
 - pandas
 - tk
 - termcolor
 - pyperclip
 - optioner>=1.5.2
 - cryptography
```

### Comparing `pasta_man-1.0.1/README.md` & `pasta_man-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
+![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
+
+
 # Overview
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
 
 ## Motivation
  - In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
  - The repeated use of single password in multiple accounts may lead to data breach or loss of data.
  - Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
@@ -29,15 +35,15 @@
 `For Example:`<br>
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
 ## Dependencies
-- Python >= v3.9+
+- Python>=3.9
 - pandas
 - tk
 - termcolor
 - pyperclip
 - optioner>=1.5.2
 - cryptography
```

### Comparing `pasta_man-1.0.1/pyproject.toml` & `pasta_man-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0.1"
+version = "1.0.2"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `pasta_man-1.0.1/src/pasta_man/encryption.py` & `pasta_man-1.0.2/src/pasta_man/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.1/src/pasta_man/gui.py` & `pasta_man-1.0.2/src/pasta_man/gui.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,53 +4,72 @@
 
 # import project specific modules
 from pasta_man.targets import targets
 from pasta_man.encryption import Encryption
 
 # import libs
 from tkinter import *
-from tkinter import ttk, simpledialog, messagebox
+from tkinter import ttk, simpledialog, messagebox, PhotoImage
 from os.path import join as jPath
 from pathlib import Path
 import pyperclip
 import threading
+import ttkthemes
+import ttkthemes.themed_style
 
 class pmanager:
     def __init__(self, master:Tk, masterpassword: bytes):
         self.parent = master
         self.parent.title('Pasta-Man')
         self.parent.geometry('530x300+400+280')
         self.arch = targets(masterpassword)
+        self.style = ttkthemes.themed_style.ThemedStyle(theme='arc')
         
         # create Enclosing Frame
         self.EF = ttk.Frame(self.parent)
         self.EF.pack(fill=BOTH, expand=True)
         
         self.initthread = threading.Thread(target=self.arch.init).start()
     
     def _makeinitscreen_(self):
         # create two notebooks
         # -> Add and Get --> Get will have submods
         self.notebook = ttk.Notebook(self.EF)
         self.notebook.pack(expand=True, fill=BOTH)
         
         # -> create the tabs --> Add
+        self.hometab = Frame(self.notebook, bg='black')
         self.addtab = ttk.Frame(self.notebook)
         self.gettab = ttk.Frame(self.notebook)
         
         # -> add the tabs under notebook
+        self.notebook.add(self.hometab, text='Home')
         self.notebook.add(self.addtab, text='Add')
         self.notebook.add(self.gettab, text='Fetch')
         
+        # -> invoke _makeHome)=_ to create Home screen
+        self._makeHome_()
+        
         # -> invoke _makeAdd_ to create Add Screen
         self._makeAdd_()
         
         # -> invoke _makeFetch_ to create Fetch Screen
         self._makeFetch_()
     
+    def _makeHome_(self):
+        # -> create Enclosing frame
+        self.HEF = Frame(self.hometab, bg='black')
+        self.HEF.pack(expand=True, fill=BOTH)
+        
+        # -> Create gif frames OR LABEL
+        self.homelabel = Label(self.HEF, text="Pasta-Man is your very own Password Manager\nWith tripple layer security and the all new search.", font=('Verdana', 18))
+        self.homelabel.place(anchor='center', relx=0.5, rely=0.5)
+        
+        self.homelabel.config(bg='black', fg='white')
+    
     def _makeFetch_(self):
         # -> create eclosing frame under Fetch
         self.FEF = ttk.Frame(self.gettab)
         self.FEF.pack(fill=BOTH, expand=True)
         
         # # -> find targets and fetch it later
         # t1 = threading.Thread(target=self.arch.targets)
```

### Comparing `pasta_man-1.0.1/src/pasta_man/helptext.py` & `pasta_man-1.0.2/src/pasta_man/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.1/src/pasta_man/pasta_man.py` & `pasta_man-1.0.2/src/pasta_man/pasta_man.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.1/src/pasta_man/targets.py` & `pasta_man-1.0.2/src/pasta_man/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.1/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.2/src/pasta_man.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.1
+Version: 1.0.2
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -44,14 +44,20 @@
 Requires-Dist: cryptography
 Requires-Dist: pandas
 Requires-Dist: termcolor
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
 
+![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
+![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
+![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
+
+
 # Overview
 Pasta-Man is a software application designed to securely store passwords and sensitive information in an encrypted format. It provides users with a convenient way to manage their passwords, ensuring they are protected from unauthorized access. 
 
 ## Motivation
  - In the digital login password age we need a one stop vault for storing all our login credentials with concerned of atmost  security.
  - The repeated use of single password in multiple accounts may lead to data breach or loss of data.
  - Weak passwords are easy to interpreat for attackers, use of strong passwords is recommended,but it is difficult to remember complex passwords.
@@ -79,15 +85,15 @@
 `For Example:`<br>
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
 ## Dependencies
-- Python >= v3.9+
+- Python>=3.9
 - pandas
 - tk
 - termcolor
 - pyperclip
 - optioner>=1.5.2
 - cryptography
```

