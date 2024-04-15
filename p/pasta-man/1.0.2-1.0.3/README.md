# Comparing `tmp/pasta_man-1.0.2.tar.gz` & `tmp/pasta_man-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasta_man-1.0.2.tar", last modified: Mon Apr 15 08:53:45 2024, max compression
+gzip compressed data, was "pasta_man-1.0.3.tar", last modified: Mon Apr 15 18:17:15 2024, max compression
```

## Comparing `pasta_man-1.0.2.tar` & `pasta_man-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.186797 pasta_man-1.0.2/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.2/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     5763 2024-04-15 08:53:45.186317 pasta_man-1.0.2/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3312 2024-04-15 08:21:04.000000 pasta_man-1.0.2/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1407 2024-04-15 01:32:28.000000 pasta_man-1.0.2/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 08:53:45.186864 pasta_man-1.0.2/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.176022 pasta_man-1.0.2/src/
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.182072 pasta_man-1.0.2/src/pasta_man/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/__init__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/__main__.py
--rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/encryption.py
--rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/exceptions.py
--rw-r--r--   0 d33pster   (501) staff       (20)    10798 2024-04-15 08:51:18.000000 pasta_man-1.0.2/src/pasta_man/gui.py
--rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/helptext.py
--rwxr-xr-x   0 d33pster   (501) staff       (20)     3623 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/pasta_man.py
--rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 01:10:20.000000 pasta_man-1.0.2/src/pasta_man/targets.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 08:53:45.185654 pasta_man-1.0.2/src/pasta_man.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     5763 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      463 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/entry_points.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       59 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/requires.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 08:53:45.000000 pasta_man-1.0.2/src/pasta_man.egg-info/top_level.txt
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.888887 pasta_man-1.0.3/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-15 01:10:20.000000 pasta_man-1.0.3/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     6508 2024-04-15 18:17:15.888438 pasta_man-1.0.3/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     4032 2024-04-15 18:16:25.000000 pasta_man-1.0.3/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1420 2024-04-15 09:34:52.000000 pasta_man-1.0.3/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-15 18:17:15.888945 pasta_man-1.0.3/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.877930 pasta_man-1.0.3/src/
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.882841 pasta_man-1.0.3/src/pasta_man/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      129 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/__main__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      776 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/encryption.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      237 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/exceptions.py
+-rw-r--r--   0 d33pster   (501) staff       (20)    11416 2024-04-15 17:27:12.000000 pasta_man-1.0.3/src/pasta_man/gui.py
+-rwxr-xr-x   0 d33pster   (501) staff       (20)     3450 2024-04-15 17:30:19.000000 pasta_man-1.0.3/src/pasta_man/pasta_man.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     9793 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/targets.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.887091 pasta_man-1.0.3/src/pasta_man/utilities/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-15 17:26:23.000000 pasta_man-1.0.3/src/pasta_man/utilities/__init__.py
+-rw-r--r--   0 d33pster   (501) staff       (20)      639 2024-04-15 01:10:20.000000 pasta_man-1.0.3/src/pasta_man/utilities/helptext.py
+-rw-r--r--   0 d33pster   (501) staff       (20)     7546 2024-04-15 18:13:03.000000 pasta_man-1.0.3/src/pasta_man/utilities/pasta_menu.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-15 18:17:15.887860 pasta_man-1.0.3/src/pasta_man.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     6508 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      547 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       55 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/entry_points.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       69 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/requires.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       10 2024-04-15 18:17:15.000000 pasta_man-1.0.3/src/pasta_man.egg-info/top_level.txt
```

### Comparing `pasta_man-1.0.2/LICENSE` & `pasta_man-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.2/PKG-INFO` & `pasta_man-1.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.2
+Version: 1.0.3
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -43,14 +43,15 @@
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: pandas
 Requires-Dist: termcolor
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
+Requires-Dist: ttkthemes
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
 
@@ -84,29 +85,59 @@
 
 `For Example:`<br>
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
+### Faster than basic tkinter apps
+`Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
+
+### Themes
+User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
+
+Themes can be changed using the MenuBar 
+
+<!-- <img src="images/MenuBar.png"> -->
+
+#### Currently Supported Themes
+
+- Adapta
+- Arc
+- Aquativo
+- Black
+- Blue
+- Breeze
+- Clearlooks
+- Elegance
+- Equilux
+- Keramic
+- Kroc
+- Plastik
+- Radiance (Ubuntu)
+- Smog
+- Win XP
+- Yaru
+
 ## Dependencies
 - Python>=3.9
 - pandas
 - tk
+- ttkthemes
 - termcolor
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man
+pip install pasta-man==1.0.3
 ```
 
 ## Usage
 
 - To run `Pasta-Man`, run the following in the terminal/CMD.
 
     ```bash
```

### Comparing `pasta_man-1.0.2/pyproject.toml` & `pasta_man-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pasta-man"
-version = "1.0.2"
+version = "1.0.3"
 description = "Password Manager"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Software Development",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -24,15 +24,15 @@
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"},
     {name = "Sairam Pimple", email = "sairampimple003@gmail.com"},
     {name = "Shubham Narendra Singh", email = "shubh1122000@gmail.com"}
 ]
 maintainers = [
     {name = "Soumyo Deep Gupta", email = "deep.main.ac@gmail.com"}
 ]
-dependencies = ['cryptography', 'pandas', 'termcolor', 'tk', 'optioner>=1.5.2', 'pyperclip']
+dependencies = ['cryptography', 'pandas', 'termcolor', 'tk', 'optioner>=1.5.2', 'pyperclip', 'ttkthemes']
 
 [project.scripts]
 pasta-man = "pasta_man.pasta_man:main"
 
 [project.urls]
 GitHub = 'https://github.com/d33pster/pasta-man'
 Issues = 'https://github.com/d33pster/pasta-man/issues'
```

### Comparing `pasta_man-1.0.2/src/pasta_man/encryption.py` & `pasta_man-1.0.3/src/pasta_man/encryption.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.2/src/pasta_man/gui.py` & `pasta_man-1.0.3/src/pasta_man/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 #
 # This is the pmanager class file
 #
 
 # import project specific modules
 from pasta_man.targets import targets
 from pasta_man.encryption import Encryption
+from pasta_man.utilities.pasta_menu import __menu__
 
 # import libs
 from tkinter import *
-from tkinter import ttk, simpledialog, messagebox, PhotoImage
+from tkinter import ttk, simpledialog, messagebox
 from os.path import join as jPath
 from pathlib import Path
 import pyperclip
 import threading
-import ttkthemes
-import ttkthemes.themed_style
 
 class pmanager:
     def __init__(self, master:Tk, masterpassword: bytes):
+        # create a master object
         self.parent = master
+        # set title
         self.parent.title('Pasta-Man')
+        # set geometry
         self.parent.geometry('530x300+400+280')
+        # set architecture
         self.arch = targets(masterpassword)
-        self.style = ttkthemes.themed_style.ThemedStyle(theme='arc')
+        
+        # set menu
+        menu = Menu(self.parent)
+        self.parent.config(menu=menu)
+        # -> add menus
+        self.pasta_menu = __menu__(menuparent=menu)
+        self.pasta_menu.Themes()
         
         # create Enclosing Frame
         self.EF = ttk.Frame(self.parent)
         self.EF.pack(fill=BOTH, expand=True)
         
         self.initthread = threading.Thread(target=self.arch.init).start()
     
@@ -58,17 +67,29 @@
     def _makeHome_(self):
         # -> create Enclosing frame
         self.HEF = Frame(self.hometab, bg='black')
         self.HEF.pack(expand=True, fill=BOTH)
         
         # -> Create gif frames OR LABEL
         self.homelabel = Label(self.HEF, text="Pasta-Man is your very own Password Manager\nWith tripple layer security and the all new search.", font=('Verdana', 18))
-        self.homelabel.place(anchor='center', relx=0.5, rely=0.5)
+        self.homelabel.place(anchor='center', relx=0.5, rely=0.35)
         
         self.homelabel.config(bg='black', fg='white')
+        
+        # -> create a button
+        self.homeNextLabel = Label(self.HEF, text="Next >", bg='black', fg='white', font=('Verdana', 15))
+        self.homeNextLabel.place(anchor='center', relx=0.5, rely=0.67)
+        
+        # -> bind command
+        self.homeNextLabel.bind('<Button-1>', lambda e: self.homenext())
+    
+    def homenext(self):
+        self.notebook.select(1)
+        # -> set focus to targetEntry
+        self.targetEntry.focus()
     
     def _makeFetch_(self):
         # -> create eclosing frame under Fetch
         self.FEF = ttk.Frame(self.gettab)
         self.FEF.pack(fill=BOTH, expand=True)
         
         # # -> find targets and fetch it later
@@ -216,28 +237,25 @@
         self.usernameEntry.place(anchor='center', rely=0.4, relx=0.57)
         
         # -> create password label and input
         self.passLabel = ttk.Label(self.AEF, text='Password:')
         self.passLabel.place(anchor='center', relx=0.235, rely=0.52)
         # --> textvar for passEntry
         self.varpass = StringVar()
-        self.passEntry = ttk.Entry(self.AEF, width=25, show="!", textvariable=self.varpass)
+        self.passEntry = ttk.Entry(self.AEF, width=25, show="-", textvariable=self.varpass)
         self.passEntry.place(anchor='center', rely=0.52, relx=0.57)
         
         # -> create Add button
         self.addbutton = ttk.Button(self.AEF, text='[ Add ]', default=ACTIVE, command=self.add)
         self.addbutton.place(anchor='center', relx=0.5, rely=0.76)
         
         # -> create status label
         self.status = StringVar()
         self.statusbar = ttk.Label(self.AEF, textvariable=self.status)
         self.statusbar.place(anchor='center', relx=0.5, rely=0.88)
-
-        # -> set focus to targetEntry
-        self.targetEntry.focus()
         
         # -> bind pass entry with enter
         self.passEntry.bind('<Return>', self.add)
     
     def fetchstatusReset(self):
         self.fetchstatusvar.set('')
```

### Comparing `pasta_man-1.0.2/src/pasta_man/helptext.py` & `pasta_man-1.0.3/src/pasta_man/utilities/helptext.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.2/src/pasta_man/pasta_man.py` & `pasta_man-1.0.3/src/pasta_man/pasta_man.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # version info
 __version__ = "1.0"
 
 # import project specific modules
 from pasta_man.gui import pmanager
 from pasta_man.encryption import Encryption
 from pasta_man.exceptions import NoneTypeVariable, OptError
-from pasta_man.helptext import helptext
+from pasta_man.utilities.helptext import helptext
 
 # import libs
 from tkinter import *
 from tkinter import simpledialog
 from termcolor import colored
 from pathlib import Path
 from os.path import join as jPath, exists as there
@@ -38,19 +38,14 @@
         # ask dialog
         masterpassword = simpledialog.askstring("User Input", "Enter Master Password: ")
         # check if it is empty or non
         if masterpassword=='' or masterpassword==None:
             raise NoneTypeVariable('Aborted.')
         # encode it
         masterpassword = masterpassword.encode('ascii')
-        # lock it -> store it
-        # -> define Encryption object
-        # enc = Encryption("pastaman".encode('ascii'), masterpassword)
-        # # -> lock it
-        # enc.lock()
         enct = threading.Thread(target=locker, args=(masterpassword.decode('ascii'),))
         enct.start()
         enct.join()
         # -> store it
         with open(jPath(home, '.pastaman', '.m'), 'wb') as m:
             m.write(encb)
     else:
```

### Comparing `pasta_man-1.0.2/src/pasta_man/targets.py` & `pasta_man-1.0.3/src/pasta_man/targets.py`

 * *Files identical despite different names*

### Comparing `pasta_man-1.0.2/src/pasta_man.egg-info/PKG-INFO` & `pasta_man-1.0.3/src/pasta_man.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasta-man
-Version: 1.0.2
+Version: 1.0.3
 Summary: Password Manager
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>, Sairam Pimple <sairampimple003@gmail.com>, Shubham Narendra Singh <shubh1122000@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -43,14 +43,15 @@
 License-File: LICENSE
 Requires-Dist: cryptography
 Requires-Dist: pandas
 Requires-Dist: termcolor
 Requires-Dist: tk
 Requires-Dist: optioner>=1.5.2
 Requires-Dist: pyperclip
+Requires-Dist: ttkthemes
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pasta-man)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pasta-man)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pasta-man)
 ![PyPI - License](https://img.shields.io/pypi/l/pasta-man)
 
 
@@ -84,29 +85,59 @@
 
 `For Example:`<br>
 If there is a target (say, abcde) which contains a keyword (say, abc), the user can search `abc` in `keyword-type == target`. Similarly, if there is a target-type (say, link) which contains a keyword (say, github), the user can search for `github` in `keyword-type == target-type`.
 
 ### Copy to Clipboard
 Upon [Search](#search), `Pasta-Man` allows to copy the password for the found match to user's clipboard (given, the user provides the master password), instead of revealing it because of bad management. `Pasta-Man` also allows to Remove that match search result.
 
+### Faster than basic tkinter apps
+`Pasta-Man` actively uses Threads to carry out intensive tasks in order to minimize GUI lag as well as have better performance than any basic app created through python tkinter lib.
+
+### Themes
+User can now change Theme for the app from the Menu Bar. Default is `Arc`. Whatever theme the user chooses, It will be set as default and next time `Pasta-Man` is launched, that theme will be loaded.
+
+Themes can be changed using the MenuBar 
+
+<!-- <img src="images/MenuBar.png"> -->
+
+#### Currently Supported Themes
+
+- Adapta
+- Arc
+- Aquativo
+- Black
+- Blue
+- Breeze
+- Clearlooks
+- Elegance
+- Equilux
+- Keramic
+- Kroc
+- Plastik
+- Radiance (Ubuntu)
+- Smog
+- Win XP
+- Yaru
+
 ## Dependencies
 - Python>=3.9
 - pandas
 - tk
+- ttkthemes
 - termcolor
 - pyperclip
 - optioner>=1.5.2
 - cryptography
 
 ## Installation
 
 Easily install pasta-man using pip.
 
 ```bash
-pip install pasta-man
+pip install pasta-man==1.0.3
 ```
 
 ## Usage
 
 - To run `Pasta-Man`, run the following in the terminal/CMD.
 
     ```bash
```

