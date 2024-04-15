# Comparing `tmp/safetensors-0.4.2rc0.tar.gz` & `tmp/safetensors-0.4.3rc0.tar.gz`

## Comparing `safetensors-0.4.2rc0.tar` & `safetensors-0.4.3rc0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0     1001      127     1045 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/Cargo.toml
--rw-r--r--   0     1001      127    11357 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/LICENSE
--rw-r--r--   0     1001      127    10566 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/README.md
--rw-r--r--   0     1001      127     1701 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/benches/benchmark.rs
--rw-r--r--   0     1001      127      184 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/src/lib.rs
--rw-r--r--   0     1001      127    16641 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/src/slice.rs
--rw-r--r--   0     1001      127    41672 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/src/tensor.rs
--rw-r--r--   0     1001      127    10566 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/README.md
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 safetensors-0.4.2rc0/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      685 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/.gitignore
--rw-r--r--   0     1001      127      190 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/MANIFEST.in
--rw-r--r--   0     1001      127     1103 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/Makefile
--rw-r--r--   0     1001      127      852 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/README.md
--rw-r--r--   0     1001      127     2142 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_flax.py
--rw-r--r--   0     1001      127     2177 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_mlx.py
--rw-r--r--   0     1001      127     1968 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_paddle.py
--rw-r--r--   0     1001      127     4764 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_pt.py
--rw-r--r--   0     1001      127     2631 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_tf.py
--rw-r--r--   0     1001      127    14769 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/convert.py
--rw-r--r--   0     1001      127     1459 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/convert_all.py
--rw-r--r--   0     1001      127      729 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/fuzz.py
--rw-r--r--   0     1001      127      171 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/__init__.py
--rw-r--r--   0     1001      127     1970 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/__init__.pyi
--rw-r--r--   0     1001      127     3846 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/flax.py
--rw-r--r--   0     1001      127     3837 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/mlx.py
--rw-r--r--   0     1001      127     4937 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/numpy.py
--rw-r--r--   0     1001      127     4163 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/paddle.py
--rw-r--r--   0     1001      127        0 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/py.typed
--rw-r--r--   0     1001      127     3890 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/tensorflow.py
--rw-r--r--   0     1001      127    17294 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/torch.py
--rw-r--r--   0     1001      127      891 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/setup.cfg
--rw-r--r--   0     1001      127    39822 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     5370 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/stub.py
--rw-r--r--   0     1001      127        0 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/data/__init__.py
--rw-r--r--   0     1001      127     2337 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_flax_comparison.py
--rw-r--r--   0     1001      127     2010 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_mlx_comparison.py
--rw-r--r--   0     1001      127     1492 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_paddle_comparison.py
--rw-r--r--   0     1001      127    12107 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_pt_comparison.py
--rw-r--r--   0     1001      127    10195 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_pt_model.py
--rw-r--r--   0     1001      127     9151 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_simple.py
--rw-r--r--   0     1001      127     2841 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_tf_comparison.py
--rw-r--r--   0     1001      127     9094 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/Cargo.lock
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 safetensors-0.4.2rc0/pyproject.toml
--rw-r--r--   0     1001      127     3837 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/mlx.py
--rw-r--r--   0     1001      127     3846 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/flax.py
--rw-r--r--   0     1001      127     1970 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/__init__.pyi
--rw-r--r--   0     1001      127    17294 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/torch.py
--rw-r--r--   0     1001      127     4163 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/paddle.py
--rw-r--r--   0     1001      127      171 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/__init__.py
--rw-r--r--   0     1001      127     3890 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/tensorflow.py
--rw-r--r--   0     1001      127     4937 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/numpy.py
--rw-r--r--   0     1001      127        0 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/py.typed
--rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 safetensors-0.4.2rc0/PKG-INFO
+-rw-r--r--   0     1001      127     1044 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/Cargo.toml
+-rw-r--r--   0     1001      127    11357 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/LICENSE
+-rw-r--r--   0     1001      127    10566 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/README.md
+-rw-r--r--   0     1001      127     1701 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/benches/benchmark.rs
+-rw-r--r--   0     1001      127      184 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/src/lib.rs
+-rw-r--r--   0     1001      127    19437 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/src/slice.rs
+-rw-r--r--   0     1001      127    41672 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/safetensors/src/tensor.rs
+-rw-r--r--   0     1001      127    10566 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/README.md
+-rw-r--r--   0        0        0      422 1970-01-01 00:00:00.000000 safetensors-0.4.3rc0/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      685 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/.gitignore
+-rw-r--r--   0     1001      127      190 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/MANIFEST.in
+-rw-r--r--   0     1001      127     1103 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/Makefile
+-rw-r--r--   0     1001      127      852 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/README.md
+-rw-r--r--   0     1001      127     2142 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/benches/test_flax.py
+-rw-r--r--   0     1001      127     2177 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/benches/test_mlx.py
+-rw-r--r--   0     1001      127     1968 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/benches/test_paddle.py
+-rw-r--r--   0     1001      127     4764 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/benches/test_pt.py
+-rw-r--r--   0     1001      127     2631 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/benches/test_tf.py
+-rw-r--r--   0     1001      127    14769 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/convert.py
+-rw-r--r--   0     1001      127     1459 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/convert_all.py
+-rw-r--r--   0     1001      127      729 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/fuzz.py
+-rw-r--r--   0     1001      127      171 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/__init__.py
+-rw-r--r--   0     1001      127     1970 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/__init__.pyi
+-rw-r--r--   0     1001      127     3846 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/flax.py
+-rw-r--r--   0     1001      127     3837 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/mlx.py
+-rw-r--r--   0     1001      127     4937 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/numpy.py
+-rw-r--r--   0     1001      127     4175 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/paddle.py
+-rw-r--r--   0     1001      127        0 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/py.typed
+-rw-r--r--   0     1001      127     3890 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/tensorflow.py
+-rw-r--r--   0     1001      127    17582 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/py_src/safetensors/torch.py
+-rw-r--r--   0     1001      127      891 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/setup.cfg
+-rw-r--r--   0     1001      127    41526 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     5370 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/stub.py
+-rw-r--r--   0     1001      127        0 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/data/__init__.py
+-rw-r--r--   0     1001      127     2337 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_flax_comparison.py
+-rw-r--r--   0     1001      127     2010 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_mlx_comparison.py
+-rw-r--r--   0     1001      127     1492 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_paddle_comparison.py
+-rw-r--r--   0     1001      127    12107 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_pt_comparison.py
+-rw-r--r--   0     1001      127    10195 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_pt_model.py
+-rw-r--r--   0     1001      127    12484 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_simple.py
+-rw-r--r--   0     1001      127     2841 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/tests/test_tf_comparison.py
+-rw-r--r--   0     1001      127     9332 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/bindings/python/Cargo.lock
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 safetensors-0.4.3rc0/pyproject.toml
+-rw-r--r--   0     1001      127     3846 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/flax.py
+-rw-r--r--   0     1001      127      171 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/__init__.py
+-rw-r--r--   0     1001      127    17582 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/torch.py
+-rw-r--r--   0     1001      127     3837 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/mlx.py
+-rw-r--r--   0     1001      127        0 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/py.typed
+-rw-r--r--   0     1001      127     3890 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/tensorflow.py
+-rw-r--r--   0     1001      127     1970 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/__init__.pyi
+-rw-r--r--   0     1001      127     4175 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/paddle.py
+-rw-r--r--   0     1001      127     4937 2024-04-15 10:30:00.000000 safetensors-0.4.3rc0/py_src/safetensors/numpy.py
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 safetensors-0.4.3rc0/PKG-INFO
```

### Comparing `safetensors-0.4.2rc0/safetensors/Cargo.toml` & `safetensors-0.4.3rc0/safetensors/Cargo.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "safetensors"
-version = "0.4.2-rc.0"
+version = "0.4.3-rc0"
 edition = "2021"
 homepage = "https://github.com/huggingface/safetensors"
 repository = "https://github.com/huggingface/safetensors"
 documentation = "https://docs.rs/safetensors/"
 license = "Apache-2.0"
 keywords = ["safetensors", "huggingface", "Tensors", "Pytorch", "Tensorflow"]
 readme = "./README.md"
@@ -21,14 +21,14 @@
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 serde = {version = "1.0", features = ["derive"]}
 serde_json = "1.0"
 
 [dev-dependencies]
-criterion = "0.4"
-memmap2 = "0.5"
-proptest = "1.1"
+criterion = "0.5"
+memmap2 = "0.9"
+proptest = "1.4"
 
 [[bench]]
 name = "benchmark"
 harness = false
```

### Comparing `safetensors-0.4.2rc0/safetensors/LICENSE` & `safetensors-0.4.3rc0/safetensors/LICENSE`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/safetensors/README.md` & `safetensors-0.4.3rc0/safetensors/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/safetensors/benches/benchmark.rs` & `safetensors-0.4.3rc0/safetensors/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/safetensors/src/slice.rs` & `safetensors-0.4.3rc0/safetensors/src/slice.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,67 @@
 //! Module handling lazy loading via iterating on slices on the original buffer.
 use crate::tensor::TensorView;
+use std::fmt;
 use std::ops::{
     Bound, Range, RangeBounds, RangeFrom, RangeFull, RangeInclusive, RangeTo, RangeToInclusive,
 };
 
 /// Error representing invalid slicing attempt
 #[derive(Debug)]
 pub enum InvalidSlice {
     /// When the client asked for more slices than the tensors has dimensions
     TooManySlices,
+    /// When the client asked for a slice that exceeds the allowed bounds
+    SliceOutOfRange {
+        /// The rank of the dimension that has the out of bounds
+        dim_index: usize,
+        /// The problematic value
+        asked: usize,
+        /// The dimension size we shouldn't go over.
+        dim_size: usize,
+    },
 }
 
 #[derive(Debug, Clone)]
 /// Generic structure used to index a slice of the tensor
 pub enum TensorIndexer {
-    //Select(usize),
+    /// This is selecting an entire dimension
+    Select(usize),
     /// This is a regular slice, purely indexing a chunk of the tensor
     Narrow(Bound<usize>, Bound<usize>),
     //IndexSelect(Tensor),
 }
 
-// impl From<usize> for TensorIndexer {
-//     fn from(index: usize) -> Self {
-//         TensorIndexer::Select(index)
-//     }
-// }
+fn display_bound(bound: &Bound<usize>) -> String {
+    match bound {
+        Bound::Unbounded => "".to_string(),
+        Bound::Excluded(n) => format!("{n}"),
+        Bound::Included(n) => format!("{n}"),
+    }
+}
+
+/// Intended for Python users mostly or at least for its conventions
+impl fmt::Display for TensorIndexer {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        match self {
+            TensorIndexer::Select(n) => {
+                write!(f, "{n}")
+            }
+            TensorIndexer::Narrow(left, right) => {
+                write!(f, "{}:{}", display_bound(left), display_bound(right))
+            }
+        }
+    }
+}
+
+impl From<usize> for TensorIndexer {
+    fn from(index: usize) -> Self {
+        TensorIndexer::Select(index)
+    }
+}
 
 // impl From<&[usize]> for TensorIndexer {
 //     fn from(index: &[usize]) -> Self {
 //         let tensor = index.into();
 //         TensorIndexer::IndexSelect(tensor)
 //     }
 // }
@@ -245,16 +278,26 @@
                     TensorIndexer::Narrow(Bound::Excluded(s), Bound::Unbounded) => (*s + 1, shape),
                     TensorIndexer::Narrow(Bound::Excluded(s), Bound::Excluded(stop)) => {
                         (*s + 1, *stop)
                     }
                     TensorIndexer::Narrow(Bound::Excluded(s), Bound::Included(stop)) => {
                         (*s + 1, *stop + 1)
                     }
+                    TensorIndexer::Select(s) => (*s, *s + 1),
                 };
-                newshape.push(stop - start);
+                if start >= shape && stop > shape {
+                    return Err(InvalidSlice::SliceOutOfRange {
+                        dim_index: i,
+                        asked: stop.saturating_sub(1),
+                        dim_size: shape,
+                    });
+                }
+                if let TensorIndexer::Narrow(..) = slice {
+                    newshape.push(stop - start);
+                }
                 if indices.is_empty() {
                     if start == 0 && stop == shape {
                         // We haven't started to slice yet, just increase the span
                     } else {
                         let offset = start * span;
                         let small_span = stop * span - offset;
                         indices.push((offset, offset + small_span));
@@ -483,8 +526,51 @@
             ],
         )
         .unwrap();
         assert_eq!(iterator.next(), Some(&data[4..12]));
         assert_eq!(iterator.next(), Some(&data[16..24]));
         assert_eq!(iterator.next(), None);
     }
+
+    #[test]
+    fn test_slice_select() {
+        let data: Vec<u8> = vec![0.0f32, 1.0, 2.0, 3.0, 4.0, 5.0]
+            .into_iter()
+            .flat_map(|f| f.to_le_bytes())
+            .collect();
+
+        let attn_0 = TensorView::new(Dtype::F32, vec![2, 3], &data).unwrap();
+
+        let mut iterator = SliceIterator::new(
+            &attn_0,
+            &[
+                TensorIndexer::Select(1),
+                TensorIndexer::Narrow(Bound::Included(1), Bound::Excluded(3)),
+            ],
+        )
+        .unwrap();
+        assert_eq!(iterator.next(), Some(&data[16..24]));
+        assert_eq!(iterator.next(), None);
+
+        let mut iterator = SliceIterator::new(
+            &attn_0,
+            &[
+                TensorIndexer::Select(0),
+                TensorIndexer::Narrow(Bound::Included(1), Bound::Excluded(3)),
+            ],
+        )
+        .unwrap();
+        assert_eq!(iterator.next(), Some(&data[4..12]));
+        assert_eq!(iterator.next(), None);
+
+        let mut iterator = SliceIterator::new(
+            &attn_0,
+            &[
+                TensorIndexer::Narrow(Bound::Included(1), Bound::Excluded(2)),
+                TensorIndexer::Select(0),
+            ],
+        )
+        .unwrap();
+        assert_eq!(iterator.next(), Some(&data[12..16]));
+        assert_eq!(iterator.next(), None);
+    }
 }
```

### Comparing `safetensors-0.4.2rc0/safetensors/src/tensor.rs` & `safetensors-0.4.3rc0/safetensors/src/tensor.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/README.md` & `safetensors-0.4.3rc0/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/.gitignore` & `safetensors-0.4.3rc0/bindings/python/.gitignore`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/Makefile` & `safetensors-0.4.3rc0/bindings/python/Makefile`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/README.md` & `safetensors-0.4.3rc0/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/benches/test_flax.py` & `safetensors-0.4.3rc0/bindings/python/benches/test_flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/benches/test_mlx.py` & `safetensors-0.4.3rc0/bindings/python/benches/test_mlx.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/benches/test_paddle.py` & `safetensors-0.4.3rc0/bindings/python/benches/test_paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/benches/test_pt.py` & `safetensors-0.4.3rc0/bindings/python/benches/test_pt.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/benches/test_tf.py` & `safetensors-0.4.3rc0/bindings/python/benches/test_tf.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/convert.py` & `safetensors-0.4.3rc0/bindings/python/convert.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/convert_all.py` & `safetensors-0.4.3rc0/bindings/python/convert_all.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/fuzz.py` & `safetensors-0.4.3rc0/bindings/python/fuzz.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/__init__.pyi` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/flax.py` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/mlx.py` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/mlx.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/numpy.py` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/paddle.py` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/paddle.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 def load_file(filename: Union[str, os.PathLike], device="cpu") -> Dict[str, paddle.Tensor]:
     """
     Loads a safetensors file into paddle format.
 
     Args:
         filename (`str`, or `os.PathLike`)):
             The name of the file which contains the tensors
-        device (`Dict[str, any]`, *optional*, defaults to `cpu`):
+        device (`Union[Dict[str, any], str]`, *optional*, defaults to `cpu`):
             The device where the tensors need to be located after load.
             available options are all regular paddle device locations
 
     Returns:
         `Dict[str, paddle.Tensor]`: dictionary that contains name as key, value as `paddle.Tensor`
 
     Example:
```

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/tensorflow.py` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/torch.py` & `safetensors-0.4.3rc0/bindings/python/py_src/safetensors/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,36 +169,39 @@
         save_file(state_dict, filename, metadata=metadata)
     except ValueError as e:
         msg = str(e)
         msg += " Or use save_model(..., force_contiguous=True), read the docs for potential caveats."
         raise ValueError(msg)
 
 
-def load_model(model: torch.nn.Module, filename: Union[str, os.PathLike], strict=True) -> Tuple[List[str], List[str]]:
+def load_model(model: torch.nn.Module, filename: Union[str, os.PathLike], strict: bool = True, device: Union[str, int] = "cpu") -> Tuple[List[str], List[str]]:
     """
     Loads a given filename onto a torch model.
     This method exists specifically to avoid tensor sharing issues which are
     not allowed in `safetensors`. [More information on tensor sharing](../torch_shared_tensors)
 
     Args:
         model (`torch.nn.Module`):
             The model to load onto.
         filename (`str`, or `os.PathLike`):
             The filename location to load the file from.
         strict (`bool`, *optional*, defaults to True):
-            Wether to fail if you're missing keys or having unexpected ones
+            Whether to fail if you're missing keys or having unexpected ones.
             When false, the function simply returns missing and unexpected names.
+        device (`Union[str, int]`, *optional*, defaults to `cpu`):
+            The device where the tensors need to be located after load.
+            available options are all regular torch device locations.
 
     Returns:
         `(missing, unexpected): (List[str], List[str])`
             `missing` are names in the model which were not modified during loading
             `unexpected` are names that are on the file, but weren't used during
             the load.
     """
-    state_dict = load_file(filename)
+    state_dict = load_file(filename, device=device)
     model_state_dict = model.state_dict()
     to_removes = _remove_duplicate_names(model_state_dict, preferred_names=state_dict.keys())
     missing, unexpected = model.load_state_dict(state_dict, strict=False)
     missing = set(missing)
     for to_remove_group in to_removes.values():
         for to_remove in to_remove_group:
             if to_remove not in missing:
@@ -277,24 +280,24 @@
     tensors = {"embedding": torch.zeros((512, 1024)), "attention": torch.zeros((256, 256))}
     save_file(tensors, "model.safetensors")
     ```
     """
     serialize_file(_flatten(tensors), filename, metadata=metadata)
 
 
-def load_file(filename: Union[str, os.PathLike], device="cpu") -> Dict[str, torch.Tensor]:
+def load_file(filename: Union[str, os.PathLike], device: Union[str, int] = "cpu") -> Dict[str, torch.Tensor]:
     """
     Loads a safetensors file into torch format.
 
     Args:
         filename (`str`, or `os.PathLike`):
             The name of the file which contains the tensors
-        device (`Dict[str, any]`, *optional*, defaults to `cpu`):
+        device (`Union[str, int]`, *optional*, defaults to `cpu`):
             The device where the tensors need to be located after load.
-            available options are all regular torch device locations
+            available options are all regular torch device locations.
 
     Returns:
         `Dict[str, torch.Tensor]`: dictionary that contains name as key, value as `torch.Tensor`
 
     Example:
 
     ```python
```

### Comparing `safetensors-0.4.2rc0/bindings/python/setup.cfg` & `safetensors-0.4.3rc0/bindings/python/setup.cfg`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/src/lib.rs` & `safetensors-0.4.3rc0/bindings/python/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #![deny(missing_docs)]
 //! Dummy doc
 use memmap2::{Mmap, MmapOptions};
 use pyo3::exceptions::{PyException, PyFileNotFoundError};
-use pyo3::once_cell::GILOnceCell;
+use pyo3::sync::GILOnceCell;
 use pyo3::prelude::*;
 use pyo3::types::IntoPyDict;
 use pyo3::types::PySlice;
 use pyo3::types::{PyByteArray, PyBytes, PyDict, PyList};
 use pyo3::{intern, PyErr};
 use safetensors::slice::TensorIndexer;
 use safetensors::tensor::{Dtype, Metadata, SafeTensors, TensorInfo, TensorView};
 use std::collections::HashMap;
 use std::fs::File;
 use std::iter::FromIterator;
 use std::ops::Bound;
+use pyo3::{Bound as PyBound};
 use std::path::PathBuf;
 use std::sync::Arc;
 
 static TORCH_MODULE: GILOnceCell<Py<PyModule>> = GILOnceCell::new();
 static NUMPY_MODULE: GILOnceCell<Py<PyModule>> = GILOnceCell::new();
 static TENSORFLOW_MODULE: GILOnceCell<Py<PyModule>> = GILOnceCell::new();
 static FLAX_MODULE: GILOnceCell<Py<PyModule>> = GILOnceCell::new();
@@ -54,15 +55,15 @@
                         dtype_str => {
                             return Err(SafetensorError::new_err(format!(
                                 "dtype {dtype_str} is not covered",
                             )));
                         }
                     }
                 }
-                "data" => data = value.extract()?,
+                "data" => data = Some(value.extract::<&[u8]>()?),
                 _ => println!("Ignored unknown kwarg option {key}"),
             };
         }
         let shape = shape.ok_or_else(|| {
             SafetensorError::new_err(format!("Missing `shape` in {tensor_desc:?}"))
         })?;
         let dtype = dtype.ok_or_else(|| {
@@ -92,20 +93,20 @@
 ///         The serialized content.
 #[pyfunction]
 #[pyo3(text_signature = "(tensor_dict, metadata=None)")]
 fn serialize<'b>(
     py: Python<'b>,
     tensor_dict: HashMap<String, &PyDict>,
     metadata: Option<HashMap<String, String>>,
-) -> PyResult<&'b PyBytes> {
+) -> PyResult<PyBound<'b, PyBytes>> {
     let tensors = prepare(tensor_dict)?;
     let metadata_map = metadata.map(HashMap::from_iter);
     let out = safetensors::tensor::serialize(&tensors, &metadata_map)
         .map_err(|e| SafetensorError::new_err(format!("Error while serializing: {e:?}")))?;
-    let pybytes = PyBytes::new(py, &out);
+    let pybytes = PyBytes::new_bound(py, &out);
     Ok(pybytes)
 }
 
 /// Serializes raw data.
 ///
 /// Args:
 ///     tensor_dict (`Dict[str, Dict[Any]]`):
@@ -148,47 +149,64 @@
     let safetensor = SafeTensors::deserialize(bytes)
         .map_err(|e| SafetensorError::new_err(format!("Error while deserializing: {e:?}")))?;
 
     let tensors = safetensor.tensors();
     let mut items = Vec::with_capacity(tensors.len());
 
     for (tensor_name, tensor) in tensors {
-        let pyshape: PyObject = PyList::new(py, tensor.shape().iter()).into();
+        let pyshape: PyObject = PyList::new_bound(py, tensor.shape().iter()).into();
         let pydtype: PyObject = format!("{:?}", tensor.dtype()).into_py(py);
 
-        let pydata: PyObject = PyByteArray::new(py, tensor.data()).into();
+        let pydata: PyObject = PyByteArray::new_bound(py, tensor.data()).into();
 
         let map = HashMap::from([
             ("shape".to_string(), pyshape),
             ("dtype".to_string(), pydtype),
             ("data".to_string(), pydata),
         ]);
         items.push((tensor_name, map));
     }
     Ok(items)
 }
 
-fn slice_to_indexer(slice: &PySlice) -> Result<TensorIndexer, PyErr> {
-    let py_start = slice.getattr(intern!(slice.py(), "start"))?;
-    let start: Option<usize> = py_start.extract()?;
-    let start = if let Some(start) = start {
-        Bound::Included(start)
-    } else {
-        Bound::Unbounded
-    };
-
-    let py_stop = slice.getattr(intern!(slice.py(), "stop"))?;
-    let stop: Option<usize> = py_stop.extract()?;
-    let stop = if let Some(stop) = stop {
-        Bound::Excluded(stop)
-    } else {
-        Bound::Unbounded
-    };
+fn slice_to_indexer(
+    (dim_idx, (slice_index, dim)): (usize, (SliceIndex, usize)),
+) -> Result<TensorIndexer, PyErr> {
+    match slice_index {
+        SliceIndex::Slice(slice) => {
+            let py_start = slice.getattr(intern!(slice.py(), "start"))?;
+            let start: Option<usize> = py_start.extract()?;
+            let start = if let Some(start) = start {
+                Bound::Included(start)
+            } else {
+                Bound::Unbounded
+            };
 
-    Ok(TensorIndexer::Narrow(start, stop))
+            let py_stop = slice.getattr(intern!(slice.py(), "stop"))?;
+            let stop: Option<usize> = py_stop.extract()?;
+            let stop = if let Some(stop) = stop {
+                Bound::Excluded(stop)
+            } else {
+                Bound::Unbounded
+            };
+            Ok(TensorIndexer::Narrow(start, stop))
+        }
+        SliceIndex::Index(idx) => {
+            if idx < 0 {
+                let idx = dim
+                    .checked_add_signed(idx as isize)
+                    .ok_or(SafetensorError::new_err(format!(
+                        "Invalid index {idx} for dimension {dim_idx} of size {dim}"
+                    )))?;
+                Ok(TensorIndexer::Select(idx))
+            } else {
+                Ok(TensorIndexer::Select(idx as usize))
+            }
+        }
+    }
 }
 
 #[derive(Debug, Clone, PartialEq, Eq)]
 enum Framework {
     Pytorch,
     Numpy,
     Tensorflow,
@@ -376,19 +394,19 @@
         })?;
 
         let offset = n + 8;
 
         Python::with_gil(|py| -> PyResult<()> {
             match framework {
                 Framework::Pytorch => {
-                    let module = PyModule::import(py, intern!(py, "torch"))?;
+                    let module = PyModule::import_bound(py, intern!(py, "torch"))?;
                     TORCH_MODULE.get_or_init(py, || module.into())
                 }
                 _ => {
-                    let module = PyModule::import(py, intern!(py, "numpy"))?;
+                    let module = PyModule::import_bound(py, intern!(py, "numpy"))?;
                     NUMPY_MODULE.get_or_init(py, || module.into())
                 }
             };
 
             Ok(())
         })?;
 
@@ -409,21 +427,21 @@
                     let (size_name, storage_name) = if version >= Version::new(2, 0, 0) {
                         (intern!(py, "nbytes"), intern!(py, "UntypedStorage"))
                     } else {
                         (intern!(py, "size"), intern!(py, "ByteStorage"))
                     };
 
                     let kwargs =
-                        [(intern!(py, "shared"), shared), (size_name, size)].into_py_dict(py);
+                        [(intern!(py, "shared"), shared), (size_name, size)].into_py_dict_bound(py);
                     let storage = module
                         .getattr(storage_name)?
-                        .getattr(intern!(py, "from_file"))?
-                        .call((py_filename,), Some(kwargs))?;
+                        // .getattr(intern!(py, "from_file"))?
+                        .call_method("from_file", (py_filename,), Some(&kwargs))?;
 
-                    let untyped: &PyAny = match storage.getattr(intern!(py, "untyped")) {
+                    let untyped: PyBound<'_, PyAny> = match storage.getattr(intern!(py, "untyped")) {
                         Ok(untyped) => untyped,
                         Err(_) => storage.getattr(intern!(py, "_untyped"))?,
                     };
                     let storage = untyped.call0()?.into_py(py);
                     let gil_storage = GILOnceCell::new();
                     gil_storage.get_or_init(py, || storage);
 
@@ -493,88 +511,87 @@
         // })?;
 
         match &self.storage.as_ref() {
             Storage::Mmap(mmap) => {
                 let data =
                     &mmap[info.data_offsets.0 + self.offset..info.data_offsets.1 + self.offset];
 
-                let array: PyObject = Python::with_gil(|py| PyByteArray::new(py, data).into_py(py));
+                let array: PyObject = Python::with_gil(|py| PyByteArray::new_bound(py, data).into_py(py));
 
                 create_tensor(
                     &self.framework,
                     info.dtype,
                     &info.shape,
                     array,
                     &self.device,
                 )
             }
             Storage::TorchStorage(storage) => {
                 Python::with_gil(|py| -> PyResult<PyObject> {
                     let torch = get_module(py, &TORCH_MODULE)?;
                     let dtype: PyObject = get_pydtype(torch, info.dtype, false)?;
                     let torch_uint8: PyObject = get_pydtype(torch, Dtype::U8, false)?;
-                    let kwargs = [(intern!(py, "dtype"), torch_uint8)].into_py_dict(py);
-                    let view_kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict(py);
+                    let kwargs = [(intern!(py, "dtype"), torch_uint8)].into_py_dict_bound(py);
+                    let view_kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict_bound(py);
                     let shape = info.shape.to_vec();
                     let shape: PyObject = shape.into_py(py);
 
                     let start = (info.data_offsets.0 + self.offset) as isize;
                     let stop = (info.data_offsets.1 + self.offset) as isize;
-                    let slice = PySlice::new(py, start, stop, 1);
+                    let slice = PySlice::new_bound(py, start, stop, 1);
                     let storage: &PyObject = storage
                         .get(py)
                         .ok_or_else(|| SafetensorError::new_err("Could not find storage"))?;
-                    let storage: &PyAny = storage.as_ref(py);
+                    let storage: &PyBound<PyAny> = storage.bind(py);
                     let storage_slice = storage
                         .getattr(intern!(py, "__getitem__"))?
                         .call1((slice,))?;
 
-                    let sys = PyModule::import(py, intern!(py, "sys"))?;
+                    let sys = PyModule::import_bound(py, intern!(py, "sys"))?;
                     let byteorder: String = sys.getattr(intern!(py, "byteorder"))?.extract()?;
 
                     let mut tensor = torch
                         .getattr(intern!(py, "asarray"))?
-                        .call((storage_slice,), Some(kwargs))?
+                        .call((storage_slice,), Some(&kwargs))?
                         .getattr(intern!(py, "view"))?
-                        .call((), Some(view_kwargs))?;
+                        .call((), Some(&view_kwargs))?;
 
                     if byteorder == "big" {
                         let inplace_kwargs =
-                            [(intern!(py, "inplace"), false.into_py(py))].into_py_dict(py);
+                            [(intern!(py, "inplace"), false.into_py(py))].into_py_dict_bound(py);
                         if info.dtype == Dtype::BF16 {
                             let torch_f16: PyObject = get_pydtype(torch, Dtype::F16, false)?;
                             tensor = tensor.getattr(intern!(py, "to"))?.call(
                                 (),
-                                Some([(intern!(py, "dtype"), torch_f16)].into_py_dict(py)),
+                                Some(&[(intern!(py, "dtype"), torch_f16)].into_py_dict_bound(py)),
                             )?;
                         }
 
                         let numpy = tensor
                             .getattr(intern!(py, "numpy"))?
                             .call0()?
                             .getattr("byteswap")?
-                            .call((), Some(inplace_kwargs))?;
+                            .call((), Some(&inplace_kwargs))?;
                         tensor = torch.getattr(intern!(py, "from_numpy"))?.call1((numpy,))?;
 
                         if info.dtype == Dtype::BF16 {
                             let torch_bf16: PyObject = get_pydtype(torch, Dtype::BF16, false)?;
                             tensor = tensor.getattr(intern!(py, "to"))?.call(
                                 (),
-                                Some([(intern!(py, "dtype"), torch_bf16)].into_py_dict(py)),
+                                Some(&[(intern!(py, "dtype"), torch_bf16)].into_py_dict_bound(py)),
                             )?;
                         }
                     }
 
                     tensor = tensor.getattr(intern!(py, "reshape"))?.call1((shape,))?;
                     if self.device != Device::Cpu {
                         let device: PyObject = self.device.clone().into_py(py);
-                        let kwargs = PyDict::new(py);
+                        let kwargs = PyDict::new_bound(py);
                         tensor = tensor
-                            .getattr(intern!(py, "to"))?
-                            .call((device,), Some(kwargs))?;
+                            .call_method("to", (device,), Some(&kwargs))?;
                     }
                     Ok(tensor.into_py(py))
                     // torch.asarray(storage[start + n : stop + n], dtype=torch.uint8).view(dtype=dtype).reshape(shape)
                 })
             }
         }
     }
@@ -726,18 +743,38 @@
     framework: Framework,
     offset: usize,
     device: Device,
     storage: Arc<Storage>,
 }
 
 #[derive(FromPyObject)]
-enum Slice<'a> {
-    // Index(usize),
+enum SliceIndex<'a> {
     Slice(&'a PySlice),
-    Slices(Vec<&'a PySlice>),
+    Index(i32),
+}
+
+#[derive(FromPyObject)]
+enum Slice<'a> {
+    Slice(SliceIndex<'a>),
+    Slices(Vec<SliceIndex<'a>>),
+}
+
+use std::fmt;
+struct Disp(Vec<TensorIndexer>);
+
+/// Should be more readable that the standard
+/// `Debug`
+impl fmt::Display for Disp {
+    fn fmt(&self, f: &mut fmt::Formatter<'_>) -> fmt::Result {
+        write!(f, "[")?;
+        for item in &self.0 {
+            write!(f, "{item}")?;
+        }
+        write!(f, "]")
+    }
 }
 
 #[pymethods]
 impl PySafeSlice {
     /// Returns the shape of the full underlying tensor
     ///
     /// Returns:
@@ -776,48 +813,53 @@
     /// ```
     pub fn get_dtype(&self, py: Python) -> PyResult<PyObject> {
         let dtype = self.info.dtype;
         let dtype: PyObject = format!("{:?}", dtype).into_py(py);
         Ok(dtype)
     }
 
-    pub fn __getitem__(&self, slices: Slice) -> PyResult<PyObject> {
-        let slices: Vec<&PySlice> = match slices {
-            Slice::Slice(slice) => vec![slice],
-            Slice::Slices(slices) => slices,
-        };
-
+    pub fn __getitem__(&self, slices: &PyBound<'_, PyAny>) -> PyResult<PyObject> {
         match &self.storage.as_ref() {
             Storage::Mmap(mmap) => {
+                let slices: Slice = slices.extract()?;
+                let slices: Vec<SliceIndex> = match slices {
+                    Slice::Slice(slice) => vec![slice],
+                    Slice::Slices(slices) => slices,
+                };
                 let data = &mmap[self.info.data_offsets.0 + self.offset
                     ..self.info.data_offsets.1 + self.offset];
 
+                let shape = self.info.shape.clone();
+
                 let tensor = TensorView::new(self.info.dtype, self.info.shape.clone(), data)
                     .map_err(|e| {
                         SafetensorError::new_err(format!("Error preparing tensor view: {e:?}"))
                     })?;
                 let slices: Vec<TensorIndexer> = slices
                     .into_iter()
+                    .zip(shape)
+                    .enumerate()
                     .map(slice_to_indexer)
                     .collect::<Result<_, _>>()?;
 
                 let iterator = tensor.sliced_data(&slices).map_err(|e| {
                     SafetensorError::new_err(format!(
-                        "Error during slicing {slices:?} vs {:?}:  {:?}",
-                        self.info.shape, e
+                        "Error during slicing {} with shape {:?}:  {:?}",
+                        Disp(slices),
+                        self.info.shape,
+                        e
                     ))
                 })?;
                 let newshape = iterator.newshape();
 
                 let mut offset = 0;
                 let length = iterator.remaining_byte_len();
-
                 Python::with_gil(|py| {
                     let array: PyObject =
-                        PyByteArray::new_with(py, length, |bytes: &mut [u8]| {
+                        PyByteArray::new_bound_with(py, length, |bytes: &mut [u8]| {
                             for slice in iterator {
                                 let len = slice.len();
                                 bytes[offset..offset + slice.len()].copy_from_slice(slice);
                                 offset += len;
                             }
                             Ok(())
                         })?
@@ -831,181 +873,179 @@
                     )
                 })
             }
             Storage::TorchStorage(storage) => Python::with_gil(|py| -> PyResult<PyObject> {
                 let torch = get_module(py, &TORCH_MODULE)?;
                 let dtype: PyObject = get_pydtype(torch, self.info.dtype, false)?;
                 let torch_uint8: PyObject = get_pydtype(torch, Dtype::U8, false)?;
-                let kwargs = [(intern!(py, "dtype"), torch_uint8)].into_py_dict(py);
-                let view_kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict(py);
+                let kwargs = [(intern!(py, "dtype"), torch_uint8)].into_py_dict_bound(py);
+                let view_kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict_bound(py);
                 let shape = self.info.shape.to_vec();
                 let shape: PyObject = shape.into_py(py);
 
                 let start = (self.info.data_offsets.0 + self.offset) as isize;
                 let stop = (self.info.data_offsets.1 + self.offset) as isize;
-                let slice = PySlice::new(py, start, stop, 1);
+                let slice = PySlice::new_bound(py, start, stop, 1);
                 let storage: &PyObject = storage
                     .get(py)
                     .ok_or_else(|| SafetensorError::new_err("Could not find storage"))?;
-                let storage: &PyAny = storage.as_ref(py);
+                let storage: &PyBound<'_, PyAny> = storage.bind(py);
 
                 let storage_slice = storage
                     .getattr(intern!(py, "__getitem__"))?
                     .call1((slice,))?;
 
                 let slices = slices.into_py(py);
 
-                let sys = PyModule::import(py, intern!(py, "sys"))?;
+                let sys = PyModule::import_bound(py, intern!(py, "sys"))?;
                 let byteorder: String = sys.getattr(intern!(py, "byteorder"))?.extract()?;
 
                 let mut tensor = torch
                     .getattr(intern!(py, "asarray"))?
-                    .call((storage_slice,), Some(kwargs))?
+                    .call((storage_slice,), Some(&kwargs))?
                     .getattr(intern!(py, "view"))?
-                    .call((), Some(view_kwargs))?;
+                    .call((), Some(&view_kwargs))?;
                 if byteorder == "big" {
                     let inplace_kwargs =
-                        [(intern!(py, "inplace"), false.into_py(py))].into_py_dict(py);
+                        [(intern!(py, "inplace"), false.into_py(py))].into_py_dict_bound(py);
 
                     let numpy = tensor
                         .getattr(intern!(py, "numpy"))?
                         .call0()?
                         .getattr("byteswap")?
-                        .call((), Some(inplace_kwargs))?;
+                        .call((), Some(&inplace_kwargs))?;
                     tensor = torch.getattr(intern!(py, "from_numpy"))?.call1((numpy,))?;
                 }
                 tensor = tensor
                     .getattr(intern!(py, "reshape"))?
                     .call1((shape,))?
                     .getattr(intern!(py, "__getitem__"))?
                     .call1((slices,))?;
                 if self.device != Device::Cpu {
                     let device: PyObject = self.device.clone().into_py(py);
-                    let kwargs = PyDict::new(py);
+                    let kwargs = PyDict::new_bound(py);
                     tensor = tensor
-                        .getattr(intern!(py, "to"))?
-                        .call((device,), Some(kwargs))?;
+                        .call_method("to", (device,), Some(&kwargs))?;
                 }
                 Ok(tensor.into_py(py))
             }),
         }
     }
 }
 
 fn get_module<'a>(
     py: Python<'a>,
     cell: &'static GILOnceCell<Py<PyModule>>,
-) -> PyResult<&'a PyModule> {
-    let module: &PyModule = cell
+) -> PyResult<&'a PyBound<'a, PyModule>> {
+    let module: &PyBound<'a, PyModule> = cell
         .get(py)
         .ok_or_else(|| SafetensorError::new_err("Could not find module"))?
-        .as_ref(py);
+        .bind(py);
     Ok(module)
 }
 
-fn create_tensor(
-    framework: &Framework,
+fn create_tensor<'a>(
+    framework: &'a Framework,
     dtype: Dtype,
-    shape: &[usize],
+    shape: &'a [usize],
     array: PyObject,
-    device: &Device,
+    device: &'a Device,
 ) -> PyResult<PyObject> {
     Python::with_gil(|py| -> PyResult<PyObject> {
-        let (module, is_numpy): (&PyModule, bool) = match framework {
+        let (module, is_numpy): (&PyBound<'_, PyModule>, bool) = match framework {
             Framework::Pytorch => (
                 TORCH_MODULE
                     .get(py)
                     .ok_or_else(|| {
                         SafetensorError::new_err(format!("Could not find module {framework:?}",))
                     })?
-                    .as_ref(py),
+                    .bind(py),
                 false,
             ),
             _ => (
                 NUMPY_MODULE
                     .get(py)
                     .ok_or_else(|| {
                         SafetensorError::new_err(format!("Could not find module {framework:?}",))
                     })?
-                    .as_ref(py),
+                    .bind(py),
                 true,
             ),
         };
         let dtype: PyObject = get_pydtype(module, dtype, is_numpy)?;
         let count: usize = shape.iter().product();
         let shape = shape.to_vec();
         let shape: PyObject = shape.into_py(py);
         let tensor = if count == 0 {
             // Torch==1.10 does not allow frombuffer on empty buffers so we create
             // the tensor manually.
-            let zeros = module.getattr(intern!(py, "zeros"))?;
+            // let zeros = module.getattr(intern!(py, "zeros"))?;
             let args = (shape.clone(),);
-            let kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict(py);
-            zeros.call(args, Some(kwargs))?
+            let kwargs = [(intern!(py, "dtype"), dtype)].into_py_dict_bound(py);
+            module.call_method("zeros", args, Some(&kwargs))?
         } else {
-            let frombuffer = module.getattr(intern!(py, "frombuffer"))?;
+            // let frombuffer = module.getattr(intern!(py, "frombuffer"))?;
             let kwargs = [
                 (intern!(py, "buffer"), array),
                 (intern!(py, "dtype"), dtype),
             ]
-            .into_py_dict(py);
-            frombuffer.call((), Some(kwargs))?
+            .into_py_dict_bound(py);
+            module.call_method("frombuffer", (), Some(&kwargs))?
         };
-        let mut tensor: &PyAny = tensor.getattr(intern!(py, "reshape"))?.call1((shape,))?;
+        let mut tensor: PyBound<'_, PyAny> = tensor.call_method1("reshape", (shape,))?;
         let tensor = match framework {
             Framework::Flax => {
                 let module = Python::with_gil(|py| -> PyResult<&Py<PyModule>> {
-                    let module = PyModule::import(py, intern!(py, "jax"))?;
+                    let module = PyModule::import_bound(py, intern!(py, "jax"))?;
                     Ok(FLAX_MODULE.get_or_init(py, || module.into()))
                 })?
-                .as_ref(py);
+                .bind(py);
                 module
                     .getattr(intern!(py, "numpy"))?
                     .getattr(intern!(py, "array"))?
                     .call1((tensor,))?
             }
             Framework::Tensorflow => {
                 let module = Python::with_gil(|py| -> PyResult<&Py<PyModule>> {
-                    let module = PyModule::import(py, intern!(py, "tensorflow"))?;
+                    let module = PyModule::import_bound(py, intern!(py, "tensorflow"))?;
                     Ok(TENSORFLOW_MODULE.get_or_init(py, || module.into()))
                 })?
-                .as_ref(py);
+                .bind(py);
                 module
                     .getattr(intern!(py, "convert_to_tensor"))?
                     .call1((tensor,))?
             }
             Framework::Mlx => {
                 let module = Python::with_gil(|py| -> PyResult<&Py<PyModule>> {
-                    let module = PyModule::import(py, intern!(py, "mlx"))?;
+                    let module = PyModule::import_bound(py, intern!(py, "mlx"))?;
                     Ok(MLX_MODULE.get_or_init(py, || module.into()))
                 })?
-                .as_ref(py);
+                .bind(py);
                 module
                     .getattr(intern!(py, "core"))?
-                    .getattr(intern!(py, "array"))?
-                    .call1((tensor,))?
+                    // .getattr(intern!(py, "array"))?
+                    .call_method1("array", (tensor,))?
             }
             Framework::Pytorch => {
                 if device != &Device::Cpu {
                     let device: PyObject = device.clone().into_py(py);
-                    let kwargs = PyDict::new(py);
+                    let kwargs = PyDict::new_bound(py);
                     tensor = tensor
-                        .getattr(intern!(py, "to"))?
-                        .call((device,), Some(kwargs))?;
+                        .call_method("to", (device,), Some(&kwargs))?;
                 }
                 tensor
             }
             Framework::Numpy => tensor,
         };
-        let tensor = tensor.into_py(py);
-        Ok(tensor)
+        // let tensor = tensor.into_py_bound(py);
+        Ok(tensor.into_py(py))
     })
 }
 
-fn get_pydtype(module: &PyModule, dtype: Dtype, is_numpy: bool) -> PyResult<PyObject> {
+fn get_pydtype(module: &PyBound<'_, PyModule>, dtype: Dtype, is_numpy: bool) -> PyResult<PyObject> {
     Python::with_gil(|py| {
         let dtype: PyObject = match dtype {
             Dtype::F64 => module.getattr(intern!(py, "float64"))?.into(),
             Dtype::F32 => module.getattr(intern!(py, "float32"))?.into(),
             Dtype::BF16 => {
                 if is_numpy {
                     module
@@ -1023,15 +1063,15 @@
             Dtype::I32 => module.getattr(intern!(py, "int32"))?.into(),
             Dtype::U16 => module.getattr(intern!(py, "uint16"))?.into(),
             Dtype::I16 => module.getattr(intern!(py, "int16"))?.into(),
             Dtype::U8 => module.getattr(intern!(py, "uint8"))?.into(),
             Dtype::I8 => module.getattr(intern!(py, "int8"))?.into(),
             Dtype::BOOL => {
                 if is_numpy {
-                    py.import("builtins")?.getattr(intern!(py, "bool"))?.into()
+                    py.import_bound("builtins")?.getattr(intern!(py, "bool"))?.into()
                 } else {
                     module.getattr(intern!(py, "bool"))?.into()
                 }
             }
             Dtype::F8_E4M3 => module.getattr(intern!(py, "float8_e4m3fn"))?.into(),
             Dtype::F8_E5M2 => module.getattr(intern!(py, "float8_e5m2"))?.into(),
             dtype => {
@@ -1049,20 +1089,20 @@
     SafetensorError,
     PyException,
     "Custom Python Exception for Safetensor errors."
 );
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn _safetensors_rust(py: Python, m: &PyModule) -> PyResult<()> {
+fn _safetensors_rust(m: &PyBound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(serialize, m)?)?;
     m.add_function(wrap_pyfunction!(serialize_file, m)?)?;
     m.add_function(wrap_pyfunction!(deserialize, m)?)?;
     m.add_class::<safe_open>()?;
-    m.add("SafetensorError", py.get_type::<SafetensorError>())?;
+    m.add("SafetensorError", m.py().get_type_bound::<SafetensorError>())?;
     m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
```

### Comparing `safetensors-0.4.2rc0/bindings/python/stub.py` & `safetensors-0.4.3rc0/bindings/python/stub.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/tests/test_flax_comparison.py` & `safetensors-0.4.3rc0/bindings/python/tests/test_flax_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/tests/test_mlx_comparison.py` & `safetensors-0.4.3rc0/bindings/python/tests/test_mlx_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/tests/test_paddle_comparison.py` & `safetensors-0.4.3rc0/bindings/python/tests/test_paddle_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/tests/test_pt_comparison.py` & `safetensors-0.4.3rc0/bindings/python/tests/test_pt_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/tests/test_pt_model.py` & `safetensors-0.4.3rc0/bindings/python/tests/test_pt_model.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/tests/test_tf_comparison.py` & `safetensors-0.4.3rc0/bindings/python/tests/test_tf_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/bindings/python/Cargo.lock` & `safetensors-0.4.3rc0/bindings/python/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -24,54 +24,54 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "libc"
-version = "0.2.151"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memmap2"
-version = "0.5.10"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
+checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -98,88 +98,96 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.75"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "907a61bd0f64c2f29cd1cf1dc34d05176426a3f504a78010f08416ddb7b13708"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
@@ -187,29 +195,29 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "safetensors"
-version = "0.4.2-rc.0"
+version = "0.4.3-rc0"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "safetensors-python"
-version = "0.4.2-rc.0"
+version = "0.4.3-rc0"
 dependencies = [
  "memmap2",
  "pyo3",
  "safetensors",
  "serde_json",
 ]
 
@@ -217,65 +225,65 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.194"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b114498256798c94a0689e1a15fec6005dee8ac1f41de56404b67afc2a4b773"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.194"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a3385e45322e8f9931410f01b3031ec534c3947d0e94c18049af4d9f9907d4e0"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.111"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176e46fa42316f18edd598015a5166857fc835ec732f5215eac6b7bdbf0a84f4"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.47"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1726efe18f42ae774cc644f330953a5e7b3c3003d3edcecf18850fe9d4dd9afb"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
```

### Comparing `safetensors-0.4.2rc0/pyproject.toml` & `safetensors-0.4.3rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/mlx.py` & `safetensors-0.4.3rc0/py_src/safetensors/mlx.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/flax.py` & `safetensors-0.4.3rc0/py_src/safetensors/flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/__init__.pyi` & `safetensors-0.4.3rc0/py_src/safetensors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/torch.py` & `safetensors-0.4.3rc0/py_src/safetensors/torch.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,36 +169,39 @@
         save_file(state_dict, filename, metadata=metadata)
     except ValueError as e:
         msg = str(e)
         msg += " Or use save_model(..., force_contiguous=True), read the docs for potential caveats."
         raise ValueError(msg)
 
 
-def load_model(model: torch.nn.Module, filename: Union[str, os.PathLike], strict=True) -> Tuple[List[str], List[str]]:
+def load_model(model: torch.nn.Module, filename: Union[str, os.PathLike], strict: bool = True, device: Union[str, int] = "cpu") -> Tuple[List[str], List[str]]:
     """
     Loads a given filename onto a torch model.
     This method exists specifically to avoid tensor sharing issues which are
     not allowed in `safetensors`. [More information on tensor sharing](../torch_shared_tensors)
 
     Args:
         model (`torch.nn.Module`):
             The model to load onto.
         filename (`str`, or `os.PathLike`):
             The filename location to load the file from.
         strict (`bool`, *optional*, defaults to True):
-            Wether to fail if you're missing keys or having unexpected ones
+            Whether to fail if you're missing keys or having unexpected ones.
             When false, the function simply returns missing and unexpected names.
+        device (`Union[str, int]`, *optional*, defaults to `cpu`):
+            The device where the tensors need to be located after load.
+            available options are all regular torch device locations.
 
     Returns:
         `(missing, unexpected): (List[str], List[str])`
             `missing` are names in the model which were not modified during loading
             `unexpected` are names that are on the file, but weren't used during
             the load.
     """
-    state_dict = load_file(filename)
+    state_dict = load_file(filename, device=device)
     model_state_dict = model.state_dict()
     to_removes = _remove_duplicate_names(model_state_dict, preferred_names=state_dict.keys())
     missing, unexpected = model.load_state_dict(state_dict, strict=False)
     missing = set(missing)
     for to_remove_group in to_removes.values():
         for to_remove in to_remove_group:
             if to_remove not in missing:
@@ -277,24 +280,24 @@
     tensors = {"embedding": torch.zeros((512, 1024)), "attention": torch.zeros((256, 256))}
     save_file(tensors, "model.safetensors")
     ```
     """
     serialize_file(_flatten(tensors), filename, metadata=metadata)
 
 
-def load_file(filename: Union[str, os.PathLike], device="cpu") -> Dict[str, torch.Tensor]:
+def load_file(filename: Union[str, os.PathLike], device: Union[str, int] = "cpu") -> Dict[str, torch.Tensor]:
     """
     Loads a safetensors file into torch format.
 
     Args:
         filename (`str`, or `os.PathLike`):
             The name of the file which contains the tensors
-        device (`Dict[str, any]`, *optional*, defaults to `cpu`):
+        device (`Union[str, int]`, *optional*, defaults to `cpu`):
             The device where the tensors need to be located after load.
-            available options are all regular torch device locations
+            available options are all regular torch device locations.
 
     Returns:
         `Dict[str, torch.Tensor]`: dictionary that contains name as key, value as `torch.Tensor`
 
     Example:
 
     ```python
```

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/paddle.py` & `safetensors-0.4.3rc0/py_src/safetensors/paddle.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 def load_file(filename: Union[str, os.PathLike], device="cpu") -> Dict[str, paddle.Tensor]:
     """
     Loads a safetensors file into paddle format.
 
     Args:
         filename (`str`, or `os.PathLike`)):
             The name of the file which contains the tensors
-        device (`Dict[str, any]`, *optional*, defaults to `cpu`):
+        device (`Union[Dict[str, any], str]`, *optional*, defaults to `cpu`):
             The device where the tensors need to be located after load.
             available options are all regular paddle device locations
 
     Returns:
         `Dict[str, paddle.Tensor]`: dictionary that contains name as key, value as `paddle.Tensor`
 
     Example:
```

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/tensorflow.py` & `safetensors-0.4.3rc0/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/py_src/safetensors/numpy.py` & `safetensors-0.4.3rc0/py_src/safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2rc0/PKG-INFO` & `safetensors-0.4.3rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: safetensors
-Version: 0.4.2rc0
+Version: 0.4.3rc0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -30,16 +30,16 @@
 Requires-Dist: paddlepaddle >=2.4.1 ; extra == 'paddlepaddle'
 Requires-Dist: black ==22.3 ; extra == 'quality'
 Requires-Dist: click ==8.0.4 ; extra == 'quality'
 Requires-Dist: isort >=5.5.4 ; extra == 'quality'
 Requires-Dist: flake8 >=3.8.3 ; extra == 'quality'
 Requires-Dist: safetensors[numpy] ; extra == 'testing'
 Requires-Dist: h5py >=3.7.0 ; extra == 'testing'
-Requires-Dist: huggingface_hub >=0.12.1 ; extra == 'testing'
-Requires-Dist: setuptools_rust >=1.5.2 ; extra == 'testing'
+Requires-Dist: huggingface-hub >=0.12.1 ; extra == 'testing'
+Requires-Dist: setuptools-rust >=1.5.2 ; extra == 'testing'
 Requires-Dist: pytest >=7.2.0 ; extra == 'testing'
 Requires-Dist: pytest-benchmark >=4.0.0 ; extra == 'testing'
 Requires-Dist: hypothesis >=6.70.2 ; extra == 'testing'
 Requires-Dist: safetensors[torch] ; extra == 'all'
 Requires-Dist: safetensors[numpy] ; extra == 'all'
 Requires-Dist: safetensors[pinned-tf] ; extra == 'all'
 Requires-Dist: safetensors[jax] ; extra == 'all'
```

