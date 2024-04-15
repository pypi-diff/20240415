# Comparing `tmp/PyCosmoMMF-0.0.6.tar.gz` & `tmp/PyCosmoMMF-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCosmoMMF-0.0.6.tar", last modified: Fri Apr  5 21:12:50 2024, max compression
+gzip compressed data, was "PyCosmoMMF-0.0.7.tar", last modified: Mon Apr 15 15:47:20 2024, max compression
```

## Comparing `PyCosmoMMF-0.0.6.tar` & `PyCosmoMMF-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-05 21:12:50.768143 PyCosmoMMF-0.0.6/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2024-03-12 07:03:50.000000 PyCosmoMMF-0.0.6/LICENSE
--rw-r--r--   0 jamessunseri   (501) staff       (20)      109 2024-03-12 22:35:52.000000 PyCosmoMMF-0.0.6/MANIFEST.in
--rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-04-05 21:12:50.768232 PyCosmoMMF-0.0.6/PKG-INFO
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-05 21:12:50.767323 PyCosmoMMF-0.0.6/PyCosmoMMF/
--rw-r--r--   0 jamessunseri   (501) staff       (20)      346 2024-03-23 18:29:11.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/__init__.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     4245 2024-03-23 18:28:22.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/filter.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     1973 2024-03-23 18:27:34.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/hessian.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)     3660 2024-03-23 18:27:51.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/signatures.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)    13385 2024-04-05 21:09:54.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/tagging.py
--rw-r--r--   0 jamessunseri   (501) staff       (20)   131200 2024-03-12 20:43:00.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/test_density_cube.npy
--rw-r--r--   0 jamessunseri   (501) staff       (20)      661 2024-03-23 18:28:11.000000 PyCosmoMMF-0.0.6/PyCosmoMMF/utils.py
-drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-05 21:12:50.768022 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/
--rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/PKG-INFO
--rw-r--r--   0 jamessunseri   (501) staff       (20)      382 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/SOURCES.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/dependency_links.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       11 2024-04-05 21:12:50.000000 PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/top_level.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)     6546 2024-03-12 21:49:32.000000 PyCosmoMMF-0.0.6/README.md
--rw-r--r--   0 jamessunseri   (501) staff       (20)      167 2024-03-12 20:11:18.000000 PyCosmoMMF-0.0.6/pyproject.toml
--rw-r--r--   0 jamessunseri   (501) staff       (20)       42 2024-03-12 21:43:49.000000 PyCosmoMMF-0.0.6/requirements.txt
--rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2024-04-05 21:12:50.768435 PyCosmoMMF-0.0.6/setup.cfg
--rw-r--r--   0 jamessunseri   (501) staff       (20)     2188 2024-04-05 21:10:16.000000 PyCosmoMMF-0.0.6/setup.py
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-15 15:47:20.704554 PyCosmoMMF-0.0.7/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     1070 2024-03-12 07:03:50.000000 PyCosmoMMF-0.0.7/LICENSE
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      109 2024-03-12 22:35:52.000000 PyCosmoMMF-0.0.7/MANIFEST.in
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-04-15 15:47:20.704669 PyCosmoMMF-0.0.7/PKG-INFO
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-15 15:47:20.703701 PyCosmoMMF-0.0.7/PyCosmoMMF/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      346 2024-03-23 18:29:11.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/__init__.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     4401 2024-04-15 15:46:02.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/filter.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     1972 2024-04-15 15:41:35.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/hessian.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     3704 2024-04-15 15:45:00.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/signatures.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)    13385 2024-04-05 21:09:54.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/tagging.py
+-rw-r--r--   0 jamessunseri   (501) staff       (20)   131200 2024-03-12 20:43:00.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/test_density_cube.npy
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      661 2024-03-23 18:28:11.000000 PyCosmoMMF-0.0.7/PyCosmoMMF/utils.py
+drwxr-xr-x   0 jamessunseri   (501) staff       (20)        0 2024-04-15 15:47:20.704428 PyCosmoMMF-0.0.7/PyCosmoMMF.egg-info/
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     7708 2024-04-15 15:47:20.000000 PyCosmoMMF-0.0.7/PyCosmoMMF.egg-info/PKG-INFO
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      382 2024-04-15 15:47:20.000000 PyCosmoMMF-0.0.7/PyCosmoMMF.egg-info/SOURCES.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)        1 2024-04-15 15:47:20.000000 PyCosmoMMF-0.0.7/PyCosmoMMF.egg-info/dependency_links.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       11 2024-04-15 15:47:20.000000 PyCosmoMMF-0.0.7/PyCosmoMMF.egg-info/top_level.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     6546 2024-03-12 21:49:32.000000 PyCosmoMMF-0.0.7/README.md
+-rw-r--r--   0 jamessunseri   (501) staff       (20)      167 2024-03-12 20:11:18.000000 PyCosmoMMF-0.0.7/pyproject.toml
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       42 2024-03-12 21:43:49.000000 PyCosmoMMF-0.0.7/requirements.txt
+-rw-r--r--   0 jamessunseri   (501) staff       (20)       98 2024-04-15 15:47:20.705024 PyCosmoMMF-0.0.7/setup.cfg
+-rw-r--r--   0 jamessunseri   (501) staff       (20)     2188 2024-04-15 15:43:17.000000 PyCosmoMMF-0.0.7/setup.py
```

### Comparing `PyCosmoMMF-0.0.6/LICENSE` & `PyCosmoMMF-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.6/PKG-INFO` & `PyCosmoMMF-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCosmoMMF
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for detecting structures in the Cosmic Web.
 Home-page: https://github.com/James11222/PyCosmoMMF/
 Author: James Sunseri
 Author-email: js7501@princeton.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/PyCosmoMMF/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF/filter.py` & `PyCosmoMMF-0.0.7/PyCosmoMMF/filter.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     
     Returns
     -------
     kx, ky, kz : tuple
         The wavevectors in each dimension.
     """
     sample_rate = 2*np.pi * (np.array(dims) / box_size)
-    kx = np.fft.fftfreq(dims[0], 1/sample_rate[0]) * (2*np.pi / dims[0])
-    ky = np.fft.fftfreq(dims[1], 1/sample_rate[1]) * (2*np.pi / dims[1])
-    kz = np.fft.fftfreq(dims[2], 1/sample_rate[2]) * (2*np.pi / dims[2])
+    kx = (np.fft.fftfreq(dims[0], 1/sample_rate[0]) * (2*np.pi / dims[0])).astype(np.float32)
+    ky = (np.fft.fftfreq(dims[1], 1/sample_rate[1]) * (2*np.pi / dims[1])).astype(np.float32)
+    kz = (np.fft.fftfreq(dims[2], 1/sample_rate[2]) * (2*np.pi / dims[2])).astype(np.float32)
     return kx, ky, kz
 
 @jit_compiler
 def kspace_gaussian_filter(R_S, kv):
     """
     create a Gaussian filter in k-space.
 
@@ -46,15 +46,15 @@
     Returns
     -------
     filter_k : array
         The filter in k-space.
     """
     kx, ky, kz = kv
     nx, ny, nz = len(kx), len(ky), len(kz)
-    filter_k = np.zeros((nx, ny, nz))
+    filter_k = np.zeros((nx, ny, nz), dtype=np.float32)
     for ix in nb.prange(nx):
         for iy in range(ny):
             for iz in range(nz):
                 filter_k[ix, iy, iz] = np.exp(
                     -(kx[ix]**2 + ky[iy]**2 + kz[iz]**2) * R_S**2 / 2)
     return filter_k
 
@@ -74,15 +74,15 @@
     -------
     filter_k : array
         The filter in k-space.
     """
 
     kx, ky, kz = kv
     nx, ny, nz = len(kx), len(ky), len(kz)
-    filter_k = np.zeros((nx, ny, nz))
+    filter_k = np.zeros((nx, ny, nz), dtype=np.float32)
 
     for ix in nb.prange(nx):
         for iy in range(ny):
             for iz in range(nz):
                 k = np.sqrt(kx[ix]**2 + ky[iy]**2 + kz[iz]**2)
                 if k == 0.0:
                     filter_k[ix, iy, iz] = 1.0
@@ -108,15 +108,15 @@
     -------
     f_Rn : array
         The smoothed field.
     """
     GF = kspace_top_hat_filter(R_S, kv)
     f_Rn = np.real(np.fft.ifftn(GF * np.fft.fftn(f)))
     f_Rn = f_Rn * (np.sum(f) / np.sum(f_Rn))
-    return f_Rn
+    return f_Rn.astype(np.float32)
 
 def smooth_gauss(f, R_S, kv):
     """
     apply a Gaussian filter to a field f.
 
     Parameters
     ----------
@@ -131,15 +131,15 @@
     -------
     f_Rn : array
         The smoothed field.
     """
     GF = kspace_gaussian_filter(R_S, kv)
     f_Rn = np.real(np.fft.ifftn(GF * np.fft.fftn(f)))
     f_Rn = f_Rn * (np.sum(f) / np.sum(f_Rn))
-    return f_Rn
+    return f_Rn.astype(np.float32)
 
 
 def smooth_loggauss(f, R_S, kv):
     """
     apply a Gaussian filter to the log of a field f.
 
     Parameters
@@ -174,9 +174,9 @@
     # Convert back to linear scale
     f_result = 10 ** np.real(f_ifft)
 
     # Normalize the result
     norm = np.sum(f) / np.sum(f_result)
     f_result *= norm
 
-    return f_result
+    return f_result.astype(np.float32)
```

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF/hessian.py` & `PyCosmoMMF-0.0.7/PyCosmoMMF/hessian.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     -------
     hessian : 3D array
         The hessian matrix.
     """
 
     f_Rn_hat = np.fft.fftn(f_Rn)
     dims = f_Rn_hat.shape
-    hessian = np.zeros((dims[0], dims[1], dims[2], 6), dtype=np.complex128)
+    hessian = np.zeros((dims[0], dims[1], dims[2], 6), dtype=np.complex64)
     kx, ky, kz = kv[0], kv[1], kv[2]
 
     @jit_compiler
     def perform_loop(hessian):
         """
         This function is a loop that calculates the hessian matrix
         for each point in the 3D array.
```

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF/signatures.py` & `PyCosmoMMF-0.0.7/PyCosmoMMF/signatures.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     Returns
     -------
     sigs : 4D array
         The signatures.
     """
     
     hsize = hessian.shape[:3]
-    sigs = np.zeros((hsize[0], hsize[1], hsize[2], 3))
+    sigs = np.zeros((hsize[0], hsize[1], hsize[2], 3), dtype=np.float32)
 
     #helper functions
     def θ(x):
         """
         Heaviside step function. Returns one if the argument is positive, zero otherwise.
         """
         if x > 0:
@@ -91,23 +91,24 @@
     sigmax : 4D array
         The maximum signatures.
     """
     if alg not in ['NEXUS', 'NEXUSPLUS']:
         raise ValueError("alg must be either 'NEXUS' or 'NEXUSPLUS'")
     
     nx, ny, nz = field.shape
+    eps = 1e-5
     
     # Make sure the field has no 0 values
-    field = field + 0.0001
+    field = field + eps
     
     # Calculate wave vectors for our field
     wave_vecs = wavevectors3D((nx, ny, nz))
     
     # Calculate signatures at each scale Rn, determine max
-    sigmax = np.ones((nx, ny, nz, 3)) * 0.00001
+    sigmax = np.ones((nx, ny, nz, 3), dtype=np.float32) * eps
 
     @jit_compiler
     def perform_loop(sigmax, sigs_Rn, nx, ny, nz):
         for ix in nb.prange(nx):
             for iy in range(ny):
                 for iz in range(nz):
                     for sigtype in range(3):
```

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF/tagging.py` & `PyCosmoMMF-0.0.7/PyCosmoMMF/tagging.py`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF/test_density_cube.npy` & `PyCosmoMMF-0.0.7/PyCosmoMMF/test_density_cube.npy`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF/utils.py` & `PyCosmoMMF-0.0.7/PyCosmoMMF/utils.py`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.6/PyCosmoMMF.egg-info/PKG-INFO` & `PyCosmoMMF-0.0.7/PyCosmoMMF.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCosmoMMF
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for detecting structures in the Cosmic Web.
 Home-page: https://github.com/James11222/PyCosmoMMF/
 Author: James Sunseri
 Author-email: js7501@princeton.edu
 License: MIT
 Project-URL: Bug Reports, https://github.com/James11222/PyCosmoMMF/issues
 Project-URL: Funding, https://donate.pypi.org
```

### Comparing `PyCosmoMMF-0.0.6/README.md` & `PyCosmoMMF-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `PyCosmoMMF-0.0.6/setup.py` & `PyCosmoMMF-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from setuptools import setup
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name='PyCosmoMMF',  # Required
-    version='0.0.6',  # Required
+    version='0.0.7',  # Required
     description='A package for detecting structures in the Cosmic Web.',  # Optional
     long_description=(here / 'README.md').read_text(encoding='utf-8'),  # Optional
     long_description_content_type='text/markdown',  # Optional (see note above)
     url='https://github.com/James11222/PyCosmoMMF/',  # Optional
 
     author='James Sunseri',  # Optional
```

