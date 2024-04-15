# Comparing `tmp/amolkit-1.0.4.tar.gz` & `tmp/amolkit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amolkit-1.0.4.tar", last modified: Thu Apr  4 23:24:05 2024, max compression
+gzip compressed data, was "amolkit-1.0.5.tar", last modified: Mon Apr 15 21:49:28 2024, max compression
```

## Comparing `amolkit-1.0.4.tar` & `amolkit-1.0.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-04 23:24:05.636194 amolkit-1.0.4/
--rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.4/LICENSE
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-04 23:24:05.636194 amolkit-1.0.4/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.4/README.md
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-04 23:24:05.636194 amolkit-1.0.4/amolkit/
--rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.4/amolkit/EleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.4/amolkit/__init__.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.4/amolkit/amolsystem.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3406 2024-04-03 21:23:50.000000 amolkit-1.0.4/amolkit/atom.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.4/amolkit/genic.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3309 2023-08-10 06:31:01.000000 amolkit-1.0.4/amolkit/getEleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.4/amolkit/getring.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)      313 2023-08-10 20:56:51.000000 amolkit-1.0.4/amolkit/misc.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    22858 2024-04-03 22:23:43.000000 amolkit-1.0.4/amolkit/molecule.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.4/amolkit/moltransform.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.4/amolkit/parameter.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.4/amolkit/psf.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3254 2023-08-16 19:17:38.000000 amolkit-1.0.4/amolkit/stringmanip.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    17660 2023-08-19 01:57:53.000000 amolkit-1.0.4/amolkit/topology.py
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-04 23:24:05.636194 amolkit-1.0.4/amolkit.egg-info/
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)      454 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/SOURCES.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/dependency_links.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.4/amolkit.egg-info/not-zip-safe
--rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/top_level.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-04-04 23:24:05.636194 amolkit-1.0.4/setup.cfg
--rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2023-08-16 22:08:35.000000 amolkit-1.0.4/setup.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-15 21:49:28.318029 amolkit-1.0.5/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.5/LICENSE
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-15 21:49:28.318029 amolkit-1.0.5/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.5/README.md
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-15 21:49:28.318029 amolkit-1.0.5/amolkit/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.5/amolkit/EleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.5/amolkit/__init__.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.5/amolkit/amolsystem.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3406 2024-04-03 21:23:50.000000 amolkit-1.0.5/amolkit/atom.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.5/amolkit/genic.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3309 2023-08-10 06:31:01.000000 amolkit-1.0.5/amolkit/getEleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.5/amolkit/gethybridstate.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.5/amolkit/getring.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      313 2023-08-10 20:56:51.000000 amolkit-1.0.5/amolkit/misc.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23176 2024-04-15 21:29:07.000000 amolkit-1.0.5/amolkit/molecule.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.5/amolkit/moltransform.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.5/amolkit/parameter.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.5/amolkit/psf.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3254 2023-08-16 19:17:38.000000 amolkit-1.0.5/amolkit/stringmanip.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    17660 2023-08-19 01:57:53.000000 amolkit-1.0.5/amolkit/topology.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-15 21:49:28.318029 amolkit-1.0.5/amolkit.egg-info/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      480 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.5/amolkit.egg-info/not-zip-safe
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-04-15 21:49:28.000000 amolkit-1.0.5/amolkit.egg-info/top_level.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-04-15 21:49:28.318029 amolkit-1.0.5/setup.cfg
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-04-15 21:43:38.000000 amolkit-1.0.5/setup.py
```

### Comparing `amolkit-1.0.4/LICENSE` & `amolkit-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/EleInfo.py` & `amolkit-1.0.5/amolkit/EleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/amolsystem.py` & `amolkit-1.0.5/amolkit/amolsystem.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/atom.py` & `amolkit-1.0.5/amolkit/atom.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/genic.py` & `amolkit-1.0.5/amolkit/genic.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/getEleInfo.py` & `amolkit-1.0.5/amolkit/getEleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/getring.py` & `amolkit-1.0.5/amolkit/getring.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/molecule.py` & `amolkit-1.0.5/amolkit/molecule.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,25 +326,34 @@
 
 def genMol(atomnames:list,atomcoords:list,**kwargs):
     if not isinstance(atomnames,list) and not isinstance(atomcoords,list):
         raise ValueError ("Provide list of atomnames and list of coords")
     if len(atomnames) != len(atomcoords):
         raise IndexError ("Length of atomnames and coords are not same.")
     
+    resname = "RESN"; resid = 1; segname = "SEGN"
+    if 'resname' in kwargs:
+       resname = resname if resname else "RESN"
+    if 'resid' in kwargs:
+       resid = resid if resid else 1
+    if 'segname' in kwargs:
+       segname = segname if segname else "SEGN"
+
     mol = Molecule()
-    mol.nmolatoms = len(atomname) 
+    mol.nmolatoms = len(atomnames) 
     
     for i in range(len(atomnames)): 
         ind = i + 1
+        mol.atomname_byIdx[ind] = atomnames[i]
         mol.atomcoord_byIdx[ind] = atomcoords[i] 
         mol.atomserial_byIdx[ind]= ind 
         mol.atomele_byIdx[ind]   = gei.atomsymbol_by_anyatomname(atomnames[i]) 
-        mol.atomresn_byIdx[ind]  = "RESN" 
-        mol.atomresid_byIdx[ind] = 1 
-        mol.atomsegn_byIdx[ind]  = "SEGN" 
+        mol.atomresn_byIdx[ind]  = resname
+        mol.atomresid_byIdx[ind] = resid
+        mol.atomsegn_byIdx[ind]  = segname 
     return mol
 
 def coordline(molecule,ind,serialnum=None,resid=None):
     '''
     For index = ind in molinstance, this function assigns variables required 
     for writing coordinate line in crd/pdb/xyz/mol2
     Arguments:
```

### Comparing `amolkit-1.0.4/amolkit/moltransform.py` & `amolkit-1.0.5/amolkit/moltransform.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/parameter.py` & `amolkit-1.0.5/amolkit/parameter.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/psf.py` & `amolkit-1.0.5/amolkit/psf.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/stringmanip.py` & `amolkit-1.0.5/amolkit/stringmanip.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/amolkit/topology.py` & `amolkit-1.0.5/amolkit/topology.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.4/setup.py` & `amolkit-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
      with open("README.md","r") as f:
           long_description=f.read()
 except:
      long_description=""
      pass
 
 setup(name='amolkit', 
-      version='1.0.4', 
+      version='1.0.5', 
       description='Library for extracting molecule information', 
       long_description=long_description,
       url='https://github.com/anmolecule/amolkit', 
       author='Anmol Kumar', 
       author_email='anmolecule@gmail.com', 
       license='BSD 3-Clause "New" or "Revised" License',
       packages=find_packages(),
```

