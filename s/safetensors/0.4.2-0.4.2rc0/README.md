# Comparing `tmp/safetensors-0.4.2.tar.gz` & `tmp/safetensors-0.4.2rc0.tar.gz`

## Comparing `safetensors-0.4.2.tar` & `safetensors-0.4.2rc0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0     1001      127     1040 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/Cargo.toml
--rw-r--r--   0     1001      127    11357 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/LICENSE
--rw-r--r--   0     1001      127    10566 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/README.md
--rw-r--r--   0     1001      127     1701 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/benches/benchmark.rs
--rw-r--r--   0     1001      127      184 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/src/lib.rs
--rw-r--r--   0     1001      127    16641 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/src/slice.rs
--rw-r--r--   0     1001      127    41672 2024-01-23 09:02:26.000000 safetensors-0.4.2/safetensors/src/tensor.rs
--rw-r--r--   0     1001      127    10566 2024-01-23 09:02:26.000000 safetensors-0.4.2/README.md
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 safetensors-0.4.2/bindings/python/Cargo.toml
--rw-r--r--   0     1001      127      685 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/.gitignore
--rw-r--r--   0     1001      127      190 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/MANIFEST.in
--rw-r--r--   0     1001      127     1103 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/Makefile
--rw-r--r--   0     1001      127      852 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/README.md
--rw-r--r--   0     1001      127     2142 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/benches/test_flax.py
--rw-r--r--   0     1001      127     2177 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/benches/test_mlx.py
--rw-r--r--   0     1001      127     1968 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/benches/test_paddle.py
--rw-r--r--   0     1001      127     4764 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/benches/test_pt.py
--rw-r--r--   0     1001      127     2631 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/benches/test_tf.py
--rw-r--r--   0     1001      127    14769 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/convert.py
--rw-r--r--   0     1001      127     1459 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/convert_all.py
--rw-r--r--   0     1001      127      729 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/fuzz.py
--rw-r--r--   0     1001      127      171 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/__init__.py
--rw-r--r--   0     1001      127     1970 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/__init__.pyi
--rw-r--r--   0     1001      127     3846 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/flax.py
--rw-r--r--   0     1001      127     3837 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/mlx.py
--rw-r--r--   0     1001      127     4937 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/numpy.py
--rw-r--r--   0     1001      127     4163 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/paddle.py
--rw-r--r--   0     1001      127        0 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/py.typed
--rw-r--r--   0     1001      127     3890 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/tensorflow.py
--rw-r--r--   0     1001      127    17294 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/py_src/safetensors/torch.py
--rw-r--r--   0     1001      127      891 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/setup.cfg
--rw-r--r--   0     1001      127    39822 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/src/lib.rs
--rw-r--r--   0     1001      127     5370 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/stub.py
--rw-r--r--   0     1001      127        0 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/data/__init__.py
--rw-r--r--   0     1001      127     2337 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_flax_comparison.py
--rw-r--r--   0     1001      127     2010 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_mlx_comparison.py
--rw-r--r--   0     1001      127     1492 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_paddle_comparison.py
--rw-r--r--   0     1001      127    12107 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_pt_comparison.py
--rw-r--r--   0     1001      127    10195 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_pt_model.py
--rw-r--r--   0     1001      127     9151 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_simple.py
--rw-r--r--   0     1001      127     2841 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/tests/test_tf_comparison.py
--rw-r--r--   0     1001      127     9084 2024-01-23 09:02:26.000000 safetensors-0.4.2/bindings/python/Cargo.lock
--rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 safetensors-0.4.2/pyproject.toml
--rw-r--r--   0     1001      127     3837 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/mlx.py
--rw-r--r--   0     1001      127     3846 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/flax.py
--rw-r--r--   0     1001      127     1970 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/__init__.pyi
--rw-r--r--   0     1001      127    17294 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/torch.py
--rw-r--r--   0     1001      127     4163 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/paddle.py
--rw-r--r--   0     1001      127      171 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/__init__.py
--rw-r--r--   0     1001      127     3890 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/tensorflow.py
--rw-r--r--   0     1001      127     4937 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/numpy.py
--rw-r--r--   0     1001      127        0 2024-01-23 09:02:26.000000 safetensors-0.4.2/py_src/safetensors/py.typed
--rw-r--r--   0        0        0     3842 1970-01-01 00:00:00.000000 safetensors-0.4.2/PKG-INFO
+-rw-r--r--   0     1001      127     1045 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/Cargo.toml
+-rw-r--r--   0     1001      127    11357 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/LICENSE
+-rw-r--r--   0     1001      127    10566 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/README.md
+-rw-r--r--   0     1001      127     1701 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/benches/benchmark.rs
+-rw-r--r--   0     1001      127      184 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/src/lib.rs
+-rw-r--r--   0     1001      127    16641 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/src/slice.rs
+-rw-r--r--   0     1001      127    41672 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/safetensors/src/tensor.rs
+-rw-r--r--   0     1001      127    10566 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/README.md
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 safetensors-0.4.2rc0/bindings/python/Cargo.toml
+-rw-r--r--   0     1001      127      685 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/.gitignore
+-rw-r--r--   0     1001      127      190 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/MANIFEST.in
+-rw-r--r--   0     1001      127     1103 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/Makefile
+-rw-r--r--   0     1001      127      852 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/README.md
+-rw-r--r--   0     1001      127     2142 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_flax.py
+-rw-r--r--   0     1001      127     2177 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_mlx.py
+-rw-r--r--   0     1001      127     1968 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_paddle.py
+-rw-r--r--   0     1001      127     4764 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_pt.py
+-rw-r--r--   0     1001      127     2631 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/benches/test_tf.py
+-rw-r--r--   0     1001      127    14769 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/convert.py
+-rw-r--r--   0     1001      127     1459 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/convert_all.py
+-rw-r--r--   0     1001      127      729 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/fuzz.py
+-rw-r--r--   0     1001      127      171 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/__init__.py
+-rw-r--r--   0     1001      127     1970 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/__init__.pyi
+-rw-r--r--   0     1001      127     3846 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/flax.py
+-rw-r--r--   0     1001      127     3837 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/mlx.py
+-rw-r--r--   0     1001      127     4937 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/numpy.py
+-rw-r--r--   0     1001      127     4163 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/paddle.py
+-rw-r--r--   0     1001      127        0 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/py.typed
+-rw-r--r--   0     1001      127     3890 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/tensorflow.py
+-rw-r--r--   0     1001      127    17294 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/py_src/safetensors/torch.py
+-rw-r--r--   0     1001      127      891 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/setup.cfg
+-rw-r--r--   0     1001      127    39822 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/src/lib.rs
+-rw-r--r--   0     1001      127     5370 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/stub.py
+-rw-r--r--   0     1001      127        0 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/data/__init__.py
+-rw-r--r--   0     1001      127     2337 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_flax_comparison.py
+-rw-r--r--   0     1001      127     2010 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_mlx_comparison.py
+-rw-r--r--   0     1001      127     1492 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_paddle_comparison.py
+-rw-r--r--   0     1001      127    12107 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_pt_comparison.py
+-rw-r--r--   0     1001      127    10195 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_pt_model.py
+-rw-r--r--   0     1001      127     9151 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_simple.py
+-rw-r--r--   0     1001      127     2841 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/tests/test_tf_comparison.py
+-rw-r--r--   0     1001      127     9094 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/bindings/python/Cargo.lock
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 safetensors-0.4.2rc0/pyproject.toml
+-rw-r--r--   0     1001      127     3837 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/mlx.py
+-rw-r--r--   0     1001      127     3846 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/flax.py
+-rw-r--r--   0     1001      127     1970 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/__init__.pyi
+-rw-r--r--   0     1001      127    17294 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/torch.py
+-rw-r--r--   0     1001      127     4163 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/paddle.py
+-rw-r--r--   0     1001      127      171 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/__init__.py
+-rw-r--r--   0     1001      127     3890 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/tensorflow.py
+-rw-r--r--   0     1001      127     4937 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/numpy.py
+-rw-r--r--   0     1001      127        0 2024-01-22 19:19:52.000000 safetensors-0.4.2rc0/py_src/safetensors/py.typed
+-rw-r--r--   0        0        0     3845 1970-01-01 00:00:00.000000 safetensors-0.4.2rc0/PKG-INFO
```

### Comparing `safetensors-0.4.2/safetensors/Cargo.toml` & `safetensors-0.4.2rc0/safetensors/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "safetensors"
-version = "0.4.2"
+version = "0.4.2-rc.0"
 edition = "2021"
 homepage = "https://github.com/huggingface/safetensors"
 repository = "https://github.com/huggingface/safetensors"
 documentation = "https://docs.rs/safetensors/"
 license = "Apache-2.0"
 keywords = ["safetensors", "huggingface", "Tensors", "Pytorch", "Tensorflow"]
 readme = "./README.md"
```

### Comparing `safetensors-0.4.2/safetensors/LICENSE` & `safetensors-0.4.2rc0/safetensors/LICENSE`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/safetensors/README.md` & `safetensors-0.4.2rc0/safetensors/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/safetensors/benches/benchmark.rs` & `safetensors-0.4.2rc0/safetensors/benches/benchmark.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/safetensors/src/slice.rs` & `safetensors-0.4.2rc0/safetensors/src/slice.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/safetensors/src/tensor.rs` & `safetensors-0.4.2rc0/safetensors/src/tensor.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/README.md` & `safetensors-0.4.2rc0/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/.gitignore` & `safetensors-0.4.2rc0/bindings/python/.gitignore`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/Makefile` & `safetensors-0.4.2rc0/bindings/python/Makefile`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/README.md` & `safetensors-0.4.2rc0/bindings/python/README.md`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/benches/test_flax.py` & `safetensors-0.4.2rc0/bindings/python/benches/test_flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/benches/test_mlx.py` & `safetensors-0.4.2rc0/bindings/python/benches/test_mlx.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/benches/test_paddle.py` & `safetensors-0.4.2rc0/bindings/python/benches/test_paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/benches/test_pt.py` & `safetensors-0.4.2rc0/bindings/python/benches/test_pt.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/benches/test_tf.py` & `safetensors-0.4.2rc0/bindings/python/benches/test_tf.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/convert.py` & `safetensors-0.4.2rc0/bindings/python/convert.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/convert_all.py` & `safetensors-0.4.2rc0/bindings/python/convert_all.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/fuzz.py` & `safetensors-0.4.2rc0/bindings/python/fuzz.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/__init__.pyi` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/flax.py` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/mlx.py` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/mlx.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/numpy.py` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/paddle.py` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/tensorflow.py` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/py_src/safetensors/torch.py` & `safetensors-0.4.2rc0/bindings/python/py_src/safetensors/torch.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/setup.cfg` & `safetensors-0.4.2rc0/bindings/python/setup.cfg`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/src/lib.rs` & `safetensors-0.4.2rc0/bindings/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/stub.py` & `safetensors-0.4.2rc0/bindings/python/stub.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_flax_comparison.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_flax_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_mlx_comparison.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_mlx_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_paddle_comparison.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_paddle_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_pt_comparison.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_pt_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_pt_model.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_pt_model.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_simple.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/tests/test_tf_comparison.py` & `safetensors-0.4.2rc0/bindings/python/tests/test_tf_comparison.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/bindings/python/Cargo.lock` & `safetensors-0.4.2rc0/bindings/python/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 name = "itoa"
 version = "1.0.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.151"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "302d7ab3130588088d277783b1e2d2e10c9e9e4a16dd9050e6ec93fb3e7048f4"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
@@ -99,17 +99,17 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.75"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "907a61bd0f64c2f29cd1cf1dc34d05176426a3f504a78010f08416ddb7b13708"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.2"
@@ -193,23 +193,23 @@
 name = "ryu"
 version = "1.0.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
 
 [[package]]
 name = "safetensors"
-version = "0.4.2"
+version = "0.4.2-rc.0"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "safetensors-python"
-version = "0.4.2"
+version = "0.4.2-rc.0"
 dependencies = [
  "memmap2",
  "pyo3",
  "safetensors",
  "serde_json",
 ]
 
@@ -217,26 +217,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.195"
+version = "1.0.194"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "63261df402c67811e9ac6def069e4786148c4563f4b50fd4bf30aa370d626b02"
+checksum = "0b114498256798c94a0689e1a15fec6005dee8ac1f41de56404b67afc2a4b773"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.195"
+version = "1.0.194"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "46fe8f8603d81ba86327b23a2e9cdf49e1255fb94a4c5f297f6ee0547178ea2c"
+checksum = "a3385e45322e8f9931410f01b3031ec534c3947d0e94c18049af4d9f9907d4e0"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -248,23 +248,23 @@
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.11.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.47"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "1726efe18f42ae774cc644f330953a5e7b3c3003d3edcecf18850fe9d4dd9afb"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `safetensors-0.4.2/pyproject.toml` & `safetensors-0.4.2rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/mlx.py` & `safetensors-0.4.2rc0/py_src/safetensors/mlx.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/flax.py` & `safetensors-0.4.2rc0/py_src/safetensors/flax.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/__init__.pyi` & `safetensors-0.4.2rc0/py_src/safetensors/__init__.pyi`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/torch.py` & `safetensors-0.4.2rc0/py_src/safetensors/torch.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/paddle.py` & `safetensors-0.4.2rc0/py_src/safetensors/paddle.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/tensorflow.py` & `safetensors-0.4.2rc0/py_src/safetensors/tensorflow.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/py_src/safetensors/numpy.py` & `safetensors-0.4.2rc0/py_src/safetensors/numpy.py`

 * *Files identical despite different names*

### Comparing `safetensors-0.4.2/PKG-INFO` & `safetensors-0.4.2rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safetensors
-Version: 0.4.2
+Version: 0.4.2rc0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

