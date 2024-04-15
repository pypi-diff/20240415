# Comparing `tmp/cykooz.heif-1.0.0.tar.gz` & `tmp/cykooz.heif-1.0.1.tar.gz`

## Comparing `cykooz.heif-1.0.0.tar` & `cykooz.heif-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      341 1970-01-01 00:00:00.000000 cykooz.heif-1.0.0/Cargo.toml
--rw-r--r--   0        0        0     4016 2024-01-26 12:09:48.000000 cykooz.heif-1.0.0/CHANGES.rst
--rw-r--r--   0        0        0      448 2024-01-26 12:09:48.000000 cykooz.heif-1.0.0/DEV.md
--rw-r--r--   0        0        0     1073 2024-01-26 12:09:48.000000 cykooz.heif-1.0.0/LICENSE
--rw-r--r--   0        0        0     1911 2024-01-26 12:09:48.000000 cykooz.heif-1.0.0/README.rst
--rw-r--r--   0        0        0       65 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/python/cykooz/__init__.py
--rw-r--r--   0        0        0       67 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/python/cykooz/heif/__init__.py
--rw-r--r--   0        0        0      106 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/python/cykooz/heif/errors.py
--rw-r--r--   0        0        0     2646 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/python/cykooz/heif/image.py
--rw-r--r--   0        0        0     1807 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/python/cykooz/heif/pil.py
--rw-r--r--   0        0        0      170 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/python/cykooz/heif/typing.py
--rw-r--r--   0        0        0     6078 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/src/lib.rs
--rw-r--r--   0        0        0     4693 2024-01-26 12:09:51.000000 cykooz.heif-1.0.0/src/stream.rs
--rw-r--r--   0        0        0    18675 2024-01-26 12:09:48.000000 cykooz.heif-1.0.0/Cargo.lock
--rw-r--r--   0        0        0     1238 2024-01-26 12:09:48.000000 cykooz.heif-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 cykooz.heif-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 cykooz.heif-1.0.1/Cargo.toml
+-rw-r--r--   0        0        0     4168 2024-04-15 08:12:52.000000 cykooz.heif-1.0.1/CHANGES.rst
+-rw-r--r--   0        0        0      448 2024-04-15 08:12:52.000000 cykooz.heif-1.0.1/DEV.md
+-rw-r--r--   0        0        0     1073 2024-04-15 08:12:52.000000 cykooz.heif-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1911 2024-04-15 08:12:52.000000 cykooz.heif-1.0.1/README.rst
+-rw-r--r--   0        0        0       65 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/python/cykooz/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/python/cykooz/heif/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/python/cykooz/heif/errors.py
+-rw-r--r--   0        0        0     2646 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/python/cykooz/heif/image.py
+-rw-r--r--   0        0        0     1807 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/python/cykooz/heif/pil.py
+-rw-r--r--   0        0        0      170 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/python/cykooz/heif/typing.py
+-rw-r--r--   0        0        0     6109 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/src/lib.rs
+-rw-r--r--   0        0        0     4808 2024-04-15 08:12:56.000000 cykooz.heif-1.0.1/src/stream.rs
+-rw-r--r--   0        0        0    18901 2024-04-15 08:12:52.000000 cykooz.heif-1.0.1/Cargo.lock
+-rw-r--r--   0        0        0     1238 2024-04-15 08:12:52.000000 cykooz.heif-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 cykooz.heif-1.0.1/PKG-INFO
```

### Comparing `cykooz.heif-1.0.0/CHANGES.rst` & `cykooz.heif-1.0.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,27 @@
         - Changes
         - Bug Fixes
         - Docs
 
 CHANGELOG
 *********
 
+Next release
+============
+
+Changes
+-------
+
+- Updated version of ``pyo3`` to 0.21.
+
+Bug Fixes
+---------
+
+- Updated version of ``libheif-rs`` to 1.0.1.
+
 1.0.0 (2024-01-26)
 =================
 
 Features
 --------
 
 - Added support for Pillow >= 10.1
```

### Comparing `cykooz.heif-1.0.0/LICENSE` & `cykooz.heif-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cykooz.heif-1.0.0/README.rst` & `cykooz.heif-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `cykooz.heif-1.0.0/python/cykooz/heif/image.py` & `cykooz.heif-1.0.1/python/cykooz/heif/image.py`

 * *Files identical despite different names*

### Comparing `cykooz.heif-1.0.0/python/cykooz/heif/pil.py` & `cykooz.heif-1.0.1/python/cykooz/heif/pil.py`

 * *Files identical despite different names*

### Comparing `cykooz.heif-1.0.0/src/lib.rs` & `cykooz.heif-1.0.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -62,25 +62,25 @@
         let planes = image.planes();
 
         let data: PyObject;
         let stride: PyObject;
         let bits_pre_pixel: PyObject;
         match planes.interleaved {
             Some(plane) => {
-                data = PyBytes::new(py, plane.data).into();
+                data = PyBytes::new_bound(py, plane.data).into();
                 stride = plane.stride.to_object(py);
                 bits_pre_pixel = plane.bits_per_pixel.to_object(py);
             }
             None => {
                 data = py.None();
                 stride = py.None();
                 bits_pre_pixel = py.None();
             }
         };
-        let res: PyObject = PyTuple::new(py, &[data, stride, bits_pre_pixel]).into();
+        let res: PyObject = PyTuple::new_bound(py, &[data, stride, bits_pre_pixel]).into();
         Ok(res)
     }
 
     fn get_exif(&self, py: Python) -> PyResult<PyObject> {
         let context = self.heif_context.lock().unwrap();
         let handle = result2pyresult(context.primary_image_handle())?;
         let mut meta_ids: [ItemId; 1] = [0];
@@ -89,15 +89,15 @@
             Ok(py.None())
         } else {
             if handle.metadata_size(meta_ids[0]) == 0 {
                 // Invalid Exif block. It may have been incorrectly removed from the file.
                 return Ok(py.None());
             }
             let exif = result2pyresult(handle.metadata(meta_ids[0]))?;
-            Ok(PyBytes::new(py, &exif[4..]).into())
+            Ok(PyBytes::new_bound(py, &exif[4..]).into())
         }
     }
 }
 
 /// open_heif_from_path(path: str) -> HeifImage
 /// --
 ///
@@ -167,28 +167,28 @@
 /// Check file type by it first bytes.
 /// Input data should be at least 12 bytes.
 ///
 /// :type data: bytes
 /// :rtype: str
 #[pyfunction]
 fn check_file_type(py: Python, data: PyObject) -> PyResult<String> {
-    let py_bytes = data.downcast::<PyBytes>(py)?;
+    let py_bytes = data.downcast_bound::<PyBytes>(py)?;
     let bytes = py_bytes.as_bytes();
     let res = libheif_rs::check_file_type(bytes);
     Ok(match res {
         FileTypeResult::No => "no".into(),
         FileTypeResult::Supported => "supported".into(),
         FileTypeResult::Unsupported => "unsupported".into(),
         FileTypeResult::MayBe => "maybe".into(),
     })
 }
 
 /// This module is a python module implemented in Rust.
 #[pymodule]
-fn rust_lib(_py: Python, m: &PyModule) -> PyResult<()> {
+fn rust_lib(_py: Python, m: &Bound<PyModule>) -> PyResult<()> {
     m.add_wrapped(wrap_pyfunction!(open_heif_from_path))?;
     m.add_wrapped(wrap_pyfunction!(open_heif_from_reader))?;
     m.add_wrapped(wrap_pyfunction!(check_file_type))?;
     m.add_class::<HeifImage>()?;
 
     Ok(())
 }
```

### Comparing `cykooz.heif-1.0.0/src/stream.rs` & `cykooz.heif-1.0.1/src/stream.rs`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 }
 
 impl io::Read for StreamFromPy {
     fn read(&mut self, buf: &mut [u8]) -> io::Result<usize> {
         Python::with_gil(
             |py| match self.py_stream.call_method1(py, "read", (buf.len(),)) {
                 Ok(v) => {
-                    let py_bytes: &PyBytes = v.downcast(py).map_err(|_| {
+                    let py_bytes: &Bound<PyBytes> = v.downcast_bound(py).map_err(|_| {
                         io::Error::new(
                             io::ErrorKind::Other,
                             "Error during casting PyObject into PyBytes \
                          ('read' method returns not a bytes)",
                         )
                     })?;
                     let bytes = py_bytes.as_bytes();
@@ -75,18 +75,19 @@
 
     use pyo3::types::IntoPyDict;
 
     use super::*;
 
     #[test]
     fn test_read() -> PyResult<()> {
+        pyo3::prepare_freethreaded_python();
         Python::with_gil(|py| {
-            let locals = [("io", py.import("io")?)].into_py_dict(py);
+            let locals = [("io", py.import_bound("io")?)].into_py_dict_bound(py);
             let code = "io.BytesIO(b'a' * 100 + b'b' * 50)";
-            let result = py.eval(code, None, Some(locals))?;
+            let result = py.eval_bound(code, None, Some(&locals))?;
             let mut stream_from_py = StreamFromPy {
                 py_stream: result.into_py(py),
             };
             let mut buf = vec![0u8; 100];
 
             let size = stream_from_py.read(&mut buf)?;
             assert_eq!(size, 100);
@@ -104,41 +105,42 @@
 
             Ok(())
         })
     }
 
     #[test]
     fn test_seek() -> PyResult<()> {
+        pyo3::prepare_freethreaded_python();
         Python::with_gil(|py| {
-            let locals = [("io", py.import("io")?)].into_py_dict(py);
+            let locals = [("io", py.import_bound("io")?)].into_py_dict_bound(py);
             let code = "io.BytesIO(b'a' * 100 + b'b' * 50)";
-            let result = py.eval(code, None, Some(locals))?;
+            let result = py.eval_bound(code, None, Some(&locals))?;
             let mut stream_from_py = StreamFromPy {
                 py_stream: result.into_py(py),
             };
 
             let pos = stream_from_py.seek(io::SeekFrom::Start(0))?;
             assert_eq!(pos, 0);
 
             let pos = stream_from_py.seek(io::SeekFrom::End(0))?;
             assert_eq!(pos, 150);
 
             let pos = stream_from_py.seek(io::SeekFrom::Start(100))?;
             assert_eq!(pos, 100);
 
-            let pos = stream_from_py.seek(io::SeekFrom::Current(0))?;
+            let pos = stream_from_py.stream_position()?;
             assert_eq!(pos, 100);
 
             let mut buf = vec![0u8; 100];
             let size = stream_from_py.read(&mut buf)?;
             assert_eq!(size, 50);
             let mut expect = vec![b'b'; 50];
             expect.append(&mut vec![0u8; 50]);
             assert_eq!(buf, expect);
 
-            let pos = stream_from_py.seek(io::SeekFrom::Current(0))?;
+            let pos = stream_from_py.stream_position()?;
             assert_eq!(pos, 150);
 
             Ok(())
         })
     }
 }
```

### Comparing `cykooz.heif-1.0.0/Cargo.lock` & `cykooz.heif-1.0.1/Cargo.lock`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bindgen"
-version = "0.69.2"
+version = "0.69.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4c69fae65a523209d34240b60abe0c42d33d1045d445c0839d8a4894a736e2d"
+checksum = "a00dc851838a2120612785d195287475a3ac45514741da670b735818822129a0"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cexpr",
  "clang-sys",
+ "itertools",
  "lazy_static",
  "lazycell",
  "log",
- "peeking_take_while",
  "prettyplease",
  "proc-macro2",
  "quote",
  "regex",
  "rustc-hash",
  "shlex",
  "syn",
@@ -44,17 +44,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "cexpr"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
 dependencies = [
@@ -76,17 +76,17 @@
  "glob",
  "libc",
  "libloading",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "a47c1c47d2f5964e29c61246e81db715514cd532db6b5116a25ea3c03d6780a2"
 
 [[package]]
 name = "enumn"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
 dependencies = [
@@ -98,15 +98,15 @@
 [[package]]
 name = "errno"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
- "windows-sys 0.52.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "four-cc"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "431a4c31778fde52b4400de34975f219eeca55cc829a9de157cd743a5b230ecb"
@@ -125,22 +125,31 @@
 
 [[package]]
 name = "home"
 version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
- "windows-sys 0.52.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
+
+[[package]]
+name = "itertools"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
@@ -148,23 +157,23 @@
 name = "lazycell"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libheif-rs"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fc66735697217d6676b6fe89b33cbd0e7c580e5beffbc3861bdf42eb1ce1aa70"
+checksum = "ceb8665b2462b0e04af7444ebfa61eeeb7fdb4e8829f7a8b080bab643257a017"
 dependencies = [
  "enumn",
  "four-cc",
  "libc",
  "libheif-sys",
 ]
 
@@ -179,20 +188,20 @@
  "pkg-config",
  "vcpkg",
  "walkdir",
 ]
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
@@ -205,29 +214,29 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
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
 name = "minimal-lexical"
 version = "0.2.1"
@@ -270,110 +279,112 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "peeking_take_while"
-version = "0.1.2"
+name = "pkg-config"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
-name = "pkg-config"
-version = "0.3.29"
+name = "portable-atomic"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2900ede94e305130c13ddd391e0ab7cbaeb783945ae07a279c268cb05109c6cb"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.16"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
+checksum = "5ac2cf0f2e4f42b49f5ffd07dae8d746508ef7526c13940e5f524012ae6c6550"
 dependencies = [
  "proc-macro2",
  "syn",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
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
@@ -381,40 +392,40 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rust_lib"
 version = "0.7.0"
 dependencies = [
  "libheif-rs",
  "pyo3",
@@ -424,23 +435,23 @@
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.38.30"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "322394588aaf33c24007e8bb3238ee3e4c5c09c084ab32bc73890b99ff326bca"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys 0.52.0",
+ "windows-sys",
 ]
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
@@ -458,34 +469,34 @@
 name = "shlex"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fda2ff0d084019ba4d7c6f371c95d8fd75ce3524c3cb8fb653a3023f6323e64"
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
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
 
@@ -499,17 +510,17 @@
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "which"
@@ -552,28 +563,19 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.48.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
-dependencies = [
- "windows-targets 0.48.5",
-]
-
-[[package]]
-name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -585,103 +587,110 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
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
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
```

### Comparing `cykooz.heif-1.0.0/pyproject.toml` & `cykooz.heif-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.2.3"]
 build-backend = "maturin"
 
 
 [project]
 name = "cykooz.heif"
-version = "1.0.0"
+version = "1.0.1"
 description = "A decoder of HEIF format of images"
 readme = "README.rst"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
```

### Comparing `cykooz.heif-1.0.0/PKG-INFO` & `cykooz.heif-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: cykooz.heif
-Version: 1.0.0
+Version: 1.0.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Multimedia :: Graphics :: Graphics Conversion
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: wheel ; extra == 'dev'
 Requires-Dist: maturin[zig,patchelf] ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
-Requires-Dist: Pillow ; extra == 'dev'
+Requires-Dist: pillow ; extra == 'dev'
 Requires-Dist: piexif ; extra == 'dev'
 Provides-Extra: dev
 License-File: LICENSE
 Summary: A decoder of HEIF format of images
 Keywords: heif,heic,libheif,pil,pillow
 Home-Page: https://github.com/Cykooz/cykooz.heif
 Author: Kirill Kuzminykh <cykooz@gmail.com>
```

