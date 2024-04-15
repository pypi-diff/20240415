# Comparing `tmp/sansa-1.0.0.tar.gz` & `tmp/sansa-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sansa-1.0.0.tar", last modified: Sun Mar 24 12:35:57 2024, max compression
+gzip compressed data, was "sansa-1.1.0.tar", last modified: Mon Apr 15 20:46:30 2024, max compression
```

## Comparing `sansa-1.0.0.tar` & `sansa-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.137355 sansa-1.0.0/
--rw-r--r--   0 masp       (501) staff       (20)    11357 2023-11-07 09:30:05.000000 sansa-1.0.0/LICENSE
--rw-r--r--   0 masp       (501) staff       (20)      560 2023-11-07 09:30:05.000000 sansa-1.0.0/NOTICE
--rw-r--r--   0 masp       (501) staff       (20)    24042 2024-03-24 12:35:57.137152 sansa-1.0.0/PKG-INFO
--rw-r--r--   0 masp       (501) staff       (20)     9051 2024-03-24 11:18:03.000000 sansa-1.0.0/README.md
--rw-r--r--   0 masp       (501) staff       (20)     1854 2024-03-24 12:02:16.000000 sansa-1.0.0/pyproject.toml
--rw-r--r--   0 masp       (501) staff       (20)       38 2024-03-24 12:35:57.137397 sansa-1.0.0/setup.cfg
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.132289 sansa-1.0.0/src/
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.133615 sansa-1.0.0/src/sansa/
--rw-r--r--   0 masp       (501) staff       (20)      276 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/__init__.py
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.134885 sansa-1.0.0/src/sansa/core/
--rw-r--r--   0 masp       (501) staff       (20)      429 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/core/__init__.py
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.135513 sansa-1.0.0/src/sansa/core/_ops/
--rw-r--r--   0 masp       (501) staff       (20)       84 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/core/_ops/__init__.py
--rw-r--r--   0 masp       (501) staff       (20)     8063 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/core/_ops/_factor_ops.py
--rw-r--r--   0 masp       (501) staff       (20)    16403 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/core/_ops/_inverse_ops.py
--rw-r--r--   0 masp       (501) staff       (20)    10975 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/core/factorizers.py
--rw-r--r--   0 masp       (501) staff       (20)     3354 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/core/inverters.py
--rw-r--r--   0 masp       (501) staff       (20)     5245 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/model.py
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.136468 sansa-1.0.0/src/sansa/utils/
--rw-r--r--   0 masp       (501) staff       (20)      325 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/utils/__init__.py
--rw-r--r--   0 masp       (501) staff       (20)      666 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/utils/matmat.py
--rw-r--r--   0 masp       (501) staff       (20)      863 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/utils/norms.py
--rw-r--r--   0 masp       (501) staff       (20)      978 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/utils/scaling.py
--rw-r--r--   0 masp       (501) staff       (20)     1654 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/utils/sparsify.py
--rw-r--r--   0 masp       (501) staff       (20)      746 2024-03-24 11:18:03.000000 sansa-1.0.0/src/sansa/utils/topk.py
-drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-03-24 12:35:57.136624 sansa-1.0.0/src/sansa.egg-info/
--rw-r--r--   0 masp       (501) staff       (20)    24042 2024-03-24 12:35:57.000000 sansa-1.0.0/src/sansa.egg-info/PKG-INFO
--rw-r--r--   0 masp       (501) staff       (20)      590 2024-03-24 12:35:57.000000 sansa-1.0.0/src/sansa.egg-info/SOURCES.txt
--rw-r--r--   0 masp       (501) staff       (20)        1 2024-03-24 12:35:57.000000 sansa-1.0.0/src/sansa.egg-info/dependency_links.txt
--rw-r--r--   0 masp       (501) staff       (20)      166 2024-03-24 12:35:57.000000 sansa-1.0.0/src/sansa.egg-info/requires.txt
--rw-r--r--   0 masp       (501) staff       (20)        6 2024-03-24 12:35:57.000000 sansa-1.0.0/src/sansa.egg-info/top_level.txt
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.205050 sansa-1.1.0/
+-rw-r--r--   0 masp       (501) staff       (20)    11357 2023-11-07 09:30:05.000000 sansa-1.1.0/LICENSE
+-rw-r--r--   0 masp       (501) staff       (20)      560 2023-11-07 09:30:05.000000 sansa-1.1.0/NOTICE
+-rw-r--r--   0 masp       (501) staff       (20)    24218 2024-04-15 20:46:30.204836 sansa-1.1.0/PKG-INFO
+-rw-r--r--   0 masp       (501) staff       (20)     9227 2024-04-15 20:37:40.000000 sansa-1.1.0/README.md
+-rw-r--r--   0 masp       (501) staff       (20)     1854 2024-04-15 20:38:07.000000 sansa-1.1.0/pyproject.toml
+-rw-r--r--   0 masp       (501) staff       (20)       38 2024-04-15 20:46:30.205089 sansa-1.1.0/setup.cfg
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.200956 sansa-1.1.0/src/
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.201973 sansa-1.1.0/src/sansa/
+-rw-r--r--   0 masp       (501) staff       (20)      276 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/__init__.py
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.202960 sansa-1.1.0/src/sansa/core/
+-rw-r--r--   0 masp       (501) staff       (20)      429 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/core/__init__.py
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.203309 sansa-1.1.0/src/sansa/core/_ops/
+-rw-r--r--   0 masp       (501) staff       (20)       84 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/core/_ops/__init__.py
+-rw-r--r--   0 masp       (501) staff       (20)     7928 2024-04-15 20:37:40.000000 sansa-1.1.0/src/sansa/core/_ops/_factor_ops.py
+-rw-r--r--   0 masp       (501) staff       (20)    16403 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/core/_ops/_inverse_ops.py
+-rw-r--r--   0 masp       (501) staff       (20)    12704 2024-04-15 20:37:40.000000 sansa-1.1.0/src/sansa/core/factorizers.py
+-rw-r--r--   0 masp       (501) staff       (20)     3351 2024-04-15 20:37:40.000000 sansa-1.1.0/src/sansa/core/inverters.py
+-rw-r--r--   0 masp       (501) staff       (20)     6162 2024-04-15 20:37:40.000000 sansa-1.1.0/src/sansa/model.py
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.204033 sansa-1.1.0/src/sansa/utils/
+-rw-r--r--   0 masp       (501) staff       (20)      325 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/utils/__init__.py
+-rw-r--r--   0 masp       (501) staff       (20)      666 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/utils/matmat.py
+-rw-r--r--   0 masp       (501) staff       (20)      863 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/utils/norms.py
+-rw-r--r--   0 masp       (501) staff       (20)      978 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/utils/scaling.py
+-rw-r--r--   0 masp       (501) staff       (20)     1654 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/utils/sparsify.py
+-rw-r--r--   0 masp       (501) staff       (20)      746 2024-03-24 11:18:03.000000 sansa-1.1.0/src/sansa/utils/topk.py
+drwxr-xr-x   0 masp       (501) staff       (20)        0 2024-04-15 20:46:30.204184 sansa-1.1.0/src/sansa.egg-info/
+-rw-r--r--   0 masp       (501) staff       (20)    24218 2024-04-15 20:46:30.000000 sansa-1.1.0/src/sansa.egg-info/PKG-INFO
+-rw-r--r--   0 masp       (501) staff       (20)      590 2024-04-15 20:46:30.000000 sansa-1.1.0/src/sansa.egg-info/SOURCES.txt
+-rw-r--r--   0 masp       (501) staff       (20)        1 2024-04-15 20:46:30.000000 sansa-1.1.0/src/sansa.egg-info/dependency_links.txt
+-rw-r--r--   0 masp       (501) staff       (20)      166 2024-04-15 20:46:30.000000 sansa-1.1.0/src/sansa.egg-info/requires.txt
+-rw-r--r--   0 masp       (501) staff       (20)        6 2024-04-15 20:46:30.000000 sansa-1.1.0/src/sansa.egg-info/top_level.txt
```

### Comparing `sansa-1.0.0/LICENSE` & `sansa-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/NOTICE` & `sansa-1.1.0/NOTICE`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/PKG-INFO` & `sansa-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sansa
-Version: 1.0.0
+Version: 1.1.0
 Summary: Scalable collaborative filtering model based on sparse approximate inverse
 Author-email: Martin Spisak <masp430@gmail.com>, Radek Bartyzal <radek.bartyzal@glami.cz>, Antonin Hoskovec <antonin.hoskovec@glami.cz>, Ladislav Peska <ladislav.peska@matfyz.cuni.cz>, Miroslav Tuma <miroslav.tuma@mff.cuni.cz>
 Maintainer-email: Martin Spisak <masp430@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -270,14 +270,18 @@
 - Training memory requirements are proportional to the number of non-zero elements in $X^TX$ (and this can be improved further).  
 - The model's density is prescribed via a hyperparameter. 
 - As a sparse neural network, SANSA offers *very fast inference* times.
 
 ### Learn more in our [short paper](https://dl.acm.org/doi/10.1145/3604915.3608827), or check out the conference [poster](assets/poster.pdf).
 
 ## Installation
+```bash
+pip install sansa
+```
+(make sure to install prerequisites first, see next section)
 ### Prerequisites
 Training of SANSA uses [scikit-sparse](https://github.com/scikit-sparse/scikit-sparse), which depends on the [SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse) numerical library. To install SuiteSparse on Ubuntu and macOS, run the commands below: 
 ```bash
 # Ubuntu
 sudo apt-get install libsuitesparse-dev
 
 # macOS
@@ -357,14 +361,16 @@
 config = ...  # specify configuration of SANSA model
 
 # Instantiate model with the config
 model = SANSA(config)
 
 # Train model on the user-item matrix
 model.fit(X)
+# or on a precomputed symmetric item-item matrix
+model.fit(X, compute_gramian=False)
 ```
 Weights of a SANSA model can be accessed using the `weights` attribute:
 ```python
 w1, w2 = model.weights  # tuple of scipy.sparse.csr_matrix of shape (num_items, num_items)
 ```
 Weights can be loaded into a model using the `load_weights` method:
 ```python
```

### Comparing `sansa-1.0.0/README.md` & `sansa-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,18 @@
 - Training memory requirements are proportional to the number of non-zero elements in $X^TX$ (and this can be improved further).  
 - The model's density is prescribed via a hyperparameter. 
 - As a sparse neural network, SANSA offers *very fast inference* times.
 
 ### Learn more in our [short paper](https://dl.acm.org/doi/10.1145/3604915.3608827), or check out the conference [poster](assets/poster.pdf).
 
 ## Installation
+```bash
+pip install sansa
+```
+(make sure to install prerequisites first, see next section)
 ### Prerequisites
 Training of SANSA uses [scikit-sparse](https://github.com/scikit-sparse/scikit-sparse), which depends on the [SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse) numerical library. To install SuiteSparse on Ubuntu and macOS, run the commands below: 
 ```bash
 # Ubuntu
 sudo apt-get install libsuitesparse-dev
 
 # macOS
@@ -111,14 +115,16 @@
 config = ...  # specify configuration of SANSA model
 
 # Instantiate model with the config
 model = SANSA(config)
 
 # Train model on the user-item matrix
 model.fit(X)
+# or on a precomputed symmetric item-item matrix
+model.fit(X, compute_gramian=False)
 ```
 Weights of a SANSA model can be accessed using the `weights` attribute:
 ```python
 w1, w2 = model.weights  # tuple of scipy.sparse.csr_matrix of shape (num_items, num_items)
 ```
 Weights can be loaded into a model using the `load_weights` method:
 ```python
```

### Comparing `sansa-1.0.0/pyproject.toml` & `sansa-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sansa"
-version = "1.0.0"
+version = "1.1.0"
 description = "Scalable collaborative filtering model based on sparse approximate inverse"
 dependencies = [
   "numba >= 0.57.0",
   "numpy >= 1.22.3",
   "scikit-sparse >= 0.4.8",
   "scipy >= 1.7.3",
 ]
```

### Comparing `sansa-1.0.0/src/sansa/core/_ops/_factor_ops.py` & `sansa-1.1.0/src/sansa/core/_ops/_factor_ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 def icf(
     A: sp.csc_matrix,
     l2: float,
     max_nnz: int,
     shift_step: float = 1e-3,
     shift_multiplier: float = 2.0,
 ) -> sp.csc_matrix:
-
     if isinstance(A, sp.csr_matrix):
         A = A.T
     if not isinstance(A, sp.csc_matrix):
         raise ValueError("Matrix A must be a scipy.sparse.csc_matrix")
     m, n = A.shape
     assert m == n, f"A must be square, got shape {A.shape}"
     # need at least 1 element per column
@@ -103,36 +102,38 @@
     """
     nnz = 0
     c_n = 0
     s = np.zeros(n, np.int64)  # Next non-zero row index i in column j of L
     t = np.zeros(n, np.int64)  # First subdiagonal index i in column j of A
     l = np.zeros(n, np.int64) - 1  # Linked list of non-zero columns in row k of L
     a = np.zeros(n, np.float32)  # Values of column j
-    r = np.zeros(n, np.float32)  # r[j] = sum(abs(A[j:, j])) for relative threshold
     b = np.zeros(n, np.bool_)  # b[i] indicates if the i-th element of column j is non-zero
     c = np.empty(n, np.int64)  # Row indices of non-zero elements in column j
     d = np.full(n, shift, np.float32)  # Diagonal elements of A
+
     for j in range(n):
+
         for idx in range(Ap[j], Ap[j + 1]):
             i = Ar[idx]
             if i == j:
                 d[j] += Av[idx]
                 t[j] = idx + 1
-            if i >= j:
-                r[j] += abs(Av[idx])
+
     for j in range(n):  # For each column j
+
         for idx in range(t[j], Ap[j + 1]):  # For each L_ij
             i = Ar[idx]
             L_ij = Av[idx]
             if L_ij != 0.0 and i > j:
                 a[i] += L_ij  # Assign non-zero value to L_ij in sparse column
                 if not b[i]:
                     b[i] = True  # Mark it as non-zero
                     c[c_n] = i  # Remember index for later deletion
                     c_n += 1
+
         k = l[j]  # Find index k of column with non-zero element in row j
         while k != -1:  # For each column of that type
             k0 = s[k]  # Start index of non-zero elements in column k
             k1 = Lp[k + 1]  # End index
             k2 = l[k]  # Remember next column index before it is overwritten
             L_jk = Lv[k0]  # Value of non-zero element at start of column
             k0 += 1  # Advance to next non-zero element in column
@@ -146,29 +147,33 @@
                     L_ik = Lv[idx]
                     a[i] -= L_ik * L_jk  # Update element L_ij in sparse column
                     if not b[i]:  # Check if sparse column element was zero
                         b[i] = True  # Mark as non-zero in sparse column
                         c[c_n] = i  # Remember index for later deletion
                         c_n += 1
             k = k2  # Advance to next column k
+
         if d[j] <= 0.0:
             return np.int64(-1)
+
         max_j_nnz = (max_nnz - nnz) // (n - j)  # Maximum num. of nnz elements in col j
         # keep only min(c_n, max_j_nnz) largest values in a
         if c_n > max_j_nnz:
             cc = c[:c_n]
             aa = np.abs(a[cc])
             largest_indices = np.argpartition(aa, -max_j_nnz)[-max_j_nnz:]
             b[cc] = False
             b[cc[largest_indices]] = True
+
         d[j] = np.sqrt(d[j])  # Update diagonal element L_ii
         Lv[nnz] = d[j]  # Add diagonal element L_ii to L
         Lr[nnz] = j  # Add row index of L_ii to L
         nnz += 1
         s[j] = nnz  # Set first non-zero index of column j
+
         for i in np.sort(c[:c_n]):  # Sort row indices of column j for correct insertion order into L
             L_ij = a[i] / d[j]  # Get non-zero element from sparse column j
             d[i] -= L_ij * L_ij  # Update diagonal element L_ii
             if b[i]:  # If element is not discarded and sufficiently non-zero
                 Lv[nnz] = L_ij  # Add element L_ij to L
                 Lr[nnz] = i  # Add row index of L_ij
                 nnz += 1
@@ -176,8 +181,9 @@
             b[i] = False  # Mark element as zero
         c_n = 0  # Discard row indices of non-zero elements in column j.
         Lp[j + 1] = nnz  # Update count of non-zero elements up to column j
         if Lp[j] + 1 < Lp[j + 1]:  # If column j has a non-zero element below diagonal
             i = Lr[Lp[j] + 1]  # Row index of first off-diagonal non-zero element
             l[j] = l[i]  # Remember old list i index in list j
             l[i] = j  # Insert index of non-zero element into list i
+
     return np.int64(nnz)
```

### Comparing `sansa-1.0.0/src/sansa/core/_ops/_inverse_ops.py` & `sansa-1.1.0/src/sansa/core/_ops/_inverse_ops.py`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/src/sansa/core/factorizers.py` & `sansa-1.1.0/src/sansa/core/factorizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,28 +90,31 @@
                 """
             )
             return minimum_density
         return factor_density
 
     @abstractmethod
     def approximate_cholesky(
-        self, X: sp.csr_matrix, l2: float, factor_density: float
+        self, X: sp.csr_matrix, l2: float, factor_density: float, compute_gramian: bool
     ) -> tuple[sp.csc_matrix, np.ndarray]:
         raise NotImplementedError("Implement this")
 
     def approximate_ldlt(
         self,
         X: sp.csr_matrix,
         l2: float,
         factor_density: float,
+        compute_gramian: bool,
     ) -> tuple[sp.csc_matrix, sp.dia_matrix, np.ndarray]:
 
-        # 1. Compute incomplete Cholesky decomposition of P(X^TX + self.l2 * I)P^T
+        # 1. Compute incomplete Cholesky decomposition of
+        # - P(X^TX + self.l2 * I)P^T if compute_gramian=True
+        # - P(X + self.l2 * I)P^T if compute_gramian=False
         logger.info(f"Computing incomplete Cholesky decomposition of X^TX + {l2}*I...")
-        L, p = self.approximate_cholesky(X, l2, factor_density)
+        L, p = self.approximate_cholesky(X, l2, factor_density, compute_gramian)
 
         # 2. Compute LDL^T decomposition of A' from LL^T decomposition
         logger.info("Scaling columns and creating diagonal matrix D (LL^T -> L'DL'^T)...")
         d = L.diagonal()
         # The following operation raises divide by zero warning when using intel MKL numpy (caused by endianness)
         with np.errstate(divide="ignore"):
             inplace_scale_along_compressed_axis(L, 1 / d)
@@ -146,34 +149,49 @@
             )
 
     def approximate_cholesky(
         self,
         X: sp.csr_matrix,
         l2: float,
         factor_density: float,
+        compute_gramian: bool,
     ) -> tuple[sp.csc_matrix, np.ndarray]:
 
         # 0. Clip density to a reasonable minimum
         minimum_density = 2 / X.shape[1]
         factor_density = self._clip_density_to_lower_bound(factor_density, minimum_density)
         self._suggest_icf_if_desired_density_too_low(factor_density)
 
-        # 1. Compute symbolic Cholesky factorization of X^TX along with fill-in reducing ordering
+        # 1. Compute symbolic Cholesky factorization
+        # - of X^TX if compute_gramian=True
+        # - of X if compute_gramian=False
+        # along with fill-in reducing ordering
         logger.info(f"Finding a fill-in reducing ordering (method = {self.reordering_method.value})...")
-        factor = cholmod.analyze_AAt(
-            X.transpose(),
-            mode=self.reordering_mode.value,
-            use_long=self.reordering_use_long,
-            ordering_method=self.reordering_method.value,
-        )
+        if compute_gramian:
+            factor = cholmod.analyze_AAt(
+                X.transpose(),
+                mode=self.reordering_mode.value,
+                use_long=self.reordering_use_long,
+                ordering_method=self.reordering_method.value,
+            )
+        else:
+            factor = cholmod.analyze(
+                X.transpose(),
+                mode=self.reordering_mode.value,
+                use_long=self.reordering_use_long,
+                ordering_method=self.reordering_method.value,
+            )
         p = factor.P()
 
         # 2. Compute numerical factorization
         logger.info(f"Computing approximate Cholesky decomposition (method = {self.factorization_method.value})...")
-        factor.cholesky_AAt_inplace(X.transpose(), beta=l2)
+        if compute_gramian:
+            factor.cholesky_AAt_inplace(X.transpose(), beta=l2)
+        else:
+            factor.cholesky_inplace(X.transpose(), beta=l2)
         L = factor.L().tocsc()
         del factor
         gc.collect()
 
         # 3. Drop small values from L
         current_density = L.nnz / (L.shape[0] ** 2)
         logger.info(f"Dropping small entries in L ({current_density:%} dense, target = {factor_density:%})...")
@@ -237,47 +255,75 @@
             )
 
     def approximate_cholesky(
         self,
         X: sp.csr_matrix,
         l2: float,
         factor_density: float,
+        compute_gramian: bool,
     ) -> tuple[sp.csc_matrix, np.ndarray]:
 
         # 0. Clip density to a reasonable minimum
         minimum_density = 2 / X.shape[1]
         factor_density = self._clip_density_to_lower_bound(factor_density, minimum_density)
         self._suggest_cholmod_if_desired_density_too_high(factor_density)
 
         # 1. Compute COLAMD permutation of A ( A' = [p, :]A[:, p]] )
         logger.info(f"Finding a fill-in reducing ordering (method = {self.reordering_method.value})...")
-        p = cholmod.analyze_AAt(
-            X.transpose(),
-            mode=self.reordering_mode.value,
-            use_long=self.reordering_use_long,
-            ordering_method=self.reordering_method.value,
-        ).P()
+        if compute_gramian:
+            p = cholmod.analyze_AAt(
+                X.transpose(),
+                mode=self.reordering_mode.value,
+                use_long=self.reordering_use_long,
+                ordering_method=self.reordering_method.value,
+            ).P()
+        else:
+            p = cholmod.analyze(
+                X.transpose(),
+                mode=self.reordering_mode.value,
+                use_long=self.reordering_use_long,
+                ordering_method=self.reordering_method.value,
+            ).P()
         gc.collect()
 
-        # 2. permute columns of X
-        X_P = X[:, p]
 
-        # 3. Compute A = P(X^TX)P^T
-        logger.info("Computing X^TX...")
-        A = matmat(X_P.transpose(), X_P)
-        logger.info(
-            f"""
-            X^TX info:
-                shape = {A.shape} 
-                nnz = {A.nnz} 
-                density = {A.nnz / (A.shape[0] ** 2):%} 
-                size = {(A.data.nbytes + A.indices.nbytes + A.indptr.nbytes) / 1e6:.1f} MB
-            """
-        )
-        self._suggest_cholmod_if_A_too_dense(A)
+        if compute_gramian:
+            # 2. permute columns of X
+            X_P = X[:, p]  # column permutation
+        else:
+            X_P = X[:, p]  # column permutation
+            # 2. permute row and columns of X
+            X_P = X_P[p, :]  # row permutation
+
+        if compute_gramian:
+            # 3. Compute A = P(X^TX)P^T
+            logger.info("Computing X^TX...")
+            A = matmat(X_P.transpose(), X_P)
+            logger.info(
+                f"""
+                X^TX info:
+                    shape = {A.shape} 
+                    nnz = {A.nnz} 
+                    density = {A.nnz / (A.shape[0] ** 2):%} 
+                    size = {(A.data.nbytes + A.indices.nbytes + A.indptr.nbytes) / 1e6:.1f} MB
+                """
+            )
+            self._suggest_cholmod_if_A_too_dense(A)
+        else:
+            A = X_P
+            logger.info(
+                f"""
+                X info:
+                    shape = {A.shape} 
+                    nnz = {A.nnz} 
+                    density = {A.nnz / (A.shape[0] * A.shape[1]):%} 
+                    size = {(A.data.nbytes + A.indices.nbytes + A.indptr.nbytes) / 1e6:.1f} MB
+                """
+            )
+        del X_P
 
         # 4. Prepare A for ICF algorithm
         logger.info("Sorting indices of A...")
         A.sort_indices()
         self._index_dtypes_to_int64(A)
         gc.collect()
```

### Comparing `sansa-1.0.0/src/sansa/core/inverters.py` & `sansa-1.1.0/src/sansa/core/inverters.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     @property
     @abstractmethod
     def config(self) -> UnitLowerTriangleInverterConfig:
         raise NotImplementedError("Implement this")
 
     @classmethod
-    def from_config(cls, config: UnitLowerTriangleInverterConfig) -> "UnitLowerTriangleInverterConfig":
+    def from_config(cls, config: UnitLowerTriangleInverterConfig) -> "UnitLowerTriangleInverter":
         module = importlib.import_module(__name__)
         class_name = "".join([config.approximate_inverse_method.value, cls.__name__])
         factorizer_class = getattr(module, class_name)
         return factorizer_class(config)
 
     @abstractmethod
     def invert(self, L: sp.csc_matrix) -> sp.csc_matrix:
@@ -92,11 +92,11 @@
         # Final residual norm evaluation:
         # Compute residual matrix
         R = get_residual_matrix(L, L_inv)
         # Compute column norms of R
         norms = get_norms_along_compressed_axis(R)
         del R
         max_res = np.max(norms)  # Maximum residual
-        loss = np.mean(norms)  # Loss = n * MSE = mean (column norm)^2 = (relative Frobenius norm)^2
+        loss = np.mean(norms**2)  # Loss = n * MSE = mean (column norm)^2 = (relative Frobenius norm)^2
         logger.info(f"Current maximum residual: {max_res}, relative Frobenius norm squared: {loss}")
 
         return L_inv
```

### Comparing `sansa-1.0.0/src/sansa/model.py` & `sansa-1.1.0/src/sansa/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -18,26 +18,38 @@
     inplace_scale_along_compressed_axis,
     inplace_scale_along_uncompressed_axis,
     matmat,
     top_k_along_compressed_axis,
 )
 
 logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
+logging.basicConfig(level=logging.INFO)
 
 
-def _apply_icf_scaling(X: sp.csr_matrix) -> None:
-    """Inplace scale columns of X by square roots of column norms of X^TX."""
-    logger.info(f"Computing column norms of X^TX...")
-    da = np.sqrt(np.sqrt(get_squared_norms_along_compressed_axis(matmat(X.T, X))))
-    # Divide columns of X by the computed square roots of row norms of X^TX
-    da[da == 0] = 1  # ignore zero elements
-    logger.info(f"Scaling columns of X by computed norms...")
-    inplace_scale_along_uncompressed_axis(X, 1 / da)  # CSR column scaling
-    del da
+def _apply_icf_scaling(X: sp.csr_matrix, compute_gramian: bool) -> None:
+    if compute_gramian:
+        # Inplace scale columns of X by square roots of column norms of X^TX.
+        logger.info(f"Computing column norms of X^TX...")
+        da = np.sqrt(np.sqrt(get_squared_norms_along_compressed_axis(matmat(X.T, X))))
+        # Divide columns of X by the computed square roots of row norms of X^TX
+        da[da == 0] = 1  # ignore zero elements
+        logger.info(f"Scaling columns of X by computed norms...")
+        inplace_scale_along_uncompressed_axis(X, 1 / da)  # CSR column scaling
+        del da
+    else:
+        # Inplace scale rows and columns of X by square roots of row norms of X.
+        logger.info(f"Computing row norms of X...")
+        da = np.sqrt(np.sqrt(get_squared_norms_along_compressed_axis(X)))
+        # Divide rows and columns of X by the computed square roots of row norms of X
+        da[da == 0] = 1  # ignore zero elements
+        logger.info(f"Scaling rows and columns of X by computed norms...")
+        inplace_scale_along_uncompressed_axis(X, 1 / da)  # CSR column scaling
+        inplace_scale_along_compressed_axis(X, 1 / da)  # CSR row scaling
+        del da
+
 
 
 @dataclass
 class SANSAConfig:
     l2: float
     weight_matrix_density: float
     gramian_factorizer_config: GramianFactorizerConfig
@@ -62,29 +74,36 @@
             self.inverter.config,
         )
 
     def load_weights(self, weights: Tuple[sp.csr_matrix, sp.csr_matrix]) -> "SANSA":
         self.weights = weights
         return self
 
-    def fit(self, user_item_matrix: sp.csr_matrix) -> "SANSA":
+    def fit(self, training_matrix: sp.csr_matrix, compute_gramian=True) -> "SANSA":
         """
-        Fit SANSA model with user item matrix.
+        Fit SANSA model with user-item or item-item matrix.
         """
         # create a working copy of user_item_matrix
-        X = user_item_matrix.copy()
+        X = training_matrix.copy()
         X = X.astype(np.float32)
 
         if self.factorization_method == FactorizationMethod.ICF:
             # scale matrix X
-            _apply_icf_scaling(X)
+            _apply_icf_scaling(X, compute_gramian)
 
-        # Compute LDL^T decomposition of P(X^TX + self.l2 * I)P^T
+        # Compute LDL^T decomposition of
+        # - P(X^TX + self.l2 * I)P^T if compute_gramian=True
+        # - P(X + self.l2 * I)P^T if compute_gramian=False
         logger.info("Computing LDL^T decomposition of permuted item-item matrix...")
-        L, D, p = self.factorizer.approximate_ldlt(X, self.l2, self.weight_matrix_density)
+        L, D, p = self.factorizer.approximate_ldlt(
+            X,
+            self.l2,
+            self.weight_matrix_density,
+            compute_gramian=compute_gramian,
+        )
         del X
 
         # Compute approximate inverse of L using selected method
         logger.info("Computing approximate inverse of L...")
         L_inv = self.inverter.invert(L)
         del L
```

### Comparing `sansa-1.0.0/src/sansa/utils/matmat.py` & `sansa-1.1.0/src/sansa/utils/matmat.py`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/src/sansa/utils/norms.py` & `sansa-1.1.0/src/sansa/utils/norms.py`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/src/sansa/utils/scaling.py` & `sansa-1.1.0/src/sansa/utils/scaling.py`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/src/sansa/utils/sparsify.py` & `sansa-1.1.0/src/sansa/utils/sparsify.py`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/src/sansa/utils/topk.py` & `sansa-1.1.0/src/sansa/utils/topk.py`

 * *Files identical despite different names*

### Comparing `sansa-1.0.0/src/sansa.egg-info/PKG-INFO` & `sansa-1.1.0/src/sansa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sansa
-Version: 1.0.0
+Version: 1.1.0
 Summary: Scalable collaborative filtering model based on sparse approximate inverse
 Author-email: Martin Spisak <masp430@gmail.com>, Radek Bartyzal <radek.bartyzal@glami.cz>, Antonin Hoskovec <antonin.hoskovec@glami.cz>, Ladislav Peska <ladislav.peska@matfyz.cuni.cz>, Miroslav Tuma <miroslav.tuma@mff.cuni.cz>
 Maintainer-email: Martin Spisak <masp430@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -270,14 +270,18 @@
 - Training memory requirements are proportional to the number of non-zero elements in $X^TX$ (and this can be improved further).  
 - The model's density is prescribed via a hyperparameter. 
 - As a sparse neural network, SANSA offers *very fast inference* times.
 
 ### Learn more in our [short paper](https://dl.acm.org/doi/10.1145/3604915.3608827), or check out the conference [poster](assets/poster.pdf).
 
 ## Installation
+```bash
+pip install sansa
+```
+(make sure to install prerequisites first, see next section)
 ### Prerequisites
 Training of SANSA uses [scikit-sparse](https://github.com/scikit-sparse/scikit-sparse), which depends on the [SuiteSparse](https://github.com/DrTimothyAldenDavis/SuiteSparse) numerical library. To install SuiteSparse on Ubuntu and macOS, run the commands below: 
 ```bash
 # Ubuntu
 sudo apt-get install libsuitesparse-dev
 
 # macOS
@@ -357,14 +361,16 @@
 config = ...  # specify configuration of SANSA model
 
 # Instantiate model with the config
 model = SANSA(config)
 
 # Train model on the user-item matrix
 model.fit(X)
+# or on a precomputed symmetric item-item matrix
+model.fit(X, compute_gramian=False)
 ```
 Weights of a SANSA model can be accessed using the `weights` attribute:
 ```python
 w1, w2 = model.weights  # tuple of scipy.sparse.csr_matrix of shape (num_items, num_items)
 ```
 Weights can be loaded into a model using the `load_weights` method:
 ```python
```

### Comparing `sansa-1.0.0/src/sansa.egg-info/SOURCES.txt` & `sansa-1.1.0/src/sansa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

