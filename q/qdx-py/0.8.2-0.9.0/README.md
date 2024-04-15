# Comparing `tmp/qdx_py-0.8.2.tar.gz` & `tmp/qdx_py-0.9.0.tar.gz`

## Comparing `qdx_py-0.8.2.tar` & `qdx_py-0.9.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 qdx_py-0.8.2/Cargo.toml
--rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.8.2/.github/workflows/CI.yml
--rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.8.2/.gitignore
--rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.8.2/README.md
--rw-r--r--   0     1000      100     7839 2024-04-04 06:34:15.000000 qdx_py-0.8.2/src/lib.rs
--rw-r--r--   0     1000      100    27252 2024-04-04 06:35:23.000000 qdx_py-0.8.2/Cargo.lock
--rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      600 1970-01-01 00:00:00.000000 qdx_py-0.9.0/Cargo.toml
+-rw-r--r--   0     1000      100     2809 2023-11-16 02:44:04.000000 qdx_py-0.9.0/.github/workflows/CI.yml
+-rw-r--r--   0     1000      100      685 2023-11-16 02:44:04.000000 qdx_py-0.9.0/.gitignore
+-rw-r--r--   0     1000      100     2028 2024-04-04 02:54:02.000000 qdx_py-0.9.0/README.md
+-rw-r--r--   0     1000      100      513 2024-04-15 06:01:05.000000 qdx_py-0.9.0/src/lib.rs
+-rw-r--r--   0     1000      100     7083 2024-04-15 05:53:38.000000 qdx_py-0.9.0/src/qdx.rs
+-rw-r--r--   0     1000      100    27482 2024-04-15 05:53:12.000000 qdx_py-0.9.0/Cargo.lock
+-rw-r--r--   0     1000      100      366 2023-12-01 06:07:08.000000 qdx_py-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 qdx_py-0.9.0/PKG-INFO
```

### Comparing `qdx_py-0.8.2/.github/workflows/CI.yml` & `qdx_py-0.9.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `qdx_py-0.8.2/.gitignore` & `qdx_py-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qdx_py-0.8.2/README.md` & `qdx_py-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qdx_py-0.8.2/src/lib.rs` & `qdx_py-0.9.0/src/qdx.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,97 @@
 use std::collections::HashSet;
 
 use pyo3::{exceptions::PyRuntimeError, prelude::*};
 use qdx_common::{AtomCheckStrictness, Conformer};
 
 /// Converts a pdb string into an array of qdx conformers as a json string
 #[pyfunction]
-fn pdb_to_conformer(
+pub fn pdb_to_conformer(
     pdb_contents: String,
     keep_residues: Option<HashSet<String>>,
     skip_residues: Option<HashSet<String>>,
 ) -> PyResult<String> {
     serde_json::to_string(
         &qdx_common::convert::pdb::from_pdb(pdb_contents, keep_residues, skip_residues)
             .map_err(|e| PyRuntimeError::new_err(e.to_string()))?,
     )
     .map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Returns the pdb string for a qdx conformer json string
 #[pyfunction]
-fn conformer_to_pdb(conformer_contents: String) -> PyResult<String> {
+pub fn conformer_to_pdb(conformer_contents: String) -> PyResult<String> {
     Ok(qdx_common::convert::pdb::to_pdb(
         &serde_json::from_str(&conformer_contents)
             .map_err(|e| PyRuntimeError::new_err(e.to_string()))?,
     ))
 }
 
 #[pyfunction]
-fn sdf_to_conformer(sdf_contents: String) -> PyResult<String> {
+pub fn sdf_to_conformer(sdf_contents: String) -> PyResult<String> {
     let conformer = qdx_common::convert::sdf::from_sdf(&sdf_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     let conformer_serialized =
         serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     Ok(conformer_serialized)
 }
 
 #[pyfunction]
-fn conformer_to_sdf(conformer_contents: String) -> PyResult<String> {
+pub fn conformer_to_sdf(conformer_contents: String) -> PyResult<String> {
     let conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     let sdf_serialized = qdx_common::convert::sdf::to_sdf(&conformer)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     Ok(sdf_serialized)
 }
 
 /// Takes two conformer json strings and concatenates them
 #[pyfunction]
-fn concat(conformer_1_contents: String, conformer_2_contents: String) -> PyResult<String> {
+pub fn concat(conformer_1_contents: String, conformer_2_contents: String) -> PyResult<String> {
     let mut conformer_1: Conformer = serde_json::from_str(&conformer_1_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     let conformer_2: Conformer = serde_json::from_str(&conformer_2_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     conformer_1.extend(conformer_2);
 
     serde_json::to_string(&conformer_1).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Drops amino acids from a conformer json string
 #[pyfunction]
-fn drop_amino_acids(
+pub fn drop_amino_acids(
     conformer_contents: String,
     amino_acids_to_drop: Vec<usize>,
 ) -> PyResult<String> {
     let mut conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     conformer.drop_amino_acids(&amino_acids_to_drop);
 
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Drops residues from a conformer json string
 #[pyfunction]
-fn drop_residues(conformer_contents: String, residues_to_drop: Vec<usize>) -> PyResult<String> {
+pub fn drop_residues(conformer_contents: String, residues_to_drop: Vec<usize>) -> PyResult<String> {
     let mut conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     conformer.drop_residues(&residues_to_drop);
 
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Charges standard amino acids given a conformer json string,
 #[pyfunction]
-fn formal_charge(conformer_contents: String, missing_atom_strictness: String) -> PyResult<String> {
+pub fn formal_charge(
+    conformer_contents: String,
+    missing_atom_strictness: String,
+) -> PyResult<String> {
     let mut conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     let strictness: AtomCheckStrictness =
         serde_json::from_str(&format!("\"{missing_atom_strictness}\""))
             .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
@@ -103,15 +106,15 @@
     conformer.topology.assign_fragment_charges();
 
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Fragments a conformer, updating the fragment formal charges based on existing atom charges
 #[pyfunction]
-fn fragment(
+pub fn fragment(
     conformer_contents: String,
     missing_atom_strictness: String,
     backbone_steps: usize,
     terminal_fragment_sidechain_size: Option<usize>,
 ) -> PyResult<String> {
     let mut conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
@@ -130,15 +133,15 @@
     conformer.topology.assign_fragment_charges();
 
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Fragments a conformer by atom labels, updating the fragment formal charges based on existing atom charges
 #[pyfunction]
-fn fragment_by_label(
+pub fn fragment_by_label(
     conformer_contents: String,
     missing_atom_strictness: String,
 ) -> PyResult<String> {
     let mut conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     let strictness: AtomCheckStrictness =
@@ -149,25 +152,27 @@
         .perceive_bonds(strictness)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
     conformer
         .perceive_formal_charges()
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
 
-    conformer.fragment_by_label().map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
+    conformer
+        .fragment_by_label()
+        .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
     conformer.topology.assign_fragment_charges();
-    
-    assert!(conformer.is_valid());   
-    
+
+    assert!(conformer.is_valid());
+
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
 
 /// Fragments a conformer, using distance based bond inference instead of pattern based bond inference
 #[pyfunction]
-fn fragment_legacy(
+pub fn fragment_legacy(
     conformer_contents: String,
     bond_length_tolerance: f32,
     backbone_steps: usize,
     terminal_fragment_sidechain_size: Option<usize>,
 ) -> PyResult<String> {
     let mut conformer: Conformer = serde_json::from_str(&conformer_contents)
         .map_err(|e| PyRuntimeError::new_err(e.to_string()))?;
@@ -181,25 +186,7 @@
     conformer.topology.fragments =
         Some(conformer.fragment(backbone_steps, terminal_fragment_sidechain_size));
 
     conformer.topology.fragment_charges = conformer.topology.explicit_fragment_charges();
 
     serde_json::to_string(&conformer).map_err(|e| PyRuntimeError::new_err(e.to_string()))
 }
-
-/// QDX-Common utilities for python
-#[pymodule]
-fn qdx_py(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add("__version__", env!("CARGO_PKG_VERSION"))?;
-    m.add_function(wrap_pyfunction!(pdb_to_conformer, m)?)?;
-    m.add_function(wrap_pyfunction!(conformer_to_pdb, m)?)?;
-    m.add_function(wrap_pyfunction!(sdf_to_conformer, m)?)?;
-    m.add_function(wrap_pyfunction!(conformer_to_sdf, m)?)?;
-    m.add_function(wrap_pyfunction!(concat, m)?)?;
-    m.add_function(wrap_pyfunction!(formal_charge, m)?)?;
-    m.add_function(wrap_pyfunction!(fragment, m)?)?;
-    m.add_function(wrap_pyfunction!(fragment_legacy, m)?)?;
-    m.add_function(wrap_pyfunction!(fragment_by_label, m)?)?;
-    m.add_function(wrap_pyfunction!(drop_amino_acids, m)?)?;
-    m.add_function(wrap_pyfunction!(drop_residues, m)?)?;
-    Ok(())
-}
```

### Comparing `qdx_py-0.8.2/Cargo.lock` & `qdx_py-0.9.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.81"
+version = "1.0.82"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
+checksum = "f538837af36e6f6a9be0faa67f9a314f8119e4e4b5867c6ab40ed60360142519"
 
 [[package]]
 name = "assertables"
 version = "7.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c24e9d990669fbd16806bff449e4ac644fd9b1fca014760087732fe4102f131"
 
@@ -54,23 +54,23 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -81,15 +81,15 @@
 checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "js-sys",
  "num-traits",
  "wasm-bindgen",
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
@@ -98,17 +98,17 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "either"
-version = "1.10.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
@@ -125,28 +125,28 @@
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "half"
-version = "2.4.0"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
  "serde",
 ]
 
 [[package]]
@@ -306,26 +306,26 @@
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ouroboros"
 version = "0.1.0"
-source = "git+ssh://git@github.com/talo/ouroboros.git#fd6d061bb3247f6b804caf6fa9a119801eb4db3b"
+source = "git+ssh://git@github.com/talo/ouroboros.git#c7e5e46c3282ed639803c449e590502504c1abf8"
 dependencies = [
  "ouroboros-proc-macro",
  "serde",
  "serde_json",
  "thiserror",
 ]
 
 [[package]]
 name = "ouroboros-proc-macro"
 version = "0.1.0"
-source = "git+ssh://git@github.com/talo/ouroboros.git#fd6d061bb3247f6b804caf6fa9a119801eb4db3b"
+source = "git+ssh://git@github.com/talo/ouroboros.git#c7e5e46c3282ed639803c449e590502504c1abf8"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -386,26 +386,26 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -414,61 +414,61 @@
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "qdx-common"
-version = "0.8.1"
-source = "git+ssh://git@github.com/talo/qdx-common.git#c96f8a19e4d0bbb4e34740dd33e8b6970930f09c"
+version = "0.8.2"
+source = "git+ssh://git@github.com/talo/qdx-common.git#4c4bbdaed55a957d86f801e51b29d13504ac4745"
 dependencies = [
  "anyhow",
  "assertables",
  "base64",
  "euclid",
  "half",
  "itertools",
@@ -487,27 +487,27 @@
  "tracing",
  "tracing-subscriber",
  "uuid",
 ]
 
 [[package]]
 name = "qdx-py"
-version = "0.8.2"
+version = "0.9.0"
 dependencies = [
  "pyo3",
  "qdx-common",
  "serde",
  "serde_json",
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
@@ -568,17 +568,17 @@
 checksum = "8395b4f860856b740f20a296ea2cd4d823e81a2658cf05ef61be22916026a906"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.14"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
+checksum = "80af6f9131f277a45a3fba6ce8e2258037bb0477a67e610d3c1fe046ab31de47"
 
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -672,17 +672,17 @@
  "quote",
  "rustversion",
  "syn",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -894,15 +894,15 @@
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -914,109 +914,116 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xml-rs"
 version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "791978798f0597cfc70478424c2b4fdc2b7a8024aaff78497ef00f24ef674193"
```

### Comparing `qdx_py-0.8.2/PKG-INFO` & `qdx_py-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qdx-py
-Version: 0.8.2
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # QDX-py
```

