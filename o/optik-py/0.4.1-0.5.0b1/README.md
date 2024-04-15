# Comparing `tmp/optik_py-0.4.1.tar.gz` & `tmp/optik_py-0.5.0b1.tar.gz`

## Comparing `optik_py-0.4.1.tar` & `optik_py-0.5.0b1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0     1001      127      687 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/Cargo.toml
--rw-r--r--   0     1001      127     2027 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/benches/bench.rs
--rw-r--r--   0     1001      127     1250 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/src/config.rs
--rw-r--r--   0     1001      127    10434 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/src/kinematics.rs
--rw-r--r--   0     1001      127    10063 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/src/lib.rs
--rw-r--r--   0     1001      127     6871 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/src/math.rs
--rw-r--r--   0     1001      127     1972 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/src/objective.rs
--rw-r--r--   0     1001      127     6888 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_fk_inputs.json
--rw-r--r--   0     1001      127    11169 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_fk_outputs.json
--rw-r--r--   0     1001      127     2281 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_math_inputs.json
--rw-r--r--   0     1001      127     1162 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_se3_log.json
--rw-r--r--   0     1001      127     5836 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json
--rw-r--r--   0     1001      127      808 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_so3_log.json
--rw-r--r--   0     1001      127     1717 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json
--rwxr-xr-x   0     1001      127    12531 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/data/ur3e.urdf
--rw-r--r--   0     1001      127      670 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/test_fk.rs
--rw-r--r--   0     1001      127     1575 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/test_gradient.rs
--rw-r--r--   0     1001      127     4300 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/test_ik.rs
--rw-r--r--   0     1001      127     1897 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik/tests/test_math.rs
--rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 optik_py-0.4.1/crates/optik-py/Cargo.toml
--rw-r--r--   0     1001      127       71 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik-py/build.rs
--rw-r--r--   0     1001      127     3097 2024-02-28 17:12:24.000000 optik_py-0.4.1/crates/optik-py/src/lib.rs
--rw-r--r--   0     1001      127    31446 2024-02-28 17:12:24.000000 optik_py-0.4.1/Cargo.lock
--rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 optik_py-0.4.1/Cargo.toml
--rw-r--r--   0     1001      127      533 2024-02-28 17:12:24.000000 optik_py-0.4.1/pyproject.toml
--rw-r--r--   0     1001      127     5866 2024-02-28 17:12:24.000000 optik_py-0.4.1/README.md
--rw-r--r--   0        0        0     6324 1970-01-01 00:00:00.000000 optik_py-0.4.1/PKG-INFO
+-rw-r--r--   0     1001      127      688 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/Cargo.toml
+-rw-r--r--   0     1001      127     2047 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/benches/bench.rs
+-rw-r--r--   0     1001      127     1507 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/config.rs
+-rw-r--r--   0     1001      127    10434 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/kinematics.rs
+-rw-r--r--   0     1001      127    10583 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/lib.rs
+-rw-r--r--   0     1001      127     6871 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/math.rs
+-rw-r--r--   0     1001      127     2792 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/src/objective.rs
+-rw-r--r--   0     1001      127     6888 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_fk_inputs.json
+-rw-r--r--   0     1001      127    11169 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_fk_outputs.json
+-rw-r--r--   0     1001      127     2281 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_inputs.json
+-rw-r--r--   0     1001      127     1162 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_log.json
+-rw-r--r--   0     1001      127     5836 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json
+-rw-r--r--   0     1001      127      808 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_log.json
+-rw-r--r--   0     1001      127     1717 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json
+-rwxr-xr-x   0     1001      127    12531 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/data/ur3e.urdf
+-rw-r--r--   0     1001      127      670 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_fk.rs
+-rw-r--r--   0     1001      127     1761 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_gradient.rs
+-rw-r--r--   0     1001      127     4300 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_ik.rs
+-rw-r--r--   0     1001      127     1897 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik/tests/test_math.rs
+-rw-r--r--   0        0        0      391 1970-01-01 00:00:00.000000 optik_py-0.5.0b1/crates/optik-py/Cargo.toml
+-rw-r--r--   0     1001      127       71 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik-py/build.rs
+-rw-r--r--   0     1001      127     3408 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/crates/optik-py/src/lib.rs
+-rw-r--r--   0     1001      127    31698 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/Cargo.lock
+-rw-r--r--   0        0        0      281 1970-01-01 00:00:00.000000 optik_py-0.5.0b1/Cargo.toml
+-rw-r--r--   0     1001      127      533 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/pyproject.toml
+-rw-r--r--   0     1001      127     5866 2024-04-15 21:08:32.000000 optik_py-0.5.0b1/README.md
+-rw-r--r--   0        0        0     6326 1970-01-01 00:00:00.000000 optik_py-0.5.0b1/PKG-INFO
```

### Comparing `optik_py-0.4.1/crates/optik/Cargo.toml` & `optik_py-0.5.0b1/crates/optik/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [dependencies]
 nalgebra = "0.32"
 nlopt = { git = "https://github.com/kylc/rust-nlopt.git", branch = "optik-patches" }
 ordered-float = "4.2"
 petgraph = "0.6"
 rand = "0.8"
 rand_chacha = "0.3"
-rayon = "1.8"
+rayon = "1.10"
 urdf-rs = "0.8"
 
 [[example]]
 name = "example"
 path = "../../examples/example.rs"
 
 [dev-dependencies]
```

### Comparing `optik_py-0.4.1/crates/optik/benches/bench.rs` & `optik_py-0.5.0b1/crates/optik/benches/bench.rs`

 * *Files 2% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
     let q = robot.random_configuration(&mut rand::thread_rng());
     let mut g = vec![0.0; q.len()];
     let tfm_target = Isometry3::identity();
 
     c.bench_function("gradient", |b| {
         let fk = robot.fk(&q);
-        b.iter(|| objective_grad(&robot, &tfm_target, &fk, &mut g))
+        b.iter(|| objective_grad(&robot, &tfm_target, &fk, &mut g, 0.0, 0.0))
     });
 }
 
 fn bench_objective(c: &mut Criterion) {
     use optik::objective::objective;
 
     let robot = load_benchmark_model();
 
     let q = robot.random_configuration(&mut rand::thread_rng());
     let fk = robot.fk(&q);
     let tfm_target = Isometry3::identity();
     c.bench_function("objective", |b| {
-        b.iter(|| objective(&robot, &tfm_target, &fk))
+        b.iter(|| objective(&robot, &tfm_target, &fk, 0.0, 0.0))
     });
 }
 
 fn bench_fk(c: &mut Criterion) {
     let robot = load_benchmark_model();
     let x0 = vec![0.1, 0.2, 0.0, 0.3, -0.2, -1.1];
```

### Comparing `optik_py-0.4.1/crates/optik/src/config.rs` & `optik_py-0.5.0b1/crates/optik/src/config.rs`

 * *Files 12% similar despite different names*

```diff
@@ -37,21 +37,29 @@
     pub tol_f: f64,
 
     /// Stopping criteria: |f(x_{n+1}) - f(x)| < tol_df
     pub tol_df: f64,
 
     /// Stopping criteria: ||x_{n+1} - x_n|| < tol_dx
     pub tol_dx: f64,
+
+    /// Linear cost term goes to zero once ||e_linear|| <= tol_linear
+    pub tol_linear: f64,
+
+    /// Angular cost term goes to zero once ||e_angular|| <= tol_angular
+    pub tol_angular: f64,
 }
 
 impl Default for SolverConfig {
     fn default() -> Self {
         SolverConfig {
             solution_mode: SolutionMode::Speed,
             max_time: 0.1,
             max_restarts: u64::MAX,
             tol_f: 1e-6,
             tol_df: -1.0,
             tol_dx: -1.0,
+            tol_linear: -1.0,
+            tol_angular: -1.0,
         }
     }
 }
```

### Comparing `optik_py-0.4.1/crates/optik/src/kinematics.rs` & `optik_py-0.5.0b1/crates/optik/src/kinematics.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/src/lib.rs` & `optik_py-0.5.0b1/crates/optik/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -164,19 +164,32 @@
                             // Share kinematic results between the gradient and
                             // objective function evaluations, when possible.
                             self.chain.forward_kinematics_mut(x, fk);
 
                             // Compute the gradient only if it was requested by
                             // the optimizer.
                             if let Some(g) = grad {
-                                objective_grad(self, tfm_target, fk, g);
+                                objective_grad(
+                                    self,
+                                    tfm_target,
+                                    fk,
+                                    g,
+                                    config.tol_linear,
+                                    config.tol_angular,
+                                );
                             }
 
                             // Always compute the objective value.
-                            Some(objective(self, tfm_target, fk))
+                            Some(objective(
+                                self,
+                                tfm_target,
+                                fk,
+                                config.tol_linear,
+                                config.tol_angular,
+                            ))
                         },
                         Target::Minimize,
                         // Cache the forward kinematic container within each
                         // thread to avoid re-allocating memory each objective
                         // iteration.
                         ForwardKinematics::default(),
                     );
```

### Comparing `optik_py-0.4.1/crates/optik/src/math.rs` & `optik_py-0.5.0b1/crates/optik/src/math.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_fk_inputs.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_fk_inputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_fk_outputs.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_fk_outputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_math_inputs.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_math_inputs.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_se3_log.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_log.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_se3_right_jacobian.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_so3_log.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_log.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json` & `optik_py-0.5.0b1/crates/optik/tests/data/test_math_outputs_so3_right_jacobian.json`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/data/ur3e.urdf` & `optik_py-0.5.0b1/crates/optik/tests/data/ur3e.urdf`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/test_fk.rs` & `optik_py-0.5.0b1/crates/optik/tests/test_fk.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/test_gradient.rs` & `optik_py-0.5.0b1/crates/optik/tests/test_gradient.rs`

 * *Files 18% similar despite different names*

```diff
@@ -30,30 +30,39 @@
 
     DVector::from_row_slice(&g)
 }
 
 #[test]
 fn test_gradient_analytical_vs_numerical() {
     let robot = Robot::from_urdf_str(TEST_MODEL_STR, "ur_base_link", "ur_ee_link");
+    let tol_linear = 0.0;
+    let tol_angular = 0.0;
 
     let mut rng = StdRng::seed_from_u64(42);
     for _ in 0..100 {
         let x0: Vector6<f64> = rng.gen();
         let tfm_target = rng.gen();
         let fk = robot.fk(x0.as_slice());
 
         // Analytical gradient
         let mut g_a = Vector6::zeros();
-        objective_grad(&robot, &tfm_target, &fk, g_a.as_mut_slice());
+        objective_grad(
+            &robot,
+            &tfm_target,
+            &fk,
+            g_a.as_mut_slice(),
+            tol_linear,
+            tol_angular,
+        );
 
         // Numerical gradient
         let g_n = finite_difference(
             |x| {
                 let fk = robot.fk(x);
-                objective(&robot, &tfm_target, &fk)
+                objective(&robot, &tfm_target, &fk, tol_linear, tol_angular)
             },
             x0.as_slice(),
         );
 
         assert_abs_diff_eq!(g_a.as_slice(), g_n.as_slice(), epsilon = 1e-6);
     }
 }
```

### Comparing `optik_py-0.4.1/crates/optik/tests/test_ik.rs` & `optik_py-0.5.0b1/crates/optik/tests/test_ik.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik/tests/test_math.rs` & `optik_py-0.5.0b1/crates/optik/tests/test_math.rs`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/crates/optik-py/src/lib.rs` & `optik_py-0.5.0b1/crates/optik-py/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#![allow(non_local_definitions)] // silence warning from pyo3::pymethods macro
+
 use optik::{Robot, SolverConfig};
 
 use nalgebra::{Isometry3, Matrix4};
 use pyo3::prelude::*;
 
 #[pyclass]
 #[pyo3(name = "SolverConfig")]
@@ -11,36 +13,43 @@
 impl PySolverConfig {
     #[new]
     #[pyo3(signature=(solution_mode="speed",
                       max_time=0.1,
                       max_restarts=u64::MAX,
                       tol_f=1e-6,
                       tol_df=-1.0,
-                      tol_dx=-1.0))]
+                      tol_dx=-1.0,
+                      tol_linear=-1.0,
+                      tol_angular=-1.0))]
+    #[allow(clippy::too_many_arguments)]
     fn py_new(
         solution_mode: &str,
         max_time: f64,
         max_restarts: u64,
         tol_f: f64,
         tol_df: f64,
         tol_dx: f64,
+        tol_linear: f64,
+        tol_angular: f64,
     ) -> Self {
         let solution_mode = solution_mode.parse().expect("invalid solution mode");
 
         if max_time == 0.0 && max_restarts == 0 {
             panic!("no time or restart limit applied -- solver would run forever")
         }
 
         PySolverConfig(SolverConfig {
             solution_mode,
             max_time,
             max_restarts,
             tol_f,
             tol_df,
             tol_dx,
+            tol_linear,
+            tol_angular,
         })
     }
 }
 
 #[pyclass]
 #[pyo3(name = "Robot")]
 pub struct PyRobot(Robot);
@@ -112,12 +121,12 @@
         let target = parse_pose(target);
         robot.ik(&config.0, &target, x0)
     }
 }
 
 #[pymodule()]
 #[pyo3(name = "optik")]
-fn optik_extension(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+fn optik_extension(_py: Python<'_>, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PyRobot>()?;
     m.add_class::<PySolverConfig>()?;
     Ok(())
 }
```

### Comparing `optik_py-0.4.1/Cargo.lock` & `optik_py-0.5.0b1/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
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
 name = "anes"
 version = "0.1.6"
@@ -30,47 +30,47 @@
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
 
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
 
 [[package]]
 name = "bumpalo"
-version = "3.15.3"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea184aa71bb362a1157c896979544cc23974e08fd265f29ea96b59f0b4a555b"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.3"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2ef034f05691a48569bd920a96c81b9d91bbad1ab5ac7c4616c1f6ef36cb79f"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.88"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02f341c093d19155a6e41631ce5971aac4e9a868262212153124c15fa22d1cdc"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -99,26 +99,26 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.5.1"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c918d541ef2913577a0f9566e9ce27cb35b6df072075769e0b26cb5a554520da"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.5.1"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f3e7391dad68afb0c2ede1bf619f579a3dc9c2ec67f089baa397123a2f3d1eb"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -200,17 +200,17 @@
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
 
@@ -218,28 +218,28 @@
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
 ]
 
 [[package]]
 name = "hashbrown"
@@ -251,33 +251,33 @@
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.8"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "379dada1584ad501b383485dd706b8afb7a70fcbc7f4da7d780638a5a6124a60"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "indexmap"
-version = "2.2.3"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "233cf39063f058ea2caae4091bf4a3ef70a653afbc026f5c4a4135d114e3c177"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "is-terminal"
 version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
@@ -293,23 +293,23 @@
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "js-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "406cda4b368d531c842222cf9d2600a9a4acce8d29423695379c6868a143a9ee"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.153"
@@ -330,48 +330,48 @@
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
@@ -451,15 +451,15 @@
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
 name = "optik"
-version = "0.4.1"
+version = "0.5.0-beta.1"
 dependencies = [
  "approx",
  "criterion",
  "nalgebra",
  "nlopt",
  "ordered-float",
  "petgraph",
@@ -469,24 +469,24 @@
  "serde",
  "serde_json",
  "urdf-rs",
 ]
 
 [[package]]
 name = "optik-cpp"
-version = "0.4.1"
+version = "0.5.0-beta.1"
 dependencies = [
  "nalgebra",
  "optik",
  "rand",
 ]
 
 [[package]]
 name = "optik-py"
-version = "0.4.1"
+version = "0.5.0-beta.1"
 dependencies = [
  "nalgebra",
  "optik",
  "pyo3",
  "pyo3-build-config",
 ]
 
@@ -576,26 +576,26 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
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
@@ -603,62 +603,62 @@
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
- "syn 2.0.51",
+ "syn 2.0.59",
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
- "syn 2.0.51",
+ "syn 2.0.59",
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
 name = "rand"
 version = "0.8.5"
@@ -703,17 +703,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4963ed1bc86e4f3ee217022bd855b297cef07fb9eac5dfa1f788b220b49b3bd"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -732,40 +732,40 @@
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
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
@@ -806,22 +806,22 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.59",
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
@@ -835,64 +835,64 @@
  "num-traits",
  "paste",
  "wide",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.51"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ab617d94515e94ae53b8406c628598680aa0c9587474ecbe58188f7b345d66c"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
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
- "syn 2.0.51",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
@@ -931,97 +931,97 @@
  "xml-rs",
  "yaserde",
  "yaserde_derive",
 ]
 
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
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1e124130aee3fb58c5bdd6b639a0509486b0338acaaae0c84a5124b0f588b7f"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c9e7e1900c352b609c8488ad12639a311045f40a35491fb69ba8c12f758af70b"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.59",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b30af9e2d358182b5c7449424f017eba305ed32a7010509ede96cdc4696c46ed"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "642f325be6301eb8107a83d12a8ac6c1e1c54345a7ef1a9261962dfefda09e66"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.51",
+ "syn 2.0.59",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.91"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f186bd2dcf04330886ce82d6f33dd75a7bfcf69ecf5763b89fcde53b6ac9838"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "web-sys"
-version = "0.3.68"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "96565907687f7aceb35bc5fc03770a8a0471d82e479f25832f54a0e3f4b28446"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wide"
-version = "0.7.15"
+version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
+checksum = "81a1851a719f11d1d2fea40e15c72f6c00de8c142d7ac47c1441cc7e4d0d5bc6"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1056,15 +1056,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.3",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1076,116 +1076,123 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d380ba1dc7187569a8a9e91ed34b8ccfc33123bbacb8c0aed2d1ad7f3ef2dc5f"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.3",
- "windows_aarch64_msvc 0.52.3",
- "windows_i686_gnu 0.52.3",
- "windows_i686_msvc 0.52.3",
- "windows_x86_64_gnu 0.52.3",
- "windows_x86_64_gnullvm 0.52.3",
- "windows_x86_64_msvc 0.52.3",
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
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "68e5dcfb9413f53afd9c8f86e56a7b4d86d9a2fa26090ea2dc9e40fba56c6ec6"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8dab469ebbc45798319e69eebf92308e541ce46760b49b18c6b3fe5e8965b30f"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.3"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a4e9b6a7cac734a8b4138a4e1044eac3404d8326b6c0f939276560687a033fb"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28b0ec9c422ca95ff34a78755cfa6ad4a51371da2a5ace67500cf7ca5f232c58"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "704131571ba93e89d7cd43482277d6632589b18ecf4468f591fbae0a8b101614"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "42079295511643151e98d61c38c0acc444e52dd42ab456f7ccfd5152e8ecf21c"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.3"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0770833d60a970638e989b3fa9fd2bb1aaadcf88963d1659fd7d9990196ed2d6"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "xml-rs"
-version = "0.8.19"
+version = "0.8.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fcb9cbac069e033553e8bb871be2fbdffcab578eb25bd0f7c508cedc6dcd75a"
+checksum = "791978798f0597cfc70478424c2b4fdc2b7a8024aaff78497ef00f24ef674193"
 
 [[package]]
 name = "yaserde"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bf52af554a50b866aaad63d7eabd6fca298db3dfe49afd50b7ba5a33dfa0582"
 dependencies = [
```

### Comparing `optik_py-0.4.1/pyproject.toml` & `optik_py-0.5.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/README.md` & `optik_py-0.5.0b1/README.md`

 * *Files identical despite different names*

### Comparing `optik_py-0.4.1/PKG-INFO` & `optik_py-0.5.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: optik-py
-Version: 0.4.1
+Version: 0.5.0b1
 Classifier: Topic :: Scientific/Engineering
 License-File: LICENSE-APACHE
 License-File: LICENSE-MIT
 Summary: An optimizing IK solver based on the Lie group of rigid transforms SE(3)
 Author: Kyle Cesare
 Author-email: kcesare@gmail.com
 License: MIT OR Apache-2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optik-py Version: 0.4.1 Classifier: Topic ::
+Metadata-Version: 2.3 Name: optik-py Version: 0.5.0b1 Classifier: Topic ::
 Scientific/Engineering License-File: LICENSE-APACHE License-File: LICENSE-MIT
 Summary: An optimizing IK solver based on the Lie group of rigid transforms SE
 (3) Author: Kyle Cesare Author-email: kcesare@gmail.com License: MIT OR Apache-
 2.0 Requires-Python: >=3.8 Description-Content-Type: text/markdown;
 charset=UTF-8; variant=GFM Project-URL: homepage, https://github.com/kylc/optik
 # OptIK
 _[_M_I_T_]_[_A_p_a_c_h_e_]_[_c_i_]_[_P_y_P_I_]_[_D_O_I_]
```

