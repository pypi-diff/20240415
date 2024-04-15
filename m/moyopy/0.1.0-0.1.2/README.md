# Comparing `tmp/moyopy-0.1.0.tar.gz` & `tmp/moyopy-0.1.2.tar.gz`

## Comparing `moyopy-0.1.0.tar` & `moyopy-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,65 @@
--rw-r--r--   0     1001      127      481 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/Cargo.toml
--rw-r--r--   0     1001      127     2926 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base/cell.rs
--rw-r--r--   0     1001      127      919 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base/error.rs
--rw-r--r--   0     1001      127     2932 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base/lattice.rs
--rw-r--r--   0     1001      127     3820 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base/operation.rs
--rw-r--r--   0     1001      127      116 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base/tolerance.rs
--rw-r--r--   0     1001      127     9346 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base/transformation.rs
--rw-r--r--   0     1001      127      567 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/base.rs
--rw-r--r--   0     1001      127     8405 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/arithmetic_crystal_class.rs
--rw-r--r--   0     1001      127     7841 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/classification.rs
--rw-r--r--   0     1001      127    19560 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/hall_symbol.rs
--rw-r--r--   0     1001      127    81241 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/hall_symbol_database.rs
--rw-r--r--   0     1001      127     7762 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/point_group.rs
--rw-r--r--   0     1001      127     3370 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/setting.rs
--rw-r--r--   0     1001      127   201241 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data/wyckoff.rs
--rw-r--r--   0     1001      127      740 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/data.rs
--rw-r--r--   0     1001      127    15738 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/identify/point_group.rs
--rw-r--r--   0     1001      127    12712 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/identify/space_group.rs
--rw-r--r--   0     1001      127       75 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/identify.rs
--rw-r--r--   0     1001      127     7233 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/lib.rs
--rw-r--r--   0     1001      127      901 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/cycle_checker.rs
--rw-r--r--   0     1001      127     5124 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/delaunay.rs
--rw-r--r--   0     1001      127     2284 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/elementary.rs
--rw-r--r--   0     1001      127     3797 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/hnf.rs
--rw-r--r--   0     1001      127     2440 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/integer_system.rs
--rw-r--r--   0     1001      127     7889 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/minkowski.rs
--rw-r--r--   0     1001      127    14588 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/niggli.rs
--rw-r--r--   0     1001      127     4889 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math/snf.rs
--rw-r--r--   0     1001      127      386 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/math.rs
--rw-r--r--   0     1001      127    11725 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/search/primitive_cell.rs
--rw-r--r--   0     1001      127     6779 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/search/solve.rs
--rw-r--r--   0     1001      127     9462 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/search/symmetry_search.rs
--rw-r--r--   0     1001      127      156 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/search.rs
--rw-r--r--   0     1001      127    12509 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/symmetrize/standardize.rs
--rw-r--r--   0     1001      127      101 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/src/symmetrize.rs
--rw-r--r--   0     1001      127    12598 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyo/tests/test_moyo_dataset.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 moyopy-0.1.0/moyopy/Cargo.toml
--rw-r--r--   0     1001      127       35 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/README.md
--rw-r--r--   0     1001      127       35 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/python/moyopy/__init__.py
--rw-r--r--   0     1001      127     2273 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127        0 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/python/moyopy/py.typed
--rw-r--r--   0     1001      127      623 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/python/tests/conftest.py
--rw-r--r--   0     1001      127      176 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/python/tests/test_moyo_dataset.py
--rw-r--r--   0     1001      127     3103 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/src/base.rs
--rw-r--r--   0     1001      127      702 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/src/data.rs
--rw-r--r--   0     1001      127     3755 2024-03-11 03:49:14.000000 moyopy-0.1.0/moyopy/src/lib.rs
--rw-r--r--   0     1001      127    21761 2024-03-11 03:49:17.000000 moyopy-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 moyopy-0.1.0/Cargo.toml
--rw-r--r--   0        0        0     1552 1970-01-01 00:00:00.000000 moyopy-0.1.0/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-03-11 03:49:14.000000 moyopy-0.1.0/python/moyopy/py.typed
--rw-r--r--   0     1001      127     2273 2024-03-11 03:49:14.000000 moyopy-0.1.0/python/moyopy/_moyopy.pyi
--rw-r--r--   0     1001      127       35 2024-03-11 03:49:14.000000 moyopy-0.1.0/python/moyopy/__init__.py
--rw-r--r--   0     1001      127       35 2024-03-11 03:49:14.000000 moyopy-0.1.0/README.md
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 moyopy-0.1.0/PKG-INFO
+-rw-r--r--   0     1001      127      903 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/Cargo.toml
+-rw-r--r--   0     1001      127      245 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/README.md
+-rw-r--r--   0     1001      127      703 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/benches/dataset.rs
+-rw-r--r--   0     1001      127     2493 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/benches/translation_search.rs
+-rw-r--r--   0     1001      127     2926 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/cell.rs
+-rw-r--r--   0     1001      127     1123 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/error.rs
+-rw-r--r--   0     1001      127     2932 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/lattice.rs
+-rw-r--r--   0     1001      127     3820 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/operation.rs
+-rw-r--r--   0     1001      127     2146 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/tolerance.rs
+-rw-r--r--   0     1001      127     9891 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base/transformation.rs
+-rw-r--r--   0     1001      127      559 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/base.rs
+-rw-r--r--   0     1001      127     8405 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/arithmetic_crystal_class.rs
+-rw-r--r--   0     1001      127     7841 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/classification.rs
+-rw-r--r--   0     1001      127    20576 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/hall_symbol.rs
+-rw-r--r--   0     1001      127    81241 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/hall_symbol_database.rs
+-rw-r--r--   0     1001      127     7762 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/point_group.rs
+-rw-r--r--   0     1001      127     3370 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/setting.rs
+-rw-r--r--   0     1001      127   201241 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data/wyckoff.rs
+-rw-r--r--   0     1001      127      740 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/data.rs
+-rw-r--r--   0     1001      127    19605 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/identify/point_group.rs
+-rw-r--r--   0     1001      127    13483 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/identify/space_group.rs
+-rw-r--r--   0     1001      127       68 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/identify.rs
+-rw-r--r--   0     1001      127     8765 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/lib.rs
+-rw-r--r--   0     1001      127      901 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/cycle_checker.rs
+-rw-r--r--   0     1001      127     5124 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/delaunay.rs
+-rw-r--r--   0     1001      127     2284 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/elementary.rs
+-rw-r--r--   0     1001      127     3797 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/hnf.rs
+-rw-r--r--   0     1001      127     2440 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/integer_system.rs
+-rw-r--r--   0     1001      127     7889 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/minkowski.rs
+-rw-r--r--   0     1001      127    14588 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/niggli.rs
+-rw-r--r--   0     1001      127     4889 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math/snf.rs
+-rw-r--r--   0     1001      127      344 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/math.rs
+-rw-r--r--   0     1001      127    11991 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search/primitive_cell.rs
+-rw-r--r--   0     1001      127    12095 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search/solve.rs
+-rw-r--r--   0     1001      127    12714 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search/symmetry_search.rs
+-rw-r--r--   0     1001      127      250 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/search.rs
+-rw-r--r--   0     1001      127    14886 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/symmetrize/standardize.rs
+-rw-r--r--   0     1001      127       94 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/src/symmetrize.rs
+-rw-r--r--   0     1001      127     5985 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1185639.json
+-rw-r--r--   0     1001      127     5374 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1197586.json
+-rw-r--r--   0     1001      127     9958 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1201492.json
+-rw-r--r--   0     1001      127      820 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1221598.json
+-rw-r--r--   0     1001      127      735 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-1277787.json
+-rw-r--r--   0     1001      127     3820 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-30665.json
+-rw-r--r--   0     1001      127     1370 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-550745.json
+-rw-r--r--   0     1001      127     5272 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/assets/mp-569901.json
+-rw-r--r--   0     1001      127    20173 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyo/tests/test_moyo_dataset.rs
+-rw-r--r--   0        0        0      682 1970-01-01 00:00:00.000000 moyopy-0.1.2/moyopy/Cargo.toml
+-rw-r--r--   0     1001      127      315 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/README.md
+-rw-r--r--   0     1001      127       37 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127     2504 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127        0 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/moyopy/py.typed
+-rw-r--r--   0     1001      127      623 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/tests/conftest.py
+-rw-r--r--   0     1001      127      394 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/python/tests/test_moyo_dataset.py
+-rw-r--r--   0     1001      127     4934 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/src/base.rs
+-rw-r--r--   0     1001      127      704 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/src/data.rs
+-rw-r--r--   0     1001      127     4119 2024-04-15 03:02:38.000000 moyopy-0.1.2/moyopy/src/lib.rs
+-rw-r--r--   0     1001      127    42754 2024-04-15 03:02:38.000000 moyopy-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 moyopy-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 moyopy-0.1.2/pyproject.toml
+-rw-r--r--   0     1001      127     2504 2024-04-15 03:02:38.000000 moyopy-0.1.2/python/moyopy/_moyopy.pyi
+-rw-r--r--   0     1001      127       37 2024-04-15 03:02:38.000000 moyopy-0.1.2/python/moyopy/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-15 03:02:38.000000 moyopy-0.1.2/python/moyopy/py.typed
+-rw-r--r--   0     1001      127      315 2024-04-15 03:02:38.000000 moyopy-0.1.2/README.md
+-rw-r--r--   0        0        0     1402 1970-01-01 00:00:00.000000 moyopy-0.1.2/PKG-INFO
```

### Comparing `moyopy-0.1.0/moyo/src/base/cell.rs` & `moyopy-0.1.2/moyo/src/base/cell.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/base/lattice.rs` & `moyopy-0.1.2/moyo/src/base/lattice.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/base/operation.rs` & `moyopy-0.1.2/moyo/src/base/operation.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/base/transformation.rs` & `moyopy-0.1.2/moyo/src/base/transformation.rs`

 * *Files 9% similar despite different names*

```diff
@@ -39,14 +39,18 @@
         }
     }
 
     pub fn from_linear(linear: UnimodularLinear) -> Self {
         Self::new(linear, OriginShift::zeros())
     }
 
+    pub fn from_origin_shift(origin_shift: OriginShift) -> Self {
+        Self::new(UnimodularLinear::identity(), origin_shift)
+    }
+
     pub fn linear_as_f64(&self) -> Matrix3<f64> {
         self.linear.map(|e| e as f64)
     }
 
     pub fn transform_lattice(&self, lattice: &Lattice) -> Lattice {
         Lattice::new((lattice.basis * self.linear_as_f64()).transpose())
     }
@@ -107,24 +111,32 @@
         }
     }
 
     pub fn from_linear(linear: Linear) -> Self {
         Self::new(linear, OriginShift::zeros())
     }
 
+    pub fn from_origin_shift(origin_shift: OriginShift) -> Self {
+        Self::new(Linear::identity(), origin_shift)
+    }
+
     pub fn linear_as_f64(&self) -> Matrix3<f64> {
         self.linear.map(|e| e as f64)
     }
 
     pub fn transform_lattice(&self, lattice: &Lattice) -> Lattice {
-        Lattice::new((lattice.basis * self.linear_as_f64()).transpose())
+        self.transform_lattice_with_linear(lattice, &self.linear_as_f64())
     }
 
     pub fn inverse_transform_lattice(&self, lattice: &Lattice) -> Lattice {
-        Lattice::new((lattice.basis * self.linear_inv).transpose())
+        self.transform_lattice_with_linear(lattice, &self.linear_inv)
+    }
+
+    fn transform_lattice_with_linear(&self, lattice: &Lattice, linear: &Matrix3<f64>) -> Lattice {
+        Lattice::new((lattice.basis * linear).transpose())
     }
 
     /// (P, p)^-1 (W, w) (P, p)
     /// This function may decrease the number of operations if the transformation is not compatible with an operation.
     pub fn transform_operations(&self, operations: &Operations) -> Operations {
         let mut new_rotations = vec![];
         let mut new_translations = vec![];
@@ -158,15 +170,15 @@
             .zip(operations.translations.iter())
         {
             if let Some((new_rotation, new_translation)) = transform_operation_as_f64(
                 rotation,
                 translation,
                 &self.linear_inv,
                 &self.linear.map(|e| e as f64),
-                &self.origin_shift,
+                &(-self.linear_as_f64() * self.origin_shift),
             ) {
                 new_rotations.push(new_rotation);
                 new_translations.push(new_translation);
             }
         }
         Operations::new(new_rotations, new_translations)
     }
@@ -213,14 +225,15 @@
         (
             Cell::new(new_lattice, new_positions, new_numbers),
             site_mapping,
         )
     }
 }
 
+/// Transform operation (rotation, translation) by transformation (linear, origin_shift).
 fn transform_operation_as_f64(
     rotation: &Rotation,
     translation: &Translation,
     linear: &Matrix3<f64>,
     linear_inv: &Matrix3<f64>,
     origin_shift: &OriginShift,
 ) -> Option<(Rotation, Translation)> {
```

### Comparing `moyopy-0.1.0/moyo/src/base.rs` & `moyopy-0.1.2/moyo/src/base.rs`

 * *Files 21% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 pub use cell::{AtomicSpecie, Cell, Position};
 pub use error::MoyoError;
 pub use lattice::Lattice;
 pub use operation::{Operations, Permutation, Rotation, Translation};
 pub use tolerance::AngleTolerance;
 pub use transformation::{Linear, OriginShift};
 
-pub(crate) use cell::orbits_from_permutations;
+pub use cell::orbits_from_permutations;
 #[allow(unused_imports)]
-pub(crate) use operation::traverse;
-pub(crate) use tolerance::EPS;
-pub(crate) use transformation::{Transformation, UnimodularLinear, UnimodularTransformation};
+pub use operation::traverse;
+pub use tolerance::{ToleranceHandler, EPS};
+pub use transformation::{Transformation, UnimodularLinear, UnimodularTransformation};
```

### Comparing `moyopy-0.1.0/moyo/src/data/arithmetic_crystal_class.rs` & `moyopy-0.1.2/moyo/src/data/arithmetic_crystal_class.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/data/classification.rs` & `moyopy-0.1.2/moyo/src/data/classification.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/data/hall_symbol.rs` & `moyopy-0.1.2/moyo/src/data/hall_symbol.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::collections::hash_map::Entry;
 use std::collections::{HashMap, VecDeque};
 
 use nalgebra::{matrix, Matrix3, Vector3};
 use strum_macros::EnumIter;
 
 use super::hall_symbol_database::{hall_symbol_entry, HallNumber};
 use crate::base::{Linear, Operations, Rotation, Transformation, Translation, EPS};
@@ -21,14 +22,15 @@
 /// <T>              := [abcnuvwd] | [1-6]  # Table A.1.4.2.3
 /// <V>              := "(" [0-11] [0-11] [0-11] ")"
 #[derive(Debug)]
 pub struct HallSymbol {
     pub hall_symbol: String,
     pub centering: Centering,
     pub centering_translations: Vec<Translation>,
+    /// Generators of the space group except pure translations
     pub generators: Operations,
 }
 
 #[derive(Debug, Copy, Clone, PartialEq, EnumIter)]
 pub enum Centering {
     P, // Primitive
     A, // A-face centered
@@ -167,38 +169,39 @@
         let mut rotations = vec![];
         let mut translations = vec![];
 
         queue.push_back((Rotation::identity(), Translation::zeros()));
 
         while !queue.is_empty() {
             let (rotation_lhs, translation_lhs) = queue.pop_front().unwrap();
-            if hm_translations.contains_key(&rotation_lhs) {
+            let entry = hm_translations.entry(rotation_lhs);
+            if let Entry::Occupied(_) = entry {
                 continue;
             }
-            hm_translations.insert(rotation_lhs, translation_lhs);
+            entry.or_insert(translation_lhs);
             rotations.push(rotation_lhs);
             translations.push(translation_lhs);
 
             for (rotation_rhs, translation_rhs) in self
                 .generators
                 .rotations
                 .iter()
                 .zip(self.generators.translations.iter())
             {
-                let rotation = rotation_lhs * rotation_rhs;
-                let translation =
+                let new_rotation = rotation_lhs * rotation_rhs;
+                let new_translation =
                     rotation_lhs.map(|e| e as f64) * translation_rhs + translation_lhs;
-                let translation_mod1 = translation.map(|e| {
+                let new_translation_mod1 = new_translation.map(|e| {
                     let mut eint = (e * (MAX_DENOMINATOR as f64)).round() as i32;
                     eint = eint.rem_euclid(MAX_DENOMINATOR);
                     (eint as f64) / (MAX_DENOMINATOR as f64)
                 });
 
-                if !hm_translations.contains_key(&rotation) {
-                    queue.push_back((rotation, translation_mod1));
+                if !hm_translations.contains_key(&new_rotation) {
+                    queue.push_back((new_rotation, new_translation_mod1));
                 }
             }
         }
 
         Operations::new(rotations, translations)
     }
 
@@ -257,17 +260,17 @@
             })
             .filter(|s| !s.is_empty())
             .collect::<Vec<&str>>();
         if tokens.len() != 3 {
             return None;
         }
         let origin_shift = Vector3::<f64>::new(
-            (tokens[0].parse::<i32>().unwrap() / MAX_DENOMINATOR) as f64,
-            (tokens[1].parse::<i32>().unwrap() / MAX_DENOMINATOR) as f64,
-            (tokens[2].parse::<i32>().unwrap() / MAX_DENOMINATOR) as f64,
+            tokens[0].parse::<f64>().unwrap() / MAX_DENOMINATOR as f64,
+            tokens[1].parse::<f64>().unwrap() / MAX_DENOMINATOR as f64,
+            tokens[2].parse::<f64>().unwrap() / MAX_DENOMINATOR as f64,
         );
         Some(origin_shift)
     }
 
     fn parse_operation(
         token: &str,
         count: usize,
@@ -555,25 +558,27 @@
             _ => None,
         }
     }
 }
 
 #[cfg(test)]
 mod tests {
+    use nalgebra::{matrix, vector};
     use rstest::rstest;
     use strum::IntoEnumIterator;
 
     use super::{Centering, HallSymbol};
     use crate::base::Transformation;
     use crate::data::hall_symbol_database::iter_hall_symbol_entry;
 
     #[rstest]
     #[case("P 2 2ab -1ab", Centering::P, 0, 3, 8)] // No. 51
     #[case("P 31 2 (0 0 4)", Centering::P, 0, 2, 6)] // No. 151
     #[case("P 65", Centering::P, 0, 1, 6)] // No. 170
+    #[case("P 61 2 (0 0 5)", Centering::P, 0, 2, 12)] // No. 178
     #[case("-P 6c 2c", Centering::P, 0, 3, 24)] // No. 194
     #[case("F 4d 2 3", Centering::F, 3, 3, 24)] // No. 210
     fn test_hall_symbol_small(
         #[case] hall_symbol: &str,
         #[case] lattice_symbol: Centering,
         #[case] num_centering_translations: usize,
         #[case] num_generators: usize,
@@ -584,14 +589,40 @@
         assert_eq!(hs.centering_translations.len(), num_centering_translations);
         assert_eq!(hs.generators.num_operations(), num_generators);
         let operations = hs.traverse();
         assert_eq!(operations.num_operations(), num_operations);
     }
 
     #[test]
+    fn test_hall_symbol_generators() {
+        // No. 178
+        let hs = HallSymbol::new("P 61 2 (0 0 5)").unwrap();
+        let generators = hs.generators;
+        assert_eq!(generators.num_operations(), 2);
+        assert_eq!(
+            generators.rotations[0],
+            matrix![
+                1, -1, 0;
+                1, 0, 0;
+                0, 0, 1;
+            ]
+        );
+        assert_relative_eq!(generators.translations[0], vector![0.0, 0.0, 1.0 / 6.0]);
+        assert_eq!(
+            generators.rotations[1],
+            matrix![
+                0, -1, 0;
+                -1, 0, 0;
+                0, 0, -1;
+            ]
+        );
+        assert_relative_eq!(generators.translations[1], vector![0.0, 0.0, 5.0 / 6.0]);
+    }
+
+    #[test]
     fn test_hall_symbol_whole() {
         for entry in iter_hall_symbol_entry() {
             let hs = HallSymbol::new(entry.hall_symbol).unwrap();
             assert_eq!(48 % hs.traverse().num_operations(), 0);
         }
     }
```

### Comparing `moyopy-0.1.0/moyo/src/data/hall_symbol_database.rs` & `moyopy-0.1.2/moyo/src/data/hall_symbol_database.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/data/point_group.rs` & `moyopy-0.1.2/moyo/src/data/point_group.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/data/setting.rs` & `moyopy-0.1.2/moyo/src/data/setting.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/data/wyckoff.rs` & `moyopy-0.1.2/moyo/src/data/wyckoff.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/data.rs` & `moyopy-0.1.2/moyo/src/data.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/identify/point_group.rs` & `moyopy-0.1.2/moyo/src/identify/point_group.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use std::cmp::Ordering;
 
 use itertools::Itertools;
+use log::debug;
 use nalgebra::{Dyn, Matrix3, OMatrix, OVector, U9};
 
 use crate::base::{MoyoError, Rotation, UnimodularLinear};
 use crate::data::{
     iter_arithmetic_crystal_entry, ArithmeticNumber, Centering, CrystalSystem,
     GeometricCrystalClass, PointGroupRepresentative,
 };
@@ -19,15 +20,16 @@
 }
 
 impl PointGroup {
     /// Identify the arithmetic crystal class from the given rotations and transformation matrix into the representative
     /// Assume the rotations are given in the (reduced) primitive basis
     pub fn new(prim_rotations: &Vec<Rotation>) -> Result<Self, MoyoError> {
         let rotation_types = prim_rotations.iter().map(identify_rotation_type).collect();
-        let geometric_crystal_class = identify_geometric_crystal_class(&rotation_types);
+        let geometric_crystal_class = identify_geometric_crystal_class(&rotation_types)?;
+        debug!("Geometric crystal class: {:?}", geometric_crystal_class);
 
         let crystal_system = CrystalSystem::from_geometric_crystal_class(geometric_crystal_class);
         match crystal_system {
             // Skip triclinic cases as trivial
             CrystalSystem::Triclinic => match geometric_crystal_class {
                 GeometricCrystalClass::C1 => Ok(PointGroup {
                     arithmetic_number: 1,
@@ -220,14 +222,78 @@
             }
         }
     }
 
     Err(MoyoError::ArithmeticCrystalClassIdentificationError)
 }
 
+#[allow(dead_code)]
+pub fn integral_normalizer(
+    prim_rotations: &Vec<Rotation>,
+    prim_generators: &Vec<Rotation>,
+) -> Vec<UnimodularLinear> {
+    let rotation_types = prim_rotations
+        .iter()
+        .map(identify_rotation_type)
+        .collect::<Vec<_>>();
+    let prim_generator_rotation_types = prim_generators
+        .iter()
+        .map(identify_rotation_type)
+        .collect::<Vec<_>>();
+
+    // Try to map generators
+    let order = prim_rotations.len();
+    let candidates: Vec<Vec<usize>> = prim_generator_rotation_types
+        .iter()
+        .map(|&rotation_type| {
+            (0..order)
+                .filter(|&i| rotation_types[i] == rotation_type)
+                .collect()
+        })
+        .collect();
+
+    // TODO: unify with match_with_point_group
+    let mut conjugators = vec![];
+    for pivot in candidates
+        .iter()
+        .map(|v| v.iter())
+        .multi_cartesian_product()
+    {
+        // Solve P^-1 * prim_rotations[prim_rotations[pivot[i]]] * P = prim_generators[i] (for all i)
+        if let Some(trans_mat_basis) = sylvester(
+            &pivot
+                .iter()
+                .map(|&i| prim_rotations[*i])
+                .collect::<Vec<_>>(),
+            &prim_generators,
+        ) {
+            // Search integer linear combination such that the transformation matrix is unimodular
+            // Consider coefficients in [-2, 2], which will be sufficient for Delaunay reduced basis
+            for comb in (0..trans_mat_basis.len())
+                .map(|_| -2..=2)
+                .multi_cartesian_product()
+            {
+                let mut prim_trans_mat = UnimodularLinear::zeros();
+                for (i, matrix) in trans_mat_basis.iter().enumerate() {
+                    prim_trans_mat += comb[i] * matrix;
+                }
+                let det = prim_trans_mat.map(|e| e as f64).determinant().round() as i32;
+                if det < 0 {
+                    prim_trans_mat *= -1;
+                }
+                if det == 1 {
+                    conjugators.push(prim_trans_mat);
+                    break;
+                }
+            }
+        }
+    }
+    conjugators
+}
+
 /// Solve P^-1 * A[i] * P = B[i] (for all i)
 /// vec(A * P - P * B) = (I_3 \otimes A - B^T \otimes I_3) * vec(P)
 fn sylvester(a: &Vec<Matrix3<i32>>, b: &Vec<Matrix3<i32>>) -> Option<Vec<Matrix3<i32>>> {
     let size = a.len();
     assert_eq!(size, b.len());
 
     let mut coeffs = OMatrix::<i32, Dyn, U9>::zeros(9 * size);
@@ -278,15 +344,17 @@
         (-1, -1) => RotationType::RotoInversion4,
         (-2, -1) => RotationType::RotoInversion6,
         _ => unreachable!("Unknown rotation type"),
     }
 }
 
 /// Use look up table in Table 6 of https://arxiv.org/pdf/1808.01590.pdf
-fn identify_geometric_crystal_class(rotation_types: &Vec<RotationType>) -> GeometricCrystalClass {
+fn identify_geometric_crystal_class(
+    rotation_types: &Vec<RotationType>,
+) -> Result<GeometricCrystalClass, MoyoError> {
     // count RotationTypes in point_group
     let mut rotation_types_count = [0; 10];
     for rotation_type in rotation_types {
         match rotation_type {
             RotationType::RotoInversion6 => rotation_types_count[0] += 1,
             RotationType::RotoInversion4 => rotation_types_count[1] += 1,
             RotationType::RotoInversion3 => rotation_types_count[2] += 1,
@@ -297,62 +365,68 @@
             RotationType::Rotation3 => rotation_types_count[7] += 1,
             RotationType::Rotation4 => rotation_types_count[8] += 1,
             RotationType::Rotation6 => rotation_types_count[9] += 1,
         }
     }
     match rotation_types_count {
         // Triclinic
-        [0, 0, 0, 0, 0, 1, 0, 0, 0, 0] => GeometricCrystalClass::C1,
-        [0, 0, 0, 0, 1, 1, 0, 0, 0, 0] => GeometricCrystalClass::Ci,
+        [0, 0, 0, 0, 0, 1, 0, 0, 0, 0] => Ok(GeometricCrystalClass::C1),
+        [0, 0, 0, 0, 1, 1, 0, 0, 0, 0] => Ok(GeometricCrystalClass::Ci),
         // Monoclinic
-        [0, 0, 0, 0, 0, 1, 1, 0, 0, 0] => GeometricCrystalClass::C2,
-        [0, 0, 0, 1, 0, 1, 0, 0, 0, 0] => GeometricCrystalClass::C1h,
-        [0, 0, 0, 1, 1, 1, 1, 0, 0, 0] => GeometricCrystalClass::C2h,
+        [0, 0, 0, 0, 0, 1, 1, 0, 0, 0] => Ok(GeometricCrystalClass::C2),
+        [0, 0, 0, 1, 0, 1, 0, 0, 0, 0] => Ok(GeometricCrystalClass::C1h),
+        [0, 0, 0, 1, 1, 1, 1, 0, 0, 0] => Ok(GeometricCrystalClass::C2h),
         // Orthorhombic
-        [0, 0, 0, 0, 0, 1, 3, 0, 0, 0] => GeometricCrystalClass::D2,
-        [0, 0, 0, 2, 0, 1, 1, 0, 0, 0] => GeometricCrystalClass::C2v,
-        [0, 0, 0, 3, 1, 1, 3, 0, 0, 0] => GeometricCrystalClass::D2h,
+        [0, 0, 0, 0, 0, 1, 3, 0, 0, 0] => Ok(GeometricCrystalClass::D2),
+        [0, 0, 0, 2, 0, 1, 1, 0, 0, 0] => Ok(GeometricCrystalClass::C2v),
+        [0, 0, 0, 3, 1, 1, 3, 0, 0, 0] => Ok(GeometricCrystalClass::D2h),
         // Tetragonal
-        [0, 0, 0, 0, 0, 1, 1, 0, 2, 0] => GeometricCrystalClass::C4,
-        [0, 2, 0, 0, 0, 1, 1, 0, 0, 0] => GeometricCrystalClass::S4,
-        [0, 2, 0, 1, 1, 1, 1, 0, 2, 0] => GeometricCrystalClass::C4h,
-        [0, 0, 0, 0, 0, 1, 5, 0, 2, 0] => GeometricCrystalClass::D4,
-        [0, 0, 0, 4, 0, 1, 1, 0, 2, 0] => GeometricCrystalClass::C4v,
-        [0, 2, 0, 2, 0, 1, 3, 0, 0, 0] => GeometricCrystalClass::D2d,
-        [0, 2, 0, 5, 1, 1, 5, 0, 2, 0] => GeometricCrystalClass::D4h,
+        [0, 0, 0, 0, 0, 1, 1, 0, 2, 0] => Ok(GeometricCrystalClass::C4),
+        [0, 2, 0, 0, 0, 1, 1, 0, 0, 0] => Ok(GeometricCrystalClass::S4),
+        [0, 2, 0, 1, 1, 1, 1, 0, 2, 0] => Ok(GeometricCrystalClass::C4h),
+        [0, 0, 0, 0, 0, 1, 5, 0, 2, 0] => Ok(GeometricCrystalClass::D4),
+        [0, 0, 0, 4, 0, 1, 1, 0, 2, 0] => Ok(GeometricCrystalClass::C4v),
+        [0, 2, 0, 2, 0, 1, 3, 0, 0, 0] => Ok(GeometricCrystalClass::D2d),
+        [0, 2, 0, 5, 1, 1, 5, 0, 2, 0] => Ok(GeometricCrystalClass::D4h),
         // Trigonal
-        [0, 0, 0, 0, 0, 1, 0, 2, 0, 0] => GeometricCrystalClass::C3,
-        [0, 0, 2, 0, 1, 1, 0, 2, 0, 0] => GeometricCrystalClass::C3i,
-        [0, 0, 0, 0, 0, 1, 3, 2, 0, 0] => GeometricCrystalClass::D3,
-        [0, 0, 0, 3, 0, 1, 0, 2, 0, 0] => GeometricCrystalClass::C3v,
-        [0, 0, 2, 3, 1, 1, 3, 2, 0, 0] => GeometricCrystalClass::D3d,
+        [0, 0, 0, 0, 0, 1, 0, 2, 0, 0] => Ok(GeometricCrystalClass::C3),
+        [0, 0, 2, 0, 1, 1, 0, 2, 0, 0] => Ok(GeometricCrystalClass::C3i),
+        [0, 0, 0, 0, 0, 1, 3, 2, 0, 0] => Ok(GeometricCrystalClass::D3),
+        [0, 0, 0, 3, 0, 1, 0, 2, 0, 0] => Ok(GeometricCrystalClass::C3v),
+        [0, 0, 2, 3, 1, 1, 3, 2, 0, 0] => Ok(GeometricCrystalClass::D3d),
         // Hexagonal
-        [0, 0, 0, 0, 0, 1, 1, 2, 0, 2] => GeometricCrystalClass::C6,
-        [2, 0, 0, 1, 0, 1, 0, 2, 0, 0] => GeometricCrystalClass::C3h,
-        [2, 0, 2, 1, 1, 1, 1, 2, 0, 2] => GeometricCrystalClass::C6h,
-        [0, 0, 0, 0, 0, 1, 7, 2, 0, 2] => GeometricCrystalClass::D6,
-        [0, 0, 0, 6, 0, 1, 1, 2, 0, 2] => GeometricCrystalClass::C6v,
-        [2, 0, 0, 4, 0, 1, 3, 2, 0, 0] => GeometricCrystalClass::D3h,
-        [2, 0, 2, 7, 1, 1, 7, 2, 0, 2] => GeometricCrystalClass::D6h,
+        [0, 0, 0, 0, 0, 1, 1, 2, 0, 2] => Ok(GeometricCrystalClass::C6),
+        [2, 0, 0, 1, 0, 1, 0, 2, 0, 0] => Ok(GeometricCrystalClass::C3h),
+        [2, 0, 2, 1, 1, 1, 1, 2, 0, 2] => Ok(GeometricCrystalClass::C6h),
+        [0, 0, 0, 0, 0, 1, 7, 2, 0, 2] => Ok(GeometricCrystalClass::D6),
+        [0, 0, 0, 6, 0, 1, 1, 2, 0, 2] => Ok(GeometricCrystalClass::C6v),
+        [2, 0, 0, 4, 0, 1, 3, 2, 0, 0] => Ok(GeometricCrystalClass::D3h),
+        [2, 0, 2, 7, 1, 1, 7, 2, 0, 2] => Ok(GeometricCrystalClass::D6h),
         // Cubic
-        [0, 0, 0, 0, 0, 1, 3, 8, 0, 0] => GeometricCrystalClass::T,
-        [0, 0, 8, 3, 1, 1, 3, 8, 0, 0] => GeometricCrystalClass::Th,
-        [0, 0, 0, 0, 0, 1, 9, 8, 6, 0] => GeometricCrystalClass::O,
-        [0, 6, 0, 6, 0, 1, 3, 8, 0, 0] => GeometricCrystalClass::Td,
-        [0, 6, 8, 9, 1, 1, 9, 8, 6, 0] => GeometricCrystalClass::Oh,
+        [0, 0, 0, 0, 0, 1, 3, 8, 0, 0] => Ok(GeometricCrystalClass::T),
+        [0, 0, 8, 3, 1, 1, 3, 8, 0, 0] => Ok(GeometricCrystalClass::Th),
+        [0, 0, 0, 0, 0, 1, 9, 8, 6, 0] => Ok(GeometricCrystalClass::O),
+        [0, 6, 0, 6, 0, 1, 3, 8, 0, 0] => Ok(GeometricCrystalClass::Td),
+        [0, 6, 8, 9, 1, 1, 9, 8, 6, 0] => Ok(GeometricCrystalClass::Oh),
         // Unknown
-        _ => unreachable!("Unknown point group"),
+        _ => {
+            debug!(
+                "Unknown geometric crystal class: {:?}",
+                rotation_types_count
+            );
+            Err(MoyoError::GeometricCrystalClassIdentificationError)
+        }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use std::collections::HashSet;
 
-    use super::{PointGroup, PointGroupRepresentative};
+    use super::{integral_normalizer, PointGroup, PointGroupRepresentative};
     use crate::base::traverse;
 
     #[test]
     fn test_point_group_match() {
         for arithmetic_number in 1..=73 {
             let point_group_db =
                 PointGroupRepresentative::from_arithmetic_crystal_class(arithmetic_number);
@@ -386,8 +460,41 @@
                 .map(|r| prim_trans_inv * r * point_group.prim_trans_mat)
                 .collect();
             for rotation in prim_rotations_actual {
                 assert!(prim_rotations_set.contains(&rotation));
             }
         }
     }
+
+    #[test]
+    fn test_integral_normalizer() {
+        for arithmetic_number in 1..=73 {
+            let point_group_db =
+                PointGroupRepresentative::from_arithmetic_crystal_class(arithmetic_number);
+            let prim_generators = point_group_db.primitive_generators();
+            let prim_rotations = traverse(&prim_generators);
+
+            let mut prim_rotations_set = HashSet::new();
+            for rotation in prim_rotations.iter() {
+                prim_rotations_set.insert(rotation.clone());
+            }
+
+            let conjugators = integral_normalizer(&prim_rotations, &prim_generators);
+            assert!(conjugators.len() > 0);
+
+            for linear in conjugators.iter() {
+                let linear_inv = linear
+                    .map(|e| e as f64)
+                    .try_inverse()
+                    .unwrap()
+                    .map(|e| e.round() as i32);
+                let prim_rotations_actual: Vec<_> = prim_rotations
+                    .iter()
+                    .map(|r| linear_inv * r * linear)
+                    .collect();
+                for rotation in prim_rotations_actual {
+                    assert!(prim_rotations_set.contains(&rotation));
+                }
+            }
+        }
+    }
 }
```

### Comparing `moyopy-0.1.0/moyo/src/identify/space_group.rs` & `moyopy-0.1.2/moyo/src/identify/space_group.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 use std::collections::HashMap;
 
+use log::debug;
 use nalgebra::{Dyn, Matrix3, OMatrix, OVector, Vector3, U3};
 
 use super::point_group::PointGroup;
 use crate::base::{MoyoError, Operations, OriginShift, UnimodularLinear, UnimodularTransformation};
 use crate::data::{
-    arithmetic_crystal_class_entry, hall_symbol_entry, ArithmeticNumber, CrystalSystem, HallNumber,
-    HallSymbol, Number, PointGroupRepresentative, Setting,
+    arithmetic_crystal_class_entry, hall_symbol_entry, ArithmeticNumber, GeometricCrystalClass,
+    HallNumber, HallSymbol, Number, PointGroupRepresentative, Setting,
 };
 use crate::math::SNF;
 
 #[derive(Debug)]
 pub struct SpaceGroup {
     pub number: Number,
     pub hall_number: HallNumber,
@@ -24,31 +25,38 @@
     pub fn new(
         prim_operations: &Operations,
         setting: Setting,
         epsilon: f64,
     ) -> Result<Self, MoyoError> {
         // point_group.trans_mat: self -> primitive
         let point_group = PointGroup::new(&prim_operations.rotations)?;
+        debug!(
+            "Arithmetic crystal class: No. {}",
+            point_group.arithmetic_number
+        );
 
         for hall_number in setting.hall_numbers() {
             let entry = hall_symbol_entry(hall_number);
             if entry.arithmetic_number != point_group.arithmetic_number {
                 continue;
             }
 
             let hall_symbol = HallSymbol::from_hall_number(hall_number);
             let db_prim_generators = hall_symbol.primitive_generators();
 
             // Try several correction transformation matrices for monoclinic and orthorhombic
-            for trans_mat_corr in correction_transformation_matrices(point_group.arithmetic_number)
-            {
+            for trans_mat_corr in correction_transformation_matrices(entry.arithmetic_number) {
                 let trans_mat = point_group.prim_trans_mat * trans_mat_corr;
                 if let Some(origin_shift) =
                     match_origin_shift(prim_operations, &trans_mat, &db_prim_generators, epsilon)
                 {
+                    debug!(
+                        "Matched with Hall number {} (No. {})",
+                        hall_number, entry.number
+                    );
                     return Ok(Self {
                         number: entry.number,
                         hall_number,
                         transformation: UnimodularTransformation::new(trans_mat, origin_shift),
                     });
                 }
             }
@@ -59,73 +67,89 @@
 }
 
 fn correction_transformation_matrices(
     arithmetic_number: ArithmeticNumber,
 ) -> Vec<UnimodularLinear> {
     let geometric_crystal_class =
         arithmetic_crystal_class_entry(arithmetic_number).geometric_crystal_class;
-    let crystal_system = CrystalSystem::from_geometric_crystal_class(geometric_crystal_class);
 
-    // conventional -> conventional(cell choice 1 for monoclinic, abc for orthorhombic)
-    let convs = match crystal_system {
-        CrystalSystem::Monoclinic => vec![
-            UnimodularLinear::identity(),
-            // b2 to b1
-            UnimodularLinear::new(
-                0, 0, -1, //
-                0, 1, 0, //
-                1, 0, -1, //
-            ),
-            // b3 to b1
-            UnimodularLinear::new(
-                -1, 0, 1, //
-                0, 1, 0, //
-                -1, 0, 0, //
-            ),
-        ],
-        CrystalSystem::Orthorhombic => vec![
-            // abc
-            UnimodularLinear::identity(),
-            // ba-c
-            UnimodularLinear::new(
-                0, 1, 0, //
-                1, 0, 0, //
-                0, 0, -1, //
-            ),
-            // cab
-            UnimodularLinear::new(
-                0, 0, 1, //
-                1, 0, 0, //
-                0, 1, 0, //
-            ),
-            // -cba
-            UnimodularLinear::new(
-                0, 0, -1, //
-                0, 1, 0, //
-                1, 0, 0, //
-            ),
-            // bca
-            UnimodularLinear::new(
-                0, 1, 0, //
-                0, 0, 1, //
-                1, 0, 0, //
-            ),
-            // a-cb
-            UnimodularLinear::new(
-                1, 0, 0, //
-                0, 0, -1, //
-                0, 1, 0, //
-            ),
-        ],
+    // conventional -> conventional(standard)
+    let convs = match geometric_crystal_class {
+        // Monoclinic crystal system
+        GeometricCrystalClass::C2 | GeometricCrystalClass::C1h | GeometricCrystalClass::C2h => {
+            vec![
+                UnimodularLinear::identity(),
+                // b2 to b1
+                UnimodularLinear::new(
+                    0, 0, -1, //
+                    0, 1, 0, //
+                    1, 0, -1, //
+                ),
+                // b3 to b1
+                UnimodularLinear::new(
+                    -1, 0, 1, //
+                    0, 1, 0, //
+                    -1, 0, 0, //
+                ),
+            ]
+        }
+        // Orthorhombic crystal system
+        GeometricCrystalClass::D2 | GeometricCrystalClass::C2v | GeometricCrystalClass::D2h => {
+            vec![
+                // abc
+                UnimodularLinear::identity(),
+                // ba-c
+                UnimodularLinear::new(
+                    0, 1, 0, //
+                    1, 0, 0, //
+                    0, 0, -1, //
+                ),
+                // cab
+                UnimodularLinear::new(
+                    0, 0, 1, //
+                    1, 0, 0, //
+                    0, 1, 0, //
+                ),
+                // -cba
+                UnimodularLinear::new(
+                    0, 0, -1, //
+                    0, 1, 0, //
+                    1, 0, 0, //
+                ),
+                // bca
+                UnimodularLinear::new(
+                    0, 1, 0, //
+                    0, 0, 1, //
+                    1, 0, 0, //
+                ),
+                // a-cb
+                UnimodularLinear::new(
+                    1, 0, 0, //
+                    0, 0, -1, //
+                    0, 1, 0, //
+                ),
+            ]
+        }
+        // m-3
+        GeometricCrystalClass::Th => {
+            vec![
+                UnimodularLinear::identity(),
+                UnimodularLinear::new(
+                    0, 0, 1, //
+                    0, -1, 0, //
+                    1, 0, 0, //
+                ),
+            ]
+        }
         _ => vec![UnimodularLinear::identity()],
     };
 
-    // primitive -> conventional -> conventional(cell choice 1 for monoclinic, abc for orthorhombic) -> primitive
-    let centering =
-        PointGroupRepresentative::from_arithmetic_crystal_class(arithmetic_number).centering;
+    // primitive -> conventional -> conventional(standard) -> primitive
+    let point_group = PointGroupRepresentative::from_arithmetic_crystal_class(arithmetic_number);
+    let centering = point_group.centering;
     let corrections: Vec<UnimodularLinear> = convs
         .iter()
         .map(|trans_corr| {
             let corr = (centering.linear() * trans_corr).map(|e| e as f64) * centering.inverse();
             corr.map(|e| e.round() as i32)
         })
         .filter(|corr| corr.map(|e| e as f64).determinant().round() as i32 == 1)
@@ -164,32 +188,30 @@
     for (k, (rotation, other_translation)) in db_prim_generators
         .rotations
         .iter()
         .zip(db_prim_generators.translations.iter())
         .enumerate()
     {
         // Correction transformation matrix may not be normalizer of the point group. For example, mm2 -> 2mm
-        if !hm_translations.contains_key(rotation) {
-            return None;
-        }
+        let target_translation = hm_translations.get(rotation)?;
 
-        let target_translation = hm_translations.get(rotation).unwrap();
         let ak = rotation - Matrix3::<i32>::identity();
         let bk = other_translation - target_translation;
         for i in 0..3 {
             for j in 0..3 {
                 a[(3 * k + i, j)] = ak[(i, j)];
             }
             b[3 * k + i] = bk[i];
         }
     }
 
     match solve_mod1(&a, &b, epsilon) {
         Some(s) => {
             let origin_shift = (trans_mat.map(|e| e as f64) * s).map(|e| e % 1.);
+
             Some(origin_shift)
         }
         None => None,
     }
 }
 
 /// Solve a * x = b (mod 1)
```

### Comparing `moyopy-0.1.0/moyo/src/lib.rs` & `moyopy-0.1.2/moyo/src/lib.rs`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #[allow(unused_imports)]
 #[macro_use]
 extern crate approx;
 
 pub mod base;
 pub mod data;
-
-mod identify;
-mod math;
-mod search;
-mod symmetrize;
+pub mod identify;
+pub mod math;
+pub mod search;
+pub mod symmetrize;
 
 use nalgebra::Matrix3;
 
-use crate::base::{AngleTolerance, Cell, MoyoError, Operations, OriginShift, Transformation};
+use crate::base::{
+    AngleTolerance, Cell, MoyoError, Operations, OriginShift, ToleranceHandler, Transformation,
+};
 use crate::data::{HallNumber, Number, Setting};
 use crate::identify::SpaceGroup;
 use crate::search::{PrimitiveCell, PrimitiveSymmetrySearch};
 use crate::symmetrize::{orbits_in_cell, StandardizedCell};
 
 #[derive(Debug)]
 pub struct MoyoDataset {
@@ -58,27 +59,30 @@
     /// Linear part of transformation from the input cell to the primitive standardized cell.
     pub prim_std_linear: Matrix3<f64>,
     /// Origin shift of transformation from the input cell to the primitive standardized cell.
     pub prim_std_origin_shift: OriginShift,
     /// Mapping sites in the input cell to those in the primitive standardized cell.
     /// The `i`th atom in the input cell is mapped to the `mapping_to_std_prim[i]`th atom in the primitive standardized cell.
     pub mapping_std_prim: Vec<usize>,
+    // ------------------------------------------------------------------------
+    // Final parameters
+    // ------------------------------------------------------------------------
+    pub symprec: f64,
+    pub angle_tolerance: AngleTolerance,
 }
 
 impl MoyoDataset {
     pub fn new(
         cell: &Cell,
         symprec: f64,
         angle_tolerance: AngleTolerance,
         setting: Setting,
     ) -> Result<Self, MoyoError> {
-        // Symmetry search
-        let prim_cell = PrimitiveCell::new(cell, symprec)?;
-        let symmetry_search =
-            PrimitiveSymmetrySearch::new(&prim_cell.cell, symprec, angle_tolerance)?;
+        let (prim_cell, symmetry_search, symprec, angle_tolerance) =
+            iterative_symmetry_search(cell, symprec, angle_tolerance)?;
         let operations = operations_in_cell(&prim_cell, &symmetry_search.operations);
 
         // Space-group type identification
         let epsilon = symprec / prim_cell.cell.lattice.volume().powf(1.0 / 3.0);
         let space_group = SpaceGroup::new(&symmetry_search.operations, setting, epsilon)?;
 
         // Standardized cell
@@ -135,22 +139,59 @@
             // Site symmetry
             orbits,
             wyckoffs: wyckoffs.iter().map(|w| w.letter).collect(),
             site_symmetry_symbols: wyckoffs
                 .iter()
                 .map(|w| w.site_symmetry.to_string())
                 .collect(),
+            // Final parameters
+            symprec,
+            angle_tolerance,
         })
     }
 
     pub fn num_operations(&self) -> usize {
         self.operations.num_operations()
     }
 }
 
+const MAX_SYMMETRY_SEARCH_TRIALS: usize = 16;
+
+fn iterative_symmetry_search(
+    cell: &Cell,
+    symprec: f64,
+    angle_tolerance: AngleTolerance,
+) -> Result<(PrimitiveCell, PrimitiveSymmetrySearch, f64, AngleTolerance), MoyoError> {
+    let mut tolerance_handler = ToleranceHandler::new(symprec, angle_tolerance);
+
+    for _ in 0..MAX_SYMMETRY_SEARCH_TRIALS {
+        match PrimitiveCell::new(cell, tolerance_handler.symprec) {
+            Ok(prim_cell) => {
+                match PrimitiveSymmetrySearch::new(
+                    &prim_cell.cell,
+                    tolerance_handler.symprec,
+                    tolerance_handler.angle_tolerance,
+                ) {
+                    Ok(symmetry_search) => {
+                        return Ok((
+                            prim_cell,
+                            symmetry_search,
+                            tolerance_handler.symprec,
+                            tolerance_handler.angle_tolerance,
+                        ));
+                    }
+                    Err(err) => tolerance_handler.update(err),
+                }
+            }
+            Err(err) => tolerance_handler.update(err),
+        }
+    }
+    Err(MoyoError::PrimitiveSymmetrySearchError)
+}
+
 fn operations_in_cell(prim_cell: &PrimitiveCell, prim_operations: &Operations) -> Operations {
     let mut rotations = vec![];
     let mut translations = vec![];
     let input_operations =
         Transformation::from_linear(prim_cell.linear).transform_operations(prim_operations);
     for t1 in prim_cell.translations.iter() {
         for (rotation, t2) in input_operations
```

### Comparing `moyopy-0.1.0/moyo/src/math/cycle_checker.rs` & `moyopy-0.1.2/moyo/src/math/cycle_checker.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/delaunay.rs` & `moyopy-0.1.2/moyo/src/math/delaunay.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/elementary.rs` & `moyopy-0.1.2/moyo/src/math/elementary.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/hnf.rs` & `moyopy-0.1.2/moyo/src/math/hnf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/integer_system.rs` & `moyopy-0.1.2/moyo/src/math/integer_system.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/minkowski.rs` & `moyopy-0.1.2/moyo/src/math/minkowski.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/niggli.rs` & `moyopy-0.1.2/moyo/src/math/niggli.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/math/snf.rs` & `moyopy-0.1.2/moyo/src/math/snf.rs`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyo/src/search/primitive_cell.rs` & `moyopy-0.1.2/moyo/src/search/primitive_cell.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use std::collections::BTreeMap;
 
+use log::{debug, warn};
 use nalgebra::{Dyn, Matrix3, OMatrix, Vector3, U3};
 
 use super::solve::{
     pivot_site_indices, solve_correspondence, symmetrize_translation_from_permutation,
+    PeriodicKdTree,
 };
 use crate::base::{
     orbits_from_permutations, Cell, Linear, MoyoError, Permutation, Position, Rotation,
     Transformation, Translation, UnimodularTransformation, EPS,
 };
 use crate::math::HNF;
 
@@ -39,38 +41,38 @@
         let minimum_basis_norm = reduced_lattice
             .basis
             .column_iter()
             .map(|v| v.norm())
             .fold(f64::INFINITY, f64::min);
         let rough_symprec = 2.0 * symprec;
         if rough_symprec > minimum_basis_norm / 2.0 {
-            return Err(MoyoError::TooSmallSymprecError);
+            warn!("symprec is too large compared to the basis vectors. Consider reducing symprec.");
+            return Err(MoyoError::TooLargeToleranceError);
         }
 
         // Try possible translations: overlap the `src`the site to the `dst`th site
+        let pkdtree = PeriodicKdTree::new(&reduced_cell, rough_symprec);
         let pivot_site_indices = pivot_site_indices(&reduced_cell.numbers);
         let mut permutations_translations_tmp = vec![];
         let src = pivot_site_indices[0];
         for dst in pivot_site_indices.iter() {
             let translation = reduced_cell.positions[*dst] - reduced_cell.positions[src];
             let new_positions: Vec<Position> = reduced_cell
                 .positions
                 .iter()
                 .map(|pos| pos + translation)
                 .collect();
 
             // Because the translation may not be optimal to minimize distance between input and acted positions,
             // use a larger symprec (diameter of a Ball) for finding correspondence
-            if let Some(permutation) =
-                solve_correspondence(&reduced_cell, &new_positions, rough_symprec)
+            if let Some(permutation) = solve_correspondence(&pkdtree, &reduced_cell, &new_positions)
             {
                 permutations_translations_tmp.push((permutation, translation));
             }
         }
-        assert!(!permutations_translations_tmp.is_empty());
 
         // Purify translations by permutations
         let mut translations = vec![];
         let mut permutations = vec![];
         for (permutation, rough_translation) in permutations_translations_tmp.iter() {
             let (translation, distance) = symmetrize_translation_from_permutation(
                 &reduced_cell,
@@ -81,18 +83,19 @@
             if distance < symprec {
                 translations.push(translation);
                 permutations.push(permutation.clone());
             }
         }
 
         let size = translations.len() as i32;
-        assert!(size > 0);
-        if reduced_cell.num_atoms() % (size as usize) != 0 {
-            return Err(MoyoError::PrimitiveCellError);
+        if (size == 0) || (reduced_cell.num_atoms() % (size as usize) != 0) {
+            warn!("Failed to properly find translations: {} translations in {} atoms. Consider increasing symprec.", size, reduced_cell.num_atoms());
+            return Err(MoyoError::TooSmallToleranceError);
         }
+        debug!("Found {} pure translations", size);
 
         // Recover a transformation matrix from primitive to input cell
         let mut columns: Vec<Vector3<i32>> = vec![
             Vector3::new(size, 0, 0),
             Vector3::new(0, size, 0),
             Vector3::new(0, 0, size),
         ];
@@ -109,42 +112,39 @@
             .ok_or(MoyoError::PrimitiveCellError)?
             .map(|e| e.round() as i32);
         if relative_ne!(
             trans_mat.map(|e| e as f64).determinant(),
             size as f64,
             epsilon = EPS
         ) {
-            return Err(MoyoError::PrimitiveCellError);
+            warn!("Failed to find a transformation matrix to a primitive cell. Consider increasing symprec.");
+            return Err(MoyoError::TooSmallToleranceError);
         }
 
         // Primitive cell
         let (primitive_cell, site_mapping) = primitive_cell_from_transformation(
             &reduced_cell,
             &trans_mat,
             &translations,
             &permutations,
-        )
-        .ok_or(MoyoError::PrimitiveCellError)?;
+        );
         let (_, prim_trans_mat) = primitive_cell.lattice.minkowski_reduce()?;
         let reduced_prim_cell =
             UnimodularTransformation::from_linear(prim_trans_mat).transform_cell(&primitive_cell);
 
         // (input cell)
         //    -[reduced_trans_mat]-> (reduced cell)
         //    <-[trans_mat]- (primitive cell)
         //    -[prim_trans_mat]-> (reduced primitive cell)
         let inv_prim_trans_mat = prim_trans_mat
             .map(|e| e as f64)
             .try_inverse()
             .unwrap()
             .map(|e| e.round() as i32);
-        let inv_reduced_trans_mat = reduced_trans_mat
-            .map(|e| e as f64)
-            .try_inverse()
-            .ok_or(MoyoError::PrimitiveCellError)?;
+        let inv_reduced_trans_mat = reduced_trans_mat.map(|e| e as f64).try_inverse().unwrap();
         Ok(Self {
             cell: reduced_prim_cell,
             linear: ((inv_prim_trans_mat * trans_mat).map(|e| e as f64) * inv_reduced_trans_mat)
                 .map(|e| e.round() as i32),
             site_mapping,
             translations: translations
                 .iter()
@@ -157,15 +157,15 @@
 
 /// Transform `cell` to a primitive cell by inverse of `trans_mat`
 fn primitive_cell_from_transformation(
     cell: &Cell,
     trans_mat: &Linear,
     translations: &Vec<Translation>,
     permutations: &[Permutation],
-) -> Option<(Cell, Vec<usize>)> {
+) -> (Cell, Vec<usize>) {
     let new_lattice =
         Transformation::from_linear(*trans_mat).inverse_transform_lattice(&cell.lattice);
 
     let num_atoms = cell.num_atoms();
     let orbits = orbits_from_permutations(num_atoms, permutations);
     let representatives = (0..num_atoms)
         .filter(|&i| orbits[i] == i)
@@ -189,24 +189,26 @@
         new_positions[i] = trans_mat.map(|e| e as f64)
             * (cell.positions[orbit_i] + acc / (translations.len() as f64));
         new_numbers[i] = cell.numbers[orbit_i];
     }
 
     let primitive_cell = Cell::new(new_lattice, new_positions, new_numbers);
     let site_mapping = site_mapping_from_orbits(&orbits);
-    Some((primitive_cell, site_mapping))
+    (primitive_cell, site_mapping)
 }
 
-#[allow(clippy::map_entry)]
 fn site_mapping_from_orbits(orbits: &[usize]) -> Vec<usize> {
     let mut mapping = BTreeMap::new();
+    let mut count = 0;
     for ri in orbits.iter() {
-        if !mapping.contains_key(&ri) {
-            mapping.insert(ri, mapping.len());
-        }
+        mapping.entry(ri).or_insert_with(|| {
+            let value = count;
+            count += 1;
+            value
+        });
     }
 
     orbits.iter().map(|ri| *mapping.get(&ri).unwrap()).collect()
 }
 
 #[cfg(test)]
 mod tests {
@@ -295,16 +297,14 @@
                 Vector3::new(2.0 / 3.0, 1.0 / 3.0, 1.0 / 3.0 + 0.1),
                 Vector3::new(1.0 / 3.0, 2.0 / 3.0, 2.0 / 3.0 + 0.1),
             ],
             vec![0, 0, 0, 0, 0, 0],
         );
         let symprec = 1e-4;
         let prim_cell = PrimitiveCell::new(&cell, symprec).unwrap();
-        dbg!(prim_cell.cell.lattice.volume());
-        dbg!(cell.lattice.volume());
 
         assert_relative_eq!(
             prim_cell.cell.lattice.basis * prim_cell.linear.map(|e| e as f64),
             cell.lattice.basis,
             epsilon = 1e-8
         );
     }
```

### Comparing `moyopy-0.1.0/moyo/src/search/symmetry_search.rs` & `moyopy-0.1.2/moyo/src/search/symmetry_search.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 use itertools::iproduct;
-use std::collections::HashSet;
+use std::collections::{HashMap, HashSet, VecDeque};
 
+use log::{debug, warn};
 use nalgebra::{Matrix3, Vector3};
 
 use super::solve::{
     pivot_site_indices, solve_correspondence, symmetrize_translation_from_permutation,
+    PeriodicKdTree,
 };
 use crate::base::{
-    AngleTolerance, Cell, Lattice, MoyoError, Operations, Permutation, Position, Rotation, EPS,
+    traverse, AngleTolerance, Cell, Lattice, MoyoError, Operations, Permutation, Position,
+    Rotation, Translation, EPS,
 };
 
 #[derive(Debug)]
 pub struct PrimitiveSymmetrySearch {
     /// Operations in the given primitive cell
     pub operations: Operations,
     pub permutations: Vec<Permutation>,
     pub bravais_group: Vec<Rotation>,
 }
 
 impl PrimitiveSymmetrySearch {
     /// Return coset representatives of the space group w.r.t. its translation subgroup.
     /// Assume `primitive_cell` is a primitive cell and its basis vectors are Minkowski reduced.
+    /// Returned operations are guaranteed to form a group.
+    /// If the group closure and tolerance (symprec and angle_tolerance) are incompatible, the former is prioritized.
     /// Possible replacements for spglib/src/spacegroup.h::spa_search_spacegroup
     pub fn new(
         primitive_cell: &Cell,
         symprec: f64,
         angle_tolerance: AngleTolerance,
     ) -> Result<Self, MoyoError> {
         // Check if symprec is sufficiently small
         let minimum_basis_norm = primitive_cell.lattice.basis.column(0).norm();
         let rough_symprec = 2.0 * symprec;
         if rough_symprec > minimum_basis_norm / 2.0 {
-            return Err(MoyoError::TooSmallSymprecError);
+            warn!("symprec is too large compared to the basis vectors. Consider reducing symprec.");
+            return Err(MoyoError::TooLargeToleranceError);
         }
 
         // Search symmetry operations
+        let pkdtree = PeriodicKdTree::new(primitive_cell, rough_symprec);
         let bravais_group =
             search_bravais_group(&primitive_cell.lattice, symprec, angle_tolerance)?;
         let pivot_site_indices = pivot_site_indices(&primitive_cell.numbers);
         let mut symmetries_tmp = vec![];
         let src = pivot_site_indices[0];
         for rotation in bravais_group.iter() {
             for dst in pivot_site_indices.iter() {
@@ -48,45 +55,110 @@
                 let new_positions: Vec<Position> = primitive_cell
                     .positions
                     .iter()
                     .map(|pos| rotation.map(|e| e as f64) * pos + translation)
                     .collect();
 
                 if let Some(permutation) =
-                    solve_correspondence(primitive_cell, &new_positions, rough_symprec)
+                    solve_correspondence(&pkdtree, primitive_cell, &new_positions)
                 {
                     symmetries_tmp.push((*rotation, translation, permutation));
-                    // If a translation part is found, it should be unique (up to lattice translations)
-                    break;
+                    // Do not break here because there may be multiple translations with the rough tolerance
                 }
             }
         }
-        assert!(!symmetries_tmp.is_empty());
+        debug!(
+            "Number of symmetry operation candidates: {}",
+            symmetries_tmp.len()
+        );
 
         // Purify symmetry operations by permutations
-        let mut rotations = vec![];
-        let mut translations = vec![];
-        let mut permutations = vec![];
+        let mut operations_and_permutations = vec![];
         for (rotation, rough_translation, permutation) in symmetries_tmp.iter() {
             let (translation, distance) = symmetrize_translation_from_permutation(
                 primitive_cell,
                 permutation,
                 rotation,
                 rough_translation,
             );
             if distance < symprec {
-                rotations.push(*rotation);
-                translations.push(translation);
-                permutations.push(permutation.clone());
+                operations_and_permutations.push((rotation, translation, permutation.clone()));
+            }
+        }
+        if operations_and_permutations.is_empty() {
+            warn!(
+                "No symmetry operations are found. Consider increasing symprec and angle_tolerance."
+            );
+            return Err(MoyoError::TooSmallToleranceError);
+        }
+
+        // Recover operations by group multiplication
+        let mut queue = VecDeque::new();
+        let mut visited = HashSet::new();
+        let mut rotations = vec![];
+        let mut translations = vec![];
+        let mut permutations = vec![];
+        queue.push_back((
+            Rotation::identity(),
+            Translation::zeros(),
+            Permutation::identity(primitive_cell.num_atoms()),
+        ));
+        while !queue.is_empty() {
+            let (rotation_lhs, translation_lhs, permutation_lhs) = queue.pop_front().unwrap();
+            if visited.contains(&rotation_lhs) {
+                continue;
+            }
+            visited.insert(rotation_lhs);
+            rotations.push(rotation_lhs);
+            translations.push(translation_lhs);
+            permutations.push(permutation_lhs.clone());
+
+            for (&rotation_rhs, translation_rhs, permutation_rhs) in
+                operations_and_permutations.iter()
+            {
+                let new_rotation = rotation_lhs * rotation_rhs;
+                let new_translation = (rotation_lhs.map(|e| e as f64) * translation_rhs
+                    + translation_lhs)
+                    .map(|e| e - e.round());
+                let new_permutation = permutation_lhs.clone() * permutation_rhs.clone();
+                queue.push_back((new_rotation, new_translation, new_permutation));
             }
         }
-        if rotations.is_empty() {
-            return Err(MoyoError::PrimitiveSymmetrySearchError);
+        if rotations.len() != operations_and_permutations.len() {
+            warn!("Found operations do not form a group. Consider reducing symprec and angle_tolerance.");
+            return Err(MoyoError::TooLargeToleranceError);
         }
 
+        // Check closure
+        let mut translations_map = HashMap::new();
+        for (rotation, translation) in rotations.iter().zip(translations.iter()) {
+            translations_map.insert(rotation.clone(), translation.clone());
+        }
+        let mut closed = true;
+        for (r1, t1) in rotations.iter().zip(translations.iter()) {
+            if !closed {
+                break;
+            }
+            for (r2, t2) in rotations.iter().zip(translations.iter()) {
+                // (r1, t1) * (r2, t2) = (r1 * r2, r1 * t2 + t1)
+                let r = r1 * r2;
+                let t = r1.map(|e| e as f64) * t2 + t1;
+                let diff = (translations_map[&r] - t).map(|e| e - e.round());
+                if primitive_cell.lattice.cartesian_coords(&diff).norm() > rough_symprec {
+                    closed = false;
+                    break;
+                }
+            }
+        }
+        if !closed {
+            warn!("Some centering translations are missing. Consider reducing symprec and angle_tolerance.");
+            return Err(MoyoError::TooLargeToleranceError);
+        }
+
+        debug!("Order of point group: {}", rotations.len());
         Ok(Self {
             operations: Operations::new(rotations, translations),
             permutations,
             bravais_group,
         })
     }
 }
@@ -180,31 +252,22 @@
                 continue;
             }
 
             rotations.push(rotation);
         }
     }
 
-    if rotations.is_empty() {
-        return Err(MoyoError::BravaisGroupSearchError);
-    }
-
-    // Check to reproduce rotation operations by group multiplication
-    let mut rotation_set = HashSet::new();
-    for rotation in rotations.iter() {
-        rotation_set.insert(*rotation);
+    // Recover rotations by group multiplication
+    let complemented_rotations = traverse(&rotations);
+    if complemented_rotations.len() != rotations.len() {
+        warn!("Found automorphisms for the lattice do not form a group. Consider reducing symprec and angle_tolerance.");
+        return Err(MoyoError::TooLargeToleranceError);
     }
-    for (r1, r2) in iproduct!(rotation_set.iter(), rotation_set.iter()) {
-        let r12 = r1 * r2;
-        if !rotation_set.contains(&r12) {
-            return Err(MoyoError::BravaisGroupSearchError);
-        }
-    }
-
-    Ok(rotations)
+    debug!("Order of Bravais group: {}", complemented_rotations.len());
+    Ok(complemented_rotations)
 }
 
 /// Compare (basis.column(col1), basis.column(col2)) and (b1, b2)
 /// Return true if these pairs of vectors are close enough
 fn compare_nondiagonal_matrix_tensor_element(
     basis: &Matrix3<f64>,
     b1: &Vector3<f64>,
```

### Comparing `moyopy-0.1.0/moyo/src/symmetrize/standardize.rs` & `moyopy-0.1.2/moyo/src/symmetrize/standardize.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use itertools::{iproduct, izip};
+use log::warn;
 use nalgebra::linalg::{Cholesky, QR};
 use nalgebra::{vector, Matrix3, Vector3};
 use std::collections::HashMap;
 
 use crate::base::{
     orbits_from_permutations, Cell, Lattice, MoyoError, Operations, Permutation, Position,
     Rotation, Transformation, UnimodularTransformation, EPS,
@@ -37,48 +38,146 @@
     /// TODO: option not to rotate basis vectors
     pub fn new(
         prim_cell: &PrimitiveCell,
         symmetry_search: &PrimitiveSymmetrySearch,
         space_group: &SpaceGroup,
         symprec: f64,
     ) -> Result<Self, MoyoError> {
+        let (
+            prim_std_cell,
+            prim_std_permutations,
+            prim_transformation,
+            std_cell,
+            transformation,
+            rotation_matrix,
+            site_mapping,
+        ) = Self::standardize_and_symmetrize_cell(prim_cell, symmetry_search, space_group)?;
+
+        let wyckoffs = Self::assign_wyckoffs(
+            &prim_std_cell,
+            &prim_std_permutations,
+            &std_cell,
+            &site_mapping,
+            space_group.hall_number,
+            symprec,
+        )?;
+
+        Ok(StandardizedCell {
+            prim_cell: prim_std_cell,
+            prim_transformation,
+            cell: std_cell,
+            wyckoffs,
+            transformation,
+            rotation_matrix,
+            site_mapping,
+        })
+    }
+
+    #[allow(clippy::type_complexity)]
+    fn standardize_and_symmetrize_cell(
+        prim_cell: &PrimitiveCell,
+        symmetry_search: &PrimitiveSymmetrySearch,
+        space_group: &SpaceGroup,
+    ) -> Result<
+        (
+            Cell,
+            Vec<Permutation>,
+            UnimodularTransformation,
+            Cell,
+            Transformation,
+            Matrix3<f64>,
+            Vec<usize>,
+        ),
+        MoyoError,
+    > {
         let entry = hall_symbol_entry(space_group.hall_number);
         let arithmetic_number = entry.arithmetic_number;
         let bravais_class = arithmetic_crystal_class_entry(arithmetic_number).bravais_class;
         let lattice_system = LatticeSystem::from_bravais_class(bravais_class);
 
         // To standardized primitive cell
         let prim_transformation = match lattice_system {
             LatticeSystem::Triclinic => {
                 let (_, linear) = prim_cell.cell.lattice.niggli_reduce()?;
                 UnimodularTransformation::from_linear(linear)
             }
             _ => space_group.transformation.clone(),
         };
-        let new_prim_positions = symmetrize_positions(
-            &prim_cell.cell,
-            &symmetry_search.operations,
-            &symmetry_search.permutations,
+        let prim_std_cell_tmp = prim_transformation.transform_cell(&prim_cell.cell);
+
+        // Symmetrize positions of prim_std_cell by refined symmetry operations
+        // - Prepare operations in primitive standard
+        let hs = HallSymbol::from_hall_number(space_group.hall_number);
+        let conv_std_operations = hs.traverse();
+        let prim_std_operations = Transformation::from_linear(entry.centering.linear())
+            .inverse_transform_operations(&conv_std_operations);
+
+        // - Reorder permutations
+        let mut permutation_mapping = HashMap::new();
+        let prim_operations = prim_transformation.transform_operations(&symmetry_search.operations);
+        for (prim_rotation, permutation) in izip!(
+            prim_operations.rotations.iter(),
+            symmetry_search.permutations.iter()
+        ) {
+            permutation_mapping.insert(*prim_rotation, permutation.clone());
+        }
+        let prim_std_permutations = prim_std_operations
+            .rotations
+            .iter()
+            .map(|rotation| permutation_mapping.get(rotation).unwrap().clone())
+            .collect();
+        let new_prim_std_positions = symmetrize_positions(
+            &prim_std_cell_tmp,
+            &prim_std_operations,
+            &prim_std_permutations,
         );
+
         // Note: prim_transformation.transform_cell does not change the order of sites
-        let prim_std_cell = prim_transformation.transform_cell(&Cell::new(
-            prim_cell.cell.lattice.clone(),
-            new_prim_positions,
-            prim_cell.cell.numbers.clone(),
-        ));
+        let prim_std_cell = Cell::new(
+            prim_std_cell_tmp.lattice.clone(),
+            new_prim_std_positions,
+            prim_std_cell_tmp.numbers.clone(),
+        );
 
         // To (conventional) standardized cell
         let conv_trans = Transformation::from_linear(entry.centering.linear());
         let (std_cell, site_mapping) = conv_trans.transform_cell(&prim_std_cell);
 
+        // Symmetrize lattice
+        let (_, rotation_matrix) =
+            symmetrize_lattice(&std_cell.lattice, &conv_std_operations.rotations);
+
+        Ok((
+            prim_std_cell.rotate(&rotation_matrix),
+            prim_std_permutations,
+            prim_transformation.clone(),
+            std_cell.rotate(&rotation_matrix),
+            // prim_transformation * (conv_trans.linear, 0)
+            Transformation::new(
+                prim_transformation.linear * conv_trans.linear,
+                prim_transformation.origin_shift,
+            ),
+            rotation_matrix,
+            site_mapping,
+        ))
+    }
+
+    fn assign_wyckoffs(
+        prim_std_cell: &Cell,
+        prim_std_permutations: &[Permutation],
+        std_cell: &Cell,
+        site_mapping: &Vec<usize>,
+        hall_number: HallNumber,
+        symprec: f64,
+    ) -> Result<Vec<WyckoffPosition>, MoyoError> {
         // Group sites in std_cell by crystallographic orbits
         let orbits = orbits_in_cell(
-            prim_cell.cell.num_atoms(),
-            &symmetry_search.permutations,
-            &site_mapping,
+            prim_std_cell.num_atoms(),
+            prim_std_permutations,
+            site_mapping,
         );
         let mut num_orbits = 0;
         let mut mapping = vec![0; std_cell.num_atoms()]; // [std_cell.num_atoms()] -> [num_orbits]
         let mut remapping = vec![]; // [num_orbits] -> [std_cell.num_atoms()]
         for i in 0..std_cell.num_atoms() {
             if orbits[i] == i {
                 mapping[i] = num_orbits;
@@ -92,58 +191,48 @@
         // multiplicities: orbit -> multiplicity
         let mut multiplicities = vec![0; num_orbits];
         for i in 0..std_cell.num_atoms() {
             multiplicities[mapping[i]] += 1;
         }
         // Assign Wyckoff positions to representative sites: orbit -> WyckoffPosition
         let mut representative_wyckoffs = vec![None; num_orbits];
-        for i in 0..std_cell.num_atoms() {
+        for (i, position) in std_cell.positions.iter().enumerate() {
             let orbit = mapping[i];
-            if !representative_wyckoffs[orbit].is_none() {
+            if representative_wyckoffs[orbit].is_some() {
                 continue;
             }
 
             if let Ok(wyckoff) = assign_wyckoff_position(
-                &std_cell.positions[i],
+                position,
                 multiplicities[orbit],
-                space_group.hall_number,
+                hall_number,
                 &std_cell.lattice,
                 symprec,
             ) {
                 representative_wyckoffs[orbit] = Some(wyckoff);
             }
         }
+
+        for (i, wyckoff) in representative_wyckoffs.iter().enumerate() {
+            if wyckoff.is_none() {
+                warn!(
+                    "Failed to assign Wyckoff positions with multiplicity {}: {:?}",
+                    multiplicities[i], std_cell.positions[i]
+                );
+            }
+        }
         let representative_wyckoffs = representative_wyckoffs
             .into_iter()
             .map(|wyckoff| wyckoff.ok_or(MoyoError::WyckoffPositionAssignmentError))
             .collect::<Result<Vec<_>, _>>()?;
 
         let wyckoffs = (0..std_cell.num_atoms())
             .map(|i| representative_wyckoffs[mapping[orbits[i]]].clone())
             .collect::<Vec<_>>();
-
-        // Symmetrize lattice
-        let std_rotations = HallSymbol::from_hall_number(entry.hall_number)
-            .traverse()
-            .rotations;
-        let (_, rotation_matrix) = symmetrize_lattice(&std_cell.lattice, &std_rotations);
-
-        Ok(StandardizedCell {
-            prim_cell: prim_std_cell.rotate(&rotation_matrix),
-            prim_transformation: prim_transformation.clone(),
-            cell: std_cell.rotate(&rotation_matrix),
-            wyckoffs,
-            // prim_transformation * (conv_trans.linear, 0)
-            transformation: Transformation::new(
-                prim_transformation.linear * conv_trans.linear,
-                prim_transformation.origin_shift,
-            ),
-            rotation_matrix,
-            site_mapping,
-        })
+        Ok(wyckoffs)
     }
 }
 
 /// * `prim_num_atoms` - Number of atoms in the primitive cell
 /// * `prim_permutations` - Permutations of the primitive cell
 /// * `site_mapping` - Mapping from the site in cell to that in its primitive cell
 pub fn orbits_in_cell(
@@ -171,43 +260,34 @@
     multiplicity: usize,
     hall_number: HallNumber,
     lattice: &Lattice,
     symprec: f64,
 ) -> Result<WyckoffPosition, MoyoError> {
     for wyckoff in iter_wyckoff_positions(hall_number, multiplicity) {
         // Find variable `y` and integers offset `offset` such that
-        //    | space.linear * y + space.origin - position - offset | < symprec.
+        //    | lattice * (space.linear * y + space.origin - position - offset) | < symprec.
         // Let SNF decomposition of space.linear be
         //    D = L * space.linear * R.
-        // argmin_{y in Q^3, n in Z^3} | space.linear * y + space.origin - position - offset |
-        //    = argmin_{y in Q^3, n in Z^3} | L^-1 * D * R^-1 * y + space.origin - position - offset |
-        //    = argmin_{y in Q^3, n in Z^3} | D * R^-1 * y - L * (offset + position - space.origin) |
+        // lattice * (space.linear * y + space.origin - position - offset)
+        //    = lattice * (L^-1 * D * R^-1 * y + space.origin - position - offset)
+        //    = lattice * L^-1 * (D * R^-1 * y + L * (space.origin - position - offset))
+
+        //    = lattice * (D * R^-1 * y - L * (offset + position - space.origin)
         let space = WyckoffPositionSpace::new(wyckoff.coordinates);
         let snf = SNF::new(&space.linear);
         for offset in iproduct!(-1..=1, -1..=1, -1..=1) {
             let offset = Vector3::new(offset.0 as f64, offset.1 as f64, offset.2 as f64);
             let b = snf.l.map(|e| e as f64) * (offset + position - space.origin);
             let mut rinvy = Vector3::zeros();
-            let mut valid = true;
             for i in 0..3 {
-                if snf.d[(i, i)] == 0 {
-                    let mut bi = Vector3::zeros();
-                    bi[i] = b[i];
-                    if lattice.cartesian_coords(&bi).norm() > symprec {
-                        valid = false;
-                        break;
-                    }
-                } else {
+                if snf.d[(i, i)] != 0 {
                     rinvy[i] = b[i] / snf.d[(i, i)] as f64;
                 }
             }
 
-            if !valid {
-                continue;
-            }
             let y = snf.r.map(|e| e as f64) * rinvy;
             let diff = space.linear.map(|e| e as f64) * y + space.origin - position - offset;
             if lattice.cartesian_coords(&diff).norm() < symprec {
                 return Ok(wyckoff.clone());
             }
         }
     }
@@ -220,25 +300,23 @@
     operations: &Operations,
     permutations: &Vec<Permutation>,
 ) -> Vec<Position> {
     let inverse_permutations = permutations
         .iter()
         .map(|permutation| permutation.inverse())
         .collect::<Vec<_>>();
+
     (0..cell.num_atoms())
         .map(|i| {
             let mut acc = Vector3::zeros();
             for (inv_perm, rotation, translation) in izip!(
                 inverse_permutations.iter(),
                 operations.rotations.iter(),
                 operations.translations.iter(),
             ) {
-                if inv_perm.apply(i) == i {
-                    continue;
-                }
                 let mut frac_displacements =
                     rotation.map(|e| e as f64) * cell.positions[inv_perm.apply(i)] + translation
                         - cell.positions[i];
                 frac_displacements -= frac_displacements.map(|e| e.round()); // in [-0.5, 0.5]
                 acc += frac_displacements;
             }
             cell.positions[i] + acc / (permutations.len() as f64)
```

### Comparing `moyopy-0.1.0/moyo/tests/test_moyo_dataset.rs` & `moyopy-0.1.2/moyo/tests/test_moyo_dataset.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 #[macro_use]
 extern crate approx;
 
 use nalgebra::{matrix, vector, Matrix3, Vector3};
+use serde_json;
+use std::fs;
+use std::path::Path;
+use test_log::test;
 
 use moyo::base::{AngleTolerance, Cell, Lattice, Permutation, Rotation, Translation};
 use moyo::data::Setting;
 use moyo::MoyoDataset;
 
 /// Sanity-check MoyoDataset
 fn assert_dataset(
@@ -207,17 +211,14 @@
         // 2c
         Vector3::new(1.0 / 3.0, 2.0 / 3.0, 1.0 / 4.0),
         Vector3::new(2.0 / 3.0, 1.0 / 3.0, 3.0 / 4.0),
     ];
     let numbers = vec![0, 0];
     let cell = Cell::new(lattice, positions, numbers);
 
-    let serialized = serde_json::to_string(&cell).unwrap();
-    println!("{:?}", serialized);
-
     let symprec = 1e-4;
     let angle_tolerance = AngleTolerance::Default;
     let setting = Setting::Standard;
 
     let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
     assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
     assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
@@ -348,7 +349,214 @@
         dataset.wyckoffs,
         vec![
             'c', 'c', 'c', 'c', 'c', 'c', 'c', 'c', 'c', 'c', 'c', 'c', 'e', 'e', 'e', 'e', 'e',
             'e', 'e', 'e', 'e', 'e', 'e', 'e', 'e', 'e', 'e', 'e', 'e', 'e',
         ]
     );
 }
+
+#[test]
+#[allow(non_snake_case)]
+fn test_with_hexagonal_Sc() {
+    // P6_122 (No. 178)
+    // https://legacy.materialsproject.org/materials/mp-601273/
+    let a = 3.234;
+    let c = 16.386;
+    let lattice = Lattice::new(matrix![
+        a, 0.0, 0.0;
+        -a / 2.0, a * 3.0_f64.sqrt() / 2.0, 0.0;
+        0.0, 0.0, c;
+    ]);
+    let x_6a = 0.4702;
+    let positions = vec![
+        // 6a
+        Vector3::new(x_6a, 0.0, 0.0),
+        Vector3::new(0.0, x_6a, 1.0 / 3.0),
+        Vector3::new(-x_6a, -x_6a, 2.0 / 3.0),
+        Vector3::new(-x_6a, 0.0, 0.5),
+        Vector3::new(0.0, -x_6a, 5.0 / 6.0),
+        Vector3::new(x_6a, x_6a, 1.0 / 6.0),
+    ];
+    let numbers = vec![0, 0, 0, 0, 0, 0];
+    let cell = Cell::new(lattice, positions, numbers);
+
+    let symprec = 1e-4;
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 178);
+    assert_eq!(dataset.hall_number, 472);
+    assert_eq!(dataset.num_operations(), 12);
+    assert_eq!(dataset.orbits, vec![0, 0, 0, 0, 0, 0]);
+    assert_eq!(dataset.wyckoffs, vec!['a', 'a', 'a', 'a', 'a', 'a']);
+}
+
+#[test]
+#[allow(non_snake_case)]
+fn test_with_trigonal_Sc() {
+    // https://next-gen.materialsproject.org/materials/mp-1055932
+    let lattice = Lattice::new(matrix![
+        -0.882444, 0.564392, -3.041088;
+        -1.66822, -2.81974, -0.089223;
+        -1.521212, 2.804144, -0.808507;
+    ]);
+    let positions = vec![Vector3::new(0.999917, 3.2999999999999996e-05, 1.7e-05)];
+    let numbers = vec![0];
+    let cell = Cell::new(lattice, positions, numbers);
+
+    let symprec = 1e-1; // This structure is distorted
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 166);
+    assert_eq!(dataset.hall_number, 458);
+    assert_eq!(dataset.num_operations(), 12); // Rhombohedral setting
+    assert_eq!(dataset.orbits, vec![0]);
+    if dataset.wyckoffs[0] != 'a' && dataset.wyckoffs[0] != 'b' {
+        panic!("Unexpected Wyckoff letter: {}", dataset.wyckoffs[0]);
+    }
+}
+
+#[test]
+#[allow(non_snake_case)]
+fn test_with_clathrate_Si() {
+    // https://next-gen.materialsproject.org/materials/mp-1201492/
+    // Pa-3
+    let path = Path::new("tests/assets/mp-1201492.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-4;
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 205);
+    assert_eq!(dataset.hall_number, 501);
+    assert_eq!(dataset.num_operations(), 24);
+}
+
+#[test]
+fn test_with_mp_1197586() {
+    // https://next-gen.materialsproject.org/materials/mp-1197586
+    let path = Path::new("tests/assets/mp-1197586.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-3; // 1e-4 gives C2/m
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 194); // P6_3/mmc
+    assert_eq!(dataset.hall_number, 488);
+    assert_eq!(dataset.num_operations(), 24);
+}
+
+#[test]
+fn test_with_mp_1185639() {
+    // https://next-gen.materialsproject.org/materials/mp-1185639
+    let path = Path::new("tests/assets/mp-1185639.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-2;
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 187); // P-6m2
+    assert_eq!(dataset.hall_number, 481);
+    assert_eq!(dataset.num_operations(), 12);
+}
+
+#[test]
+fn test_with_mp_1221598() {
+    // https://next-gen.materialsproject.org/materials/mp-1221598
+    let path = Path::new("tests/assets/mp-1221598.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-1;
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 225); // Fm-3m
+}
+
+#[test]
+fn test_with_mp_569901() {
+    let path = Path::new("tests/assets/mp-569901.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-1;
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+
+    assert_eq!(dataset.number, 118); // P-4n2
+}
+
+#[test]
+fn test_with_mp_30665() {
+    let path = Path::new("tests/assets/mp-30665.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-1;
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+}
+
+#[test]
+fn test_monotonic_symmetry_recovery() {
+    let path = Path::new("tests/assets/mp-1277787.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let angle_tolerance = AngleTolerance::Default;
+    let setting = Setting::Standard;
+
+    let symprec = 5e-2;
+    let dataset1 = MoyoDataset::new(&cell, symprec, angle_tolerance, setting).unwrap();
+
+    let symprec = 1e-1;
+    let dataset2 = MoyoDataset::new(&cell, symprec, angle_tolerance, setting).unwrap();
+
+    assert!(dataset1.number <= dataset2.number);
+}
+
+#[test]
+fn test_with_mp_550745() {
+    let path = Path::new("tests/assets/mp-550745.json");
+    let cell: Cell = serde_json::from_str(&fs::read_to_string(&path).unwrap()).unwrap();
+
+    let symprec = 1e-2;
+    let angle_tolerance = AngleTolerance::Radian(0.1);
+    let setting = Setting::Standard;
+
+    let dataset = assert_dataset(&cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.std_cell, symprec, angle_tolerance, setting);
+    assert_dataset(&dataset.prim_std_cell, symprec, angle_tolerance, setting);
+}
```

### Comparing `moyopy-0.1.0/moyopy/Cargo.toml` & `moyopy-0.1.2/moyopy/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 authors.workspace = true
 description.workspace = true
 edition.workspace = true
 license.workspace = true
 repository.workspace = true
 version.workspace = true
 
+[package.metadata.release]
+release = false
+
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "moyopy"
 crate-type = ["cdylib"]
 
 [dependencies]
 moyo = { path = "../moyo" }
 nalgebra.workspace = true
+serde.workspace = true
+serde_json.workspace = true
+approx.workspace = true
 
 [dependencies.pyo3]
 version = "0.20.0"
 # "abi3-py38" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.8
 features = ["abi3-py38"]
```

### Comparing `moyopy-0.1.0/moyopy/python/moyopy/_moyopy.pyi` & `moyopy-0.1.2/moyopy/python/moyopy/_moyopy.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     ): ...
     @property
     def basis(self) -> list[list[float]]: ...
     @property
     def positions(self) -> list[list[float]]: ...
     @property
     def numbers(self) -> list[int]: ...
+    def serialize_json(self) -> str: ...
+    @classmethod
+    def deserialize_json(cls, json_str: str) -> Cell: ...
 
 class Operations:
     @property
     def rotations(self) -> list[list[list[float]]]: ...
     @property
     def translations(self) -> list[list[float]]: ...
 
@@ -72,7 +75,11 @@
     def prim_std_cell(self) -> Cell: ...
     @property
     def prim_std_linear(self) -> list[list[float]]: ...
     @property
     def prim_std_origin_shift(self) -> list[float]: ...
     @property
     def mapping_std_prim(self) -> list[int]: ...
+    @property
+    def symprec(self) -> float: ...
+    @property
+    def angle_tolerance(self) -> float | None: ...
```

### Comparing `moyopy-0.1.0/moyopy/python/tests/conftest.py` & `moyopy-0.1.2/moyopy/python/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `moyopy-0.1.0/moyopy/src/data.rs` & `moyopy-0.1.2/moyopy/src/data.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use pyo3::prelude::*;
 use pyo3::types::PyType;
 
 use moyo::data::Setting;
 
 #[derive(Debug, Clone)]
 #[pyclass(name = "Setting")]
-#[pyo3(module = "moyo")]
+#[pyo3(module = "moyopy")]
 pub struct PySetting(Setting);
 
 #[pymethods]
 impl PySetting {
     #[classmethod]
     pub fn spglib(_cls: &PyType) -> PyResult<Self> {
         Ok(Self(Setting::Spglib))
```

### Comparing `moyopy-0.1.0/moyopy/src/lib.rs` & `moyopy-0.1.2/moyopy/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 use moyo::MoyoDataset;
 
 use crate::base::{PyMoyoError, PyStructure};
 use crate::data::PySetting;
 
 #[derive(Debug)]
 #[pyclass(name = "MoyoDataset")]
-#[pyo3(module = "moyo")]
+#[pyo3(module = "moyopy")]
 pub struct PyMoyoDataset(MoyoDataset);
 
 #[pymethods]
 impl PyMoyoDataset {
     #[new]
     #[pyo3(signature = (cell, *, symprec=1e-4, angle_tolerance=None, setting=None))]
     pub fn new(
@@ -108,35 +108,50 @@
         self.0.prim_std_origin_shift.into()
     }
 
     #[getter]
     pub fn mapping_std_prim(&self) -> Vec<usize> {
         self.0.mapping_std_prim.clone()
     }
+
+    #[getter]
+    pub fn symprec(&self) -> f64 {
+        self.0.symprec
+    }
+
+    #[getter]
+    pub fn angle_tolerance(&self) -> Option<f64> {
+        if let AngleTolerance::Radian(angle_tolerance) = self.0.angle_tolerance {
+            return Some(angle_tolerance);
+        } else {
+            return None;
+        }
+    }
 }
 
 // https://github.com/pydantic/pydantic-core/blob/main/src/lib.rs
-pub fn moyo_version() -> &'static str {
-    static MOYO_VERSION: OnceLock<String> = OnceLock::new();
+pub fn moyopy_version() -> &'static str {
+    static MOYOPY_VERSION: OnceLock<String> = OnceLock::new();
 
-    MOYO_VERSION.get_or_init(|| {
+    MOYOPY_VERSION.get_or_init(|| {
         let version = env!("CARGO_PKG_VERSION");
         // cargo uses "1.0-alpha1" etc. while python uses "1.0.0a1", this is not full compatibility,
         // but it's good enough for now
         // see https://docs.rs/semver/1.0.9/semver/struct.Version.html#method.parse for rust spec
         // see https://peps.python.org/pep-0440/ for python spec
         // it seems the dot after "alpha/beta" e.g. "-alpha.1" is not necessary, hence why this works
         version.replace("-alpha", "a").replace("-beta", "b")
     })
 }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn _moyo(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add("__version__", moyo_version())?;
+#[pyo3(name = "_moyopy")]
+fn moyopy(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add("__version__", moyopy_version())?;
 
     // lib
     m.add_class::<PyMoyoDataset>()?;
 
     // base
     m.add_class::<base::PyStructure>()?;
     m.add_class::<base::PyMoyoError>()?;
```

### Comparing `moyopy-0.1.0/Cargo.lock` & `moyopy-0.1.2/Cargo.lock`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,324 @@
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
+name = "anes"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
+
+[[package]]
+name = "anstream"
+version = "0.6.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
+dependencies = [
+ "anstyle",
+ "anstyle-parse",
+ "anstyle-query",
+ "anstyle-wincon",
+ "colorchoice",
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
+
+[[package]]
+name = "anstyle-parse"
+version = "0.2.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
+dependencies = [
+ "utf8parse",
+]
+
+[[package]]
+name = "anstyle-query"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e28923312444cdd728e4738b3f9c9cac739500909bb3d3c94b43551b16517648"
+dependencies = [
+ "windows-sys",
+]
+
+[[package]]
+name = "anstyle-wincon"
+version = "3.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1cd54b81ec8d6180e24654d0b371ad22fc3dd083b6ff8ba325b72e00c87660a7"
+dependencies = [
+ "anstyle",
+ "windows-sys",
+]
+
+[[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "atty"
+version = "0.2.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
+dependencies = [
+ "hermit-abi",
+ "libc",
+ "winapi",
+]
+
+[[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+
+[[package]]
+name = "az"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bumpalo"
+version = "3.15.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+
+[[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
+
+[[package]]
+name = "cast"
+version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
+
+[[package]]
+name = "cc"
+version = "1.0.90"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "ciborium"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42e69ffd6f0917f5c029256a24d0161db17cea3997d185db0d35926308770f0e"
+dependencies = [
+ "ciborium-io",
+ "ciborium-ll",
+ "serde",
+]
+
+[[package]]
+name = "ciborium-io"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05afea1e0a06c9be33d539b876f1ce3692f4afea2cb41f740e7743225ed1c757"
+
+[[package]]
+name = "ciborium-ll"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "57663b653d948a338bfb3eeba9bb2fd5fcfaecb9e199e87e1eda4d9e8b240fd9"
+dependencies = [
+ "ciborium-io",
+ "half",
+]
+
+[[package]]
+name = "clap"
+version = "3.2.25"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
+dependencies = [
+ "bitflags",
+ "clap_lex",
+ "indexmap",
+ "textwrap",
+]
+
+[[package]]
+name = "clap_lex"
+version = "0.2.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+dependencies = [
+ "os_str_bytes",
+]
+
+[[package]]
+name = "colorchoice"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
+
+[[package]]
+name = "criterion"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+dependencies = [
+ "anes",
+ "atty",
+ "cast",
+ "ciborium",
+ "clap",
+ "criterion-plot",
+ "itertools 0.10.5",
+ "lazy_static",
+ "num-traits",
+ "oorandom",
+ "plotters",
+ "rayon",
+ "regex",
+ "serde",
+ "serde_derive",
+ "serde_json",
+ "tinytemplate",
+ "walkdir",
+]
+
+[[package]]
+name = "criterion-plot"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
+dependencies = [
+ "cast",
+ "itertools 0.10.5",
+]
+
+[[package]]
+name = "crossbeam-deque"
+version = "0.8.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
+dependencies = [
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
+dependencies = [
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
+name = "crunchy"
+version = "0.2.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
+
+[[package]]
+name = "divrem"
+version = "1.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "69dde51e8fef5e12c1d65e0929b03d66e4c0c18282bc30ed2ca050ad6f44dd82"
+
+[[package]]
+name = "doc-comment"
+version = "0.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fea41bba32d969b513997752735605054bc0dfa92b4c56bf1189f2e174be7a10"
+
+[[package]]
 name = "either"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
+name = "elapsed"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f4e5af126dafd0741c2ad62d47f68b28602550102e5f0dd45c8a97fc8b49c29"
+
+[[package]]
+name = "env_filter"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a009aa4810eb158359dda09d0c87378e4bbb89b5a801f016885a4707ba24f7ea"
+dependencies = [
+ "log",
+ "regex",
+]
+
+[[package]]
+name = "env_logger"
+version = "0.11.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38b35839ba51819680ba087cd351788c9a3c476841207e0b8cee0b04722343b9"
+dependencies = [
+ "anstream",
+ "anstyle",
+ "env_filter",
+ "humantime",
+ "log",
+]
+
+[[package]]
+name = "fixed"
+version = "1.27.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2fc715d38bea7b5bf487fcd79bcf8c209f0b58014f3018a7a19c2b855f472048"
+dependencies = [
+ "az",
+ "bytemuck",
+ "half",
+ "num-traits",
+ "typenum",
+]
+
+[[package]]
 name = "futures"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -102,15 +366,15 @@
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -142,56 +406,172 @@
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
+name = "generator"
+version = "0.7.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5cc16584ff22b460a382b7feec54b23d2908d858152e5739a120b949293bd74e"
+dependencies = [
+ "cc",
+ "libc",
+ "log",
+ "rustversion",
+ "windows",
+]
+
+[[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "a06fddc2749e0528d2813f95e050e87e52c8cbbae56223b9babf73b3e53b0cc6"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
+name = "half"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
+dependencies = [
+ "cfg-if",
+ "crunchy",
+]
+
+[[package]]
+name = "hashbrown"
+version = "0.12.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+
+[[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "hermit-abi"
+version = "0.1.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
+dependencies = [
+ "libc",
+]
+
+[[package]]
+name = "humantime"
+version = "2.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
+
+[[package]]
+name = "indexmap"
+version = "1.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+dependencies = [
+ "autocfg",
+ "hashbrown",
+]
+
+[[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
+
+[[package]]
+name = "init_with"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "0175f63815ce00183bf755155ad0cb48c65226c5d17a724e369c25418d2b7699"
+
+[[package]]
+name = "itertools"
+version = "0.10.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
 
 [[package]]
 name = "itertools"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
+name = "itertools"
+version = "0.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
+dependencies = [
+ "either",
+]
+
+[[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
+
+[[package]]
+name = "js-sys"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
+dependencies = [
+ "wasm-bindgen",
+]
+
+[[package]]
+name = "kiddo"
+version = "4.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d2f8d9e1bc7c6919ad2cdc83472a9a4b5ed2ea2c5392c9514fdf958a7920f9a"
+dependencies = [
+ "az",
+ "divrem",
+ "doc-comment",
+ "elapsed",
+ "fixed",
+ "generator",
+ "init_with",
+ "itertools 0.12.1",
+ "log",
+ "num-traits",
+ "ordered-float",
+ "sorted-vec",
+ "tracing",
+ "tracing-subscriber",
+ "ubyte",
+]
+
+[[package]]
+name = "lazy_static"
+version = "1.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
@@ -202,69 +582,83 @@
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
+name = "log"
+version = "0.4.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
+
+[[package]]
 name = "matrixmultiply"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7574c1cf36da4798ab73da5b215bbf444f50718207754cb522201d78d1cd0ff2"
 dependencies = [
  "autocfg",
  "rawpointer",
 ]
 
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
 name = "moyo"
-version = "0.1.0"
+version = "0.1.2"
 dependencies = [
  "approx",
- "itertools",
+ "criterion",
+ "env_logger",
+ "itertools 0.11.0",
+ "kiddo",
+ "log",
  "nalgebra",
  "rand",
  "rstest",
  "serde",
  "serde_json",
  "strum",
  "strum_macros",
+ "test-log",
  "thiserror",
  "union-find",
 ]
 
 [[package]]
 name = "moyopy"
-version = "0.1.0"
+version = "0.1.2"
 dependencies = [
+ "approx",
  "moyo",
  "nalgebra",
  "pyo3",
+ "serde",
+ "serde_json",
 ]
 
 [[package]]
 name = "nalgebra"
-version = "0.32.4"
+version = "0.32.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4541eb06dce09c0241ebbaab7102f0a01a0c8994afed2e5d0d66775016e25ac2"
+checksum = "3ea4908d4f23254adda3daa60ffef0f1ac7b8c3e9a864cf3cc154b251908a2ef"
 dependencies = [
  "approx",
  "matrixmultiply",
  "nalgebra-macros",
  "num-complex",
  "num-rational",
  "num-traits",
@@ -281,14 +675,24 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "nu-ansi-term"
+version = "0.46.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
+dependencies = [
+ "overload",
+ "winapi",
+]
+
+[[package]]
 name = "num-complex"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "num-traits",
  "serde",
@@ -326,14 +730,41 @@
 [[package]]
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
+name = "oorandom"
+version = "11.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
+
+[[package]]
+name = "ordered-float"
+version = "4.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a76df7075c7d4d01fdcb46c912dd17fba5b60c78ea480b475f2b6ab6f666584e"
+dependencies = [
+ "num-traits",
+]
+
+[[package]]
+name = "os_str_bytes"
+version = "6.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e2355d85b9a3786f481747ced0e0ff2ba35213a1f9bd406ed906554d7af805a1"
+
+[[package]]
+name = "overload"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
@@ -345,52 +776,80 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
+name = "plotters"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
+dependencies = [
+ "num-traits",
+ "plotters-backend",
+ "plotters-svg",
+ "wasm-bindgen",
+ "web-sys",
+]
+
+[[package]]
+name = "plotters-backend"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
+
+[[package]]
+name = "plotters-svg"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
+dependencies = [
+ "plotters-backend",
+]
+
+[[package]]
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -434,28 +893,28 @@
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
@@ -496,27 +955,47 @@
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
+name = "rayon"
+version = "1.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.12.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
+dependencies = [
+ "crossbeam-deque",
+ "crossbeam-utils",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
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
 
@@ -529,17 +1008,17 @@
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
 name = "relative-path"
 version = "1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e898588f33fdd5b9420719948f9f2a32c922a246964576f71ba7f24f80610fbc"
 
@@ -564,15 +1043,15 @@
  "cfg-if",
  "glob",
  "proc-macro2",
  "quote",
  "regex",
  "relative-path",
  "rustc_version",
- "syn 2.0.52",
+ "syn 2.0.58",
  "unicode-ident",
 ]
 
 [[package]]
 name = "rustc_version"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -599,14 +1078,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
+name = "same-file"
+version = "1.0.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
+dependencies = [
+ "winapi-util",
+]
+
+[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "semver"
@@ -627,29 +1115,38 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "sharded-slab"
+version = "0.1.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
+dependencies = [
+ "lazy_static",
+]
+
+[[package]]
 name = "simba"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "061507c94fc6ab4ba1c9a0305018408e312e17c041eb63bef8aa726fa33aceae"
 dependencies = [
  "approx",
  "num-complex",
@@ -665,17 +1162,23 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
+
+[[package]]
+name = "sorted-vec"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "c6734caf0b6f51addd5eeacca12fb39b2c6c14e8d4f3ac42f3a78955c0467458"
 
 [[package]]
 name = "strum"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
 
@@ -685,15 +1188,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.52",
+ "syn 2.0.58",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -701,56 +1204,166 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
+name = "test-log"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b319995299c65d522680decf80f2c108d85b861d81dfe340a10d16cee29d9e6"
+dependencies = [
+ "env_logger",
+ "test-log-macros",
+]
+
+[[package]]
+name = "test-log-macros"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c8f546451eaa38373f549093fe9fd05e7d2bade739e2ddf834b9968621d60107"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "textwrap"
+version = "0.16.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
+
+[[package]]
 name = "thiserror"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e45bcbe8ed29775f228095caf2cd67af7a4ccf756ebff23a306bf3e8b47b24b"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a953cb265bef375dae3de6663da4d3804eee9682ea80d8e2542529b73c531c81"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.52",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "thread_local"
+version = "1.1.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+]
+
+[[package]]
+name = "tinytemplate"
+version = "1.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
+dependencies = [
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "tracing"
+version = "0.1.40"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
+dependencies = [
+ "pin-project-lite",
+ "tracing-attributes",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-attributes"
+version = "0.1.27"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+]
+
+[[package]]
+name = "tracing-core"
+version = "0.1.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
+dependencies = [
+ "once_cell",
+ "valuable",
+]
+
+[[package]]
+name = "tracing-log"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
+dependencies = [
+ "log",
+ "once_cell",
+ "tracing-core",
+]
+
+[[package]]
+name = "tracing-subscriber"
+version = "0.3.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
+dependencies = [
+ "nu-ansi-term",
+ "sharded-slab",
+ "smallvec",
+ "thread_local",
+ "tracing-core",
+ "tracing-log",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
 
 [[package]]
+name = "ubyte"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f720def6ce1ee2fc44d40ac9ed6d3a59c361c80a75a7aa8e75bb9baed31cf2ea"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
@@ -761,78 +1374,270 @@
 [[package]]
 name = "union-find"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c109a31f4b2557d711f79c65b0e097359c033c78ba6416b78593e78f3dba930f"
 
 [[package]]
+name = "utf8parse"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
+
+[[package]]
+name = "valuable"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
+
+[[package]]
+name = "walkdir"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
+dependencies = [
+ "same-file",
+ "winapi-util",
+]
+
+[[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
+name = "wasm-bindgen"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
+dependencies = [
+ "cfg-if",
+ "wasm-bindgen-macro",
+]
+
+[[package]]
+name = "wasm-bindgen-backend"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
+dependencies = [
+ "bumpalo",
+ "log",
+ "once_cell",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-macro"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
+dependencies = [
+ "quote",
+ "wasm-bindgen-macro-support",
+]
+
+[[package]]
+name = "wasm-bindgen-macro-support"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.58",
+ "wasm-bindgen-backend",
+ "wasm-bindgen-shared",
+]
+
+[[package]]
+name = "wasm-bindgen-shared"
+version = "0.2.92"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
+
+[[package]]
+name = "web-sys"
+version = "0.3.69"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
+dependencies = [
+ "js-sys",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "wide"
 version = "0.7.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
+name = "winapi"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
+dependencies = [
+ "winapi-i686-pc-windows-gnu",
+ "winapi-x86_64-pc-windows-gnu",
+]
+
+[[package]]
+name = "winapi-i686-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
+
+[[package]]
+name = "winapi-util"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
+dependencies = [
+ "winapi",
+]
+
+[[package]]
+name = "winapi-x86_64-pc-windows-gnu"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
+
+[[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.4",
+]
+
+[[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
+
+[[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
```

### Comparing `moyopy-0.1.0/pyproject.toml` & `moyopy-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -16,26 +16,32 @@
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
+    "pre-commit",
 ]
 
 [tool.maturin]
 python-source = "python"
-module-name = "moyopy._moyo"
+module-name = "moyopy._moyopy"
 # "extension-module" tells pyo3 we want to build an extension module (skips linking against libpython.so)
 features = ["pyo3/extension-module"]
 manifest-path = "moyopy/Cargo.toml"
 
 [tool.ruff]
 line-length = 99
 extend-select = [
```

### Comparing `moyopy-0.1.0/python/moyopy/_moyopy.pyi` & `moyopy-0.1.2/python/moyopy/_moyopy.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     ): ...
     @property
     def basis(self) -> list[list[float]]: ...
     @property
     def positions(self) -> list[list[float]]: ...
     @property
     def numbers(self) -> list[int]: ...
+    def serialize_json(self) -> str: ...
+    @classmethod
+    def deserialize_json(cls, json_str: str) -> Cell: ...
 
 class Operations:
     @property
     def rotations(self) -> list[list[list[float]]]: ...
     @property
     def translations(self) -> list[list[float]]: ...
 
@@ -72,7 +75,11 @@
     def prim_std_cell(self) -> Cell: ...
     @property
     def prim_std_linear(self) -> list[list[float]]: ...
     @property
     def prim_std_origin_shift(self) -> list[float]: ...
     @property
     def mapping_std_prim(self) -> list[int]: ...
+    @property
+    def symprec(self) -> float: ...
+    @property
+    def angle_tolerance(self) -> float | None: ...
```

