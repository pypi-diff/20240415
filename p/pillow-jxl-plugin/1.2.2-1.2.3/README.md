# Comparing `tmp/pillow_jxl_plugin-1.2.2.tar.gz` & `tmp/pillow_jxl_plugin-1.2.3.tar.gz`

## Comparing `pillow_jxl_plugin-1.2.2.tar` & `pillow_jxl_plugin-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,63 @@
--rw-r--r--   0        0        0      638 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.2/Cargo.toml
--rw-r--r--   0     1001      127     9422 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      758 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/.gitignore
--rw-r--r--   0     1001      127     1065 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/LICENSE
--rw-r--r--   0     1001      127     1931 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/README.md
--rw-r--r--   0     1001      127     1862 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/build.rs
--rw-r--r--   0     1001      127     4256 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/pillow_jxl/JpegXLImagePlugin.py
--rw-r--r--   0     1001      127      165 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/pillow_jxl/__init__.py
--rw-r--r--   0     1001      127     1182 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/pillow_jxl/__init__.pyi
--rw-r--r--   0     1001      127        0 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/pillow_jxl/py.typed
--rw-r--r--   0     1001      127     6958 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/src/lib.rs
--rw-r--r--   0     1001      127    12387 2024-03-31 08:07:17.000000 pillow_jxl_plugin-1.2.2/Cargo.lock
--rw-r--r--   0     1001      127      426 2024-03-31 08:06:23.000000 pillow_jxl_plugin-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.2/PKG-INFO
+-rw-r--r--   0     1001      127     1506 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/Cargo.toml
+-rw-r--r--   0     1001      127    35148 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/COPYING
+-rw-r--r--   0     1001      127      698 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/LICENSE
+-rw-r--r--   0     1001      127     3767 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/README.md
+-rw-r--r--   0     1001      127     1439 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/benches/decode.rs
+-rw-r--r--   0     1001      127     1829 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/benches/encode.rs
+-rw-r--r--   0     1001      127     3667 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/common.rs
+-rw-r--r--   0     1001      127     3211 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/decode/result.rs
+-rw-r--r--   0     1001      127    17932 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/decode.rs
+-rw-r--r--   0     1001      127    22931 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/encode.rs
+-rw-r--r--   0     1001      127     4368 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/errors.rs
+-rw-r--r--   0     1001      127     7720 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/image.rs
+-rw-r--r--   0     1001      127     5835 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/lib.rs
+-rw-r--r--   0     1001      127     4491 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/memory.rs
+-rw-r--r--   0     1001      127     3298 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel/resizable_runner.rs
+-rw-r--r--   0     1001      127     3130 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel/threads_runner.rs
+-rw-r--r--   0     1001      127     3332 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/parallel.rs
+-rw-r--r--   0     1001      127     4162 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests/decode.rs
+-rw-r--r--   0     1001      127     5918 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests/encode.rs
+-rw-r--r--   0     1001      127      480 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/tests.rs
+-rw-r--r--   0     1001      127     1536 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-rs/src/utils.rs
+-rw-r--r--   0     1001      127     3767 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/README.md
+-rw-r--r--   0     1001      127       78 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/Cargo.toml
+-rw-r--r--   0     1001      127      968 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/Cargo.toml
+-rw-r--r--   0     1001      127    35148 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/COPYING
+-rw-r--r--   0     1001      127      697 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/LICENSE
+-rw-r--r--   0     1001      127      618 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/README.md
+-rw-r--r--   0     1001      127     1138 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/build.rs
+-rw-r--r--   0     1001      127     2292 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/cms.rs
+-rw-r--r--   0     1001      127     2884 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/codestream_header.rs
+-rw-r--r--   0     1001      127     1259 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/color_encoding.rs
+-rw-r--r--   0     1001      127     9423 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/decode.rs
+-rw-r--r--   0     1001      127    10492 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/encode.rs
+-rw-r--r--   0     1001      127    14713 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/lib.rs
+-rw-r--r--   0     1001      127      371 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/memory_manager.rs
+-rw-r--r--   0     1001      127      551 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/parallel_runner.rs
+-rw-r--r--   0     1001      127     1529 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/resizable_parallel_runner.rs
+-rw-r--r--   0     1001      127      981 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/stats.rs
+-rw-r--r--   0     1001      127     1379 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/thread_parallel_runner.rs
+-rw-r--r--   0     1001      127     1821 2024-04-15 05:31:10.000000 pillow_jxl_plugin-1.2.3/jpegxl-rs/jpegxl-sys/src/types.rs
+-rw-r--r--   0        0        0      557 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.3/Cargo.toml
+-rw-r--r--   0     1001      127      451 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.github/dependabot.yml
+-rw-r--r--   0     1001      127     6270 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.github/workflows/release.yml
+-rw-r--r--   0     1001      127     1877 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      725 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.gitignore
+-rw-r--r--   0     1001      127      108 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/.gitmodules
+-rw-r--r--   0     1001      127     1065 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/LICENSE
+-rw-r--r--   0     1001      127     1931 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/README.md
+-rw-r--r--   0     1001      127     1862 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/build.rs
+-rw-r--r--   0     1001      127     4296 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/JpegXLImagePlugin.py
+-rw-r--r--   0     1001      127      165 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/__init__.py
+-rw-r--r--   0     1001      127     1182 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/__init__.pyi
+-rw-r--r--   0     1001      127        0 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pillow_jxl/py.typed
+-rw-r--r--   0     1001      127        7 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/requirements-dev.txt
+-rw-r--r--   0     1001      127     2818 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/src/decode.rs
+-rw-r--r--   0     1001      127     4356 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/src/encode.rs
+-rw-r--r--   0     1001      127      298 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/src/lib.rs
+-rw-r--r--   0     1001      127   106457 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/test/images/icc_profile/62AHB.jpg
+-rw-r--r--   0     1001      127    80683 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/test/images/icc_profile/62AHB.jxl
+-rw-r--r--   0     1001      127      395 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/test/test_plugin.py
+-rw-r--r--   0     1001      127    12051 2024-04-15 05:31:30.000000 pillow_jxl_plugin-1.2.3/Cargo.lock
+-rw-r--r--   0     1001      127      426 2024-04-15 05:31:09.000000 pillow_jxl_plugin-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 pillow_jxl_plugin-1.2.3/PKG-INFO
```

### Comparing `pillow_jxl_plugin-1.2.2/Cargo.toml` & `pillow_jxl_plugin-1.2.3/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [package]
 name = "pillow-jxl-plugin"
-version = "1.2.2"
+version = "1.2.3"
 edition = "2021"
 build = "build.rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pillow_jxl"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = "0.20.3"
-# jpegxl-rs = { version = "0.9.0", default-features = false, features = ["threads"] }
-jpegxl-rs = { git = "https://github.com/Isotr0py/jpegxl-rs.git", branch = "plugin", default-features = false, features = ["threads"] }
+pyo3 = { version="0.21.1", features = ["extension-module"] }
+jpegxl-rs = { path="./jpegxl-rs/jpegxl-rs", default-features = false, features = ["threads"] }
 
 [features]
 # Enables parallel processing support by enabling the "rayon" feature of jpeg-decoder.
 vendored = ["jpegxl-rs/vendored"]
 dynamic = []
```

### Comparing `pillow_jxl_plugin-1.2.2/.gitignore` & `pillow_jxl_plugin-1.2.3/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,10 @@
 /target
 Cargo.lock
 
-# for test
-*.ipynb
-*.jxl
-*.jpeg
-
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
 *.so
```

### Comparing `pillow_jxl_plugin-1.2.2/LICENSE` & `pillow_jxl_plugin-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.2/README.md` & `pillow_jxl_plugin-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.2/build.rs` & `pillow_jxl_plugin-1.2.3/build.rs`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.2/pillow_jxl/JpegXLImagePlugin.py` & `pillow_jxl_plugin-1.2.3/pillow_jxl/JpegXLImagePlugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,22 @@
     __loaded = -1
     __frame = 0
 
     def _open(self):
         self.fc = self.fp.read()
         self._decoder = Decoder()
 
-        self.jpeg, self._jxlinfo, self._data = self._decoder(self.fc)
+        self.jpeg, self._jxlinfo, self._data, icc_profile = self._decoder(self.fc)
         # FIXME (Isotr0py): Maybe slow down jpeg reconstruction
         if self.jpeg:
             with Image.open(BytesIO(self._data)) as im:
                 self._data = im.tobytes()
         self._size = (self._jxlinfo.width, self._jxlinfo.height)
         self.rawmode = self._jxlinfo.mode
+        self.info["icc_profile"] = icc_profile
         # NOTE (Isotr0py): PIL 10.1.0 changed the mode to property, use _mode instead
         if parse(PIL.__version__) >= parse("10.1.0"):
             self._mode = self.rawmode
         else:
             self.mode = self.rawmode
 
         self.tile = []
@@ -114,26 +115,26 @@
         effort=effort,
         use_container=use_container,
     )
     # FIXME (Isotr0py): im.filename maybe None if parse stream
     # TODO (Isotr0py): This part should be refactored in the near future
     if im.format == "JPEG" and im.filename:
         with open(im.filename, "rb") as f:
-            data = enc(f.read(), im.width, im.height, jpeg_encode=True, metadata={})
+            data = enc(f.read(), im.width, im.height, jpeg_encode=True)
     else:
         exif = info.get("exif", im.getexif().tobytes())
         if exif and exif.startswith(b"Exif\x00\x00"):
             exif = exif[6:]
         metadata = {
             "exif": exif,
             "jumb": info.get("jumb", b""),
             "xmp": info.get("xmp", b""),
         }
         data = enc(
-            im.tobytes(), im.width, im.height, jpeg_encode=False, metadata=metadata
+            im.tobytes(), im.width, im.height, jpeg_encode=False, **metadata
         )
     fp.write(data)
 
 
 Image.register_open(JXLImageFile.format, JXLImageFile, _accept)
 Image.register_save(JXLImageFile.format, _save)
 Image.register_extension(JXLImageFile.format, ".jxl")
```

### Comparing `pillow_jxl_plugin-1.2.2/pillow_jxl/__init__.pyi` & `pillow_jxl_plugin-1.2.3/pillow_jxl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pillow_jxl_plugin-1.2.2/Cargo.lock` & `pillow_jxl_plugin-1.2.3/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
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
 
@@ -117,17 +117,17 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
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
 ]
 
 [[package]]
 name = "heck"
@@ -146,35 +146,32 @@
 version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "jpegxl-rs"
 version = "0.10.2+libjxl-0.10.2"
-source = "git+https://github.com/Isotr0py/jpegxl-rs.git?branch=plugin#4d8f77c4f02ddfd0580abef7a4e2f883d89f36c6"
 dependencies = [
  "byteorder",
  "derive_builder",
  "half",
  "jpegxl-sys",
  "thiserror",
 ]
 
 [[package]]
 name = "jpegxl-src"
 version = "0.10.4"
-source = "git+https://github.com/Isotr0py/jpegxl-rs.git?branch=plugin#4d8f77c4f02ddfd0580abef7a4e2f883d89f36c6"
 dependencies = [
  "cmake",
 ]
 
 [[package]]
 name = "jpegxl-sys"
 version = "0.10.2+libjxl-0.10.2"
-source = "git+https://github.com/Isotr0py/jpegxl-rs.git?branch=plugin#4d8f77c4f02ddfd0580abef7a4e2f883d89f36c6"
 dependencies = [
  "jpegxl-src",
  "pkg-config",
 ]
 
 [[package]]
 name = "libc"
@@ -228,15 +225,15 @@
  "redox_syscall",
  "smallvec",
  "windows-targets",
 ]
 
 [[package]]
 name = "pillow-jxl-plugin"
-version = "1.2.2"
+version = "1.2.3"
 dependencies = [
  "jpegxl-rs",
  "pyo3",
 ]
 
 [[package]]
 name = "pkg-config"
@@ -248,26 +245,26 @@
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
@@ -275,62 +272,62 @@
  "pyo3-ffi",
  "pyo3-macros",
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
@@ -356,17 +353,17 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "2.0.57"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
```

### Comparing `pillow_jxl_plugin-1.2.2/PKG-INFO` & `pillow_jxl_plugin-1.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pillow-jxl-plugin
-Version: 1.2.2
+Version: 1.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: packaging
 Requires-Dist: pillow
 License-File: LICENSE
 Requires-Python: >=3.8
```

