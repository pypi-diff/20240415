# Comparing `tmp/sparse-ir-1.1.0.tar.gz` & `tmp/sparse-ir-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparse-ir-1.1.0.tar", last modified: Sun Mar 24 08:12:22 2024, max compression
+gzip compressed data, was "sparse-ir-1.1.1.tar", last modified: Mon Apr 15 08:00:15 2024, max compression
```

## Comparing `sparse-ir-1.1.0.tar` & `sparse-ir-1.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:12:22.569729 sparse-ir-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-24 08:12:22.569729 sparse-ir-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 08:12:22.569729 sparse-ir-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:12:22.565729 sparse-ir-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:12:22.569729 sparse-ir-1.1.0/src/sparse_ir/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/_roots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/augment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12833 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/basis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/dlr.py
--rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/poly.py
--rw-r--r--   0 runner    (1001) docker     (127)    13801 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/svd.py
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/src/sparse_ir/sve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:12:22.569729 sparse-ir-1.1.0/src/sparse_ir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-03-24 08:12:22.000000 sparse-ir-1.1.0/src/sparse_ir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-24 08:12:22.000000 sparse-ir-1.1.0/src/sparse_ir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 08:12:22.000000 sparse-ir-1.1.0/src/sparse_ir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-24 08:12:22.000000 sparse-ir-1.1.0/src/sparse_ir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-24 08:12:22.000000 sparse-ir-1.1.0/src/sparse_ir.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 08:12:22.569729 sparse-ir-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_basis_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_dlr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_poly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_scipost_sample_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_sve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-24 08:12:21.000000 sparse-ir-1.1.0/test/test_whitespace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:00:15.711616 sparse-ir-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-15 08:00:15.711616 sparse-ir-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 08:00:15.711616 sparse-ir-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:00:15.707616 sparse-ir-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:00:15.711616 sparse-ir-1.1.1/src/sparse_ir/
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/_roots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8351 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13316 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/basis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/dlr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18487 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18359 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13879 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/svd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir/sve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:00:15.711616 sparse-ir-1.1.1/src/sparse_ir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/src/sparse_ir.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 08:00:15.711616 sparse-ir-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_dlr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_poly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_scipost_sample_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_sve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-15 08:00:15.000000 sparse-ir-1.1.1/test/test_whitespace.py
```

### Comparing `sparse-ir-1.1.0/LICENSE.txt` & `sparse-ir-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/PKG-INFO` & `sparse-ir-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-ir
-Version: 1.1.0
+Version: 1.1.1
 Summary: intermediate representation (IR) basis for electronic propagator
 Home-page: https://github.com/SpM-lab/sparse-ir
 Author: ['Markus Wallerberger', 'Hiroshi Shinaoka', 'Kazuyoshi Yoshimi', 'Junya Otsuki', 'Chikano Naoya']
 Author-email: markus.wallerberger@tuwien.ac.at
 License: UNKNOWN
 Keywords: irbasis many-body propagator svd
 Platform: UNKNOWN
```

### Comparing `sparse-ir-1.1.0/README.rst` & `sparse-ir-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/setup.py` & `sparse-ir-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/__init__.py` & `sparse-ir-1.1.1/src/sparse_ir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,14 @@
 
  - on-the-fly computation of basis functions for arbitrary cutoff Λ
  - basis functions and singular values are accurate to full precision
  - routines for sparse sampling
 """
 __copyright__ = "2020-2024 Markus Wallerberger, Hiroshi Shinaoka, and others"
 __license__ = "MIT"
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 from .kernel import RegularizedBoseKernel, LogisticKernel
 from .sve import compute as compute_sve, SVEResult
 from .basis import FiniteTempBasis, finite_temp_bases
 from .basis_set import FiniteTempBasisSet
 from .sampling import TauSampling, MatsubaraSampling
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir/_gauss.py` & `sparse-ir-1.1.1/src/sparse_ir/_gauss.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/_roots.py` & `sparse-ir-1.1.1/src/sparse_ir/_roots.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/_util.py` & `sparse-ir-1.1.1/src/sparse_ir/_util.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/abstract.py` & `sparse-ir-1.1.1/src/sparse_ir/abstract.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,22 +146,34 @@
         raise NotImplementedError()
 
     @property
     def wmax(self):
         """Real frequency cutoff or `None` if not present"""
         raise NotImplementedError()
 
-    def default_tau_sampling_points(self):
-        """Default sampling points on the imaginary time axis"""
+    def default_tau_sampling_points(self, *, npoints=None):
+        """Default sampling points on the imaginary time axis
+
+        Arguments:
+            npoints (int):
+                Minimum number of sampling points to return.
+
+                .. versionadded: 1.1
+        """
         raise NotImplementedError()
 
-    def default_matsubara_sampling_points(self, *, positive_only=False):
+    def default_matsubara_sampling_points(self, *, npoints=None,
+                                          positive_only=False):
         """Default sampling points on the imaginary frequency axis
 
         Arguments:
+            npoints (int):
+                Minimum number of sampling points to return.
+
+                .. versionadded: 1.1
             positive_only (bool):
                 Only return non-negative frequencies.  This is useful if the
                 object to be fitted is symmetric in Matsubura frequency,
                 ``ghat(w) == ghat(-w).conj()``, or, equivalently, real in
                 imaginary time.
         """
         raise NotImplementedError()
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir/adapter.py` & `sparse-ir-1.1.1/src/sparse_ir/adapter.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/augment.py` & `sparse-ir-1.1.1/src/sparse_ir/augment.py`

 * *Files 3% similar despite different names*

```diff
@@ -102,21 +102,29 @@
     def beta(self):
         return self._basis.beta
 
     @property
     def wmax(self):
         return self._basis.wmax
 
-    def default_tau_sampling_points(self):
-        x = basis._default_sampling_points(self._basis.sve_result.u, self.size)
-        return self.beta/2 * (x + 1)
+    def default_tau_sampling_points(self, *, npoints=None):
+        if npoints is None:
+            npoints = self.size
 
-    def default_matsubara_sampling_points(self, *, positive_only=False):
-        return basis._default_matsubara_sampling_points(
-                    self._basis._uhat_full, self.size, positive_only=positive_only)
+        # Return the sampling points of the underlying basis, but since we
+        # use the size of self, we add two further points.  One then has to
+        # hope that these give good sampling points.
+        return self._basis.default_tau_sampling_points(npoints=npoints)
+
+    def default_matsubara_sampling_points(self, *, npoints=None,
+                                          positive_only=False):
+        if npoints is None:
+            npoints = self.size
+        return self._basis.default_matsubara_sampling_points(
+                                npoints=npoints, positive_only=positive_only)
 
     @property
     def is_well_conditioned(self):
         wbasis = self._basis.is_well_conditioned
         waug = (len(self._augmentations) == 1
                 and isinstance(self._augmentations[0], MatsubaraConst))
         return wbasis and waug
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir/basis.py` & `sparse-ir-1.1.1/src/sparse_ir/basis.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,24 +165,39 @@
         """Kernel of which this is the singular value expansion"""
         return self._kernel
 
     @property
     def sve_result(self):
         return self._sve_result
 
-    def default_tau_sampling_points(self):
-        x = _default_sampling_points(self._sve_result.u, self.size)
+    def default_tau_sampling_points(self, *, npoints=None):
+        if npoints is None:
+            npoints = self.size
+        x = _default_sampling_points(self._sve_result.u, npoints)
         return self._beta/2 * (x + 1)
 
-    def default_matsubara_sampling_points(self, *, positive_only=False):
-        return _default_matsubara_sampling_points(self._uhat_full, self.size,
+    def default_matsubara_sampling_points(self, *, npoints=None,
+                                          positive_only=False):
+        if npoints is None:
+            npoints = self.size
+        return _default_matsubara_sampling_points(self._uhat_full, npoints,
                                                   positive_only=positive_only)
 
-    def default_omega_sampling_points(self):
-        y = _default_sampling_points(self._sve_result.v, self.size)
+    def default_omega_sampling_points(self, *, npoints=None):
+        """Return default sampling points in imaginary time.
+
+        Arguments:
+            npoints (int):
+                Minimum number of sampling points to return.
+
+                .. versionadded: 1.1
+        """
+        if npoints is None:
+            npoints = self.size
+        y = _default_sampling_points(self._sve_result.v, npoints)
         return self._wmax * y
 
     def rescale(self, new_beta):
         """Return a basis for different temperature.
 
         Uses the same kernel with the same ``eps``, but a different
         temperature.  Note that this implies a different UV cutoff ``wmax``,
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir/basis_set.py` & `sparse-ir-1.1.1/src/sparse_ir/basis_set.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/dlr.py` & `sparse-ir-1.1.1/src/sparse_ir/dlr.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/kernel.py` & `sparse-ir-1.1.1/src/sparse_ir/kernel.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/poly.py` & `sparse-ir-1.1.1/src/sparse_ir/poly.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             phat(n) == ∫ dx exp(1j * pi * n * x / (xmax - xmin)) p(x)
 
     The polynomial is continued either periodically (``freq='even'``), in which
     case ``n`` must be even, or antiperiodically (``freq='odd'``), in which case
     ``n`` must be odd.
     """
     _DEFAULT_GRID = np.hstack([np.arange(2**6),
-                        (2**np.linspace(6, 25, 16*(25-6)+1)).astype(int)])
+                        (2**np.linspace(6, 35, 16*(35-6)+1)).astype(int)])
 
     def __init__(self, poly, freq='even', n_asymp=None, power_model=None):
         if poly.xmin != -1 or poly.xmax != 1:
             raise NotImplementedError("Only interval [-1, 1] supported")
         self.poly = poly
         self.freq = freq
         self.zeta = {'any': None, 'even': 0, 'odd': 1}[freq]
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir/sampling.py` & `sparse-ir-1.1.1/src/sparse_ir/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
                 Axis or dimension of `al` along which to evaluate the function.
                 Defaults to the last, i.e., rightmost axis.
             points (vector):
                 Points on which the results should be evaluated.  Defaults
                 to the sampling points for which the sampling objects was
                 created.
 
+                .. versionadded:: 1.1
+
         Return:
             Array where the `n`-th item along `axis` corresponds to the
             value on the `n`-th sampling point (or value on `point[n]`, if
             given.)
 
         Note:
             If `points` is given, a new sampling is created at each invocation,
@@ -62,14 +64,16 @@
             axis (integer):
                 Axis or dimension of `ax` along which to fit the function.
                 Defaults to the last, i.e., rightmost axis.
             points (vector):
                 Points on which the `ax` is given.  Defaults to the sampling
                 points for which the sampling objects was created.
 
+                .. versionadded:: 1.1
+
         Return:
             Array where the `l`-th item along `axis` corresponds to the
             `l`-th basis coefficient
 
         Note:
             If `points` is given, a new sampling is created at each invocation,
             which can result in a performance hit.  Consider caching sampling
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir/svd.py` & `sparse-ir-1.1.1/src/sparse_ir/svd.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir/sve.py` & `sparse-ir-1.1.1/src/sparse_ir/sve.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/src/sparse_ir.egg-info/PKG-INFO` & `sparse-ir-1.1.1/src/sparse_ir.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparse-ir
-Version: 1.1.0
+Version: 1.1.1
 Summary: intermediate representation (IR) basis for electronic propagator
 Home-page: https://github.com/SpM-lab/sparse-ir
 Author: ['Markus Wallerberger', 'Hiroshi Shinaoka', 'Kazuyoshi Yoshimi', 'Junya Otsuki', 'Chikano Naoya']
 Author-email: markus.wallerberger@tuwien.ac.at
 License: UNKNOWN
 Keywords: irbasis many-body propagator svd
 Platform: UNKNOWN
```

### Comparing `sparse-ir-1.1.0/src/sparse_ir.egg-info/SOURCES.txt` & `sparse-ir-1.1.1/src/sparse_ir.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_augment.py` & `sparse-ir-1.1.1/test/test_augment.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_basis_set.py` & `sparse-ir-1.1.1/test/test_basis_set.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_compare.py` & `sparse-ir-1.1.1/test/test_compare.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_dlr.py` & `sparse-ir-1.1.1/test/test_dlr.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_gauss.py` & `sparse-ir-1.1.1/test/test_gauss.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_kernel.py` & `sparse-ir-1.1.1/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_poly.py` & `sparse-ir-1.1.1/test/test_poly.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_sampling.py` & `sparse-ir-1.1.1/test/test_sampling.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_scipost_sample_code.py` & `sparse-ir-1.1.1/test/test_scipost_sample_code.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_sve.py` & `sparse-ir-1.1.1/test/test_sve.py`

 * *Files identical despite different names*

### Comparing `sparse-ir-1.1.0/test/test_whitespace.py` & `sparse-ir-1.1.1/test/test_whitespace.py`

 * *Files identical despite different names*

