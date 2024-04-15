# Comparing `tmp/pyracf-0.8.2.tar.gz` & `tmp/pyracf-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.8.2.tar", last modified: Sun Apr  7 11:10:19 2024, max compression
+gzip compressed data, was "pyracf-0.8.3.tar", last modified: Mon Apr 15 18:27:33 2024, max compression
```

## Comparing `pyracf-0.8.2.tar` & `pyracf-0.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2024-03-30 10:31:52.000000 pyracf-0.8.2/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2024-03-30 10:31:52.000000 pyracf-0.8.2/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-07 11:10:19.286604 pyracf-0.8.2/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-07 11:09:44.000000 pyracf-0.8.2/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-07 11:10:19.286604 pyracf-0.8.2/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-07 11:09:44.000000 pyracf-0.8.2/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    56865 2024-04-07 11:09:44.000000 pyracf-0.8.2/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-07 11:09:44.000000 pyracf-0.8.2/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-07 11:09:44.000000 pyracf-0.8.2/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-07 11:10:19.286604 pyracf-0.8.2/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-07 11:10:19.000000 pyracf-0.8.2/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.8.3/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.8.3/MANIFEST.in
+-rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-15 18:27:33.583570 pyracf-0.8.3/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-15 10:15:48.000000 pyracf-0.8.3/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-15 18:27:33.583570 pyracf-0.8.3/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-15 18:11:35.000000 pyracf-0.8.3/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    56953 2024-04-15 18:26:41.000000 pyracf-0.8.3/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-15 10:15:48.000000 pyracf-0.8.3/src/pyracf/getOffsets.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-15 10:15:48.000000 pyracf-0.8.3/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/src/pyracf.egg-info/
+-rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.8.2/LICENSE` & `pyracf-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.2/PKG-INFO` & `pyracf-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.2
+Version: 0.8.3
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyracf-0.8.2/README.md` & `pyracf-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.2/setup.py` & `pyracf-0.8.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.8.2",
+    version="0.8.3",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.8.2/src/pyracf/__init__.py` & `pyracf-0.8.3/src/pyracf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,14 +184,25 @@
         '''
         return RACF.accessKeywords[RACF.accessKeywords.index(level):]
 
     def __init__(self, irrdbu00=None, pickles=None, prefix=''):
 
         self._state = self.STATE_INIT
 
+                
+        # activate acl() method on our dataframes, so it get called with our instance's variables, the frame, and all optional parms
+        # e.g. msys._datasetAccess.loc[['SYS1.**']].acl(permits=True, explode=False, resolve=False, admin=False, sort="user")
+        pd.core.base.PandasObject.acl = lambda *x,**y: RACF.acl(self,*x,**y)
+
+        # generic and regex filter on the index levels of a frame
+        # e.g. msys._datasets.gfilter('SYS1.**').acl(resolve=True, allows='UPDATE', sort="user")
+        pd.core.base.PandasObject.gfilter = RACF.gfilter
+        pd.core.base.PandasObject.rfilter = RACF.rfilter
+
+
         if not irrdbu00 and not pickles:
             self._state = self.STATE_BAD
         else:
             if not pickles:
                 self._irrdbu00 = irrdbu00
                 self._state    = self.STATE_INIT
                 self._unloadlines = sum(1 for _ in open(self._irrdbu00, errors="ignore"))
@@ -219,14 +230,16 @@
             for (rtype,rinfo) in RACF._recordtype_info.items():
                 if 'publisher' in rinfo:
                     publisher = rinfo['publisher'] if rinfo['publisher']!='*' else rinfo['df'].lstrip('_')
                     if hasattr(self, rinfo['df']):
                         setattr(self, publisher, getattr(self, rinfo['df']))
                     else:
                         setattr(self, publisher, lambda x: warnings.warn(f"{publisher} has not been collected."))
+            self._state = self.STATE_CORRELATING
+            self._correlate()
             self._state = self.STATE_READY
             self._stoptime = datetime.now()
 
         else:
             # Running threads
             self.THREAD_COUNT = 0
 
@@ -351,24 +364,14 @@
     def parsed(self, rname):
         """ how many records with this name (type) were parsed """
         rtype = RACF._recordname_type[rname]
         return self._records[rtype]['parsed'] if rtype in self._records else 0
         
     def _correlate(self, thingswewant=_recordtype_info.keys()):
         """ construct tables that combine the raw dataframes for improved processing """
-        
-        # activate acl() method on our dataframes, so it get called with our instance's variables, the frame, and all optional parms
-        # e.g. msys._datasetAccess.loc[['SYS1.**']].acl(permits=True, explode=False, resolve=False, admin=False, sort="user")
-        pd.core.base.PandasObject.acl = lambda *x,**y: RACF.acl(self,*x,**y)
-
-        # generic and regex filter on the index levels of a frame
-        # e.g. msys._datasets.gfilter('SYS1.**').acl(resolve=True, allows='UPDATE', sort="user")
-        pd.core.base.PandasObject.gfilter = RACF.gfilter
-        pd.core.base.PandasObject.rfilter = RACF.rfilter
-
 
         # set consistent index columns for existing dfs: profile key, connect group+user, of profile class+key (for G.R.)
         for (rtype,rinfo) in RACF._recordtype_info.items():
             if rtype in thingswewant and rtype in self._records and self._records[rtype]['parsed']>0:
                 if "index" in rinfo:
                     keys = rinfo["index"]
                     names = [keys[i].replace(rinfo["name"]+"_","_") for i in range(len(keys))]
```

### Comparing `pyracf-0.8.2/src/pyracf/getOffsets.py` & `pyracf-0.8.3/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.2/src/pyracf/offsets.json` & `pyracf-0.8.3/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.2/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.3/src/pyracf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.2
+Version: 0.8.3
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

