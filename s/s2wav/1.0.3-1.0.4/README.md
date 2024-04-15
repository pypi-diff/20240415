# Comparing `tmp/s2wav-1.0.3.tar.gz` & `tmp/s2wav-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2wav-1.0.3.tar", last modified: Sat Apr 13 08:12:19 2024, max compression
+gzip compressed data, was "s2wav-1.0.4.tar", last modified: Mon Apr 15 11:26:23 2024, max compression
```

## Comparing `s2wav-1.0.3.tar` & `s2wav-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.048276 s2wav-1.0.3/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1078 2023-02-16 11:48:15.000000 s2wav-1.0.3/LICENCE.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-13 08:12:19.048043 s2wav-1.0.3/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)     9936 2024-04-13 08:09:50.000000 s2wav-1.0.3/README.md
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.045654 s2wav-1.0.3/s2wav/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      778 2024-04-09 14:10:43.000000 s2wav-1.0.3/s2wav/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    24417 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/filters.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    21732 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/samples.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.046963 s2wav-1.0.3/s2wav/transforms/
--rw-r--r--   0 cosmomatt   (503) staff       (20)      137 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/transforms/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    15960 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/transforms/base.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4599 2024-04-09 13:46:46.000000 s2wav-1.0.3/s2wav/transforms/construct.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    14965 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/transforms/wavelet.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11850 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/transforms/wavelet_precompute.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    11129 2024-04-13 08:09:50.000000 s2wav-1.0.3/s2wav/transforms/wavelet_precompute_torch.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.047786 s2wav-1.0.3/s2wav.egg-info/
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/PKG-INFO
--rw-r--r--   0 cosmomatt   (503) staff       (20)      555 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/SOURCES.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/dependency_links.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       46 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/requires.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       12 2024-04-13 08:12:19.000000 s2wav-1.0.3/s2wav.egg-info/top_level.txt
--rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-13 08:12:19.048315 s2wav-1.0.3/setup.cfg
--rw-r--r--   0 cosmomatt   (503) staff       (20)     1145 2024-04-13 08:11:03.000000 s2wav-1.0.3/setup.py
-drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-13 08:12:19.047621 s2wav-1.0.3/tests/
--rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-01-19 15:54:18.000000 s2wav-1.0.3/tests/__init__.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4073 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/conftest.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4822 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_filters.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     4813 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_gradients.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)    10154 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_wavelets.py
--rw-r--r--   0 cosmomatt   (503) staff       (20)     6260 2024-04-09 13:46:46.000000 s2wav-1.0.3/tests/test_wavelets_base.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 11:26:23.737721 s2wav-1.0.4/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1078 2023-02-16 11:48:15.000000 s2wav-1.0.4/LICENCE.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-15 11:26:23.737430 s2wav-1.0.4/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9936 2024-04-13 08:09:50.000000 s2wav-1.0.4/README.md
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 11:26:23.734055 s2wav-1.0.4/s2wav/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      989 2024-04-15 11:25:20.000000 s2wav-1.0.4/s2wav/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    24417 2024-04-09 13:46:46.000000 s2wav-1.0.4/s2wav/filters.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    21732 2024-04-13 08:09:50.000000 s2wav-1.0.4/s2wav/samples.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 11:26:23.736048 s2wav-1.0.4/s2wav/transforms/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      161 2024-04-15 11:25:20.000000 s2wav-1.0.4/s2wav/transforms/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    15960 2024-04-09 13:46:46.000000 s2wav-1.0.4/s2wav/transforms/base.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4599 2024-04-09 13:46:46.000000 s2wav-1.0.4/s2wav/transforms/construct.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11217 2024-04-15 11:25:20.000000 s2wav-1.0.4/s2wav/transforms/wavelet.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    10254 2024-04-15 11:25:20.000000 s2wav-1.0.4/s2wav/transforms/wavelet_c.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11858 2024-04-15 11:25:20.000000 s2wav-1.0.4/s2wav/transforms/wavelet_precompute.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)    11129 2024-04-13 08:09:50.000000 s2wav-1.0.4/s2wav/transforms/wavelet_precompute_torch.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 11:26:23.736905 s2wav-1.0.4/s2wav.egg-info/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4464 2024-04-15 11:26:23.000000 s2wav-1.0.4/s2wav.egg-info/PKG-INFO
+-rw-r--r--   0 cosmomatt   (503) staff       (20)      585 2024-04-15 11:26:23.000000 s2wav-1.0.4/s2wav.egg-info/SOURCES.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        1 2024-04-15 11:26:23.000000 s2wav-1.0.4/s2wav.egg-info/dependency_links.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       46 2024-04-15 11:26:23.000000 s2wav-1.0.4/s2wav.egg-info/requires.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       12 2024-04-15 11:26:23.000000 s2wav-1.0.4/s2wav.egg-info/top_level.txt
+-rw-r--r--   0 cosmomatt   (503) staff       (20)       38 2024-04-15 11:26:23.737762 s2wav-1.0.4/setup.cfg
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     1145 2024-04-15 11:25:20.000000 s2wav-1.0.4/setup.py
+drwxr-xr-x   0 cosmomatt   (503) staff       (20)        0 2024-04-15 11:26:23.736737 s2wav-1.0.4/tests/
+-rw-r--r--   0 cosmomatt   (503) staff       (20)        0 2023-01-19 15:54:18.000000 s2wav-1.0.4/tests/__init__.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4073 2024-04-09 13:46:46.000000 s2wav-1.0.4/tests/conftest.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4822 2024-04-09 13:46:46.000000 s2wav-1.0.4/tests/test_filters.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     4597 2024-04-15 11:25:20.000000 s2wav-1.0.4/tests/test_gradients.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     9529 2024-04-15 11:25:20.000000 s2wav-1.0.4/tests/test_wavelets.py
+-rw-r--r--   0 cosmomatt   (503) staff       (20)     6260 2024-04-09 13:46:46.000000 s2wav-1.0.4/tests/test_wavelets_base.py
```

### Comparing `s2wav-1.0.3/LICENCE.txt` & `s2wav-1.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/PKG-INFO` & `s2wav-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2wav
-Version: 1.0.3
+Version: 1.0.4
 Summary: Differentiable and accelerated wavelet transforms with JAX
 Home-page: https://github.com/astro-informatics/s2wav
 Author: Authors & Contributors
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE.txt
 Requires-Dist: numpy
 Requires-Dist: colorlog
 Requires-Dist: pyyaml==6.0
 Requires-Dist: scipy
-Requires-Dist: s2fft>=1.1.0
+Requires-Dist: s2fft>=1.1.1
 
 .. image:: https://github.com/astro-informatics/s2wav/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/astro-informatics/s2wav/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/astro-informatics/s2wav/branch/main/graph/badge.svg?token=ZES6J4K3KZ
     :target: https://codecov.io/gh/astro-informatics/s2wav
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
     :target: https://opensource.org/licenses/MIT
```

### Comparing `s2wav-1.0.3/README.md` & `s2wav-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/s2wav/__init__.py` & `s2wav-1.0.4/s2wav/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 from . import transforms
 
 # ~~ Aliases ~~
 
 # JAX recursive transforms
 from .transforms.wavelet import analysis, synthesis, flm_to_analysis
 
+# C Backend transforms
+from .transforms.wavelet_c import analysis as analysis_c
+from .transforms.wavelet_c import synthesis as synthesis_c
+from .transforms.wavelet_c import flm_to_analysis as flm_to_analysis_c
+
 # Base transforms
 from .transforms.base import analysis as analysis_base
 from .transforms.base import synthesis as synthesis_base
 
 # JAX precompute transforms
 from .transforms.wavelet_precompute import analysis as analysis_precomp_jax
 from .transforms.wavelet_precompute import synthesis as synthesis_precomp_jax
```

### Comparing `s2wav-1.0.3/s2wav/filters.py` & `s2wav-1.0.4/s2wav/filters.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/s2wav/samples.py` & `s2wav-1.0.4/s2wav/samples.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/s2wav/transforms/base.py` & `s2wav-1.0.4/s2wav/transforms/base.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/s2wav/transforms/construct.py` & `s2wav-1.0.4/s2wav/transforms/construct.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/s2wav/transforms/wavelet_precompute.py` & `s2wav-1.0.4/s2wav/transforms/wavelet_precompute.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,30 +162,28 @@
             with shape :math:`[n_{\theta}, n_{\phi}]`.
     """
     if precomps == None:
         raise ValueError("Must provide precomputed kernels for this transform!")
 
     J = samples.j_max(L, lam)
     Ls = samples.scal_bandlimit(L, J_min, lam, True)
-
-    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
-    f_wav = samples.construct_f_jax(L, J_min, J, lam)
-
     wav_lm = jnp.einsum(
         "jln, l->jln",
         jnp.conj(filters[0]),
         8 * jnp.pi**2 / (2 * jnp.arange(L) + 1),
         optimize=True,
     )
 
     flm = spherical.forward_transform_jax(
         f, precomps[0], L, sampling, reality, spin, nside
     )
     # Project all wigner coefficients for each lmn onto wavelet coefficients
     # Note that almost the entire compute is concentrated at the highest J
+    f_wav = []
+    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
     for j in range(J_min, J + 1):
         Lj, Nj, L0j = samples.LN_j(L, j, N, lam, True)
         f_wav_lmn[j - J_min] = (
             f_wav_lmn[j - J_min]
             .at[::2, L0j:]
             .add(
                 jnp.einsum(
@@ -193,22 +191,24 @@
                     flm[L0j:Lj, L - Lj : L - 1 + Lj],
                     wav_lm[j, L0j:Lj, L - Nj : L - 1 + Nj : 2],
                     optimize=True,
                 )
             )
         )
         shift = 0 if j < J else -1
-        f_wav[j - J_min] = wigner.inverse_transform_jax(
-            f_wav_lmn[j - J_min],
-            precomps[2][j - J_min + shift],
-            Lj,
-            Nj,
-            sampling,
-            reality,
-            nside,
+        f_wav.append(
+            wigner.inverse_transform_jax(
+                f_wav_lmn[j - J_min],
+                precomps[2][j - J_min + shift],
+                Lj,
+                Nj,
+                sampling,
+                reality,
+                nside,
+            )
         )
 
     # Project all harmonic coefficients for each lm onto scaling coefficients
     phi = filters[1][:Ls] * jnp.sqrt(4 * jnp.pi / (2 * jnp.arange(Ls) + 1))
     temp = jnp.einsum("lm,l->lm", flm[:Ls, L - Ls : L - 1 + Ls], phi, optimize=True)
     # Handle edge case
     if Ls == 1:
@@ -259,42 +259,40 @@
         reality (bool, optional): Whether :math:`f \in \mathbb{R}`, if True exploits
             conjugate symmetry of harmonic coefficients. Defaults to False.
 
         filters (Tuple[jnp.ndarray], optional): Precomputed wavelet filters. Defaults to None.
 
         precomps (List[jnp.ndarray]): Precomputed list of recursion coefficients. At most
             of length :math:`L^2`, which is a minimal memory overhead.
-        
+
         _precomp_shift (bool, optional): Whether or not the duplicated highest wavelet scale
             precomputes are provided or not.
 
     Returns:
         f_wav (jnp.ndarray): Array of wavelet pixel-space coefficients
             with shape :math:`[n_{J}, 2N-1, n_{\theta}, n_{\phi}]`.
 
         f_scal (jnp.ndarray): Array of scaling pixel-space coefficients
             with shape :math:`[n_{\theta}, n_{\phi}]`.
     """
     if precomps == None:
         raise ValueError("Must provide precomputed kernels for this transform!")
 
     J = J_max if J_max is not None else samples.j_max(L, lam)
-
-    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
-    f_wav = samples.construct_f_jax(L, J_min, J, lam)
-
     wav_lm = jnp.einsum(
         "jln, l->jln",
         jnp.conj(filters),
         8 * jnp.pi**2 / (2 * jnp.arange(L) + 1),
         optimize=True,
     )
 
     # Project all wigner coefficients for each lmn onto wavelet coefficients
     # Note that almost the entire compute is concentrated at the highest J
+    f_wav = []
+    f_wav_lmn = samples.construct_flmn_jax(L, N, J_min, J, lam, True)
     for j in range(J_min, J + 1):
         Lj, Nj, L0j = samples.LN_j(L, j, N, lam, True)
         f_wav_lmn[j - J_min] = (
             f_wav_lmn[j - J_min]
             .at[::2, L0j:]
             .add(
                 jnp.einsum(
@@ -304,17 +302,19 @@
                     optimize=True,
                 )
             )
         )
         shift = 0 if j < J else -1
         shift = shift if _precomp_shift else 0
 
-        f_wav[j - J_min] = wigner.inverse_transform_jax(
-            f_wav_lmn[j - J_min],
-            precomps[2][j - J_min + shift],
-            Lj,
-            Nj,
-            sampling,
-            reality,
-            nside,
+        f_wav.append(
+            wigner.inverse_transform_jax(
+                f_wav_lmn[j - J_min],
+                precomps[2][j - J_min + shift],
+                Lj,
+                Nj,
+                sampling,
+                reality,
+                nside,
+            )
         )
     return f_wav
```

### Comparing `s2wav-1.0.3/s2wav/transforms/wavelet_precompute_torch.py` & `s2wav-1.0.4/s2wav/transforms/wavelet_precompute_torch.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/s2wav.egg-info/PKG-INFO` & `s2wav-1.0.4/s2wav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s2wav
-Version: 1.0.3
+Version: 1.0.4
 Summary: Differentiable and accelerated wavelet transforms with JAX
 Home-page: https://github.com/astro-informatics/s2wav
 Author: Authors & Contributors
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENCE.txt
 Requires-Dist: numpy
 Requires-Dist: colorlog
 Requires-Dist: pyyaml==6.0
 Requires-Dist: scipy
-Requires-Dist: s2fft>=1.1.0
+Requires-Dist: s2fft>=1.1.1
 
 .. image:: https://github.com/astro-informatics/s2wav/actions/workflows/tests.yml/badge.svg?branch=main
     :target: https://github.com/astro-informatics/s2wav/actions/workflows/tests.yml
 .. image:: https://codecov.io/gh/astro-informatics/s2wav/branch/main/graph/badge.svg?token=ZES6J4K3KZ
     :target: https://codecov.io/gh/astro-informatics/s2wav
 .. image:: https://img.shields.io/badge/License-MIT-yellow.svg
     :target: https://opensource.org/licenses/MIT
```

### Comparing `s2wav-1.0.3/s2wav.egg-info/SOURCES.txt` & `s2wav-1.0.4/s2wav.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 s2wav.egg-info/dependency_links.txt
 s2wav.egg-info/requires.txt
 s2wav.egg-info/top_level.txt
 s2wav/transforms/__init__.py
 s2wav/transforms/base.py
 s2wav/transforms/construct.py
 s2wav/transforms/wavelet.py
+s2wav/transforms/wavelet_c.py
 s2wav/transforms/wavelet_precompute.py
 s2wav/transforms/wavelet_precompute_torch.py
 tests/__init__.py
 tests/conftest.py
 tests/test_filters.py
 tests/test_gradients.py
 tests/test_wavelets.py
```

### Comparing `s2wav-1.0.3/setup.py` & `s2wav-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     name="s2wav",
-    version="1.0.3",
+    version="1.0.4",
     url="https://github.com/astro-informatics/s2wav",
     author="Authors & Contributors",
     license="GNU General Public License v3 (GPLv3)",
     python_requires=">=3.8",
     install_requires=requirements,
     description=("Differentiable and accelerated wavelet transforms with JAX"),
     long_description_content_type="text/x-rst",
```

### Comparing `s2wav-1.0.3/tests/conftest.py` & `s2wav-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/tests/test_filters.py` & `s2wav-1.0.4/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `s2wav-1.0.3/tests/test_gradients.py` & `s2wav-1.0.4/tests/test_gradients.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,39 @@
 import jax
 
 jax.config.update("jax_enable_x64", True)
 import pytest
 import jax.numpy as jnp
 from jax.test_util import check_grads
 import s2fft
-from s2wav.transforms import wavelet, wavelet_precompute, construct
+from s2wav.transforms import wavelet, wavelet_c, wavelet_precompute, construct
 from s2wav import filters, samples
 
 L_to_test = [8]
 N_to_test = [3]
 J_min_to_test = [2]
 reality = [False, True]
 recursive_transform = [False, True]
 using_c_backend = [False, True]
-_ssht_backends = [0, 1]
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("J_min", J_min_to_test)
 @pytest.mark.parametrize("reality", reality)
 @pytest.mark.parametrize("recursive", recursive_transform)
 @pytest.mark.parametrize("using_c_backend", using_c_backend)
-@pytest.mark.parametrize("_ssht_backend", _ssht_backends)
 def test_jax_synthesis_gradients(
     wavelet_generator,
     L: int,
     N: int,
     J_min: int,
     reality: bool,
     recursive: bool,
     using_c_backend: bool,
-    _ssht_backend: int,
 ):
     J = samples.j_max(L)
 
     # Exceptions
     if J_min >= J:
         pytest.skip("J_min larger than J which isn't a valid test case.")
     if not recursive and using_c_backend:
@@ -56,62 +53,59 @@
         if using_c_backend
         else (
             construct.generate_wigner_precomputes
             if recursive
             else construct.generate_full_precomputes
         )
     )
-    synthesis = wavelet.synthesis if recursive else wavelet_precompute.synthesis
+    synthesis = (
+        (wavelet_c.synthesis if using_c_backend else wavelet.synthesis)
+        if recursive
+        else wavelet_precompute.synthesis
+    )
 
     precomps = (
         None
         if using_c_backend
         else generator(L, N, J_min, 2, forward=True, reality=reality)
     )
 
-    args = (
-        {"use_c_backend": using_c_backend, "_ssht_backend": _ssht_backend}
-        if using_c_backend
-        else {}
-    )
+    args = {"precomps": precomps} if not using_c_backend else {}
 
     def func(f_wav, f_scal):
         f = synthesis(
             f_wav,
             f_scal,
             L,
             N,
             J_min,
             reality=reality,
             filters=filter,
-            precomps=precomps,
             **args,
         )
         return jnp.sum(jnp.abs(f) ** 2)
 
     check_grads(func, (f_wav, f_scal), order=1, modes=("rev"))
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("J_min", J_min_to_test)
 @pytest.mark.parametrize("reality", reality)
 @pytest.mark.parametrize("recursive", recursive_transform)
 @pytest.mark.parametrize("using_c_backend", using_c_backend)
-@pytest.mark.parametrize("_ssht_backend", _ssht_backends)
 def test_jax_analysis_gradients(
     flm_generator,
     wavelet_generator,
     L: int,
     N: int,
     J_min: int,
     reality: bool,
     recursive: bool,
     using_c_backend: bool,
-    _ssht_backend: int,
 ):
     J = samples.j_max(L)
     if J_min >= J:
         pytest.skip("J_min larger than J which isn't a valid test case.")
     if not recursive and using_c_backend:
         pytest.skip("Precompute transform not supported from C backend libraries.")
     if reality and using_c_backend:
@@ -133,30 +127,30 @@
         if using_c_backend
         else (
             construct.generate_wigner_precomputes
             if recursive
             else construct.generate_full_precomputes
         )
     )
-    analysis = wavelet.analysis if recursive else wavelet_precompute.analysis
+    analysis = (
+        (wavelet_c.analysis if using_c_backend else wavelet.analysis)
+        if recursive
+        else wavelet_precompute.analysis
+    )
     precomps = (
         None
         if using_c_backend
         else generator(L, N, J_min, forward=False, reality=reality)
     )
 
-    args = (
-        {"use_c_backend": using_c_backend, "_ssht_backend": _ssht_backend}
-        if using_c_backend
-        else {}
-    )
+    args = {"precomps": precomps} if not using_c_backend else {}
 
     def func(f):
         f_wav, f_scal = analysis(
-            f, L, N, J_min, reality=reality, filters=filter, precomps=precomps, **args
+            f, L, N, J_min, reality=reality, filters=filter, **args
         )
         loss = jnp.sum(jnp.abs(f_scal - f_scal_target) ** 2)
         for j in range(J - J_min):
             loss += jnp.sum(jnp.abs(f_wav[j - J_min] - f_wav_target[j - J_min]) ** 2)
         return loss
 
     check_grads(func, (f.real if reality else f,), order=1, modes=("rev"))
```

### Comparing `s2wav-1.0.3/tests/test_wavelets.py` & `s2wav-1.0.4/tests/test_wavelets.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pytest
 import numpy as np
 import torch
 import pys2let as s2let
 from s2fft import base_transforms as sht_base
 from s2wav.transforms import (
     wavelet,
+    wavelet_c,
     wavelet_precompute,
     wavelet_precompute_torch,
     construct,
 )
 from s2wav import filters, samples
 
 L_to_test = [8]
@@ -19,37 +20,34 @@
 J_min_to_test = [2]
 lam_to_test = [2, 3]
 reality = [False, True]
 sampling_to_test = ["mw", "mwss", "dh", "gl"]
 recursive_transform = [False, True]
 using_torch_frontend = [False, True]
 using_c_backend = [False, True]
-_ssht_backends = [0, 1]
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("J_min", J_min_to_test)
 @pytest.mark.parametrize("lam", lam_to_test)
 @pytest.mark.parametrize("reality", reality)
 @pytest.mark.parametrize("recursive", recursive_transform)
 @pytest.mark.parametrize("using_torch", using_torch_frontend)
 @pytest.mark.parametrize("using_c_backend", using_c_backend)
-@pytest.mark.parametrize("_ssht_backend", _ssht_backends)
 def test_synthesis(
     wavelet_generator,
     L: int,
     N: int,
     J_min: int,
     lam: int,
     reality: bool,
     recursive: bool,
     using_torch: bool,
     using_c_backend: bool,
-    _ssht_backend: int,
 ):
     J = samples.j_max(L, lam)
 
     # Exceptions
     if J_min >= J:
         pytest.skip("J_min larger than J which isn't a valid test case.")
     if recursive and using_torch:
@@ -81,46 +79,33 @@
         else (
             construct.generate_wigner_precomputes
             if recursive
             else construct.generate_full_precomputes
         )
     )
     synthesis = (
-        wavelet.synthesis
+        (wavelet_c.synthesis if using_c_backend else wavelet.synthesis)
         if recursive
         else (
             wavelet_precompute_torch.synthesis
             if using_torch
             else wavelet_precompute.synthesis
         )
     )
     precomps = (
         None
         if using_c_backend
         else generator(
             L, N, J_min, lam, forward=True, reality=reality, using_torch=using_torch
         )
     )
-    args = (
-        {"use_c_backend": using_c_backend, "_ssht_backend": _ssht_backend}
-        if using_c_backend
-        else {}
-    )
+    args = {"precomps": precomps} if not using_c_backend else {}
 
     f_check = synthesis(
-        f_wav,
-        f_scal,
-        L,
-        N,
-        J_min,
-        lam,
-        reality=reality,
-        filters=filter,
-        precomps=precomps,
-        **args,
+        f_wav, f_scal, L, N, J_min, lam, reality=reality, filters=filter, **args
     )
 
     if using_torch:
         f_check = f_check.resolve_conj().numpy()
 
     f = np.real(f) if reality else f
     np.testing.assert_allclose(f, f_check.flatten("C"), atol=1e-14)
@@ -130,27 +115,25 @@
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("J_min", J_min_to_test)
 @pytest.mark.parametrize("lam", lam_to_test)
 @pytest.mark.parametrize("reality", reality)
 @pytest.mark.parametrize("recursive", recursive_transform)
 @pytest.mark.parametrize("using_torch", using_torch_frontend)
 @pytest.mark.parametrize("using_c_backend", using_c_backend)
-@pytest.mark.parametrize("_ssht_backend", _ssht_backends)
 def test_analysis(
     flm_generator,
     f_wav_converter,
     L: int,
     N: int,
     J_min: int,
     lam: int,
     reality: bool,
     recursive: bool,
     using_torch: bool,
     using_c_backend: bool,
-    _ssht_backend: int,
 ):
     J = samples.j_max(L, lam)
 
     # Exceptions
     if J_min >= J:
         pytest.skip("J_min larger than J which isn't a valid test case.")
     if recursive and using_torch:
@@ -173,15 +156,15 @@
         else (
             construct.generate_wigner_precomputes
             if recursive
             else construct.generate_full_precomputes
         )
     )
     analysis = (
-        wavelet.analysis
+        (wavelet_c.analysis if using_c_backend else wavelet.analysis)
         if recursive
         else (
             wavelet_precompute_torch.analysis
             if using_torch
             else wavelet_precompute.analysis
         )
     )
@@ -189,29 +172,24 @@
         None
         if using_c_backend
         else generator(
             L, N, J_min, lam, forward=False, reality=reality, using_torch=using_torch
         )
     )
 
-    args = (
-        {"use_c_backend": using_c_backend, "_ssht_backend": _ssht_backend}
-        if using_c_backend
-        else {}
-    )
+    args = {"precomps": precomps} if not using_c_backend else {}
 
     f_wav_check, f_scal_check = analysis(
         torch.from_numpy(f) if using_torch else f,
         L,
         N,
         J_min,
         lam,
         reality=reality,
         filters=filter,
-        precomps=precomps,
         **args,
     )
 
     f_wav_check = f_wav_converter(f_wav_check, L, N, J_min, lam, using_torch)
 
     np.testing.assert_allclose(f_wav, f_wav_check, atol=1e-14)
     np.testing.assert_allclose(
@@ -226,90 +204,74 @@
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("J_min", J_min_to_test)
 @pytest.mark.parametrize("lam", lam_to_test)
 @pytest.mark.parametrize("reality", reality)
 @pytest.mark.parametrize("sampling", sampling_to_test)
 @pytest.mark.parametrize("using_c_backend", using_c_backend)
-@pytest.mark.parametrize("_ssht_backend", _ssht_backends)
 def test_round_trip(
     flm_generator,
     L: int,
     N: int,
     J_min: int,
     lam: int,
     reality: bool,
     sampling: str,
     using_c_backend: bool,
-    _ssht_backend: int,
 ):
     J = samples.j_max(L, lam)
 
     # Exceptions
     if J_min >= J:
         pytest.skip("J_min larger than J which isn't a valid test case.")
 
     flm = flm_generator(L=L, L_lower=0, spin=0, reality=reality)
     f = sht_base.spherical.inverse(flm, L, reality=reality, sampling=sampling)
     filter = filters.filters_directional_vectorised(L, N, J_min, lam)
 
-    args = (
-        {"use_c_backend": using_c_backend, "_ssht_backend": _ssht_backend}
-        if using_c_backend
-        else {}
-    )
+    analysis_func = wavelet_c.analysis if using_c_backend else wavelet.analysis
+    synthesis_func = wavelet_c.synthesis if using_c_backend else wavelet.synthesis
 
-    f_wav, f_scal = wavelet.analysis(
-        f,
-        L,
-        N,
-        J_min,
-        lam,
-        reality=reality,
-        sampling=sampling,
-        filters=filter,
-        **args,
+    f_wav, f_scal = analysis_func(
+        f, L, N, J_min, lam, reality=reality, sampling=sampling, filters=filter
     )
-    f_check = wavelet.synthesis(
+    f_check = synthesis_func(
         f_wav,
         f_scal,
         L,
         N,
         J_min,
         lam,
         sampling=sampling,
         reality=reality,
         filters=filter,
-        **args,
     )
 
     np.testing.assert_allclose(f, f_check, atol=1e-14)
 
 
 @pytest.mark.parametrize("L", L_to_test)
 @pytest.mark.parametrize("N", N_to_test)
 @pytest.mark.parametrize("J_min", J_min_to_test)
 @pytest.mark.parametrize("lam", lam_to_test)
 @pytest.mark.parametrize("reality", reality)
 @pytest.mark.parametrize("recursive", recursive_transform)
 @pytest.mark.parametrize("using_torch", using_torch_frontend)
 @pytest.mark.parametrize("using_c_backend", using_c_backend)
-@pytest.mark.parametrize("_ssht_backend", _ssht_backends)
 def test_flm_to_analysis(
     flm_generator,
     f_wav_converter,
     L: int,
     N: int,
     J_min: int,
     lam: int,
     reality: bool,
     recursive: bool,
     using_torch: bool,
     using_c_backend: bool,
-    _ssht_backend: int,
 ):
     J = samples.j_max(L, lam)
 
     # Exceptions
     if J_min >= J:
         pytest.skip("J_min larger than J which isn't a valid test case.")
     if recursive and using_torch:
@@ -333,15 +295,15 @@
         else (
             construct.generate_wigner_precomputes
             if recursive
             else construct.generate_full_precomputes
         )
     )
     analysis = (
-        wavelet.flm_to_analysis
+        (wavelet_c.flm_to_analysis if using_c_backend else wavelet.flm_to_analysis)
         if recursive
         else (
             wavelet_precompute_torch.flm_to_analysis
             if using_torch
             else wavelet_precompute.flm_to_analysis
         )
     )
@@ -349,29 +311,24 @@
         None
         if using_c_backend
         else generator(
             L, N, J_min, lam, forward=False, reality=reality, using_torch=using_torch
         )
     )
 
-    args = (
-        {"use_c_backend": using_c_backend, "_ssht_backend": _ssht_backend}
-        if using_c_backend
-        else {}
-    )
+    args = {"precomps": precomps} if not using_c_backend else {}
 
     f_wav_check = analysis(
         torch.from_numpy(flm) if using_torch else flm,
         L,
         N,
         J_min,
         None,
         lam,
         reality=reality,
         filters=filter,
-        precomps=precomps,
         **args,
     )
 
     f_wav_check = f_wav_converter(f_wav_check, L, N, J_min, lam, using_torch)
 
     np.testing.assert_allclose(f_wav, f_wav_check, atol=1e-14)
```

### Comparing `s2wav-1.0.3/tests/test_wavelets_base.py` & `s2wav-1.0.4/tests/test_wavelets_base.py`

 * *Files identical despite different names*

