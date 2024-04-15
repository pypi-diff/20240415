# Comparing `tmp/bean_rs-0.2.2.tar.gz` & `tmp/bean_rs-0.3.0.tar.gz`

## Comparing `bean_rs-0.2.2.tar` & `bean_rs-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 bean_rs-0.2.2/Cargo.toml
--rw-r--r--   0     1001      127      612 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.github/workflows/crates.yml
--rw-r--r--   0     1001      127     3863 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.github/workflows/pypi.yml
--rw-r--r--   0     1001      127      260 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.github/workflows/test.yml
--rw-r--r--   0     1001      127      686 2024-04-09 15:54:02.000000 bean_rs-0.2.2/.gitignore
--rw-r--r--   0     1001      127    36722 2024-04-09 15:54:02.000000 bean_rs-0.2.2/Cargo.lock
--rw-r--r--   0     1001      127     1070 2024-04-09 15:54:02.000000 bean_rs-0.2.2/LICENSE
--rw-r--r--   0     1001      127      342 2024-04-09 15:54:02.000000 bean_rs-0.2.2/Makefile
--rw-r--r--   0     1001      127     1600 2024-04-09 15:54:02.000000 bean_rs-0.2.2/README.md
--rw-r--r--   0     1001      127     1248 2024-04-09 15:54:02.000000 bean_rs-0.2.2/example.bean
--rw-r--r--   0     1001      127     3209 2024-04-09 15:54:02.000000 bean_rs-0.2.2/grammar.pest
--rw-r--r--   0     1001      127    15030 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/book.rs
--rw-r--r--   0     1001      127    23315 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/data.rs
--rw-r--r--   0     1001      127     1090 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/error.rs
--rw-r--r--   0     1001      127       95 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/grammar.rs
--rw-r--r--   0     1001      127      222 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/ledger.rs
--rw-r--r--   0     1001      127     1469 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/lib.rs
--rw-r--r--   0     1001      127     4404 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/loader.rs
--rw-r--r--   0     1001      127     1285 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/main.rs
--rw-r--r--   0     1001      127     2753 2024-04-09 15:54:02.000000 bean_rs-0.2.2/src/utils.rs
--rw-r--r--   0     1001      127      536 2024-04-09 15:54:02.000000 bean_rs-0.2.2/tests/cli.rs
--rw-r--r--   0     1001      127     1327 2024-04-09 15:54:02.000000 bean_rs-0.2.2/tests/integration_test.rs
--rw-r--r--   0     1001      127      459 2024-04-09 15:54:02.000000 bean_rs-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2171 1970-01-01 00:00:00.000000 bean_rs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 bean_rs-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      127      612 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.github/workflows/crates.yml
+-rw-r--r--   0     1001      127     3863 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.github/workflows/pypi.yml
+-rw-r--r--   0     1001      127      260 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127      686 2024-04-15 21:47:40.000000 bean_rs-0.3.0/.gitignore
+-rw-r--r--   0     1001      127    36722 2024-04-15 21:47:40.000000 bean_rs-0.3.0/Cargo.lock
+-rw-r--r--   0     1001      127     1070 2024-04-15 21:47:40.000000 bean_rs-0.3.0/LICENSE
+-rw-r--r--   0     1001      127      381 2024-04-15 21:47:40.000000 bean_rs-0.3.0/Makefile
+-rw-r--r--   0     1001      127     1600 2024-04-15 21:47:40.000000 bean_rs-0.3.0/README.md
+-rw-r--r--   0     1001      127     1248 2024-04-15 21:47:40.000000 bean_rs-0.3.0/example.bean
+-rw-r--r--   0     1001      127     3209 2024-04-15 21:47:40.000000 bean_rs-0.3.0/grammar.pest
+-rw-r--r--   0     1001      127      223 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/bean_rs/__init__.py
+-rw-r--r--   0     1001      127      281 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/bean_rs/bean_rs.pyi
+-rw-r--r--   0     1001      127        0 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/bean_rs/py.typed
+-rw-r--r--   0     1001      127      137 2024-04-15 21:47:40.000000 bean_rs-0.3.0/python/tests/test_load.py
+-rw-r--r--   0     1001      127      421 2024-04-15 21:47:40.000000 bean_rs-0.3.0/requirements-dev.lock
+-rw-r--r--   0     1001      127      207 2024-04-15 21:47:40.000000 bean_rs-0.3.0/requirements.lock
+-rw-r--r--   0     1001      127    15030 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/book.rs
+-rw-r--r--   0     1001      127    23315 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/data.rs
+-rw-r--r--   0     1001      127     1082 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/error.rs
+-rw-r--r--   0     1001      127       95 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/grammar.rs
+-rw-r--r--   0     1001      127      239 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/ledger.rs
+-rw-r--r--   0     1001      127     1494 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      127     4404 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/loader.rs
+-rw-r--r--   0     1001      127     1285 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/main.rs
+-rw-r--r--   0     1001      127     2753 2024-04-15 21:47:40.000000 bean_rs-0.3.0/src/utils.rs
+-rw-r--r--   0     1001      127      536 2024-04-15 21:47:40.000000 bean_rs-0.3.0/tests/cli.rs
+-rw-r--r--   0     1001      127     1327 2024-04-15 21:47:40.000000 bean_rs-0.3.0/tests/integration_test.rs
+-rw-r--r--   0     1001      127     1264 2024-04-15 21:47:40.000000 bean_rs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2303 1970-01-01 00:00:00.000000 bean_rs-0.3.0/PKG-INFO
```

### Comparing `bean_rs-0.2.2/Cargo.toml` & `bean_rs-0.3.0/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "bean-rs"
 license = "MIT"
 authors = ["Chris Arderne <chris@rdrn.me"]
 description = "beancount clone in Rust"
-version = "0.2.2"  # set by Github Actions CI
+version = "0.3.0"  # set by Github Actions CI
 edition = "2021"
 
 [dependencies]
 chrono = "0.4.31"
 clap = { version = "4.4.18", features = ["derive"] }
 env_logger = "0.11.0"
 log = "0.4.20"
```

### Comparing `bean_rs-0.2.2/.github/workflows/crates.yml` & `bean_rs-0.3.0/.github/workflows/crates.yml`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/.github/workflows/pypi.yml` & `bean_rs-0.3.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/.gitignore` & `bean_rs-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/Cargo.lock` & `bean_rs-0.3.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "bean-rs"
-version = "0.2.2"
+version = "0.3.0"
 dependencies = [
  "assert_cmd",
  "chrono",
  "clap",
  "env_logger",
  "log",
  "pest",
```

### Comparing `bean_rs-0.2.2/LICENSE` & `bean_rs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/README.md` & `bean_rs-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/example.bean` & `bean_rs-0.3.0/example.bean`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/grammar.pest` & `bean_rs-0.3.0/grammar.pest`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/src/book.rs` & `bean_rs-0.3.0/src/book.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/src/data.rs` & `bean_rs-0.3.0/src/data.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/src/error.rs` & `bean_rs-0.3.0/src/error.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use pyo3::pyclass;
 use std::fmt;
 
 use crate::data::{DebugLine, Directive};
 
 #[derive(Clone, Debug, Eq, Hash, PartialEq)]
 pub enum ErrorType {
     Badline, // un-parseable line found in input
@@ -12,18 +13,18 @@
     DuplicateOpen,
     DuplicateClose,
     BalanceAssertion,
     UnusedPad,
     InvalidCcy,
 }
 
-#[allow(dead_code)]
-#[derive(Debug)]
+#[pyclass]
+#[derive(Clone, Debug)]
 pub struct BeanError {
-    pub ty: ErrorType, // not yet used anywhere
+    pub ty: ErrorType,
     pub debug: DebugLine,
     pub msg: String,
 }
 
 impl BeanError {
     pub fn new(ty: ErrorType, debug: &DebugLine, msg: &str, dir: Option<&Directive>) -> Self {
         let mut msg = msg.to_owned();
```

### Comparing `bean_rs-0.2.2/src/lib.rs` & `bean_rs-0.3.0/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -41,18 +41,19 @@
     let mut errs = ledger.errs;
     errs.extend(book_errs);
     (bals, errs)
 }
 
 /// Load the ledger from Python
 #[pyfunction]
+#[pyo3(name = "load")]
 fn py_load(path: &str) -> Ledger {
     let text = std::fs::read_to_string(path).expect("cannot read file");
     load(text)
 }
 
-/// `bean_rs` importable from Python
+/// `_bean_rs` importable from Python
 #[pymodule]
-fn bean_rs(m: &Bound<'_, PyModule>) -> PyResult<()> {
+fn _bean_rs(m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_function(wrap_pyfunction!(py_load, m)?)?;
     Ok(())
 }
```

### Comparing `bean_rs-0.2.2/src/loader.rs` & `bean_rs-0.3.0/src/loader.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/src/main.rs` & `bean_rs-0.3.0/src/main.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/src/utils.rs` & `bean_rs-0.3.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/tests/cli.rs` & `bean_rs-0.3.0/tests/cli.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/tests/integration_test.rs` & `bean_rs-0.3.0/tests/integration_test.rs`

 * *Files identical despite different names*

### Comparing `bean_rs-0.2.2/PKG-INFO` & `bean_rs-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.3
 Name: bean-rs
-Version: 0.2.2
+Version: 0.3.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: CPython
 License-File: LICENSE
 Summary: beancount clone in Rust
 Author: Chris Arderne <chris@rdrn.me
 Author-email: Chris Arderne <chris@rdrn.me
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/carderne/signal-export
+Project-URL: repository, https://github.com/carderne/signal-export
 
 # bean-rs
 
 Basic [beancount](https://github.com/beancount/beancount) clone (one day...) in Rust!
 
 Still very very alpha and doesn't do most things that are necessary to be at all useful.
```

