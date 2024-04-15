# Comparing `tmp/VASP2KP-1.1.1.tar.gz` & `tmp/VASP2KP-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VASP2KP-1.1.1.tar", last modified: Sat Apr 13 14:57:39 2024, max compression
+gzip compressed data, was "VASP2KP-1.1.2.tar", last modified: Mon Apr 15 02:34:27 2024, max compression
```

## Comparing `VASP2KP-1.1.1.tar` & `VASP2KP-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-13 14:57:39.310530 VASP2KP-1.1.1/
--rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.1/LICENSE.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-13 14:57:39.310247 VASP2KP-1.1.1/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.1/README.md
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-13 14:57:39.308596 VASP2KP-1.1.1/VASP2KP/
--rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.1/VASP2KP/__init__.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    31348 2024-04-13 14:51:46.000000 VASP2KP-1.1.1/VASP2KP/_get_kp_Zeeman.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.1/VASP2KP/_numeric_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    51333 2024-04-13 14:47:52.000000 VASP2KP-1.1.1/VASP2KP/_read_data.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    91234 2024-04-13 14:23:44.000000 VASP2KP-1.1.1/VASP2KP/_standard_kp.py
--rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.1/VASP2KP/_transform_matrix.py
-drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-13 14:57:39.309955 VASP2KP-1.1.1/VASP2KP.egg-info/
--rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/PKG-INFO
--rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/SOURCES.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/dependency_links.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/not-zip-safe
--rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/requires.txt
--rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-04-13 14:57:39.000000 VASP2KP-1.1.1/VASP2KP.egg-info/top_level.txt
--rwxrwxrwx   0 shengzhang   (501) staff       (20)     8618 2024-04-13 13:03:07.000000 VASP2KP-1.1.1/mat2kp
--rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-04-13 14:57:39.310595 VASP2KP-1.1.1/setup.cfg
--rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-04-13 14:57:31.000000 VASP2KP-1.1.1/setup.py
--rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.1/vasp2mat.5.3-patch-1.0.1.sh
--rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.1/vasp2mat.6.4-patch-1.0.1.sh
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-15 02:34:27.544859 VASP2KP-1.1.2/
+-rw-r--r--   0 shengzhang   (501) staff       (20)    35145 2023-12-06 04:04:45.000000 VASP2KP-1.1.2/LICENSE.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-15 02:34:27.544617 VASP2KP-1.1.2/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1153 2023-12-06 08:17:03.000000 VASP2KP-1.1.2/README.md
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-15 02:34:27.542833 VASP2KP-1.1.2/VASP2KP/
+-rw-r--r--   0 shengzhang   (501) staff       (20)      676 2023-12-06 06:46:55.000000 VASP2KP-1.1.2/VASP2KP/__init__.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    31562 2024-04-15 02:26:54.000000 VASP2KP-1.1.2/VASP2KP/_get_kp_Zeeman.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    64667 2024-04-13 14:49:00.000000 VASP2KP-1.1.2/VASP2KP/_numeric_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    52438 2024-04-15 02:27:19.000000 VASP2KP-1.1.2/VASP2KP/_read_data.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    91234 2024-04-13 14:23:44.000000 VASP2KP-1.1.2/VASP2KP/_standard_kp.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)    24467 2024-04-13 10:00:38.000000 VASP2KP-1.1.2/VASP2KP/_transform_matrix.py
+drwxr-xr-x   0 shengzhang   (501) staff       (20)        0 2024-04-15 02:34:27.544304 VASP2KP-1.1.2/VASP2KP.egg-info/
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1205 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/PKG-INFO
+-rw-r--r--   0 shengzhang   (501) staff       (20)      421 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/SOURCES.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/dependency_links.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        1 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/not-zip-safe
+-rw-r--r--   0 shengzhang   (501) staff       (20)       34 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/requires.txt
+-rw-r--r--   0 shengzhang   (501) staff       (20)        8 2024-04-15 02:34:27.000000 VASP2KP-1.1.2/VASP2KP.egg-info/top_level.txt
+-rwxrwxrwx   0 shengzhang   (501) staff       (20)     8381 2024-04-15 02:27:44.000000 VASP2KP-1.1.2/mat2kp
+-rw-r--r--   0 shengzhang   (501) staff       (20)       38 2024-04-15 02:34:27.544908 VASP2KP-1.1.2/setup.cfg
+-rw-r--r--   0 shengzhang   (501) staff       (20)     1720 2024-04-15 02:34:23.000000 VASP2KP-1.1.2/setup.py
+-rw-r--r--   0 shengzhang   (501) staff       (20)   129670 2023-12-06 06:49:23.000000 VASP2KP-1.1.2/vasp2mat.5.3-patch-1.0.1.sh
+-rw-r--r--   0 shengzhang   (501) staff       (20)   128779 2023-12-06 06:50:33.000000 VASP2KP-1.1.2/vasp2mat.6.4-patch-1.0.1.sh
```

### Comparing `VASP2KP-1.1.1/LICENSE.txt` & `VASP2KP-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/PKG-INFO` & `VASP2KP-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.1/README.md` & `VASP2KP-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/VASP2KP/__init__.py` & `VASP2KP-1.1.2/VASP2KP/__init__.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/VASP2KP/_get_kp_Zeeman.py` & `VASP2KP-1.1.2/VASP2KP/_get_kp_Zeeman.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,33 +138,39 @@
     # calculate the numerical kp hamiltonian and Zeeman's coupling
     numeric_kp = get_numeric_kp(pi_list,sigma_list,U,eigen_energy,band_interest_set,order,gfactor,acc)
     print("Finish downfolding processes!")
     
     # calculate the standard kp Hamiltonian
     if order>=1:
         result_kp_array,kpmodel_coe = get_std_kp(Symmetry,order,gfactor,msg_num,kvec,numeric_kp,print_flag,log)
-        print('''Finish constructing kp invariant Hamiltonian in "kp-parameters.out"!''')
+        if print_flag == 2:
+            print('''Finish constructing kp invariant Hamiltonian in "kp-parameters.out"!''')
+        else:
+            print('''Finish constructing kp invariant Hamiltonian!''')
     else:
         result_kp_array = 0
         kpmodel_coe={}
     
     if gfactor == 1: # calculate the Zeeman's coupling
     
         G_4c4 = numeric_kp["B"]
         result_Zeeman_array,Zeeman_coe = get_Zeeman(Symmetry,msg_num,kvec,G_4c4,order,print_flag,log)
-        print('''Finish constructing Zeeman's coupling in "g-factors.out"!''')
+        if print_flag == 2:
+            print('''Finish constructing Zeeman's coupling in "g-factors.out"!''')
+        else:
+            print('''Finish constructing Zeeman's coupling!''')
         return result_kp_array,kpmodel_coe,result_Zeeman_array,Zeeman_coe
     
     return result_kp_array,kpmodel_coe
 ###############################################################################
 
 
 
 ###############################################################################
-def get_std_kp_Zeeman(Symmetry,vaspMAT='mat',vmat_k = 1,kpmodel = 1, repr_split = True,order = 2,gfactor = 1,print_flag = 2,log = 0,acc = 0,msg_num = None,kvec = None):
+def get_std_kp_Zeeman(Symmetry,vaspMAT='mat',kpmodel = 1, repr_split = True,order = 2,gfactor = 1,print_flag = 2,log = 0,acc = 0,msg_num = None,kvec = None):
     '''
     The main function 
     Obtain the kp Hamiltonian matrix as well as the Zeeman's coupling as well as the numerical parameters
     
     Notice: you can treat the parameters msg_num and kvec as not existing
     
     Parameters
@@ -309,15 +315,16 @@
             print('ERROR: '+wrong_str)
             sys.exit()
     
     if kpmodel == 0:
         order = 0        
     
     # load data from .m file
-    operator,data,eigen_energy,band_interest_set,dim_list = load_data(Symmetry,vaspMAT,gfactor,vmat_k,repr_split)
+    operator,data,eigen_energy,band_interest_set,dim_list = load_data(Symmetry,vaspMAT,gfactor,repr_split)
+    
     # unified dimensions
     size = 0
     
     for i in data.keys():
         size = max(size,data[i].shape[0])
         
     eigen_energy = eigen_energy[:size]
```

### Comparing `VASP2KP-1.1.1/VASP2KP/_numeric_kp.py` & `VASP2KP-1.1.2/VASP2KP/_numeric_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/VASP2KP/_read_data.py` & `VASP2KP-1.1.2/VASP2KP/_read_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -373,15 +373,15 @@
     
     return band_start_all,band_end_all
 ###############################################################################
 
 
 
 ###############################################################################
-def load_data(Symmetry,vaspMAT,gfactor=1,vmat_k=1,repr_split = True, data_name_list=["Pi","sig"]):
+def load_data(Symmetry,vaspMAT,gfactor=1,repr_split = True, data_name_list=["Pi","sig"]):
     '''
     load all the input files
 
     Parameters
     ----------
     Symmetry : dictionary
         a dictionary according to the user's input, the rotation matrices, the standard corepresentation matrices of all generators.
@@ -402,14 +402,31 @@
         the list of eigen energies obtained by VASP.
     band_interest_set : list
         id list of the bands of interest.
     '''
     
     folder_path = vaspMAT
     
+    try:
+        file = open(os.path.join(folder_path,"MAT_Pi.m"),'r')
+    except:
+        try:
+            file = open(os.path.join(folder_path,"MAT_pi.m",'r'))
+        except:
+            print("ERROR: Cannot fild the file 'MAT_Pi.m'!")
+    file.readline()
+    file.readline()
+    kpoints = file.readline().strip().split(' ')
+    file.close()
+    
+    while '' in kpoints:
+        kpoints.remove('')
+        
+    kpoints = np.array([eval(i) for i in kpoints[3:6]])
+    
     # read the EIGENVAL file
     try:
         file=open(os.path.join(folder_path,"EIGENVAL"),"r")
         
     except:
         
         try:
@@ -436,23 +453,42 @@
         try:
             band_inf.remove('')
         except:
             break
     
     num_k = eval(band_inf[1])
     num_band = eval(band_inf[2])
-    if vmat_k > num_k:
-        print("ERROR: vmat_k is larger than the number of total kpoints!")
-        sys.exit()
+    # if vmat_k > num_k:
+    #     print("ERROR: vmat_k is larger than the number of total kpoints!")
+    #     sys.exit()
     
-    skipline = (vmat_k - 1)*(num_band + 2) + 2
+    # skipline = (vmat_k - 1)*(num_band + 2) + 2
     
-    for i in range(skipline):
-        file.readline()
+    # for i in range(skipline):
+    #     file.readline()
 
+    find_flag = False
+    for i in range(num_k):
+        file.readline()
+        kpoints_eig = file.readline().strip().split(' ')
+        while '' in kpoints_eig:
+            kpoints_eig.remove('')
+        kpoints_eig = np.array([eval(l) for l in kpoints_eig[0:3]])
+        dif = np.linalg.norm(kpoints_eig-kpoints)
+        
+        if dif < 1e-6:
+            find_flag = True
+            break
+        else:
+            for j in range(num_band):
+                file.readline()
+    
+    if not find_flag:
+        print("ERROR: Cannot find KPOINT "+str(kpoints[0])+' '+str(kpoints[1])+'  '+str(kpoints[2])+' in EIGENVAL!!!')
+    
     eigen_energy = []
     eigen_start = 0
     
     for i in file.readlines():
         i=i.strip().split(' ')
         
         # remove all '' in i
```

### Comparing `VASP2KP-1.1.1/VASP2KP/_standard_kp.py` & `VASP2KP-1.1.2/VASP2KP/_standard_kp.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/VASP2KP/_transform_matrix.py` & `VASP2KP-1.1.2/VASP2KP/_transform_matrix.py`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/VASP2KP.egg-info/PKG-INFO` & `VASP2KP-1.1.2/VASP2KP.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VASP2KP
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/zjwang11/VASP2KP
 Author: Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang
 Author-email: zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn
 License: GPLv3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `VASP2KP-1.1.1/mat2kp` & `VASP2KP-1.1.2/mat2kp`

 * *Files 2% similar despite different names*

```diff
@@ -175,22 +175,14 @@
     if 'kpmodel' in locals_key_low:
         kpmodel_id = locals_key_low.index('kpmodel')
         kpmodel = eval(locals_key[kpmodel_id])
         
     else:
         kpmodel = 1
      
-if 'vmat_k' not in locals_key:
-    
-    if 'vmat_k' in locals_key_low:
-        vmat_k_id = locals_key_low.index('vmat_k')
-        vmat_k = eval(locals_key[vmat_k_id])
-        
-    else:
-        vmat_k = 1
     
 if 'repr_split' not in locals_key:
     if 'repr_split' in locals_key_low:
         repr_split_id = locals_key_low.index('repr_split')
         repr_split = eval(locals_key[repr_split_id])
         
     else:
@@ -231,19 +223,19 @@
     print(r"Warning!!! Parameter 'print_flag' is set to 1, all the result will be output on console, not into files!")
     
     
 # calculate the result
 try:
     if no_vasp_kp:
         result_kp, result_Zeeman = \
-        get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log, vmat_k = vmat_k,repr_split = repr_split)
+        get_std_kp_Zeeman_no_coe(Symmetry, order=order, gfactor=gfactor, print_flag=print_flag, log=log, repr_split = repr_split)
     
     else:
         result_kp, result_Zeeman = \
-        get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc, vmat_k = vmat_k,repr_split = repr_split)
+        get_std_kp_Zeeman(Symmetry, vaspMAT, kpmodel=kpmodel, order=order, gfactor=gfactor, print_flag=print_flag, log=log, acc=acc, repr_split = repr_split)
 
 except:
     pass
 
 else:
     print("Congratulations! The computation of VASP2KP has finished!!!")
```

### Comparing `VASP2KP-1.1.1/setup.py` & `VASP2KP-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from setuptools import setup
 
 README = """A tool for computing k.p effective Hamiltonians and Zeeman's coupling under given symmetry constraints from VASP calculations."""
 
 
 setup(name='VASP2KP',
       python_requires=">=3.6",
-      version = "1.1.1",
+      version = "1.1.2",
       long_description=README,
       install_requires=[
         'sympy', 'numpy', 'scipy', 'kdotp_generator'
         ],
       packages=['VASP2KP'],
       author = 'Sheng Zhang, Haohao Sheng, Zhi-Da Song, Chenhao Liang, Zhijun Wang',
       author_email='zhangsheng221@mails.ucas.ac.cn, songzd@pku.edu.cn, wzj@iphy.ac.cn',
```

### Comparing `VASP2KP-1.1.1/vasp2mat.5.3-patch-1.0.1.sh` & `VASP2KP-1.1.2/vasp2mat.5.3-patch-1.0.1.sh`

 * *Files identical despite different names*

### Comparing `VASP2KP-1.1.1/vasp2mat.6.4-patch-1.0.1.sh` & `VASP2KP-1.1.2/vasp2mat.6.4-patch-1.0.1.sh`

 * *Files identical despite different names*

