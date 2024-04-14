# Comparing `tmp/pystaleds-0.1.3.tar.gz` & `tmp/pystaleds-0.1.4.tar.gz`

## Comparing `pystaleds-0.1.3.tar` & `pystaleds-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pystaleds-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-04-14 21:53:48.000000 pystaleds-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     1391 2024-04-14 21:53:48.000000 pystaleds-0.1.3/.github/workflows/linting.yml
--rw-r--r--   0     1001      127     2437 2024-04-14 21:53:48.000000 pystaleds-0.1.3/.github/workflows/tests.yml
--rw-r--r--   0     1001      127      686 2024-04-14 21:53:48.000000 pystaleds-0.1.3/.gitignore
--rw-r--r--   0     1001      127    25979 2024-04-14 21:53:48.000000 pystaleds-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127     1062 2024-04-14 21:53:48.000000 pystaleds-0.1.3/LICENSE
--rw-r--r--   0     1001      127     5458 2024-04-14 21:53:48.000000 pystaleds-0.1.3/README.md
--rw-r--r--   0     1001      127     2579 2024-04-14 21:53:48.000000 pystaleds-0.1.3/src/ast_parsing.rs
--rw-r--r--   0     1001      127      324 2024-04-14 21:53:48.000000 pystaleds-0.1.3/src/debug.rs
--rw-r--r--   0     1001      127       69 2024-04-14 21:53:48.000000 pystaleds-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127     5739 2024-04-14 21:53:48.000000 pystaleds-0.1.3/src/main.rs
--rw-r--r--   0     1001      127     6880 2024-04-14 21:53:48.000000 pystaleds-0.1.3/src/parsing.rs
--rw-r--r--   0     1001      127    21679 2024-04-14 21:53:48.000000 pystaleds-0.1.3/src/rules_checking.rs
--rw-r--r--   0     1001      127      188 2024-04-14 21:53:48.000000 pystaleds-0.1.3/test.py
--rw-r--r--   0     1001      127      335 2024-04-14 21:53:48.000000 pystaleds-0.1.3/test_folder/test.py
--rw-r--r--   0     1001      127      152 2024-04-14 21:53:48.000000 pystaleds-0.1.3/test_folder/test_cp.py
--rw-r--r--   0     1001      127      857 2024-04-14 21:53:48.000000 pystaleds-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6155 1970-01-01 00:00:00.000000 pystaleds-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 pystaleds-0.1.4/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-04-14 23:09:20.000000 pystaleds-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     1391 2024-04-14 23:09:20.000000 pystaleds-0.1.4/.github/workflows/linting.yml
+-rw-r--r--   0     1001      127     2437 2024-04-14 23:09:20.000000 pystaleds-0.1.4/.github/workflows/tests.yml
+-rw-r--r--   0     1001      127      686 2024-04-14 23:09:20.000000 pystaleds-0.1.4/.gitignore
+-rw-r--r--   0     1001      127    25979 2024-04-14 23:09:20.000000 pystaleds-0.1.4/Cargo.lock
+-rw-r--r--   0     1001      127     1062 2024-04-14 23:09:20.000000 pystaleds-0.1.4/LICENSE
+-rw-r--r--   0     1001      127     5458 2024-04-14 23:09:20.000000 pystaleds-0.1.4/README.md
+-rw-r--r--   0     1001      127     2714 2024-04-14 23:09:20.000000 pystaleds-0.1.4/src/ast_parsing.rs
+-rw-r--r--   0     1001      127      324 2024-04-14 23:09:20.000000 pystaleds-0.1.4/src/debug.rs
+-rw-r--r--   0     1001      127       69 2024-04-14 23:09:20.000000 pystaleds-0.1.4/src/lib.rs
+-rw-r--r--   0     1001      127     5719 2024-04-14 23:09:20.000000 pystaleds-0.1.4/src/main.rs
+-rw-r--r--   0     1001      127     6880 2024-04-14 23:09:20.000000 pystaleds-0.1.4/src/parsing.rs
+-rw-r--r--   0     1001      127    21679 2024-04-14 23:09:20.000000 pystaleds-0.1.4/src/rules_checking.rs
+-rw-r--r--   0     1001      127      335 2024-04-14 23:09:20.000000 pystaleds-0.1.4/test_folder/test.py
+-rw-r--r--   0     1001      127      152 2024-04-14 23:09:20.000000 pystaleds-0.1.4/test_folder/test_cp.py
+-rw-r--r--   0     1001      127      857 2024-04-14 23:09:20.000000 pystaleds-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     6155 1970-01-01 00:00:00.000000 pystaleds-0.1.4/PKG-INFO
```

### Comparing `pystaleds-0.1.3/Cargo.toml` & `pystaleds-0.1.4/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pystaleds"
-version = "0.1.3"
+version = "0.1.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "pystaleds"
 crate-type = ["lib"]
```

### Comparing `pystaleds-0.1.3/.github/workflows/CI.yml` & `pystaleds-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/.github/workflows/linting.yml` & `pystaleds-0.1.4/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/.github/workflows/tests.yml` & `pystaleds-0.1.4/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/.gitignore` & `pystaleds-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/Cargo.lock` & `pystaleds-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -405,15 +405,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.58",
 ]
 
 [[package]]
 name = "pystaleds"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "cc",
  "clap",
  "glob",
  "pyo3",
  "rayon",
```

### Comparing `pystaleds-0.1.3/LICENSE` & `pystaleds-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/README.md` & `pystaleds-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/src/ast_parsing.rs` & `pystaleds-0.1.4/src/ast_parsing.rs`

 * *Files 18% similar despite different names*

```diff
@@ -21,43 +21,49 @@
         return None;
     }
 
     let params_node = node.child_by_field_name("parameters")?;
     params.clear();
 
     for child in params_node.children(&mut params_node.walk()) {
-        if child.utf8_text(source_code.as_bytes()).unwrap() == "self" {
+        let text = child
+            .utf8_text(source_code.as_bytes())
+            .expect("should be valid utf-8");
+
+        if text == "self" {
             continue;
         }
 
         if child.kind() == "typed_parameter" || child.kind() == "typed_default_parameter" {
             let mut identifier = None;
             let mut typ = None;
 
             let mut d = child.walk();
 
-            for child in child.children(&mut d) {
-                if child.kind() == "identifier" {
-                    identifier = Some(child.utf8_text(source_code.as_bytes()).unwrap());
-                } else if child.kind() == "type" {
-                    typ = Some(child.utf8_text(source_code.as_bytes()).unwrap());
+            for inner_child in child.children(&mut d) {
+                let text_of_inner_child = inner_child
+                    .utf8_text(source_code.as_bytes())
+                    .expect("should be valid utf-8");
+
+                if inner_child.kind() == "identifier" {
+                    identifier = Some(text_of_inner_child);
+                } else if inner_child.kind() == "type" {
+                    typ = Some(text_of_inner_child);
                 }
             }
 
             if let (Some(identifier), Some(typ)) = (identifier, typ) {
                 params.push((identifier, Some(typ)));
             }
         } else if child.kind() == "identifier" {
-            params.push((child.utf8_text(source_code.as_bytes()).unwrap(), None));
+            params.push((text, None));
         } else if child.kind() == "default_parameter" {
-            let (name, _) = child
-                .utf8_text(source_code.as_bytes())
-                .unwrap()
+            let (name, _) = text
                 .split_once('=')
-                .unwrap();
+                .expect("parameter with default value should have '=' in the text");
 
             params.push((name, None));
         }
     }
 
     let mut block = None;
     for child in node.children(&mut node.walk()) {
```

### Comparing `pystaleds-0.1.3/src/main.rs` & `pystaleds-0.1.4/src/main.rs`

 * *Files 5% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     forbid_no_args_in_docstring: bool,
 
     #[arg(long, default_value_t = false, alias = "nu")]
     /// Will consider an error for an arg in docstring to be untyped. Otherwise, only
     /// raises an error if the docstring's type and the signature's type are mismatched.
     forbid_untyped_docstrings: bool,
 
-    #[arg(long, alias = "g")]
+    #[arg(short, long)]
     /// Runs over glob matches considering root to be the path specified in the command.
     /// Disconsiders the allow_hidden flag.
     glob: Option<String>,
 
-    #[arg(long, default_value_t, value_enum, alias = "s")]
+    #[arg(short, long, default_value_t, value_enum)]
     /// Determines the docstring style to consider for parsing.
     docstyle: DocstringStyle,
 }
 
 /// Determines if a file or folder is hidden, i.e. if it starts with '.'.
 fn is_hidden(e: &DirEntry) -> bool {
     e.file_name()
@@ -57,26 +57,26 @@
         .without_time()
         .with_writer(non_blocking)
         .init();
     rayon::ThreadPoolBuilder::new()
         .num_threads(0)
         .stack_size(100_000_000) // TODO: Make the algorithm non-recursive and remove the stack expansion.
         .build_global()
-        .unwrap();
+        .expect("thread pool should be possible to initialize");
 
     let args = Args::parse();
 
     let path = Path::new(&args.path);
 
     let files_with_errors = if let Some(s) = &args.glob {
         set_current_dir(path)?;
 
         let files_with_errors = AtomicU32::new(0);
 
-        let paths = glob(s).unwrap();
+        let paths = glob(s).expect("glob pattern should be valid");
 
         paths.into_iter().par_bridge().for_each(|entry| {
             let Ok(entry) = entry else {
                 return;
             };
 
             let entry = entry.as_path();
@@ -108,16 +108,15 @@
                     let entry = entry.path();
 
                     assess_success(entry, &args, &files_with_errors)
                 });
 
             files_with_errors.into_inner()
         } else {
-            let span = tracing::error_span!("file", file_name = path.as_os_str().to_str().unwrap());
-            _ = span.enter();
+            // In this branch, path is a file.
 
             if is_file_compliant(
                 path,
                 args.break_on_empty_line,
                 args.forbid_no_docstring,
                 args.forbid_no_args_in_docstring,
                 args.forbid_untyped_docstrings,
```

### Comparing `pystaleds-0.1.3/src/parsing.rs` & `pystaleds-0.1.4/src/parsing.rs`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/src/rules_checking.rs` & `pystaleds-0.1.4/src/rules_checking.rs`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/pyproject.toml` & `pystaleds-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pystaleds-0.1.3/PKG-INFO` & `pystaleds-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pystaleds
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Documentation
 License-File: LICENSE
 Summary: CLI tool for checking stale docstrings.
 Keywords: rust,docstrings,pre-commit,cli,tool,testing,ci
```

