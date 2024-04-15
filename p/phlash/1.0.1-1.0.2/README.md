# Comparing `tmp/phlash-1.0.1.tar.gz` & `tmp/phlash-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phlash-1.0.1.tar", last modified: Mon Mar 11 16:05:00 2024, max compression
+gzip compressed data, was "phlash-1.0.2.tar", last modified: Mon Apr 15 18:04:13 2024, max compression
```

## Comparing `phlash-1.0.1.tar` & `phlash-1.0.2.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0       54 2024-01-18 15:50:39.314184 phlash-1.0.1/AUTHORS.md
--rw-r--r--   0        0        0     1102 2024-02-23 17:51:48.581326 phlash-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2012 2024-03-11 15:53:47.896597 phlash-1.0.1/README.md
--rw-r--r--   0        0        0     2434 2024-03-11 16:05:00.774773 phlash-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1089 2024-02-23 17:51:48.581326 phlash-1.0.1/src/phlash/__init__.py
--rw-r--r--   0        0        0      467 2024-03-07 16:19:49.405975 phlash-1.0.1/src/phlash/_version.py
--rw-r--r--   0        0        0      986 2024-03-07 01:41:49.831734 phlash-1.0.1/src/phlash/afs.py
--rw-r--r--   0        0        0     4850 2024-03-11 16:00:02.229807 phlash-1.0.1/src/phlash/cband.py
--rw-r--r--   0        0        0    17009 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/data.py
--rw-r--r--   0        0        0    22530 2024-02-25 18:47:13.332034 phlash-1.0.1/src/phlash/gpu.py
--rw-r--r--   0        0        0     1212 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/hmm.py
--rw-r--r--   0        0        0     2431 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/jax_ppoly.py
--rw-r--r--   0        0        0     4459 2024-02-25 01:52:38.841162 phlash-1.0.1/src/phlash/liveplot.py
--rw-r--r--   0        0        0    12174 2024-03-11 15:36:03.541212 phlash-1.0.1/src/phlash/mcmc.py
--rw-r--r--   0        0        0     2644 2024-03-07 01:41:49.831734 phlash-1.0.1/src/phlash/model.py
--rw-r--r--   0        0        0      646 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/mp.py
--rw-r--r--   0        0        0     3537 2024-02-25 18:55:33.686447 phlash-1.0.1/src/phlash/params.py
--rw-r--r--   0        0        0      726 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/plot.py
--rw-r--r--   0        0        0    10355 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/sim.py
--rw-r--r--   0        0        0    11828 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/size_history.py
--rw-r--r--   0        0        0     2612 2024-02-23 17:51:48.585326 phlash-1.0.1/src/phlash/transition.py
--rw-r--r--   0        0        0     1301 2024-03-07 01:43:16.655984 phlash-1.0.1/src/phlash/util.py
--rw-r--r--   0        0        0    53248 2023-12-14 20:24:56.454022 phlash-1.0.1/tests/.coverage
--rw-r--r--   0        0        0       37 2024-02-07 01:57:37.951589 phlash-1.0.1/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2024-02-07 01:57:37.951589 phlash-1.0.1/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2024-02-07 01:57:37.951589 phlash-1.0.1/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0      191 2024-02-24 09:47:21.894842 phlash-1.0.1/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1945 2024-02-24 10:22:02.233052 phlash-1.0.1/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2024-02-24 10:22:02.257052 phlash-1.0.1/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      662 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/conftest.py
--rw-r--r--   0        0        0  1306723 2024-02-24 19:03:38.092173 phlash-1.0.1/tests/fixtures/elpd_bug.pkl
--rw-r--r--   0        0        0   131135 2024-01-07 18:27:14.126332 phlash-1.0.1/tests/fixtures/sample.bcf
--rw-r--r--   0        0        0      244 2024-01-07 18:27:14.126332 phlash-1.0.1/tests/fixtures/sample.bcf.csi
--rw-r--r--   0        0        0    17967 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/fixtures/tv_bug.pkl
--rw-r--r--   0        0        0      940 2024-03-07 01:41:49.831734 phlash-1.0.1/tests/test_afs.py
--rw-r--r--   0        0        0     1019 2024-03-11 16:00:58.769990 phlash-1.0.1/tests/test_cband.py
--rw-r--r--   0        0        0     2412 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_data.py
--rw-r--r--   0        0        0     1359 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_gpu.py
--rw-r--r--   0        0        0      473 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_hmm.py
--rw-r--r--   0        0        0     1628 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_jax_ppoly.py
--rw-r--r--   0        0        0      434 2024-03-07 01:51:29.865410 phlash-1.0.1/tests/test_mcmc.py
--rw-r--r--   0        0        0      574 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_model.py
--rw-r--r--   0        0        0      631 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_sim.py
--rw-r--r--   0        0        0     4518 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_size_history.py
--rw-r--r--   0        0        0      818 2024-02-23 17:51:48.585326 phlash-1.0.1/tests/test_transition.py
--rw-r--r--   0        0        0     3368 1970-01-01 00:00:00.000000 phlash-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-01-18 15:50:39.314184 phlash-1.0.2/AUTHORS.md
+-rw-r--r--   0        0        0     1102 2024-02-23 17:51:48.581326 phlash-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2176 2024-04-15 15:25:43.833513 phlash-1.0.2/README.md
+-rw-r--r--   0        0        0     2480 2024-04-15 18:04:13.809324 phlash-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1089 2024-02-23 17:51:48.581326 phlash-1.0.2/src/phlash/__init__.py
+-rw-r--r--   0        0        0      467 2024-03-07 16:19:49.405975 phlash-1.0.2/src/phlash/_version.py
+-rw-r--r--   0        0        0      986 2024-03-07 01:41:49.831734 phlash-1.0.2/src/phlash/afs.py
+-rw-r--r--   0        0        0     4798 2024-04-15 17:47:41.920951 phlash-1.0.2/src/phlash/cband.py
+-rw-r--r--   0        0        0    18202 2024-04-15 17:56:27.355273 phlash-1.0.2/src/phlash/data.py
+-rw-r--r--   0        0        0    21860 2024-04-15 17:25:10.586956 phlash-1.0.2/src/phlash/gpu.py
+-rw-r--r--   0        0        0     2467 2024-04-15 17:11:30.103462 phlash-1.0.2/src/phlash/hmm.py
+-rw-r--r--   0        0        0     2431 2024-02-23 17:51:48.585326 phlash-1.0.2/src/phlash/jax_ppoly.py
+-rw-r--r--   0        0        0      794 2024-04-15 17:25:29.551038 phlash-1.0.2/src/phlash/kernel.py
+-rw-r--r--   0        0        0     4459 2024-02-25 01:52:38.841162 phlash-1.0.2/src/phlash/liveplot.py
+-rw-r--r--   0        0        0    12267 2024-04-15 16:41:29.503757 phlash-1.0.2/src/phlash/mcmc.py
+-rw-r--r--   0        0        0     2430 2024-04-15 14:57:48.773013 phlash-1.0.2/src/phlash/model.py
+-rw-r--r--   0        0        0      646 2024-02-23 17:51:48.585326 phlash-1.0.2/src/phlash/mp.py
+-rw-r--r--   0        0        0     3536 2024-04-15 14:56:43.652824 phlash-1.0.2/src/phlash/params.py
+-rw-r--r--   0        0        0      726 2024-02-23 17:51:48.585326 phlash-1.0.2/src/phlash/plot.py
+-rw-r--r--   0        0        0    10355 2024-04-15 18:04:01.489269 phlash-1.0.2/src/phlash/sim.py
+-rw-r--r--   0        0        0    12105 2024-03-26 00:31:45.400238 phlash-1.0.2/src/phlash/size_history.py
+-rw-r--r--   0        0        0     2616 2024-03-25 20:23:13.263219 phlash-1.0.2/src/phlash/transition.py
+-rw-r--r--   0        0        0     1301 2024-03-07 01:43:16.655984 phlash-1.0.2/src/phlash/util.py
+-rw-r--r--   0        0        0    48861 2024-03-15 16:55:50.847090 phlash-1.0.2/tests/.benchmarks/Linux-CPython-3.10-64bit/0001_gpu_vs_jax.json
+-rw-r--r--   0        0        0    53248 2023-12-14 20:24:56.454022 phlash-1.0.2/tests/.coverage
+-rw-r--r--   0        0        0       37 2024-02-07 01:57:37.951589 phlash-1.0.2/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2024-02-07 01:57:37.951589 phlash-1.0.2/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2024-02-07 01:57:37.951589 phlash-1.0.2/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0     1895 2024-03-15 16:55:50.895090 phlash-1.0.2/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    13396 2024-03-15 16:55:50.851090 phlash-1.0.2/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2024-03-15 16:55:50.895090 phlash-1.0.2/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      665 2024-04-15 17:12:20.383672 phlash-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0  1306723 2024-02-24 19:03:38.092173 phlash-1.0.2/tests/fixtures/elpd_bug.pkl
+-rw-r--r--   0        0        0   131135 2024-01-07 18:27:14.126332 phlash-1.0.2/tests/fixtures/sample.bcf
+-rw-r--r--   0        0        0      244 2024-01-07 18:27:14.126332 phlash-1.0.2/tests/fixtures/sample.bcf.csi
+-rw-r--r--   0        0        0      105 2024-04-15 17:52:56.714345 phlash-1.0.2/tests/fixtures/sample.psmcfa
+-rw-r--r--   0        0        0    17967 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/fixtures/tv_bug.pkl
+-rw-r--r--   0        0        0      940 2024-03-07 01:41:49.831734 phlash-1.0.2/tests/test_afs.py
+-rw-r--r--   0        0        0     1019 2024-03-11 16:00:58.769990 phlash-1.0.2/tests/test_cband.py
+-rw-r--r--   0        0        0     2872 2024-04-15 17:56:27.011272 phlash-1.0.2/tests/test_data.py
+-rw-r--r--   0        0        0     1599 2024-04-15 17:12:32.355723 phlash-1.0.2/tests/test_gpu.py
+-rw-r--r--   0        0        0      473 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_hmm.py
+-rw-r--r--   0        0        0     1628 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_jax_ppoly.py
+-rw-r--r--   0        0        0      434 2024-04-15 15:39:57.675107 phlash-1.0.2/tests/test_mcmc.py
+-rw-r--r--   0        0        0      574 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_model.py
+-rw-r--r--   0        0        0      631 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_sim.py
+-rw-r--r--   0        0        0     4518 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_size_history.py
+-rw-r--r--   0        0        0     1121 2024-04-15 17:18:55.073344 phlash-1.0.2/tests/test_speed.py
+-rw-r--r--   0        0        0      818 2024-02-23 17:51:48.585326 phlash-1.0.2/tests/test_transition.py
+-rw-r--r--   0        0        0     3636 1970-01-01 00:00:00.000000 phlash-1.0.2/PKG-INFO
```

### Comparing `phlash-1.0.1/LICENSE.txt` & `phlash-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/README.md` & `phlash-1.0.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,41 +2,51 @@
 history given whole genome sequence data. You can think of it as a Bayesian version
 of Li & Durbin's popular [PSMC](https://github.com/lh3/psmc) program, with a more
 modern interface and GPU acceleration built in.
 
 ## Requirements
 
 - Python 3.10 or greater.
+
+Optional but _highly recommended_:
+
 - An NVIDIA GPU. Any relatively recent model should work. phlash has been tested on:
     - RTX 4090
     - A40
     - A100
     - V100
 
 ## Installation
 
-phlash can be installed from PyPI using pip, however the usual `pip install phlash`
-will fail because of dependence on CUDA and Jax packages which are not published on
-PyPI. Instead, you must run:
+phlash can be installed from PyPI using pip:
+
+```
+$ pip install phlash
+```
+
+If your machine contains an Nvidia GPU, you should install the `gpu` variant in order to enable it.
+In this case, you should run:
 
 ```
 $ pip install \
     -f "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html" \
     --extra-index-url "https://pypi.ngc.nvidia.com" \
-    phlash
+    phlash[gpu]
 ```
 
 I recommend installing phlash into a separate virtual environment: before running the
 above, do
 
 ```
 $ python3 -mvenv /path/to/phlash  # replace with desired path
 $ source /path/to/phlash/bin/activate
 $ pip3 install -U pip setuptools  # recent version of pip and setuptools are required
 ```
+## Running the program
+See [notebooks/example.md](notebooks/example.md) for example code and usage instructions.
 
 ## Troubleshooting / FAQ
 
 I (Jonathan) am happy to assist you with using phlash, as much as my time allows.
 
 - If you encounter a **bug** (program crash or other unexpected behavior) please
 [file an issue](https://github.com/jthlab/phlash/issues/new) describing the bug.
```

### Comparing `phlash-1.0.1/pyproject.toml` & `phlash-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,49 +6,53 @@
     { name = "Jonathan Terhorst", email = "jonth@umich.edu" },
 ]
 dependencies = [
     "blackjax<2.0.0,>=1.1.0",
     "cuda-python<13,>=12.3",
     "cyvcf2<1.0.0,>=0.30.28",
     "intervaltree<4.0.0,>=3.1.0",
-    "jax[cuda12_pip]>=0.4.24",
+    "jax>=0.4.24",
     "loguru<1.0.0,>=0.7.2",
     "matplotlib<4.0.0,>=3.8.2",
     "msprime<2.0.0,>=1.3.0",
-    "nvidia-cuda-nvrtc-cu12>=12.3,<13",
     "numpy<2.0.0,>=1.26.3",
     "optax<1.0.0,>=0.1.9",
     "plotly<6.0.0,>=5.18.0",
     "scipy<2.0.0,>=1.12.0",
     "stdpopsim<1.0.0,>=0.2.0",
     "tqdm<5.0.0,>=4.66.1",
     "tskit<1.0.0,>=0.5.6",
     "demes<1.0.0,>=0.2.3",
     "jax-dataclasses<2.0.0,>=1.6.0",
     "tszip<1.0.0,>=0.2.3",
     "jaxtyping<1.0.0,>=0.2.25",
     "pulp>=2.8.0",
+    "dinopy>=3.0.0",
 ]
 requires-python = ">=3.10,<4.0"
 readme = "README.md"
-version = "1.0.1"
+version = "1.0.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/jthlab/phlash"
 "Bug Reports" = "https://github.com/jthlab/phlash/issues"
 Source = "https://github.com/jthlab/phlash/"
 
 [project.optional-dependencies]
 webui = [
     "jupyter>=1.0.0",
     "notebook>=7.1.1",
 ]
+gpu = [
+    "jax[cuda12_pip]>=0.4.24",
+    "nvidia-cuda-nvrtc-cu12>=12.3",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
```

### Comparing `phlash-1.0.1/src/phlash/__init__.py` & `phlash-1.0.2/src/phlash/__init__.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/afs.py` & `phlash-1.0.2/src/phlash/afs.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/cband.py` & `phlash-1.0.2/src/phlash/cband.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,14 @@
     Raises:
         ValueError: If T and A have different shapes.
     """
     # defer the import to here as it prints some annoying warning messages that
     # most users don't need to see
     import pulp as pl
 
-    if solver is None:
-        solver = pl.GUROBI()
     N, K = A.shape
     if t.shape != (K,):
         raise ValueError("A and t have incompatible shapes")
 
     # Setting up the problem
     prob = pl.LpProblem("Confidence_Bands", pl.LpMinimize)
     u = pl.LpVariable.dicts("u", range(K), cat="Continuous")
```

### Comparing `phlash-1.0.1/src/phlash/data.py` & `phlash-1.0.2/src/phlash/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 "Classes for importing data"
 
 import re
 from abc import ABC, abstractmethod
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import as_completed
 from dataclasses import asdict, dataclass, field
 from typing import NamedTuple
 
 import cyvcf2
+import dinopy
 import numpy as np
 import tqdm.auto as tqdm
 import tskit
 import tszip
 from intervaltree import IntervalTree
 from jaxtyping import Array, Int, Int8
 from loguru import logger
 
+from phlash.mp import JaxCpuProcessPoolExecutor
+
 
 class ChunkedContig(NamedTuple):
     chunks: Int8[Array, "N L"]
     afs: Int[Array, "n"]
 
 
 def _trim_het_matrix(het_matrix: np.ndarray):
@@ -112,14 +115,43 @@
 @dataclass(frozen=True)
 class RawContig(Contig):
     "A contig with pre-computed het matrix and afs."
     het_matrix: Int8[Array, "N L"]
     afs: Int[Array, "n"]
     window_size: int
 
+    @classmethod
+    def from_psmcfa(
+        cls, psmcfa_path: str, contig: str, window_size: int
+    ) -> "RawContig":
+        """Construct a contig from a PSMC FASTA (.psmcfa) file.
+
+        Args:
+            psmcfa_path: The path to the .psmcfa file.
+            contig: The name of the contig to read in.
+            window_size: The size of the window that was used when binning entries
+                to construct the FASTA file.
+
+        Notes:
+            The `window_size` parameter corresponds to the `-s` option that was passed
+            to the `fq2psmcfa` utility when creating the .psmcfa file, and is usually
+            set to 100bp.
+        """
+        # parse psmcfa file
+        far = dinopy.FastaReader(psmcfa_path)
+        try:
+            c = next(far.chromosomes(contig))
+        except StopIteration:
+            raise ValueError(f"A contig named {contig} was not found in {psmcfa_path}")
+        seq = np.frombuffer(c.sequence, dtype="c")
+        data = (seq == b"K").astype(np.uint8)
+        (L,) = data.shape
+        afs = np.ones(1)
+        return cls(het_matrix=data[None], afs=afs, window_size=window_size)
+
     @property
     def N(self):
         # the het matrix has one row per diploid pair, so the number of ploids
         # is twice its first dimension.
         if self.het_matrix is None:
             return None
         return 2 * self.het_matrix.shape[0]
@@ -468,29 +500,29 @@
         logger.warning(
             "The chunk size is {}, which is less than 10 times the overlap ({}).",
             chunk_size,
             overlap,
         )
     chunks = []
     total_size = sum(ds.size for ds in data if ds.size)
-    with ThreadPoolExecutor(num_workers) as pool:
+    with JaxCpuProcessPoolExecutor(num_workers) as pool:
         futs = {}
         for i, ds in enumerate(data):
             fut = pool.submit(
                 ds.to_chunked,
                 overlap=overlap,
                 chunk_size=chunk_size,
                 window_size=window_size,
             )
             futs[fut] = i
         with tqdm.tqdm(total=total_size, unit="bp", unit_scale=True) as pbar:
             for f in as_completed(futs):
                 i = futs[f]
                 size = data[i].size
-                data[i] = None  # free memory associated with dataset
+                # data[i] = None  # free memory associated with dataset
                 if size:
                     pbar.update(size)
                 d = f.result()
                 if d.afs is not None:
                     afss.append(d.afs)
                 if d.chunks is not None:
                     chunks.append(d.chunks)
```

### Comparing `phlash-1.0.1/src/phlash/gpu.py` & `phlash-1.0.2/src/phlash/gpu.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,23 +116,14 @@
         except CudaError as e:
             logger.debug(f"{data.shape=}")
             raise MemoryError(
                 f"While trying to allocate {data.nbytes} bytes on GPU"
             ) from e
         (err,) = cuda.cuMemcpyHtoD(self._data_gpu, data, data.nbytes)
         ASSERT_DRV(err)
-        a = data[:, ::-1] == -1
-        end_j = self._L - np.argmax(a, 1) - 1
-        # 1 + end because the command returns closed intervals (inclusive of endpoints)
-        L_max = self._L_max = np.ascontiguousarray(1 + end_j).astype(np.int64)
-        assert L_max.shape == (self._N,)
-        err, self._L_max_gpu = cuda.cuMemAlloc(L_max.nbytes)
-        ASSERT_DRV(err)
-        (err,) = cuda.cuMemcpyHtoD(self._L_max_gpu, L_max, L_max.nbytes)
-        ASSERT_DRV(err)
         # some more checks
         if M != 16:
             warnings.warn("Performance is optimized when M=16")
         self._M = M
         src = [f"#define M {M}"]
         if double_precision:
             src.append("typedef double FLOAT;")
@@ -162,15 +153,14 @@
         # I don't understand how this can happen since it's initialized at the top of
         # the file. everything is surrounded with try/catch blocks to guard against.
         if hasattr(self, "_mod"):
             (err,) = cuda.cuModuleUnload(self._mod)
             ASSERT_DRV(err)
         for a in (
             "_data_gpu",
-            "_L_max_gpu",
             "_inds_gpu",
             "_pa_gpu",
             "_ll_gpu",
             "_dlog_gpu",
         ):
             if hasattr(self, a) and getattr(self, a) is not None:
                 (err,) = cuda.cuMemFree(getattr(self, a))
@@ -244,22 +234,21 @@
         (err,) = cuda.cuMemcpyHtoDAsync(self._inds_gpu, inds, inds.nbytes, self._stream)
         ASSERT_DRV(err)
         (err,) = cuda.cuMemcpyHtoDAsync(self._pa_gpu, pa, pa.nbytes, self._stream)
         ASSERT_DRV(err)
         (err,) = cuda.cuMemcpyHtoDAsync(self._ll_gpu, ll, ll.nbytes, self._stream)
         arg_values = (
             self._data_gpu,
-            self._L_max_gpu,
             np.int64(self._L),
             np.int64(N),
             self._inds_gpu,
             self._pa_gpu,
             self._ll_gpu,
         )
-        arg_types = (None, None, ctypes.c_int64, ctypes.c_int64, None, None, None)
+        arg_types = (None, ctypes.c_int64, ctypes.c_int64, None, None, None)
         if grad:
             f = self._f["loglik_grad"]
             (err,) = cuda.cuMemcpyHtoDAsync(
                 self._dlog_gpu, dlog, dlog.nbytes, self._stream
             )
             ASSERT_DRV(err)
             arg_values += (self._dlog_gpu,)
@@ -529,15 +518,14 @@
     return EMIS(ob, m);
 }
 
 extern "C"
 __global__ void
 // log-likelihood function without gradient
 loglik(int8_t const *datag,
-       const int64_t *L_max,
        const int64_t L,
        const int64_t N,
        const int64_t *inds,
        FLOAT const *pg,  // [B, P, M]
        double *loglik
        ) {
     const int64_t b = blockIdx.x;
@@ -558,16 +546,15 @@
         h[m] = PI(m);  // initialize to pi
     }
     double ll = 0.;
     // local variables
     const int8_t *data = &datag[inds[s] * L];
     int8_t ob;
     int64_t ell;
-    const int64_t Lm = L_max[inds[s]];
-    for (ell = 0; ell < Lm; ell++) {
+    for (ell = 0; ell < L; ell++) {
         matvec(h, p);
         ob = data[ell];
         c = 0.;
         for (m = 0; m < M; ++m) {
             h[m] *= p_emis(ob, p, m);
             c += h[m];
         }
@@ -578,15 +565,14 @@
 }
 
 extern "C"
 __global__ void
 __launch_bounds__(7 * M)
 // value and gradient of the log-likelihood function
 loglik_grad(int8_t const *datag,
-          const int64_t *L_max,
           const int64_t L,
           const int64_t N,
           const int64_t *inds,
           FLOAT const *pg,
           double *loglik,
           FLOAT *dlog
          ) {
@@ -635,16 +621,15 @@
         delta = +1;
     }
     // main data loop
     const int8_t *data = &datag[inds[s] * L];
     int64_t ell;
     c = 0.;
     __syncthreads();
-    const int64_t Lm = L_max[inds[s]];
-    for (ell = 0; ell < Lm; ell++) {
+    for (ell = 0; ell < L; ell++) {
         // read chunks of the data from coalesced global memory
         ob = data[ell];
         // update each derivative matrix
         matvec(&LOG_X(m, 0), p, LOG_X_STRIDE);
         sum1 = 0.;
         sum2 = 0.;
         for (j = start; j >= 0 && j < M; j += delta) {
```

### Comparing `phlash-1.0.1/src/phlash/jax_ppoly.py` & `phlash-1.0.2/src/phlash/jax_ppoly.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/liveplot.py` & `phlash-1.0.2/src/phlash/liveplot.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/mcmc.py` & `phlash-1.0.2/src/phlash/mcmc.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from jax import numpy as jnp
 from jax import vmap
 from jax.flatten_util import ravel_pytree
 from loguru import logger
 
 from phlash.afs import bws_transform, fold_transform
 from phlash.data import Contig, init_mcmc_data
+from phlash.kernel import get_kernel
 from phlash.model import log_density
 from phlash.params import MCMCParams
 from phlash.size_history import DemographicModel
 from phlash.util import Pattern, tree_unstack
 
 
 def _check_jax_gpu():
@@ -75,16 +76,20 @@
     # the amount overlap between adjacent windows, used to break long sequential hmm
     # observations into parallelizable batches. this should generally be left at the
     # default 500. see manuscript for more information on this parameter.
     overlap = options.get("overlap", 500)
     # the size of each "chunk", see manuscript. this is estimated from data.
     chunk_size = options.get("chunk_size")
     max_samples = options.get("max_samples", 20)
-    # the number of parallel workers
+
+    # data loading routines. this can take a little while.
+    # the number of parallel workers. by default, use all cores, but this can take up
+    # too much memory. set num_workers=1 to process the data sequentially.
     num_workers = options.get("num_workers")
+    logger.info("Loading data")
     afs, chunks = init_mcmc_data(
         data, window_size, overlap, chunk_size, max_samples, num_workers
     )
     # to conserve memory, we get rid of data at this point
     del data
     # the mutation rate per generation, if known.
     mutation_rate = options.get("mutation_rate")
@@ -191,32 +196,29 @@
     state = svgd.init(initial_particles)
     # this function takes gradients steps.
     step = jit(svgd.step, static_argnames=["kern"])
 
     # the warmup chunks and data chunks are analyzed differently; the data chunks load
     # onto the GPU whereas the warmup chunks are processed by native jax.
     warmup_chunks, data_chunks = np.split(chunks, [overlap], axis=1)
-    # defer loading the gpu module until necessary, to keep from having to initialize
-    # CUDA on overall package load.
-    from phlash.gpu import PSMCKernel
 
-    train_kern = PSMCKernel(
+    train_kern = get_kernel(
         M=M,
         data=np.ascontiguousarray(data_chunks),
         double_precision=options.get("double_precision", False),
     )
 
     # if there is a test set, define elpd() function for computing expected
     # log-predictive density. used to gauge convergence.
     if test_data:
         d = test_data.get_data(window_size)
         test_afs = d["afs"]
         test_data = d["het_matrix"][:max_samples]
         N_test = test_data.shape[0]
-        test_kern = PSMCKernel(
+        test_kern = get_kernel(
             M=M,
             data=np.ascontiguousarray(d["het_matrix"]),
             double_precision=False,
         )
 
         @jit
         def elpd(mcps):
```

### Comparing `phlash-1.0.1/src/phlash/model.py` & `phlash-1.0.2/src/phlash/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 import jax
 import jax.numpy as jnp
-import jax.scipy as jsp
 from jax import vmap
 from jax.scipy.special import xlogy
 from jaxtyping import Array, Float, Float64, Int8, Int64
 
 import phlash.hmm
 from phlash.params import MCMCParams, PSMCParams
 
 
 def log_prior(mcp: MCMCParams) -> float:
-    dm = mcp.to_dm()
     ret = sum(
         jax.scipy.stats.norm.logpdf(a, loc=mu, scale=sigma).sum()
         for (a, mu, sigma) in [
             (jnp.log(mcp.rho_over_theta), 0.0, 1.0),
         ]
     )
     ret -= mcp.alpha * jnp.sum(jnp.diff(mcp.log_c) ** 2)
     x, _ = jax.flatten_util.ravel_pytree(mcp)
-    # ret -= mcp.beta * x.dot(x)
-    pi = jnp.maximum(1e-8, dm.eta.pi)
-    # (lack of) entropy penalty
-    H = -jsp.special.xlogy(pi, pi).sum()
-    # jax.debug.print("pi={} H={}", pi, H)
-    ret += H
+    ret -= mcp.beta * x.dot(x)
     return ret
 
 
 def log_density(
     mcp: MCMCParams,
     c: Float64[Array, "3"],
     inds: Int64[Array, "batch"],
```

### Comparing `phlash-1.0.1/src/phlash/mp.py` & `phlash-1.0.2/src/phlash/mp.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/params.py` & `phlash-1.0.2/src/phlash/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         pattern: str,
         t1: float,
         tM: float,
         c: jax.Array,
         theta: float,
         rho: float,
         alpha: float = 0.0,
-        beta: float = 1e-3,
+        beta: float = 0.0,
     ) -> "MCMCParams":
         dtM = tM - t1
         t_tr = jnp.array([jnp.log(t1), jnp.log(dtM)])
         assert len(Pattern(pattern)) == len(c)  # one c per epoch
         rho_over_theta_tr = jsp.special.logit((rho / theta - 0.1) / 9.9)
         return cls(
             pattern=pattern,
```

### Comparing `phlash-1.0.1/src/phlash/plot.py` & `phlash-1.0.2/src/phlash/plot.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/sim.py` & `phlash-1.0.2/src/phlash/sim.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/src/phlash/size_history.py` & `phlash-1.0.2/src/phlash/size_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,23 @@
 
     def p_coal(self) -> np.ndarray:
         "returns the coalescence density at each time"
         Ci = -jnp.diff(self.surv())
         return jnp.concatenate([1.0 - Ci.sum(keepdims=True), Ci])
 
     def __call__(self, x: float, Ne: bool = False) -> float:
+        """Evaluate this function at the points x.
+
+        Args:
+            x: vector of points at which to evaluate eta.
+            Ne: If False, return eta(x). If True, return 1 / (2 * eta(x)).
+
+        Returns:
+            The function value at each point x.
+        """
         i = jnp.searchsorted(jnp.append(self.t, jnp.inf), x, "right") - 1
         if Ne:
             return 1.0 / 2.0 / self.c[i]
         return self.c[i]
         # return self.to_pp()(x)
 
     def density(self, c: float = 1.0) -> Callable[[float], float]:
```

### Comparing `phlash-1.0.1/src/phlash/transition.py` & `phlash-1.0.2/src/phlash/transition.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     ect = dm.eta.ect()
 
     t_aug = jnp.stack([dm.eta.t, dm.eta.ect()], 1).flatten()
     dt_aug = jnp.diff(t_aug)
     dt0 = jnp.isclose(dt_aug, 0.0)
     dt_safe = jnp.where(dt0, 1.0, dt_aug)
     cr = jnp.repeat(dm.eta.c, 2, axis=0)[:-1]
-    P = jax.vmap(_expQ, (0, 0, None))(dt_safe * dm.rho, dt_aug * cr, n)
+    P = jax.vmap(_expQ, (0, 0, None))(2 * dt_safe * dm.rho, dt_aug * cr, n)
     P = jnp.where(dt0[:, None, None], jnp.eye(3)[None], P)
     Pinf = jnp.array([[0.0, 0.0, 1.0]] * 3)
     P = jnp.concatenate([jnp.eye(3)[None], P, Pinf[None]], 0)
     Pcum = jax.lax.associative_scan(jnp.matmul, P)
 
     P_t = Pcum[::2]
     P_ect = Pcum[1::2]
```

### Comparing `phlash-1.0.1/src/phlash/util.py` & `phlash-1.0.2/src/phlash/util.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/.coverage` & `phlash-1.0.2/tests/.coverage`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/conftest.py` & `phlash-1.0.2/tests/conftest.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jax
 import numpy as np
 from pytest import fixture
 
-from phlash.gpu import PSMCKernel
+from phlash.kernel import get_kernel
 from phlash.params import PSMCParams
 from phlash.size_history import DemographicModel
 
 jax.config.update("jax_enable_x64", True)
 
 
 @fixture(params=[0, 1, 2])
@@ -27,8 +27,8 @@
 @fixture
 def pp(dm) -> PSMCParams:
     return PSMCParams.from_dm(dm)
 
 
 @fixture
 def kern(data):
-    return PSMCKernel(M=16, data=data, double_precision=True)
+    return get_kernel(M=16, data=data, double_precision=True)
```

### Comparing `phlash-1.0.1/tests/fixtures/elpd_bug.pkl` & `phlash-1.0.2/tests/fixtures/elpd_bug.pkl`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/fixtures/sample.bcf` & `phlash-1.0.2/tests/fixtures/sample.bcf`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/fixtures/tv_bug.pkl` & `phlash-1.0.2/tests/fixtures/tv_bug.pkl`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_afs.py` & `phlash-1.0.2/tests/test_afs.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_cband.py` & `phlash-1.0.2/tests/test_cband.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_gpu.py` & `phlash-1.0.2/tests/test_gpu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import jax
 import jax.test_util
 import numpy as np
 from pytest import fixture
 
+from phlash.hmm import psmc_ll
+from phlash.kernel import get_kernel
 from phlash.params import PSMCParams
 
 jax.config.update("jax_enable_x64", True)
 
 
 @fixture
-def data(rng):
-    U = rng.uniform(size=(128, 1_000))
-    data = (1 * (U < 0.01) + 2 * (U < 0.1) + 3 * (U < 0.2)).astype(np.int8)
-    # randomly insert some missing data
+def missing_data(data, rng):
     inds = rng.integers(0, data.size, size=int(0.01 * data.size))
     data.flat[inds] = -1
     return data.clip(-1, 1)
 
 
 def rel_err(a, b):
     return np.abs(a - b) / np.abs(a)
@@ -32,16 +31,26 @@
     "test that the likelihood is the same using either method"
     inds = np.arange(len(data))
     ll1, _ = kern(pp, inds, grad=True)
     ll2 = kern(pp, inds, grad=False)
     np.testing.assert_allclose(ll1, ll2)
 
 
-# def test_skip_missing(pp: PSMCParams, rng: np.random.Generator, kern_cls):
-#     U = rng.uniform(size=(100, 1000))
-#     data = (U < 0.01).astype(np.int8)
-#     # randomly insert some missing data
-#     data[50, -500:] = -1
-#     kern = kern_cls(M=pp.M, data=data, double_precision=True)
-#     assert np.all(kern._L_max[:50] == 1000)
-#     assert np.all(kern._L_max[51:] == 1000)
-#     assert kern._L_max[50] == 500
+def test_pyll_vs_cuda(dm, data, kern):
+    ll1 = kern.loglik(dm, 0)
+    ll2 = psmc_ll(dm, data[0])[1]
+    np.testing.assert_allclose(ll1, ll2, rtol=1e-4)
+
+
+def test_pyll_vs_cuda_missing(dm, missing_data):
+    kern = get_kernel(M=16, data=missing_data, double_precision=True)
+    ll1 = kern.loglik(dm, 0)
+    ll2 = psmc_ll(dm, missing_data[0])[1]
+    np.testing.assert_allclose(ll1, ll2, rtol=1e-4)
+
+
+def test_pyll_vg_vs_cuda(dm, data, kern):
+    ll1, dll1 = jax.value_and_grad(kern.loglik)(dm, 0)
+    ll2, dll2 = jax.value_and_grad(lambda dm: psmc_ll(dm, data[0])[1])(dm)
+    np.testing.assert_allclose(ll1, ll2, atol=1e-8, rtol=1e-5)
+    for x, y in zip(dll1, dll2):
+        np.testing.assert_allclose(x, y, atol=1e-8, rtol=1e-5)
```

### Comparing `phlash-1.0.1/tests/test_jax_ppoly.py` & `phlash-1.0.2/tests/test_jax_ppoly.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_model.py` & `phlash-1.0.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_sim.py` & `phlash-1.0.2/tests/test_sim.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_size_history.py` & `phlash-1.0.2/tests/test_size_history.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/tests/test_transition.py` & `phlash-1.0.2/tests/test_transition.py`

 * *Files identical despite different names*

### Comparing `phlash-1.0.1/PKG-INFO` & `phlash-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,91 @@
 Metadata-Version: 2.1
 Name: phlash
-Version: 1.0.1
+Version: 1.0.2
 Summary: Bayesian inference of population size history from recombining sequence data.
 Author-Email: Jonathan Terhorst <jonth@umich.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jthlab/phlash
 Project-URL: Bug reports, https://github.com/jthlab/phlash/issues
 Project-URL: Source, https://github.com/jthlab/phlash/
 Requires-Python: <4.0,>=3.10
 Requires-Dist: blackjax<2.0.0,>=1.1.0
 Requires-Dist: cuda-python<13,>=12.3
 Requires-Dist: cyvcf2<1.0.0,>=0.30.28
 Requires-Dist: intervaltree<4.0.0,>=3.1.0
-Requires-Dist: jax[cuda12_pip]>=0.4.24
+Requires-Dist: jax>=0.4.24
 Requires-Dist: loguru<1.0.0,>=0.7.2
 Requires-Dist: matplotlib<4.0.0,>=3.8.2
 Requires-Dist: msprime<2.0.0,>=1.3.0
-Requires-Dist: nvidia-cuda-nvrtc-cu12<13,>=12.3
 Requires-Dist: numpy<2.0.0,>=1.26.3
 Requires-Dist: optax<1.0.0,>=0.1.9
 Requires-Dist: plotly<6.0.0,>=5.18.0
 Requires-Dist: scipy<2.0.0,>=1.12.0
 Requires-Dist: stdpopsim<1.0.0,>=0.2.0
 Requires-Dist: tqdm<5.0.0,>=4.66.1
 Requires-Dist: tskit<1.0.0,>=0.5.6
 Requires-Dist: demes<1.0.0,>=0.2.3
 Requires-Dist: jax-dataclasses<2.0.0,>=1.6.0
 Requires-Dist: tszip<1.0.0,>=0.2.3
 Requires-Dist: jaxtyping<1.0.0,>=0.2.25
 Requires-Dist: pulp>=2.8.0
+Requires-Dist: dinopy>=3.0.0
 Requires-Dist: jupyter>=1.0.0; extra == "webui"
 Requires-Dist: notebook>=7.1.1; extra == "webui"
+Requires-Dist: jax[cuda12_pip]>=0.4.24; extra == "gpu"
+Requires-Dist: nvidia-cuda-nvrtc-cu12>=12.3; extra == "gpu"
 Provides-Extra: webui
+Provides-Extra: gpu
 Description-Content-Type: text/markdown
 
 phlash is a program for sampling from the posterior distribution of population size
 history given whole genome sequence data. You can think of it as a Bayesian version
 of Li & Durbin's popular [PSMC](https://github.com/lh3/psmc) program, with a more
 modern interface and GPU acceleration built in.
 
 ## Requirements
 
 - Python 3.10 or greater.
+
+Optional but _highly recommended_:
+
 - An NVIDIA GPU. Any relatively recent model should work. phlash has been tested on:
     - RTX 4090
     - A40
     - A100
     - V100
 
 ## Installation
 
-phlash can be installed from PyPI using pip, however the usual `pip install phlash`
-will fail because of dependence on CUDA and Jax packages which are not published on
-PyPI. Instead, you must run:
+phlash can be installed from PyPI using pip:
+
+```
+$ pip install phlash
+```
+
+If your machine contains an Nvidia GPU, you should install the `gpu` variant in order to enable it.
+In this case, you should run:
 
 ```
 $ pip install \
     -f "https://storage.googleapis.com/jax-releases/jax_cuda_releases.html" \
     --extra-index-url "https://pypi.ngc.nvidia.com" \
-    phlash
+    phlash[gpu]
 ```
 
 I recommend installing phlash into a separate virtual environment: before running the
 above, do
 
 ```
 $ python3 -mvenv /path/to/phlash  # replace with desired path
 $ source /path/to/phlash/bin/activate
 $ pip3 install -U pip setuptools  # recent version of pip and setuptools are required
 ```
+## Running the program
+See [notebooks/example.md](notebooks/example.md) for example code and usage instructions.
 
 ## Troubleshooting / FAQ
 
 I (Jonathan) am happy to assist you with using phlash, as much as my time allows.
 
 - If you encounter a **bug** (program crash or other unexpected behavior) please
 [file an issue](https://github.com/jthlab/phlash/issues/new) describing the bug.
```

