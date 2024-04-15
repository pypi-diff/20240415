# Comparing `tmp/pyAnaf-0.0.2.tar.gz` & `tmp/pyanaf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyAnaf-0.0.2.tar", last modified: Wed Dec 12 20:19:20 2018, max compression
+gzip compressed data, was "pyanaf-0.0.3.tar", last modified: Mon Apr 15 10:58:29 2024, max compression
```

## Comparing `pyAnaf-0.0.2.tar` & `pyanaf-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 radu       (501) staff       (20)        0 2018-12-12 20:19:20.000000 pyAnaf-0.0.2/
--rw-r--r--   0 radu       (501) staff       (20)     4429 2018-12-12 20:19:20.000000 pyAnaf-0.0.2/PKG-INFO
-drwxr-xr-x   0 radu       (501) staff       (20)        0 2018-12-12 20:19:20.000000 pyAnaf-0.0.2/pyAnaf.egg-info/
--rw-r--r--   0 radu       (501) staff       (20)     4429 2018-12-12 20:19:19.000000 pyAnaf-0.0.2/pyAnaf.egg-info/PKG-INFO
--rw-r--r--   0 radu       (501) staff       (20)      239 2018-12-12 20:19:19.000000 pyAnaf-0.0.2/pyAnaf.egg-info/SOURCES.txt
--rw-r--r--   0 radu       (501) staff       (20)       48 2018-12-12 20:19:19.000000 pyAnaf-0.0.2/pyAnaf.egg-info/entry_points.txt
--rw-r--r--   0 radu       (501) staff       (20)        7 2018-12-12 20:19:19.000000 pyAnaf-0.0.2/pyAnaf.egg-info/top_level.txt
--rw-r--r--   0 radu       (501) staff       (20)        1 2018-12-12 20:19:19.000000 pyAnaf-0.0.2/pyAnaf.egg-info/dependency_links.txt
-drwxr-xr-x   0 radu       (501) staff       (20)        0 2018-12-12 20:19:20.000000 pyAnaf-0.0.2/pyAnaf/
--rw-r--r--   0 radu       (501) staff       (20)     1314 2018-12-12 19:23:48.000000 pyAnaf-0.0.2/pyAnaf/console.py
--rw-r--r--   0 radu       (501) staff       (20)      520 2018-12-12 17:05:25.000000 pyAnaf-0.0.2/pyAnaf/models.py
--rw-r--r--   0 radu       (501) staff       (20)        0 2018-12-12 14:05:51.000000 pyAnaf-0.0.2/pyAnaf/__init__.py
--rw-r--r--   0 radu       (501) staff       (20)     4308 2018-12-12 19:23:59.000000 pyAnaf-0.0.2/pyAnaf/api.py
--rw-r--r--   0 radu       (501) staff       (20)     2350 2018-12-12 19:31:43.000000 pyAnaf-0.0.2/README.md
--rw-r--r--   0 radu       (501) staff       (20)     1532 2018-12-12 20:09:58.000000 pyAnaf-0.0.2/setup.py
--rw-r--r--   0 radu       (501) staff       (20)       38 2018-12-12 20:19:20.000000 pyAnaf-0.0.2/setup.cfg
+drwxr-xr-x   0 alexmacstudio   (501) staff       (20)        0 2024-04-15 10:58:29.867930 pyanaf-0.0.3/
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)       62 2024-04-15 08:40:29.000000 pyanaf-0.0.3/AUTHORS
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     1055 2024-04-15 08:40:29.000000 pyanaf-0.0.3/LICENSE
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     3755 2024-04-15 10:58:29.867715 pyanaf-0.0.3/PKG-INFO
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     2352 2024-04-15 10:20:07.000000 pyanaf-0.0.3/README.md
+drwxr-xr-x   0 alexmacstudio   (501) staff       (20)        0 2024-04-15 10:58:29.866638 pyanaf-0.0.3/pyAnaf/
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)        0 2024-04-15 08:40:29.000000 pyanaf-0.0.3/pyAnaf/__init__.py
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     3681 2024-04-15 10:14:18.000000 pyanaf-0.0.3/pyAnaf/api.py
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     1286 2024-04-15 09:54:06.000000 pyanaf-0.0.3/pyAnaf/console.py
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)      667 2024-04-15 10:13:34.000000 pyanaf-0.0.3/pyAnaf/models.py
+drwxr-xr-x   0 alexmacstudio   (501) staff       (20)        0 2024-04-15 10:58:29.867542 pyanaf-0.0.3/pyAnaf.egg-info/
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     3755 2024-04-15 10:58:29.000000 pyanaf-0.0.3/pyAnaf.egg-info/PKG-INFO
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)      255 2024-04-15 10:58:29.000000 pyanaf-0.0.3/pyAnaf.egg-info/SOURCES.txt
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)        1 2024-04-15 10:58:29.000000 pyanaf-0.0.3/pyAnaf.egg-info/dependency_links.txt
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)       47 2024-04-15 10:58:29.000000 pyanaf-0.0.3/pyAnaf.egg-info/entry_points.txt
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)        7 2024-04-15 10:58:29.000000 pyanaf-0.0.3/pyAnaf.egg-info/top_level.txt
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)       38 2024-04-15 10:58:29.867971 pyanaf-0.0.3/setup.cfg
+-rw-r--r--   0 alexmacstudio   (501) staff       (20)     1681 2024-04-15 10:17:18.000000 pyanaf-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyAnaf-0.0.2/PKG-INFO` & `pyanaf-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,136 @@
 Metadata-Version: 2.1
 Name: pyAnaf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper API of ANAF web services
 Home-page: https://github.com/agilegeeks/pyAnaf.git
 Author: Radu Boncea
 Author-email: radu.boncea@gmail.com
-License: UNKNOWN
-Description: # A wrapper API of ANAF web services
-        
-        
-        ## Compatibility
-        >=Python 2.6
-        Tested on python 2.6, 3.4, 3.5 and 3.6
-        
-        ## Installation
-        
-            $ pip install pyAnaf
-        
-        
-        ## Usage
-        
-        ##### From Python:
-        
-        ```python
-        import datetime
-        from pyAnaf.api import Anaf
-        
-        anaf = Anaf()
-        anaf.setLimit(500) #optional
-        
-        # adding a list of CUIs and an optional query date
-        anaf.setCUIList( [36804251, 2785503], date =  datetime.date.today())
-        
-        # adding a CUI one by one
-        anaf.addCUI(36804251)
-        anaf.addCUI(2785503)
-        
-        # submit the request to ANAF and hope for the best
-        anaf.Request()
-        
-        # printing the json returned from ANAF
-        print (anaf.result)
-        
-        # or doing more programmatic stuff
-        first_cui = anaf.getCUIData(36804251)
-        print (first_cui.cui)
-        print (first_cui.name)
-        print (first_cui.address)
-        print (first_cui.is_active)
-        print (first_cui.vat_eligible)
-        print (first_cui.vat_split_eligible)
-        print (first_cui.vat_collection_eligible)
-        
-        ```
-        
-        ##### From the console:
-        
-        	$ pyanaf <list_of_CUIs> <max_limit>
-        
-        For python3 you might have to set python encoding for your environment (e.g. export PYTHONIOENCODING=utf-8)
-        
-        E.g.:
-        
-            $ pyanaf 36804251,2785503 500
-            $ {   'adresa': '',
-            'cui': 34434,
-            'data': '2018-12-12',
-            'dataActualizareTvaInc': '',
-            'dataAnulareSplitTVA': '',
-            'dataInactivare': ' ',
-            'dataInceputSplitTVA': '',
-            'dataInceputTvaInc': '',
-            'dataPublicare': ' ',
-            'dataPublicareTvaInc': '',
-            'dataRadiere': ' ',
-            'dataReactivare': ' ',
-            'dataSfarsitTvaInc': '',
-            'data_anul_imp_ScpTVA': '',
-            'data_inceput_ScpTVA': '',
-            'data_sfarsit_ScpTVA': '',
-            'denumire': '',
-            'mesaj_ScpTVA': '',
-            'scpTVA': False,
-            'statusInactivi': False,
-            'statusSplitTVA': False,
-            'statusTvaIncasare': False,
-            'tipActTvaInc': ''}
-        	{   'adresa': '',
-            'cui': 2,
-            'data': '2018-12-12',
-            'dataActualizareTvaInc': '',
-            'dataAnulareSplitTVA': '',
-            'dataInactivare': ' ',
-            'dataInceputSplitTVA': '',
-            'dataInceputTvaInc': '',
-            'dataPublicare': ' ',
-            'dataPublicareTvaInc': '',
-            'dataRadiere': ' ',
-            'dataReactivare': ' ',
-            'dataSfarsitTvaInc': '',
-            'data_anul_imp_ScpTVA': '',
-            'data_inceput_ScpTVA': '',
-            'data_sfarsit_ScpTVA': '',
-            'denumire': '',
-            'mesaj_ScpTVA': '',
-            'scpTVA': False,
-            'statusInactivi': False,
-            'statusSplitTVA': False,
-            'statusTvaIncasare': False,
-            'tipActTvaInc': ''}
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# A wrapper API of ANAF web services
+
+
+## Compatibility
+>=Python 3.4
+Tested on python 3.4, 3.5, 3.6, and 3.11
+
+## Installation
+
+    $ pip install pyAnaf
+
+
+## Usage
+
+##### From Python:
+
+```python
+import datetime
+from pyAnaf.api import Anaf
+
+anaf = Anaf()
+anaf.setLimit(500) #optional
+
+# adding a list of CUIs and an optional query date
+anaf.setCUIList( [36804251, 2785503], date =  datetime.date.today())
+
+# adding a CUI one by one
+anaf.addCUI(36804251)
+anaf.addCUI(2785503)
+
+# submit the request to ANAF and hope for the best
+anaf.Request()
+
+# printing the json returned from ANAF
+print (anaf.result)
+
+# or doing more programmatic stuff
+first_cui = anaf.getCUIData(36804251)
+print (first_cui.cui)
+print (first_cui.name)
+print (first_cui.address)
+print (first_cui.is_active)
+print (first_cui.vat_eligible)
+print (first_cui.vat_split_eligible)
+print (first_cui.vat_collection_eligible)
+
+```
+
+##### From the console:
+
+	$ pyanaf <list_of_CUIs> <max_limit>
+
+For python3 you might have to set python encoding for your environment (e.g. export PYTHONIOENCODING=utf-8)
+
+E.g.:
+
+    $ pyanaf 36804251,2785503 500
+    $ {   'adresa': '',
+    'cui': 34434,
+    'data': '2018-12-12',
+    'dataActualizareTvaInc': '',
+    'dataAnulareSplitTVA': '',
+    'dataInactivare': ' ',
+    'dataInceputSplitTVA': '',
+    'dataInceputTvaInc': '',
+    'dataPublicare': ' ',
+    'dataPublicareTvaInc': '',
+    'dataRadiere': ' ',
+    'dataReactivare': ' ',
+    'dataSfarsitTvaInc': '',
+    'data_anul_imp_ScpTVA': '',
+    'data_inceput_ScpTVA': '',
+    'data_sfarsit_ScpTVA': '',
+    'denumire': '',
+    'mesaj_ScpTVA': '',
+    'scpTVA': False,
+    'statusInactivi': False,
+    'statusSplitTVA': False,
+    'statusTvaIncasare': False,
+    'tipActTvaInc': ''}
+	{   'adresa': '',
+    'cui': 2,
+    'data': '2018-12-12',
+    'dataActualizareTvaInc': '',
+    'dataAnulareSplitTVA': '',
+    'dataInactivare': ' ',
+    'dataInceputSplitTVA': '',
+    'dataInceputTvaInc': '',
+    'dataPublicare': ' ',
+    'dataPublicareTvaInc': '',
+    'dataRadiere': ' ',
+    'dataReactivare': ' ',
+    'dataSfarsitTvaInc': '',
+    'data_anul_imp_ScpTVA': '',
+    'data_inceput_ScpTVA': '',
+    'data_sfarsit_ScpTVA': '',
+    'denumire': '',
+    'mesaj_ScpTVA': '',
+    'scpTVA': False,
+    'statusInactivi': False,
+    'statusSplitTVA': False,
+    'statusTvaIncasare': False,
+    'tipActTvaInc': ''}
```

### Comparing `pyAnaf-0.0.2/pyAnaf.egg-info/PKG-INFO` & `pyanaf-0.0.3/pyAnaf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,136 @@
 Metadata-Version: 2.1
 Name: pyAnaf
-Version: 0.0.2
+Version: 0.0.3
 Summary: A wrapper API of ANAF web services
 Home-page: https://github.com/agilegeeks/pyAnaf.git
 Author: Radu Boncea
 Author-email: radu.boncea@gmail.com
-License: UNKNOWN
-Description: # A wrapper API of ANAF web services
-        
-        
-        ## Compatibility
-        >=Python 2.6
-        Tested on python 2.6, 3.4, 3.5 and 3.6
-        
-        ## Installation
-        
-            $ pip install pyAnaf
-        
-        
-        ## Usage
-        
-        ##### From Python:
-        
-        ```python
-        import datetime
-        from pyAnaf.api import Anaf
-        
-        anaf = Anaf()
-        anaf.setLimit(500) #optional
-        
-        # adding a list of CUIs and an optional query date
-        anaf.setCUIList( [36804251, 2785503], date =  datetime.date.today())
-        
-        # adding a CUI one by one
-        anaf.addCUI(36804251)
-        anaf.addCUI(2785503)
-        
-        # submit the request to ANAF and hope for the best
-        anaf.Request()
-        
-        # printing the json returned from ANAF
-        print (anaf.result)
-        
-        # or doing more programmatic stuff
-        first_cui = anaf.getCUIData(36804251)
-        print (first_cui.cui)
-        print (first_cui.name)
-        print (first_cui.address)
-        print (first_cui.is_active)
-        print (first_cui.vat_eligible)
-        print (first_cui.vat_split_eligible)
-        print (first_cui.vat_collection_eligible)
-        
-        ```
-        
-        ##### From the console:
-        
-        	$ pyanaf <list_of_CUIs> <max_limit>
-        
-        For python3 you might have to set python encoding for your environment (e.g. export PYTHONIOENCODING=utf-8)
-        
-        E.g.:
-        
-            $ pyanaf 36804251,2785503 500
-            $ {   'adresa': '',
-            'cui': 34434,
-            'data': '2018-12-12',
-            'dataActualizareTvaInc': '',
-            'dataAnulareSplitTVA': '',
-            'dataInactivare': ' ',
-            'dataInceputSplitTVA': '',
-            'dataInceputTvaInc': '',
-            'dataPublicare': ' ',
-            'dataPublicareTvaInc': '',
-            'dataRadiere': ' ',
-            'dataReactivare': ' ',
-            'dataSfarsitTvaInc': '',
-            'data_anul_imp_ScpTVA': '',
-            'data_inceput_ScpTVA': '',
-            'data_sfarsit_ScpTVA': '',
-            'denumire': '',
-            'mesaj_ScpTVA': '',
-            'scpTVA': False,
-            'statusInactivi': False,
-            'statusSplitTVA': False,
-            'statusTvaIncasare': False,
-            'tipActTvaInc': ''}
-        	{   'adresa': '',
-            'cui': 2,
-            'data': '2018-12-12',
-            'dataActualizareTvaInc': '',
-            'dataAnulareSplitTVA': '',
-            'dataInactivare': ' ',
-            'dataInceputSplitTVA': '',
-            'dataInceputTvaInc': '',
-            'dataPublicare': ' ',
-            'dataPublicareTvaInc': '',
-            'dataRadiere': ' ',
-            'dataReactivare': ' ',
-            'dataSfarsitTvaInc': '',
-            'data_anul_imp_ScpTVA': '',
-            'data_inceput_ScpTVA': '',
-            'data_sfarsit_ScpTVA': '',
-            'denumire': '',
-            'mesaj_ScpTVA': '',
-            'scpTVA': False,
-            'statusInactivi': False,
-            'statusSplitTVA': False,
-            'statusTvaIncasare': False,
-            'tipActTvaInc': ''}
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.0
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: 3.2
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database :: Front-Ends
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# A wrapper API of ANAF web services
+
+
+## Compatibility
+>=Python 3.4
+Tested on python 3.4, 3.5, 3.6, and 3.11
+
+## Installation
+
+    $ pip install pyAnaf
+
+
+## Usage
+
+##### From Python:
+
+```python
+import datetime
+from pyAnaf.api import Anaf
+
+anaf = Anaf()
+anaf.setLimit(500) #optional
+
+# adding a list of CUIs and an optional query date
+anaf.setCUIList( [36804251, 2785503], date =  datetime.date.today())
+
+# adding a CUI one by one
+anaf.addCUI(36804251)
+anaf.addCUI(2785503)
+
+# submit the request to ANAF and hope for the best
+anaf.Request()
+
+# printing the json returned from ANAF
+print (anaf.result)
+
+# or doing more programmatic stuff
+first_cui = anaf.getCUIData(36804251)
+print (first_cui.cui)
+print (first_cui.name)
+print (first_cui.address)
+print (first_cui.is_active)
+print (first_cui.vat_eligible)
+print (first_cui.vat_split_eligible)
+print (first_cui.vat_collection_eligible)
+
+```
+
+##### From the console:
+
+	$ pyanaf <list_of_CUIs> <max_limit>
+
+For python3 you might have to set python encoding for your environment (e.g. export PYTHONIOENCODING=utf-8)
+
+E.g.:
+
+    $ pyanaf 36804251,2785503 500
+    $ {   'adresa': '',
+    'cui': 34434,
+    'data': '2018-12-12',
+    'dataActualizareTvaInc': '',
+    'dataAnulareSplitTVA': '',
+    'dataInactivare': ' ',
+    'dataInceputSplitTVA': '',
+    'dataInceputTvaInc': '',
+    'dataPublicare': ' ',
+    'dataPublicareTvaInc': '',
+    'dataRadiere': ' ',
+    'dataReactivare': ' ',
+    'dataSfarsitTvaInc': '',
+    'data_anul_imp_ScpTVA': '',
+    'data_inceput_ScpTVA': '',
+    'data_sfarsit_ScpTVA': '',
+    'denumire': '',
+    'mesaj_ScpTVA': '',
+    'scpTVA': False,
+    'statusInactivi': False,
+    'statusSplitTVA': False,
+    'statusTvaIncasare': False,
+    'tipActTvaInc': ''}
+	{   'adresa': '',
+    'cui': 2,
+    'data': '2018-12-12',
+    'dataActualizareTvaInc': '',
+    'dataAnulareSplitTVA': '',
+    'dataInactivare': ' ',
+    'dataInceputSplitTVA': '',
+    'dataInceputTvaInc': '',
+    'dataPublicare': ' ',
+    'dataPublicareTvaInc': '',
+    'dataRadiere': ' ',
+    'dataReactivare': ' ',
+    'dataSfarsitTvaInc': '',
+    'data_anul_imp_ScpTVA': '',
+    'data_inceput_ScpTVA': '',
+    'data_sfarsit_ScpTVA': '',
+    'denumire': '',
+    'mesaj_ScpTVA': '',
+    'scpTVA': False,
+    'statusInactivi': False,
+    'statusSplitTVA': False,
+    'statusTvaIncasare': False,
+    'tipActTvaInc': ''}
```

### Comparing `pyAnaf-0.0.2/pyAnaf/console.py` & `pyanaf-0.0.3/pyAnaf/console.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,59 @@
 # coding: utf-8
-
-from __future__ import print_function
 import sys
 import os
 import datetime
 import pprint
 
 
 try:
     from pyAnaf.api import Anaf
 except:
-    sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
+    sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
     from pyAnaf.api import Anaf
 
 
-class MyPrettyPrinter(pprint.PrettyPrinter):
+class CustomPrettyPrinter(pprint.PrettyPrinter):
     def format(self, object, context, maxlevels, level):
-        #print (type(object))
-        #print (object)
+        # print (type(object))
+        # print (object)
         # if isinstance(object, str):
         #     return (object.encode('utf8'), True, False)
         return pprint.PrettyPrinter.format(self, object, context, maxlevels, level)
 
+
 def print_err(*args, **kwargs):
     print(*args, file=sys.stderr, **kwargs)
 
+
 def main():
     if len(sys.argv) < 2:
         print_err("usage: %s <cuis_separated_by_comma> <limit>\n" % sys.argv[0])
         sys.exit(-255)
 
     limit = 5
-
-    cuis = sys.argv[1].split(',')
-
+    cuis = sys.argv[1].split(",")
 
     try:
         limit = int(sys.argv[2])
     except:
         pass
 
     today = datetime.date.today()
-
     anaf = Anaf()
     anaf.setLimit(limit)
+
     for cui in cuis:
         try:
             anaf.addCUI(int(cui), date=today)
         except Exception as e:
             print_err(e)
 
     anaf.Request()
+    pp = CustomPrettyPrinter(indent=4)
 
-    pp = MyPrettyPrinter(indent=4)
     for entry in anaf.result:
         pp.pprint(entry)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `pyAnaf-0.0.2/pyAnaf/api.py` & `pyanaf-0.0.3/pyAnaf/api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,110 +1,85 @@
-from __future__ import unicode_literals, print_function
-
 import datetime
-import sys
-
-PY_3_OR_HIGHER = sys.version_info >= (3, 0)
-
-try:
-    import urllib.request as urllib_request
-    import urllib.error as urllib_error
-except ImportError:
-    import urllib2 as urllib_request
-    import urllib2 as urllib_error
-
-try:
-    from cStringIO import StringIO
-except ImportError:
-    from io import BytesIO as StringIO
-
-try:
-    import http.client as http_client
-except ImportError:
-    import httplib as http_client
-
-try:
-    import json
-except ImportError:
-    import simplejson as json
-
+import json
+import urllib.request as urllib_request
+import urllib.error as urllib_error
 from .models import AnafResultEntry
 
 
 class AnafError(Exception):
     """
     Base Exception thrown by the Anaf object when there is a
     general error interacting with the API.
     """
+
     pass
 
 
 class AnafHTTPError(Exception):
     """
     Exception thrown by the Anaf object when there is an
     HTTP error interacting with anaf.ro.
     """
+
     pass
 
 
 class AnafResponseError(Exception):
     """
     Exception thrown by the Anaf object when there is an
     error the response returned from ANAF.
     """
+
     pass
 
 
-class Anaf(object):
+class Anaf:
     WS_ENDPOINTS = {
-        'sync': 'https://webservicesp.anaf.ro/PlatitorTvaRest/api/v3/ws/tva',
-        'async': 'https://webservicesp.anaf.ro/AsynchWebService/api/v3/ws/tva'
+        "sync": "https://webservicesp.anaf.ro/PlatitorTvaRest/api/v8/ws/tva",
+        "async": "https://webservicesp.anaf.ro/AsynchWebService/api/v8/ws/tva",
     }
     LIMIT = 500
 
     def __init__(self):
         self.cuis = {}
         self.result = None
         self.entries = {}
 
     @staticmethod
     def _validate_cui(cui):
         if not isinstance(cui, int):
-            raise AnafError('CUI should be integer')
+            raise AnafError("CUI should be integer")
 
     @staticmethod
     def _validate_date(date):
         if not isinstance(date, datetime.date):
-            raise AnafError('Date should be of type datetime.date')
+            raise AnafError("Date should be of type datetime.date")
 
     @staticmethod
     def _prepare_data(data):
-        if PY_3_OR_HIGHER:
-            return bytes(data, 'utf-8')
-        else:
-            return data
-
-    def addEndpoint(self, url, target='sync'):
-        if target not in ['sync', 'async']:
-            raise AnafError('Invalid target for endpoint. Must be one of \'sync\' or \'async\'')
+        return bytes(data, "utf-8")
+
+    def addEndpoint(self, url, target="sync"):
+        if target not in ["sync", "async"]:
+            raise AnafError("Invalid target for endpoint. Must be one of 'sync' or 'async'")
 
-        self.WS_ENDPOINTS[target] = url;
+        self.WS_ENDPOINTS[target] = url
 
     def setLimit(self, limit):
         try:
             self.LIMIT = int(limit)
         except:
-            raise AnafError('Limit should be an integer')
+            raise AnafError("Limit should be an integer")
 
     def setCUIList(self, cui_list=[], date=None):
         if date is None:
             date = datetime.date.today()
 
         if len(cui_list) > self.LIMIT:
-            raise AnafError('Too many CUIs to be queried. Should limit to %d' % self.LIMIT)
+            raise AnafError("Too many CUIs to be queried. Should limit to %d" % self.LIMIT)
 
         self._validate_date(date)
         for cui in cui_list:
             self._validate_cui(cui)
             self.cuis[cui] = date
 
     def addCUI(self, cui, date=None):
@@ -112,50 +87,45 @@
             date = datetime.date.today()
 
         self._validate_cui(cui)
         self._validate_date(date)
 
         self.cuis[cui] = date
         if len(self.cuis.items()) > self.LIMIT:
-            raise AnafError('Too many CUIs to be queried. Should limit to %d' % self.LIMIT)
+            raise AnafError("Too many CUIs to be queried. Should limit to %d" % self.LIMIT)
 
     def Request(self):
         # translate cuis entries to ANAF json format
         cui_list = []
         for entry in self.cuis.items():
-            cui_list.append(
-                {
-                    'cui': entry[0],
-                    'data': entry[1].isoformat()
-                }
-            )
+            cui_list.append({"cui": entry[0], "data": entry[1].isoformat()})
 
-        request = urllib_request.Request(self.WS_ENDPOINTS['sync'])
-        request.add_header('Content-Type', 'application/json')
+        request = urllib_request.Request(self.WS_ENDPOINTS["sync"])
+        request.add_header("Content-Type", "application/json")
 
         try:
             response = urllib_request.urlopen(request, self._prepare_data(json.dumps(cui_list)))
         except urllib_error.HTTPError as e:
-            raise AnafHTTPError('Error connecting to ANAF. Got a %d HTTP code.' % e.code)
+            raise AnafHTTPError("Error connecting to ANAF. Got a %d HTTP code." % e.code)
 
         data = response.read()
         if isinstance(data, bytes):
-            data = data.decode('utf-8')
+            data = data.decode("utf-8")
         try:
             result = json.loads(data)
         except:
-            raise AnafResponseError('Error parsing json response from ANAF.')
+            raise AnafResponseError("Error parsing json response from ANAF.")
 
-        if result['cod'] != 200:
-            raise AnafResponseError('%s' % result['message'])
+        if result["cod"] != 200:
+            raise AnafResponseError("%s" % result["message"])
 
-        result = result['found']
+        result = result["found"]
         self.result = result
 
         for entry in result:
-            self.entries[entry['cui']] = AnafResultEntry(entry)
+            self.entries[entry["date_generale"]["cui"]] = AnafResultEntry(entry)
 
     def getCUIData(self, cui):
         if cui not in self.entries.keys():
             return None
 
         return self.entries[cui]
```

### Comparing `pyAnaf-0.0.2/README.md` & `pyanaf-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # A wrapper API of ANAF web services
 
 
 ## Compatibility
->=Python 2.6
-Tested on python 2.6, 3.4, 3.5 and 3.6
+>=Python 3.4
+Tested on python 3.4, 3.5, 3.6, and 3.11
 
 ## Installation
 
     $ pip install pyAnaf
 
 
 ## Usage
```

### Comparing `pyAnaf-0.0.2/setup.py` & `pyanaf-0.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyAnaf",
-    version="0.0.2",
+    version="0.0.3",
     author="Radu Boncea",
     author_email="radu.boncea@gmail.com",
     description="A wrapper API of ANAF web services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/agilegeeks/pyAnaf.git",
     packages=setuptools.find_packages(),
@@ -21,22 +21,25 @@
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 2.6",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Database :: Front-Ends",
         "Topic :: Office/Business :: Financial :: Accounting",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
     ],
 )
```

