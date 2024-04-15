# Comparing `tmp/embed_anything-0.1.7.tar.gz` & `tmp/embed_anything-0.1.8.tar.gz`

## Comparing `embed_anything-0.1.7.tar` & `embed_anything-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 embed_anything-0.1.7/Cargo.toml
--rw-r--r--   0        0        0     3664 2024-04-15 08:59:21.000000 embed_anything-0.1.7/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1123 2024-04-15 08:59:21.000000 embed_anything-0.1.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      752 2024-04-15 08:59:21.000000 embed_anything-0.1.7/.gitignore
--rw-r--r--   0        0        0    95013 2024-04-15 10:05:29.000000 embed_anything-0.1.7/Cargo.lock
--rw-r--r--   0        0        0    35823 2024-04-15 08:59:21.000000 embed_anything-0.1.7/LICENSE
--rw-r--r--   0        0        0     5770 2024-04-15 08:59:21.000000 embed_anything-0.1.7/README.md
--rw-r--r--   0        0        0     1486 2024-04-15 08:59:21.000000 embed_anything-0.1.7/embed_anything.pyi
--rw-r--r--   0        0        0     1940 2024-04-15 08:59:21.000000 embed_anything-0.1.7/examples/clip.rs
--rw-r--r--   0        0        0      223 2024-04-15 09:17:19.000000 embed_anything-0.1.7/python/embed_anything/__init__.py
--rw-r--r--   0        0        0     1486 2024-04-15 09:18:47.000000 embed_anything-0.1.7/python/embed_anything/embed_anything.pyi
--rw-r--r--   0        0        0  2047000 2024-04-15 08:59:21.000000 embed_anything-0.1.7/python/embed_anything/lib/libiomp5md.dll
--rw-r--r--   0        0        0        0 2024-04-15 08:59:21.000000 embed_anything-0.1.7/python/embed_anything/py.typed
--rw-r--r--   0        0        0     3537 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/embedding_model/bert.rs
--rw-r--r--   0        0        0     5765 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/embedding_model/clip.rs
--rw-r--r--   0        0        0     1749 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/embedding_model/embed.rs
--rw-r--r--   0        0        0     3427 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/embedding_model/jina.rs
--rw-r--r--   0        0        0       76 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/embedding_model/mod.rs
--rw-r--r--   0        0        0     1691 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/embedding_model/openai.rs
--rw-r--r--   0        0        0     1422 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/file_embed.rs
--rw-r--r--   0        0        0     4804 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/lib.rs
--rw-r--r--   0        0        0     2390 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/parser.rs
--rw-r--r--   0        0        0      296 2024-04-15 08:59:21.000000 embed_anything-0.1.7/src/pdf_processor.rs
--rw-r--r--   0        0        0      689 2024-04-15 09:18:23.000000 embed_anything-0.1.7/test.py
--rw-r--r--   0        0        0  2224388 2024-04-15 08:59:21.000000 embed_anything-0.1.7/test_files/clip/cat1.jpg
--rw-r--r--   0        0        0     5378 2024-04-15 08:59:21.000000 embed_anything-0.1.7/test_files/clip/cat2.jpeg
--rw-r--r--   0        0        0   121984 2024-04-15 08:59:21.000000 embed_anything-0.1.7/test_files/clip/dog1.jpg
--rw-r--r--   0        0        0     9979 2024-04-15 08:59:21.000000 embed_anything-0.1.7/test_files/clip/dog2.jpeg
--rw-r--r--   0        0        0    42380 2024-04-15 08:59:21.000000 embed_anything-0.1.7/test_files/clip/monkey1.jpg
--rw-r--r--   0        0        0      764 2024-04-15 08:59:21.000000 embed_anything-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6327 1970-01-01 00:00:00.000000 embed_anything-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 embed_anything-0.1.8/Cargo.toml
+-rw-r--r--   0        0        0     3664 2024-04-15 08:59:21.000000 embed_anything-0.1.8/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1123 2024-04-15 08:59:21.000000 embed_anything-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      752 2024-04-15 08:59:21.000000 embed_anything-0.1.8/.gitignore
+-rw-r--r--   0        0        0    95013 2024-04-15 17:42:43.000000 embed_anything-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0    35823 2024-04-15 08:59:21.000000 embed_anything-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4455 2024-04-15 11:00:04.000000 embed_anything-0.1.8/README.md
+-rw-r--r--   0        0        0     1486 2024-04-15 08:59:21.000000 embed_anything-0.1.8/embed_anything.pyi
+-rw-r--r--   0        0        0     1940 2024-04-15 08:59:21.000000 embed_anything-0.1.8/examples/clip.rs
+-rw-r--r--   0        0        0      154 2024-04-15 17:42:14.000000 embed_anything-0.1.8/python/embed_anything/__init__.py
+-rw-r--r--   0        0        0     1486 2024-04-15 09:18:47.000000 embed_anything-0.1.8/python/embed_anything/embed_anything.pyi
+-rw-r--r--   0        0        0  2047000 2024-04-15 08:59:21.000000 embed_anything-0.1.8/python/embed_anything/libiomp5md.dll
+-rw-r--r--   0        0        0        0 2024-04-15 08:59:21.000000 embed_anything-0.1.8/python/embed_anything/py.typed
+-rw-r--r--   0        0        0     3537 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/embedding_model/bert.rs
+-rw-r--r--   0        0        0     5765 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/embedding_model/clip.rs
+-rw-r--r--   0        0        0     1749 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/embedding_model/embed.rs
+-rw-r--r--   0        0        0     3427 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/embedding_model/jina.rs
+-rw-r--r--   0        0        0       76 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/embedding_model/mod.rs
+-rw-r--r--   0        0        0     1691 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/embedding_model/openai.rs
+-rw-r--r--   0        0        0     1422 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/file_embed.rs
+-rw-r--r--   0        0        0     4804 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/lib.rs
+-rw-r--r--   0        0        0     2390 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/parser.rs
+-rw-r--r--   0        0        0      296 2024-04-15 08:59:21.000000 embed_anything-0.1.8/src/pdf_processor.rs
+-rw-r--r--   0        0        0      689 2024-04-15 09:18:23.000000 embed_anything-0.1.8/test.py
+-rw-r--r--   0        0        0  2224388 2024-04-15 08:59:21.000000 embed_anything-0.1.8/test_files/clip/cat1.jpg
+-rw-r--r--   0        0        0     5378 2024-04-15 08:59:21.000000 embed_anything-0.1.8/test_files/clip/cat2.jpeg
+-rw-r--r--   0        0        0   121984 2024-04-15 08:59:21.000000 embed_anything-0.1.8/test_files/clip/dog1.jpg
+-rw-r--r--   0        0        0     9979 2024-04-15 08:59:21.000000 embed_anything-0.1.8/test_files/clip/dog2.jpeg
+-rw-r--r--   0        0        0    42380 2024-04-15 08:59:21.000000 embed_anything-0.1.8/test_files/clip/monkey1.jpg
+-rw-r--r--   0        0        0      764 2024-04-15 08:59:21.000000 embed_anything-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5012 1970-01-01 00:00:00.000000 embed_anything-0.1.8/PKG-INFO
```

### Comparing `embed_anything-0.1.7/Cargo.toml` & `embed_anything-0.1.8/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "embed_anything"
-version = "0.1.7"
+version = "0.1.8"
 edition = "2021"
 
 [lib]
 name = "embed_anything"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `embed_anything-0.1.7/.github/workflows/CI.yml` & `embed_anything-0.1.8/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/.github/workflows/python-publish.yml` & `embed_anything-0.1.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/.gitignore` & `embed_anything-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/Cargo.lock` & `embed_anything-0.1.8/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -712,15 +712,15 @@
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "embed_anything"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "anyhow",
  "candle-core",
  "candle-nn",
  "candle-pyo3",
  "candle-transformers",
  "futures",
```

### Comparing `embed_anything-0.1.7/LICENSE` & `embed_anything-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/embed_anything.pyi` & `embed_anything-0.1.8/embed_anything.pyi`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/examples/clip.rs` & `embed_anything-0.1.8/examples/clip.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/python/embed_anything/embed_anything.pyi` & `embed_anything-0.1.8/python/embed_anything/embed_anything.pyi`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/python/embed_anything/lib/libiomp5md.dll` & `embed_anything-0.1.8/python/embed_anything/libiomp5md.dll`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/embedding_model/bert.rs` & `embed_anything-0.1.8/src/embedding_model/bert.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/embedding_model/clip.rs` & `embed_anything-0.1.8/src/embedding_model/clip.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/embedding_model/embed.rs` & `embed_anything-0.1.8/src/embedding_model/embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/embedding_model/jina.rs` & `embed_anything-0.1.8/src/embedding_model/jina.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/embedding_model/openai.rs` & `embed_anything-0.1.8/src/embedding_model/openai.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/file_embed.rs` & `embed_anything-0.1.8/src/file_embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/lib.rs` & `embed_anything-0.1.8/src/lib.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/src/parser.rs` & `embed_anything-0.1.8/src/parser.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/test.py` & `embed_anything-0.1.8/test.py`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/test_files/clip/cat1.jpg` & `embed_anything-0.1.8/test_files/clip/cat1.jpg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/test_files/clip/cat2.jpeg` & `embed_anything-0.1.8/test_files/clip/cat2.jpeg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/test_files/clip/dog1.jpg` & `embed_anything-0.1.8/test_files/clip/dog1.jpg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/test_files/clip/dog2.jpeg` & `embed_anything-0.1.8/test_files/clip/dog2.jpeg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/test_files/clip/monkey1.jpg` & `embed_anything-0.1.8/test_files/clip/monkey1.jpg`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.7/pyproject.toml` & `embed_anything-0.1.8/pyproject.toml`

 * *Files identical despite different names*

