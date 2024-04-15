# Comparing `tmp/gwdali-0.1.3.tar.gz` & `tmp/gwdali-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdali-0.1.3.tar", last modified: Wed Apr 10 15:32:32 2024, max compression
+gzip compressed data, was "gwdali-0.1.4.tar", last modified: Mon Apr 15 18:28:18 2024, max compression
```

## Comparing `gwdali-0.1.3.tar` & `gwdali-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.466494 gwdali-0.1.3/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.454492 gwdali-0.1.3/GWDALI/
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.462494 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78018 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_CE.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78021 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_ET.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    83058 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_K.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    56323 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_L.txt
--rwxrwxr-x   0 josiel    (1000) josiel    (1000)    84000 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_V.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       14 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/__init__.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      921 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/Detectors_Sensitivity/plot_Sn.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     6741 2024-03-08 17:26:00.000000 gwdali-0.1.3/GWDALI/GWDALI.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      143 2024-02-12 16:14:07.000000 gwdali-0.1.3/GWDALI/__init__.py
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.466494 gwdali-0.1.3/GWDALI/lib/
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     3381 2024-03-07 16:18:03.000000 gwdali-0.1.3/GWDALI/lib/Angles_lib.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     4429 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/Auxiliar.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     5858 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/Corner_Plots.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     2685 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/Dictionaries.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     8866 2024-04-10 14:58:57.000000 gwdali-0.1.3/GWDALI/lib/Diff_Signal_Tensors.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     4303 2024-03-08 17:28:57.000000 gwdali-0.1.3/GWDALI/lib/Get_Tensors.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     8245 2024-04-09 20:19:01.000000 gwdali-0.1.3/GWDALI/lib/Likelihood.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)     4181 2024-04-09 19:50:18.000000 gwdali-0.1.3/GWDALI/lib/Waveforms.py
--rw-rw-r--   0 josiel    (1000) josiel    (1000)      145 2024-02-29 14:02:42.000000 gwdali-0.1.3/GWDALI/lib/__init__.py
--rw-r--r--   0 josiel    (1000) josiel    (1000)     1519 2024-02-07 21:23:28.000000 gwdali-0.1.3/LICENSE
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5178 2024-04-10 15:32:32.466494 gwdali-0.1.3/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)     4822 2023-07-17 17:42:50.000000 gwdali-0.1.3/README.md
-drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-10 15:32:32.466494 gwdali-0.1.3/gwdali.egg-info/
--rw-r--r--   0 josiel    (1000) josiel    (1000)     5178 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/PKG-INFO
--rw-r--r--   0 josiel    (1000) josiel    (1000)      689 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/SOURCES.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)        1 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/dependency_links.txt
--rw-r--r--   0 josiel    (1000) josiel    (1000)        7 2024-04-10 15:32:32.000000 gwdali-0.1.3/gwdali.egg-info/top_level.txt
--rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2024-04-10 15:32:32.466494 gwdali-0.1.3/setup.cfg
--rw-r--r--   0 josiel    (1000) josiel    (1000)      767 2024-04-10 15:31:33.000000 gwdali-0.1.3/setup.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-15 18:28:18.085377 gwdali-0.1.4/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-15 18:28:18.073376 gwdali-0.1.4/GWDALI/
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-15 18:28:18.077376 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78018 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_CE.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    78021 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_ET.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    83058 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_K.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    56323 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_L.txt
+-rwxrwxr-x   0 josiel    (1000) josiel    (1000)    84000 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_V.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       14 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/__init__.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      921 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/Detectors_Sensitivity/plot_Sn.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     6750 2024-04-15 18:26:19.000000 gwdali-0.1.4/GWDALI/GWDALI.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      143 2024-02-12 16:14:07.000000 gwdali-0.1.4/GWDALI/__init__.py
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-15 18:28:18.085377 gwdali-0.1.4/GWDALI/lib/
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     3381 2024-03-07 16:18:03.000000 gwdali-0.1.4/GWDALI/lib/Angles_lib.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     4429 2024-02-29 14:02:42.000000 gwdali-0.1.4/GWDALI/lib/Auxiliar.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     5858 2024-02-29 14:02:42.000000 gwdali-0.1.4/GWDALI/lib/Corner_Plots.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     2685 2024-02-29 14:02:42.000000 gwdali-0.1.4/GWDALI/lib/Dictionaries.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     9658 2024-04-15 13:11:30.000000 gwdali-0.1.4/GWDALI/lib/Diff_Signal_Tensors.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     4303 2024-03-08 17:28:57.000000 gwdali-0.1.4/GWDALI/lib/Get_Tensors.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     8783 2024-04-15 18:07:53.000000 gwdali-0.1.4/GWDALI/lib/Likelihood.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)     4181 2024-04-09 19:50:18.000000 gwdali-0.1.4/GWDALI/lib/Waveforms.py
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)      145 2024-02-29 14:02:42.000000 gwdali-0.1.4/GWDALI/lib/__init__.py
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     1519 2024-02-07 21:23:28.000000 gwdali-0.1.4/LICENSE
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5627 2024-04-15 18:28:18.085377 gwdali-0.1.4/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5271 2024-04-15 18:26:25.000000 gwdali-0.1.4/README.md
+drwxrwxr-x   0 josiel    (1000) josiel    (1000)        0 2024-04-15 18:28:18.085377 gwdali-0.1.4/gwdali.egg-info/
+-rw-r--r--   0 josiel    (1000) josiel    (1000)     5627 2024-04-15 18:28:18.000000 gwdali-0.1.4/gwdali.egg-info/PKG-INFO
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      689 2024-04-15 18:28:18.000000 gwdali-0.1.4/gwdali.egg-info/SOURCES.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)        1 2024-04-15 18:28:18.000000 gwdali-0.1.4/gwdali.egg-info/dependency_links.txt
+-rw-r--r--   0 josiel    (1000) josiel    (1000)        7 2024-04-15 18:28:18.000000 gwdali-0.1.4/gwdali.egg-info/top_level.txt
+-rw-rw-r--   0 josiel    (1000) josiel    (1000)       38 2024-04-15 18:28:18.085377 gwdali-0.1.4/setup.cfg
+-rw-r--r--   0 josiel    (1000) josiel    (1000)      767 2024-04-15 18:27:10.000000 gwdali-0.1.4/setup.py
```

### Comparing `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_CE.txt` & `gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_CE.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_ET.txt` & `gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_ET.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_K.txt` & `gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_K.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_L.txt` & `gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_L.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/Sn_V.txt` & `gwdali-0.1.4/GWDALI/Detectors_Sensitivity/Sn_V.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/Detectors_Sensitivity/plot_Sn.py` & `gwdali-0.1.4/GWDALI/Detectors_Sensitivity/plot_Sn.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/GWDALI.py` & `gwdali-0.1.4/GWDALI/GWDALI.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,9 +185,9 @@
 	Result['SNR']	  = SNR
 	Result['Tensors'] = Tensors
 
 	if(save_samples): Aux.Save_Samples(path,index,Detection_Dict,FreeParams,M)
 	if(plot_corner): Aux.PlotCorner(M,truths,Cov,FreeParams,[dT_min,dT_sec],dali_method,path,index)
 
 	# Result (dict)
-	# keys: Fisher, CovFisher, Covariance, Samples, Error, Recovery, SNR
+	# keys: Fisher, CovFisher, Covariance, Samples, Error, Recovery, SNR, Tensors
 	return Result
```

### Comparing `gwdali-0.1.3/GWDALI/lib/Angles_lib.py` & `gwdali-0.1.4/GWDALI/lib/Angles_lib.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/lib/Auxiliar.py` & `gwdali-0.1.4/GWDALI/lib/Auxiliar.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/lib/Corner_Plots.py` & `gwdali-0.1.4/GWDALI/lib/Corner_Plots.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/lib/Dictionaries.py` & `gwdali-0.1.4/GWDALI/lib/Dictionaries.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/lib/Diff_Signal_Tensors.py` & `gwdali-0.1.4/GWDALI/lib/Diff_Signal_Tensors.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,37 @@
 		dL = prms["DL"] * 1.e3
 	else:
 		print(">> Parameter 'DL' not found!")
 		print(">> Received Parameters:", list(prms.keys()))
 		quit()
 	return dL
 
+def get_spins(prms):
+	if(all([x in prms.keys() for x in ['sx1','sy1','sz1','sx2','sy2','sz2'] ])):
+		sx1 = prms['sx1']
+		sy1 = prms['sy1']
+		sz1 = prms['sz1']
+		sx2 = prms['sx2']
+		sy2 = prms['sy2']
+		sz2 = prms['sz2']
+	elif( all( [x in prms.keys() for x in ['S1','theta_1','phi_1','S2','theta_2','phi_2']] ) ):
+		sx1 = prms['S1']*np.sin( prms['theta_1'] )*np.cos( prms['phi_1'] )
+		sy1 = prms['S1']*np.sin( prms['theta_1'] )*np.sin( prms['phi_1'] )
+		sz1 = prms['S1']*np.cos( prms['theta_1'] )
+		sx2 = prms['S2']*np.sin( prms['theta_2'] )*np.cos( prms['phi_2'] )
+		sy2 = prms['S2']*np.sin( prms['theta_2'] )*np.sin( prms['phi_2'] )
+		sz2 = prms['S2']*np.cos( prms['theta_2'] )
+	else:
+		print(">> Invalid or Incomplete Spin Inputs!")
+		print(">> GWDALI works with:")
+		print("\t ['S1','theta_1','phi_1','S2','theta_2','phi_2'] , or")
+		print("\t ['sx1','sy1','sz1','sx2','sy2','sz2']")
+		quit()
+	return [sx1, sy1, sz1], [sx2, sy2, sz2]
+
 def get_mass(prms):
 	keys = list(prms.keys())
 	Mass = {}	
 	for key in keys:
 		if( key in ['m1','m2','q','eta','Mc'] ):
 			Mass[key] = prms[key]
 	
@@ -134,23 +157,15 @@
 	keys = list(params.keys())
 	
 	m1, m2   = get_mass(params)
 	iota 	 = get_iota(params) # rad
 	DL       = get_dL(params)   # Mpc
 	psi      = params['psi']    # rad
 
-	sx1 = params['sx1']
-	sy1 = params['sy1']
-	sz1 = params['sz1']
-	sx2 = params['sx2']
-	sy2 = params['sy2']
-	sz2 = params['sz2']
-
-	s1 = [sx1, sy1, sz1]
-	s2 = [sx2, sy2, sz2]
+	s1, s2 = get_spins(params)
 
 	hp, hx, freq0 = wf.Waveforms(m1,m2,iota,DL,s1,s2,freq, approx=approx)
 
 	return hp, hx, freq0
 
 # det: abreviation of detector
 def Signal(params,dets,approx):
@@ -178,16 +193,16 @@
 
 	# t_coal := t_(0,a)
 	# tau_ab := tau_a - tau_b = t_(0,a) - t_(0,b)
 	# t_(0,b) = t_(0,a) - tau_ab
 	Phase = 2*np.pi*freq0*(t_coal-tau_ab) - phi_coal
 	H = (Fp*hp + Fx*hx)*np.exp(1.j*Phase)
 	
-	#gw_signal = interp1d(freq0,H,bounds_error=False,fill_value='extrapolate')
-	#h = gw_signal(freq)
+	gw_signal = interp1d(freq0,H,bounds_error=False,fill_value='extrapolate')
+	H = gw_signal(freq)
 
 	return H
 
 #-------------------------------------------------
 
 # eps (standard) = 1.e-6
 def split_prms(params,x,eps, diff_order):
```

### Comparing `gwdali-0.1.3/GWDALI/lib/Get_Tensors.py` & `gwdali-0.1.4/GWDALI/lib/Get_Tensors.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/GWDALI/lib/Likelihood.py` & `gwdali-0.1.4/GWDALI/lib/Likelihood.py`

 * *Files 10% similar despite different names*

```diff
@@ -152,14 +152,21 @@
 #----------------------------#----------------------------#----------------------------
 Priors_std['sx1']    = bilby.core.prior.Uniform(name='sx1',minimum=0, maximum=1.0)
 Priors_std['sy1']    = bilby.core.prior.Uniform(name='sy1',minimum=0, maximum=1.0)
 Priors_std['sz1']    = bilby.core.prior.Uniform(name='sz1',minimum=0, maximum=1.0)
 Priors_std['sx2']    = bilby.core.prior.Uniform(name='sx2',minimum=0, maximum=1.0)
 Priors_std['sy2']    = bilby.core.prior.Uniform(name='sy2',minimum=0, maximum=1.0)
 Priors_std['sz2']    = bilby.core.prior.Uniform(name='sz2',minimum=0, maximum=1.0)
+#----------------------------
+Priors_std['S1']		= bilby.core.prior.Uniform(name='S1',minimum=0, maximum=.9)
+Priors_std['theta_1']	= bilby.core.prior.Sine(name='theta_1',minimum=0, maximum=np.pi)
+Priors_std['phi_1']		= bilby.core.prior.Uniform(name='phi_1',minimum=0, maximum=2*np.pi)
+Priors_std['S2']		= bilby.core.prior.Uniform(name='S2',minimum=0, maximum=.9)
+Priors_std['theta_2']	= bilby.core.prior.Sine(name='theta_2',minimum=0, maximum=np.pi)
+Priors_std['phi_2']		= bilby.core.prior.Uniform(name='phi_2',minimum=0, maximum=2*np.pi)
 #----------------------------#----------------------------#----------------------------
 Priors_std['phi_coal']  = bilby.core.prior.Uniform(name='phi_coal',minimum=0, maximum=2*np.pi) # radians
 Priors_std['t_coal']    = bilby.core.prior.Uniform(name='t_coal',minimum=0, maximum=3600) # seconds
 #----------------------------#----------------------------#----------------------------
 
 def get_posterior(FreeParams, Theta0, Detection_Dict, GwData, approximant, Detectors, Tensors, dali_method, sampler_method, npoints,new_priors):
 	Priors = {}
```

### Comparing `gwdali-0.1.3/GWDALI/lib/Waveforms.py` & `gwdali-0.1.4/GWDALI/lib/Waveforms.py`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/LICENSE` & `gwdali-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/PKG-INFO` & `gwdali-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: josiel.jms7@gmail.com
 License: BSD 3-Clause License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -75,36 +75,44 @@
     #----------------------------------------------------------------------
     # "approximant" options:
     #               [Leading_Order, TaylorF2_py, ...] or any lal approximant
     #----------------------------------------------------------------------
     # "dali_method" options:
     #               [Fisher, Fisher_Sampling, Doublet, Triplet, Standard]
     #----------------------------------------------------------------------
-    res = gw.GWDALI( Detection_Dict = params,
-                     FreeParams     = FreeParams,
-                     detectors      = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer
-                     approximant    = 'TaylorF2_py',
-                     dali_method    = 'Doublet',
-                     sampler_method = 'nestle', # Same as Bilby sampling method
-                     save_fisher    = False,
-                     save_cov       = False,
-                     plot_corner    = False,
-                     save_samples   = False,
-                     hide_info      = True,
-                     index          = 1,
-                     rcond          = 1.e-4,
-                     npoints=300) # points for "nested sampling" or steps/walkers for "MCMC"
+    res = gw.GWDALI(Detection_Dict = params, 
+                    FreeParams = FreeParams, 
+                    detectors = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer, 
+                    approximant = 'TaylorF2_py',
+                    fmin  = 1., 
+                    fmax  = 1.e4, 
+                    fsize = 3000, 
+                    dali_method    = 'Doublet',
+                    sampler_method = 'nestle', # Same as Bilby sampling method
+                    npoints      = 300, # points for "nested sampling" or steps/walkers for "MCMC"
+                    rcond        = 1.e-4,
+                    new_priors   = None, # If you want to change the standard priors
+                    save_samples = False, 
+                    save_cov     = False, 
+                    save_fisher  = False,
+                    plot_corner  = False,
+                    hide_info    = False,
+                    step_size    = 1.e-6, # dx := max( step_size , step_size*abs(x) )
+                    diff_order   = 2, # Numerical Derivative (Finite Difference) precision O(2) or O(4)
+                    run_sampler  = True, # If you want to run MCMC.
+                    index        = 1)
 
     Samples = res['Samples']
     Fisher  = res['Fisher']
     CovFish = res['CovFisher']
     Cov     = res['Covariance']
     Rec     = res['Recovery']
     Err     = res['Error']
     SNR     = res['SNR']
+    Tensors = res['Tensors']
 
 ## References
 
 [1] L. S. Finn and D. F. Chernoff, “Observing binary inspiral in gravitational radiation: One interferometer,” Phys. Rev. D, vol. 47, pp. 2198–2219, 1993.
 
 [2] E. Sellentin, M. Quartin, and L. Amendola, “Breaking the spell of gaussianity: forecasting with higher order fisher matrices,” Monthly Notices of the Royal Astronomical Society, vol. 441, no. 2, pp. 1831–1840, 2014.
```

### Comparing `gwdali-0.1.3/README.md` & `gwdali-0.1.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -64,36 +64,44 @@
     #----------------------------------------------------------------------
     # "approximant" options:
     #               [Leading_Order, TaylorF2_py, ...] or any lal approximant
     #----------------------------------------------------------------------
     # "dali_method" options:
     #               [Fisher, Fisher_Sampling, Doublet, Triplet, Standard]
     #----------------------------------------------------------------------
-    res = gw.GWDALI( Detection_Dict = params,
-                     FreeParams     = FreeParams,
-                     detectors      = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer
-                     approximant    = 'TaylorF2_py',
-                     dali_method    = 'Doublet',
-                     sampler_method = 'nestle', # Same as Bilby sampling method
-                     save_fisher    = False,
-                     save_cov       = False,
-                     plot_corner    = False,
-                     save_samples   = False,
-                     hide_info      = True,
-                     index          = 1,
-                     rcond          = 1.e-4,
-                     npoints=300) # points for "nested sampling" or steps/walkers for "MCMC"
+    res = gw.GWDALI(Detection_Dict = params, 
+                    FreeParams = FreeParams, 
+                    detectors = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer, 
+                    approximant = 'TaylorF2_py',
+                    fmin  = 1., 
+                    fmax  = 1.e4, 
+                    fsize = 3000, 
+                    dali_method    = 'Doublet',
+                    sampler_method = 'nestle', # Same as Bilby sampling method
+                    npoints      = 300, # points for "nested sampling" or steps/walkers for "MCMC"
+                    rcond        = 1.e-4,
+                    new_priors   = None, # If you want to change the standard priors
+                    save_samples = False, 
+                    save_cov     = False, 
+                    save_fisher  = False,
+                    plot_corner  = False,
+                    hide_info    = False,
+                    step_size    = 1.e-6, # dx := max( step_size , step_size*abs(x) )
+                    diff_order   = 2, # Numerical Derivative (Finite Difference) precision O(2) or O(4)
+                    run_sampler  = True, # If you want to run MCMC.
+                    index        = 1)
 
     Samples = res['Samples']
     Fisher  = res['Fisher']
     CovFish = res['CovFisher']
     Cov     = res['Covariance']
     Rec     = res['Recovery']
     Err     = res['Error']
     SNR     = res['SNR']
+    Tensors = res['Tensors']
 
 ## References
 
 [1] L. S. Finn and D. F. Chernoff, “Observing binary inspiral in gravitational radiation: One interferometer,” Phys. Rev. D, vol. 47, pp. 2198–2219, 1993.
 
 [2] E. Sellentin, M. Quartin, and L. Amendola, “Breaking the spell of gaussianity: forecasting with higher order fisher matrices,” Monthly Notices of the Royal Astronomical Society, vol. 441, no. 2, pp. 1831–1840, 2014.
```

### Comparing `gwdali-0.1.3/gwdali.egg-info/PKG-INFO` & `gwdali-0.1.4/gwdali.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdali
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Fisher-Based Software for Parameter Estimation from Gravitational Waves
 Author: Josiel Mendonça Soares de Souza
 Author-email: josiel.jms7@gmail.com
 License: BSD 3-Clause License
 Keywords: fisher matrix,gravitational waves,gw,dali
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -75,36 +75,44 @@
     #----------------------------------------------------------------------
     # "approximant" options:
     #               [Leading_Order, TaylorF2_py, ...] or any lal approximant
     #----------------------------------------------------------------------
     # "dali_method" options:
     #               [Fisher, Fisher_Sampling, Doublet, Triplet, Standard]
     #----------------------------------------------------------------------
-    res = gw.GWDALI( Detection_Dict = params,
-                     FreeParams     = FreeParams,
-                     detectors      = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer
-                     approximant    = 'TaylorF2_py',
-                     dali_method    = 'Doublet',
-                     sampler_method = 'nestle', # Same as Bilby sampling method
-                     save_fisher    = False,
-                     save_cov       = False,
-                     plot_corner    = False,
-                     save_samples   = False,
-                     hide_info      = True,
-                     index          = 1,
-                     rcond          = 1.e-4,
-                     npoints=300) # points for "nested sampling" or steps/walkers for "MCMC"
+    res = gw.GWDALI(Detection_Dict = params, 
+                    FreeParams = FreeParams, 
+                    detectors = [det0,det1,det2,det3], # Einstein Telescope + Cosmic Explorer, 
+                    approximant = 'TaylorF2_py',
+                    fmin  = 1., 
+                    fmax  = 1.e4, 
+                    fsize = 3000, 
+                    dali_method    = 'Doublet',
+                    sampler_method = 'nestle', # Same as Bilby sampling method
+                    npoints      = 300, # points for "nested sampling" or steps/walkers for "MCMC"
+                    rcond        = 1.e-4,
+                    new_priors   = None, # If you want to change the standard priors
+                    save_samples = False, 
+                    save_cov     = False, 
+                    save_fisher  = False,
+                    plot_corner  = False,
+                    hide_info    = False,
+                    step_size    = 1.e-6, # dx := max( step_size , step_size*abs(x) )
+                    diff_order   = 2, # Numerical Derivative (Finite Difference) precision O(2) or O(4)
+                    run_sampler  = True, # If you want to run MCMC.
+                    index        = 1)
 
     Samples = res['Samples']
     Fisher  = res['Fisher']
     CovFish = res['CovFisher']
     Cov     = res['Covariance']
     Rec     = res['Recovery']
     Err     = res['Error']
     SNR     = res['SNR']
+    Tensors = res['Tensors']
 
 ## References
 
 [1] L. S. Finn and D. F. Chernoff, “Observing binary inspiral in gravitational radiation: One interferometer,” Phys. Rev. D, vol. 47, pp. 2198–2219, 1993.
 
 [2] E. Sellentin, M. Quartin, and L. Amendola, “Breaking the spell of gaussianity: forecasting with higher order fisher matrices,” Monthly Notices of the Royal Astronomical Society, vol. 441, no. 2, pp. 1831–1840, 2014.
```

### Comparing `gwdali-0.1.3/gwdali.egg-info/SOURCES.txt` & `gwdali-0.1.4/gwdali.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdali-0.1.3/setup.py` & `gwdali-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md",'r') as arq:
 	readme = arq.read()
 
 setup(
 	name = 'gwdali',
-	version = '0.1.3',
+	version = '0.1.4',
 	license = 'BSD 3-Clause License',
 	author  = 'Josiel Mendonça Soares de Souza',
 	long_description = readme,
 	long_description_content_type = "text/markdown",
 	author_email = 'josiel.jms7@gmail.com',
 	keywords = 'fisher matrix, gravitational waves, gw, dali',
 	description = 'A Fisher-Based Software for Parameter Estimation from Gravitational Waves',
```

