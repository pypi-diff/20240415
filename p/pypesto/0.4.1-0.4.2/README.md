# Comparing `tmp/pypesto-0.4.1.tar.gz` & `tmp/pypesto-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypesto-0.4.1.tar", last modified: Wed Dec  6 08:42:06 2023, max compression
+gzip compressed data, was "pypesto-0.4.2.tar", last modified: Mon Apr 15 18:09:01 2024, max compression
```

## Comparing `pypesto-0.4.1.tar` & `pypesto-0.4.2.tar`

### file list

```diff
@@ -1,187 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.486087 pypesto-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-06 08:41:52.000000 pypesto-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2023-12-06 08:42:06.486087 pypesto-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2023-12-06 08:41:52.000000 pypesto-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.466087 pypesto-0.4.1/pypesto/
--rw-r--r--   0 runner    (1001) docker     (127)     9118 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/C.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.466087 pypesto-0.4.1/pypesto/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/multi_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/multi_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/single_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/engine/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.466087 pypesto-0.4.1/pypesto/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/ensemble/covariance_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/ensemble/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    43639 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/ensemble/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/ensemble/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    11582 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/ensemble/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.470087 pypesto-0.4.1/pypesto/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17294 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/inner_calculator_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.470087 pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7361 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27567 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    42771 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/petab.py
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.470087 pypesto-0.4.1/pypesto/hierarchical/spline_approximation/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/spline_approximation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/spline_approximation/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/spline_approximation/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15350 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/spline_approximation/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)    31495 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/spline_approximation/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8972 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/hierarchical/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.470087 pypesto-0.4.1/pypesto/history/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15337 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9654 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    16190 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/history/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/objective/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/objective/aesara/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/aesara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/aesara/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/aggregated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/objective/amici/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/amici/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22221 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/amici/amici.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/amici/amici_calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13240 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/amici/amici_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    22784 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    24326 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (127)     7744 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/objective/jax/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8662 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/jax/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/objective/julia/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/julia/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7288 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/julia/petabJl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/julia/petab_jl_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/pre_post_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    17150 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/objective/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/optimize/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.474087 pypesto-0.4.1/pypesto/optimize/ess/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/ess/cess.py
--rw-r--r--   0 runner    (1001) docker     (127)    22578 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/ess/ess.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/ess/function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7051 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/ess/refset.py
--rw-r--r--   0 runner    (1001) docker     (127)    33525 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/ess/sacess.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     5327 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    42461 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/optimize/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.478087 pypesto-0.4.1/pypesto/petab/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34791 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/petab/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.478087 pypesto-0.4.1/pypesto/predict/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17224 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/predict/amici_predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/predict/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.478087 pypesto-0.4.1/pypesto/problem/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18549 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/problem/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.478087 pypesto-0.4.1/pypesto/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/approximate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    15436 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/profile_next_guess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5230 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/validation_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/profile/walk_along_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.478087 pypesto-0.4.1/pypesto/result/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13812 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/result/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)    12223 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/result/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     8066 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/result/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/result/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/result/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.482087 pypesto-0.4.1/pypesto/sample/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/adaptive_metropolis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/adaptive_parallel_tempering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/dynesty.py
--rw-r--r--   0 runner    (1001) docker     (127)     7835 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/emcee.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/geweke_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/parallel_tempering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8003 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/pymc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/sample/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.482087 pypesto-0.4.1/pypesto/select/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18673 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/select/method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/select/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/select/model_problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/select/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/select/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.482087 pypesto-0.4.1/pypesto/startpoint/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/startpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/startpoint/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/startpoint/latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/startpoint/uniform.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/startpoint/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.482087 pypesto-0.4.1/pypesto/store/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/store/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/store/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    10758 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/store/read_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/store/save_to_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.482087 pypesto-0.4.1/pypesto/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/testing/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.486087 pypesto-0.4.1/pypesto/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/clust_color.py
--rw-r--r--   0 runner    (1001) docker     (127)     8800 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)    12764 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)    12196 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)    13027 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/optimization_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/optimizer_convergence.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/optimizer_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    32256 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/ordinal_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)    19308 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/profile_cis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/reference_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    46051 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/select.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/spline_approximation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2023-12-06 08:41:52.000000 pypesto-0.4.1/pypesto/visualize/waterfall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 08:42:06.466087 pypesto-0.4.1/pypesto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2023-12-06 08:42:06.000000 pypesto-0.4.1/pypesto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2023-12-06 08:42:06.000000 pypesto-0.4.1/pypesto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 08:42:06.000000 pypesto-0.4.1/pypesto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2023-12-06 08:42:06.000000 pypesto-0.4.1/pypesto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-06 08:42:06.000000 pypesto-0.4.1/pypesto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-06 08:41:52.000000 pypesto-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-12-06 08:42:06.486087 pypesto-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-06 08:41:52.000000 pypesto-0.4.1/setup.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.160216 pypesto-0.4.2/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1484 2024-04-15 18:06:52.000000 pypesto-0.4.2/LICENSE
+-rw-r--r--   0 dweindl   (1000) dweindl   (1000)    12948 2024-04-15 18:09:01.160216 pypesto-0.4.2/PKG-INFO
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3976 2024-04-15 18:06:52.000000 pypesto-0.4.2/README.md
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.145217 pypesto-0.4.2/pypesto/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9483 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/C.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      950 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/__init__.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.146216 pypesto-0.4.2/pypesto/engine/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      401 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      593 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1520 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/mpi_pool.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2400 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/multi_process.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2014 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/multi_thread.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      922 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/single_core.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      456 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/engine/task.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.146216 pypesto-0.4.2/pypesto/ensemble/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      673 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11818 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/covariance_analysis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9071 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/dimension_reduction.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    43707 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/ensemble.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      918 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/task.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11582 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/ensemble/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.146216 pypesto-0.4.2/pypesto/hierarchical/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1284 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4256 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/base_parameter.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8607 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/base_problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1317 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/base_solver.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20724 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/inner_calculator_collector.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/hierarchical/ordinal/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1466 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7146 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2716 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/parameter.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    27982 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    42258 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/ordinal/solver.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24360 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/petab.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/hierarchical/relative/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1256 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12343 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9797 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    21213 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/solver.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15533 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/relative/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      801 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6978 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1981 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/parameter.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15869 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    36195 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/hierarchical/semiquantitative/solver.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.147216 pypesto-0.4.2/pypesto/history/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      654 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7865 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/amici.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15341 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9866 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/csv.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1471 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/generate.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    16392 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/hdf5.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3872 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/memory.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9808 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/optimizer.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3497 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/options.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1762 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/history/util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1902 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/logging.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      313 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/__init__.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/aesara/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       77 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/aesara/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8974 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/aesara/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5267 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/aggregated.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/amici/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      141 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23449 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/amici.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7665 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/amici_calculator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13240 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/amici/amici_util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    22972 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    24326 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/finite_difference.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7744 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/function.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/jax/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       71 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/jax/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8662 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/jax/base.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.148216 pypesto-0.4.2/pypesto/objective/julia/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      136 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6169 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7289 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/petabJl.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9836 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/julia/petab_jl_importer.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4259 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/pre_post_process.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17150 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/objective/priors.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/optimize/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      699 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/__init__.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/optimize/ess/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      328 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    11596 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/cess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    23679 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/ess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9279 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/function_evaluator.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7051 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/refset.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    35269 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/ess/sacess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8254 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/load.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5327 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/optimize.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    43623 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/optimizer.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1963 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/options.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2000 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/task.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5523 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/optimize/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/petab/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      601 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/petab/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    37717 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/petab/importer.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/predict/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      211 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/predict/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18014 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/predict/amici_predictor.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1304 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/predict/task.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.149217 pypesto-0.4.2/pypesto/problem/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      207 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/problem/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18549 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/problem/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2709 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/problem/hierarchical.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.150216 pypesto-0.4.2/pypesto/profile/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      288 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3536 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/approximate.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4205 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/options.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5832 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/profile.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15436 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/profile_next_guess.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2440 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/task.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6840 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5230 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/validation_intervals.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5524 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/profile/walk_along_profile.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.150216 pypesto-0.4.2/pypesto/result/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      415 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13868 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/optimize.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12263 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/predict.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8066 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/profile.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1409 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/result.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3753 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/result/sample.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.150216 pypesto-0.4.2/pypesto/sample/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      644 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7431 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/adaptive_metropolis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1988 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/adaptive_parallel_tempering.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1762 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/auto_correlation.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3742 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/diagnostics.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9649 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/dynesty.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7835 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/emcee.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5653 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/geweke_test.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7031 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/metropolis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6133 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/parallel_tempering.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8004 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/pymc.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3169 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/sample.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4143 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/sampler.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3352 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/sample/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/select/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      582 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    18540 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/method.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5492 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/misc.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7769 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/model_problem.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5522 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/postprocessors.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     9881 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/select/problem.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/startpoint/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      483 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     7756 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/base.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2895 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/latin_hypercube.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1263 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/uniform.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      455 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/startpoint/util.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/store/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      486 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2553 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/auto.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2239 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/hdf5.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10876 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/read_from_hdf5.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    10049 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/store/save_to_hdf5.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.151216 pypesto-0.4.2/pypesto/testing/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       49 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/testing/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     4020 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/testing/examples.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8964 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/util.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       22 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/version.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.152216 pypesto-0.4.2/pypesto/visualize/
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1738 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/__init__.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6832 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/clust_color.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     8800 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/dimension_reduction.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12766 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/ensemble.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    12196 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/misc.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13183 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/model_fit.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    13029 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/optimization_stats.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     1813 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/optimizer_convergence.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15923 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/optimizer_history.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    32126 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/ordinal_categories.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    20133 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/parameters.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2684 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/profile_cis.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    15189 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/profiles.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5722 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/reference_points.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    46051 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/sampling.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     6219 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/select.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    17460 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/spline_approximation.py
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)    14103 2024-04-15 18:06:52.000000 pypesto-0.4.2/pypesto/visualize/waterfall.py
+drwxrwxr-x   0 dweindl   (1000) dweindl   (1000)        0 2024-04-15 18:09:01.152216 pypesto-0.4.2/pypesto.egg-info/
+-rw-r--r--   0 dweindl   (1000) dweindl   (1000)    12948 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/PKG-INFO
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     5058 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        1 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     2186 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/requires.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)        8 2024-04-15 18:09:01.000000 pypesto-0.4.2/pypesto.egg-info/top_level.txt
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)      377 2024-04-15 18:06:52.000000 pypesto-0.4.2/pyproject.toml
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)     3041 2024-04-15 18:09:01.161216 pypesto-0.4.2/setup.cfg
+-rw-rw-r--   0 dweindl   (1000) dweindl   (1000)       88 2024-04-15 18:06:52.000000 pypesto-0.4.2/setup.py
```

### Comparing `pypesto-0.4.1/LICENSE` & `pypesto-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/README.md` & `pypesto-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/C.py` & `pypesto-0.4.2/pypesto/C.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,37 +80,38 @@
 START_TIME = 'start_time'  # start time
 X = 'x'
 X0 = 'x0'
 ID = 'id'
 
 
 ###############################################################################
-# HIERARCHICAL
+# HIERARCHICAL SCALING + OFFSET
 
 INNER_PARAMETERS = 'inner_parameters'
 INNER_RDATAS = 'inner_rdatas'
 PARAMETER_TYPE = 'parameterType'
 X_INNER_OPT = 'x_inner_opt'
+RELATIVE = 'relative'
 
 
 class InnerParameterType(str, Enum):
     """Specifies different inner parameter types."""
 
     OFFSET = 'offset'
     SCALING = 'scaling'
     SIGMA = 'sigma'
-    OPTIMAL_SCALING = 'optimal_scaling'
+    ORDINAL = 'ordinal'
     SPLINE = 'spline'
 
 
 DUMMY_INNER_VALUE = {
     InnerParameterType.OFFSET: 0.0,
     InnerParameterType.SCALING: 1.0,
     InnerParameterType.SIGMA: 1.0,
-    InnerParameterType.OPTIMAL_SCALING: 0.0,
+    InnerParameterType.ORDINAL: 0.0,
     InnerParameterType.SPLINE: 0.0,
 }
 
 INNER_PARAMETER_BOUNDS = {
     InnerParameterType.OFFSET: {
         LOWER_BOUND: -float('inf'),
         UPPER_BOUND: float('inf'),
@@ -119,15 +120,15 @@
         LOWER_BOUND: -float('inf'),
         UPPER_BOUND: float('inf'),
     },
     InnerParameterType.SIGMA: {
         LOWER_BOUND: 0,
         UPPER_BOUND: float('inf'),
     },
-    InnerParameterType.OPTIMAL_SCALING: {
+    InnerParameterType.ORDINAL: {
         LOWER_BOUND: -float('inf'),
         UPPER_BOUND: float('inf'),
     },
     InnerParameterType.SPLINE: {
         LOWER_BOUND: -float('inf'),
         UPPER_BOUND: float('inf'),
     },
@@ -153,15 +154,15 @@
 MAXMIN = 'max-min'
 MAX = 'max'
 
 METHOD = 'method'
 REPARAMETERIZED = 'reparameterized'
 INTERVAL_CONSTRAINTS = 'interval_constraints'
 MIN_GAP = 'min_gap'
-OPTIMAL_SCALING_OPTIONS = [
+ORDINAL_OPTIONS = [
     METHOD,
     REPARAMETERIZED,
     INTERVAL_CONSTRAINTS,
     MIN_GAP,
 ]
 
 CAT_LB = 'cat_lb'
@@ -182,23 +183,30 @@
 W_DOT_MATRIX = 'W_dot_matrix'
 
 SCIPY_SUCCESS = 'success'
 SCIPY_FUN = 'fun'
 SCIPY_X = 'x'
 
 ###############################################################################
-# SPLINE APPROXIMATION
+# SPLINE APPROXIMATION FOR SEMIQUANTITATIVE DATA
 
 MEASUREMENT_TYPE = 'measurementType'
 
-NONLINEAR_MONOTONE = 'nonlinear_monotone'
+SEMIQUANTITATIVE = 'semiquantitative'
 
 SPLINE_RATIO = 'spline_ratio'
 MIN_DIFF_FACTOR = 'min_diff_factor'
-SPLINE_APPROXIMATION_OPTIONS = [SPLINE_RATIO, MIN_DIFF_FACTOR]
+REGULARIZE_SPLINE = 'regularize_spline'
+REGULARIZATION_FACTOR = 'regularization_factor'
+SPLINE_APPROXIMATION_OPTIONS = [
+    SPLINE_RATIO,
+    MIN_DIFF_FACTOR,
+    REGULARIZE_SPLINE,
+    REGULARIZATION_FACTOR,
+]
 
 MIN_SIM_RANGE = 1e-16
 
 SPLINE_PAR_TYPE = 'spline'
 N_SPLINE_PARS = 'n_spline_pars'
 DATAPOINTS = 'datapoints'
 MIN_DATAPOINT = 'min_datapoint'
@@ -220,14 +228,20 @@
 EXITFLAG = "exitflag"
 TRACE_SAVE_ITER = "trace_save_iter"
 
 SUFFIXES_CSV = ["csv"]
 SUFFIXES_HDF5 = ["hdf5", "h5"]
 SUFFIXES = SUFFIXES_CSV + SUFFIXES_HDF5
 
+CPU_TIME_TOTAL = 'cpu_time_total'
+PREEQ_CPU_TIME = 'preeq_cpu_time'
+PREEQ_CPU_TIME_BACKWARD = 'preeq_cpu_timeB'
+POSTEQ_CPU_TIME = 'posteq_cpu_time'
+POSTEQ_CPU_TIME_BACKWARD = 'posteq_cpu_timeB'
+
 
 ###############################################################################
 # PRIOR
 
 LIN = 'lin'  # linear
 LOG = 'log'  # logarithmic to basis e
 LOG10 = 'log10'  # logarithmic to basis 10
```

### Comparing `pypesto-0.4.1/pypesto/__init__.py` & `pypesto-0.4.2/pypesto/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 from .version import __version__
 
 # import basic objects into global namespace
 from .history import (
     CountHistory,
     CountHistoryBase,
     CsvHistory,
+    CsvAmiciHistory,
     Hdf5History,
+    Hdf5AmiciHistory,
     NoHistory,
     HistoryBase,
     HistoryOptions,
     MemoryHistory,
     OptimizerHistory,
 )
 from .objective import (
```

### Comparing `pypesto-0.4.1/pypesto/engine/base.py` & `pypesto-0.4.2/pypesto/engine/single_core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-"""Abstract engine base class."""
-import abc
+"""Engines without parallelization."""
+
 from typing import Any
 
+from ..util import tqdm
+from .base import Engine
 from .task import Task
 
 
-class Engine(abc.ABC):
-    """Abstract engine base class."""
+class SingleCoreEngine(Engine):
+    """
+    Dummy engine for sequential execution on one core.
+
+    .. note:: The objective itself may be multithreaded.
+    """
 
     def __init__(self):
-        pass
+        super().__init__()
 
-    @abc.abstractmethod
     def execute(
-        self, tasks: list[Task], progress_bar: bool = True
+        self, tasks: list[Task], progress_bar: bool = None
     ) -> list[Any]:
-        """Execute tasks.
+        """Execute all tasks in a simple for loop sequentially.
 
         Parameters
         ----------
         tasks:
             List of tasks to execute.
         progress_bar:
-            Whether to display a progress bar. Defaults to ``True``.
+            Whether to display a progress bar.
+
+        Returns
+        -------
+        A list of results.
         """
-        raise NotImplementedError("This engine is not intended to be called.")
+        results = []
+        for task in tqdm(
+            tasks,
+            enable=progress_bar,
+        ):
+            results.append(task.execute())
+
+        return results
```

### Comparing `pypesto-0.4.1/pypesto/engine/mpi_pool.py` & `pypesto-0.4.2/pypesto/engine/mpi_pool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Engines with multi-node parallelization."""
+
 import logging
 from typing import Any
 
 import cloudpickle as pickle
 from mpi4py import MPI
 from mpi4py.futures import MPIPoolExecutor
-from tqdm import tqdm
 
+from ..util import tqdm
 from .base import Engine
 from .task import Task
 
 logger = logging.getLogger(__name__)
 
 
 def work(pickled_task):
@@ -28,33 +29,33 @@
     ``mpiexec -np #Workers+1 python -m mpi4py.futures YOURFILE.py``
     """
 
     def __init__(self):
         super().__init__()
 
     def execute(
-        self, tasks: list[Task], progress_bar: bool = True
+        self, tasks: list[Task], progress_bar: bool = None
     ) -> list[Any]:
         """
         Pickle tasks and distribute work to workers.
 
         Parameters
         ----------
         tasks:
             List of :class:`pypesto.engine.Task` to execute.
         progress_bar:
-            Whether to display a progress bar. Defaults to ``True``.
+            Whether to display a progress bar.
 
         Returns
         -------
         A list of results.
         """
         pickled_tasks = [pickle.dumps(task) for task in tasks]
 
         n_procs = MPI.COMM_WORLD.Get_size()  # Size of communicator
         logger.info(f"Parallelizing on {n_procs-1} workers with one manager.")
 
         with MPIPoolExecutor() as executor:
             results = executor.map(
-                work, tqdm(pickled_tasks, disable=not progress_bar)
+                work, tqdm(pickled_tasks, enable=progress_bar)
             )
         return results
```

### Comparing `pypesto-0.4.1/pypesto/engine/multi_process.py` & `pypesto-0.4.2/pypesto/engine/multi_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Engines with multi-process parallelization."""
+
 import logging
 import multiprocessing
 import os
 from typing import Any, Union
 
 import cloudpickle as pickle
-from tqdm import tqdm
 
+from ..util import tqdm
 from .base import Engine
 from .task import Task
 
 logger = logging.getLogger(__name__)
 
 
 def work(pickled_task):
@@ -48,24 +49,24 @@
             logger.info(
                 f"Engine will use up to {n_procs} processes (= CPU count)."
             )
         self.n_procs: int = n_procs
         self.method: str = method
 
     def execute(
-        self, tasks: list[Task], progress_bar: bool = True
+        self, tasks: list[Task], progress_bar: bool = None
     ) -> list[Any]:
         """Pickle tasks and distribute work over parallel processes.
 
         Parameters
         ----------
         tasks:
             List of :class:`pypesto.engine.Task` to execute.
         progress_bar:
-            Whether to display a progress bar. Defaults to ``True``.
+            Whether to display a progress bar.
 
         Returns
         -------
         A list of results.
         """
         n_tasks = len(tasks)
 
@@ -77,12 +78,12 @@
         ctx = multiprocessing.get_context(method=self.method)
 
         with ctx.Pool(processes=n_procs) as pool:
             results = list(
                 tqdm(
                     pool.imap(work, pickled_tasks),
                     total=len(pickled_tasks),
-                    disable=not progress_bar,
+                    enable=progress_bar,
                 ),
             )
 
         return results
```

### Comparing `pypesto-0.4.1/pypesto/engine/multi_thread.py` & `pypesto-0.4.2/pypesto/engine/multi_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Engines with multi-threading parallelization."""
+
 import copy
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Union
 
-from tqdm import tqdm
-
+from ..util import tqdm
 from .base import Engine
 from .task import Task
 
 logger = logging.getLogger(__name__)
 
 
 def work(task):
@@ -39,15 +39,15 @@
             n_threads = os.cpu_count()
             logger.info(
                 f"Engine will use up to {n_threads} threads (= CPU count)."
             )
         self.n_threads: int = n_threads
 
     def execute(
-        self, tasks: list[Task], progress_bar: bool = True
+        self, tasks: list[Task], progress_bar: bool = None
     ) -> list[Any]:
         """Deepcopy tasks and distribute work over parallel threads.
 
         Parameters
         ----------
         tasks:
             List of tasks to execute.
@@ -66,12 +66,12 @@
         logger.debug(f"Parallelizing on {n_threads} threads.")
 
         with ThreadPoolExecutor(max_workers=n_threads) as pool:
             results = list(
                 tqdm(
                     pool.map(work, copied_tasks),
                     total=len(copied_tasks),
-                    disable=not progress_bar,
+                    enable=progress_bar,
                 ),
             )
 
         return results
```

### Comparing `pypesto-0.4.1/pypesto/ensemble/__init__.py` & `pypesto-0.4.2/pypesto/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/ensemble/covariance_analysis.py` & `pypesto-0.4.2/pypesto/ensemble/covariance_analysis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/ensemble/dimension_reduction.py` & `pypesto-0.4.2/pypesto/ensemble/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/ensemble/ensemble.py` & `pypesto-0.4.2/pypesto/ensemble/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 from __future__ import annotations
 
 import logging
 from functools import partial
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Callable, Optional, Sequence, Union
 
 import numpy as np
 import pandas as pd
 from scipy.stats import chi2
 
 from ..C import (
     ENSEMBLE_TYPE,
@@ -67,15 +58,15 @@
 
 class EnsemblePrediction:
     """
     Class of ensemble prediction.
 
     An ensemble prediction consists of an ensemble, i.e., a set of parameter
     vectors and their identifiers such as a sample, and a prediction function.
-    It can be attached to a ensemble-type object
+    It can be attached to an ensemble-type object.
     """
 
     def __init__(
         self,
         predictor: Optional[Callable[[Sequence], PredictionResult]] = None,
         prediction_id: str = None,
         prediction_results: Sequence[PredictionResult] = None,
@@ -99,16 +90,14 @@
             the same shape as the output of the predictions, i.e., a list of
             numpy array (one list entry per condition), with the arrays having
             the shape of n_timepoints x n_outputs for each condition.
         upper_bound:
             array of potential upper bounds for the parameters
         """
         self.predictor = predictor
-        if predictor is None:
-            logger.info("This `EnsemblePrediction` has no predictor.")
         self.prediction_id = prediction_id
         self.prediction_results = prediction_results
         if prediction_results is None:
             self.prediction_results = []
 
         # handle bounds, Not yet Implemented
         if lower_bound is not None:
@@ -200,15 +189,15 @@
         }
 
     def compute_summary(
         self,
         percentiles_list: Sequence[int] = (5, 20, 80, 95),
         weighting: bool = False,
         compute_weighted_sigma: bool = False,
-    ) -> Dict:
+    ) -> dict:
         """
         Compute summary from the ensemble prediction results.
 
         Summary includes the mean, the median, the standard deviation and
         possibly percentiles. Those summary results are added as a data
         member to the EnsemblePrediction object.
 
@@ -220,34 +209,33 @@
             Whether weights should be used for trajectory.
         compute_weighted_sigma:
             Whether weighted standard deviation of the ensemble mean trajectory
             should be computed. Defaults to False.
 
         Returns
         -------
-        summary:
-            dictionary of predictions results with the keys mean, std, median,
-            percentiles, ...
+        dictionary of predictions results with the keys mean, std, median,
+        percentiles, ...
         """
         # check if prediction results are available
         if not self.prediction_results:
             raise ArithmeticError(
                 'Cannot compute summary statistics from '
                 'empty prediction results.'
             )
         # if weightings shall be used, check whether weights are there
         if weighting:
             if not self.prediction_results[0].conditions[0].output_weight:
                 raise ValueError(
-                    'There are no weights in the ' 'prediction results.'
+                    'There are no weights in the prediction results.'
                 )
 
         n_conditions = len(self.prediction_results[0].conditions)
 
-        def _stack_outputs(ic: int):
+        def _stack_outputs(ic: int) -> np.array:
             """
             Stack outputs.
 
             Group outputs for different parameter vectors of one ensemble
             together, if they belong to the same simulation condition, and
             stack them in one array.
             """
@@ -258,34 +246,34 @@
             output_list = [
                 prediction.conditions[ic].output
                 for prediction in self.prediction_results
             ]
             # stack into one numpy array
             return np.stack(output_list, axis=-1)
 
-        def _stack_outputs_sensi(ic: int):
+        def _stack_outputs_sensi(ic: int) -> np.array:
             """
             Stack output sensitivities.
 
             Group output sensitivities for different parameter vectors of one
             ensemble together, if they belong to the same simulation condition,
             and stack them in one array.
             """
-            # Were output sensitivitiess computed
+            # Were output sensitivities computed?
             if self.prediction_results[0].conditions[ic].output_sensi is None:
                 return None
             # stack predictions
             output_sensi_list = [
                 prediction.conditions[ic].output_sensi
                 for prediction in self.prediction_results
             ]
             # stack into one numpy array
             return np.stack(output_sensi_list, axis=-1)
 
-        def _stack_weights(ic: int) -> np.ndarray:
+        def _stack_weights(ic: int) -> Union[np.ndarray, None]:
             """
             Stack weights.
 
             Group weights for different parameter vectors of one ensemble
             together, if they belong to the same simulation condition, and
             stack them in one array
 
@@ -361,15 +349,15 @@
         if compute_weighted_sigma:
             cond_lists[WEIGHTED_SIGMA] = []
         for perc in percentiles_list:
             cond_lists[get_percentile_label(perc)] = []
 
         # iterate over conditions, compute summary
         for i_cond in range(n_conditions):
-            # use some short hand
+            # use some shorthand
             current_cond = self.prediction_results[0].conditions[i_cond]
 
             # create a temporary array with all the outputs needed and wanted
             tmp_output = _stack_outputs(i_cond)
             tmp_output_sensi = _stack_outputs_sensi(i_cond)
             tmp_weights = np.ones(tmp_output.shape[-1])
             if weighting:
@@ -418,15 +406,15 @@
             )
             for i_key in cond_lists.keys()
         }
 
         # also return the object
         return self.prediction_summary
 
-    def compute_chi2(self, amici_objective: AmiciObjective):
+    def compute_chi2(self, amici_objective: AmiciObjective) -> float:
         """
         Compute the chi^2 error of the weighted mean trajectory.
 
         Parameters
         ----------
         amici_objective:
             The objective function of the model,
@@ -485,15 +473,15 @@
     other.
     """
 
     def __init__(
         self,
         x_vectors: np.ndarray,
         x_names: Sequence[str] = None,
-        vector_tags: Sequence[Tuple[int, int]] = None,
+        vector_tags: Sequence[tuple[int, int]] = None,
         ensemble_type: EnsembleType = None,
         predictions: Sequence[EnsemblePrediction] = None,
         lower_bound: np.ndarray = None,
         upper_bound: np.ndarray = None,
     ):
         """
         Initialize.
@@ -502,29 +490,29 @@
         ----------
         x_vectors:
             parameter vectors of the ensemble, in the format
             n_parameter x n_vectors
         x_names:
             Names or identifiers of the parameters
         vector_tags:
-            Additional tag, which adds information about the the parameter
-            vectors of the form (optimization_run, optimization_step) if the
-            ensemble is created from an optimization result or
-            (sampling_chain, sampling_step) if the ensemble is created from a
-            sampling result.
+            Additional tag, which adds information about the parameter
+            vectors. For example, `(optimization_run, optimization_step)` if the
+            ensemble is created from an optimization result or history
+            (see :meth:`from_optimization_endpoints`, :meth:`from_optimization_history`).
         ensemble_type:
-            Type of ensemble: Ensemble (default), sample, or unprocessed_chain
+            Type of ensemble: :obj:`EnsembleType.ensemble` (default), :obj:`EnsembleType.sample`,
+            or :obj:`EnsembleType.unprocessed_chain`.
             Samples are meant to be representative, ensembles can be any
-            ensemble of parameters, and unprocessed chains still have burn-ins
+            ensemble of parameters, and unprocessed chains still have burn-ins.
         predictions:
-            List of EnsemblePrediction objects
+            List of :class:`EnsemblePrediction` objects.
         lower_bound:
-            array of potential lower bounds for the parameters
+            Array of potential lower bounds for the parameters.
         upper_bound:
-            array of potential upper bounds for the parameters
+            Array of potential upper bounds for the parameters.
         """
         # Do we have a representative sample or just random ensemble?
         self.ensemble_type = EnsembleType.ensemble
         if ensemble_type is not None:
             self.ensemble_type = ensemble_type
 
         # handle parameter vectors and sizes
@@ -564,15 +552,15 @@
         result: Result,
         remove_burn_in: bool = True,
         chain_slice: slice = None,
         x_names: Sequence[str] = None,
         lower_bound: np.ndarray = None,
         upper_bound: np.ndarray = None,
         **kwargs,
-    ):
+    ) -> Ensemble:
         """
         Construct an ensemble from a sample.
 
         Parameters
         ----------
         result:
             A pyPESTO result that contains a sample result.
@@ -621,15 +609,15 @@
     @staticmethod
     def from_optimization_endpoints(
         result: Result,
         rel_cutoff: float = None,
         max_size: int = np.inf,
         percentile: float = None,
         **kwargs,
-    ):
+    ) -> Ensemble:
         """
         Construct an ensemble from an optimization result.
 
         Parameters
         ----------
         result:
             A pyPESTO result that contains an optimization result.
@@ -713,15 +701,15 @@
         result: Result,
         rel_cutoff: float = None,
         max_size: int = np.inf,
         max_per_start: int = np.inf,
         distribute: bool = True,
         percentile: float = None,
         **kwargs,
-    ):
+    ) -> Ensemble:
         """
         Construct an ensemble from the history of an optimization.
 
         Parameters
         ----------
         result:
             A pyPESTO result that contains an optimization result
@@ -737,15 +725,15 @@
             The maximum number of vectors to be included from a
             single optimization start.
         distribute:
             Boolean flag, whether the best (False) values from the
             start should be taken or whether the indices should be
             more evenly distributed.
         percentile:
-            Percentile of a chi^2 distribution. Used to determinie the
+            Percentile of a chi^2 distribution. Used to determine the
             cutoff value.
 
         Returns
         -------
         The ensemble.
         """
         if rel_cutoff is None and percentile is None:
@@ -850,53 +838,54 @@
         yield LOWER_BOUND, self.lower_bound
         yield UPPER_BOUND, self.upper_bound
 
     def _map_parameters_by_objective(
         self,
         predictor: Callable,
         default_value: float = None,
-    ):
+    ) -> list[Union[int, float]]:
         """
-        Create mapping for parameters from ensebmle to predictor.
+        Create mapping for parameters from ensemble to predictor.
 
         The parameters of the ensemble don't need to have the same ordering as
         in the predictor.
         """
         # create short hands
         parameter_ids_objective = predictor.amici_objective.x_names
-        parameter_ids_ensemble = self.x_names
+        parameter_ids_ensemble = list(self.x_names)
         # map, and fill with `default_value` if not found and `default_value`
         # is specified.
         mapping = []
         for parameter_id_objective in parameter_ids_objective:
             if parameter_id_objective in parameter_ids_ensemble:
+                # Append index of parameter in ensemble.
                 mapping.append(
                     parameter_ids_ensemble.index(parameter_id_objective)
                 )
             elif default_value is not None:
                 mapping.append(default_value)
         return mapping
 
     def predict(
         self,
         predictor: Callable,
         prediction_id: str = None,
-        sensi_orders: Tuple = (0,),
+        sensi_orders: tuple = (0,),
         default_value: float = None,
         mode: ModeType = MODE_FUN,
         include_llh_weights: bool = False,
         include_sigmay: bool = False,
         engine: Engine = None,
-        progress_bar: bool = True,
+        progress_bar: bool = None,
     ) -> EnsemblePrediction:
         """
         Run predictions for a full ensemble.
 
         User needs to hand over a predictor function and settings, then all
-        results are grouped as EnsemblePrediction for the whole ensemble
+        results are grouped as :class:`EnsemblePrediction` for the whole ensemble.
 
         Parameters
         ----------
         predictor:
             Prediction function, e.g., an AmiciPredictor
         prediction_id:
             Identifier for the predictions
@@ -923,15 +912,15 @@
         Returns
         -------
         The prediction of the ensemble.
         """
         if engine is None:
             engine = SingleCoreEngine()
 
-        # Vectors are chunked to improve parallization performance.
+        # Vectors are chunked to improve parallelization performance.
         n_chunks = self.n_vectors  # Default is no chunking.
         if isinstance(engine, MultiProcessEngine):
             n_chunks = engine.n_procs
         if isinstance(engine, MultiThreadEngine):
             n_chunks = engine.n_threads
         chunks = [
             (
@@ -946,27 +935,27 @@
 
         # Get the correct parameter mapping.
         mapping = self._map_parameters_by_objective(
             predictor,
             default_value=default_value,
         )
 
-        # Setup the tasks with the prediction method and chunked vectors.
+        # Set up the tasks with the prediction method and chunked vectors.
         method = partial(
             predictor,
             sensi_orders=sensi_orders,
             mode=mode,
             include_sigmay=include_sigmay,
             include_llh_weights=include_llh_weights,
         )
         tasks = [
             EnsembleTask(
                 method=method,
                 vectors=self.x_vectors[mapping, chunk_start:chunk_end],
-                id=chunk_i,
+                id=str(chunk_i),
             )
             for chunk_i, (chunk_start, chunk_end) in enumerate(chunks)
         ]
 
         # Execute tasks and flatten chunked results.
         prediction_results = [
             prediction_result
@@ -980,31 +969,30 @@
             predictor=predictor,
             prediction_id=prediction_id,
             prediction_results=prediction_results,
         )
 
     def compute_summary(
         self, percentiles_list: Sequence[int] = (5, 20, 80, 95)
-    ):
+    ) -> dict[str, np.array]:
         """
         Compute summary for the parameters of the ensemble.
 
         Summary includes the mean, the median, the standard deviation and
         possibly percentiles. Those summary results are added as a data
         member to the EnsemblePrediction object.
 
         Parameters
         ----------
         percentiles_list:
             List or tuple of percent numbers for the percentiles
 
         Returns
         -------
-        summary:
-            Dict with mean, std, median, and percentiles of parameter vectors
+        Dict with mean, std, median, and percentiles of parameter vectors
         """
         # compute summaries based on parameters
         summary = {
             MEAN: np.mean(self.x_vectors, axis=1),
             STANDARD_DEVIATION: np.std(self.x_vectors, axis=1),
             MEDIAN: np.median(self.x_vectors, axis=1),
         }
@@ -1017,16 +1005,16 @@
         return summary
 
     def check_identifiability(self) -> pd.DataFrame:
         """
         Check identifiability of ensemble.
 
         Use ensemble mean and standard deviation to assess (in a rudimentary
-        way) whether or not parameters are identifiable. Returns a dataframe
-        with tuples, which specify whether or not the lower and the upper
+        way) whether parameters are identifiable. Returns a dataframe
+        with tuples, which specify whether the lower and the upper
         bounds are violated.
 
         Returns
         -------
         parameter_identifiability:
             DataFrame indicating parameter identifiability based on mean
             plus/minus standard deviations and parameter bounds
@@ -1084,19 +1072,19 @@
             'parameterId'
         ]
 
         return parameter_identifiability
 
 
 def entries_per_start(
-    fval_traces: List['np.ndarray'],
+    fval_traces: list['np.ndarray'],
     cutoff: float,
     max_size: int,
     max_per_start: int,
-):
+) -> list[int]:
     """
     Create the indices of each start that will be included in the ensemble.
 
     Parameters
     ----------
     fval_traces:
         the fval-trace of each start.
@@ -1107,24 +1095,24 @@
         The maximum size the ensemble should be.
     max_per_start:
         The maximum number of vectors to be included from a
         single optimization start.
 
     Returns
     -------
-        A list of number of candidates per start that are to
-        be included in the ensemble.
+    A list of number of candidates per start that are to
+    be included in the ensemble.
     """
     # choose possible candidates
     ens_ind = [np.flatnonzero(fval <= cutoff) for fval in fval_traces]
 
     # count the number of candidates per start
     n_theo = np.array([len(start) for start in ens_ind])
 
-    # trimm down starts that exceed the limit:
+    # trim down starts that exceed the limit:
     n_per_start = [min(n, max_per_start) for n in n_theo]
 
     # if all possible indices can be included, return
     if sum(n_per_start) < max_size:
         return n_per_start
     n_equally = max_size // len(n_per_start)
     n_left = max_size % len(n_per_start)
@@ -1162,15 +1150,15 @@
     distribute:
         Boolean flag, whether the best (False) values from the
         start should be taken or whether the indices should be
         more evenly distributed.
 
     Returns
     -------
-        The indices to include in the ensemble.
+    The indices to include in the ensemble.
     """
     candidates = np.flatnonzero(trace_start <= cutoff)
 
     if distribute:
         indices = np.round(np.linspace(0, len(candidates) - 1, n_vectors))
         return candidates[indices.astype(int)]
     else:
@@ -1209,23 +1197,23 @@
             percentile_str += '...'
         percentile = percentile_str
     return f'{PERCENTILE} {percentile}'
 
 
 def calculate_cutoff(
     result: Result,
-    percentile: float = 0.95,
+    percentile: float = 95,
     cr_option: str = SIMULTANEOUS,
 ):
     """
     Calculate the cutoff of the ensemble.
 
     Based on the number of parameters of the problem. Based on the
     assumption that the difference of the nllh's of the true and optimal
-    parameter is chi^2 distributed with n_theta degress of freedom.
+    parameter is chi^2 distributed with n_theta degrees of freedom.
 
     Parameters
     ----------
     result:
         The optimization result from which to create the ensemble.
     percentile:
         The percentile of the chi^2 distribution. Between 0 and 100.
```

### Comparing `pypesto-0.4.1/pypesto/ensemble/task.py` & `pypesto-0.4.2/pypesto/ensemble/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/ensemble/util.py` & `pypesto-0.4.2/pypesto/ensemble/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/hierarchical/calculator.py` & `pypesto-0.4.2/pypesto/hierarchical/ordinal/calculator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,227 @@
-from __future__ import annotations
+"""Definition of an optimal scaling calculator class."""
 
 import copy
-from typing import Dict, List, Optional, Sequence, Tuple
+from typing import Sequence
 
 import numpy as np
 
-try:
-    import amici
-    from amici.parameter_mapping import ParameterMapping
-except ImportError:
-    pass
-
-from ..C import (
+from ...C import (
     AMICI_SIGMAY,
+    AMICI_SSIGMAY,
+    AMICI_SY,
     AMICI_Y,
+    FVAL,
     GRAD,
     HESS,
-    INNER_PARAMETERS,
-    INNER_RDATAS,
+    MODE_RES,
     RDATAS,
-    ModeType,
+    RES,
+    SRES,
+    X_INNER_OPT,
 )
-from ..objective.amici.amici_calculator import (
+from ...objective.amici.amici_calculator import (
     AmiciCalculator,
     AmiciModel,
     AmiciSolver,
 )
-from .problem import AmiciInnerProblem
-from .solver import AnalyticalInnerSolver, InnerSolver
+from ...objective.amici.amici_util import (
+    filter_return_dict,
+    init_return_values,
+)
+from .problem import OrdinalProblem
+from .solver import OrdinalInnerSolver
 
+try:
+    import amici
+    from amici.parameter_mapping import ParameterMapping
+except ImportError:
+    pass
 
-class HierarchicalAmiciCalculator(AmiciCalculator):
-    """A calculator that is passed as `calculator` to the pypesto.AmiciObjective."""
+
+class OrdinalCalculator(AmiciCalculator):
+    """A calculator is passed as `calculator` to the pypesto.AmiciObjective.
+
+    The object is called by :func:`pypesto.AmiciObjective.call_unprocessed`
+    to calculate the current objective function values and gradient.
+    """
 
     def __init__(
         self,
-        inner_problem: AmiciInnerProblem,
-        inner_solver: Optional[InnerSolver] = None,
+        inner_problem: OrdinalProblem,
+        inner_solver: OrdinalInnerSolver = None,
     ):
         """Initialize the calculator from the given problem.
 
-        Arguments
-        ---------
+        Parameters
+        ----------
         inner_problem:
-            The inner problem of a hierarchical optimization problem.
+            The optimal scaling inner problem.
         inner_solver:
             A solver to solve ``inner_problem``.
-            Defaults to ``pypesto.hierarchical.solver.AnalyticalInnerSolver``.
+            Defaults to ``OptimalScalingInnerSolver``.
         """
         super().__init__()
-
         self.inner_problem = inner_problem
 
         if inner_solver is None:
-            inner_solver = AnalyticalInnerSolver()
+            inner_solver = OrdinalInnerSolver()
         self.inner_solver = inner_solver
+        if (
+            self.inner_problem.method
+            is not self.inner_solver.options['method']
+        ):
+            raise ValueError(
+                f"The inner problem method {self.inner_problem.method} and the inner solver method {self.inner_solver.options['method']} have to coincide."
+            )
 
     def initialize(self):
         """Initialize."""
-        super().initialize()
         self.inner_solver.initialize()
-
-    def get_inner_parameter_ids(self) -> List[str]:
-        """Get the ids of the inner parameters."""
-        return self.inner_problem.get_x_ids()
+        self.inner_problem.initialize()
 
     def __call__(
         self,
-        x_dct: Dict,
-        sensi_orders: Tuple[int],
-        mode: ModeType,
+        x_dct: dict,
+        sensi_orders: tuple[int, ...],
+        mode: str,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: List[amici.ExpData],
+        edatas: list['amici.ExpData'],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
+        rdatas: list['amici.ReturnData'] = None,
     ):
-        """Perform the actual AMICI call, with hierarchical optimization.
-
-        See documentation for
-        `pypesto.objective.amici.amici_calculator.AmiciCalculator.__call__()`.
+        """Perform the actual AMICI call.
 
-        The return object also includes the simulation results that were
-        generated to solve the inner problem, as well as the parameters that
-        solver the inner problem.
+        Parameters
+        ----------
+        x_dct:
+            Parameters for which to compute function value and derivatives.
+        sensi_orders:
+            Tuple of requested sensitivity orders.
+        mode:
+            Call mode (function value or residual based).
+        amici_model:
+            The AMICI model.
+        amici_solver:
+            The AMICI solver.
+        edatas:
+            The experimental data.
+        n_threads:
+            Number of threads for AMICI call.
+        x_ids:
+            Ids of optimization parameters.
+        parameter_mapping:
+            Mapping of optimization to simulation parameters.
+        fim_for_hess:
+            Whether to use the FIM (if available) instead of the Hessian (if
+            requested).
+        rdatas:
+            AMICI simulation return data. In case the calculator is part of
+            the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
+            it will already simulate the model and pass the results here.
+
+        Returns
+        -------
+        inner_result:
+            A dict containing the calculation results: FVAL, GRAD, RDATAS and X_INNER_OPT.
         """
-        if not self.inner_problem.check_edatas(edatas=edatas):
+        if mode == MODE_RES:
             raise ValueError(
-                'The experimental data provided to this call differs from '
-                'the experimental data used to setup the hierarchical '
-                'optimizer.'
+                "Optimal scaling method cannot be called with residual mode."
+            )
+        if 2 in sensi_orders:
+            raise ValueError(
+                "Hessian and FIM are not implemented for the optimal scaling calculator."
             )
 
-        # compute optimal inner parameters
-        x_dct = copy.deepcopy(x_dct)
-        x_dct.update(self.inner_problem.get_dummy_values(scaled=True))
-        inner_result = super().__call__(
-            x_dct=x_dct,
-            sensi_orders=(0,),
-            mode=mode,
-            amici_model=amici_model,
-            amici_solver=amici_solver,
-            edatas=edatas,
-            n_threads=n_threads,
-            x_ids=x_ids,
-            parameter_mapping=parameter_mapping,
-            fim_for_hess=fim_for_hess,
+        # get dimension of outer problem
+        dim = len(x_ids)
+
+        # initialize return values
+        nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
+            sensi_orders, mode, dim
         )
-        inner_rdatas = inner_result[RDATAS]
+        # set order in solver
+        sensi_order = 0
+        if sensi_orders:
+            sensi_order = max(sensi_orders)
+
+        # If AMICI ReturnData is not provided, we need to simulate the model
+        if rdatas is None:
+            amici_solver.setSensitivityOrder(sensi_order)
+
+            x_dct = copy.deepcopy(x_dct)
+
+            # fill in parameters
+            amici.parameter_mapping.fill_in_parameters(
+                edatas=edatas,
+                problem_parameters=x_dct,
+                scaled_parameters=True,
+                parameter_mapping=parameter_mapping,
+                amici_model=amici_model,
+            )
+            # run amici simulation
+            rdatas = amici.runAmiciSimulations(
+                amici_model,
+                amici_solver,
+                edatas,
+                num_threads=min(n_threads, len(edatas)),
+            )
+
+        inner_result = {
+            FVAL: nllh,
+            GRAD: snllh,
+            HESS: s2nllh,
+            RES: res,
+            SRES: sres,
+            RDATAS: rdatas,
+            X_INNER_OPT: self.inner_problem.get_inner_parameter_dictionary(),
+        }
 
         # if any amici simulation failed, it's unlikely we can compute
         # meaningful inner parameters, so we better just fail early.
-        if any(rdata.status != amici.AMICI_SUCCESS for rdata in inner_rdatas):
-            # if the gradient was requested, we need to provide some value
-            # for it
-            dim = len(x_ids)
+        if any(rdata.status != amici.AMICI_SUCCESS for rdata in rdatas):
+            inner_result[FVAL] = np.inf
+            # if the gradient was requested,
+            # we need to provide some value for it
             if 1 in sensi_orders:
-                inner_result[GRAD] = np.full(shape=dim, fill_value=np.nan)
-            if 2 in sensi_orders:
-                inner_result[HESS] = np.full(
-                    shape=(dim, dim), fill_value=np.nan
+                inner_result[GRAD] = np.full(
+                    shape=len(x_ids), fill_value=np.nan
                 )
-            return inner_result
+            return filter_return_dict(inner_result)
 
-        inner_parameters = self.inner_solver.solve(
-            problem=self.inner_problem,
-            sim=[rdata[AMICI_Y] for rdata in inner_rdatas],
-            sigma=[rdata[AMICI_SIGMAY] for rdata in inner_rdatas],
-            scaled=True,
-        )
+        sim = [rdata[AMICI_Y] for rdata in rdatas]
+        sigma = [rdata[AMICI_SIGMAY] for rdata in rdatas]
 
-        # fill in optimal values
-        # directly writing to parameter mapping ensures that plists do not
-        # include hierarchically computed parameters
-        x_dct = copy.deepcopy(x_dct)
-        x_dct.update(inner_parameters)
-
-        # TODO use plist to compute only required derivatives, in
-        #  `super.__call__`, `amici.parameter_mapping.fill_in_parameters`
-        # TODO speed gain: if no gradient is required, then simulation can be
-        #  skipped here, and rdatas can be updated in place
-        #  (y, sigma, res, llh).
-        result = super().__call__(
-            x_dct=x_dct,
-            sensi_orders=sensi_orders,
-            mode=mode,
-            amici_model=amici_model,
-            amici_solver=amici_solver,
-            edatas=edatas,
-            n_threads=n_threads,
-            x_ids=x_ids,
-            parameter_mapping=parameter_mapping,
-            fim_for_hess=fim_for_hess,
+        # compute optimal inner parameters
+        x_inner_opt = self.inner_solver.solve(self.inner_problem, sim, sigma)
+        inner_result[FVAL] = self.inner_solver.calculate_obj_function(
+            x_inner_opt
         )
-        result[INNER_PARAMETERS] = inner_parameters
-        result[INNER_RDATAS] = inner_rdatas
+        inner_result[
+            X_INNER_OPT
+        ] = self.inner_problem.get_inner_parameter_dictionary()
+
+        # calculate analytical gradients if requested
+        if sensi_order > 0:
+            # print([opt['fun'] for opt in x_inner_opt])
+            sy = [rdata[AMICI_SY] for rdata in rdatas]
+            ssigma = [rdata[AMICI_SSIGMAY] for rdata in rdatas]
+            inner_result[GRAD] = self.inner_solver.calculate_gradients(
+                problem=self.inner_problem,
+                x_inner_opt=x_inner_opt,
+                sim=sim,
+                sy=sy,
+                sigma=sigma,
+                ssigma=ssigma,
+                parameter_mapping=parameter_mapping,
+                par_opt_ids=x_ids,
+                par_sim_ids=amici_model.getParameterIds(),
+                par_edatas_indices=[edata.plist for edata in edatas],
+                snllh=snllh,
+            )
 
-        return result
+        return filter_return_dict(inner_result)
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/inner_calculator_collector.py` & `pypesto-0.4.2/pypesto/hierarchical/inner_calculator_collector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 """Module for the InnerCalculatorCollector class.
 
-In case of non-quantitative measurements, this class is used to collect
-hierarchical inner calculators for each data type and merge their results.
+In case of semi-quantitative or qualitative measurements, this class is used
+to collect hierarchical inner calculators for each data type and merge their results.
 """
+
 from __future__ import annotations
 
 import copy
-from typing import Dict, List, Sequence, Tuple, Union
+from typing import Sequence, Union
 
 import numpy as np
 
 from ..C import (
     AMICI_SIGMAY,
     AMICI_SSIGMAY,
     AMICI_SSIGMAZ,
     AMICI_SY,
     AMICI_Y,
     CENSORED,
     FVAL,
     GRAD,
     HESS,
     INNER_PARAMETERS,
-    MEASUREMENT_TYPE,
     METHOD,
     MODE_RES,
-    NONLINEAR_MONOTONE,
-    OPTIMAL_SCALING_OPTIONS,
     ORDINAL,
+    ORDINAL_OPTIONS,
     RDATAS,
+    RELATIVE,
     RES,
+    SEMIQUANTITATIVE,
     SPLINE_APPROXIMATION_OPTIONS,
     SPLINE_RATIO,
     SRES,
     X_INNER_OPT,
     ModeType,
 )
 from ..objective.amici.amici_calculator import AmiciCalculator
-from ..objective.amici.amici_util import filter_return_dict, init_return_values
+from ..objective.amici.amici_util import (
+    add_sim_grad_to_opt_grad,
+    filter_return_dict,
+    init_return_values,
+)
 
 try:
     import amici
     import petab
     from amici.parameter_mapping import ParameterMapping
-    from petab.C import OBSERVABLE_ID
 except ImportError:
     petab = None
     ParameterMapping = None
 
-from .optimal_scaling import (
-    OptimalScalingAmiciCalculator,
-    OptimalScalingInnerSolver,
-    OptimalScalingProblem,
-)
-from .spline_approximation import (
-    SplineAmiciCalculator,
-    SplineInnerProblem,
-    SplineInnerSolver,
+from .ordinal import OrdinalCalculator, OrdinalInnerSolver, OrdinalProblem
+from .relative import RelativeAmiciCalculator, RelativeInnerProblem
+from .semiquantitative import (
+    SemiquantCalculator,
+    SemiquantInnerSolver,
+    SemiquantProblem,
 )
 
 AmiciModel = Union['amici.Model', 'amici.ModelPtr']
 AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
 
 
 class InnerCalculatorCollector(AmiciCalculator):
@@ -82,167 +83,209 @@
         The experimental data.
     inner_options:
         Options for the inner problems and solvers.
     """
 
     def __init__(
         self,
-        data_types: List[str],
+        data_types: set[str],
         petab_problem: 'petab.Problem',
         model: AmiciModel,
-        edatas: List['amici.ExpData'],
-        inner_options: Dict,
+        edatas: list['amici.ExpData'],
+        inner_options: dict,
     ):
         super().__init__()
         self.validate_options(inner_options)
 
         self.data_types = data_types
-        self.inner_calculators = []
+        self.inner_calculators: list[
+            AmiciCalculator
+        ] = (
+            []
+        )  # TODO make into a dictionary (future PR, together with .hierarchical of Problem)
         self.construct_inner_calculators(
             petab_problem, model, edatas, inner_options
         )
 
-        self.quantitative_data_mask = self._get_quantitative_data_mask(
-            petab_problem, model.getObservableIds(), edatas
-        )
+        self.quantitative_data_mask = self._get_quantitative_data_mask(edatas)
 
         self._known_least_squares_safe = False
 
     def initialize(self):
         """Initialize."""
         self.best_fval = np.inf
         for calculator in self.inner_calculators:
             calculator.initialize()
 
     def construct_inner_calculators(
         self,
         petab_problem: 'petab.Problem',
         model: AmiciModel,
-        edatas: List['amici.ExpData'],
-        inner_options: Dict,
+        edatas: list['amici.ExpData'],
+        inner_options: dict,
     ):
         """Construct inner calculators for each data type."""
-        self.noise_dummy_values = {}
+        self.necessary_par_dummy_values = {}
         self.best_fval = np.inf
+
+        if RELATIVE in self.data_types:
+            relative_inner_problem = RelativeInnerProblem.from_petab_amici(
+                petab_problem, model, edatas
+            )
+            self.necessary_par_dummy_values.update(
+                relative_inner_problem.get_dummy_values(scaled=True)
+            )
+            relative_inner_solver = RelativeAmiciCalculator(
+                inner_problem=relative_inner_problem
+            )
+            self.inner_calculators.append(relative_inner_solver)
+
         if ORDINAL in self.data_types or CENSORED in self.data_types:
             optimal_scaling_inner_options = {
                 key: value
                 for key, value in inner_options.items()
-                if key in OPTIMAL_SCALING_OPTIONS
+                if key in ORDINAL_OPTIONS
             }
             inner_problem_method = optimal_scaling_inner_options.get(
                 METHOD, None
             )
-            os_inner_problem = OptimalScalingProblem.from_petab_amici(
+            ordinal_inner_problem = OrdinalProblem.from_petab_amici(
                 petab_problem, model, edatas, inner_problem_method
             )
-            os_inner_solver = OptimalScalingInnerSolver(
+            ordinal_inner_solver = OrdinalInnerSolver(
                 options=optimal_scaling_inner_options
             )
-            os_calculator = OptimalScalingAmiciCalculator(
-                os_inner_problem, os_inner_solver
+            ordinal_calculator = OrdinalCalculator(
+                ordinal_inner_problem, ordinal_inner_solver
             )
-            self.inner_calculators.append(os_calculator)
+            self.inner_calculators.append(ordinal_calculator)
 
-        if NONLINEAR_MONOTONE in self.data_types:
+        if SEMIQUANTITATIVE in self.data_types:
             spline_inner_options = {
                 key: value
                 for key, value in inner_options.items()
                 if key in SPLINE_APPROXIMATION_OPTIONS
             }
             spline_ratio = spline_inner_options.pop(SPLINE_RATIO, None)
-            spline_inner_problem = SplineInnerProblem.from_petab_amici(
+            semiquant_problem = SemiquantProblem.from_petab_amici(
                 petab_problem, model, edatas, spline_ratio
             )
-            spline_inner_solver = SplineInnerSolver(
+            semiquant_inner_solver = SemiquantInnerSolver(
                 options=spline_inner_options
             )
-            spline_calculator = SplineAmiciCalculator(
-                spline_inner_problem, spline_inner_solver
+            semiquant_calculator = SemiquantCalculator(
+                semiquant_problem, semiquant_inner_solver
             )
-            self.noise_dummy_values = (
-                spline_inner_problem.get_noise_dummy_values(scaled=True)
+            self.necessary_par_dummy_values.update(
+                semiquant_problem.get_noise_dummy_values(scaled=True)
             )
-            self.inner_calculators.append(spline_calculator)
-        # TODO relative data
+            self.inner_calculators.append(semiquant_calculator)
 
-        if set(self.data_types) - {ORDINAL, CENSORED, NONLINEAR_MONOTONE}:
-            unsupported_data_types = set(self.data_types) - {
+        if self.data_types - {
+            RELATIVE,
+            ORDINAL,
+            CENSORED,
+            SEMIQUANTITATIVE,
+        }:
+            unsupported_data_types = self.data_types - {
+                RELATIVE,
                 ORDINAL,
                 CENSORED,
-                NONLINEAR_MONOTONE,
+                SEMIQUANTITATIVE,
             }
             raise NotImplementedError(
                 f"Data types {unsupported_data_types} are not supported."
             )
 
-    def validate_options(self, inner_options: Dict):
+    def validate_options(self, inner_options: dict):
         """Validate the inner options.
 
         Parameters
         ----------
         inner_options:
             Options for the inner problems and solvers.
         """
         for key in inner_options:
             if (
-                key not in OPTIMAL_SCALING_OPTIONS
+                key not in ORDINAL_OPTIONS
                 and key not in SPLINE_APPROXIMATION_OPTIONS
             ):
                 raise ValueError(f"Unknown inner option {key}.")
 
     def _get_quantitative_data_mask(
         self,
-        petab_problem: 'petab.Problem',
-        observable_ids: List[str],
-        edatas: List['amici.ExpData'],
-    ) -> List[np.ndarray]:
+        edatas: list['amici.ExpData'],
+    ) -> list[np.ndarray]:
         # transform experimental data
         edatas = [
             amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
         ]
 
-        measurement_df = petab_problem.measurement_df
-
         quantitative_data_mask = [
-            np.zeros_like(edata, dtype=bool) for edata in edatas
+            np.ones_like(edata, dtype=bool) for edata in edatas
         ]
 
-        for observable_idx, observable_id in enumerate(observable_ids):
-            observable_df = measurement_df[
-                measurement_df[OBSERVABLE_ID] == observable_id
-            ]
-            # If the MEASUREMENT_TYPE column is filled with nans,
-            # then fill that axis of the mask with True
-            if observable_df[MEASUREMENT_TYPE].isna().all():
-                for condition_mask in quantitative_data_mask:
-                    condition_mask[:, observable_idx] = True
+        # iterate over inner problems
+        for calculator in self.inner_calculators:
+            inner_parameters = calculator.inner_problem.xs.values()
+            # Remove inner parameter masks from quantitative data mask
+            for inner_par in inner_parameters:
+                for cond_idx, condition_mask in enumerate(
+                    quantitative_data_mask
+                ):
+                    condition_mask[inner_par.ixs[cond_idx]] = False
 
         # If there is no quantitative data, return None
         if not all(mask.any() for mask in quantitative_data_mask):
             return None
 
         return quantitative_data_mask
 
-    def get_inner_parameter_ids(self) -> List[str]:
-        """Return the ids of the inner parameters."""
+    def get_inner_par_ids(self) -> list[str]:
+        """Return the ids of inner parameters of all inner problems."""
         return [
             parameter_id
             for inner_calculator in self.inner_calculators
-            for parameter_id in inner_calculator.get_inner_parameter_ids()
+            for parameter_id in inner_calculator.inner_problem.get_x_ids()
         ]
 
+    def get_interpretable_inner_par_ids(self) -> list[str]:
+        """Return the ids of interpretable inner parameters of all inner problems.
+
+        See :func:`InnerProblem.get_interpretable_x_ids`.
+        """
+        return [
+            parameter_id
+            for inner_calculator in self.inner_calculators
+            for parameter_id in inner_calculator.inner_problem.get_interpretable_x_ids()
+        ]
+
+    def get_interpretable_inner_par_bounds(
+        self,
+    ) -> tuple[np.ndarray, np.ndarray]:
+        """Return the bounds of interpretable inner parameters of all inner problems."""
+        lb = []
+        ub = []
+        for inner_calculator in self.inner_calculators:
+            (
+                lb_i,
+                ub_i,
+            ) = inner_calculator.inner_problem.get_interpretable_x_bounds()
+            lb.extend(lb_i)
+            ub.extend(ub_i)
+        return np.asarray(lb), np.asarray(ub)
+
     def __call__(
         self,
-        x_dct: Dict,
-        sensi_orders: Tuple[int],
+        x_dct: dict,
+        sensi_orders: tuple[int],
         mode: ModeType,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: List[amici.ExpData],
+        edatas: list[amici.ExpData],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
     ):
         """Perform the actual AMICI call.
 
@@ -271,43 +314,92 @@
             Mapping of optimization to simulation parameters.
         fim_for_hess:
             Whether to use the FIM (if available) instead of the Hessian (if
             requested).
         """
         import amici.parameter_mapping
 
-        if mode == MODE_RES:
+        if mode == MODE_RES and any(
+            data_type in self.data_types
+            for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
+        ):
             raise NotImplementedError(
-                f"Mode {mode} is not implemented for the :class:`pypesto.objective.amici.InnerCalculatorCollector`."
+                f"Mode {mode} is not implemented for ordinal, censored or semi-quantitative data. "
+                "However, it can be used if the only non-quantitative data type is relative data."
             )
 
-        if 2 in sensi_orders:
+        if 2 in sensi_orders and any(
+            data_type in self.data_types
+            for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
+        ):
             raise ValueError(
-                "Hessian and FIM are not implemented for the :class:`pypesto.objective.amici.InnerCalculatorCollector`."
+                "Hessian and FIM are not implemented for ordinal, censored or semi-quantitative data. "
+                "However, they can be used if the only non-quantitative data type is relative data."
             )
 
+        if (
+            amici_solver.getSensitivityMethod()
+            == amici.SensitivityMethod_adjoint
+            and any(
+                data_type in self.data_types
+                for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
+            )
+        ):
+            raise NotImplementedError(
+                "Adjoint sensitivity analysis is not implemented for ordinal, censored or semi-quantitative data. "
+                "However, it can be used if the only non-quantitative data type is relative data."
+            )
+
+        # if we're using adjoint sensitivity analysis or need second order
+        # sensitivities or are in residual mode, we can do so if the only
+        # non-quantitative data type is relative data. In this case, we
+        # use the relative calculator directly.
+        if (
+            amici_solver.getSensitivityMethod()
+            == amici.SensitivityMethod_adjoint
+            or 2 in sensi_orders
+            or mode == MODE_RES
+        ):
+            relative_calculator = self.inner_calculators[0]
+            ret = relative_calculator(
+                x_dct=x_dct,
+                sensi_orders=sensi_orders,
+                mode=mode,
+                amici_model=amici_model,
+                amici_solver=amici_solver,
+                edatas=edatas,
+                n_threads=n_threads,
+                x_ids=x_ids,
+                parameter_mapping=parameter_mapping,
+                fim_for_hess=fim_for_hess,
+            )
+            # only return inner parameters if the objective value improved
+            if ret[FVAL] > self.best_fval:
+                ret[INNER_PARAMETERS] = None
+            return filter_return_dict(ret)
+
         # get dimension of outer problem
         dim = len(x_ids)
 
         # initialize return values
         nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
             sensi_orders, mode, dim
         )
         all_inner_pars = {}
-        interpretable_inner_pars = {}
+        interpretable_inner_pars = []
 
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
         amici_solver.setSensitivityOrder(sensi_order)
 
         x_dct = copy.deepcopy(x_dct)
-        x_dct.update(self.noise_dummy_values)
+        x_dct.update(self.necessary_par_dummy_values)
         # fill in parameters
         amici.parameter_mapping.fill_in_parameters(
             edatas=edatas,
             problem_parameters=x_dct,
             scaled_parameters=True,
             parameter_mapping=parameter_mapping,
             amici_model=amici_model,
@@ -328,15 +420,15 @@
                 FVAL: nllh,
                 GRAD: snllh,
                 HESS: s2nllh,
                 RES: res,
                 SRES: sres,
                 RDATAS: rdatas,
                 X_INNER_OPT: all_inner_pars,
-                INNER_PARAMETERS: interpretable_inner_pars,
+                INNER_PARAMETERS: None,
             }
             ret[FVAL] = np.inf
             # if the gradient was requested,
             # we need to provide some value for it
             if 1 in sensi_orders:
                 ret[GRAD] = np.full(shape=len(x_ids), fill_value=np.nan)
             return filter_return_dict(ret)
@@ -360,15 +452,15 @@
                     'Cannot use least squares solver with'
                     'parameter dependent sigma! Support can be '
                     'enabled via '
                     'amici_model.setAddSigmaResiduals().'
                 )
             self._known_least_squares_safe = True  # don't check this again
 
-        # call inner calculators
+        # call inner calculators and collect results
         for calculator in self.inner_calculators:
             inner_result = calculator(
                 x_dct=x_dct,
                 sensi_orders=sensi_orders,
                 mode=mode,
                 amici_model=amici_model,
                 amici_solver=amici_solver,
@@ -376,37 +468,36 @@
                 n_threads=n_threads,
                 x_ids=x_ids,
                 parameter_mapping=parameter_mapping,
                 fim_for_hess=fim_for_hess,
                 rdatas=rdatas,
             )
             nllh += inner_result[FVAL]
-            if sensi_order > 0:
+            if 1 in sensi_orders:
                 snllh += inner_result[GRAD]
 
             all_inner_pars.update(inner_result[X_INNER_OPT])
             if INNER_PARAMETERS in inner_result:
-                interpretable_inner_pars.update(inner_result[INNER_PARAMETERS])
+                interpretable_inner_pars.extend(inner_result[INNER_PARAMETERS])
 
-        # add result for quantitative data
+        # add the quantitative data contribution
         if self.quantitative_data_mask is not None:
             quantitative_result = calculate_quantitative_result(
                 rdatas=rdatas,
                 sensi_orders=sensi_orders,
                 edatas=edatas,
                 mode=mode,
                 quantitative_data_mask=self.quantitative_data_mask,
                 dim=dim,
                 parameter_mapping=parameter_mapping,
                 par_opt_ids=x_ids,
                 par_sim_ids=amici_model.getParameterIds(),
-                par_edatas_indices=[edata.plist for edata in edatas],
             )
             nllh += quantitative_result[FVAL]
-            if sensi_order > 0:
+            if 1 in sensi_orders:
                 snllh += quantitative_result[GRAD]
 
         ret = {
             FVAL: nllh,
             GRAD: snllh,
             HESS: s2nllh,
             RES: res,
@@ -414,31 +505,34 @@
             RDATAS: rdatas,
         }
 
         # Add inner parameters to return dict
         # only if the objective value improved.
         if ret[FVAL] < self.best_fval:
             ret[X_INNER_OPT] = all_inner_pars
-            ret[INNER_PARAMETERS] = interpretable_inner_pars
+            ret[INNER_PARAMETERS] = (
+                interpretable_inner_pars
+                if len(interpretable_inner_pars) > 0
+                else None
+            )
             self.best_fval = ret[FVAL]
 
         return filter_return_dict(ret)
 
 
 def calculate_quantitative_result(
-    rdatas: List[amici.ReturnDataView],
-    edatas: List[amici.ExpData],
-    sensi_orders: Tuple[int],
+    rdatas: list[amici.ReturnDataView],
+    edatas: list[amici.ExpData],
+    sensi_orders: tuple[int],
     mode: ModeType,
-    quantitative_data_mask: List[np.ndarray],
+    quantitative_data_mask: list[np.ndarray],
     dim: int,
     parameter_mapping: ParameterMapping,
-    par_opt_ids: List[str],
-    par_sim_ids: List[str],
-    par_edatas_indices: List[List[int]],
+    par_opt_ids: list[str],
+    par_sim_ids: list[str],
 ):
     """Calculate the function values from rdatas and return as dict."""
     nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
         sensi_orders, mode, dim
     )
 
     # transform experimental data
@@ -464,21 +558,19 @@
         ]
         # iterate over simulation conditions
         for (
             rdata,
             edata,
             mask,
             condition_map_sim_var,
-            par_edata_indices,
         ) in zip(
             rdatas,
             edatas,
             quantitative_data_mask,
             parameter_map_sim_var,
-            par_edatas_indices,
         ):
             data_i = edata[mask]
             sim_i = rdata[AMICI_Y][mask]
             sigma_i = rdata[AMICI_SIGMAY][mask]
 
             n_parameters = rdata[AMICI_SY].shape[1]
 
@@ -487,41 +579,44 @@
                 [
                     rdata[AMICI_SY][:, parameter_index, :][mask]
                     for parameter_index in range(n_parameters)
                 ]
             )
             ssigma_i = np.asarray(
                 [
-                    rdata[AMICI_SSIGMAY][:, parameter_index][mask]
+                    rdata[AMICI_SSIGMAY][:, parameter_index, :][mask]
                     for parameter_index in range(n_parameters)
                 ]
             )
             # calculate the gradient for the condition
-            gradient_for_condition = ssigma_i @ (
-                (
-                    np.full(len(data_i), 1)
-                    - (data_i - sim_i) ** 2 / sigma_i**2
-                )
-                / sigma_i
-            ) - sensitivities_i @ ((data_i - sim_i) / sigma_i**2)
-
-            # add gradient to correct index of snllh
-            for par_sim, par_opt in condition_map_sim_var.items():
-                if not isinstance(par_opt, str):
-                    continue
-                par_opt_idx = par_opt_ids.index(par_opt)
-                par_sim_idx = par_sim_ids.index(par_sim)
-                par_edata_idx = (
-                    par_edata_indices.index(par_sim_idx)
-                    if par_sim_idx in par_edata_indices
-                    else None
-                )
-
-                if par_edata_idx is not None:
-                    snllh[par_opt_idx] += gradient_for_condition[par_edata_idx]
+            gradient_for_condition = np.nansum(
+                np.multiply(
+                    ssigma_i,
+                    (
+                        (
+                            np.full(len(data_i), 1)
+                            - (data_i - sim_i) ** 2 / sigma_i**2
+                        )
+                        / sigma_i
+                    ),
+                ),
+                axis=1,
+            ) + np.nansum(
+                np.multiply(
+                    sensitivities_i, ((sim_i - data_i) / sigma_i**2)
+                ),
+                axis=1,
+            )
+            add_sim_grad_to_opt_grad(
+                par_opt_ids=par_opt_ids,
+                par_sim_ids=par_sim_ids,
+                condition_map_sim_var=condition_map_sim_var,
+                sim_grad=gradient_for_condition,
+                opt_grad=snllh,
+            )
 
     ret = {
         FVAL: nllh,
         GRAD: snllh,
         HESS: s2nllh,
         RES: res,
         SRES: sres,
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/__init__.py` & `pypesto-0.4.2/pypesto/hierarchical/ordinal/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
-Optimal scaling
-===============
+Ordinal and censored data integration
+=====================================
 
 Contains the implementation of the optimal scaling approach, applied for integration
 of ordinal and censored data in ODE modeling. Each ordinal datapoint is defined as
 being part of a category, where the mutual ordering of the categories of the same observable
 is known. The category interval bounds are numerically optimized and quantitative surrogate
 measurements are calculated to represent the ordinal measurements. This constitutes
 the inner subproblem of the hierarchical optimization problem. For censored data, as the
 category interval bounds are known, the surrogate measurements are directly calculated.
 
-An example of parameter estimation with ordinal data can be found in pypesto/doc/examples/example_ordinal.ipynb.
-An example of parameter estimation with censored data can be found in pypesto/doc/examples/example_censored.ipynb.
+An example of parameter estimation with ordinal data
+can be found in pypesto/doc/examples/ordinal_data.ipynb.
+An example of parameter estimation with censored data
+can be found in pypesto/doc/examples/censored_data.ipynb.
 
 Details on the optimal scaling approach can be found in Shepard, 1962 (https://doi.org/10.1007/BF02289621).
 Details on the application of the gradient-based optimal scaling approach to mechanistic modeling
 with ordinal data can be found in Schmiester et al. 2020 (https://doi.org/10.1007/s00285-020-01522-w)
 and Schmiester et al. 2021 (https://doi.org/10.1093/bioinformatics/btab512).
 """
 
-from .calculator import OptimalScalingAmiciCalculator
-from .parameter import OptimalScalingParameter
-from .problem import OptimalScalingProblem
-from .solver import OptimalScalingInnerSolver
+from .calculator import OrdinalCalculator
+from .parameter import OrdinalParameter
+from .problem import OrdinalProblem
+from .solver import OrdinalInnerSolver
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/calculator.py` & `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Definition of an optimal scaling calculator class."""
 import copy
-from typing import Dict, List, Sequence, Tuple
+from typing import Sequence
 
 import numpy as np
 
 from ...C import (
     AMICI_SIGMAY,
     AMICI_SSIGMAY,
     AMICI_SY,
     AMICI_Y,
     FVAL,
     GRAD,
     HESS,
+    INNER_PARAMETERS,
     MODE_RES,
     RDATAS,
     RES,
     SRES,
     X_INNER_OPT,
 )
 from ...objective.amici.amici_calculator import (
@@ -23,82 +23,71 @@
     AmiciModel,
     AmiciSolver,
 )
 from ...objective.amici.amici_util import (
     filter_return_dict,
     init_return_values,
 )
-from .problem import OptimalScalingProblem
-from .solver import OptimalScalingInnerSolver
+from .problem import SemiquantProblem
+from .solver import SemiquantInnerSolver
 
 try:
     import amici
     from amici.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
-class OptimalScalingAmiciCalculator(AmiciCalculator):
+class SemiquantCalculator(AmiciCalculator):
     """A calculator is passed as `calculator` to the pypesto.AmiciObjective.
 
     The object is called by :func:`pypesto.AmiciObjective.call_unprocessed`
     to calculate the current objective function values and gradient.
     """
 
     def __init__(
         self,
-        inner_problem: OptimalScalingProblem,
-        inner_solver: OptimalScalingInnerSolver = None,
+        inner_problem: SemiquantProblem,
+        inner_solver: SemiquantInnerSolver = None,
     ):
         """Initialize the calculator from the given problem.
 
         Parameters
         ----------
         inner_problem:
             The optimal scaling inner problem.
         inner_solver:
             A solver to solve ``inner_problem``.
-            Defaults to ``OptimalScalingInnerSolver``.
+            Defaults to ``SplineInnerSolver``.
         """
         super().__init__()
         self.inner_problem = inner_problem
 
         if inner_solver is None:
-            inner_solver = OptimalScalingInnerSolver()
+            inner_solver = SemiquantInnerSolver()
         self.inner_solver = inner_solver
-        if (
-            self.inner_problem.method
-            is not self.inner_solver.options['method']
-        ):
-            raise ValueError(
-                f"The inner problem method {self.inner_problem.method} and the inner solver method {self.inner_solver.options['method']} have to coincide."
-            )
 
     def initialize(self):
         """Initialize."""
         self.inner_solver.initialize()
         self.inner_problem.initialize()
 
-    def get_inner_parameter_ids(self) -> List[str]:
-        """Get the ids of the inner parameters."""
-        return self.inner_problem.get_x_ids()
-
     def __call__(
         self,
-        x_dct: Dict,
-        sensi_orders: Tuple[int, ...],
+        x_dct: dict,
+        sensi_orders: tuple[int, ...],
         mode: str,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: List['amici.ExpData'],
+        edatas: list['amici.ExpData'],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
-        rdatas: List['amici.ReturnData'] = None,
+        rdatas: list['amici.ReturnData'] = None,
     ):
         """Perform the actual AMICI call.
 
         Parameters
         ----------
         x_dct:
             Parameters for which to compute function value and derivatives.
@@ -122,26 +111,27 @@
             Whether to use the FIM (if available) instead of the Hessian (if
             requested).
         rdatas:
             AMICI simulation return data. In case the calculator is part of
             the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
             it will already simulate the model and pass the results here.
 
+
         Returns
         -------
         inner_result:
             A dict containing the calculation results: FVAL, GRAD, RDATAS and X_INNER_OPT.
         """
         if mode == MODE_RES:
             raise ValueError(
-                "Optimal scaling method cannot be called with residual mode."
+                "Spline approximation cannot be called with residual mode."
             )
         if 2 in sensi_orders:
             raise ValueError(
-                "Hessian and FIM are not implemented for the optimal scaling calculator."
+                "Hessian and FIM are not implemented for the spline calculator."
             )
 
         # get dimension of outer problem
         dim = len(x_ids)
 
         # initialize return values
         nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
@@ -149,18 +139,22 @@
         )
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
         # If AMICI ReturnData is not provided, we need to simulate the model
+
         if rdatas is None:
             amici_solver.setSensitivityOrder(sensi_order)
 
             x_dct = copy.deepcopy(x_dct)
+            x_dct.update(
+                self.inner_problem.get_noise_dummy_values(scaled=True)
+            )
 
             # fill in parameters
             amici.parameter_mapping.fill_in_parameters(
                 edatas=edatas,
                 problem_parameters=x_dct,
                 scaled_parameters=True,
                 parameter_mapping=parameter_mapping,
@@ -184,46 +178,49 @@
             X_INNER_OPT: self.inner_problem.get_inner_parameter_dictionary(),
         }
 
         # if any amici simulation failed, it's unlikely we can compute
         # meaningful inner parameters, so we better just fail early.
         if any(rdata.status != amici.AMICI_SUCCESS for rdata in rdatas):
             inner_result[FVAL] = np.inf
-            # if the gradient was requested,
-            # we need to provide some value for it
             if 1 in sensi_orders:
-                inner_result[GRAD] = np.full(
-                    shape=len(x_ids), fill_value=np.nan
-                )
+                inner_result[GRAD] = np.full(shape=dim, fill_value=np.nan)
             return filter_return_dict(inner_result)
 
         sim = [rdata[AMICI_Y] for rdata in rdatas]
         sigma = [rdata[AMICI_SIGMAY] for rdata in rdatas]
 
+        # Clip negative simulation values to zero, to avoid numerical issues.
+        for i in range(len(sim)):
+            sim[i] = sim[i].clip(min=0)
+
         # compute optimal inner parameters
         x_inner_opt = self.inner_solver.solve(self.inner_problem, sim, sigma)
         inner_result[FVAL] = self.inner_solver.calculate_obj_function(
             x_inner_opt
         )
         inner_result[
             X_INNER_OPT
         ] = self.inner_problem.get_inner_parameter_dictionary()
 
-        # calculate analytical gradients if requested
+        inner_result[
+            INNER_PARAMETERS
+        ] = self.inner_problem.get_inner_noise_parameters()
+
+        # Calculate analytical gradients if requested
         if sensi_order > 0:
-            # print([opt['fun'] for opt in x_inner_opt])
             sy = [rdata[AMICI_SY] for rdata in rdatas]
             ssigma = [rdata[AMICI_SSIGMAY] for rdata in rdatas]
             inner_result[GRAD] = self.inner_solver.calculate_gradients(
                 problem=self.inner_problem,
                 x_inner_opt=x_inner_opt,
                 sim=sim,
+                amici_sigma=sigma,
                 sy=sy,
-                sigma=sigma,
-                ssigma=ssigma,
+                amici_ssigma=ssigma,
                 parameter_mapping=parameter_mapping,
                 par_opt_ids=x_ids,
                 par_sim_ids=amici_model.getParameterIds(),
                 par_edatas_indices=[edata.plist for edata in edatas],
                 snllh=snllh,
             )
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/parameter.py` & `pypesto-0.4.2/pypesto/hierarchical/ordinal/parameter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Definition of an optimal scaling inner parameter class."""
+
 import logging
 from typing import Literal
 
 from ...C import (
     INTERVAL_CENSORED,
     LEFT_CENSORED,
     RIGHT_CENSORED,
     InnerParameterType,
 )
-from ..parameter import InnerParameter
+from ..base_parameter import InnerParameter
 
 logger = logging.getLogger(__name__)
 
 
-class OptimalScalingParameter(InnerParameter):
-    """Inner parameter of the optimal scaling hierarchical optimization problem.
+class OrdinalParameter(InnerParameter):
+    """Inner parameter of the optimal scaling inner optimization problem for ordinal data.
 
     Attributes
     ----------
     dummy_value:
         Value to be used when the optimal parameter is not yet known
         (in particular to simulate unscaled observables).
     inner_parameter_id:
@@ -65,17 +66,17 @@
         """Construct.
 
         Parameters
         ----------
         See class attributes.
         """
         super().__init__(*args, **kwargs)
-        if self.inner_parameter_type != InnerParameterType.OPTIMAL_SCALING:
+        if self.inner_parameter_type != InnerParameterType.ORDINAL:
             raise ValueError(
-                f"For the OptimalScalingParameter class, the parameter type has to be {InnerParameterType.OPTIMAL_SCALING}."
+                f"For the OptimalScalingParameter class, the parameter type has to be {InnerParameterType.ORDINAL}."
             )
 
         if group is None:
             raise ValueError("No Parameter group provided.")
         if category is None:
             raise ValueError("No Category provided.")
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/problem.py` & `pypesto-0.4.2/pypesto/hierarchical/ordinal/problem.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Definition of an optimal scaling parameter class."""
-from typing import Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 
 from ...C import (
     C_MATRIX,
     CAT_LB,
@@ -31,65 +30,70 @@
     SURROGATE_DATA,
     TIME,
     UB_INDICES,
     W_DOT_MATRIX,
     W_MATRIX,
     InnerParameterType,
 )
-from ..problem import (
-    InnerProblem,
+from ..base_problem import (
+    AmiciInnerProblem,
     _get_timepoints_with_replicates,
     ix_matrices_from_arrays,
 )
-from .parameter import OptimalScalingParameter
+from .parameter import OrdinalParameter
 
 try:
     import amici
     import petab
     from petab.C import OBSERVABLE_ID, PARAMETER_SEPARATOR
 except ImportError:
     pass
 
 
-class OptimalScalingProblem(InnerProblem):
-    """Inner optimization problem for optimal scaling.
+class OrdinalProblem(AmiciInnerProblem):
+    r"""Inner optimization problem for ordinal or censored data.
+
+    The ordinal inner problem contains the following parameters: surrogate data,
+    lower bounds, and upper bounds. All parameters are optimized to minimize the
+    distance between the surrogate data and the simulated data while satisfying
+    the ordering constraints of the problem. Depending on the method, the problem
+    is re-formulated to reduce the number of parameters to estimate.
 
     Attributes
     ----------
     xs:
         Mapping of (inner) parameter ID to ``InnerParameters``.
     data:
-        Measurement data. One matrix (`num_timepoints` x `num_observables`)
+        Measurement data. One matrix (``num_timepoints`` x ``num_observables``)
         per simulation condition. Missing observations as NaN.
+    edatas:
+        AMICI ``ExpData``\s for each simulation condition.
     groups:
         A dictionary of the groups of the subproblem.
     method:
-        A string representing the method of the Optimal Scaling approach, either 'reduced' or 'standard'.
+        A string representing the method of the Optimal Scaling approach, either ``reduced`` or ``standard``.
     """
 
     def __init__(
         self,
-        xs: List[OptimalScalingParameter],
-        data: List[np.ndarray],
         method: str,
+        **kwargs,
     ):
         """Construct."""
-        super().__init__(xs, data)
+        super().__init__(**kwargs)
         self.groups = {}
         self.method = method
 
         self._initialize_groups()
 
     def _initialize_groups(self) -> None:
         """Initialize the groups of the subproblem."""
         self.groups = {}
 
-        for group in self.get_groups_for_xs(
-            InnerParameterType.OPTIMAL_SCALING
-        ):
+        for group in self.get_groups_for_xs(InnerParameterType.ORDINAL):
             self.groups[group] = {}
             xs = self.get_xs_for_group(group)
             self.groups[group][NUM_CATEGORIES] = len({x.category for x in xs})
             self.groups[group][NUM_DATAPOINTS] = sum(
                 [
                     sum([np.sum(ixs) for ixs in x.ixs])
                     for x in self.get_cat_ub_parameters_for_group(group)
@@ -165,67 +169,70 @@
                 self.groups[group][NUM_DATAPOINTS]
             )
 
     @staticmethod
     def from_petab_amici(
         petab_problem: petab.Problem,
         amici_model: 'amici.Model',
-        edatas: List['amici.ExpData'],
+        edatas: list['amici.ExpData'],
         method: str = None,
-    ) -> 'OptimalScalingProblem':
+    ) -> 'OrdinalProblem':
         """Construct the inner problem from the `petab_problem`."""
         if not method:
             method = REDUCED
 
         return optimal_scaling_inner_problem_from_petab_problem(
             petab_problem, amici_model, edatas, method
         )
 
-    def get_groups_for_xs(self, inner_parameter_type: str) -> List[int]:
+    def get_interpretable_x_ids(self) -> list[str]:
+        """Get IDs of interpretable inner parameters.
+
+        There are no interpretable inner parameters for the ordinal problem.
+        """
+        return []
+
+    def get_groups_for_xs(self, inner_parameter_type: str) -> list[int]:
         """Get unique list of ``OptimalScalingParameter.group`` values."""
         groups = [x.group for x in self.get_xs_for_type(inner_parameter_type)]
         return list(set(groups))
 
-    def get_xs_for_group(self, group: int) -> List[OptimalScalingParameter]:
+    def get_xs_for_group(self, group: int) -> list[OrdinalParameter]:
         r"""Get ``OptimalScalingParameter``\s that belong to the given group."""
         return [x for x in self.xs.values() if x.group == group]
 
-    def get_free_xs_for_group(
-        self, group: int
-    ) -> List[OptimalScalingParameter]:
+    def get_free_xs_for_group(self, group: int) -> list[OrdinalParameter]:
         r"""Get ``OptimalScalingParameter``\s that are free and belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group and x.estimate is True
         ]
 
-    def get_fixed_xs_for_group(
-        self, group: int
-    ) -> List[OptimalScalingParameter]:
+    def get_fixed_xs_for_group(self, group: int) -> list[OrdinalParameter]:
         r"""Get ``OptimalScalingParameter``\s that are fixed and belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group and x.estimate is False
         ]
 
     def get_cat_ub_parameters_for_group(
         self, group: int
-    ) -> List[OptimalScalingParameter]:
+    ) -> list[OrdinalParameter]:
         r"""Get ``OptimalScalingParameter``\s that are category upper boundaries and belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group and x.inner_parameter_id[:6] == CAT_UB
         ]
 
     def get_cat_lb_parameters_for_group(
         self, group: int
-    ) -> List[OptimalScalingParameter]:
+    ) -> list[OrdinalParameter]:
         r"""Get ``OptimalScalingParameter``\s that are category lower boundaries and belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group and x.inner_parameter_id[:6] == CAT_LB
         ]
 
@@ -364,15 +371,15 @@
             )
         )
         return w_dot
 
     def get_d(
         self,
         group,
-        xs: List[OptimalScalingParameter],
+        xs: list[OrdinalParameter],
         y_sim_all: np.ndarray,
         eps: float,
     ) -> np.ndarray:
         """Return vector of minimal gaps and ranges."""
         max_simulation = np.nanmax(y_sim_all)
 
         interval_range = max_simulation / (2 * len(xs) + 1)
@@ -391,15 +398,15 @@
             + self.groups[group][NUM_CATEGORIES] :
         ] = interval_range
         return d
 
     def get_dd_dtheta(
         self,
         group: int,
-        xs: List[OptimalScalingParameter],
+        xs: list[OrdinalParameter],
         y_sim_all: np.ndarray,
         sy_all: np.ndarray,
     ) -> np.ndarray:
         """Return the derivative of vector of minimal gaps and ranges with respect to an outer parameter."""
         max_sim_idx = np.argmax(y_sim_all)
         max_sy = sy_all[max_sim_idx]
         dd_dtheta = np.zeros(self.groups[group][NUM_CONSTR_FULL])
@@ -417,16 +424,16 @@
             2 * self.groups[group][NUM_DATAPOINTS]
             + self.groups[group][NUM_CATEGORIES] :
         ] = dinterval_range_dtheta
 
         return dd_dtheta
 
     def get_censored_group_quantitative_ixs(
-        self, xs: List[OptimalScalingParameter]
-    ) -> List[np.ndarray]:
+        self, xs: list[OrdinalParameter]
+    ) -> list[np.ndarray]:
         r"""Return a list of boolean masks indicating which data points are quantitative.
 
         For a given group with censored data, return a list of boolean masks indicating
         which data points are not censored, and therefore quantitative.
 
         Parameters
         ----------
@@ -454,75 +461,72 @@
         # Set to False for all censored datapoints.
         for x in xs:
             for ixs_i, quantitative_ixs_i in zip(x.ixs, quantitative_ixs):
                 quantitative_ixs_i[ixs_i] = False
 
         return quantitative_ixs
 
-    def get_inner_parameter_dictionary(self) -> Dict:
+    def get_inner_parameter_dictionary(self) -> dict:
         """Return a dictionary with inner parameter ids and their values."""
         inner_par_dict = {}
         for x_id, x in self.xs.items():
             inner_par_dict[x_id] = x.value
         return inner_par_dict
 
 
 def optimal_scaling_inner_problem_from_petab_problem(
     petab_problem: petab.Problem,
     amici_model: 'amici.Model',
-    edatas: List['amici.ExpData'],
+    edatas: list['amici.ExpData'],
     method: str,
 ):
     """Construct the inner problem from the `petab_problem`."""
     # inner parameters
     inner_parameters = optimal_scaling_inner_parameters_from_measurement_df(
         petab_problem.measurement_df, method, amici_model
     )
 
     # used indices for all measurement specific parameters
     ixs = optimal_scaling_ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, inner_parameters
     )
 
     # transform experimental data
-    edatas = [
-        amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
-    ]
+    data = [amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas]
 
     # matrixify
-    ix_matrices = ix_matrices_from_arrays(ixs, edatas)
+    ix_matrices = ix_matrices_from_arrays(ixs, data)
 
     # assign matrices
     for par in inner_parameters:
         par.ixs = ix_matrices[par.inner_parameter_id]
 
-    return OptimalScalingProblem(
-        inner_parameters,
-        edatas,
-        method,
+    return OrdinalProblem(
+        xs=inner_parameters,
+        data=data,
+        edatas=edatas,
+        method=method,
     )
 
 
 def optimal_scaling_inner_parameters_from_measurement_df(
     df: pd.DataFrame,
     method: str,
     amici_model: 'amici.Model',
-) -> List[OptimalScalingParameter]:
+) -> list[OrdinalParameter]:
     """Create list of inner free parameters from PEtab measurement table dependent on the method provided."""
     df = df.reset_index()
 
     observable_ids = amici_model.getObservableIds()
 
     estimate = get_estimate_for_method(method)
     par_types = [CAT_LB, CAT_UB]
 
     inner_parameters = []
-    lb, ub = INNER_PARAMETER_BOUNDS[
-        InnerParameterType.OPTIMAL_SCALING
-    ].values()
+    lb, ub = INNER_PARAMETER_BOUNDS[InnerParameterType.ORDINAL].values()
 
     for observable_idx, observable_id in enumerate(observable_ids):
         group = observable_idx + 1
 
         observable_df = df[df[OBSERVABLE_ID] == observable_id]
 
         if all(observable_df[MEASUREMENT_TYPE] == ORDINAL):
@@ -533,17 +537,17 @@
 
                     # Create only one set of bound parameters per category of a group.
                     if par_id not in [
                         inner_par.inner_parameter_id
                         for inner_par in inner_parameters
                     ]:
                         inner_parameters.append(
-                            OptimalScalingParameter(
+                            OrdinalParameter(
                                 inner_parameter_id=par_id,
-                                inner_parameter_type=InnerParameterType.OPTIMAL_SCALING,
+                                inner_parameter_type=InnerParameterType.ORDINAL,
                                 scale=LIN,
                                 lb=lb,
                                 ub=ub,
                                 observable_id=observable_id,
                                 category=int(row[MEASUREMENT_CATEGORY]),
                                 group=group,
                                 estimate=par_estimate,
@@ -569,17 +573,17 @@
                     par_id = f'{par_type}_{observable_id}_{row[MEASUREMENT_TYPE]}_{category}'
                     # Create only one set of bound parameters per category of a group.
                     if par_id not in [
                         inner_par.inner_parameter_id
                         for inner_par in inner_parameters
                     ]:
                         inner_parameters.append(
-                            OptimalScalingParameter(
+                            OrdinalParameter(
                                 inner_parameter_id=par_id,
-                                inner_parameter_type=InnerParameterType.OPTIMAL_SCALING,
+                                inner_parameter_type=InnerParameterType.ORDINAL,
                                 scale=LIN,
                                 lb=lb,
                                 ub=ub,
                                 observable_id=observable_id,
                                 category=category,
                                 group=group,
                                 estimate=False,
@@ -591,30 +595,30 @@
                         )
 
     inner_parameters.sort(key=lambda x: (x.group, x.category))
 
     return inner_parameters
 
 
-def get_estimate_for_method(method: str) -> Tuple[bool, bool]:
+def get_estimate_for_method(method: str) -> tuple[bool, bool]:
     """Return which inner parameters to estimate dependent on the method provided."""
     estimate_ub = True
     estimate_lb = False
 
     if method == STANDARD:
         estimate_lb = True
 
     return estimate_lb, estimate_ub
 
 
 def optimal_scaling_ixs_for_measurement_specific_parameters(
     petab_problem: 'petab.Problem',
     amici_model: 'amici.Model',
-    inner_parameters: List[OptimalScalingParameter],
-) -> Dict[str, List[Tuple[int, int, int]]]:
+    inner_parameters: list[OrdinalParameter],
+) -> dict[str, list[tuple[int, int, int]]]:
     """Create mapping of parameters to measurements.
 
     Returns
     -------
     A dictionary mapping parameter ID to a list of
     `(condition index, time index, observable index)` tuples in which this
     output parameter is used. For each condition, the time index refers to
@@ -693,17 +697,17 @@
                         ixs_for_par.setdefault(override, []).append(
                             (condition_ix, time_w_reps_ix, observable_ix)
                         )
     return ixs_for_par
 
 
 def get_inner_par_ids_for_measurement(
-    measurement: Dict,
-    inner_parameters: List[OptimalScalingParameter],
-    unique_censoring_bounds_per_observable: Dict[str, List[float]],
+    measurement: dict,
+    inner_parameters: list[OrdinalParameter],
+    unique_censoring_bounds_per_observable: dict[str, list[float]],
 ):
     """Return inner parameter ids of parameters which are related to the measurement."""
     if measurement[MEASUREMENT_TYPE] == ORDINAL:
         return [
             inner_par.inner_parameter_id
             for inner_par in inner_parameters
             if inner_par.category == measurement[MEASUREMENT_CATEGORY]
@@ -725,15 +729,15 @@
             for inner_par in inner_parameters
             if inner_par.observable_id == measurement[OBSERVABLE_ID]
             and inner_par.category == measurement_category
         ]
 
 
 def _add_value_to_censored_bound_parameter(
-    inner_parameter: OptimalScalingParameter,
+    inner_parameter: OrdinalParameter,
     row: pd.Series,
     par_type: str,
 ) -> None:
     if row[MEASUREMENT_TYPE] == LEFT_CENSORED and par_type == CAT_LB:
         inner_parameter.value = 0.0
     elif row[MEASUREMENT_TYPE] == LEFT_CENSORED and par_type == CAT_UB:
         inner_parameter.value = float(row[CENSORING_BOUNDS])
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/optimal_scaling/solver.py` & `pypesto-0.4.2/pypesto/hierarchical/ordinal/solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Definition of an optimal scaling solver class."""
+
 import warnings
-from typing import Dict, List, Tuple
 
 import numpy as np
 
 from ...C import (
     C_MATRIX,
     CENSORED,
     INTERVAL_CONSTRAINTS,
@@ -28,25 +28,25 @@
     STANDARD,
     SURROGATE_DATA,
     UB_INDICES,
     W_DOT_MATRIX,
     W_MATRIX,
     InnerParameterType,
 )
-from ..solver import InnerSolver
-from .parameter import OptimalScalingParameter
-from .problem import OptimalScalingProblem
+from ..base_solver import InnerSolver
+from .parameter import OrdinalParameter
+from .problem import OrdinalProblem
 
 try:
     from amici.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
-class OptimalScalingInnerSolver(InnerSolver):
+class OrdinalInnerSolver(InnerSolver):
     """Solve the inner subproblem of the optimal scaling approach for ordinal data.
 
     Options
     -------
     method:
         The method to use for the inner optimization problem.
         Can be 'standard' or 'reduced'. The latter is more efficient.
@@ -55,15 +55,15 @@
     intervalConstraints:
         The type of interval constraints to use.
         Can be 'max' or 'maxmin'.
     minGap:
         The minimum gap between two consecutive categories.
     """
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         """Construct."""
         self.options = {
             **self.get_default_options(),
             **(options or {}),
         }
         self.validate_options()
 
@@ -104,17 +104,17 @@
             if key not in self.get_default_options():
                 raise ValueError(
                     f"Unknown OptimalScalingInnerSolver option {key}."
                 )
 
     def solve(
         self,
-        problem: OptimalScalingProblem,
-        sim: List[np.ndarray],
-        sigma: List[np.ndarray],
+        problem: OrdinalProblem,
+        sim: list[np.ndarray],
+        sigma: list[np.ndarray],
     ) -> list:
         """Get results for every group (inner optimization problem).
 
         Parameters
         ----------
         problem:
             Optimal scaling inner problem.
@@ -124,17 +124,15 @@
             Standard deviation of the noise.
 
         Returns
         -------
         List of optimization results of the inner subproblem.
         """
         optimal_surrogates = []
-        for group in problem.get_groups_for_xs(
-            InnerParameterType.OPTIMAL_SCALING
-        ):
+        for group in problem.get_groups_for_xs(InnerParameterType.ORDINAL):
             category_upper_bounds = problem.get_cat_ub_parameters_for_group(
                 group
             )
             category_lower_bounds = problem.get_cat_lb_parameters_for_group(
                 group
             )
             if problem.groups[group][MEASUREMENT_TYPE] == ORDINAL:
@@ -195,25 +193,25 @@
                     for idx in range(len(x_inner_opt))
                 ]
             )
         return obj
 
     def calculate_gradients(
         self,
-        problem: OptimalScalingProblem,
-        x_inner_opt: List[Dict],
-        sim: List[np.ndarray],
-        sy: List[np.ndarray],
-        sigma: List[np.ndarray],
-        ssigma: List[np.ndarray],
+        problem: OrdinalProblem,
+        x_inner_opt: list[dict],
+        sim: list[np.ndarray],
+        sy: list[np.ndarray],
+        sigma: list[np.ndarray],
+        ssigma: list[np.ndarray],
         parameter_mapping: ParameterMapping,
-        par_opt_ids: List,
-        par_sim_ids: List,
-        par_edatas_indices: List,
-        snllh: Dict,
+        par_opt_ids: list,
+        par_sim_ids: list,
+        par_edatas_indices: list,
+        snllh: np.ndarray,
     ):
         """Calculate gradients of the inner objective function.
 
         Calculates gradients of the objective function with respect to outer
         (dynamical) parameters.
 
         Parameters
@@ -236,61 +234,54 @@
             Ids of outer otimization parameters.
         par_sim_ids:
             Ids of outer simulation parameters, includes fixed parameters.
         par_edata_indices:
             Indices of parameters from `amici_model.getParameterIds()` that are needed for
             sensitivity calculation. Comes from `edata.plist` for each condition.
         snllh:
-            Empty dictionary with optimization parameters as keys.
+            A zero-initialized vector of the same length as ``par_opt_ids`` to store the
+            gradients in. Will be modified in-place.
 
         Returns
         -------
-        Filled in snllh dictionary with objective function gradients.
+        The gradients with respect to the outer parameters.
         """
         already_calculated = set()
 
         for condition_map_sim_var in [
             cond_par_map.map_sim_var for cond_par_map in parameter_mapping
         ]:
             # Iterate over outer optimization parameters.
             for par_sim, par_opt in condition_map_sim_var.items():
                 if (
                     not isinstance(par_opt, str)
                     or par_opt in already_calculated
                 ):
                     continue
-                # Current fix for scaling/offset parameters in models.
-                elif par_sim.startswith('observableParameter'):
-                    continue
-                # For noise parameters optimized hierarchically, we
-                # do not calculate the gradient.
-                elif (
-                    par_sim.startswith('noiseParameter')
-                    and par_opt not in par_opt_ids
-                ):
+                elif par_opt not in par_opt_ids:
                     continue
                 else:
                     already_calculated.add(par_opt)
 
                 par_opt_idx = par_opt_ids.index(par_opt)
                 par_sim_idx = par_sim_ids.index(par_sim)
                 par_edata_idx = [
-                    par_edata_indices.index(par_sim_idx)
-                    if par_sim_idx in par_edata_indices
-                    else None
+                    (
+                        par_edata_indices.index(par_sim_idx)
+                        if par_sim_idx in par_edata_indices
+                        else None
+                    )
                     for par_edata_indices in par_edatas_indices
                 ]
 
                 grad = 0.0
 
                 # Iterate over inner parameter groups.
                 for idx, group in enumerate(
-                    problem.get_groups_for_xs(
-                        InnerParameterType.OPTIMAL_SCALING
-                    )
+                    problem.get_groups_for_xs(InnerParameterType.ORDINAL)
                 ):
                     if problem.groups[group][MEASUREMENT_TYPE] == CENSORED:
                         category_upper_bounds = (
                             problem.get_cat_ub_parameters_for_group(group)
                         )
                         category_lower_bounds = (
                             problem.get_cat_lb_parameters_for_group(group)
@@ -374,28 +365,28 @@
                         else:
                             grad += df_dtheta
 
                 snllh[par_opt_idx] = grad
         return snllh
 
     @staticmethod
-    def get_default_options() -> Dict:
+    def get_default_options() -> dict:
         """Return default options for solving the inner problem."""
         options = {
             METHOD: REDUCED,
             REPARAMETERIZED: True,
             INTERVAL_CONSTRAINTS: MAX,
             MIN_GAP: 1e-16,
         }
         return options
 
 
 def calculate_dxi_dtheta(
     group: int,
-    problem: OptimalScalingProblem,
+    problem: OrdinalProblem,
     xi: np.ndarray,
     mu: np.ndarray,
     dy_dtheta: np.ndarray,
     residual: np.ndarray,
     d: np.ndarray,
     dd_dtheta: np.ndarray,
 ):
@@ -444,24 +435,22 @@
         ]
     )
 
     dxi_dtheta = linalg.spsolve(A_sp, b)
     return dxi_dtheta[: problem.groups[group][NUM_INNER_PARAMS]]
 
 
-def get_dy_dtheta(
-    group: int, problem: OptimalScalingProblem, sy_all: np.ndarray
-):
+def get_dy_dtheta(group: int, problem: OrdinalProblem, sy_all: np.ndarray):
     """Restructure sensitivities into a numpy matrix of right dimension."""
     return np.block(
         [sy_all, np.zeros(2 * problem.groups[group][NUM_CATEGORIES])]
     )
 
 
-def get_mu(group: int, problem: OptimalScalingProblem, residual: np.ndarray):
+def get_mu(group: int, problem: OrdinalProblem, residual: np.ndarray):
     """Calculate Lagrange multipliers of the inner optimization problem.
 
     Parameters
     ----------
     group:
         Inner parameter group.
     problem:
@@ -477,18 +466,18 @@
         lapack_driver='gelsy',
     )
     return mu[0]
 
 
 def get_xi(
     group: int,
-    problem: OptimalScalingProblem,
-    x_inner_opt: Dict,
-    sim: List[np.ndarray],
-    options: Dict,
+    problem: OrdinalProblem,
+    x_inner_opt: dict,
+    sim: list[np.ndarray],
+    options: dict,
 ):
     """Extract and calculate category bounds and surrogate data.
 
     Parameters
     ----------
     group:
         Inner parameter group.
@@ -513,18 +502,18 @@
     xi[: problem.groups[group][NUM_DATAPOINTS]] = surrogate_all.flatten()
     xi[problem.groups[group][LB_INDICES]] = x_lower
     xi[problem.groups[group][UB_INDICES]] = x_upper
     return xi
 
 
 def optimize_surrogate_data_per_group(
-    category_upper_bounds: List[OptimalScalingParameter],
-    category_lower_bounds: List[OptimalScalingParameter],
-    sim: List[np.ndarray],
-    options: Dict,
+    category_upper_bounds: list[OrdinalParameter],
+    category_lower_bounds: list[OrdinalParameter],
+    sim: list[np.ndarray],
+    options: dict,
 ):
     """Run optimization for inner subproblem.
 
     Parameters
     ----------
     category_upper_bounds:
         Upper bound parameters of categories for this group.
@@ -581,21 +570,21 @@
         inner_options['x0'] = np.zeros(len(inner_options['x0']))
         results = minimize(obj_surr, jac=grad_surr, **inner_options)
 
     return results
 
 
 def get_inner_optimization_options(
-    category_upper_bounds: List[OptimalScalingParameter],
-    category_lower_bounds: List[OptimalScalingParameter],
-    sim: List[np.ndarray],
+    category_upper_bounds: list[OrdinalParameter],
+    category_lower_bounds: list[OrdinalParameter],
+    sim: list[np.ndarray],
     interval_range: float,
     interval_gap: float,
-    options: Dict,
-) -> Dict:
+    options: dict,
+) -> dict:
     """Return default options for scipy optimizer.
 
     Returns inner subproblem optimization options including startpoint
     and optimization bounds or constraints, dependent on solver method.
 
     Parameters
     ----------
@@ -678,29 +667,29 @@
             'options': {'maxiter': 2000, 'ftol': 1e-10, 'disp': None},
             'constraints': constraints,
         }
     return inner_options
 
 
 def get_min_max(
-    inner_parameters: List[OptimalScalingParameter], sim: List[np.ndarray]
-) -> Tuple[float, float]:
+    inner_parameters: list[OrdinalParameter], sim: list[np.ndarray]
+) -> tuple[float, float]:
     """Return minimal and maximal simulation value."""
     sim_all = get_sim_all(inner_parameters, sim)
 
     min_all = np.min(sim_all)
     max_all = np.max(sim_all)
 
     return min_all, max_all
 
 
 def get_sy_all(
-    inner_parameters: List[OptimalScalingParameter],
-    sy: List[np.ndarray],
-    par_edata_idx: List,
+    inner_parameters: list[OrdinalParameter],
+    sy: list[np.ndarray],
+    par_edata_idx: list,
 ):
     """Return model sensitivities for inner parameters and outer parameter index."""
     sy_all = []
     for inner_parameter in inner_parameters:
         for sy_i, mask_i, edata_idx in zip(
             sy, inner_parameter.ixs, par_edata_idx
         ):
@@ -709,32 +698,32 @@
             else:
                 sim_sy = np.full(sy_i[:, 0, :][mask_i].shape, 0)
             for sim_sy_i in sim_sy:
                 sy_all.append(sim_sy_i)
     return np.array(sy_all)
 
 
-def get_sim_all(inner_parameters, sim: List[np.ndarray]) -> list:
+def get_sim_all(inner_parameters, sim: list[np.ndarray]) -> list:
     """Return model simulations for inner parameters."""
     sim_all = []
     for inner_parameter in inner_parameters:
         for sim_i, mask_i in zip(sim, inner_parameter.ixs):
             sim_x = sim_i[mask_i]
             for sim_x_i in sim_x:
                 sim_all.append(sim_x_i)
     return sim_all
 
 
 def get_surrogate_all(
-    inner_parameters: List[OptimalScalingParameter],
-    optimal_scaling_bounds: List,
-    sim: List[np.ndarray],
+    inner_parameters: list[OrdinalParameter],
+    optimal_scaling_bounds: list,
+    sim: list[np.ndarray],
     interval_range: float,
     interval_gap: float,
-    options: Dict,
+    options: dict,
 ):
     """Return surrogate data, lower and upper category bounds."""
     if options[REPARAMETERIZED]:
         optimal_scaling_bounds = undo_inner_parameter_reparameterization(
             optimal_scaling_bounds,
             inner_parameters,
             interval_gap,
@@ -765,30 +754,30 @@
         np.array(surrogate_all),
         np.array(x_lower_all),
         np.array(x_upper_all),
     )
 
 
 def get_weight_for_surrogate(
-    inner_parameters: List[OptimalScalingParameter], sim: List[np.ndarray]
+    inner_parameters: list[OrdinalParameter], sim: list[np.ndarray]
 ) -> float:
     """Calculate weights for objective function."""
     sim_x_all = get_sim_all(inner_parameters, sim)
     eps = 1e-8
 
     w = np.sum(np.abs(sim_x_all)) + eps
 
     return w
 
 
 def compute_interval_constraints(
-    inner_parameters: List[OptimalScalingParameter],
-    sim: List[np.ndarray],
-    options: Dict,
-) -> Tuple[float, float]:
+    inner_parameters: list[OrdinalParameter],
+    sim: list[np.ndarray],
+    options: dict,
+) -> tuple[float, float]:
     """Compute minimal interval range and gap."""
     # compute constraints on interval size and interval gap size
     # similar to Pargett et al. (2014)
     if MIN_GAP not in options:
         eps = 1e-16
     else:
         eps = options[MIN_GAP]
@@ -812,15 +801,15 @@
             f"Please use {MAX} or {MAXMIN}."
         )
     return interval_range, interval_gap + eps
 
 
 def reparameterize_inner_parameters(
     original_inner_parameter_values: np.ndarray,
-    inner_parameters: List[OptimalScalingParameter],
+    inner_parameters: list[OrdinalParameter],
     interval_gap: float,
     interval_range: float,
 ) -> np.ndarray:
     """Transform original inner parameters to reparameterized inner parameters."""
     reparameterized_inner_parameter_values = np.full(
         shape=(np.shape(original_inner_parameter_values)), fill_value=np.nan
     )
@@ -844,15 +833,15 @@
             )
 
     return reparameterized_inner_parameter_values
 
 
 def undo_inner_parameter_reparameterization(
     reparameterized_inner_parameter_values: np.ndarray,
-    inner_parameters: List[OptimalScalingParameter],
+    inner_parameters: list[OrdinalParameter],
     interval_gap: float,
     interval_range: float,
 ) -> np.ndarray:
     """Transform reparameterized inner parameters to original inner parameters."""
     original_inner_parameter_values = np.full(
         shape=(np.shape(reparameterized_inner_parameter_values)),
         fill_value=np.nan,
@@ -875,21 +864,21 @@
                 + interval_range
                 + original_inner_parameter_values[inner_parameter_category - 2]
             )
     return original_inner_parameter_values
 
 
 def obj_surrogate_data(
-    xs: List[OptimalScalingParameter],
+    xs: list[OrdinalParameter],
     optimal_scaling_bounds: np.ndarray,
-    sim: List[np.ndarray],
+    sim: list[np.ndarray],
     interval_gap: float,
     interval_range: float,
     w: float,
-    options: Dict,
+    options: dict,
 ) -> float:
     """Compute optimal scaling objective function."""
     obj = 0.0
     if options[REPARAMETERIZED]:
         optimal_scaling_bounds = undo_inner_parameter_reparameterization(
             optimal_scaling_bounds, xs, interval_gap, interval_range
         )
@@ -911,21 +900,21 @@
                     continue
                 obj += (y_surrogate - y_sim_i) ** 2
     obj = np.divide(obj, w)
     return obj
 
 
 def grad_surrogate_data(
-    xs: List[OptimalScalingParameter],
+    xs: list[OrdinalParameter],
     optimal_scaling_bounds: np.ndarray,
-    sim: List[np.ndarray],
+    sim: list[np.ndarray],
     interval_gap: float,
     interval_range: float,
     w: float,
-    options: Dict,
+    options: dict,
 ) -> float:
     """Compute optimal scaling objective function."""
     grad = np.zeros(len(optimal_scaling_bounds))
     if options[REPARAMETERIZED]:
         optimal_scaling_bounds = undo_inner_parameter_reparameterization(
             optimal_scaling_bounds, xs, interval_gap, interval_range
         )
@@ -975,15 +964,15 @@
         )
     grad = np.divide(grad, w)
     return grad
 
 
 def reparameterize_gradient(
     grad: np.ndarray,
-    xs: List[OptimalScalingParameter],
+    xs: list[OrdinalParameter],
 ) -> np.ndarray:
     """Transform gradient to reparameterized gradient."""
     reparameterized_grad = np.full(
         shape=(np.shape(grad)),
         fill_value=np.nan,
     )
     for inner_parameter in xs:
@@ -991,19 +980,19 @@
         reparameterized_grad[inner_parameter_category - 1] = np.sum(
             grad[inner_parameter_category - 1 :]
         )
     return reparameterized_grad
 
 
 def get_bounds_for_category(
-    x: OptimalScalingParameter,
+    x: OrdinalParameter,
     optimal_scaling_bounds: np.ndarray,
     interval_gap: float,
-    options: Dict,
-) -> Tuple[float, float]:
+    options: dict,
+) -> tuple[float, float]:
     """Return upper and lower bound for a specific category x."""
     x_category = int(x.category)
 
     if options[METHOD] == REDUCED:
         x_upper = optimal_scaling_bounds[x_category - 1]
         if x_category == 1:
             x_lower = 0
@@ -1019,16 +1008,16 @@
             f"Unknown optimal scaling method {options[METHOD]}. "
             f"Please use {REDUCED} or {STANDARD}."
         )
     return x_upper, x_lower
 
 
 def get_constraints_for_optimization(
-    xs: List[OptimalScalingParameter], sim: List[np.ndarray], options: Dict
-) -> Dict:
+    xs: list[OrdinalParameter], sim: list[np.ndarray], options: dict
+) -> dict:
     """Return constraints for inner optimization."""
     num_categories = len(xs)
     interval_range, interval_gap = compute_interval_constraints(
         xs, sim, options
     )
     if options[METHOD] == REDUCED:
         a = np.diag(-np.ones(num_categories), -1) + np.diag(
@@ -1049,20 +1038,20 @@
         b[2::2] = interval_gap
     ineq_cons = {'type': 'ineq', 'fun': lambda x: a.dot(x) - b}
 
     return ineq_cons
 
 
 def save_inner_parameters_to_inner_problem(
-    category_upper_bounds: List[OptimalScalingParameter],
+    category_upper_bounds: list[OrdinalParameter],
     group: int,
-    problem: OptimalScalingProblem,
-    x_inner_opt: Dict,
-    sim: List[np.ndarray],
-    options: Dict,
+    problem: OrdinalProblem,
+    x_inner_opt: dict,
+    sim: list[np.ndarray],
+    options: dict,
 ) -> None:
     """Save inner parameter values to the inner subproblem."""
     interval_range, interval_gap = compute_interval_constraints(
         category_upper_bounds, sim, options
     )
 
     surrogate_all, x_lower, x_upper = get_surrogate_all(
@@ -1078,21 +1067,21 @@
     for inner_parameter in problem.get_cat_ub_parameters_for_group(group):
         inner_parameter.value = x_upper[inner_parameter.category - 1]
     for inner_parameter in problem.get_cat_lb_parameters_for_group(group):
         inner_parameter.value = x_lower[inner_parameter.category - 1]
 
 
 def calculate_censored_obj(
-    category_upper_bounds: List[OptimalScalingParameter],
-    category_lower_bounds: List[OptimalScalingParameter],
-    sim: List[np.ndarray],
-    sigma: List[np.ndarray],
+    category_upper_bounds: list[OrdinalParameter],
+    category_lower_bounds: list[OrdinalParameter],
+    sim: list[np.ndarray],
+    sigma: list[np.ndarray],
     quantitative_data: np.ndarray,
-    quantitative_ixs: List[np.ndarray],
-) -> Dict:
+    quantitative_ixs: list[np.ndarray],
+) -> dict:
     """Calculate objective function for a group with censored data.
 
     Parameters
     ----------
     category_upper_bounds:
         The upper bounds for the categories.
     category_lower_bounds:
@@ -1155,23 +1144,23 @@
         SCIPY_FUN: obj,
         SCIPY_X: np.ravel([cat_lb_values, cat_ub_values], order='F'),
     }
     return return_dictionary
 
 
 def calculate_censored_grad(
-    category_upper_bounds: List[OptimalScalingParameter],
-    category_lower_bounds: List[OptimalScalingParameter],
-    sim: List[np.ndarray],
+    category_upper_bounds: list[OrdinalParameter],
+    category_lower_bounds: list[OrdinalParameter],
+    sim: list[np.ndarray],
     sy: np.ndarray,
-    sigma: List[np.ndarray],
+    sigma: list[np.ndarray],
     ssigma: np.ndarray,
-    par_edata_idx: List,
+    par_edata_idx: list,
     quantitative_data: np.ndarray,
-    quantitative_ixs: List[np.ndarray],
+    quantitative_ixs: list[np.ndarray],
 ):
     """Calculate gradient for a group with censored data with respect to an outer parameter.
 
     Parameters
     ----------
     category_upper_bounds:
         The upper bounds for the categories.
@@ -1241,27 +1230,31 @@
         [sim_i[mask_i] for sim_i, mask_i in zip(sim, quantitative_ixs)]
     )
     quantitative_sigma = np.concatenate(
         [sigma_i[mask_i] for sigma_i, mask_i in zip(sigma, quantitative_ixs)]
     )
     quantitative_sy = np.concatenate(
         [
-            sy_i[:, edata_idx, :][mask_i]
-            if edata_idx is not None
-            else np.full(sy_i[:, 0, :][mask_i].shape, 0)
+            (
+                sy_i[:, edata_idx, :][mask_i]
+                if edata_idx is not None
+                else np.full(sy_i[:, 0, :][mask_i].shape, 0)
+            )
             for sy_i, mask_i, edata_idx in zip(
                 sy, quantitative_ixs, par_edata_idx
             )
         ]
     )
     quantitative_ssigma = np.concatenate(
         [
-            ssigma_i[:, edata_idx, :][mask_i]
-            if edata_idx is not None
-            else np.full(ssigma_i[:, 0, :][mask_i].shape, 0)
+            (
+                ssigma_i[:, edata_idx, :][mask_i]
+                if edata_idx is not None
+                else np.full(ssigma_i[:, 0, :][mask_i].shape, 0)
+            )
             for ssigma_i, mask_i, edata_idx in zip(
                 ssigma, quantitative_ixs, par_edata_idx
             )
         ]
     )
 
     # Calculate the negative log likelihood gradient for uncensored, quantitative data.
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/parameter.py` & `pypesto-0.4.2/pypesto/hierarchical/base_parameter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Literal
+from typing import Any, Literal, Optional
 
 import numpy as np
 
 from ..C import (
     DUMMY_INNER_VALUE,
     INNER_PARAMETER_BOUNDS,
     LIN,
@@ -20,16 +20,17 @@
 class InnerParameter:
     """
     An inner parameter of a hierarchical optimization problem.
 
     Attributes
     ----------
     coupled:
-        Whether the inner parameter is part of an observable that has both
-        an offset and scaling inner parameter.
+        If the inner parameter is part of an observable that has both
+        an offset and scaling inner parameter, this attribute points to
+        the other inner parameter. Otherwise, it is None.
     dummy_value:
         Value to be used when the optimal parameter is not yet known
         (in particular to simulate unscaled observables).
     inner_parameter_id:
         The inner parameter ID.
     inner_parameter_type:
         The inner parameter type.
@@ -58,35 +59,40 @@
         Construct.
 
         Parameters
         ----------
         See class attributes.
         """
         self.inner_parameter_id: str = inner_parameter_id
-        self.coupled = False
+        self.coupled: InnerParameter = None
         self.inner_parameter_type: str = inner_parameter_type
 
         if scale not in {LIN, LOG, LOG10}:
             raise ValueError(f"Scale not recognized: {scale}.")
         self.scale = scale
 
         if inner_parameter_type not in (
-            InnerParameterType.OPTIMAL_SCALING,
+            InnerParameterType.ORDINAL,
             InnerParameterType.OFFSET,
             InnerParameterType.SIGMA,
             InnerParameterType.SCALING,
             InnerParameterType.SPLINE,
         ):
             raise ValueError(
                 f"Unsupported inner parameter type `{inner_parameter_type}`."
             )
 
         self.lb: float = lb
         self.ub: float = ub
-        self.check_bounds()
+        # Scaling and offset parameters can be bounded arbitrarily
+        if inner_parameter_type not in (
+            InnerParameterType.SCALING,
+            InnerParameterType.OFFSET,
+        ):
+            self.check_bounds()
         self.ixs: Any = ixs
 
         if dummy_value is None:
             try:
                 dummy_value = DUMMY_INNER_VALUE[inner_parameter_type]
             except KeyError as e:
                 raise ValueError(
@@ -110,7 +116,25 @@
             raise ValueError(
                 "Invalid bounds for inner parameters. Parameter ID: "
                 f"`{self.inner_parameter_id}`. Provided bounds: "
                 f"`[{self.lb}, {self.ub}]`. Expected bounds: "
                 f"`[{expected_lb}, {expected_ub}]`. "
                 f"All expected parameter bounds:\n{INNER_PARAMETER_BOUNDS}"
             )
+
+    def is_within_bounds(self, value):
+        """Check whether a value is within the bounds."""
+        if value < self.lb or value > self.ub:
+            return False
+        return True
+
+    def get_unsatisfied_bound(self, value) -> Optional[str]:
+        """Get the unsatisfied bound index, if any."""
+        if value < self.lb:
+            return LOWER_BOUND
+        elif value > self.ub:
+            return UPPER_BOUND
+        return None
+
+    def get_bounds(self) -> dict:
+        """Get the bounds."""
+        return {LOWER_BOUND: self.lb, UPPER_BOUND: self.ub}
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/petab.py` & `pypesto-0.4.2/pypesto/hierarchical/petab.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 """Helper methods for hierarchical optimization with PEtab."""
 
-from typing import Dict, Literal, Tuple
+from typing import Literal
 
 import pandas as pd
 import petab
 import sympy as sp
 from more_itertools import one
-from petab.C import LIN
+from petab.C import ESTIMATE, LIN
 from petab.C import LOWER_BOUND as PETAB_LOWER_BOUND
 from petab.C import (
+    NOISE_PARAMETERS,
     OBSERVABLE_ID,
+    OBSERVABLE_PARAMETERS,
     OBSERVABLE_TRANSFORMATION,
     PARAMETER_SEPARATOR,
 )
 from petab.C import UPPER_BOUND as PETAB_UPPER_BOUND
 from petab.observables import get_formula_placeholders
 
-from ..C import INNER_PARAMETER_BOUNDS
+from ..C import (
+    CENSORING_BOUNDS,
+    CENSORING_TYPES,
+    INNER_PARAMETER_BOUNDS,
+    INTERVAL_CENSORED,
+    LEFT_CENSORED,
+)
 from ..C import LOWER_BOUND as PYPESTO_LOWER_BOUND
-from ..C import PARAMETER_TYPE
+from ..C import (
+    MEASUREMENT_CATEGORY,
+    MEASUREMENT_TYPE,
+    ORDINAL,
+    PARAMETER_TYPE,
+    RELATIVE,
+    RIGHT_CENSORED,
+    SEMIQUANTITATIVE,
+)
 from ..C import UPPER_BOUND as PYPESTO_UPPER_BOUND
 from ..C import InnerParameterType
 
 
 def correct_parameter_df_bounds(parameter_df: pd.DataFrame) -> pd.DataFrame:
     """Correct the bounds of inner parameters in a PEtab parameters table.
 
@@ -35,14 +51,19 @@
     -------
     The table, with corrected bounds.
     """
 
     def correct_row(row: pd.Series) -> pd.Series:
         if pd.isna(row[PARAMETER_TYPE]):
             return row
+        if row[PARAMETER_TYPE] in [
+            InnerParameterType.SCALING,
+            InnerParameterType.OFFSET,
+        ]:
+            return row
         bounds = INNER_PARAMETER_BOUNDS[row[PARAMETER_TYPE]]
         row[PETAB_LOWER_BOUND] = bounds[PYPESTO_LOWER_BOUND]
         row[PETAB_UPPER_BOUND] = bounds[PYPESTO_UPPER_BOUND]
         return row
 
     return parameter_df.apply(correct_row, axis=1)
 
@@ -62,15 +83,14 @@
     # ensure we only have linear parameter scale
     inner_parameter_table = petab_problem.parameter_df[
         petab_problem.parameter_df[PARAMETER_TYPE].isin(
             [
                 InnerParameterType.OFFSET,
                 InnerParameterType.SIGMA,
                 InnerParameterType.SCALING,
-                InnerParameterType.OPTIMAL_SCALING,
             ]
         )
     ]
     if (
         petab.PARAMETER_SCALE in inner_parameter_table
         and not (
             inner_parameter_table[petab.PARAMETER_SCALE].isna()
@@ -87,14 +107,16 @@
 
     inner_parameter_df = validate_measurement_formulae(
         petab_problem=petab_problem
     )
 
     validate_inner_parameter_pairings(inner_parameter_df=inner_parameter_df)
 
+    validate_observable_data_types(petab_problem=petab_problem)
+
 
 def validate_inner_parameter_pairings(
     inner_parameter_df: pd.DataFrame,
 ):
     """Validate the pairings of inner parameters.
 
     Parameters
@@ -170,15 +192,15 @@
         #      any scaling?
         #      Same for offset?
         #      Same for scaling+sigma and offset+sigma pairings?
 
 
 def get_inner_parameters(
     petab_problem: petab.Problem,
-) -> Dict[str, InnerParameterType]:
+) -> dict[str, InnerParameterType]:
     """Get information about the inner parameters.
 
     Parameters
     ----------
     petab_problem:
         The PEtab problem, with inner parameters.
 
@@ -259,16 +281,16 @@
         ],
     )
 
 
 def _validate_measurement_specific_observable_formula(
     measurement: pd.Series,
     petab_problem: petab.Problem,
-    inner_parameters: Dict[str, InnerParameterType],
-) -> Tuple[InnerParameterType, InnerParameterType]:
+    inner_parameters: dict[str, InnerParameterType],
+) -> tuple[InnerParameterType, InnerParameterType]:
     """Check whether a measurement observable formula is valid.
 
     Parameters
     ----------
     measurement:
         A row from a PEtab measurements table.
     petab_problem:
@@ -344,16 +366,16 @@
 
     return offset, scaling
 
 
 def _validate_measurement_specific_noise_formula(
     measurement: pd.Series,
     petab_problem: petab.Problem,
-    inner_parameters: Dict[str, InnerParameterType],
-) -> Tuple[InnerParameterType, InnerParameterType]:
+    inner_parameters: dict[str, InnerParameterType],
+) -> tuple[InnerParameterType, InnerParameterType]:
     """Check whether a measurement noise formula is valid.
 
     Parameters
     ----------
     measurement:
         A row from a PEtab measurements table.
     petab_problem:
@@ -396,16 +418,16 @@
     return sigma
 
 
 def _get_symbolic_formula_from_measurement(
     measurement: pd.Series,
     formula_type: Literal['observable', 'noise'],
     petab_problem: petab.Problem,
-    inner_parameters: Dict[str, InnerParameterType],
-) -> Tuple[sp.Expr, Dict[sp.Symbol, InnerParameterType]]:
+    inner_parameters: dict[str, InnerParameterType],
+) -> tuple[sp.Expr, dict[sp.Symbol, InnerParameterType]]:
     """Get a symbolic representation of a formula, with overrides overridden.
 
     Also performs some checks to ensure only valid numbers and types of inner
     parameters are in the formula.
 
     Parameters
     ----------
@@ -495,7 +517,153 @@
                 "the observable is associated with hierarchically-optimized "
                 f"inner parameters. "
                 f"Observable transformation: `{observable_transformation}`. "
                 f"Measurement:\n{measurement}"
             )
 
     return symbolic_formula, symbolic_formula_inner_parameters
+
+
+def validate_observable_data_types(petab_problem: petab.Problem) -> None:
+    """Check whether the data types of observables are valid."""
+
+    supported_data_types = [
+        SEMIQUANTITATIVE,
+        RELATIVE,
+        ORDINAL,
+    ] + CENSORING_TYPES
+
+    # Get observables across data types
+    observables_by_data_type = {}
+    meas_df = petab_problem.measurement_df
+    if MEASUREMENT_TYPE in meas_df.columns:
+        petab_data_types = meas_df[meas_df[MEASUREMENT_TYPE].notna()][
+            MEASUREMENT_TYPE
+        ].unique()
+        for data_type in petab_data_types:
+            observables_by_data_type[data_type] = set(
+                meas_df.loc[
+                    meas_df[MEASUREMENT_TYPE] == data_type, OBSERVABLE_ID
+                ]
+            )
+        # Check whether all data types are supported
+        if not set(petab_data_types).issubset(supported_data_types):
+            raise ValueError(
+                f"Unsupported data type(s): `{set(petab_data_types) - set(supported_data_types)}`."
+            )
+
+    # For relative data, we search for observable parameters in the parameter table
+    # and their corresponding observables in the measurement table.
+    relative_observables = set()
+    if PARAMETER_TYPE in petab_problem.parameter_df.columns:
+        par_df = petab_problem.parameter_df[
+            petab_problem.parameter_df[PARAMETER_TYPE].notna()
+        ]
+        meas_df_w_obs_pars = meas_df[meas_df[OBSERVABLE_PARAMETERS].notna()]
+        for par_id, row in par_df.iterrows():
+            if not row[ESTIMATE]:
+                continue
+            if row[PARAMETER_TYPE] in [
+                InnerParameterType.SCALING,
+                InnerParameterType.OFFSET,
+            ]:
+                for _, row in meas_df_w_obs_pars.iterrows():
+                    if par_id in row[OBSERVABLE_PARAMETERS].split(
+                        PARAMETER_SEPARATOR
+                    ):
+                        relative_observables.add(row[OBSERVABLE_ID])
+
+            elif row[PARAMETER_TYPE] == InnerParameterType.SIGMA:
+                corresponding_obs = set(
+                    meas_df[meas_df[NOISE_PARAMETERS] == par_id][OBSERVABLE_ID]
+                )
+                # If a sigma parameter belongs to a semi-quantiative
+                # observable, it is not a relative inner parameter.
+                if SEMIQUANTITATIVE in observables_by_data_type and (
+                    corresponding_obs
+                    & observables_by_data_type[SEMIQUANTITATIVE]
+                ):
+                    continue
+                relative_observables.update(corresponding_obs)
+
+    observables_by_data_type[RELATIVE] = relative_observables
+
+    # Check whether there is any overlap across data types
+    for data_type, observables in observables_by_data_type.items():
+        for (
+            other_data_type,
+            other_observables,
+        ) in observables_by_data_type.items():
+            if data_type == other_data_type:
+                continue
+            if observables & other_observables:
+                raise ValueError(
+                    "The same observable is associated with multiple data "
+                    f"types. Observable(s): `{observables & other_observables}`. "
+                    f"Data types: `{data_type}`, `{other_data_type}`."
+                )
+
+    # Validate ordinal measurement specification
+    if ORDINAL in observables_by_data_type:
+        meas_df_w_ordinals = meas_df[meas_df[MEASUREMENT_TYPE] == ORDINAL]
+        if MEASUREMENT_CATEGORY not in meas_df_w_ordinals.columns:
+            raise ValueError(
+                "Measurement category must be specified for ordinal "
+                "measurements."
+            )
+        for _, row in meas_df_w_ordinals.iterrows():
+            try:
+                category = float(row[MEASUREMENT_CATEGORY])
+                if category != int(category):
+                    raise ValueError
+            except ValueError as e:
+                raise ValueError(
+                    "Measurement category for ordinal measurement must be "
+                    "an integer."
+                ) from e
+
+    # Validate censored measurement specification
+    if set(CENSORING_TYPES) & set(observables_by_data_type.keys()):
+        meas_df_w_censored = meas_df[
+            meas_df[MEASUREMENT_TYPE].isin(CENSORING_TYPES)
+        ]
+        if CENSORING_BOUNDS not in meas_df_w_censored.columns:
+            raise ValueError(
+                "Censoring bounds must be specified for censored "
+                "measurements."
+            )
+        for _, row in meas_df_w_censored.iterrows():
+            if (
+                row[MEASUREMENT_TYPE] == LEFT_CENSORED
+                or row[MEASUREMENT_TYPE] == RIGHT_CENSORED
+            ):
+                try:
+                    float(row[CENSORING_BOUNDS])
+                except ValueError as e:
+                    raise ValueError(
+                        f"Censoring bound(s) for a {row[MEASUREMENT_TYPE]}"
+                        " measurement must be of type float. Failure at "
+                        f"bound: `{row[CENSORING_BOUNDS]}`."
+                    ) from e
+            elif row[MEASUREMENT_TYPE] == INTERVAL_CENSORED:
+                bounds = row[CENSORING_BOUNDS].split(PARAMETER_SEPARATOR)
+                if len(bounds) != 2:
+                    raise ValueError(
+                        f"Censoring bounds for a {INTERVAL_CENSORED} measurement"
+                        f" must be two floats separated by the separator {PARAMETER_SEPARATOR}."
+                        f" Found {len(bounds)} bounds: `{bounds}`."
+                    )
+                try:
+                    float(bounds[0])
+                    float(bounds[1])
+                except ValueError as e:
+                    raise ValueError(
+                        f"Censoring bound(s) for a {row[MEASUREMENT_TYPE]}"
+                        " measurement must be of type float. Failure at "
+                        f"bounds: `{bounds}`."
+                    ) from e
+                if float(bounds[0]) > float(bounds[1]):
+                    raise ValueError(
+                        f"Censoring bounds for a {INTERVAL_CENSORED}"
+                        " measurement must be increasing. Failure at "
+                        f"bounds: `{bounds}`."
+                    )
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/problem.py` & `pypesto-0.4.2/pypesto/hierarchical/relative/problem.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 """Inner optimization problem in hierarchical optimization."""
+
 import logging
-from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
-from ..C import PARAMETER_TYPE, InnerParameterType
-from .parameter import InnerParameter
+from ...C import (
+    MEASUREMENT_TYPE,
+    PARAMETER_TYPE,
+    SEMIQUANTITATIVE,
+    InnerParameterType,
+)
+from ..base_parameter import InnerParameter
+from ..base_problem import (
+    AmiciInnerProblem,
+    _get_timepoints_with_replicates,
+    ix_matrices_from_arrays,
+)
 
 try:
     import amici
     import petab
     from petab.C import (
         ESTIMATE,
         LOWER_BOUND,
@@ -24,120 +34,43 @@
     )
 except ImportError:
     pass
 
 logger = logging.getLogger(__name__)
 
 
-class InnerProblem:
-    """
-    Inner optimization problem in hierarchical optimization.
+class RelativeInnerProblem(AmiciInnerProblem):
+    r"""Inner optimization problem for relative data with scaling/offset.
 
     Attributes
     ----------
     xs:
         Mapping of (inner) parameter ID to ``InnerParameters``.
     data:
         Measurement data. One matrix (`num_timepoints` x `num_observables`)
         per simulation condition. Missing observations as NaN.
+    edatas:
+        AMICI ``ExpData``\s for each simulation condition.
     """
 
-    def __init__(self, xs: List[InnerParameter], data: List[np.ndarray]):
-        self.xs: Dict[str, InnerParameter] = {
-            x.inner_parameter_id: x for x in xs
-        }
-        self.data = data
-
-        logger.debug(f"Created InnerProblem with ids {self.get_x_ids()}")
-
-        if self.is_empty():
-            raise ValueError(
-                'There are no parameters in the inner problem of hierarchical '
-                'optimization.'
-            )
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
     @staticmethod
     def from_petab_amici(
         petab_problem: 'petab.Problem',
         amici_model: 'amici.Model',
-        edatas: List['amici.ExpData'],
-    ) -> 'InnerProblem':
+        edatas: list['amici.ExpData'],
+    ) -> 'RelativeInnerProblem':
         """Create an InnerProblem from a PEtab problem and AMICI objects."""
         return inner_problem_from_petab_problem(
             petab_problem, amici_model, edatas
         )
 
-    def get_x_ids(self) -> List[str]:
-        """Get IDs of inner parameters."""
-        return list(self.xs.keys())
-
-    def get_xs_for_type(
-        self, inner_parameter_type: str
-    ) -> List[InnerParameter]:
-        """Get inner parameters of the given type."""
-        return [
-            x
-            for x in self.xs.values()
-            if x.inner_parameter_type == inner_parameter_type
-        ]
-
-    def get_dummy_values(self, scaled: bool) -> Dict[str, float]:
-        """
-        Get dummy parameter values.
-
-        Get parameter values to be used for simulation before their optimal
-        values are computed.
-
-        Parameters
-        ----------
-        scaled:
-            Whether the parameters should be returned on parameter or linear
-            scale.
-        """
-        return {
-            x.inner_parameter_id: scale_value(x.dummy_value, x.scale)
-            if scaled
-            else x.dummy_value
-            for x in self.xs.values()
-        }
-
-    def get_for_id(self, inner_parameter_id: str) -> InnerParameter:
-        """Get InnerParameter for the given parameter ID."""
-        try:
-            return self.xs[inner_parameter_id]
-        except KeyError:
-            raise KeyError(f"Cannot find parameter with id {id}.")
-
-    def is_empty(self) -> bool:
-        """Check for emptiness.
-
-        Returns
-        -------
-        ``True`` if there aren't any parameters associated with this problem,
-        ``False`` otherwise.
-        """
-        return len(self.xs) == 0
-
-
-class AmiciInnerProblem(InnerProblem):
-    """
-    Inner optimization problem in hierarchical optimization.
-
-    For use with AMICI objects.
-
-    Attributes
-    ----------
-    edataviews:
-        AMICI ``ExpDataView``s for each simulation condition.
-    """
-
-    def __init__(self, edatas: List[amici.ExpData], **kwargs):
-        super().__init__(**kwargs)
-
-    def check_edatas(self, edatas: List[amici.ExpData]) -> bool:
+    def check_edatas(self, edatas: list[amici.ExpData]) -> bool:
         """Check for consistency in data.
 
         Currently only checks for the actual data values. e.g., timepoints are
         not compared.
 
         Parameters
         ----------
@@ -161,53 +94,29 @@
         for data0, data1 in zip(self.data, data):
             if not np.array_equal(data0, data1, equal_nan=True):
                 return False
 
         return True
 
 
-def scale_value_dict(
-    dct: Dict[str, float], problem: InnerProblem
-) -> Dict[str, float]:
-    """Scale a value dictionary."""
-    scaled_dct = {}
-    for key, val in dct.items():
-        x = problem.get_for_id(key)
-        scaled_dct[key] = scale_value(val, x.scale)
-    return scaled_dct
-
-
-def scale_value(
-    val: Union[float, np.array], scale: str
-) -> Union[float, np.array]:
-    """Scale a single value."""
-    if scale == 'lin':
-        return val
-    if scale == 'log':
-        return np.log(val)
-    if scale == 'log10':
-        return np.log10(val)
-    raise ValueError(f"Scale {scale} not recognized.")
-
-
 def inner_problem_from_petab_problem(
     petab_problem: 'petab.Problem',
     amici_model: 'amici.Model',
-    edatas: List['amici.ExpData'],
-) -> InnerProblem:
+    edatas: list['amici.ExpData'],
+) -> AmiciInnerProblem:
     """
     Create inner problem from PEtab problem.
 
     Hierarchical optimization is a pypesto-specific PEtab extension.
     """
     import amici
 
     # inner parameters
     inner_parameters = inner_parameters_from_parameter_df(
-        petab_problem.parameter_df
+        petab_problem.parameter_df, petab_problem.measurement_df
     )
 
     x_ids = [x.inner_parameter_id for x in inner_parameters]
 
     # used indices for all measurement specific parameters
     ixs = ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, x_ids
@@ -220,69 +129,99 @@
     ix_matrices = ix_matrices_from_arrays(ixs, data)
 
     # assign matrices
     for par in inner_parameters:
         par.ixs = ix_matrices[par.inner_parameter_id]
 
     par_group_types = {
-        tuple(obs_pars.split(';')): {
+        tuple(obs_pars.split(';')): (
             petab_problem.parameter_df.loc[obs_par, PARAMETER_TYPE]
             for obs_par in obs_pars.split(';')
-        }
+        )
         for (obs_id, obs_pars), _ in petab_problem.measurement_df.groupby(
             [petab.OBSERVABLE_ID, petab.OBSERVABLE_PARAMETERS], dropna=True
         )
         if ';' in obs_pars  # prefilter for at least 2 observable parameters
     }
 
     coupled_pars = {
-        par
+        group
         for group, types in par_group_types.items()
         if (
             (InnerParameterType.SCALING in types)
             and (InnerParameterType.OFFSET in types)
         )
-        for par in group
     }
 
+    # Check each group is of length 2
+    for group in coupled_pars:
+        if len(group) != 2:
+            raise ValueError(
+                f"Expected exactly 2 parameters in group {group}: a scaling "
+                f"and an offset parameter."
+            )
+
+    id_to_par = {par.inner_parameter_id: par for par in inner_parameters}
+
+    # assign coupling
     for par in inner_parameters:
         if par.inner_parameter_type not in [
             InnerParameterType.SCALING,
             InnerParameterType.OFFSET,
         ]:
             continue
-        if par.inner_parameter_id in coupled_pars:
-            par.coupled = True
+        for group in coupled_pars:
+            if par.inner_parameter_id in group:
+                coupled_parameter_id = group[
+                    group.index(par.inner_parameter_id) - 1
+                ]
+                par.coupled = id_to_par[coupled_parameter_id]
+                break
 
     return AmiciInnerProblem(xs=inner_parameters, data=data, edatas=edatas)
 
 
 def inner_parameters_from_parameter_df(
-    df: pd.DataFrame,
-) -> List[InnerParameter]:
+    par_df: pd.DataFrame,
+    meas_df: pd.DataFrame,
+) -> list[InnerParameter]:
     """
     Create list of inner free parameters from PEtab parameter table.
 
     Inner parameters are those that have a non-empty `parameterType` in the
     PEtab problem.
     """
     # create list of hierarchical parameters
-    df = df.reset_index()
+    par_df = par_df.reset_index()
 
     for col in (PARAMETER_TYPE,):
-        if col not in df:
-            df[col] = None
+        if col not in par_df:
+            par_df[col] = None
 
     parameters = []
 
-    for _, row in df.iterrows():
+    for _, row in par_df.iterrows():
         if not row[ESTIMATE]:
             continue
         if petab.is_empty(row[PARAMETER_TYPE]):
             continue
+        # If a sigma parameter belongs to a semiquantitative
+        # observable, it is not a relative inner parameter.
+        if row[PARAMETER_TYPE] == InnerParameterType.SIGMA:
+            if MEASUREMENT_TYPE in meas_df.columns:
+                par_id = row[PARAMETER_ID]
+                corresponding_measurements = meas_df[
+                    meas_df[NOISE_PARAMETERS] == par_id
+                ]
+                if any(
+                    corresponding_measurements[MEASUREMENT_TYPE]
+                    == SEMIQUANTITATIVE
+                ):
+                    continue
+
         parameters.append(
             InnerParameter(
                 inner_parameter_id=row[PARAMETER_ID],
                 inner_parameter_type=row[PARAMETER_TYPE],
                 scale=row[PARAMETER_SCALE],
                 lb=row[LOWER_BOUND],
                 ub=row[UPPER_BOUND],
@@ -291,22 +230,22 @@
 
     return parameters
 
 
 def ixs_for_measurement_specific_parameters(
     petab_problem: 'petab.Problem',
     amici_model: 'amici.Model',
-    x_ids: List[str],
-) -> Dict[str, List[Tuple[int, int, int]]]:
+    x_ids: list[str],
+) -> dict[str, list[tuple[int, int, int]]]:
     """
     Create mapping of parameters to measurements.
 
     Returns
     -------
-    A dictionary mapping parameter ID to a List of
+    A dictionary mapping parameter ID to a list of
     `(condition index, time index, observable index)` tuples in which this
     output parameter is used. For each condition, the time index refers to
     a sorted list of non-unique time points for which there are measurements.
     """
     ixs_for_par = {}
     observable_ids = amici_model.getObservableIds()
 
@@ -362,60 +301,7 @@
                 # try to insert if hierarchical parameter
                 for override in observable_overrides + noise_overrides:
                     if override in x_ids:
                         ixs_for_par.setdefault(override, []).append(
                             (condition_ix, time_w_reps_ix, observable_ix)
                         )
     return ixs_for_par
-
-
-def ix_matrices_from_arrays(
-    ixs: Dict[str, List[Tuple[int, int, int]]], edatas: List[np.array]
-) -> Dict[str, List[np.array]]:
-    """
-    Convert mapping of parameters to measurements to matrix form.
-
-    Returns
-    -------
-    A dictionary mapping parameter ID to a list of Boolean matrices, one per
-    simulation condition. Therein, ``True`` indicates that the respective
-    parameter is used for the model output at the respective timepoint,
-    observable and condition index.
-    """
-    ix_matrices = {
-        id: [np.zeros_like(edata, dtype=bool) for edata in edatas]
-        for id in ixs
-    }
-    for id, arr in ixs.items():
-        matrices = ix_matrices[id]
-        for condition_ix, time_ix, observable_ix in arr:
-            matrices[condition_ix][time_ix, observable_ix] = True
-    return ix_matrices
-
-
-def _get_timepoints_with_replicates(
-    measurement_df: pd.DataFrame,
-) -> List[float]:
-    """
-    Get list of timepoints including replicate measurements.
-
-    :param measurement_df:
-        PEtab measurement table subset for a single condition.
-
-    :return:
-        Sorted list of timepoints, including multiple timepoints accounting
-        for replicate measurements.
-    """
-    # create sorted list of all timepoints for which measurements exist
-    timepoints = sorted(measurement_df[TIME].unique().astype(float))
-
-    # find replicate numbers of time points
-    timepoints_w_reps = []
-    for time in timepoints:
-        # subselect for time
-        df_for_time = measurement_df[measurement_df.time == time]
-        # rep number is maximum over rep numbers for observables
-        n_reps = max(df_for_time.groupby([OBSERVABLE_ID, TIME]).size())
-        # append time point n_rep times
-        timepoints_w_reps.extend([time] * n_reps)
-
-    return timepoints_w_reps
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/solver.py` & `pypesto-0.4.2/pypesto/hierarchical/base_problem.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,300 +1,280 @@
+"""Inner optimization problem in hierarchical optimization."""
+
 import copy
-from typing import Any, Dict, List
+import logging
+from typing import Union
 
 import numpy as np
+import pandas as pd
 
-from ..C import InnerParameterType
-from ..objective import Objective
-from ..optimize import minimize
-from ..problem import Problem
-from .problem import InnerProblem, scale_value_dict
-from .util import (
-    apply_offset,
-    apply_scaling,
-    apply_sigma,
-    compute_nllh,
-    compute_optimal_offset,
-    compute_optimal_offset_coupled,
-    compute_optimal_scaling,
-    compute_optimal_sigma,
-)
+from .base_parameter import InnerParameter
 
+try:
+    import amici
+    import petab
+    from petab.C import OBSERVABLE_ID, TIME
+except ImportError:
+    pass
 
-class InnerSolver:
-    """Solver for an inner optimization problem."""
+logger = logging.getLogger(__name__)
 
-    def initialize(self):
-        """
-        (Re-)initialize the solver.
 
-        Default: Do nothing.
-        """
+class InnerProblem:
+    """
+    Inner optimization problem in hierarchical optimization.
 
-    def solve(
-        self,
-        problem: InnerProblem,
-        sim: List[np.ndarray],
-        sigma: List[np.ndarray],
-        scaled: bool,
-    ) -> Dict[str, float]:
-        """Solve the subproblem.
+    Attributes
+    ----------
+    xs:
+        Mapping of (inner) parameter ID to ``InnerParameters``.
+    data:
+        Measurement data. One matrix (`num_timepoints` x `num_observables`)
+        per simulation condition. Missing observations as NaN.
+    """
 
-        Parameters
-        ----------
-        problem:
-            The inner problem to solve.
-        sim:
-            List of model output matrices, as provided in AMICI's
-            ``ReturnData.y``. Same order as simulations in the
-            PEtab problem.
-        sigma:
-            List of sigma matrices from the model, as provided in AMICI's
-            ``ReturnData.sigmay``. Same order as simulations in the
-            PEtab problem.
-        scaled:
-            Whether to scale the results to the parameter scale specified in
-            ``problem``.
-        """
+    def __init__(self, xs: list[InnerParameter], data: list[np.ndarray]):
+        self.xs: dict[str, InnerParameter] = {
+            x.inner_parameter_id: x for x in xs
+        }
+        self.data = copy.deepcopy(data)
+
+        # create the joint mask of all inner problem parameters
+        self.data_mask = [
+            np.zeros_like(cond_data, dtype=bool) for cond_data in data
+        ]
+        for x in xs:
+            for condition_ix, cond_mask in enumerate(self.data_mask):
+                cond_mask[x.ixs[condition_ix]] = True
+
+        # mask the data: a inner problem is aware of only the data it uses
+        for i in range(len(self.data)):
+            self.data[i][~self.data_mask[i]] = np.nan
+
+        logger.debug(f"Created InnerProblem with ids {self.get_x_ids()}")
+
+        if self.is_empty():
+            raise ValueError(
+                'There are no parameters in the inner problem of hierarchical '
+                'optimization.'
+            )
 
+    @staticmethod
+    def from_petab_amici(
+        petab_problem: 'petab.Problem',
+        amici_model: 'amici.Model',
+        edatas: list['amici.ExpData'],
+    ) -> 'InnerProblem':
+        """Create an InnerProblem from a PEtab problem and AMICI objects."""
+
+    def get_x_ids(self) -> list[str]:
+        """Get IDs of inner parameters."""
+        return list(self.xs.keys())
+
+    def get_interpretable_x_ids(self) -> list[str]:
+        """Get IDs of interpretable inner parameters.
+
+        Interpretable parameters need to be easily interpretable by the user.
+        Examples are scaling factors, offsets, or noise parameters. An example
+        of non-interpretable inner parameters is the spline heights of spline
+        approximation for semiquantitative data. It is challenging to interpret
+        the meaning of these parameters based solely on their value.
+        """
+        return list(self.xs.keys())
 
-class AnalyticalInnerSolver(InnerSolver):
-    """Solve the inner subproblem analytically.
+    def get_xs_for_type(
+        self, inner_parameter_type: str
+    ) -> list[InnerParameter]:
+        """Get inner parameters of the given type."""
+        return [
+            x
+            for x in self.xs.values()
+            if x.inner_parameter_type == inner_parameter_type
+        ]
 
-    Currently, supports offset and scaling parameters (coupled or not), and
-    sigmas for additive Gaussian noise.
-    """
+    def get_dummy_values(self, scaled: bool) -> dict[str, float]:
+        """
+        Get dummy parameter values.
 
-    def solve(
-        self,
-        problem: InnerProblem,
-        sim: List[np.ndarray],
-        sigma: List[np.ndarray],
-        scaled: bool,
-    ) -> Dict[str, float]:
-        """Solve the subproblem analytically.
+        Get parameter values to be used for simulation before their optimal
+        values are computed.
 
         Parameters
         ----------
-        problem:
-            The inner problem to solve.
-        sim:
-            List of model output matrices, as provided in AMICI's
-            ``ReturnData.y``. Same order as simulations in the
-            PEtab problem.
-        sigma:
-            List of sigma matrices from the model, as provided in AMICI's
-            ``ReturnData.sigmay``. Same order as simulations in the
-            PEtab problem.
         scaled:
-            Whether to scale the results to the parameter scale specified in
-            ``problem``.
+            Whether the parameters should be returned on parameter scale (``True``)
+            or on linear scale (``False``).
         """
-        x_opt = {}
-
-        data = copy.deepcopy(problem.data)
-
-        # compute optimal offsets
-        for x in problem.get_xs_for_type(InnerParameterType.OFFSET):
-            if x.coupled:
-                x_opt[x.inner_parameter_id] = compute_optimal_offset_coupled(
-                    data=data, sim=sim, sigma=sigma, mask=x.ixs
-                )
-            else:
-                x_opt[x.inner_parameter_id] = compute_optimal_offset(
-                    data=data, sim=sim, sigma=sigma, mask=x.ixs
-                )
-        # apply offsets
-        for x in problem.get_xs_for_type(InnerParameterType.OFFSET):
-            apply_offset(
-                offset_value=x_opt[x.inner_parameter_id], data=data, mask=x.ixs
-            )
-
-        # compute optimal scalings
-        for x in problem.get_xs_for_type(InnerParameterType.SCALING):
-            x_opt[x.inner_parameter_id] = compute_optimal_scaling(
-                data=data, sim=sim, sigma=sigma, mask=x.ixs
-            )
-        # apply scalings
-        for x in problem.get_xs_for_type(InnerParameterType.SCALING):
-            apply_scaling(
-                scaling_value=x_opt[x.inner_parameter_id], sim=sim, mask=x.ixs
+        return {
+            x.inner_parameter_id: (
+                scale_value(x.dummy_value, x.scale)
+                if scaled
+                else x.dummy_value
             )
+            for x in self.xs.values()
+        }
 
-        # compute optimal sigmas
-        for x in problem.get_xs_for_type(InnerParameterType.SIGMA):
-            x_opt[x.inner_parameter_id] = compute_optimal_sigma(
-                data=data, sim=sim, mask=x.ixs
-            )
-        # apply sigmas
-        for x in problem.get_xs_for_type(InnerParameterType.SIGMA):
-            apply_sigma(
-                sigma_value=x_opt[x.inner_parameter_id],
-                sigma=sigma,
-                mask=x.ixs,
-            )
-
-        # scale
-        if scaled:
-            x_opt = scale_value_dict(x_opt, problem)
-        return x_opt
+    def get_for_id(self, inner_parameter_id: str) -> InnerParameter:
+        """Get InnerParameter for the given parameter ID."""
+        try:
+            return self.xs[inner_parameter_id]
+        except KeyError:
+            raise KeyError(f"Cannot find parameter with id {id}.")
+
+    def is_empty(self) -> bool:
+        """Check for emptiness.
+
+        Returns
+        -------
+        ``True`` if there aren't any parameters associated with this problem,
+        ``False`` otherwise.
+        """
+        return len(self.xs) == 0
 
+    def get_bounds(self) -> tuple[np.ndarray, np.ndarray]:
+        """Get bounds of inner parameters."""
+        lb = np.asarray([x.lb for x in self.xs.values()])
+        ub = np.asarray([x.ub for x in self.xs.values()])
+        return lb, ub
+
+    def get_interpretable_x_bounds(self) -> tuple[np.ndarray, np.ndarray]:
+        """Get bounds of interpretable inner parameters."""
+        interpretable_x_ids = self.get_interpretable_x_ids()
+        lb = np.asarray(
+            [
+                x.lb
+                for x in self.xs.values()
+                if x.inner_parameter_id in interpretable_x_ids
+            ]
+        )
+        ub = np.asarray(
+            [
+                x.ub
+                for x in self.xs.values()
+                if x.inner_parameter_id in interpretable_x_ids
+            ]
+        )
+        return lb, ub
 
-class NumericalInnerSolver(InnerSolver):
-    """Solve the inner subproblem numerically.
 
-    Advantage: The structure of the subproblem does not matter like, at all.
-    Disadvantage: Slower.
+class AmiciInnerProblem(InnerProblem):
+    """
+    Inner optimization problem in hierarchical optimization.
 
-    Special features: We cache the best parameters, which substantially
-    speeds things up.
+    For use with AMICI objects.
 
     Attributes
     ----------
-    minimize_kwargs:
-        Passed to the `pypesto.optimize.minimize` call.
-    n_cached:
-        Number of optimized parameter vectors to save.
-    problem_kwargs:
-        Passed to the `pypesto.Problem` constructor.
-    x_guesses:
-        Cached optimized parameter vectors, supplied as guesses to the next
-        `solve` call.
+    edatas:
+        AMICI ``ExpDataView``s for each simulation condition.
     """
 
-    def __init__(
-        self,
-        minimize_kwargs: Dict[str, Any] = None,
-        n_cached: int = 1,
-        problem_kwargs: Dict[str, Any] = None,
-    ):
-        self.minimize_kwargs = minimize_kwargs
-        if self.minimize_kwargs is None:
-            self.minimize_kwargs = {}
-        self.n_cached = n_cached
-        self.problem_kwargs = problem_kwargs
-        if self.problem_kwargs is None:
-            self.problem_kwargs = {}
+    def __init__(self, edatas: list[amici.ExpData], **kwargs):
+        super().__init__(**kwargs)
 
-        self.minimize_kwargs['n_starts'] = self.minimize_kwargs.get(
-            'n_starts', 1
-        )
-        self.minimize_kwargs['progress_bar'] = self.minimize_kwargs.get(
-            'progress_bar', False
-        )
+    def check_edatas(self, edatas: list[amici.ExpData]) -> bool:
+        """Check for consistency in data.
 
-        self.x_guesses = None
-        self.dummy_lb = -1e20
-        self.dummy_ub = +1e20
-
-    def initialize(self):
-        """(Re-)initialize the solver."""
-        self.x_guesses = None
-
-    def solve(
-        self,
-        problem: InnerProblem,
-        sim: List[np.ndarray],
-        sigma: List[np.ndarray],
-        scaled: bool,
-    ) -> Dict[str, float]:
-        """Solve the subproblem numerically.
+        Currently only checks for the actual data values. e.g., timepoints are
+        not compared.
 
         Parameters
         ----------
-        problem:
-            The inner problem to solve.
-        sim:
-            List of model output matrices, as provided in AMICI's
-            ``ReturnData.y``. Same order as simulations in the
-            PEtab problem.
-        sigma:
-            List of sigma matrices from the model, as provided in AMICI's
-            ``ReturnData.sigmay``. Same order as simulations in the
-            PEtab problem.
-        scale:
-            Whether to scale the results to the parameter scale specified in
-            ``problem``.
+        edatas:
+            A data set. Will be checked against the data set provided to the
+            constructor.
+
+        Returns
+        -------
+        Whether the data sets are consistent.
         """
-        pars = problem.xs.values()
-        # We currently cannot handle constraints on inner parameters correctly,
-        # and would have to assume [-inf, inf]. However, this may not be
-        # supported by all inner optimizers, so we go for some (arbitrary)
-        # large value.
-        lb = np.array(
-            [
-                0
-                if x.inner_parameter_type == InnerParameterType.SIGMA
-                else self.dummy_lb
-                for x in pars
-            ]
-        )
-
-        ub = np.full(shape=len(pars), fill_value=self.dummy_ub)
-
-        x_names = [x.inner_parameter_id for x in pars]
-        data = problem.data
-
-        # objective function
-        def fun(x):
-            _sim = copy.deepcopy(sim)
-            _sigma = copy.deepcopy(sigma)
-            _data = copy.deepcopy(data)
-            for x_val, par in zip(x, pars):
-                mask = par.ixs
-                if par.inner_parameter_type == InnerParameterType.OFFSET:
-                    apply_offset(x_val, _data, mask)
-                elif par.inner_parameter_type == InnerParameterType.SCALING:
-                    apply_scaling(x_val, _sim, mask)
-                elif par.inner_parameter_type == InnerParameterType.SIGMA:
-                    apply_sigma(x_val, _sigma, mask)
-                else:
-                    raise ValueError(
-                        "Can't handle parameter type "
-                        f"`{par.inner_parameter_type}`."
-                    )
-
-            return compute_nllh(_data, _sim, _sigma)
-
-        # TODO gradient
-        objective = Objective(fun)
-
-        # optimization problem
-        pypesto_problem = Problem(
-            objective, lb=lb, ub=ub, x_names=x_names, **self.problem_kwargs
-        )
-
-        if self.x_guesses is not None:
-            pypesto_problem.set_x_guesses(
-                self.x_guesses[:, pypesto_problem.x_free_indices]
-            )
-        else:
-            pypesto_problem.set_x_guesses(
-                [list(problem.get_dummy_values(scaled=False).values())]
-            )
+        # TODO replace but edata1==edata2 once this makes it into amici
+        #  https://github.com/AMICI-dev/AMICI/issues/1880
+        data = [
+            amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
+        ]
+
+        if len(self.data) != len(data):
+            return False
+
+        for data0, data1 in zip(self.data, data):
+            if not np.array_equal(data0, data1, equal_nan=True):
+                return False
+
+        return True
+
+
+def scale_value_dict(
+    dct: dict[str, float], problem: InnerProblem
+) -> dict[str, float]:
+    """Scale a value dictionary."""
+    scaled_dct = {}
+    for key, val in dct.items():
+        x = problem.get_for_id(key)
+        scaled_dct[key] = scale_value(val, x.scale)
+    return scaled_dct
+
+
+def scale_value(
+    val: Union[float, np.array], scale: str
+) -> Union[float, np.array]:
+    """Scale a single value."""
+    if scale == 'lin':
+        return val
+    if scale == 'log':
+        return np.log(val)
+    if scale == 'log10':
+        return np.log10(val)
+    raise ValueError(f"Scale {scale} not recognized.")
+
+
+def ix_matrices_from_arrays(
+    ixs: dict[str, list[tuple[int, int, int]]], edatas: list[np.array]
+) -> dict[str, list[np.array]]:
+    """
+    Convert mapping of parameters to measurements to matrix form.
 
-        # perform the actual optimization
-        result = minimize(pypesto_problem, **self.minimize_kwargs)
+    Returns
+    -------
+    A dictionary mapping parameter ID to a list of Boolean matrices, one per
+    simulation condition. Therein, ``True`` indicates that the respective
+    parameter is used for the model output at the respective timepoint,
+    observable and condition index.
+    """
+    ix_matrices = {
+        id: [np.zeros_like(edata, dtype=bool) for edata in edatas]
+        for id in ixs
+    }
+    for id, arr in ixs.items():
+        matrices = ix_matrices[id]
+        for condition_ix, time_ix, observable_ix in arr:
+            matrices[condition_ix][time_ix, observable_ix] = True
+    return ix_matrices
 
-        best_par = result.optimize_result.list[0]['x']
 
-        if (np.isclose(best_par, lb) | np.isclose(best_par, ub)).any():
-            raise RuntimeError(
-                "Active bounds in inner problem optimization. This can result "
-                "in incorrect gradient computation for the outer parameters."
-            )
+def _get_timepoints_with_replicates(
+    measurement_df: pd.DataFrame,
+) -> list[float]:
+    """
+    Get list of timepoints including replicate measurements.
 
-        x_opt = dict(zip(pypesto_problem.x_names, best_par))
+    :param measurement_df:
+        PEtab measurement table subset for a single condition.
 
-        # cache
-        self.x_guesses = np.array(
-            [
-                entry['x']
-                for entry in result.optimize_result.list[: self.n_cached]
-            ]
-        )
+    :return:
+        Sorted list of timepoints, including multiple timepoints accounting
+        for replicate measurements.
+    """
+    # create sorted list of all timepoints for which measurements exist
+    timepoints = sorted(measurement_df[TIME].unique().astype(float))
 
-        # scale
-        if scaled:
-            x_opt = scale_value_dict(x_opt, problem)
+    # find replicate numbers of time points
+    timepoints_w_reps = []
+    for time in timepoints:
+        # subselect for time
+        df_for_time = measurement_df[measurement_df.time == time]
+        # rep number is maximum over rep numbers for observables
+        n_reps = max(df_for_time.groupby([OBSERVABLE_ID, TIME]).size())
+        # append time point n_rep times
+        timepoints_w_reps.extend([time] * n_reps)
 
-        return x_opt
+    return timepoints_w_reps
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/spline_approximation/__init__.py` & `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """
-Spline approximation
-====================
+Semi-quantitative data integration
+==================================
 
-Contains the implementation of a spline approximation approach, applied for integration
-of nonlinear-monotone data in ODE modeling, where the data is assumed to have
-an unknown monotone relationship with the model output. This relationship is
-approximated by a piecewise linear (spline) function, which is numerically
-optimized to fit the data. This constitutes the inner subproblem of the
-hierarchical optimization problem.
+Contains the implementation of a spline approximation approach, applied for
+integration of semi-quantitative data in ODE modeling, where the data is
+assumed to have an unknown monotone relationship with the model output. This
+relationship is approximated by a piecewise linear (spline) function, which
+is numerically optimized to fit the data. This constitutes the inner subproblem
+of the hierarchical optimization problem.
+
+An example of parameter estimation with semi-quantitative data
+can be found in pypesto/doc/examples/semiquantitative_data.ipynb.
 """
 
-from .calculator import SplineAmiciCalculator
+from .calculator import SemiquantCalculator
 from .parameter import SplineInnerParameter
-from .problem import SplineInnerProblem
-from .solver import SplineInnerSolver
+from .problem import SemiquantProblem
+from .solver import SemiquantInnerSolver
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/spline_approximation/calculator.py` & `pypesto-0.4.2/pypesto/objective/amici/amici_calculator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,71 @@
-import copy
-from typing import Dict, List, Sequence, Tuple
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Dict, List, Sequence, Tuple, Union
 
 import numpy as np
 
 from ...C import (
-    AMICI_SIGMAY,
-    AMICI_SSIGMAY,
-    AMICI_SY,
-    AMICI_Y,
     FVAL,
     GRAD,
     HESS,
-    INNER_PARAMETERS,
+    MODE_FUN,
     MODE_RES,
     RDATAS,
     RES,
     SRES,
-    X_INNER_OPT,
-)
-from ...objective.amici.amici_calculator import (
-    AmiciCalculator,
-    AmiciModel,
-    AmiciSolver,
+    ModeType,
 )
-from ...objective.amici.amici_util import (
+from .amici_util import (
+    add_sim_grad_to_opt_grad,
+    add_sim_hess_to_opt_hess,
     filter_return_dict,
+    get_error_output,
     init_return_values,
+    log_simulation,
+    sim_sres_to_opt_sres,
 )
-from .problem import SplineInnerProblem
-from .solver import SplineInnerSolver
-
-try:
-    import amici
-    from amici.parameter_mapping import ParameterMapping
-except ImportError:
-    pass
-
 
-class SplineAmiciCalculator(AmiciCalculator):
-    """A calculator is passed as `calculator` to the pypesto.AmiciObjective.
+if TYPE_CHECKING:
+    try:
+        import amici
+        from amici.parameter_mapping import ParameterMapping
+    except ImportError:
+        ParameterMapping = None
+
+AmiciModel = Union['amici.Model', 'amici.ModelPtr']
+AmiciSolver = Union['amici.Solver', 'amici.SolverPtr']
 
-    The object is called by :func:`pypesto.AmiciObjective.call_unprocessed`
-    to calculate the current objective function values and gradient.
-    """
 
-    def __init__(
-        self,
-        inner_problem: SplineInnerProblem,
-        inner_solver: SplineInnerSolver = None,
-    ):
-        """Initialize the calculator from the given problem.
+class AmiciCalculator:
+    """Class to perform the AMICI call and obtain objective function values."""
 
-        Parameters
-        ----------
-        inner_problem:
-            The optimal scaling inner problem.
-        inner_solver:
-            A solver to solve ``inner_problem``.
-            Defaults to ``SplineInnerSolver``.
-        """
-        super().__init__()
-        self.inner_problem = inner_problem
-
-        if inner_solver is None:
-            inner_solver = SplineInnerSolver()
-        self.inner_solver = inner_solver
+    def __init__(self):
+        self._known_least_squares_safe = False
 
     def initialize(self):
-        """Initialize."""
-        self.inner_solver.initialize()
-        self.inner_problem.initialize()
-
-    def get_inner_parameter_ids(self) -> List[str]:
-        """Get the ids of the inner parameters."""
-        return self.inner_problem.get_x_ids()
+        """Initialize the calculator. Default: Do nothing."""
 
     def __call__(
         self,
         x_dct: Dict,
-        sensi_orders: Tuple[int, ...],
-        mode: str,
+        sensi_orders: Tuple[int],
+        mode: ModeType,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
-        edatas: List['amici.ExpData'],
+        edatas: List[amici.ExpData],
         n_threads: int,
         x_ids: Sequence[str],
         parameter_mapping: ParameterMapping,
         fim_for_hess: bool,
-        rdatas: List['amici.ReturnData'] = None,
     ):
         """Perform the actual AMICI call.
 
+        Called within the :func:`AmiciObjective.__call__` method.
+
         Parameters
         ----------
         x_dct:
             Parameters for which to compute function value and derivatives.
         sensi_orders:
             Tuple of requested sensitivity orders.
         mode:
@@ -110,125 +81,180 @@
         x_ids:
             Ids of optimization parameters.
         parameter_mapping:
             Mapping of optimization to simulation parameters.
         fim_for_hess:
             Whether to use the FIM (if available) instead of the Hessian (if
             requested).
-        rdatas:
-            AMICI simulation return data. In case the calculator is part of
-            the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
-            it will already simulate the model and pass the results here.
-
-
-        Returns
-        -------
-        inner_result:
-            A dict containing the calculation results: FVAL, GRAD, RDATAS and X_INNER_OPT.
         """
-        if mode == MODE_RES:
-            raise ValueError(
-                "Spline approximation cannot be called with residual mode."
-            )
-        if 2 in sensi_orders:
-            raise ValueError(
-                "Hessian and FIM are not implemented for the spline calculator."
-            )
-
-        # get dimension of outer problem
-        dim = len(x_ids)
-
-        # initialize return values
-        nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
-            sensi_orders, mode, dim
-        )
+        import amici.parameter_mapping
+
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
-        # If AMICI ReturnData is not provided, we need to simulate the model
-
-        if rdatas is None:
+        if sensi_order == 2 and fim_for_hess:
+            # we use the FIM
+            amici_solver.setSensitivityOrder(sensi_order - 1)
+        else:
             amici_solver.setSensitivityOrder(sensi_order)
 
-            x_dct = copy.deepcopy(x_dct)
-            x_dct.update(
-                self.inner_problem.get_noise_dummy_values(scaled=True)
-            )
-
-            # fill in parameters
-            amici.parameter_mapping.fill_in_parameters(
-                edatas=edatas,
-                problem_parameters=x_dct,
-                scaled_parameters=True,
-                parameter_mapping=parameter_mapping,
-                amici_model=amici_model,
-            )
-            # run amici simulation
-            rdatas = amici.runAmiciSimulations(
-                amici_model,
-                amici_solver,
-                edatas,
-                num_threads=min(n_threads, len(edatas)),
-            )
-
-        inner_result = {
-            FVAL: nllh,
-            GRAD: snllh,
-            HESS: s2nllh,
-            RES: res,
-            SRES: sres,
-            RDATAS: rdatas,
-            X_INNER_OPT: self.inner_problem.get_inner_parameter_dictionary(),
-        }
-
-        # if any amici simulation failed, it's unlikely we can compute
-        # meaningful inner parameters, so we better just fail early.
-        if any(rdata.status != amici.AMICI_SUCCESS for rdata in rdatas):
-            inner_result[FVAL] = np.inf
-            # if the gradient was requested,
-            # we need to provide some value for it
-            if 1 in sensi_orders:
-                inner_result[GRAD] = np.full(
-                    shape=len(x_ids), fill_value=np.nan
+        # fill in parameters
+        amici.parameter_mapping.fill_in_parameters(
+            edatas=edatas,
+            problem_parameters=x_dct,
+            scaled_parameters=True,
+            parameter_mapping=parameter_mapping,
+            amici_model=amici_model,
+        )
+
+        # run amici simulation
+        rdatas = amici.runAmiciSimulations(
+            amici_model,
+            amici_solver,
+            edatas,
+            num_threads=min(n_threads, len(edatas)),
+        )
+        if (
+            not self._known_least_squares_safe
+            and mode == MODE_RES
+            and 1 in sensi_orders
+        ):
+            if not amici_model.getAddSigmaResiduals() and any(
+                (
+                    (r['ssigmay'] is not None and np.any(r['ssigmay']))
+                    or (r['ssigmaz'] is not None and np.any(r['ssigmaz']))
+                )
+                for r in rdatas
+            ):
+                raise RuntimeError(
+                    'Cannot use least squares solver with'
+                    'parameter dependent sigma! Support can be '
+                    'enabled via '
+                    'amici_model.setAddSigmaResiduals().'
                 )
-            return filter_return_dict(inner_result)
+            self._known_least_squares_safe = True  # don't check this again
+
+        return calculate_function_values(
+            rdatas=rdatas,
+            sensi_orders=sensi_orders,
+            mode=mode,
+            amici_model=amici_model,
+            amici_solver=amici_solver,
+            edatas=edatas,
+            x_ids=x_ids,
+            parameter_mapping=parameter_mapping,
+            fim_for_hess=fim_for_hess,
+        )
 
-        sim = [rdata[AMICI_Y] for rdata in rdatas]
-        sigma = [rdata[AMICI_SIGMAY] for rdata in rdatas]
 
-        # Clip negative simulation values to zero, to avoid numerical issues.
-        for i in range(len(sim)):
-            sim[i] = sim[i].clip(min=0)
-
-        # compute optimal inner parameters
-        x_inner_opt = self.inner_solver.solve(self.inner_problem, sim, sigma)
-        inner_result[FVAL] = self.inner_solver.calculate_obj_function(
-            x_inner_opt
+def calculate_function_values(
+    rdatas,
+    sensi_orders: Tuple[int, ...],
+    mode: ModeType,
+    amici_model: AmiciModel,
+    amici_solver: AmiciSolver,
+    edatas: List[amici.ExpData],
+    x_ids: Sequence[str],
+    parameter_mapping: ParameterMapping,
+    fim_for_hess: bool,
+):
+    """Calculate the function values from rdatas and return as dict."""
+    import amici
+
+    # full optimization problem dimension (including fixed parameters)
+    dim = len(x_ids)
+
+    # check if the simulation failed
+    if any(rdata['status'] < 0.0 for rdata in rdatas):
+        return get_error_output(
+            amici_model, edatas, rdatas, sensi_orders, mode, dim
         )
-        inner_result[
-            X_INNER_OPT
-        ] = self.inner_problem.get_inner_parameter_dictionary()
-
-        inner_result[
-            INNER_PARAMETERS
-        ] = self.inner_problem.get_inner_noise_parameter_dictionary()
-
-        # Calculate analytical gradients if requested
-        if sensi_order > 0:
-            sy = [rdata[AMICI_SY] for rdata in rdatas]
-            ssigma = [rdata[AMICI_SSIGMAY] for rdata in rdatas]
-            inner_result[GRAD] = self.inner_solver.calculate_gradients(
-                problem=self.inner_problem,
-                x_inner_opt=x_inner_opt,
-                sim=sim,
-                amici_sigma=sigma,
-                sy=sy,
-                amici_ssigma=ssigma,
-                parameter_mapping=parameter_mapping,
-                par_opt_ids=x_ids,
-                par_sim_ids=amici_model.getParameterIds(),
-                snllh=snllh,
-            )
 
-        return filter_return_dict(inner_result)
+    nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
+        sensi_orders, mode, dim
+    )
+
+    par_sim_ids = list(amici_model.getParameterIds())
+    sensi_method = amici_solver.getSensitivityMethod()
+
+    # iterate over return data
+    for data_ix, rdata in enumerate(rdatas):
+        log_simulation(data_ix, rdata)
+
+        condition_map_sim_var = parameter_mapping[data_ix].map_sim_var
+
+        # add objective value
+        nllh -= rdata['llh']
+
+        if mode == MODE_FUN:
+            if not np.isfinite(nllh):
+                return get_error_output(
+                    amici_model, edatas, rdatas, sensi_orders, mode, dim
+                )
+
+            if 1 in sensi_orders:
+                # add gradient
+                add_sim_grad_to_opt_grad(
+                    x_ids,
+                    par_sim_ids,
+                    condition_map_sim_var,
+                    rdata['sllh'],
+                    snllh,
+                    coefficient=-1.0,
+                )
+
+                if not np.isfinite(snllh).all():
+                    return get_error_output(
+                        amici_model, edatas, rdatas, sensi_orders, mode, dim
+                    )
+
+                # Hessian
+            if 2 in sensi_orders:
+                if (
+                    sensi_method != amici.SensitivityMethod_forward
+                    or not fim_for_hess
+                ):
+                    raise ValueError("AMICI cannot compute Hessians yet.")
+                    # add FIM for Hessian
+                add_sim_hess_to_opt_hess(
+                    x_ids,
+                    par_sim_ids,
+                    condition_map_sim_var,
+                    rdata['FIM'],
+                    s2nllh,
+                    coefficient=+1.0,
+                )
+                if not np.isfinite(s2nllh).all():
+                    return get_error_output(
+                        amici_model, edatas, rdatas, sensi_orders, mode, dim
+                    )
+
+        elif mode == MODE_RES:
+            if 0 in sensi_orders:
+                chi2 += rdata['chi2']
+                res = (
+                    np.hstack([res, rdata['res']])
+                    if res.size
+                    else rdata['res']
+                )
+            if 1 in sensi_orders:
+                opt_sres = sim_sres_to_opt_sres(
+                    x_ids,
+                    par_sim_ids,
+                    condition_map_sim_var,
+                    rdata['sres'],
+                    coefficient=1.0,
+                )
+                sres = np.vstack([sres, opt_sres]) if sres.size else opt_sres
+
+    ret = {
+        FVAL: nllh,
+        GRAD: snllh,
+        HESS: s2nllh,
+        RES: res,
+        SRES: sres,
+        RDATAS: rdatas,
+    }
+
+    return filter_return_dict(ret)
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/spline_approximation/parameter.py` & `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 
 from ...C import InnerParameterType
-from ..parameter import InnerParameter
+from ..base_parameter import InnerParameter
 
 logger = logging.getLogger(__name__)
 
 
 class SplineInnerParameter(InnerParameter):
     """A spline (inner) parameter of the spline hierarchical optimization problem.
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/spline_approximation/problem.py` & `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/problem.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-from typing import Dict, List, Tuple
-
 import numpy as np
 import pandas as pd
 
 from ...C import (
     CURRENT_SIMULATION,
     DATAPOINTS,
     EXPDATA_MASK,
     INNER_NOISE_PARS,
     INNER_PARAMETER_BOUNDS,
     LIN,
     MAX_DATAPOINT,
     MEASUREMENT_TYPE,
     MIN_DATAPOINT,
     N_SPLINE_PARS,
-    NONLINEAR_MONOTONE,
     NUM_DATAPOINTS,
     OPTIMIZE_NOISE,
     PARAMETER_TYPE,
+    SEMIQUANTITATIVE,
     SPLINE_PAR_TYPE,
     TIME,
     InnerParameterType,
 )
-from ..problem import (
-    InnerProblem,
+from ..base_problem import (
+    AmiciInnerProblem,
     _get_timepoints_with_replicates,
     ix_matrices_from_arrays,
     scale_value,
 )
 from .parameter import SplineInnerParameter
 
 try:
@@ -41,38 +39,43 @@
         PARAMETER_ID,
         UPPER_BOUND,
     )
 except ImportError:
     pass
 
 
-class SplineInnerProblem(InnerProblem):
-    """Inner optimization problem for spline approximation.
+class SemiquantProblem(AmiciInnerProblem):
+    r"""Inner optimization problem for semi-quantitative data.
+
+    The inner problem for semi-quantitative data consists of spline parameters
+    and noise parameters for semi-quantitative observables. The unknown
+    nonlinear measurement mapping is estimated using a piece-wise linear spline.
 
     Attributes
     ----------
     xs:
         Mapping of (inner) parameter ID to ``InnerParameters``.
     data:
         Measurement data. One matrix (`num_timepoints` x `num_observables`)
         per simulation condition. Missing observations as NaN.
+    edatas:
+        AMICI ``ExpData``\s for each simulation condition.
     groups:
         A dictionary of the groups of the subproblem.
     spline_ratio:
         The ratio of the number of spline inner parameters and number of measurements for each group.
     """
 
     def __init__(
         self,
-        xs: List[SplineInnerParameter],
-        data: List[np.ndarray],
         spline_ratio: float = 0.5,
+        **kwargs,
     ):
         """Construct."""
-        super().__init__(xs, data)
+        super().__init__(**kwargs)
         self.spline_ratio = spline_ratio
 
         if spline_ratio <= 0:
             raise ValueError("Spline ratio must be a positive float.")
         self._initialize_groups()
 
     def _initialize_groups(self) -> None:
@@ -118,176 +121,186 @@
             )
             self.groups[group][INNER_NOISE_PARS] = 1
 
     @staticmethod
     def from_petab_amici(
         petab_problem: petab.Problem,
         amici_model: 'amici.Model',
-        edatas: List['amici.ExpData'],
+        edatas: list['amici.ExpData'],
         spline_ratio: float = None,
-    ) -> 'SplineInnerProblem':
+    ) -> 'SemiquantProblem':
         """Construct the inner problem from the `petab_problem`."""
         if spline_ratio is None:
             spline_ratio = get_default_options()
         return spline_inner_problem_from_petab_problem(
             petab_problem, amici_model, edatas, spline_ratio
         )
 
-    def get_groups_for_xs(self, inner_parameter_type: str) -> List[int]:
+    def get_interpretable_x_ids(self) -> list[str]:
+        """Get IDs of interpretable inner parameters.
+
+        The interpretable inner parameters of the semiquantitative
+        problem are the noise parameters.
+        """
+        return [
+            x.inner_parameter_id
+            for x in self.xs.values()
+            if x.inner_parameter_type == InnerParameterType.SIGMA
+        ]
+
+    def get_groups_for_xs(self, inner_parameter_type: str) -> list[int]:
         """Get unique list of ``SplineParameter.group`` values."""
         groups = [x.group for x in self.get_xs_for_type(inner_parameter_type)]
         return list(set(groups))
 
-    def get_xs_for_group(self, group: int) -> List[SplineInnerParameter]:
+    def get_xs_for_group(self, group: int) -> list[SplineInnerParameter]:
         r"""Get ``SplineParameter``\s that belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group
             and x.inner_parameter_type == InnerParameterType.SPLINE
         ]
 
-    def get_free_xs_for_group(self, group: int) -> List[SplineInnerParameter]:
+    def get_free_xs_for_group(self, group: int) -> list[SplineInnerParameter]:
         r"""Get ``SplineParameter``\s that are free and belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group
             and x.estimate is True
             and x.inner_parameter_type == InnerParameterType.SPLINE
         ]
 
-    def get_fixed_xs_for_group(self, group: int) -> List[SplineInnerParameter]:
+    def get_fixed_xs_for_group(self, group: int) -> list[SplineInnerParameter]:
         r"""Get ``SplineParameter``\s that are fixed and belong to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group
             and x.estimate is False
             and x.inner_parameter_type == InnerParameterType.SPLINE
         ]
 
+    def get_inner_noise_parameters(self) -> list[float]:
+        """Get a list with all noise parameter values."""
+        return [
+            x.value for x in self.get_xs_for_type(InnerParameterType.SIGMA)
+        ]
+
     def get_noise_parameters_for_group(
         self, group: int
     ) -> SplineInnerParameter:
         r"""Get the ``SplineParameter``\ that is a noise parameters and belongs to the given group."""
         return [
             x
             for x in self.xs.values()
             if x.group == group
             and x.inner_parameter_type == InnerParameterType.SIGMA
         ]
 
-    def get_inner_parameter_dictionary(self) -> Dict:
+    def get_inner_parameter_dictionary(self) -> dict:
         """Get a dictionary with all inner parameter ids and their values."""
         inner_par_dict = {}
         for x_id, x in self.xs.items():
             inner_par_dict[x_id] = x.value
         return inner_par_dict
 
-    def get_inner_noise_parameter_dictionary(self) -> Dict:
-        """Get a dictionary with all noise inner parameter ids and their values."""
-        inner_par_dict = {}
-        for x in self.get_xs_for_type(InnerParameterType.SIGMA):
-            inner_par_dict[x.inner_parameter_id] = x.value
-        return inner_par_dict
-
     def get_measurements_for_group(self, gr) -> np.ndarray:
         """Get measurements for a group."""
         # Taking the ixs of first inner parameter since
         # all of them are the same for the same group.
         ixs = self.get_xs_for_group(gr)[0].ixs
 
         return np.concatenate(
             [
                 self.data[condition_index][ixs[condition_index]]
                 for condition_index in range(len(ixs))
             ]
         )
 
-    def get_noise_dummy_values(self, scaled: bool) -> Dict[str, float]:
-        """Get dummy values for noise parameters of the nonlinear-monotone observable."""
+    def get_noise_dummy_values(self, scaled: bool) -> dict[str, float]:
+        """Get dummy values for noise parameters of the semiquantitative observable."""
         return {
             x_id: scale_value(x.value, x.scale) if scaled else x.value
             for x_id, x in self.xs.items()
             if x.inner_parameter_type == InnerParameterType.SIGMA
         }
 
 
-def get_default_options() -> Dict:
+def get_default_options() -> dict:
     """Return the default spline problem options dictionary."""
     spline_ratio = 1 / 2
     return spline_ratio
 
 
 def spline_inner_problem_from_petab_problem(
     petab_problem: petab.Problem,
     amici_model: 'amici.Model',
-    edatas: List['amici.ExpData'],
+    edatas: list['amici.ExpData'],
     spline_ratio: float = None,
 ):
     """Construct the inner problem from the `petab_problem`."""
     if spline_ratio is None:
         spline_ratio = get_default_options()
     elif spline_ratio <= 0:
         raise ValueError("Spline ratio must be a positive float.")
 
     # inner parameters
     inner_parameters = spline_inner_parameters_from_measurement_df(
         petab_problem.measurement_df, spline_ratio, amici_model
     )
 
-    # noise parameters for nonlinear-monotone observables
+    # noise parameters for semiquantitative observables
     noise_parameters = noise_inner_parameters_from_parameter_df(
         petab_problem, amici_model
     )
     inner_parameters.extend(noise_parameters)
 
     # used indices for all measurement specific parameters
     ixs = spline_ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, inner_parameters
     )
 
     # transform experimental data
-    edatas = [
-        amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas
-    ]
+    data = [amici.numpy.ExpDataView(edata)['observedData'] for edata in edatas]
 
     # matrixify
-    ix_matrices = ix_matrices_from_arrays(ixs, edatas)
+    ix_matrices = ix_matrices_from_arrays(ixs, data)
 
     # assign matrices
     for par in inner_parameters:
         par.ixs = ix_matrices[par.inner_parameter_id]
 
-    return SplineInnerProblem(
-        inner_parameters,
-        edatas,
-        spline_ratio,
+    return SemiquantProblem(
+        xs=inner_parameters,
+        data=data,
+        edatas=edatas,
+        spline_ratio=spline_ratio,
     )
 
 
 def spline_inner_parameters_from_measurement_df(
     df: pd.DataFrame,
     spline_ratio: float,
     amici_model: 'amici.Model',
-) -> List[SplineInnerParameter]:
+) -> list[SplineInnerParameter]:
     """Create list of inner free spline parameters from PEtab measurement table."""
     df = df.reset_index()
 
     observable_ids = amici_model.getObservableIds()
 
     par_type = SPLINE_PAR_TYPE
     estimate = True
     lb, ub = INNER_PARAMETER_BOUNDS[InnerParameterType.SPLINE].values()
 
     inner_parameters = []
 
-    # Select the nonlinear monotone measurements.
-    df = df[df[MEASUREMENT_TYPE] == NONLINEAR_MONOTONE]
+    # Select the semiquantitative measurements.
+    df = df[df[MEASUREMENT_TYPE] == SEMIQUANTITATIVE]
 
     # Iterate over groups.
     for observable_id in observable_ids:
         group = observable_ids.index(observable_id) + 1
         df_for_group = df[df[OBSERVABLE_ID] == observable_id]
 
         n_spline_parameters = int(np.ceil(len(df_for_group) * spline_ratio))
@@ -313,20 +326,20 @@
 
     return inner_parameters
 
 
 def noise_inner_parameters_from_parameter_df(
     petab_problem: 'petab.Problem',
     amici_model: 'amici.Model',
-) -> List[SplineInnerParameter]:
+) -> list[SplineInnerParameter]:
     """Create list of inner free noise parameters from PEtab parameter table."""
-    # Select the nonlinear monotone measurements.
+    # Select the semiquantitative measurements.
     measurement_df = petab_problem.measurement_df
     measurement_df = measurement_df[
-        measurement_df[MEASUREMENT_TYPE] == NONLINEAR_MONOTONE
+        measurement_df[MEASUREMENT_TYPE] == SEMIQUANTITATIVE
     ]
 
     observable_ids = amici_model.getObservableIds()
 
     # Create a dictionary with unique pairs of observable id
     # and noise parameter from the measurement table.
     noise_parameter_to_observable = {}
@@ -363,16 +376,16 @@
 
     return noise_parameters
 
 
 def spline_ixs_for_measurement_specific_parameters(
     petab_problem: 'petab.Problem',
     amici_model: 'amici.Model',
-    inner_parameters: List[SplineInnerParameter],
-) -> Dict[str, List[Tuple[int, int, int]]]:
+    inner_parameters: list[SplineInnerParameter],
+) -> dict[str, list[tuple[int, int, int]]]:
     """Create mapping of parameters to measurements.
 
     Returns
     -------
     A dictionary mapping parameter ID to a list of
     `(condition index, time index, observable index)` tuples in which this
     output parameter is used. For each condition, the time index refers to
@@ -434,16 +447,16 @@
                     ixs_for_par.setdefault(override, []).append(
                         (condition_ix, time_w_reps_ix, observable_ix)
                     )
     return ixs_for_par
 
 
 def get_spline_inner_par_ids_for_measurement(
-    measurement: Dict,
-    inner_parameters: List[SplineInnerParameter],
+    measurement: dict,
+    inner_parameters: list[SplineInnerParameter],
 ):
     """Return inner parameter ids of parameters which are related to the measurement."""
     return [
         inner_par.inner_parameter_id
         for inner_par in inner_parameters
         if inner_par.observable_id == measurement[OBSERVABLE_ID]
     ]
```

### Comparing `pypesto-0.4.1/pypesto/hierarchical/spline_approximation/solver.py` & `pypesto-0.4.2/pypesto/hierarchical/semiquantitative/solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import warnings
-from typing import Dict, List
 
 import numpy as np
 from scipy.optimize import minimize
 
 from ...C import (
     CURRENT_SIMULATION,
     DATAPOINTS,
@@ -12,62 +11,77 @@
     MAX_DATAPOINT,
     MIN_DATAPOINT,
     MIN_DIFF_FACTOR,
     MIN_SIM_RANGE,
     N_SPLINE_PARS,
     NUM_DATAPOINTS,
     OPTIMIZE_NOISE,
+    REGULARIZATION_FACTOR,
+    REGULARIZE_SPLINE,
     SCIPY_FUN,
     SCIPY_SUCCESS,
     SCIPY_X,
     InnerParameterType,
 )
-from ..solver import InnerSolver
+from ..base_solver import InnerSolver
 from .parameter import SplineInnerParameter
-from .problem import SplineInnerProblem
+from .problem import SemiquantProblem
 
 try:
     from amici.parameter_mapping import ParameterMapping
 except ImportError:
     pass
 
 
-class SplineInnerSolver(InnerSolver):
+class SemiquantInnerSolver(InnerSolver):
     """Solver of the inner subproblem of spline approximation for nonlinear-monotone data.
 
     Options
     -------
     min_diff_factor:
         Determines the minimum difference between two consecutive spline
         as ``min_diff_factor * (measurement_range) / n_spline_pars``.
         Default is 1/2.
     """
 
-    def __init__(self, options: Dict = None):
+    def __init__(self, options: dict = None):
         self.options = {
             **self.get_default_options(),
             **(options or {}),
         }
         self.validate_options()
 
     def validate_options(self):
         """Validate the current options dictionary."""
         if type(self.options[MIN_DIFF_FACTOR]) is not float:
             raise TypeError(f"{MIN_DIFF_FACTOR} must be of type float.")
         elif self.options[MIN_DIFF_FACTOR] < 0:
-            raise ValueError(f"{MIN_DIFF_FACTOR} must be greater than zero.")
+            raise ValueError(f"{MIN_DIFF_FACTOR} must not be negative.")
+
+        elif type(self.options[REGULARIZE_SPLINE]) is not bool:
+            raise TypeError(f"{REGULARIZE_SPLINE} must be of type bool.")
+        if self.options[REGULARIZE_SPLINE]:
+            if type(self.options[REGULARIZATION_FACTOR]) is not float:
+                raise TypeError(
+                    f"{REGULARIZATION_FACTOR} must be of type float."
+                )
+            elif self.options[REGULARIZATION_FACTOR] < 0:
+                raise ValueError(
+                    f"{REGULARIZATION_FACTOR} must not be negative."
+                )
+
         for key in self.options:
             if key not in self.get_default_options():
                 raise ValueError(f"Unknown SplineInnerSolver option {key}.")
 
     def solve(
         self,
-        problem: SplineInnerProblem,
-        sim: List[np.ndarray],
-        amici_sigma: List[np.ndarray],
+        problem: SemiquantProblem,
+        sim: list[np.ndarray],
+        amici_sigma: list[np.ndarray],
     ) -> list:
         """Get results for every group (inner optimization problem).
 
         Parameters
         ----------
         problem:
             InnerProblem from pyPESTO hierarchical.
@@ -82,38 +96,26 @@
         """
         inner_results = []
         for group in problem.get_groups_for_xs(InnerParameterType.SPLINE):
             group_dict = problem.groups[group]
             group_dict[CURRENT_SIMULATION] = extract_expdata_using_mask(
                 expdata=sim, mask=group_dict[EXPDATA_MASK]
             )
-            # Optimize the spline for this group.
-            inner_result_for_group = self._optimize_spline(
-                inner_parameters=problem.get_free_xs_for_group(group),
-                group_dict=group_dict,
-            )
 
-            # If the parameters are optimized in the inner problem, we
-            # calculate the sigma analytically from the inner result.
-            if group_dict[OPTIMIZE_NOISE]:
-                group_dict[INNER_NOISE_PARS] = _calculate_sigma_for_group(
-                    inner_result=inner_result_for_group,
-                    n_datapoints=group_dict[NUM_DATAPOINTS],
-                )
-            # Otherwise, we extract the sigma from the AMICI noise parameters.
-            else:
+            # If the noise parameters are optimized in the outer problem,
+            # extract them from amici return data.
+            if not group_dict[OPTIMIZE_NOISE]:
                 group_dict[INNER_NOISE_PARS] = extract_expdata_using_mask(
                     expdata=amici_sigma, mask=group_dict[EXPDATA_MASK]
                 )[0]
 
-            # Apply sigma to inner result.
-            inner_result_for_group = _calculate_nllh_for_group(
-                inner_result=inner_result_for_group,
-                sigma=group_dict[INNER_NOISE_PARS],
-                n_datapoints=group_dict[NUM_DATAPOINTS],
+            # Optimize the spline for this group.
+            inner_result_for_group = self._optimize_spline(
+                inner_parameters=problem.get_free_xs_for_group(group),
+                group_dict=group_dict,
             )
 
             inner_results.append(inner_result_for_group)
             save_inner_parameters_to_inner_problem(
                 inner_problem=problem,
                 s=inner_result_for_group[SCIPY_X],
                 group=group,
@@ -148,24 +150,25 @@
                     for idx in range(len(x_inner_opt))
                 ]
             )
         return obj
 
     def calculate_gradients(
         self,
-        problem: SplineInnerProblem,
-        x_inner_opt: List[Dict],
-        sim: List[np.ndarray],
-        amici_sigma: List[np.ndarray],
-        sy: List[np.ndarray],
-        amici_ssigma: List[np.ndarray],
+        problem: SemiquantProblem,
+        x_inner_opt: list[dict],
+        sim: list[np.ndarray],
+        amici_sigma: list[np.ndarray],
+        sy: list[np.ndarray],
+        amici_ssigma: list[np.ndarray],
         parameter_mapping: ParameterMapping,
-        par_opt_ids: List,
-        par_sim_ids: List,
-        snllh: Dict,
+        par_opt_ids: list,
+        par_sim_ids: list,
+        par_edatas_indices: list,
+        snllh: np.ndarray,
     ):
         """Calculate gradients of the inner objective function.
 
         Calculates gradients of the objective function with respect to outer
         (dynamical) parameters.
 
         Parameters
@@ -183,53 +186,59 @@
         parameter_mapping:
             Mapping of optimization to simulation parameters.
         par_opt_ids:
             Ids of outer otimization parameters.
         par_sim_ids:
             Ids of outer simulation parameters, includes fixed parameters.
         snllh:
-            Empty dictionary with optimization parameters as keys.
+            A zero-initialized vector of the same length as ``par_opt_ids`` to store the
+            gradients in. Will be modified in-place.
 
         Returns
         -------
-        Filled in snllh dictionary with objective function gradients.
+        The gradients with respect to the outer parameters.
         """
         already_calculated = set()
 
         for condition_map_sim_var in [
             cond_par_map.map_sim_var for cond_par_map in parameter_mapping
         ]:
             for par_sim, par_opt in condition_map_sim_var.items():
                 if (
                     not isinstance(par_opt, str)
                     or par_opt in already_calculated
                 ):
                     continue
-                # Current fix for scaling/offset parameters in models.
-                elif par_sim.startswith('observableParameter'):
-                    continue
-                # For noise parameters optimized hierarchically, we
-                # do not calculate the gradient.
-                elif (
-                    par_sim.startswith('noiseParameter')
-                    and par_opt not in par_opt_ids
-                ):
+                elif par_opt not in par_opt_ids:
                     continue
                 else:
                     already_calculated.add(par_opt)
                 par_sim_idx = par_sim_ids.index(par_sim)
                 par_opt_idx = par_opt_ids.index(par_opt)
                 grad = 0.0
 
                 sy_for_outer_parameter = [
-                    sy_cond[:, par_sim_idx, :] for sy_cond in sy
+                    (
+                        sy_cond[:, par_edata_indices.index(par_sim_idx), :]
+                        if par_sim_idx in par_edata_indices
+                        else np.zeros(sy_cond[:, 0, :].shape)
+                    )
+                    for sy_cond, par_edata_indices in zip(
+                        sy, par_edatas_indices
+                    )
                 ]
                 ssigma_for_outer_parameter = [
-                    ssigma_cond[:, par_sim_idx, :]
-                    for ssigma_cond in amici_ssigma
+                    (
+                        ssigma_cond[:, par_edata_indices.index(par_sim_idx), :]
+                        if par_sim_idx in par_edata_indices
+                        else np.zeros(ssigma_cond[:, 0, :].shape)
+                    )
+                    for ssigma_cond, par_edata_indices in zip(
+                        amici_ssigma, par_edatas_indices
+                    )
                 ]
 
                 for group_idx, group in enumerate(
                     problem.get_groups_for_xs(InnerParameterType.SPLINE)
                 ):
                     # Get the reformulated spline parameters
                     s = np.asarray(x_inner_opt[group_idx][SCIPY_X])
@@ -252,26 +261,30 @@
 
                     delta_c, c, n = self._rescale_spline_bases(
                         sim_all=sim_all, N=N, K=K
                     )
                     delta_c_dot, c_dot = calculate_spline_bases_gradient(
                         sim_all=sim_all, sy_all=sy_all, N=N
                     )
-                    C = np.diag(-np.ones(N))
 
                     # For the reformulated problem, mu can be calculated
                     # as the inner gradient at the optimal point s.
-                    mu = calculate_inner_gradient_for_obs(
+                    mu = _calculate_nllh_gradient_for_group(
                         s=s,
                         sim_all=sim_all,
                         measurements=measurements,
                         N=N,
                         delta_c=delta_c,
                         c=c,
                         n=n,
+                        regularization_factor=self.options[
+                            REGULARIZATION_FACTOR
+                        ],
+                        regularize_spline=self.options[REGULARIZE_SPLINE],
+                        group_dict=group_dict,
                     )
                     min_meas = group_dict[MIN_DATAPOINT]
                     max_meas = group_dict[MAX_DATAPOINT]
                     min_diff = self._get_minimal_difference(
                         measurement_range=max_meas - min_meas,
                         N=N,
                         min_diff_factor=self.options[MIN_DIFF_FACTOR],
@@ -279,163 +292,146 @@
 
                     # If the spline parameter is at its boundary, the
                     # corresponding Lagrangian multiplier mu is set to 0.
                     min_diff_all = np.full(N, min_diff)
                     min_diff_all[0] = 0.0
                     mu = np.asarray(
                         [
-                            mu[i]
-                            if np.isclose(s[i] - min_diff_all[i], 0)
-                            else 0
+                            (
+                                mu[i]
+                                if np.isclose(s[i] - min_diff_all[i], 0)
+                                else 0
+                            )
                             for i in range(len(s))
                         ]
                     )
 
-                    # Calculate (dJ_ds * ds_dtheta) term only if mu is not all 0
-                    ds_grad_term = 0.0
-                    if np.any(mu):
-                        s_dot = calculate_ds_dtheta(
-                            sim_all=sim_all,
-                            sy_all=sy_all,
-                            measurements=measurements,
-                            s=s,
-                            C=C,
-                            mu=mu,
-                            N=N,
-                            delta_c=delta_c,
-                            delta_c_dot=delta_c_dot,
-                            c=c,
-                            c_dot=c_dot,
-                            n=n,
-                            min_diff=min_diff,
-                        )
-                        dres_ds = mu
-                        ds_grad_term = dres_ds.dot(s_dot)
-
-                    # Let's calculate the (dJ_dy * dy_dtheta) term now:
+                    # Calculate the (dJ_dy * dy_dtheta) term:
                     dy_grad_term = calculate_dy_term(
                         sim_all=sim_all,
                         sy_all=sy_all,
                         measurements=measurements,
                         s=s,
                         N=N,
                         delta_c=delta_c,
                         delta_c_dot=delta_c_dot,
                         c=c,
                         c_dot=c_dot,
                         n=n,
                     )
 
-                    # Let's calculate the (dJ_dsigma^2 * dsigma^2_dtheta) term now:
+                    # Calculate the (dJ_dsigma^2 * dsigma^2_dtheta) term:
                     if not group_dict[OPTIMIZE_NOISE]:
-                        residual_squared = (
-                            calculate_objective_function_for_obs(
-                                s=s,
-                                sim_all=sim_all,
-                                measurements=measurements,
-                                N=N,
-                                delta_c=delta_c,
-                                c=c,
-                                n=n,
-                            )
+                        residual_squared = _calculate_residuals_for_group(
+                            s=s,
+                            sim_all=sim_all,
+                            measurements=measurements,
+                            N=N,
+                            delta_c=delta_c,
+                            c=c,
+                            n=n,
                         )
                         dJ_dsigma2 = (
                             K / (2 * sigma**2)
                             - residual_squared / sigma**4
                         )
-                        dsigma2_dtheta = ssigma_all[0]
+                        dsigma2_dtheta = ssigma_all[0] * sigma
                         dsigma_grad_term = dJ_dsigma2 * dsigma2_dtheta
                     # If we optimize the noise hierarchically,
                     # the last term (dJ_dsigma^2 * dsigma^2_dtheta) is always 0
                     # since the sigma is optimized such that dJ_dsigma2=0.
                     else:
                         dsigma_grad_term = 0.0
 
                     # Combine all terms to get the complete gradient contribution
-                    grad += (
-                        dy_grad_term / sigma**2
-                        + ds_grad_term / sigma**2
-                        + dsigma_grad_term
-                    )
+                    grad += dy_grad_term / sigma**2 + dsigma_grad_term
 
                 snllh[par_opt_idx] = grad
 
         return snllh
 
     @staticmethod
-    def get_default_options() -> Dict:
+    def get_default_options() -> dict:
         """Return default options for solving the inner problem."""
         options = {
-            MIN_DIFF_FACTOR: 1 / 2,
+            MIN_DIFF_FACTOR: 0.0,
+            REGULARIZE_SPLINE: False,
+            REGULARIZATION_FACTOR: 0.0,
         }
         return options
 
     def _optimize_spline(
         self,
-        inner_parameters: List[SplineInnerParameter],
-        group_dict: Dict,
+        inner_parameters: list[SplineInnerParameter],
+        group_dict: dict,
     ):
         """Run optimization for the inner problem.
 
         Parameters
         ----------
         inner_parameters:
             The spline inner parameters.
         group_dict:
             The group dictionary.
         """
-        group_measurements = group_dict[DATAPOINTS]
-        current_group_simulation = group_dict[CURRENT_SIMULATION]
-        n_datapoints = group_dict[NUM_DATAPOINTS]
-        n_spline_pars = group_dict[N_SPLINE_PARS]
-
         (
             distance_between_bases,
             spline_bases,
             intervals_per_sim,
         ) = self._rescale_spline_bases(
-            sim_all=current_group_simulation, N=n_spline_pars, K=n_datapoints
+            sim_all=group_dict[CURRENT_SIMULATION],
+            N=group_dict[N_SPLINE_PARS],
+            K=group_dict[NUM_DATAPOINTS],
         )
 
-        min_meas = group_dict[MIN_DATAPOINT]
-        max_meas = group_dict[MAX_DATAPOINT]
         min_diff = self._get_minimal_difference(
-            measurement_range=max_meas - min_meas,
-            N=n_spline_pars,
+            measurement_range=group_dict[MAX_DATAPOINT]
+            - group_dict[MIN_DATAPOINT],
+            N=group_dict[N_SPLINE_PARS],
             min_diff_factor=self.options[MIN_DIFF_FACTOR],
         )
 
         inner_options = self._get_inner_optimization_options(
             inner_parameters=inner_parameters,
-            N=n_spline_pars,
-            min_meas=min_meas,
-            max_meas=max_meas,
+            N=group_dict[N_SPLINE_PARS],
+            min_meas=group_dict[MIN_DATAPOINT],
+            max_meas=group_dict[MAX_DATAPOINT],
             min_diff=min_diff,
         )
 
+        # Wrap the analytical optimization of sigma and
+        # the regularization into the objective function
         def objective_function_wrapper(x):
-            return calculate_objective_function_for_obs(
+            return _calculate_nllh_for_group(
                 s=x,
-                sim_all=current_group_simulation,
-                measurements=group_measurements,
-                N=n_spline_pars,
+                sim_all=group_dict[CURRENT_SIMULATION],
+                measurements=group_dict[DATAPOINTS],
+                N=group_dict[N_SPLINE_PARS],
                 delta_c=distance_between_bases,
                 c=spline_bases,
                 n=intervals_per_sim,
+                regularization_factor=self.options[REGULARIZATION_FACTOR],
+                regularize_spline=self.options[REGULARIZE_SPLINE],
+                group_dict=group_dict,
             )
 
+        # Wrap the analytical optimization of sigma and
+        # the regularization into the gradient function
         def inner_gradient_wrapper(x):
-            return calculate_inner_gradient_for_obs(
+            return _calculate_nllh_gradient_for_group(
                 s=x,
-                sim_all=current_group_simulation,
-                measurements=group_measurements,
-                N=n_spline_pars,
+                sim_all=group_dict[CURRENT_SIMULATION],
+                measurements=group_dict[DATAPOINTS],
+                N=group_dict[N_SPLINE_PARS],
                 delta_c=distance_between_bases,
                 c=spline_bases,
                 n=intervals_per_sim,
+                regularization_factor=self.options[REGULARIZATION_FACTOR],
+                regularize_spline=self.options[REGULARIZE_SPLINE],
+                group_dict=group_dict,
             )
 
         results = minimize(
             objective_function_wrapper,
             jac=inner_gradient_wrapper,
             **inner_options,
         )
@@ -522,20 +518,20 @@
         min_diff_factor: float,
     ):
         """Return minimal parameter difference for spline parameters."""
         return min_diff_factor * measurement_range / N
 
     def _get_inner_optimization_options(
         self,
-        inner_parameters: List[SplineInnerParameter],
+        inner_parameters: list[SplineInnerParameter],
         N: int,
         min_meas: float,
         max_meas: float,
         min_diff: float,
-    ) -> Dict:
+    ) -> dict:
         """Return default options for scipy optimizer.
 
         Returns inner subproblem optimization options including startpoint
         and optimization bounds or constraints, dependent on solver method.
 
         Parameters
         ----------
@@ -582,42 +578,226 @@
             "options": {"ftol": 1e-16, "disp": None},
             "bounds": Bounds(lb=constraint_min_diff),
         }
 
         return inner_options
 
 
+def _calculate_nllh_for_group(
+    s: np.ndarray,
+    sim_all: np.ndarray,
+    measurements: np.ndarray,
+    N: int,
+    delta_c: float,
+    c: np.ndarray,
+    n: np.ndarray,
+    regularization_factor: float,
+    regularize_spline: bool,
+    group_dict: dict,
+) -> float:
+    """Calculate the negative log-likelihood for the group.
+
+    Combines the sum of squared residuals, the noise parameter,
+    and the regularization term to the negative log-likelihood.
+
+    Parameters
+    ----------
+    s:
+        Reformulated inner spline parameters.
+    sim_all:
+        Simulations for the group.
+    measurements:
+        Measurements for the group.
+    N:
+        Number of spline bases.
+    delta_c:
+        Distance between two spline bases.
+    c:
+        Spline bases.
+    n:
+        Indices of the spline bases.
+    regularization_factor:
+        Regularization factor.
+    regularize_spline:
+        Whether to regularize the spline.
+    group_dict:
+        Dictionary containing the group information.
+
+    Returns
+    -------
+    Negative log-likelihood.
+    """
+    # Calculate residuals
+    residuals_squared = _calculate_residuals_for_group(
+        s=s,
+        sim_all=sim_all,
+        measurements=measurements,
+        N=N,
+        delta_c=delta_c,
+        c=c,
+        n=n,
+    )
+    K = len(sim_all)
+
+    # Calculate sigma
+    if group_dict[OPTIMIZE_NOISE]:
+        sigma = _calculate_sigma_for_group(
+            residuals_squared=residuals_squared,
+            n_datapoints=N,
+        )
+        group_dict[INNER_NOISE_PARS] = sigma
+    else:
+        sigma = group_dict[INNER_NOISE_PARS]
+
+    # Calculate regularization term
+    if regularize_spline:
+        regularization_term = _calculate_regularization_for_group(
+            s=s,
+            N=N,
+            c=c,
+            regularization_factor=regularization_factor,
+        )
+    else:
+        regularization_term = 0.0
+
+    # Combine all terms into the negative log-likelihood
+    nllh = (
+        0.5 * np.log(2 * np.pi * sigma**2) * K
+        + residuals_squared / (sigma**2)
+        + regularization_term
+    )
+    return nllh
+
+
+def _calculate_nllh_gradient_for_group(
+    s: np.ndarray,
+    sim_all: np.ndarray,
+    measurements: np.ndarray,
+    N: int,
+    delta_c: float,
+    c: np.ndarray,
+    n: np.ndarray,
+    regularization_factor: float,
+    regularize_spline: bool,
+    group_dict: dict,
+) -> np.ndarray:
+    """Calculate the gradient of the nllh wrt. spline differences s for the group.
+
+    Combines the gradient of the sum of squared residuals and the gradient of the
+    regularization term to the gradient of the negative log-likelihood.
+
+    Parameters
+    ----------
+    s:
+        Reformulated inner spline parameters.
+    sim_all:
+        Simulations for the group.
+    measurements:
+        Measurements for the group.
+    N:
+        Number of spline bases.
+    delta_c:
+        Distance between two spline bases.
+    c:
+        Spline bases.
+    n:
+        Indices of the spline bases.
+    regularization_factor:
+        Regularization factor.
+    regularize_spline:
+        Whether to regularize the spline.
+    group_dict:
+        Dictionary containing the group information.
+
+    Returns
+    -------
+    Gradient of the negative log-likelihood wrt. spline differences s.
+    """
+    # Calculate gradient of residuals
+    residuals_squared_gradient = _calculate_residuals_gradient_for_group(
+        s=s,
+        sim_all=sim_all,
+        measurements=measurements,
+        N=N,
+        delta_c=delta_c,
+        c=c,
+        n=n,
+    )
+
+    # Calculate sigma
+    if group_dict[OPTIMIZE_NOISE]:
+        residuals_squared = _calculate_residuals_for_group(
+            s=s,
+            sim_all=sim_all,
+            measurements=measurements,
+            N=N,
+            delta_c=delta_c,
+            c=c,
+            n=n,
+        )
+        sigma = _calculate_sigma_for_group(
+            residuals_squared=residuals_squared,
+            n_datapoints=N,
+        )
+        group_dict[INNER_NOISE_PARS] = sigma
+    else:
+        sigma = group_dict[INNER_NOISE_PARS]
+
+    # Calculate gradient of regularization term
+    if regularize_spline:
+        regularization_term_gradient = (
+            _calculate_regularization_gradient_for_group(
+                s=s,
+                N=N,
+                c=c,
+                regularization_factor=regularization_factor,
+            )
+        )
+    else:
+        regularization_term_gradient = np.zeros_like(s)
+
+    # Combine all terms into the gradient of the negative log-likelihood
+    nllh_gradient = (
+        residuals_squared_gradient / (sigma**2)
+        + regularization_term_gradient
+    )
+    return nllh_gradient
+
+
 def _calculate_sigma_for_group(
-    inner_result: Dict,
+    residuals_squared: float,
     n_datapoints: int,
 ):
     """Calculate the noise parameter sigma.
 
     Parameters
     ----------
-    noise_parameters:
-        The noise parameters of a group of the inner problem.
-    inner_result:
-        The inner optimization result.
+    residuals_squared:
+        The sum of squared residuals divided by 2.
+    n_datapoints:
+        The number of datapoints.
     """
-    sigma = np.sqrt(2 * inner_result[SCIPY_FUN] / (n_datapoints))
+    sigma = np.sqrt(2 * residuals_squared / n_datapoints)
 
     return sigma
 
 
-def calculate_objective_function_for_obs(
+def _calculate_residuals_for_group(
     s: np.ndarray,
     sim_all: np.ndarray,
     measurements: np.ndarray,
     N: int,
     delta_c: float,
     c: np.ndarray,
     n: np.ndarray,
 ):
-    """Objective function for reformulated inner spline problem."""
+    """Residuals squared for reformulated inner spline problem.
+
+    Equal to 1/2 * sum_k (tilde{z}_k - z_k)^2
+    """
     obj = 0
 
     for y_k, z_k, n_k in zip(sim_all, measurements, n):
         i = n_k - 1
         sum_s = 0
         sum_s = np.sum(s[:i])
         if i == 0:
@@ -626,50 +806,24 @@
             obj += (z_k - sum_s) ** 2
         else:
             obj += (z_k - (y_k - c[i - 1]) * s[i] / delta_c - sum_s) ** 2
     obj = obj / 2
     return obj
 
 
-def get_spline_mapped_simulations(
-    s: np.ndarray,
-    sim_all: np.ndarray,
-    N: int,
-    delta_c: float,
-    c: np.ndarray,
-    n: np.ndarray,
-):
-    """Return model simulations mapped using the approximation spline."""
-    mapped_simulations = np.zeros(len(sim_all))
-    xi = np.zeros(len(s))
-    for i in range(len(s)):
-        xi[i] = np.sum(s[: i + 1])
-
-    for y_k, n_k, index in zip(sim_all, n, range(len(sim_all))):
-        interval_index = n_k - 1
-        if interval_index == 0 or interval_index == N:
-            mapped_simulations[index] = xi[interval_index]
-        else:
-            mapped_simulations[index] = (y_k - c[interval_index - 1]) * (
-                xi[interval_index] - xi[interval_index - 1]
-            ) / delta_c + xi[interval_index - 1]
-
-    return mapped_simulations
-
-
-def calculate_inner_gradient_for_obs(
+def _calculate_residuals_gradient_for_group(
     s: np.ndarray,
     sim_all: np.ndarray,
     measurements: np.ndarray,
     N: int,
     delta_c: float,
     c: np.ndarray,
     n: np.ndarray,
 ):
-    """Gradient of the objective function for the reformulated inner spline problem."""
+    """Gradient of the residuals with respect to the spline differences s_i for a group."""
 
     gradient = np.zeros(N)
 
     for y_k, z_k, n_k in zip(sim_all, measurements, n):
         sum_s = 0
         i = n_k - 1  # just the iterator to go over the Jacobian array
         sum_s = np.sum(s[:i])
@@ -686,14 +840,132 @@
             gradient[:i] += np.full(
                 i,
                 (y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k,
             )
     return gradient
 
 
+def _calculate_regularization_for_group(
+    s: np.ndarray,
+    N: int,
+    c: np.ndarray,
+    regularization_factor: float,
+):
+    """Calculate regularization term the given spline.
+
+    We regularize the spline to be linear. To do this, we calculate the optimal
+    linear function that minimizes the sum of squared residuals with respect to
+    the spline knots. Then we calculate the sum of squared residuals for this
+    linear function. If the calculated offset is smaller than 0, we set it to 0.
+    This is because the spline is not allowed to be negative.
+    """
+    # Calculate the spline knots xi_i from spline differences s_i
+    lower_trian = np.tril(np.ones((N, N)))
+    xi = np.dot(lower_trian, s)
+
+    # Calculate auxiliary values
+    c_sum = np.sum(c)
+    xi_sum = np.sum(xi)
+    c_squares_sum = np.sum(c**2)
+    c_dot_xi = np.dot(c, xi)
+    # Calculate the optimal linear function offset
+    if np.isclose(N * c_squares_sum - c_sum**2, 0):
+        beta_opt = xi_sum / N
+    else:
+        beta_opt = (xi_sum * c_squares_sum - c_dot_xi * c_sum) / (
+            N * c_squares_sum - c_sum**2
+        )
+
+    # If the offset is smaller than 0, we set it to 0
+    if beta_opt < 0:
+        beta_opt = 0
+
+    # Calculate the slope of the optimal linear function
+    alpha_opt = (c_dot_xi - beta_opt * c_sum) / c_squares_sum
+
+    # Calculate the sum of squared residuals for the optimal linear function
+    regularization_term = np.sum((xi - alpha_opt * c - beta_opt) ** 2) / (
+        2 * N
+    )
+
+    return regularization_term * regularization_factor
+
+
+def _calculate_regularization_gradient_for_group(
+    s: np.ndarray,
+    N: int,
+    c: np.ndarray,
+    regularization_factor: float,
+):
+    """Calculate regularization term gradient for the given spline."""
+    # Calculate the spline knots xi_i from spline differences s_i
+
+    lower_trian = np.tril(np.ones((N, N)))
+    xi = np.dot(lower_trian, s)
+
+    # Calculate auxiliary values
+    c_sum = np.sum(c)
+    xi_sum = np.sum(xi)
+    c_squares_sum = np.sum(c**2)
+    c_dot_xi = np.dot(c, xi)
+
+    # Calculate the optimal linear function offset
+    if np.isclose(N * c_squares_sum - c_sum**2, 0):
+        beta_opt = xi_sum / N
+    else:
+        beta_opt = (xi_sum * c_squares_sum - c_dot_xi * c_sum) / (
+            N * c_squares_sum - c_sum**2
+        )
+
+    # If the offset is smaller than 0, we set it to 0.
+    # Otherwise, we calculate the gradient of the offset.
+    if beta_opt < 0:
+        beta_opt = 0
+
+    # Calculate the slope of the optimal linear function
+    alpha_opt = (c_dot_xi - beta_opt * c_sum) / c_squares_sum
+
+    # Calculate some more auxiliary values
+    residuals = xi - alpha_opt * c - beta_opt
+
+    # Can remove terms from this aux_matrix due to optimality
+    # of the linear function (alpha & beta)
+    aux_matrix = lower_trian
+
+    # Calculate the gradient of the sum of squared residuals
+    regularization_gradient = residuals @ aux_matrix / N
+
+    return regularization_gradient * regularization_factor
+
+
+def get_spline_mapped_simulations(
+    s: np.ndarray,
+    sim_all: np.ndarray,
+    N: int,
+    delta_c: float,
+    c: np.ndarray,
+    n: np.ndarray,
+):
+    """Return model simulations mapped using the approximation spline."""
+    mapped_simulations = np.zeros(len(sim_all))
+    lower_trian = np.tril(np.ones((N, N)))
+    xi = np.dot(lower_trian, s)
+
+    for y_k, n_k, index in zip(sim_all, n, range(len(sim_all))):
+        interval_index = n_k - 1
+        if interval_index == 0 or interval_index == N:
+            mapped_simulations[index] = xi[interval_index]
+        else:
+            mapped_simulations[index] = (y_k - c[interval_index - 1]) * (
+                xi[interval_index] - xi[interval_index - 1]
+            ) / delta_c + xi[interval_index - 1]
+
+    return mapped_simulations
+
+
 def calculate_inner_hessian(
     s: np.ndarray,
     sim_all: np.ndarray,
     sigma: np.ndarray,
     N: int,
     delta_c: float,
     c: np.ndarray,
@@ -715,93 +987,14 @@
             hessian[j][i] += (1 / sigma_k**2) * ((y_k - c[i - 1]) / delta_c)
             for h in range(i):
                 hessian[j][h] += 1 / sigma_k**2
 
     return hessian
 
 
-def calculate_ds_dtheta(
-    sim_all: np.ndarray,
-    sy_all: np.ndarray,
-    measurements: np.ndarray,
-    s: np.ndarray,
-    C: np.ndarray,
-    mu: np.ndarray,
-    N: int,
-    delta_c: float,
-    delta_c_dot: float,
-    c: np.ndarray,
-    c_dot: np.ndarray,
-    n: np.ndarray,
-    min_diff: float,
-):
-    """Calculate derivatives of reformulated spline parameters with respect to outer parameter.
-
-    Calculates the derivative of reformulated spline parameters s with respect to the
-    dynamical parameter theta. Firstly, we calculate the derivative of the
-    first two equations of the necessary optimality conditions of the
-    optimization problem with inequality constraints. Then we solve the linear
-    system to obtain the derivatives.
-    """
-
-    dgrad_dtheta_lhs = np.zeros((N, N))
-    dgrad_dtheta_rhs = np.zeros(2 * N)
-
-    for y_k, z_k, y_dot_k, n_k in zip(sim_all, measurements, sy_all, n):
-        i = n_k - 1  # just the iterator to go over the matrix
-        sum_s = 0
-        sum_s = np.sum(s[:i])
-
-        # Calculate dgrad_dtheta in the form of a linear system:
-        if i == 0:
-            dgrad_dtheta_lhs[i][i] += 1
-        elif i == N:
-            dgrad_dtheta_lhs = dgrad_dtheta_lhs + np.full((N, N), 1)
-
-        else:
-            dgrad_dtheta_lhs[i][i] += (y_k - c[i - 1]) ** 2 / delta_c**2
-            dgrad_dtheta_rhs[i] += (
-                (2 * (y_k - c[i - 1]) / delta_c * s[i] + sum_s - z_k)
-                * (
-                    (y_dot_k - c_dot[i - 1]) * delta_c
-                    - (y_k - c[i - 1]) * delta_c_dot
-                )
-                / delta_c**2
-            )
-
-            dgrad_dtheta_lhs[i, :i] += np.full(i, (y_k - c[i - 1]) / delta_c)
-            dgrad_dtheta_lhs[:i, i] += np.full(i, (y_k - c[i - 1]) / delta_c)
-            dgrad_dtheta_rhs[:i] += np.full(
-                i,
-                (
-                    (y_dot_k - c_dot[i - 1]) * delta_c
-                    - (y_k - c[i - 1]) * delta_c_dot
-                )
-                * s[i]
-                / delta_c**2,
-            )
-            dgrad_dtheta_lhs[:i, :i] += np.full((i, i), 1)
-
-    from scipy import linalg
-
-    constraint_min_diff = np.diag(np.full(N, min_diff))
-    constraint_min_diff[0, 0] = 0
-
-    lhs = np.block(
-        [
-            [dgrad_dtheta_lhs, C],
-            [-np.diag(mu), constraint_min_diff - np.diag(s)],
-        ]
-    )
-
-    ds_dtheta = linalg.lstsq(lhs, dgrad_dtheta_rhs, lapack_driver="gelsy")
-
-    return ds_dtheta[0][:N]
-
-
 def calculate_dy_term(
     sim_all: np.ndarray,
     sy_all: np.ndarray,
     measurements: np.ndarray,
     s: np.ndarray,
     N: int,
     delta_c: float,
@@ -854,27 +1047,27 @@
         delta_c_dot = (sy_all[max_idx] - sy_all[min_idx]) / (N - 1)
         c_dot = np.linspace(sy_all[min_idx], sy_all[max_idx], N)
 
     return delta_c_dot, c_dot
 
 
 def extract_expdata_using_mask(
-    expdata: List[np.ndarray], mask: List[np.ndarray]
+    expdata: list[np.ndarray], mask: list[np.ndarray]
 ):
     """Extract data from expdata list of arrays for the given mask."""
     return np.concatenate(
         [
             expdata[condition_index][mask[condition_index]]
             for condition_index in range(len(mask))
         ]
     )
 
 
 def save_inner_parameters_to_inner_problem(
-    inner_problem: SplineInnerProblem,
+    inner_problem: SemiquantProblem,
     s: np.ndarray,
     group: int,
 ) -> None:
     """Save inner parameter values to the inner subproblem.
 
     Calculates the non-reformulated inner spline parameters from
     the reformulated inner spline parameters and saves them to
@@ -889,53 +1082,30 @@
     """
     group_dict = inner_problem.groups[group]
     inner_spline_parameters = inner_problem.get_xs_for_group(group)
     inner_noise_parameters = inner_problem.get_noise_parameters_for_group(
         group
     )
 
-    xi = np.zeros(len(s))
-    for i in range(len(s)):
-        xi[i] = np.sum(s[: i + 1])
+    lower_trian = np.tril(np.ones((len(s), len(s))))
+    xi = np.dot(lower_trian, s)
 
     for idx in range(len(inner_spline_parameters)):
         inner_spline_parameters[idx].value = xi[idx]
 
     sigma = group_dict[INNER_NOISE_PARS]
 
     if group_dict[OPTIMIZE_NOISE]:
         inner_noise_parameters[0].value = sigma
 
 
-def _calculate_nllh_for_group(
-    inner_result: Dict,
-    sigma: float,
-    n_datapoints: int,
-):
-    """Calculate the negative log-likelihood for the group.
-
-    Parameters
-    ----------
-    inner_result : dict
-        Result of the inner problem.
-    sigma : float
-        Standard deviation of the measurement noise.
-    n_datapoints : int
-        Number of datapoints.
-    """
-    inner_result[SCIPY_FUN] = 0.5 * np.log(
-        2 * np.pi * sigma**2
-    ) * n_datapoints + inner_result[SCIPY_FUN] / (sigma**2)
-    return inner_result
-
-
 def get_monotonicity_measure(measurement, simulation):
     """Get monotonicity measure by calculating inversions.
 
-    Calculate the number of inversions in the simulation data
+    Calculates the number of inversions in the simulation data
     with respect to the measurement data.
 
     Parameters
     ----------
     measurement : np.ndarray
         Measurement data.
     simulation : np.ndarray
```

### Comparing `pypesto-0.4.1/pypesto/history/base.py` & `pypesto-0.4.2/pypesto/history/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     @abstractmethod
     def get_time_trace(
         self,
         ix: Union[int, Sequence[int], None] = None,
         trim: bool = False,
     ) -> Union[Sequence[float], float]:
         """
-        Cumulative execution times.
+        Cumulative execution times [s].
 
         Takes as parameter an index or indices and returns corresponding trace
         values. If only a single value is requested, the list is flattened.
         """
         raise NotImplementedError()
 
     def get_trimmed_indices(self) -> np.ndarray:
```

### Comparing `pypesto-0.4.1/pypesto/history/csv.py` & `pypesto-0.4.2/pypesto/history/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,28 @@
         self._update_trace(x, mode, result)
 
     def finalize(self, message: str = None, exitflag: str = None):
         """See :meth:`HistoryBase.finalize`."""
         super().finalize(message=message, exitflag=exitflag)
         self._save_trace(finalize=True)
 
+    def _simulation_to_values(self, result, used_time):
+        values = {
+            TIME: used_time,
+            N_FVAL: self._n_fval,
+            N_GRAD: self._n_grad,
+            N_HESS: self._n_hess,
+            N_RES: self._n_res,
+            N_SRES: self._n_sres,
+            FVAL: result[FVAL],
+            RES: result[RES],
+            HESS: result[HESS],
+        }
+        return values
+
     def _update_trace(
         self,
         x: np.ndarray,
         mode: ModeType,
         result: ResultDict,
     ):
         """Update and possibly store the trace."""
@@ -123,25 +137,15 @@
         used_time = time.time() - self._start_time
 
         # create table row
         row = pd.Series(
             name=len(self._trace), index=self._trace.columns, dtype='object'
         )
 
-        values = {
-            TIME: used_time,
-            N_FVAL: self._n_fval,
-            N_GRAD: self._n_grad,
-            N_HESS: self._n_hess,
-            N_RES: self._n_res,
-            N_SRES: self._n_sres,
-            FVAL: result[FVAL],
-            RES: result[RES],
-            HESS: result[HESS],
-        }
+        values = self._simulation_to_values(result, used_time)
 
         for var, val in values.items():
             row[(var, np.nan)] = val
 
         for var, val in {
             X: x,
             GRAD: result[GRAD],
@@ -158,20 +162,16 @@
         self._trace = pd.concat(
             (self._trace, pd.DataFrame([row])),
         )
 
         # save trace to file
         self._save_trace()
 
-    def _init_trace(self, x: np.ndarray):
-        """Initialize the trace."""
-        if self.x_names is None:
-            self.x_names = [f'x{i}' for i, _ in enumerate(x)]
-
-        columns: list[tuple] = [
+    def _trace_columns(self) -> list[tuple]:
+        return [
             (c, np.nan)
             for c in [
                 TIME,
                 N_FVAL,
                 N_GRAD,
                 N_HESS,
                 N_RES,
@@ -179,14 +179,21 @@
                 FVAL,
                 RES,
                 SRES,
                 HESS,
             ]
         ]
 
+    def _init_trace(self, x: np.ndarray):
+        """Initialize the trace."""
+        if self.x_names is None:
+            self.x_names = [f'x{i}' for i, _ in enumerate(x)]
+
+        columns = self._trace_columns()
+
         for var in [X, GRAD]:
             if var == X or self.options[f'trace_record_{var}']:
                 columns.extend([(var, x_name) for x_name in self.x_names])
             else:
                 columns.extend([(var,)])
 
         # TODO: multi-index for res, sres, hess
```

### Comparing `pypesto-0.4.1/pypesto/history/generate.py` & `pypesto-0.4.2/pypesto/history/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from .hdf5 import Hdf5History
 from .memory import MemoryHistory
 from .options import HistoryOptions
 from .util import HistoryTypeError
 
 
 def create_history(
-    id: str,
-    x_names: Sequence[str],
-    options: HistoryOptions,
+    id: str, x_names: Sequence[str], options: HistoryOptions
 ) -> HistoryBase:
     """Create a :class:`HistoryBase` object; Factory method.
 
     Parameters
     ----------
     id:
         Identifier for the history.
```

### Comparing `pypesto-0.4.1/pypesto/history/hdf5.py` & `pypesto-0.4.2/pypesto/history/hdf5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """HDF5 history."""
 
-
 import contextlib
 import time
 from functools import wraps
 from pathlib import Path
 from typing import Sequence, Union
 
 import h5py
@@ -147,23 +146,25 @@
         if message is not None:
             grp.attrs[MESSAGE] = message
         if exitflag is not None:
             grp.attrs[EXITFLAG] = exitflag
 
     @staticmethod
     def load(
-        id: str, file: str, options: Union[HistoryOptions, dict] = None
+        id: str,
+        file: Union[str, Path],
+        options: Union[HistoryOptions, dict] = None,
     ) -> 'Hdf5History':
         """Load the History object from memory."""
         history = Hdf5History(id=id, file=file, options=options)
         if options is None:
             history.recover_options(file)
         return history
 
-    def recover_options(self, file: str):
+    def recover_options(self, file: Union[str, Path]):
         """Recover options when loading the hdf5 history from memory.
 
         Done by testing which entries were recorded.
         """
         trace_record = self._has_non_nan_entries(X)
         trace_record_grad = self._has_non_nan_entries(GRAD)
         trace_record_hess = self._has_non_nan_entries(HESS)
@@ -296,14 +297,27 @@
     def exitflag(self) -> str:
         """Optimizer exitflag in case of finished optimization."""
         try:
             return self._f[f'{HISTORY}/{self.id}/{MESSAGES}/'].attrs[EXITFLAG]
         except KeyError:
             return None
 
+    @staticmethod
+    def _simulation_to_values(x, result, used_time):
+        values = {
+            X: x,
+            FVAL: result[FVAL],
+            GRAD: result[GRAD],
+            RES: result[RES],
+            SRES: result[SRES],
+            HESS: result[HESS],
+            TIME: used_time,
+        }
+        return values
+
     @with_h5_file("a")
     def _update_trace(
         self,
         x: np.ndarray,
         sensi_orders: tuple[int],
         mode: ModeType,
         result: ResultDict,
@@ -316,23 +330,15 @@
         #  and reduce via requested history options
         result = reduce_result_via_options(
             add_fun_from_res(result), self.options
         )
 
         used_time = time.time() - self.start_time
 
-        values = {
-            X: x,
-            FVAL: result[FVAL],
-            GRAD: result[GRAD],
-            RES: result[RES],
-            SRES: result[SRES],
-            HESS: result[HESS],
-            TIME: used_time,
-        }
+        values = self._simulation_to_values(x, result, used_time)
 
         iteration = self._require_group().attrs[N_ITERATIONS]
 
         for key in values.keys():
             if values[key] is not None:
                 self._require_group()[f'{iteration}/{key}'] = values[key]
```

### Comparing `pypesto-0.4.1/pypesto/history/memory.py` & `pypesto-0.4.2/pypesto/history/memory.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/history/optimizer.py` & `pypesto-0.4.2/pypesto/history/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/history/options.py` & `pypesto-0.4.2/pypesto/history/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self,
         trace_record: bool = False,
         trace_record_grad: bool = True,
         trace_record_hess: bool = True,
         trace_record_res: bool = True,
         trace_record_sres: bool = True,
         trace_save_iter: int = 10,
-        storage_file: Union[str, None] = None,
+        storage_file: Union[str, Path, None] = None,
     ):
         super().__init__()
 
         self.trace_record: bool = trace_record
         self.trace_record_grad: bool = trace_record_grad
         self.trace_record_hess: bool = trace_record_hess
         self.trace_record_res: bool = trace_record_res
```

### Comparing `pypesto-0.4.1/pypesto/history/util.py` & `pypesto-0.4.2/pypesto/history/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/logging.py` & `pypesto-0.4.2/pypesto/logging.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/aesara/base.py` & `pypesto-0.4.2/pypesto/objective/aesara/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/aggregated.py` & `pypesto-0.4.2/pypesto/objective/aggregated.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/amici/amici.py` & `pypesto-0.4.2/pypesto/objective/amici/amici.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 import abc
 import copy
 import os
 import tempfile
 from collections import OrderedDict
+from pathlib import Path
 from typing import TYPE_CHECKING, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
-from ...C import FVAL, INNER_PARAMETERS, MODE_FUN, MODE_RES, RDATAS, ModeType
+from ...C import (
+    FVAL,
+    INNER_PARAMETERS,
+    MODE_FUN,
+    MODE_RES,
+    RDATAS,
+    SUFFIXES_CSV,
+    SUFFIXES_HDF5,
+    ModeType,
+)
+from ...history import (
+    CountHistory,
+    CsvAmiciHistory,
+    Hdf5AmiciHistory,
+    HistoryOptions,
+    HistoryTypeError,
+    MemoryHistory,
+)
 from ..base import ObjectiveBase, ResultDict
 from .amici_calculator import AmiciCalculator
 from .amici_util import (
     create_identity_parameter_mapping,
     map_par_opt_to_par_sim,
 )
 
@@ -211,26 +229,53 @@
         super().__init__(x_names=x_names)
 
         # Custom (condition-specific) timepoints. See the
         # `set_custom_timepoints` method for more information.
         self.custom_timepoints = None
 
         # Initialize the dictionary for saving of inner parameters.
-        self.inner_parameters: Dict[str, float] = {}
+        self.inner_parameters: list[float] = None
 
     def get_config(self) -> dict:
         """Return basic information of the objective configuration."""
         info = super().get_config()
         info['x_names'] = self.x_names
         info['model_name'] = self.amici_model.getName()
         info['solver'] = str(type(self.amici_solver))
         info['sensi_order'] = self.max_sensi_order
 
         return info
 
+    def create_history(
+        self, id: str, x_names: Sequence[str], options: HistoryOptions
+    ):
+        """See `history.generate.create_history` documentation."""
+        # create different history types based on the inputs
+        if options.storage_file is None:
+            if options.trace_record:
+                return MemoryHistory(options=options)
+            else:
+                return CountHistory(options=options)
+
+        # replace id template in storage file
+        storage_file = options.storage_file.replace("{id}", id)
+
+        # evaluate type
+        suffix = Path(storage_file).suffix[1:]
+
+        # create history type based on storage type
+        if suffix in SUFFIXES_CSV:
+            return CsvAmiciHistory(
+                x_names=x_names, file=storage_file, options=options
+            )
+        elif suffix in SUFFIXES_HDF5:
+            return Hdf5AmiciHistory(id=id, file=storage_file, options=options)
+        else:
+            raise HistoryTypeError(suffix)
+
     def initialize(self):
         """See `ObjectiveBase` documentation."""
         super().initialize()
         self.reset_steadystate_guesses()
         self.calculator.initialize()
 
     def __deepcopy__(self, memodict: Dict = None) -> 'AmiciObjective':
@@ -452,15 +497,15 @@
             x_ids=self.x_ids,
             parameter_mapping=parameter_mapping,
             fim_for_hess=self.fim_for_hess,
         )
 
         nllh = ret[FVAL]
         rdatas = ret[RDATAS]
-        if INNER_PARAMETERS in ret and ret[INNER_PARAMETERS]:
+        if ret.get(INNER_PARAMETERS, None) is not None:
             self.inner_parameters = ret[INNER_PARAMETERS]
 
         # check whether we should update data for preequilibration guesses
         if (
             self.guess_steadystate
             and nllh <= self.steadystate_guesses['fval']
             and nllh < np.inf
```

### Comparing `pypesto-0.4.1/pypesto/objective/amici/amici_util.py` & `pypesto-0.4.2/pypesto/objective/amici/amici_util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/base.py` & `pypesto-0.4.2/pypesto/objective/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from ..C import FVAL, GRAD, HESS, MODE_FUN, MODE_RES, RES, SRES, ModeType
-from ..history import NoHistory
+from ..history import NoHistory, create_history
 from .pre_post_process import FixedParametersProcessor, PrePostProcessor
 
 ResultDict = Dict[str, Union[float, np.ndarray, Dict]]
 
 logger = logging.getLogger(__name__)
 
 
@@ -115,14 +115,18 @@
         Initialize the objective function.
 
         This function is used at the beginning of an analysis, e.g.
         optimization, and can e.g. reset the objective memory.
         By default does nothing.
         """
 
+    def create_history(self, id, x_names, options):
+        """See `history.generate.create_history` documentation."""
+        return create_history(id, x_names, options)
+
     def __call__(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...] = (0,),
         mode: ModeType = MODE_FUN,
         return_dict: bool = False,
         **kwargs,
```

### Comparing `pypesto-0.4.1/pypesto/objective/finite_difference.py` & `pypesto-0.4.2/pypesto/objective/finite_difference.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/function.py` & `pypesto-0.4.2/pypesto/objective/function.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/jax/base.py` & `pypesto-0.4.2/pypesto/objective/jax/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/julia/base.py` & `pypesto-0.4.2/pypesto/objective/julia/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/julia/petabJl.py` & `pypesto-0.4.2/pypesto/objective/julia/petabJl.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Interface to PEtab.jl."""
+
 import logging
 import os
 
 import numpy as np
 
 from .base import JuliaObjective, _read_source
```

### Comparing `pypesto-0.4.1/pypesto/objective/julia/petab_jl_importer.py` & `pypesto-0.4.2/pypesto/objective/julia/petab_jl_importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the PetabJlImporter class."""
+
 from __future__ import annotations
 
 import logging
 import os.path
 from typing import Iterable, List, Optional, Tuple, Union
 
 import numpy as np
```

### Comparing `pypesto-0.4.1/pypesto/objective/pre_post_process.py` & `pypesto-0.4.2/pypesto/objective/pre_post_process.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/objective/priors.py` & `pypesto-0.4.2/pypesto/objective/priors.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/optimize/__init__.py` & `pypesto-0.4.2/pypesto/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/optimize/ess/cess.py` & `pypesto-0.4.2/pypesto/optimize/ess/cess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Cooperative Enhanced Scatter Search."""
+
 import logging
 import multiprocessing
 import os
 import time
 from typing import Dict, List, Optional
 from warnings import warn
 
@@ -221,14 +222,15 @@
         optimizer_result = pypesto.OptimizerResult(
             id=str(i_result),
             x=self.x_best,
             fval=self.fx_best,
             message="Global best",
             **common_result_fields,
         )
+        optimizer_result.update_to_full(problem)
         # TODO DW: Create a single History with the global best?
         result.optimize_result.append(optimizer_result)
 
         # save refsets
         for i_refset, refset in enumerate(refsets):
             for i in range(refset.dim):
                 i_result += 1
@@ -237,14 +239,15 @@
                         id=str(i_result),
                         x=refset.x[i],
                         fval=refset.fx[i],
                         message=f"RefSet[{i_refset}][{i}]",
                         **common_result_fields,
                     )
                 )
+                result.optimize_result[-1].update_to_full(result.problem)
 
         # TODO DW: also save local solutions?
         #  (need to track fvals or re-evaluate)
 
         return result
 
     def _run_scatter_searches(
```

### Comparing `pypesto-0.4.1/pypesto/optimize/ess/ess.py` & `pypesto-0.4.2/pypesto/optimize/ess/ess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Enhanced Scatter Search.
 
 See papers on ESS :footcite:p:`EgeaBal2009,EgeaMar2010`,
 CESS :footcite:p:`VillaverdeEge2012`, and saCeSS :footcite:p:`PenasGon2017`.
 """
+
 import enum
 import logging
 import time
-from typing import Callable, List, Optional, Tuple, Union
+from typing import Callable, Optional, Union
 from warnings import warn
 
 import numpy as np
 
 import pypesto.optimize
 from pypesto import OptimizerResult, Problem
+from pypesto.history import MemoryHistory
 from pypesto.startpoint import StartpointMethod
 
 from .function_evaluator import FunctionEvaluator, create_function_evaluator
 from .refset import RefSet
 
 logger = logging.getLogger(__name__)
 
@@ -60,14 +62,15 @@
             Callable[..., "pypesto.optimize.Optimizer"],
         ] = None,
         max_eval=None,
         n_diverse: int = None,
         n_procs=None,
         n_threads=None,
         max_walltime_s=None,
+        result_includes_refset: bool = False,
     ):
         """Construct new ESS instance.
 
         For plausible values of hyperparameters, see :footcite:t:`VillaverdeEge2012`.
 
         Parameters
         ----------
@@ -105,14 +108,21 @@
             0 = only quality; 1 = only diversity
         n_procs:
             Number of parallel processes to use for parallel function
             evaluation. Mutually exclusive with `n_threads`.
         n_threads:
             Number of parallel threads to use for parallel function evaluation.
             Mutually exclusive with `n_procs`.
+        history:
+            History of the best values/parameters found so far.
+            (Monotonously decreasing objective values.)
+        result_includes_refset:
+            Whether the :meth:`minimize` result should include the final
+            RefSet, or just the local search results and the overall best
+            parameters.
         """
         if max_eval is None and max_walltime_s is None and max_iter is None:
             # in this case, we'd run forever
             raise ValueError(
                 "Either `max_iter`, `max_eval` or `max_walltime_s` have to be provided."
             )
         if max_eval is None:
@@ -143,34 +153,36 @@
         # Only perform local search from best solution
         self.local_only_best_sol: bool = False
         self.max_walltime_s = max_walltime_s
         self._initialize()
         self.logger = logging.getLogger(
             f"{self.__class__.__name__}-{id(self)}"
         )
+        self._result_includes_refset = result_includes_refset
 
     def _initialize(self):
         """(Re-)Initialize."""
         # RefSet
         self.refset: Optional[RefSet] = None
         # Overall best parameters found so far
         self.x_best: Optional[np.array] = None
         # Overall best function value found so far
         self.fx_best: float = np.inf
-        # Final parameters from local searches
-        self.local_solutions: List[np.array] = []
+        # Results from local searches
+        self.local_solutions: list[OptimizerResult] = []
         # Index of current iteration
         self.n_iter: int = 0
         # ESS iteration at which the last local search took place
         self.last_local_search_niter: int = 0
         # Whether self.x_best has changed in the current iteration
         self.x_best_has_changed: bool = False
         self.exit_flag: ESSExitFlag = ESSExitFlag.DID_NOT_RUN
         self.evaluator: Optional[FunctionEvaluator] = None
         self.starttime: Optional[float] = None
+        self.history: MemoryHistory = MemoryHistory()
 
     def _initialize_minimize(
         self,
         problem: Problem = None,
         startpoint_method: StartpointMethod = None,
         refset: Optional[RefSet] = None,
     ):
@@ -246,14 +258,15 @@
         )
 
         # [PenasGon2017]_ Algorithm 1
         while self._keep_going():
             self._do_iteration()
 
         self._report_final()
+        self.history.finalize(exitflag=self.exit_flag.name)
         return self._create_result()
 
     def _do_iteration(self):
         """Perform an ESS iteration."""
         self.x_best_has_changed = False
 
         self.refset.sort()
@@ -302,32 +315,38 @@
         optimizer_result = pypesto.OptimizerResult(
             id=str(i_result),
             x=self.x_best,
             fval=self.fx_best,
             message="Global best",
             **common_result_fields,
         )
-        # TODO DW: Create a single History with the global best?
+        optimizer_result.update_to_full(result.problem)
         result.optimize_result.append(optimizer_result)
 
-        # save refset
-        for i in range(self.refset.dim):
+        # save local solutions
+        for i, optimizer_result in enumerate(self.local_solutions):
             i_result += 1
-            result.optimize_result.append(
-                pypesto.OptimizerResult(
-                    id=str(i_result),
-                    x=self.refset.x[i],
-                    fval=self.refset.fx[i],
-                    message=f"RefSet[{i}]",
-                    **common_result_fields,
+            optimizer_result.id = f"Local solution {i}"
+            optimizer_result.optimizer = str(self.local_optimizer)
+            result.optimize_result.append(optimizer_result)
+
+        if self._result_includes_refset:
+            # save refset
+            for i in range(self.refset.dim):
+                i_result += 1
+                result.optimize_result.append(
+                    pypesto.OptimizerResult(
+                        id=str(i_result),
+                        x=self.refset.x[i],
+                        fval=self.refset.fx[i],
+                        message=f"RefSet[{i}]",
+                        **common_result_fields,
+                    )
                 )
-            )
-
-        # TODO DW: also save local solutions?
-        #  (need to track fvals or re-evaluate)
+                result.optimize_result[-1].update_to_full(result.problem)
 
         return result
 
     def _keep_going(self) -> bool:
         """Check exit criteria.
 
         Returns
@@ -358,28 +377,28 @@
 
     def _get_remaining_eval(self):
         """Get remaining function evaluations."""
         if self.max_eval is None:
             return np.inf
         return self.max_eval - self.evaluator.n_eval
 
-    def _combine_solutions(self) -> Tuple[np.array, np.array]:
+    def _combine_solutions(self) -> tuple[np.array, np.array]:
         """Combine solutions and evaluate.
 
-        Creates the next generation from the RefSet by pair-wise combinations
+        Creates the next generation from the RefSet by pair-wise combination
         of all RefSet members. Creates ``RefSet.dim ** 2 - RefSet.dim`` new
         parameter vectors, tests them, and keeps the best child of each parent.
 
         Returns
         -------
         y:
-            Contains the best of all pairwise combinations of all RefSet
-            members, for each RefSet members.
+            The next generation of parameter vectors
+            (`dim_refset` x `dim_problem`).
         fy:
-            The corresponding objective values.
+            The objective values corresponding to the parameters in `y`.
         """
         y = np.zeros(shape=(self.refset.dim, self.evaluator.problem.dim))
         fy = np.full(shape=self.refset.dim, fill_value=np.inf)
         for i in range(self.refset.dim):
             xs_new = np.vstack(
                 tuple(
                     self._combine(i, j)
@@ -459,16 +478,18 @@
             and self.n_iter - self.last_local_search_niter >= self.local_n2
         ):
             quality_order = np.argsort(fx_best_children)
             # compute minimal distance between the best children and all local
             #  optima found so far
             min_distances = np.array(
                 np.min(
-                    np.linalg.norm(y_i - local_solution)
-                    for local_solution in self.local_solutions
+                    np.linalg.norm(
+                        y_i - optimizer_result.x[optimizer_result.free_indices]
+                    )
+                    for optimizer_result in self.local_solutions
                 )
                 for y_i in x_best_children
             )
             # sort by furthest distance to existing local optima
             diversity_order = np.argsort(min_distances)[::-1]
             # compute priority, balancing quality and diversity
             #  (smaller value = higher priority)
@@ -509,35 +530,37 @@
 
             self.logger.info(
                 f"Local search: {local_search_fx0} -> {optimizer_result.fval} "
                 f"took {optimizer_result.time:.3g}s, finished with "
                 f"{optimizer_result.exitflag}: {optimizer_result.message}"
             )
             if np.isfinite(optimizer_result.fval):
-                local_solution_x = optimizer_result.x[
-                    optimizer_result.free_indices
-                ]
-                local_solution_fx = optimizer_result.fval
-
-                self.local_solutions.append(local_solution_x)
+                self.local_solutions.append(optimizer_result)
 
                 self._maybe_update_global_best(
-                    local_solution_x, local_solution_fx
+                    optimizer_result.x[optimizer_result.free_indices],
+                    optimizer_result.fval,
                 )
                 break
 
         self.last_local_search_niter = self.n_iter
         self.evaluator.reset_round_counter()
 
     def _maybe_update_global_best(self, x, fx):
         """Update the global best value if the provided value is better."""
         if fx < self.fx_best:
             self.x_best = x[:]
             self.fx_best = fx
             self.x_best_has_changed = True
+            self.history.update(
+                self.x_best,
+                (0,),
+                pypesto.C.MODE_FUN,
+                {pypesto.C.FVAL: self.fx_best},
+            )
 
     def _go_beyond(self, x_best_children, fx_best_children):
         """Apply go-beyond strategy.
 
         If a child is better than its parent, intensify search in that
         direction until no further improvement is made.
```

### Comparing `pypesto-0.4.1/pypesto/optimize/ess/function_evaluator.py` & `pypesto-0.4.2/pypesto/optimize/ess/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/optimize/ess/refset.py` & `pypesto-0.4.2/pypesto/optimize/ess/refset.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/optimize/ess/sacess.py` & `pypesto-0.4.2/pypesto/optimize/ess/sacess.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Self-adaptive cooperative enhanced scatter search (SACESS)."""
+
 import itertools
 import logging
 import logging.handlers
 import multiprocessing
 import os
 import time
 from math import ceil, sqrt
@@ -45,14 +46,21 @@
     the most promising worker. See :footcite:t:`PenasGon2017` for details.
 
     :class:`SacessOptimizer` can be used with or without a local optimizer, but
     it is highly recommended to use one.
 
     .. footbibliography::
 
+    Attributes
+    ----------
+    histories:
+        List of the histories of the best values/parameters
+        found by each worker. (Monotonously decreasing objective values.)
+        See :func:`pypesto.visualize.optimizer_history.sacess_history` for
+        visualization.
     """
 
     def __init__(
         self,
         num_workers: Optional[int] = None,
         ess_init_args: Optional[List[Dict[str, Any]]] = None,
         max_walltime_s: float = np.inf,
@@ -78,29 +86,29 @@
         num_workers:
             Number of workers to be used. If this argument is given,
             (different) default ESS settings will be used for each worker.
             Mutually exclusive with ``ess_init_args``.
             See :func:`get_default_ess_options` for details on the default
             settings.
         max_walltime_s:
-            Maximum walltime in seconds. Will only be checked between local
+            Maximum walltime in seconds. It will only be checked between local
             optimizations and other simulations, and thus, may be exceeded by
             the duration of a local search. Defaults to no limit.
             Note that in order to impose the wall time limit also on the local
             optimizer, the user has to provide a wrapper function similar to
             :meth:`SacessFidesFactory.__call__`.
         ess_loglevel:
             Loglevel for ESS runs.
         sacess_loglevel:
             Loglevel for SACESS runs.
         tmpdir:
-            Directory for temporary files. Defaults to a directory in the current
-            working directory named ``SacessOptimizerTemp-{random suffix}``.
-            When setting this option, make sure any optimizers running in parallel
-            have unique tmpdirs.
+            Directory for temporary files. This defaults to a directory in the
+            current working directory named ``SacessOptimizerTemp-{random suffix}``.
+            When setting this option, make sure any optimizers running in
+            parallel have a unique `tmpdir`.
         """
         if (num_workers is None and ess_init_args is None) or (
             num_workers is not None and ess_init_args is not None
         ):
             raise ValueError(
                 "Exactly one of `num_workers` or `ess_init_args` "
                 "has to be provided."
@@ -120,29 +128,52 @@
 
         self._tmpdir = tmpdir
         if self._tmpdir is None:
             while self._tmpdir is None or self._tmpdir.exists():
                 self._tmpdir = Path(f"SacessOptimizerTemp-{str(uuid1())[:8]}")
         self._tmpdir = Path(self._tmpdir).absolute()
         self._tmpdir.mkdir(parents=True, exist_ok=True)
+        self.histories: Optional[
+            list["pypesto.history.memory.MemoryHistory"]
+        ] = None
 
     def minimize(
         self,
         problem: Problem,
         startpoint_method: StartpointMethod = None,
-    ):
+    ) -> pypesto.Result:
         """Solve the given optimization problem.
 
+        Note that if this function is called from a multithreaded program (
+        multiple threads running at the time of calling this function) and
+        the :mod:`multiprocessing` `start method` is set to ``fork``, there is
+        a good chance for deadlocks. Postpone spawning threads until after
+        `minimize` or change the *start method* to ``spawn``.
+
         Parameters
         ----------
         problem:
             Minimization problem.
+            :meth:`Problem.startpoint_method` will be used to sample random
+            points. `SacessOptimizer` will deal with non-evaluable points.
+            Therefore, using :class:`pypesto.startpoint.CheckedStartpoints`
+            with ``check_fval=True`` or ``check_grad=True`` is not recommended
+            since it would create significant overhead.
+
         startpoint_method:
             Method for choosing starting points.
             **Deprecated. Use ``problem.startpoint_method`` instead.**
+
+        Returns
+        -------
+        Result object with optimized parameters in
+        :attr:`pypesto.Result.optimize_result`.
+        Results are sorted by objective. At least the best parameters are
+        included. Additional results may be included - this is subject to
+        change.
         """
         if startpoint_method is not None:
             warn(
                 "Passing `startpoint_method` directly is deprecated, use `problem.startpoint_method` instead.",
                 DeprecationWarning,
             )
 
@@ -206,19 +237,24 @@
                 p.start()
 
             # start logging thread only AFTER starting the worker processes
             #  to prevent deadlocks
             logging_thread.start()
 
             # wait for finish
+            # collect results
+            histories = [
+                sacess_manager._result_queue.get()
+                for _ in range(self.num_workers)
+            ]
+            self.histories = histories
             for p in worker_processes:
                 p.join()
 
         logging_thread.stop()
-
         result = self._create_result(problem)
 
         walltime = time.time() - start_time
         logger.info(
             f"{self.__class__.__name__} stopped after {walltime:3g}s with global best "
             f"{result.optimize_result[0].fval}."
         )
@@ -316,14 +352,15 @@
         # initial score is the worker index
         self._worker_scores = shmem_manager.Array(
             "d", range(self._num_workers)
         )
         self._worker_comms = shmem_manager.Array("i", [0] * self._num_workers)
         self._lock = shmem_manager.RLock()
         self._logger = logging.getLogger()
+        self._result_queue = shmem_manager.Queue()
 
     def get_best_solution(self) -> Tuple[np.array, float]:
         """Get the best objective value and corresponding parameters."""
         with self._lock:
             return np.array(self._best_known_x), self._best_known_fx.value
 
     def reconfigure_worker(self, worker_idx: int) -> Dict:
@@ -503,33 +540,24 @@
         self._refset.initialize_random(
             n_diverse=max(
                 self._ess_kwargs.get('n_diverse', 10 * problem.dim),
                 self._refset.dim,
             )
         )
 
-        ess_results = pypesto.Result(problem=problem)
         ess = self._setup_ess(startpoint_method)
 
         # run ESS until exit criteria are met, but start at least one iteration
         while self._keep_going() or ess.n_iter == 0:
             # perform one ESS iteration
             ess._do_iteration()
 
-            # TODO maybe not in every iteration?
-            # drop all but the 50 best results
-            cur_ess_results = ess._create_result()
-            ess_results.optimize_result.append(
-                cur_ess_results.optimize_result,
-                prefix=f"{self._worker_idx}_{ess.n_iter}_",
-            )
-            ess_results.optimize_result.list = (
-                ess_results.optimize_result.list[:50]
-            )
             if self._tmp_result_file:
+                # TODO maybe not in every iteration?
+                ess_results = ess._create_result()
                 write_result(
                     ess_results,
                     self._tmp_result_file,
                     overwrite=True,
                     optimize=True,
                 )
             # check if the best solution of the last local ESS is sufficiently
@@ -541,14 +569,16 @@
             self._maybe_adapt(problem)
 
             self._logger.info(
                 f"sacess worker {self._worker_idx} iteration {ess.n_iter} "
                 f"(best: {self._best_known_fx})."
             )
 
+        ess.history.finalize(exitflag=ess.exit_flag.name)
+        self._manager._result_queue.put(ess.history)
         ess._report_final()
 
     def _setup_ess(self, startpoint_method: StartpointMethod) -> ESSOptimizer:
         """Run ESS."""
         ess_kwargs = self._ess_kwargs.copy()
         # account for sacess walltime limit
         ess_kwargs['max_walltime_s'] = min(
@@ -592,15 +622,15 @@
             self.replace_solution(self._refset, x=recv_x, fx=recv_fx)
 
     def _maybe_adapt(self, problem: Problem):
         """Perform adaptation step.
 
         Update ESS settings if conditions are met.
         """
-        # Update ESS settings if we received way more solutions than we  sent
+        # Update ESS settings if we received way more solutions than we sent
         # Magic numbers from [PenasGon2017]_ algorithm 5
         if (
             self._n_received_solutions > 10 * self._n_sent_solutions + 20
             and self._neval > problem.dim * 5000
         ):
             self._ess_kwargs = self._manager.reconfigure_worker(
                 self._worker_idx
@@ -740,16 +770,20 @@
     Based on https://bitbucket.org/DavidPenas/sacess-library/src/508e7ac15579104731cf1f8c3969960c6e72b872/src/method_module_fortran/eSS/parallelscattersearchfunctions.f90#lines-929
 
     Parameters
     ----------
     num_workers: Number of configurations to return.
     dim: Problem dimension (number of optimized parameters).
     local_optimizer: The local optimizer to use
-        (see same argument in :class:`ESSOptimizer`), or a boolean indicating
-        whether to set the default local optimizer (currently :class:`FidesOptimizer`).
+        (see same argument in :class:`ESSOptimizer`), a boolean indicating
+        whether to set the default local optimizer
+        (currently :class:`FidesOptimizer`), a :class:`Optimizer` instance,
+        or a :obj:`Callable` returning an optimizer instance.
+        The latter can be used to propagate walltime limits to the local
+        optimizers. See :meth:`SacessFidesFactory.__call__` for an example.
     """
     min_dimrefset = 5
 
     def dim_refset(x):
         return max(min_dimrefset, ceil((1 + sqrt(4 * dim * x)) / 2))
 
     settings = [
@@ -901,15 +935,17 @@
             'local_n2': 1,
         },
     ]
 
     # Set local optimizer
     for cur_settings in settings:
         if local_optimizer is True:
-            cur_settings['local_optimizer'] = SacessFidesFactory()
+            cur_settings['local_optimizer'] = SacessFidesFactory(
+                fides_kwargs={"verbose": logging.WARNING}
+            )
         elif local_optimizer is not False:
             cur_settings['local_optimizer'] = local_optimizer
 
     return [
         settings[0],
         *(itertools.islice(itertools.cycle(settings[1:]), num_workers - 1)),
     ]
```

### Comparing `pypesto-0.4.1/pypesto/optimize/load.py` & `pypesto-0.4.2/pypesto/optimize/load.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,17 +191,19 @@
     opt_hist = read_history_from_file(
         problem=problem, history_options=history_options, identifier=identifier
     )
     result = OptimizerResult(
         id=identifier,
         message='loaded from file',
         exitflag=EXITFLAG_LOADED_FROM_FILE,
-        time=max(opt_hist.history.get_time_trace())
-        if len(opt_hist.history)
-        else 0.0,
+        time=(
+            max(opt_hist.history.get_time_trace())
+            if len(opt_hist.history)
+            else 0.0
+        ),
     )
     result.id = identifier
     result = fill_result_from_history(
         result=result,
         optimizer_history=opt_hist,
     )
     if problem:
```

### Comparing `pypesto-0.4.1/pypesto/optimize/optimize.py` & `pypesto-0.4.2/pypesto/optimize/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     problem: Problem,
     optimizer: Optimizer = None,
     n_starts: int = 100,
     ids: Iterable[str] = None,
     startpoint_method: Union[StartpointMethod, Callable, bool] = None,
     result: Result = None,
     engine: Engine = None,
-    progress_bar: bool = True,
+    progress_bar: bool = None,
     options: OptimizeOptions = None,
     history_options: HistoryOptions = None,
     filename: Union[str, Callable, None] = None,
     overwrite: bool = False,
 ) -> Result:
     """
     Do multistart optimization.
```

### Comparing `pypesto-0.4.1/pypesto/optimize/optimizer.py` & `pypesto-0.4.2/pypesto/optimize/optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 from functools import wraps
 from typing import TYPE_CHECKING, Dict, Optional
 
 import numpy as np
 import scipy.optimize
 
 from ..C import FVAL, GRAD, INNER_PARAMETERS, MODE_FUN, MODE_RES
-from ..history import (
-    HistoryOptions,
-    NoHistory,
-    OptimizerHistory,
-    create_history,
-)
+from ..history import HistoryOptions, NoHistory, OptimizerHistory
 from ..objective import Objective
 from ..problem import Problem
 from ..result import OptimizerResult
 from .load import fill_result_from_history
 from .options import OptimizeOptions
 from .util import check_finite_bounds
 
@@ -37,14 +32,51 @@
     def __init__(self, optimizer: str):
         super().__init__(
             f'Optimizer "{optimizer}" not available, install corresponding '
             f'package e.g. via "pip install pypesto[{optimizer}]"'
         )
 
 
+def hierarchical_decorator(minimize):
+    """Add inner parameters to the optimizer result.
+
+    Default decorator for the minimize() method.
+    """
+
+    @wraps(minimize)
+    def wrapped_minimize(
+        self,
+        problem: Problem,
+        x0: np.ndarray,
+        id: str,
+        history_options: HistoryOptions = None,
+        optimize_options: OptimizeOptions = None,
+    ):
+        # perform the actual optimization
+        result = minimize(
+            self,
+            problem=problem,
+            x0=x0,
+            id=id,
+            history_options=history_options,
+            optimize_options=optimize_options,
+        )
+
+        # add inner parameters
+        if (
+            hasattr(problem.objective, INNER_PARAMETERS)
+            and problem.objective.inner_parameters is not None
+        ):
+            result[INNER_PARAMETERS] = problem.objective.inner_parameters
+
+        return result
+
+    return wrapped_minimize
+
+
 def history_decorator(minimize):
     """Initialize and extract information stored in the history.
 
     Default decorator for the minimize() method.
     """
 
     @wraps(minimize)
@@ -61,15 +93,15 @@
 
         objective = problem.objective
 
         # initialize the objective
         objective.initialize()
 
         # initialize the history
-        history = create_history(
+        history = objective.create_history(
             id=id,
             x_names=[problem.x_names[ix] for ix in problem.x_free_indices],
             options=history_options,
         )
         optimizer_history = OptimizerHistory(
             history=history,
             x0=x0,
@@ -191,29 +223,55 @@
         )
 
         return result
 
     return wrapped_minimize
 
 
+def minimize_decorator_collection(minimize):
+    """Collect all decorators for the minimize() method."""
+
+    @wraps(minimize)
+    @fix_decorator
+    @time_decorator
+    @history_decorator
+    @hierarchical_decorator
+    def wrapped_minimize(
+        self,
+        problem: Problem,
+        x0: np.ndarray,
+        id: str,
+        history_options: HistoryOptions = None,
+        optimize_options: OptimizeOptions = None,
+    ):
+        return minimize(
+            self,
+            problem=problem,
+            x0=x0,
+            id=id,
+            history_options=history_options,
+            optimize_options=optimize_options,
+        )
+
+    return wrapped_minimize
+
+
 class Optimizer(abc.ABC):
     """
     Optimizer base class, not functional on its own.
 
     An optimizer takes a problem, and possibly a start point, and then
     performs an optimization. It returns an OptimizerResult.
     """
 
     def __init__(self):
         """Initialize base class."""
 
     @abc.abstractmethod
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -280,17 +338,15 @@
         # print everything that is customized
         if self.tol is not None:
             rep += f" tol={self.tol}"
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -458,16 +514,14 @@
             x=np.array(res.x),
             fval=fval,
             grad=grad,
             hess=getattr(res, 'hess', None),
             exitflag=res.status,
             message=res.message,
         )
-        if hasattr(objective, INNER_PARAMETERS) and objective.inner_parameters:
-            optimizer_result[INNER_PARAMETERS] = objective.inner_parameters
 
         return optimizer_result
 
     def is_least_squares(self):
         """Check whether optimizer is a least squares optimizer."""
         return re.match(r'(?i)^(ls_)', self.method)
 
@@ -501,17 +555,15 @@
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -563,17 +615,15 @@
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -639,17 +689,15 @@
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -715,17 +763,15 @@
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__} par_sigma0={self.par_sigma0}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -798,17 +844,15 @@
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -874,17 +918,15 @@
     def __repr__(self) -> str:
         rep = f"<{self.__class__.__name__} par_popsize={self.par_popsize}"
         # print everything that is customized
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -1093,17 +1135,15 @@
             rep += f" local_method={self.local_method}"
         if self.options is not None:
             rep += f" options={self.options}"
         if self.local_options is not None:
             rep += f" local_options={self.local_methods}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
@@ -1278,17 +1318,15 @@
                 )
         if self.verbose is not None:
             rep += f" verbose={self.verbose}"
         if self.options is not None:
             rep += f" options={self.options}"
         return rep + ">"
 
-    @fix_decorator
-    @time_decorator
-    @history_decorator
+    @minimize_decorator_collection
     def minimize(
         self,
         problem: Problem,
         x0: np.ndarray,
         id: str,
         history_options: HistoryOptions = None,
         optimize_options: OptimizeOptions = None,
```

### Comparing `pypesto-0.4.1/pypesto/optimize/options.py` & `pypesto-0.4.2/pypesto/optimize/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/optimize/task.py` & `pypesto-0.4.2/pypesto/optimize/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/optimize/util.py` & `pypesto-0.4.2/pypesto/optimize/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/petab/__init__.py` & `pypesto-0.4.2/pypesto/petab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 PEtab
 =====
 
 pyPESTO support for the PEtab data format.
 """
+
 import warnings
 
 from .importer import PetabImporter
 
 # PEtab and amici are optional dependencies
```

### Comparing `pypesto-0.4.1/pypesto/petab/importer.py` & `pypesto-0.4.2/pypesto/petab/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Contains the PetabImporter class."""
+
 from __future__ import annotations
 
 import importlib
 import logging
 import os
 import shutil
 import sys
 import tempfile
 import warnings
 from dataclasses import dataclass
 from functools import partial
+from importlib.metadata import version
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Optional,
@@ -28,44 +30,47 @@
 from ..C import (
     CENSORED,
     CENSORING_TYPES,
     CONDITION_SEP,
     MEASUREMENT_TYPE,
     MODE_FUN,
     MODE_RES,
-    NONLINEAR_MONOTONE,
-    OPTIMAL_SCALING_OPTIONS,
     ORDINAL,
+    ORDINAL_OPTIONS,
+    PARAMETER_TYPE,
+    RELATIVE,
+    SEMIQUANTITATIVE,
     SPLINE_APPROXIMATION_OPTIONS,
+    InnerParameterType,
 )
-from ..hierarchical.calculator import HierarchicalAmiciCalculator
 from ..hierarchical.inner_calculator_collector import InnerCalculatorCollector
-from ..hierarchical.problem import InnerProblem
 from ..objective import AggregatedObjective, AmiciObjective
 from ..objective.amici import AmiciObjectBuilder
 from ..objective.priors import NegLogParameterPriors, get_parameter_prior_dict
 from ..predict import AmiciPredictor
-from ..problem import Problem
+from ..problem import HierarchicalProblem, Problem
 from ..result import PredictionResult
 from ..startpoint import CheckedStartpoints, StartpointMethod
 
 try:
     import amici
     import amici.parameter_mapping
     import amici.petab_import
     import amici.petab_objective
     import petab
     from petab.C import (
         ESTIMATE,
+        NOISE_PARAMETERS,
+        OBSERVABLE_ID,
         PREEQUILIBRATION_CONDITION_ID,
         SIMULATION_CONDITION_ID,
     )
     from petab.models import MODEL_TYPE_SBML
 except ImportError:
-    pass
+    amici = None
 
 logger = logging.getLogger(__name__)
 
 
 class PetabImporter(AmiciObjectBuilder):
     """
     Importer for PEtab files.
@@ -74,15 +79,15 @@
     :class:`pypesto.problem.Problem` from PEtab files. The created objective function is a
     negative log-likelihood function and can thus be negative. The actual
     form of the likelihood depends on the noise model specified in the provided PEtab problem.
     For more information, see the
     `PEtab documentation <https://petab.readthedocs.io/en/latest/documentation_data_format.html#noise-distributions>`_.
     """  # noqa
 
-    MODEL_BASE_DIR = "amici_models"
+    MODEL_BASE_DIR = f"amici_models/{version('amici') if amici else ''}"
 
     def __init__(
         self,
         petab_problem: petab.Problem,
         output_folder: str = None,
         model_name: str = None,
         validate_petab: bool = True,
@@ -107,29 +112,43 @@
         validate_petab_hierarchical:
             Flag indicating if the PEtab problem shall be validated in terms of
             pyPESTO's hierarchical optimization implementation.
         hierarchical:
             Whether to use hierarchical optimization or not, in case the
             underlying PEtab problem has parameters marked for hierarchical
             optimization (non-empty `parameterType` column in the PEtab
-            parameter table). Required for ordinal, censored and nonlinear-monotone data.
+            parameter table). Required for ordinal, censored and semiquantitative data.
         inner_options:
             Options for the inner problems and solvers.
             If not provided, default options will be used.
         """
         self.petab_problem = petab_problem
         self._hierarchical = hierarchical
 
         self._non_quantitative_data_types = (
             get_petab_non_quantitative_data_types(petab_problem)
         )
 
-        if self._non_quantitative_data_types and not self._hierarchical:
+        if self._non_quantitative_data_types is None and hierarchical:
+            raise ValueError(
+                "Hierarchical optimization enabled, but no non-quantitative "
+                "data types specified. Specify non-quantitative data types "
+                "or disable hierarchical optimization."
+            )
+
+        if (
+            self._non_quantitative_data_types is not None
+            and any(
+                data_type in self._non_quantitative_data_types
+                for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
+            )
+            and not self._hierarchical
+        ):
             raise ValueError(
-                "Ordinal, censored and nonlinear-monotone data require "
+                "Ordinal, censored and semiquantitative data require "
                 "hierarchical optimization to be enabled.",
             )
 
         self.inner_options = inner_options
         if self.inner_options is None:
             self.inner_options = {}
 
@@ -171,18 +190,15 @@
             output_folder=output_folder,
             model_name=model_name,
         )
 
     def validate_inner_options(self):
         """Validate the inner options."""
         for key in self.inner_options:
-            if (
-                key
-                not in OPTIMAL_SCALING_OPTIONS + SPLINE_APPROXIMATION_OPTIONS
-            ):
+            if key not in ORDINAL_OPTIONS + SPLINE_APPROXIMATION_OPTIONS:
                 raise ValueError(f"Unknown inner option {key}.")
 
     def check_gradients(
         self,
         *args,
         rtol: float = 1e-2,
         atol: float = 1e-3,
@@ -248,14 +264,15 @@
             )
             for mode_df in dfs
         )
 
     def create_model(
         self,
         force_compile: bool = False,
+        verbose: bool = True,
         **kwargs,
     ) -> amici.Model:
         """
         Import amici model.
 
         Parameters
         ----------
@@ -263,16 +280,19 @@
             If False, the model is compiled only if the output folder does not
             exist yet. If True, the output folder is deleted and the model
             (re-)compiled in either case.
 
             .. warning::
                 If `force_compile`, then an existing folder of that name will
                 be deleted.
-
-        kwargs: Extra arguments passed to amici.SbmlImporter.sbml2amici
+        verbose:
+            Passed to AMICI's model compilation. If True, the compilation
+            progress is printed.
+        kwargs:
+            Extra arguments passed to amici.SbmlImporter.sbml2amici
         """
         # courtesy check whether target is folder
         if os.path.exists(self.output_folder) and not os.path.isdir(
             self.output_folder
         ):
             raise AssertionError(
                 f"Refusing to remove {self.output_folder} for model "
@@ -287,18 +307,19 @@
         if self._must_compile(force_compile):
             logger.info(
                 f"Compiling amici model to folder " f"{self.output_folder}."
             )
             if self.petab_problem.model.type_id == MODEL_TYPE_SBML:
                 self.compile_model(
                     validate=self.validate_petab,
+                    verbose=verbose,
                     **kwargs,
                 )
             else:
-                self.compile_model(**kwargs)
+                self.compile_model(verbose=verbose, **kwargs)
         else:
             logger.debug(
                 f"Using existing amici model in folder "
                 f"{self.output_folder}."
             )
 
         return self._create_model()
@@ -364,75 +385,88 @@
         amici.petab_import.import_petab_problem(
             petab_problem=self.petab_problem,
             model_name=self.model_name,
             model_output_dir=self.output_folder,
             **kwargs,
         )
 
-    def create_solver(self, model: amici.Model = None) -> amici.Solver:
+    def create_solver(
+        self,
+        model: amici.Model = None,
+        verbose: bool = True,
+    ) -> amici.Solver:
         """Return model solver."""
         # create model
         if model is None:
-            model = self.create_model()
+            model = self.create_model(verbose=verbose)
 
         solver = model.getSolver()
         return solver
 
     def create_edatas(
-        self, model: amici.Model = None, simulation_conditions=None
+        self,
+        model: amici.Model = None,
+        simulation_conditions=None,
+        verbose: bool = True,
     ) -> List[amici.ExpData]:
         """Create list of :class:`amici.amici.ExpData` objects."""
         # create model
         if model is None:
-            model = self.create_model()
+            model = self.create_model(verbose=verbose)
 
         return amici.petab_objective.create_edatas(
             amici_model=model,
             petab_problem=self.petab_problem,
             simulation_conditions=simulation_conditions,
         )
 
     def create_objective(
         self,
         model: amici.Model = None,
         solver: amici.Solver = None,
         edatas: Sequence[amici.ExpData] = None,
         force_compile: bool = False,
+        verbose: bool = True,
         **kwargs,
     ) -> AmiciObjective:
         """Create a :class:`pypesto.objective.AmiciObjective`.
 
         Parameters
         ----------
         model:
             The AMICI model.
         solver:
             The AMICI solver.
         edatas:
             The experimental data in AMICI format.
         force_compile:
             Whether to force-compile the model if not passed.
+        verbose:
+            Passed to AMICI's model compilation. If True, the compilation
+            progress is printed.
         **kwargs:
             Additional arguments passed on to the objective. In case of ordinal
-            or nonlinear-monotone measurements, ``inner_options`` can optionally
+            or semiquantitative measurements, ``inner_options`` can optionally
             be passed here. If none are given, ``inner_options`` given to the
             importer constructor (or inner defaults) will be chosen.
 
         Returns
         -------
         A :class:`pypesto.objective.AmiciObjective` for the model and the data.
         """
         # get simulation conditions
         simulation_conditions = petab.get_simulation_conditions(
             self.petab_problem.measurement_df
         )
 
         # create model
         if model is None:
-            model = self.create_model(force_compile=force_compile)
+            model = self.create_model(
+                force_compile=force_compile, verbose=verbose
+            )
         # create solver
         if solver is None:
             solver = self.create_solver(model)
         # create conditions and edatas from measurement data
         if edatas is None:
             edatas = self.create_edatas(
                 model=model, simulation_conditions=simulation_conditions
@@ -460,47 +494,59 @@
             parameter_mapping=parameter_mapping,
             amici_model=model,
         )
 
         calculator = None
         amici_reporting = None
 
-        if self._non_quantitative_data_types and self._hierarchical:
+        if (
+            self._non_quantitative_data_types is not None
+            and self._hierarchical
+        ):
             inner_options = kwargs.pop('inner_options', None)
             inner_options = (
                 inner_options
                 if inner_options is not None
                 else self.inner_options
             )
             calculator = InnerCalculatorCollector(
                 self._non_quantitative_data_types,
                 self.petab_problem,
                 model,
                 edatas,
                 inner_options,
             )
-            amici_reporting = amici.RDataReporting.residuals
-
-        elif self._hierarchical:
-            inner_problem = InnerProblem.from_petab_amici(
-                self.petab_problem, model, edatas
-            )
-            calculator = HierarchicalAmiciCalculator(inner_problem)
             amici_reporting = amici.RDataReporting.full
 
-        if self._hierarchical:
             # FIXME: currently not supported with hierarchical
             if 'guess_steadystate' in kwargs and kwargs['guess_steadystate']:
                 warnings.warn(
                     "`guess_steadystate` not supported with hierarchical optimization. Disabling `guess_steadystate`."
                 )
             kwargs['guess_steadystate'] = False
-            inner_parameter_ids = calculator.get_inner_parameter_ids()
+            inner_parameter_ids = calculator.get_inner_par_ids()
             par_ids = [x for x in par_ids if x not in inner_parameter_ids]
 
+        max_sensi_order = kwargs.get('max_sensi_order', None)
+
+        if (
+            self._non_quantitative_data_types is not None
+            and any(
+                data_type in self._non_quantitative_data_types
+                for data_type in [ORDINAL, CENSORED, SEMIQUANTITATIVE]
+            )
+            and max_sensi_order is not None
+            and max_sensi_order > 1
+        ):
+            raise ValueError(
+                "Ordinal, censored and semiquantitative data cannot be "
+                "used with second order sensitivities. Use a up to first order "
+                "method or disable ordinal, censored and semiquantitative "
+            )
+
         # create objective
         obj = AmiciObjective(
             amici_model=model,
             amici_solver=solver,
             edatas=edatas,
             x_ids=par_ids,
             x_names=par_ids,
@@ -694,33 +740,24 @@
         x_fixed_indices = self.petab_problem.x_fixed_indices
         x_fixed_vals = self.petab_problem.x_nominal_fixed_scaled
         x_ids = self.petab_problem.x_ids
         lb = self.petab_problem.lb_scaled
         ub = self.petab_problem.ub_scaled
 
         # Raise error if the correct calculator is not used.
-
-        if self._non_quantitative_data_types:
+        if self._hierarchical:
             if not isinstance(objective.calculator, InnerCalculatorCollector):
                 raise AssertionError(
-                    f"If there are ordinal, censored or nonlinear-monotone measurements, the `calculator` attribute of the `objective` has to be {InnerCalculatorCollector} and not {objective.calculator}."
-                )
-        elif self._hierarchical:
-            if not isinstance(
-                objective.calculator, HierarchicalAmiciCalculator
-            ):
-                raise AssertionError(
-                    f"If hierarchical optimization of relative data is enabled, the `calculator` attribute of the `objective` has to be {HierarchicalAmiciCalculator} and not {objective.calculator}."
+                    f"If hierarchical optimization is enabled, the `calculator` attribute of the `objective` has to be {InnerCalculatorCollector} and not {objective.calculator}."
                 )
+
         # In case of hierarchical optimization, parameters estimated in the
         # inner subproblem are removed from the outer problem
         if self._hierarchical:
-            inner_parameter_ids = (
-                objective.calculator.get_inner_parameter_ids()
-            )
+            inner_parameter_ids = objective.calculator.get_inner_par_ids()
             lb = [b for x, b in zip(x_ids, lb) if x not in inner_parameter_ids]
             ub = [b for x, b in zip(x_ids, ub) if x not in inner_parameter_ids]
             x_ids = [x for x in x_ids if x not in inner_parameter_ids]
             x_fixed_indices = list(
                 map(x_ids.index, self.petab_problem.x_fixed_ids)
             )
 
@@ -741,15 +778,20 @@
             if self._hierarchical:
                 raise NotImplementedError(
                     "Hierarchical optimization in combination with priors "
                     "is not yet supported."
                 )
             objective = AggregatedObjective([objective, prior])
 
-        problem = Problem(
+        if self._hierarchical:
+            problem_class = HierarchicalProblem
+        else:
+            problem_class = Problem
+
+        problem = problem_class(
             objective=objective,
             lb=lb,
             ub=ub,
             x_fixed_indices=x_fixed_indices,
             x_fixed_vals=x_fixed_vals,
             x_guesses=x_guesses,
             x_names=x_ids,
@@ -763,34 +805,38 @@
 
         return problem
 
     def rdatas_to_measurement_df(
         self,
         rdatas: Sequence[amici.ReturnData],
         model: amici.Model = None,
+        verbose: bool = True,
     ) -> pd.DataFrame:
         """
         Create a measurement dataframe in the petab format.
 
         Parameters
         ----------
         rdatas:
             A list of rdatas as produced by
             ``pypesto.AmiciObjective.__call__(x, return_dict=True)['rdatas']``.
         model:
             The amici model.
+        verbose:
+            Passed to AMICI's model compilation. If True, the compilation
+            progress is printed.
 
         Returns
         -------
         A dataframe built from the rdatas in the format as in
         ``self.petab_problem.measurement_df``.
         """
         # create model
         if model is None:
-            model = self.create_model()
+            model = self.create_model(verbose=verbose)
 
         measurement_df = self.petab_problem.measurement_df
 
         return amici.petab_objective.rdatas_to_measurement_df(
             rdatas, model, measurement_df
         )
 
@@ -912,42 +958,76 @@
 def _find_model_name(output_folder: str) -> str:
     """Just re-use the last part of the output folder."""
     return os.path.split(os.path.normpath(output_folder))[-1]
 
 
 def get_petab_non_quantitative_data_types(
     petab_problem: petab.Problem,
-) -> List[str]:
+) -> set[str]:
     """
     Get the data types from the PEtab problem.
 
     Parameters
     ----------
     petab_problem:
         The PEtab problem.
 
     Returns
     -------
     data_types:
         A list of the data types.
     """
-    non_quantitative_data_types = []
-    if MEASUREMENT_TYPE in petab_problem.measurement_df.columns:
-        petab_data_types = petab_problem.measurement_df[
-            MEASUREMENT_TYPE
-        ].unique()
-        if ORDINAL in petab_data_types:
-            non_quantitative_data_types.append(ORDINAL)
-        if any(
-            censoring_type in petab_data_types
-            for censoring_type in CENSORING_TYPES
-        ):
-            non_quantitative_data_types.append(CENSORED)
-        if NONLINEAR_MONOTONE in petab_data_types:
-            non_quantitative_data_types.append(NONLINEAR_MONOTONE)
+    non_quantitative_data_types = set()
+    caught_observables = set()
+    # For ordinal, censored and semiquantitative data, search
+    # for the corresponding data types in the measurement table
+    meas_df = petab_problem.measurement_df
+    if MEASUREMENT_TYPE in meas_df.columns:
+        petab_data_types = meas_df[MEASUREMENT_TYPE].unique()
+        for data_type in [ORDINAL, SEMIQUANTITATIVE] + CENSORING_TYPES:
+            if data_type in petab_data_types:
+                non_quantitative_data_types.add(
+                    CENSORED if data_type in CENSORING_TYPES else data_type
+                )
+                caught_observables.update(
+                    set(
+                        meas_df[meas_df[MEASUREMENT_TYPE] == data_type][
+                            OBSERVABLE_ID
+                        ]
+                    )
+                )
+
+    # For relative data, search for parameters to estimate with
+    # a scaling/offset/sigma parameter type
+    if PARAMETER_TYPE in petab_problem.parameter_df.columns:
+        # get the df with non-nan parameter types
+        par_df = petab_problem.parameter_df[
+            petab_problem.parameter_df[PARAMETER_TYPE].notna()
+        ]
+        for par_id, row in par_df.iterrows():
+            if not row[ESTIMATE]:
+                continue
+            if row[PARAMETER_TYPE] in [
+                InnerParameterType.SCALING,
+                InnerParameterType.OFFSET,
+            ]:
+                non_quantitative_data_types.add(RELATIVE)
+
+            # For sigma parameters, we need to check if they belong
+            # to an observable with a non-quantitative data type
+            elif row[PARAMETER_TYPE] == InnerParameterType.SIGMA:
+                corresponding_observables = set(
+                    meas_df[meas_df[NOISE_PARAMETERS] == par_id][OBSERVABLE_ID]
+                )
+                if not (corresponding_observables & caught_observables):
+                    non_quantitative_data_types.add(RELATIVE)
+
+    # TODO this can be made much shorter if the relative measurements
+    # are also specified in the measurement table, but that would require
+    # changing the PEtab format of a lot of benchmark models.
 
     if len(non_quantitative_data_types) == 0:
         return None
     return non_quantitative_data_types
 
 
 class PetabStartpoints(CheckedStartpoints):
```

### Comparing `pypesto-0.4.1/pypesto/predict/amici_predictor.py` & `pypesto-0.4.2/pypesto/predict/amici_predictor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import TYPE_CHECKING, Callable, List, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Callable, Sequence, Union
 
 import numpy as np
 
 from ..C import (
     AMICI_LLH,
     AMICI_SIGMAY,
     AMICI_STATUS,
@@ -29,39 +29,41 @@
 )
 
 if TYPE_CHECKING:
     from ..objective import AmiciObjective
 
 from ..result import PredictionResult
 
+PostProcessor = Callable[[list[dict[str, np.array]]], list[np.ndarray]]
+
 
 class AmiciPredictor:
     """
     Do forward simulations/predictions for an AMICI model.
 
     The user may supply post-processing methods.
     If post-processing methods are supplied, and a gradient of the prediction
     is requested, then the sensitivities of the AMICI model must also be
     post-processed. There are no checks here to ensure that the sensitivities
     are correctly post-processed, this is explicitly left to the user.
     There are also no safeguards if the postprocessor routines fail. This may
-    happen if, e.g., a call to Amici fails, and no timepoints, states or
+    happen if, e.g., a call to AMICI fails, and no timepoints, states or
     observables are returned. As the AmiciPredictor is agnostic about the
     dimension of the postprocessor and also the dimension of the postprocessed
     output, these checks are also left to the user. An example for such a check
-    is provided in the default output (see _default_output()).
+    is provided in the default output (see :meth:`_default_output()`).
     """
 
     def __init__(
         self,
         amici_objective: AmiciObjective,
         amici_output_fields: Union[Sequence[str], None] = None,
-        post_processor: Union[Callable, None] = None,
-        post_processor_sensi: Union[Callable, None] = None,
-        post_processor_time: Union[Callable, None] = None,
+        post_processor: Union[PostProcessor, None] = None,
+        post_processor_sensi: Union[PostProcessor, None] = None,
+        post_processor_time: Union[PostProcessor, None] = None,
         max_chunk_size: Union[int, None] = None,
         output_ids: Union[Sequence[str], None] = None,
         condition_ids: Union[Sequence[str], None] = None,
     ):
         """
         Initialize predictor.
 
@@ -111,15 +113,15 @@
             Defaults to None, meaning that all conditions will be simulated.
         output_ids:
             IDs of outputs, as post-processing allows the creation of
             customizable outputs, which may not coincide with those from
             the AMICI model (defaults to AMICI observables).
         condition_ids:
             List of identifiers for the conditions of the edata objects of the
-            amici objective, will be passed to the PredictionResult at call.
+            amici objective, will be passed to the :class:`PredictionResult` at call.
         """
         # save settings and objective
         self.amici_objective = amici_objective
         self.max_chunk_size = max_chunk_size
         self.post_processor = post_processor
         self.post_processor_sensi = post_processor_sensi
         self.post_processor_time = post_processor_time
@@ -148,56 +150,55 @@
                 AMICI_SX,
             ]
         self.amici_output_fields = amici_output_fields
 
     def __call__(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...] = (0,),
+        sensi_orders: tuple[int, ...] = (0,),
         mode: ModeType = MODE_FUN,
         output_file: str = '',
         output_format: str = CSV,
         include_llh_weights: bool = False,
         include_sigmay: bool = False,
     ) -> PredictionResult:
         """
         Call the predictor.
 
         Simulate a model for a certain prediction function.
-        This method relies on the AmiciObjective, which is underlying, but
+        This method relies on the :class:`AmiciObjective`, which is underlying, but
         allows the user to apply any post-processing of the results, the
         sensitivities, and the timepoints.
 
         Parameters
         ----------
         x:
             The parameters for which to evaluate the prediction function.
         sensi_orders:
             Specifies which sensitivities to compute, e.g. (0,1) -> fval, grad.
         mode:
             Whether to compute function values or residuals.
         output_file:
             Path to an output file.
         output_format:
-            Either 'csv', 'h5'. If an output file is specified, this routine
+            Either ``'csv'`` or ``'h5'``. If an output file is specified, this routine
             will return a csv file, created from a DataFrame, or an h5 file,
             created from a dict.
         include_llh_weights:
             Boolean whether weights should be included in the prediction.
             Necessary for weighted means of Ensembles.
         include_sigmay:
             Boolean whether standard deviations should be included in the
             prediction output. Necessary for evaluation of weighted means
             of Ensembles.
 
         Returns
         -------
-        results:
-            PredictionResult object containing timepoints, outputs, and
-            output_sensitivities if requested
+        PredictionResult object containing timepoints, outputs, and
+        output sensitivities if requested.
         """
         # sanity check for output
         if 2 in sensi_orders:
             raise Exception(
                 'Prediction simulation does currently not support '
                 'second order output.'
             )
@@ -251,30 +252,36 @@
             # Do we want a pandas dataframe like format?
             if output_format == CSV:
                 results.write_to_csv(output_file=output_file)
             # Do we want an h5 file?
             elif output_format == H5:
                 results.write_to_h5(output_file=output_file)
             else:
-                raise Exception(
+                raise ValueError(
                     f'Call to unknown format {output_format} for '
                     f'output of pyPESTO prediction.'
                 )
 
         # return dependent on sensitivity order
         return results
 
     def _get_outputs(
         self,
         x: np.ndarray,
-        sensi_orders: Tuple[int, ...],
+        sensi_orders: tuple[int, ...],
         mode: ModeType = MODE_FUN,
         include_llh_weights: bool = False,
         include_sigmay: bool = False,
-    ) -> Tuple[List, List, List]:
+    ) -> tuple[
+        list[np.array],
+        list[np.array],
+        list[np.array],
+        list[np.array],
+        list[np.array],
+    ]:
         """
         Split the calls to amici into smaller chunks.
 
         Too large ReturnData objects from amici including many simulations
         can be problematic in terms of memory.
 
         Parameters
@@ -333,69 +340,87 @@
                 x=x,
                 sensi_orders=sensi_orders,
                 parameter_mapping=self.amici_objective.parameter_mapping[ids],
                 edatas=self.amici_objective.edatas[ids],
                 mode=mode,
             )
 
-        def _default_output(amici_outputs):
+        def _default_output(
+            amici_outputs: list[dict[str, np.array]]
+        ) -> tuple[
+            list[np.array],
+            list[np.array],
+            list[np.array],
+            list[np.array],
+            list[np.array],
+        ]:
             """
             Create default output of prediction.
 
             Equals to observables of AMICI model. We need to check that call
-            to AMICI was successful (status == 0), before writing the output.
+            to AMICI was successful (``status == 0``), before writing the output.
             """
             amici_nt = [
                 len(edata.getTimepoints())
                 for edata in self.amici_objective.edatas
             ]
             amici_ny = len(self.output_ids)
             amici_np = len(self.amici_objective.x_names)
 
             outputs = []
             outputs_sensi = []
             outputs_weights = []
             outputs_sigmay = []
             timepoints = [
-                amici_output[AMICI_T]
-                if amici_output[AMICI_STATUS] == 0
-                else np.full((amici_nt[i_condition],), np.nan)
+                (
+                    amici_output[AMICI_T]
+                    if amici_output[AMICI_STATUS] == 0
+                    else np.full((amici_nt[i_condition],), np.nan)
+                )
                 for i_condition, amici_output in enumerate(amici_outputs)
             ]
             # add outputs and sensitivities if requested
             if 0 in sensi_orders:
                 outputs = [
-                    amici_output[AMICI_Y]
-                    if amici_output[AMICI_STATUS] == 0
-                    else np.full((amici_nt[i_condition], amici_ny), np.nan)
+                    (
+                        amici_output[AMICI_Y]
+                        if amici_output[AMICI_STATUS] == 0
+                        else np.full((amici_nt[i_condition], amici_ny), np.nan)
+                    )
                     for i_condition, amici_output in enumerate(amici_outputs)
                 ]
             if 1 in sensi_orders:
                 outputs_sensi = [
-                    amici_output[AMICI_SY]
-                    if amici_output[AMICI_STATUS] == 0
-                    else np.full(
-                        (amici_nt[i_condition], amici_np, amici_ny), np.nan
+                    (
+                        amici_output[AMICI_SY]
+                        if amici_output[AMICI_STATUS] == 0
+                        else np.full(
+                            (amici_nt[i_condition], amici_np, amici_ny), np.nan
+                        )
                     )
                     for i_condition, amici_output in enumerate(amici_outputs)
                 ]
             # add likelihood as weights if requested
             if include_llh_weights:
                 outputs_weights = [
-                    amici_output[AMICI_LLH]
-                    if amici_output[AMICI_STATUS] == 0
-                    else np.nan
+                    (
+                        amici_output[AMICI_LLH]
+                        if amici_output[AMICI_STATUS] == 0
+                        else np.nan
+                    )
                     for i_condition, amici_output in enumerate(amici_outputs)
                 ]
             # add standard deviations if requested
             if include_sigmay:
                 outputs_sigmay = [
-                    amici_output[AMICI_SIGMAY]
-                    if amici_output[AMICI_STATUS] == 0
-                    else np.full((1, amici_ny), np.nan)
+                    (
+                        amici_output[AMICI_SIGMAY]
+                        if amici_output[AMICI_STATUS] == 0
+                        else np.full((1, amici_ny), np.nan)
+                    )
                     for i_condition, amici_output in enumerate(amici_outputs)
                 ]
 
             return (
                 timepoints,
                 outputs,
                 outputs_sensi,
@@ -428,16 +453,22 @@
             outputs,
             outputs_sensi,
             outputs_weights,
             outputs_sigmay,
         )
 
     def _wrap_call_to_amici(
-        self, amici_outputs, x, sensi_orders, mode, parameter_mapping, edatas
-    ):
+        self,
+        amici_outputs: list,
+        x: np.array,
+        sensi_orders: tuple[int, ...],
+        mode: ModeType,
+        parameter_mapping,
+        edatas,
+    ) -> None:
         """
         Encapsulate the call to amici.
 
         This allows to use variable scoping as a mean to clean up the memory
         after calling amici, which is beneficial if large models with large
         datasets are used.
         """
```

### Comparing `pypesto-0.4.1/pypesto/predict/task.py` & `pypesto-0.4.2/pypesto/predict/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/problem/base.py` & `pypesto-0.4.2/pypesto/problem/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/profile/approximate.py` & `pypesto-0.4.2/pypesto/profile/approximate.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/profile/options.py` & `pypesto-0.4.2/pypesto/profile/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/profile/profile.py` & `pypesto-0.4.2/pypesto/profile/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     optimizer: Optimizer,
     engine: Engine = None,
     profile_index: Iterable[int] = None,
     profile_list: int = None,
     result_index: int = 0,
     next_guess_method: Union[Callable, str] = 'adaptive_step_regression',
     profile_options: ProfileOptions = None,
-    progress_bar: bool = True,
+    progress_bar: bool = None,
     filename: Union[str, Callable, None] = None,
     overwrite: bool = False,
 ) -> Result:
     """
     Compute parameter profiles.
 
     Parameters
```

### Comparing `pypesto-0.4.1/pypesto/profile/profile_next_guess.py` & `pypesto-0.4.2/pypesto/profile/profile_next_guess.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/profile/task.py` & `pypesto-0.4.2/pypesto/profile/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/profile/util.py` & `pypesto-0.4.2/pypesto/profile/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility function for profile module."""
+
 from typing import Any, Iterable
 
 import numpy as np
 import scipy.stats
 
 from ..C import GRAD
 from ..problem import Problem
```

### Comparing `pypesto-0.4.1/pypesto/profile/validation_intervals.py` & `pypesto-0.4.2/pypesto/profile/validation_intervals.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/profile/walk_along_profile.py` & `pypesto-0.4.2/pypesto/profile/walk_along_profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/result/optimize.py` & `pypesto-0.4.2/pypesto/result/optimize.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
         self.fval0: float = fval0
         self.history: HistoryBase = history
         self.exitflag: int = exitflag
         self.time: float = time
         self.message: str = message
         self.optimizer = optimizer
         self.free_indices = None
+        self.inner_parameters = None
 
     def __getattr__(self, key):
         try:
             return self[key]
         except KeyError:
             raise AttributeError(key)
 
@@ -151,15 +152,15 @@
             full = True
         message = (
             "### Optimizer Result\n\n"
             f"* optimizer used: {self.optimizer}\n"
             f"* message: {self.message} \n"
             f"* number of evaluations: {self.n_fval}\n"
             f"* time taken to optimize: {self.time:0.3f}s\n"
-            f"* startpoint: {self.x0 if full else self.x0[self.free_indices]}\n"
+            f"* startpoint: {self.x0 if full or self.x0 is None else self.x0[self.free_indices]}\n"
             f"* endpoint: {self.x if full else self.x[self.free_indices]}\n"
         )
         # add fval, gradient, hessian, res, sres if available
         if self.fval is not None:
             message += f"* final objective value: {self.fval}\n"
         if self.grad is not None:
             message += (
```

### Comparing `pypesto-0.4.1/pypesto/result/predict.py` & `pypesto-0.4.2/pypesto/result/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,17 +138,19 @@
             prediction (e.g., PEtab uses tuples of preequilibration condition
             and simulation conditions)
         comment:
             An additional note, which can be attached to this prediction
         """
         # cast the result per condition
         self.conditions = [
-            cond
-            if isinstance(cond, PredictionConditionResult)
-            else PredictionConditionResult(**cond)
+            (
+                cond
+                if isinstance(cond, PredictionConditionResult)
+                else PredictionConditionResult(**cond)
+            )
             for cond in conditions
         ]
 
         self.condition_ids = condition_ids
         if self.condition_ids is None:
             self.condition_ids = [
                 get_condition_label(i_cond)
```

### Comparing `pypesto-0.4.1/pypesto/result/profile.py` & `pypesto-0.4.2/pypesto/result/profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/result/result.py` & `pypesto-0.4.2/pypesto/result/result.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/result/sample.py` & `pypesto-0.4.2/pypesto/result/sample.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/sample/__init__.py` & `pypesto-0.4.2/pypesto/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/sample/adaptive_metropolis.py` & `pypesto-0.4.2/pypesto/sample/adaptive_metropolis.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             # diag matrix to the cov matrix with elements of this factor
             'reg_factor': 1e-6,
             # initial covariance matrix. defaults to a unit matrix
             'cov0': None,
             # target acceptance rate
             'target_acceptance_rate': 0.234,
             # show progress
-            'show_progress': True,
+            'show_progress': None,
         }
 
     def initialize(self, problem: Problem, x0: np.ndarray):
         """Initialize the sampler."""
         super().initialize(problem, x0)
 
         if self.options['cov0'] is not None:
```

### Comparing `pypesto-0.4.1/pypesto/sample/adaptive_parallel_tempering.py` & `pypesto-0.4.2/pypesto/sample/adaptive_parallel_tempering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """AdaptiveParallelTemperingSampler class."""
+
 from typing import Dict, Sequence
 
 import numpy as np
 
 from .parallel_tempering import ParallelTemperingSampler
```

### Comparing `pypesto-0.4.1/pypesto/sample/auto_correlation.py` & `pypesto-0.4.2/pypesto/sample/auto_correlation.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/sample/diagnostics.py` & `pypesto-0.4.2/pypesto/sample/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Calculate different diagnostics of the sampling result."""
+
 import logging
 
 import numpy as np
 
 from ..result import Result
 from .auto_correlation import autocorrelation_sokal
 from .geweke_test import burn_in_by_sequential_geweke
```

### Comparing `pypesto-0.4.1/pypesto/sample/dynesty.py` & `pypesto-0.4.2/pypesto/sample/dynesty.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/sample/emcee.py` & `pypesto-0.4.2/pypesto/sample/emcee.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/sample/geweke_test.py` & `pypesto-0.4.2/pypesto/sample/geweke_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper function for `geweke_test`."""
+
 import logging
 import warnings
 from typing import Tuple
 
 import numpy as np
 from scipy.stats import norm
```

### Comparing `pypesto-0.4.1/pypesto/sample/metropolis.py` & `pypesto-0.4.2/pypesto/sample/metropolis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Dict, Sequence, Union
 
 import numpy as np
-from tqdm import tqdm
 
 from ..history import NoHistory
 from ..objective import NegLogPriors, ObjectiveBase
 from ..problem import Problem
 from ..result import McmcPtResult
+from ..util import tqdm
 from .sampler import InternalSample, InternalSampler
 
 
 class MetropolisSampler(InternalSampler):
     """Simple Metropolis-Hastings sampler with fixed proposal variance.
 
     The Metropolis-Hastings sampler is a Markov chain Monte Carlo (MCMC)
@@ -47,15 +47,15 @@
         self.temper_lpost: bool = False
 
     @classmethod
     def default_options(cls):
         """Return the default options for the sampler."""
         return {
             'std': 1.0,  # the proposal standard deviation
-            'show_progress': True,  # whether to show the progress
+            'show_progress': None,  # whether to show the progress
         }
 
     def initialize(self, problem: Problem, x0: np.ndarray):
         """Initialize the sampler."""
         self.problem = problem
         self.neglogpost = problem.objective
         self.neglogpost.history = NoHistory()
@@ -69,18 +69,18 @@
 
     def sample(self, n_samples: int, beta: float = 1.0):
         """Load last recorded particle."""
         x = self.trace_x[-1]
         lpost = -self.trace_neglogpost[-1]
         lprior = -self.trace_neglogprior[-1]
 
-        show_progress = self.options['show_progress']
+        show_progress = self.options.get('show_progress', None)
 
         # loop over iterations
-        for _ in tqdm(range(int(n_samples)), disable=not show_progress):
+        for _ in tqdm(range(int(n_samples)), enable=show_progress):
             # perform step
             x, lpost, lprior = self._perform_step(
                 x=x, lpost=lpost, lprior=lprior, beta=beta
             )
             # record step
             self.trace_x.append(x)
             self.trace_neglogpost.append(-lpost)
```

### Comparing `pypesto-0.4.1/pypesto/sample/parallel_tempering.py` & `pypesto-0.4.2/pypesto/sample/parallel_tempering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from typing import Dict, List, Sequence, Union
 
 import numpy as np
-from tqdm import tqdm
 
 from ..problem import Problem
 from ..result import McmcPtResult
+from ..util import tqdm
 from .sampler import InternalSampler, Sampler
 
 
 class ParallelTemperingSampler(Sampler):
     """Simple parallel tempering sampler.
 
     Parallel tempering is a Markov chain Monte Carlo (MCMC) method that
@@ -66,15 +66,15 @@
     @classmethod
     def default_options(cls) -> Dict:
         """Return the default options for the sampler."""
         return {
             'max_temp': 5e4,
             'exponent': 4,
             'temper_log_posterior': False,
-            'show_progress': True,
+            'show_progress': None,
         }
 
     def initialize(
         self, problem: Problem, x0: Union[np.ndarray, List[np.ndarray]]
     ):
         """Initialize all samplers."""
         n_chains = len(self.samplers)
@@ -85,17 +85,17 @@
         for sampler, x0 in zip(self.samplers, x0s):
             _problem = copy.deepcopy(problem)
             sampler.initialize(_problem, x0)
         self.betas = self.betas0
 
     def sample(self, n_samples: int, beta: float = 1.0):
         """Sample and swap in between samplers."""
-        show_progress = self.options['show_progress']
+        show_progress = self.options.get('show_progress', None)
         # loop over iterations
-        for i_sample in tqdm(range(int(n_samples)), disable=not show_progress):
+        for i_sample in tqdm(range(int(n_samples)), enable=show_progress):
             # TODO test
             # sample
             for sampler, beta in zip(self.samplers, self.betas):
                 sampler.sample(n_samples=1, beta=beta)
 
             # swap samples
             swapped = self.swap_samples()
```

### Comparing `pypesto-0.4.1/pypesto/sample/pymc.py` & `pypesto-0.4.2/pypesto/sample/pymc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Pymc v4 Sampler."""
+
 from __future__ import annotations
 
 import logging
 from typing import Union
 
 import arviz as az
 import numpy as np
```

### Comparing `pypesto-0.4.1/pypesto/sample/sample.py` & `pypesto-0.4.2/pypesto/sample/sample.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/sample/sampler.py` & `pypesto-0.4.2/pypesto/sample/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Various Sampler classes."""
+
 import abc
 from typing import Dict, List, Union
 
 import numpy as np
 
 from ..problem import Problem
 from ..result import McmcPtResult
```

### Comparing `pypesto-0.4.1/pypesto/sample/util.py` & `pypesto-0.4.2/pypesto/sample/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A set of helper functions."""
+
 import logging
 import os
 from typing import Tuple
 
 import numpy as np
 
 from ..C import PYPESTO_MAX_N_SAMPLES
```

### Comparing `pypesto-0.4.1/pypesto/select/__init__.py` & `pypesto-0.4.2/pypesto/select/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Model Selection
 ===============
 
-Perform model selection with a PEtab Select problem.
+Perform model selection with a
+`PEtab Select <https://petab-select.readthedocs.io/>`_ problem.
 """
 
 from . import postprocessors
 from .misc import model_to_pypesto_problem
 from .problem import Problem
 
 try:
```

### Comparing `pypesto-0.4.1/pypesto/select/method.py` & `pypesto-0.4.2/pypesto/select/method.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Functionality related to using a PEtab Select model selection method."""
+
 import logging
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Optional
 
 import numpy as np
 import petab_select
 from petab_select import (
     VIRTUAL_INITIAL_MODEL,
     CandidateSpace,
     Criterion,
@@ -51,15 +52,15 @@
     column_width:
         The width of columns when logging.
     column_sep:
         The substring used to separate column values when logging.
     level:
         The logging level.
     logger:
-        A logger from the `logging` module.
+        A logger from the :mod:`logging` module.
     """
 
     column_width: int = 12
     column_sep: str = " | "
 
     def __init__(self, level: str = 'info'):
         self.logger = logging.getLogger(__name__)
@@ -134,16 +135,15 @@
             Parameters
             ----------
             model:
                 The model.
 
             Returns
             -------
-            str
-                The ID.
+            The ID.
             """
             model_subspace_id = model.model_subspace_id or ''
             original_model_id = model.model_id or model.get_hash()
             model_id = model_subspace_id + ':' + original_model_id
             return model_id
 
         def float_to_str(value: float, precision: int = 3) -> str:
@@ -189,86 +189,104 @@
     """Handle calls to PEtab Select model selection methods.
 
     Attributes
     ----------
     petab_select_problem:
         The PEtab Select problem.
     candidate_space:
-        A `petab_select.CandidateSpace`, used to generate candidate models.
+        A :class:`petab_select.CandidateSpace`, used to generate candidate models.
     criterion:
         The criterion by which models will be compared.
     criterion_threshold:
-        The minimum improvement in criterion that a test model must have to
+        The minimum improvement in `criterion` that a test model must have to
         be selected. The comparison is made according to the method. For
         example, in `ForwardSelector`, test models are compared to the
         previously selected model.
     calibrated_models:
         The calibrated models of the model selection, as a `dict` where keys
         are model hashes and values are models.
     limit:
         Limit the number of calibrated models. NB: the number of accepted
         models may (likely) be fewer.
     logger:
-        A `MethodLogger`, used to log results.
-    minimize_options:
-        A dictionary that will be passed to `pypesto.minimize` as keyword
-        arguments for model optimization.
-    model_postprocessor:
-        A method that is applied to each model after calibration.
-    objective_customizer:
-        A method that is applied to the pyPESTO objective after the
-        objective is initialized, before calibration.
+        A :class:`MethodLogger`, used to log results.
     predecessor_model:
         Specify the predecessor (initial) model for the model selection
-        algorithm. If `None`, then the algorithm will generate an
+        algorithm. If ``None``, then the algorithm will generate an initial
         predecessor model if required.
     select_first_improvement:
-        If `True`, model selection will terminate as soon as a better model
+        If ``True``, model selection will terminate as soon as a better model
         is found. If `False`, all candidate models will be tested.
     startpoint_latest_mle:
-        If `True`, one of the startpoints in the multistart optimization
+        If ``True``, one of the startpoints in the multistart optimization
         will be the MLE of the latest model.
     """
 
     def __init__(
         self,
         petab_select_problem: petab_select.Problem,
-        calibrated_models: Dict[str, Model],
+        calibrated_models: dict[str, Model],
         # Arguments/attributes that can simply take the default value here.
         criterion_threshold: float = 0.0,
         limit: int = np.inf,
-        minimize_options: Dict = None,
+        # TODO deprecated
+        minimize_options: dict = None,
+        # TODO deprecated
         model_postprocessor: TYPE_POSTPROCESSOR = None,
+        # TODO deprecated
         objective_customizer: Callable = None,
         select_first_improvement: bool = False,
         startpoint_latest_mle: bool = True,
         # Arguments/attributes that should be handled more carefully.
         candidate_space: CandidateSpace = None,
         criterion: Criterion = None,
         # TODO misleading, `Method` here is simply an Enum, not a callable...
         method: Method = None,
         predecessor_model: Model = None,
+        # TODO deprecated
         model_to_pypesto_problem_method: Callable[[Any], Problem] = None,
+        model_problem_options: dict = None,
     ):
         """Arguments are used in every `__call__`, unless overridden."""
         self.petab_select_problem = petab_select_problem
         self.calibrated_models = calibrated_models
 
         self.criterion_threshold = criterion_threshold
         self.limit = limit
-        self.minimize_options = minimize_options
-        self.model_postprocessor = model_postprocessor
-        self.objective_customizer = objective_customizer
         self.predecessor_model = predecessor_model
         self.select_first_improvement = select_first_improvement
         self.startpoint_latest_mle = startpoint_latest_mle
-        self.model_to_pypesto_problem_method = model_to_pypesto_problem_method
 
         self.logger = MethodLogger()
 
+        # TODO deprecated
+        old_model_problem_options = {}
+        for key, value in [
+            ('postprocessor', model_postprocessor),
+            (
+                'model_to_pypesto_problem_method',
+                model_to_pypesto_problem_method,
+            ),
+            ('minimize_options', minimize_options),
+            ('objective_customizer', objective_customizer),
+        ]:
+            if value is not None:
+                old_model_problem_options[key] = value
+                self.logger.log(
+                    f'Specifying `{key}` as an individual argument is '
+                    'deprecated. Please instead specify it within some '
+                    '`model_problem_options` dictionary, e.g. '
+                    f'`model_problem_options={{"{key}": ...}}`.',
+                    level='warning',
+                )
+        self.model_problem_options = {}
+        self.model_problem_options |= old_model_problem_options
+        if model_problem_options is not None:
+            self.model_problem_options |= model_problem_options
+
         self.criterion = criterion
         if self.criterion is None:
             self.criterion = self.petab_select_problem.criterion
 
         # Forbid specification of both a candidate space and a method.
         if candidate_space is not None and method is not None:
             self.logger.log(
@@ -278,17 +296,19 @@
                 ),
                 level='warning',
             )
         # Get method.
         self.method = (
             method
             if method is not None
-            else candidate_space.method
-            if candidate_space is not None
-            else self.petab_select_problem.method
+            else (
+                candidate_space.method
+                if candidate_space is not None
+                else self.petab_select_problem.method
+            )
         )
         # Require either a candidate space or a method.
         if candidate_space is None and self.method is None:
             raise ValueError(
                 'Please provide one of either `candidate_space` or `method`, '
                 'or specify the `method` in the PEtab Select problem.'
             )
@@ -313,53 +333,43 @@
                     )
                 )
         # May have changed from `None` to `petab_select.VIRTUAL_INITIAL_MODEL`
         self.predecessor_model = self.candidate_space.get_predecessor_model()
 
     def __call__(
         self,
-        predecessor_model: Optional[Union[Model, None]] = None,
-        newly_calibrated_models: Optional[Dict[str, Model]] = None,
-    ) -> Tuple[List[Model], Dict[str, Model]]:
+        newly_calibrated_models: Optional[dict[str, Model]] = None,
+    ) -> tuple[list[Model], dict[str, Model]]:
         """Run a single iteration of the model selection method.
 
         A single iteration here refers to calibration of all candidate models.
         For example, given a predecessor model with 3 estimated parameters,
         with the forward method, a single iteration would involve calibration
         of all models that have both: the same 3 estimated parameters; and 1
-        additional estimated paramenter.
+        additional estimated parameter.
 
         The input `newly_calibrated_models` is from the previous iteration. The
         output `newly_calibrated_models` is from the current iteration.
 
         Parameters
         ----------
-        predecessor_model:
-            The model that will be used for comparison. Example 1: the
-            initial model of a forward method. Example 2: all models found
-            with a brute force method should be better than this model.
         newly_calibrated_models:
             The newly calibrated models from the previous iteration.
 
         Returns
         -------
-        tuple
-            A 2-tuple, with the following values:
+        A 2-tuple, with the following values:
 
-               1. the predecessor model for the newly calibrated models; and
-               2. the newly calibrated models, as a `dict` where keys are model
-                  hashes and values are models.
+           1. the predecessor model for the newly calibrated models; and
+           2. the newly calibrated models, as a `dict` where keys are model
+              hashes and values are models.
         """
         # All calibrated models in this iteration (see second return value).
         self.logger.new_selection()
 
-        if predecessor_model is None:
-            # May still be `None` (e.g. brute force method)
-            predecessor_model = self.predecessor_model
-
         candidate_space = petab_select.ui.candidates(
             problem=self.petab_select_problem,
             candidate_space=self.candidate_space,
             limit=self.limit,
             calibrated_models=self.calibrated_models,
             newly_calibrated_models=newly_calibrated_models,
             excluded_model_hashes=self.calibrated_models.keys(),
@@ -402,16 +412,15 @@
         model:
             The calibrated model.
         predecessor_model:
             The predecessor model.
 
         Returns
         -------
-        MethodSignal
-            A `MethodSignal` that describes the result.
+        A :class:`MethodSignal` that describes the result.
         """
         # Use the predecessor model from `__init__` if an iteration-specific
         # predecessor model was not supplied to `__call__`.
         if predecessor_model is None:
             # May still be `None` after this assignment.
             predecessor_model = self.predecessor_model
 
@@ -461,17 +470,16 @@
         model1:
             The new model.
         model0:
             The original model.
 
         Returns
         -------
-        bool
-            `True`, if `model1` is superior to `model0` by the criterion,
-            else `False`.
+        ``True``, if `model1` is superior to `model0` by the criterion,
+        else ``False``.
         """
         if self.criterion in [
             Criterion.AIC,
             Criterion.AICC,
             Criterion.BIC,
             Criterion.LH,
             Criterion.LLH,
@@ -505,16 +513,15 @@
             Whether the model should be considered a valid model. If it is
             not valid, it will not be calibrated.
         autorun:
             Whether the model should be calibrated upon creation.
 
         Returns
         -------
-        ModelProblem
-            The model selection problem.
+        The model selection problem.
         """
         x_guess = None
         if (
             self.startpoint_latest_mle
             and model.predecessor_model_hash in self.calibrated_models
         ):
             predecessor_model = self.calibrated_models[
@@ -534,12 +541,9 @@
 
         return ModelProblem(
             model=model,
             criterion=self.criterion,
             valid=valid,
             autorun=autorun,
             x_guess=x_guess,
-            minimize_options=self.minimize_options,
-            objective_customizer=self.objective_customizer,
-            postprocessor=self.model_postprocessor,
-            model_to_pypesto_problem_method=self.model_to_pypesto_problem_method,
+            **self.model_problem_options,
         )
```

### Comparing `pypesto-0.4.1/pypesto/select/misc.py` & `pypesto-0.4.2/pypesto/select/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Miscellaneous methods."""
+
 import logging
-from typing import Dict, Iterable
+from typing import Iterable
 
+import pandas as pd
 import petab
 import petab_select.ui
 from petab.C import ESTIMATE, NOMINAL_VALUE
 from petab_select import Model, parameter_string_to_value
 from petab_select.constants import PETAB_PROBLEM
 
 from ..objective import Objective
@@ -14,15 +16,16 @@
 
 logger = logging.getLogger(__name__)
 
 
 def model_to_pypesto_problem(
     model: Model,
     objective: Objective = None,
-    x_guesses: Iterable[Dict[str, float]] = None,
+    x_guesses: Iterable[dict[str, float]] = None,
+    hierarchical: bool = False,
 ) -> Problem:
     """Create a pyPESTO problem from a PEtab Select model.
 
     Parameters
     ----------
     model:
         The model.
@@ -32,56 +35,91 @@
         Startpoints to be used in the multi-start optimization. For example,
         this could be the maximum likelihood estimate from another model.
         Each dictionary has parameter IDs as keys, and parameter values as
         values.
         Values in `x_guess` for parameters that are not estimated will be
         ignored and replaced with their value from the PEtab Select model, if
         defined, else their nominal value in the PEtab parameters table.
+    hierarchical:
+        Whether the problem involves hierarchical optimization.
 
     Returns
     -------
-    Problem
-        The pyPESTO select problem.
+    The pyPESTO select problem.
     """
     petab_problem = petab_select.ui.model_to_petab(model=model)[PETAB_PROBLEM]
 
     corrected_x_guesses = None
     if x_guesses is not None:
         corrected_x_guesses = correct_x_guesses(
             x_guesses=x_guesses,
             model=model,
             petab_problem=petab_problem,
+            hierarchical=hierarchical,
         )
 
-    importer = PetabImporter(petab_problem)
+    importer = PetabImporter(
+        petab_problem,
+        hierarchical=hierarchical,
+    )
     if objective is None:
         amici_model = importer.create_model(
             non_estimated_parameters_as_constants=False,
         )
         objective = importer.create_objective(
             model=amici_model,
         )
     pypesto_problem = importer.create_problem(
         objective=objective,
         x_guesses=corrected_x_guesses,
     )
     return pypesto_problem
 
 
+def model_to_hierarchical_pypesto_problem(*args, **kwargs) -> Problem:
+    """Create a hierarchical pyPESTO problem from a PEtab Select model.
+
+    See :func:`model_to_pypesto_problem`.
+    """
+    pypesto_problem = model_to_pypesto_problem(
+        *args,
+        **kwargs,
+        hierarchical=True,
+    )
+    return pypesto_problem
+
+
 def correct_x_guesses(
-    x_guesses: Iterable[Dict[str, float]],
+    x_guesses: Iterable[dict[str, float]],
     model: Model,
     petab_problem: petab.Problem = None,
+    hierarchical: bool = False,
 ):
     """Fix startpoint guesses passed between models of different sizes.
 
     Any parameter values in `x_guess` for parameters that are not estimated
     should be corrected by replacing them with
     - their corresponding values in `row` if possible, else
     - their corresponding nominal values in the `petab_problem.parameter_df`.
+
+    Parameters
+    ----------
+    x_guesses:
+        The startpoints to correct.
+    model:
+        The startpoints will be corrected to match this model.
+    petab_problem:
+        The model's corresponding PEtab problem. If this is not provided,
+        it will be created from the `model`.
+    hierarchical:
+        Whether hierarchical optimization is used.
+
+    Returns
+    -------
+    The corrected startpoint guesses.
     """
     # TODO reconsider whether correcting is a good idea (`x_guess` is no longer
     # the latest MLE then). Similar todo exists in
     # `ModelSelectorMethod.new_model_problem`.
     # TODO move to PEtab Select?
     # TODO may be issues, e.g. differences in bounds of parameters between
     #      different model PEtab problems is not accounted for, or if there are
@@ -94,14 +132,22 @@
 
     corrected_x_guesses = None
     if x_guesses is not None:
         corrected_x_guesses = []
         for x_guess in x_guesses:
             corrected_x_guess = []
             for parameter_id in petab_problem.parameter_df.index:
+                if hierarchical:
+                    if not pd.isna(
+                        petab_problem.parameter_df.loc[
+                            parameter_id, "parameterType"
+                        ]
+                    ):
+                        continue
+
                 # Use the `x_guess` value, if the parameter is to be estimated.
                 if (
                     petab_problem.parameter_df[ESTIMATE].loc[parameter_id] == 1
                     and parameter_id in x_guess
                 ):
                     corrected_value = x_guess[parameter_id]
                 # Else use the PEtab Select model parameter value, if defined.
```

### Comparing `pypesto-0.4.1/pypesto/select/model_problem.py` & `pypesto-0.4.2/pypesto/select/model_problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Calibrate a PEtab Select model with pyPESTO."""
+
 import time
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Optional
 
 from petab_select import Criterion, Model
 
 from ..objective import ObjectiveBase
 from ..optimize import minimize
 from ..problem import Problem
 from ..result import OptimizerResult, Result
@@ -25,19 +26,23 @@
     Attributes
     ----------
     best_start:
         The best start from a pyPESTO optimize result.
     criterion:
         The criterion that should be computed after the model is
         calibrated.
+    minimize_method:
+        The optimization method, which should take a :class:``Problem`` as its
+        only required positional argument, and return a :class:``Result`` that
+        contains an :class:``OptimizerResult``. Other arguments can be provided
+        as keyword arguments, via ``minimize_options``.
     minimize_options:
-        Keyword argument options that will be passed on to
-        :func:`pypesto.optimize.minimize`.
+        Keyword argument options that will be passed on to `minimize_method`.
     minimize_result:
-        A pyPESTO result with an optimize result.
+        A pyPESTO result with an `optimize` result.
     model:
         A PEtab Select model.
     model_id:
         The ID of the PEtab Select model.
     objective_customizer:
         A method that takes a :class:`pypesto.objective.AmiciObjective` as
         input, and makes changes to the objective in-place.
@@ -57,40 +62,44 @@
 
     def __init__(
         self,
         model: Model,
         criterion: Criterion,
         valid: bool = True,
         autorun: bool = True,
-        x_guess: List[float] = None,
-        minimize_options: Dict = None,
+        x_guess: list[float] = None,
+        minimize_options: dict = None,
         objective_customizer: Optional[OBJECTIVE_CUSTOMIZER_TYPE] = None,
         postprocessor: Optional["TYPE_POSTPROCESSOR"] = None,
         model_to_pypesto_problem_method: Callable[[Any], Problem] = None,
+        minimize_method: Callable[[Problem], Result] = None,
     ):
         """Construct then calibrate a model problem.
 
         See the class documentation for documentation of most parameters.
 
         Parameters
         ----------
         autorun:
             If ``False``, the model parameters will not be estimated. Allows
-            users to manually call ``pypesto.minimize`` with custom options,
-            then :meth:`set_result()`.
+            users to manually call ``pypesto.optimize.minimize`` with custom
+            options, then :meth:`set_result()`.
 
         TODO: constraints
         """
         self.model = model
         self.criterion = criterion
         self.valid = valid
 
         self.minimize_options = {}
         if minimize_options is not None:
             self.minimize_options = minimize_options
+        self.minimize_method = minimize
+        if minimize_method is not None:
+            self.minimize_method = minimize_method
 
         self.model_id = self.model.model_id
         self.objective_customizer = objective_customizer
         self.postprocessor = postprocessor
         self.best_start = None
         self.minimize_result = None
         self.x_guess = x_guess
@@ -124,49 +133,57 @@
                             fval=fake_result_fval,
                             evaluation_time=fake_result_evaluation_time,
                         )
                     )
                 # TODO rename `minimize_options` to `minimize_kwargs`.
                 # TODO or allow users to provide custom `minimize` methods?
                 else:
-                    self.set_result(
-                        minimize(
-                            self.pypesto_problem,
-                            **minimize_options,
-                        )
-                    )
+                    self.set_result(self.minimize())
+
+    def minimize(self) -> Result:
+        """Optimize the model.
+
+        Returns:
+            The optimization result.
+        """
+        return self.minimize_method(
+            self.pypesto_problem,
+            **self.minimize_options,
+        )
 
     def set_result(self, result: Result):
         """Postprocess a result.
 
         Parameters
         ----------
         result:
-            A pyPESTO result with an optimize result.
+            A pyPESTO result with an `optimize` result.
         """
         self.minimize_result = result
         # TODO extract best parameter estimates, to use as start point for
         # subsequent models in model selection, for parameters in those models
         # that were estimated in this model.
         self.best_start = self.minimize_result.optimize_result.list[0]
         self.model.set_criterion(Criterion.NLLH, float(self.best_start.fval))
         self.model.compute_criterion(criterion=self.criterion)
 
-        self.model.estimated_parameters = {
+        estimated_parameters = {
             id: float(value)
             for index, (id, value) in enumerate(
-                dict(
-                    zip(
-                        self.pypesto_problem.x_names,
-                        self.best_start.x,
-                    )
-                ).items()
+                zip(
+                    self.pypesto_problem.x_names,
+                    self.best_start.x,
+                )
             )
             if index in self.pypesto_problem.x_free_indices
         }
+        self.model.set_estimated_parameters(
+            estimated_parameters=estimated_parameters,
+            scaled=True,
+        )
 
         if self.postprocessor is not None:
             self.postprocessor(self)
 
 
 def create_fake_pypesto_result_from_fval(
     fval: float,
```

### Comparing `pypesto-0.4.1/pypesto/select/postprocessors.py` & `pypesto-0.4.2/pypesto/select/postprocessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Process a model selection :class:`ModelProblem` after calibration."""
+
 from pathlib import Path
-from typing import List
 
 import matplotlib.pyplot as plt
 import numpy as np
 from petab_select.constants import ESTIMATE, TYPE_PATH, Criterion
 
 from .. import store, visualize
 from .model_problem import TYPE_POSTPROCESSOR, ModelProblem
@@ -16,15 +16,15 @@
     'save_postprocessor',
     'waterfall_plot_postprocessor',
 ]
 
 
 def multi_postprocessor(
     problem: ModelProblem,
-    postprocessors: List[TYPE_POSTPROCESSOR] = None,
+    postprocessors: list[TYPE_POSTPROCESSOR] = None,
 ):
     """Combine multiple postprocessors into a single postprocessor.
 
     See :meth:`save_postprocessor` for usage hints.
 
     Parameters
     ----------
@@ -114,15 +114,15 @@
         model_id += "1" if parameter_value == ESTIMATE else "0"
     problem.model.model_id = model_id
 
 
 def report_postprocessor(
     problem: ModelProblem,
     output_filepath: TYPE_PATH,
-    criteria: List[Criterion] = None,
+    criteria: list[Criterion] = None,
 ):
     """Create a TSV table of model selection results.
 
     Parameters
     ----------
     problem:
         A model selection :class:`ModelProblem` that has been optimized.
```

### Comparing `pypesto-0.4.1/pypesto/select/problem.py` & `pypesto-0.4.2/pypesto/select/problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Manage all components of a pyPESTO model selection problem."""
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+
+import warnings
+from typing import Any, Iterable, Optional
 
 import petab_select
 from petab_select import Model
 
 from .method import MethodCaller
 from .model_problem import TYPE_POSTPROCESSOR, ModelProblem  # noqa: F401
 
@@ -22,29 +24,41 @@
         model hashes, and values are :class:`petab_select.Model` objects.
     newly_calibrated_models:
         Storage for models that were calibrated in the previous iteration of
         model selection. Same type as ``calibrated_models``.
     method_caller:
         A :class:`MethodCaller`, used to run a single iteration of a model
         selection method.
-    model_postprocessor:
-        A method that is applied to each model after calibration.
+    model_problem_options:
+        Passed to the constructor of :class:``ModelProblem``.
     petab_select_problem:
         A PEtab Select problem.
     """
 
     # FIXME rename `best_model` to `selected_model` everywhere
 
     def __init__(
         self,
         petab_select_problem: petab_select.Problem,
         model_postprocessor: Optional[TYPE_POSTPROCESSOR] = None,
+        model_problem_options: dict = None,
     ):
         self.petab_select_problem = petab_select_problem
-        self.model_postprocessor = model_postprocessor
+
+        self.model_problem_options = {}
+        if model_problem_options is not None:
+            self.model_problem_options = model_problem_options
+        # TODO deprecated
+        if model_postprocessor is not None:
+            warnings.warn(
+                'Specifying `model_postprocessor` directly is deprecated. '
+                'Please specify it with `model_problem_options`, e.g. '
+                'model_problem_options={"postprocessor": ...}`.'
+            )
+            self.model_problem_options['postprocessor'] = model_postprocessor
 
         self.set_state(
             calibrated_models={},
             newly_calibrated_models={},
         )
 
         # TODO default caller, based on petab_select.Problem
@@ -53,52 +67,56 @@
     def create_method_caller(self, **kwargs) -> MethodCaller:
         """Create a method caller.
 
         ``kwargs`` are passed to the :class:`MethodCaller` constructor.
 
         Returns
         -------
-        MethodCaller
-            A `MethodCaller` instance.
+        A :class:`MethodCaller` instance.
         """
+        kwargs = kwargs.copy()
+        model_problem_options = self.model_problem_options | kwargs.pop(
+            'model_problem_options', {}
+        )
+
         return MethodCaller(
             petab_select_problem=self.petab_select_problem,
             calibrated_models=self.calibrated_models,
-            model_postprocessor=self.model_postprocessor,
+            model_problem_options=model_problem_options,
             **kwargs,
         )
 
     def set_state(
         self,
-        calibrated_models: Dict[str, Model],
-        newly_calibrated_models: Dict[str, Model],
+        calibrated_models: dict[str, Model],
+        newly_calibrated_models: dict[str, Model],
     ) -> None:
         """Set the state of the problem.
 
         See :class:`Problem` attributes for argument documentation.
         """
         self.calibrated_models = calibrated_models
         self.newly_calibrated_models = newly_calibrated_models
 
     def update_with_newly_calibrated_models(
         self,
-        newly_calibrated_models: Optional[Dict[str, Model]] = None,
+        newly_calibrated_models: Optional[dict[str, Model]] = None,
     ) -> None:
         """Update the state of the problem with newly calibrated models.
 
         Args:
             newly_calibrated_models:
                 See attributes of :class:`Problem`.
         """
         self.newly_calibrated_models = newly_calibrated_models
         self.calibrated_models.update(self.newly_calibrated_models)
 
     def handle_select_kwargs(
         self,
-        kwargs: Dict[str, Any],
+        kwargs: dict[str, Any],
     ):
         """Check keyword arguments to select calls."""
         if "newly_calibrated_models" in kwargs:
             raise ValueError(
                 'Please supply `newly_calibrated_models` via '
                 '`pypesto.select.Problem.set_state`.'
             )
@@ -107,32 +125,31 @@
                 'Please supply `calibrated_models` via '
                 '`pypesto.select.Problem.set_state`.'
             )
 
     def select(
         self,
         **kwargs,
-    ) -> Tuple[Model, Dict[str, Model], Dict[str, Model]]:
+    ) -> tuple[Model, dict[str, Model], dict[str, Model]]:
         """Run a single iteration of a model selection algorithm.
 
         The result is the selected model for the current run, independent of
         previous selected models.
 
         ``kwargs`` are passed to the :class:`MethodCaller` constructor.
 
         Returns
         -------
-        tuple
-            A 3-tuple, with the following values:
+        A 3-tuple, with the following values:
 
-               1. the best model;
-               2. all candidate models in this iteration, as a `dict` with
-                  model hashes as keys and models as values; and
-               3. all candidate models from all iterations, as a `dict` with
-                  model hashes as keys and models as values.
+           1. the best model;
+           2. all candidate models in this iteration, as a `dict` with
+              model hashes as keys and models as values; and
+           3. all candidate models from all iterations, as a `dict` with
+              model hashes as keys and models as values.
         """
         # TODO move some options to PEtab Select? e.g.:
         # - startpoint_latest_mle
         # - select_first_improvement
         self.handle_select_kwargs(kwargs)
         # TODO handle bidirectional
         method_caller = self.create_method_caller(**kwargs)
@@ -155,42 +172,34 @@
         # then no values need to be returned, and users can request values
         # manually.
         return best_model, newly_calibrated_models
 
     def select_to_completion(
         self,
         **kwargs,
-    ) -> List[Model]:
+    ) -> list[Model]:
         """Run an algorithm until an exception `StopIteration` is raised.
 
         ``kwargs`` are passed to the :class:`MethodCaller` constructor.
 
         An exception ``StopIteration`` is raised by
         :meth:`pypesto.select.method.MethodCaller.__call__` when no candidate models
         are found.
 
         Returns
         -------
-        list
-            The best models (the best model at each iteration).
+        The best models (the best model at each iteration).
         """
         best_models = []
         self.handle_select_kwargs(kwargs)
         method_caller = self.create_method_caller(**kwargs)
 
-        intermediate_kwargs = {}
         while True:
-            # TODO currently uses the best model so far, not the best model
-            #      from the previous iteration. Make this a possibility?
-            # TODO string literals
-            if best_models:
-                intermediate_kwargs["predecessor_model"] = best_models[-1]
             try:
                 previous_best_model, newly_calibrated_models = method_caller(
-                    **intermediate_kwargs,
                     newly_calibrated_models=self.newly_calibrated_models,
                 )
                 self.update_with_newly_calibrated_models(
                     newly_calibrated_models=newly_calibrated_models,
                 )
                 best_models.append(previous_best_model)
             except StopIteration:
@@ -204,15 +213,15 @@
 
     # TODO method that automatically generates initial models, for a specific
     # number of starts. TODO parallelise?
     def multistart_select(
         self,
         predecessor_models: Iterable[Model] = None,
         **kwargs,
-    ) -> Tuple[Model, List[Model]]:
+    ) -> tuple[Model, list[Model]]:
         """Run an algorithm multiple times, with different predecessor models.
 
         Note that the same method caller is currently shared between all calls.
         This may change when parallelization is implemented, but for now
         ensures that the same model isn't calibrated twice.
         Could also be managed by sharing the same "calibrated_models" object
         (but then the same model could be repeatedly calibrated, if the
@@ -224,19 +233,18 @@
         ----------
         predecessor_models:
             The models that will be used as initial models. One "model
             selection iteration" will be run for each predecessor model.
 
         Returns
         -------
-        tuple
-            A 2-tuple, with the following values:
+        A 2-tuple, with the following values:
 
-               1. the best model; and
-               2. the best models (the best model at each iteration).
+           1. the best model; and
+           2. the best models (the best model at each iteration).
         """
         self.handle_select_kwargs(kwargs)
         model_lists = []
         newly_calibrated_models_list = [
             self.newly_calibrated_models for _ in predecessor_models
         ]
 
@@ -245,15 +253,14 @@
             method_caller.candidate_space.previous_predecessor_model = (
                 predecessor_model
             )
             (
                 best_model,
                 newly_calibrated_models_list[start_index],
             ) = method_caller(
-                predecessor_model=predecessor_model,
                 newly_calibrated_models=newly_calibrated_models_list[
                     start_index
                 ],
             )
             self.calibrated_models.update(
                 newly_calibrated_models_list[start_index]
             )
```

### Comparing `pypesto-0.4.1/pypesto/startpoint/base.py` & `pypesto-0.4.2/pypesto/startpoint/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Startpoint base classes."""
+
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Callable, Union
 
 import numpy as np
```

### Comparing `pypesto-0.4.1/pypesto/startpoint/latin_hypercube.py` & `pypesto-0.4.2/pypesto/startpoint/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/startpoint/uniform.py` & `pypesto-0.4.2/pypesto/startpoint/uniform.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/store/auto.py` & `pypesto-0.4.2/pypesto/store/auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Auto-saving."""
 
 import binascii
 import datetime
 import logging
 import os
+from pathlib import Path
 from typing import Callable, Union
 
 import h5py
 
 from ..result import Result
 from .save_to_hdf5 import write_result
 
 logger = logging.getLogger(__name__)
 
 
 def autosave(
-    filename: Union[str, Callable, None],
+    filename: Union[Path, str, Callable, None],
     result: Result,
     store_type: str,
     overwrite: bool = False,
 ):
     """
     Save the result of optimization, profiling or sampling automatically.
 
@@ -39,14 +40,17 @@
         method the function is called in.
     overwrite:
         Whether to overwrite the currently existing results.
     """
     if filename is None:
         return
 
+    if isinstance(filename, Path):
+        filename = str(filename)
+
     if filename == "Auto":
         filename = default_filename
     elif isinstance(filename, str):
         if os.path.exists(filename) and not overwrite:
             with h5py.File(filename, 'r') as f:
                 storage_used = store_type in f.keys()
             if storage_used:
```

### Comparing `pypesto-0.4.1/pypesto/store/hdf5.py` & `pypesto-0.4.2/pypesto/store/hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/store/read_from_hdf5.py` & `pypesto-0.4.2/pypesto/store/read_from_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Include various function to read results from hdf5 Files."""
 
 import ast
 import logging
+import warnings
+from pathlib import Path
+from typing import Union
 
 import h5py
 import numpy as np
 
 from ..history import Hdf5History
 from ..objective import Objective, ObjectiveBase
 from ..problem import Problem
@@ -44,15 +47,15 @@
                 f'/profiling/{profile_id}/{parameter_id}'
             ].attrs[profile_key]
     return result
 
 
 def read_hdf5_optimization(
     f: h5py.File,
-    file_name: str,
+    file_name: Union[Path, str],
     opt_id: str,
 ) -> 'OptimizerResult':
     """Read HDF5 results per start.
 
     Parameters
     ----------
     f:
@@ -87,20 +90,20 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 problem file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """Initialize reader.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 problem file name
         """
         self.storage_filename = storage_filename
 
     def read(self, objective: ObjectiveBase = None) -> Problem:
         """Read HDF5 problem file and return pyPESTO problem object.
 
@@ -114,18 +117,17 @@
         problem:
             A problem instance with all attributes read in.
         """
         # create empty problem
         if objective is None:
             objective = Objective()
             # raise warning that objective is not loaded.
-            logger.info(
-                'WARNING: You are loading a problem.\nThis problem'
-                ' is not to be used without a separately created'
-                ' objective.'
+            warnings.warn(
+                'You are loading a problem. This problem is not to be used '
+                'without a separately created objective.'
             )
         problem = Problem(objective, [], [])
 
         with h5py.File(self.storage_filename, 'r') as f:
             for problem_key in f['/problem']:
                 if problem_key == 'config':
                     continue
@@ -149,21 +151,21 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """
         Initialize reader.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 result file name
         """
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
         """Read HDF5 result file and return pyPESTO result object."""
@@ -183,20 +185,20 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """Initialize reader.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 result file name
         """
         self.storage_filename = storage_filename
         self.results = Result()
 
     def read(self) -> Result:
         """Read HDF5 result file and return pyPESTO result object."""
@@ -222,15 +224,15 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """
         Initialize reader.
 
         Parameters
         ----------
         storage_filename:
             HDF5 result file name
@@ -257,15 +259,15 @@
                         f, profile_id=profile_id, parameter_id=parameter_id
                     )
             self.results.profile_result.list = profiling_list
         return self.results
 
 
 def read_result(
-    filename: str,
+    filename: Union[Path, str],
     problem: bool = True,
     optimize: bool = False,
     profile: bool = False,
     sample: bool = False,
 ) -> Result:
     """Save the whole pypesto.Result object in an HDF5 file.
 
@@ -335,15 +337,15 @@
                 'highly likely that no sampling result exists '
                 f'within {filename}.'
             )
 
     return result
 
 
-def load_objective_config(filename: str):
+def load_objective_config(filename: Union[str, Path]):
     """Load the objective information stored in f.
 
     Parameters
     ----------
     filename:
         The name of the file in which the information are stored.
```

### Comparing `pypesto-0.4.1/pypesto/store/save_to_hdf5.py` & `pypesto-0.4.2/pypesto/store/save_to_hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Include functions for saving various results to hdf5."""
 
 import logging
 import os
 from numbers import Integral
+from pathlib import Path
 from typing import Union
 
 import h5py
 import numpy as np
 
 from ..result import ProfilerResult, Result, SampleResult
 from .hdf5 import write_array, write_float_array
@@ -48,24 +49,24 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """
         Initialize writer.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 problem file name
         """
-        self.storage_filename = storage_filename
+        self.storage_filename = str(storage_filename)
 
     def write(self, problem, overwrite: bool = False):
         """Write HDF5 problem file from pyPESTO problem object."""
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
@@ -101,24 +102,24 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """
         Initialize Writer.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 result file name
         """
-        self.storage_filename = storage_filename
+        self.storage_filename = str(storage_filename)
 
     def write(self, result: Result, overwrite=False):
         """Write HDF5 result file from pyPESTO result object."""
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
@@ -150,24 +151,24 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """
         Initialize Writer.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 result file name
         """
-        self.storage_filename = storage_filename
+        self.storage_filename = str(storage_filename)
 
     def write(self, result: Result, overwrite: bool = False):
         """Write HDF5 sampling file from pyPESTO result object."""
         # if there is no sample available, log a warning and return
         # SampleResult is only a dummy class created by the Result class
         # and always indicates the lack of a sampling result.
         if isinstance(result.sample_result, SampleResult):
@@ -203,24 +204,24 @@
 
     Attributes
     ----------
     storage_filename:
         HDF5 result file name
     """
 
-    def __init__(self, storage_filename: str):
+    def __init__(self, storage_filename: Union[str, Path]):
         """
         Initialize Writer.
 
         Parameters
         ----------
-        storage_filename: str
+        storage_filename:
             HDF5 result file name
         """
-        self.storage_filename = storage_filename
+        self.storage_filename = str(storage_filename)
 
     def write(self, result: Result, overwrite: bool = False):
         """Write HDF5 result file from pyPESTO result object."""
         # Create destination directory
         if isinstance(self.storage_filename, str):
             basedir = os.path.dirname(self.storage_filename)
             if basedir:
@@ -262,15 +263,15 @@
                 raise ValueError(
                     f"Error writing {key} ({value}) to {result_grp}."
                 ) from e
 
 
 def write_result(
     result: Result,
-    filename: str,
+    filename: Union[str, Path],
     overwrite: bool = False,
     problem: bool = True,
     optimize: bool = False,
     profile: bool = False,
     sample: bool = False,
 ):
     """
```

### Comparing `pypesto-0.4.1/pypesto/testing/examples.py` & `pypesto-0.4.2/pypesto/testing/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Creates a modified version of the Boehm_JProteomeRes2014 benchmark problem,
     suitable for hierarchical optimization.
     """
     import petab
     from benchmark_models_petab import get_problem
 
-    from pypesto.hierarchical.problem import PARAMETER_TYPE
+    from pypesto.C import PARAMETER_TYPE
 
     petab_problem = get_problem("Boehm_JProteomeRes2014")
     # Add scaling and offset parameters
     petab_problem.observable_df[petab.OBSERVABLE_FORMULA] = [
         f"observableParameter2_{obs_id} + observableParameter1_{obs_id} "
         f"* {obs_formula}"
         for obs_id, obs_formula in zip(
```

### Comparing `pypesto-0.4.1/pypesto/util.py` & `pypesto-0.4.2/pypesto/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Utilities
 =========
 
 Package-wide utilities.
 
 """
+
 from numbers import Number
-from typing import Any, Callable, Optional, Tuple, Union
+from operator import itemgetter
+from typing import Any, Callable, Optional, Sequence, Tuple, Union
 
 import numpy as np
 from scipy import cluster
+from tqdm import tqdm as _tqdm
 
 
 def _check_none(fun: Callable[..., Any]) -> Callable[..., Union[Any, None]]:
     """Return None if any input argument is None; Wrapper function."""
 
     def checked_fun(*args, **kwargs):
         if any(x is None for x in [*args, *(kwargs.values())]):
@@ -237,15 +240,15 @@
         cluster_size[index] = sum(clust == i_clust)
 
     return cluster_indices, cluster_size
 
 
 def delete_nan_inf(
     fvals: np.ndarray,
-    x: Optional[np.ndarray] = None,
+    x: Optional[Sequence[Union[np.ndarray, list[float]]]] = None,
     xdim: Optional[int] = 1,
     magnitude_bound: Optional[float] = np.inf,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Delete nan and inf values in fvals.
 
     If parameters 'x' are passed, also the corresponding entries are deleted.
@@ -268,28 +271,68 @@
         array of parameters without nan or inf
     fvals:
         array of fval without nan or inf
     """
     fvals = np.asarray(fvals)
     finite_fvals = np.isfinite(fvals) & (np.absolute(fvals) < magnitude_bound)
     if x is not None:
-        # if we start out with a list of x, the x corresponding
-        # to finite fvals may be None, so we cannot stack the x before taking
-        # subindexing
-        # If none of the fvals are finite, np.vstack will fail and np.take
-        # will not yield the correct dimension, so we try to construct an
-        # empty np.ndarray with the correct dimension (other functions rely
-        # on x.shape[1] to be of correct dimension)
         if np.isfinite(fvals).any():
-            x = np.vstack(np.take(x, np.where(finite_fvals)[0], axis=0))
+            finite_indices = np.where(finite_fvals)[0]
+            x = np.array(itemgetter(*finite_indices)(x))
+            # itemgetter does not return list for single element
+            if len(x.shape) == 1:
+                x = x.reshape((1, x.shape[0]))
         else:
+            # If none of the fvals are finite we try to construct an
+            # empty np.ndarray with the correct dimension (other functions rely
+            # on x.shape[1] to be of correct dimension)
+            x = np.array(x)
             x = np.empty(
                 (
                     0,
-                    x.shape[1]
-                    if x.ndim == 2
-                    else x[0].shape[0]
-                    if x[0] is not None
-                    else xdim,
+                    (
+                        x.shape[1]
+                        if x.ndim == 2
+                        else x[0].shape[0]
+                        if x[0] is not None
+                        else xdim
+                    ),
                 )
             )
     return x, fvals[finite_fvals]
+
+
+def tqdm(*args, enable: bool = None, **kwargs):
+    """
+    Create a progress bar using tqdm.
+
+    Parameters
+    ----------
+    args:
+        Arguments passed to tqdm.
+    enable:
+        Whether to enable the progress bar.
+        If None, use tqdm defaults.
+        Mutually exclusive with `disable`.
+    kwargs:
+        Keyword arguments passed to tqdm.
+
+    Returns
+    -------
+    progress_bar:
+        A progress bar.
+    """
+    # Drop the `disable` argument unless it is not-None.
+    # This way, we don't interfere with TQDM_DISABLE or other global
+    # tqdm settings.
+    disable = kwargs.pop("disable", None)
+
+    if enable is not None:
+        if disable is not None and enable != disable:
+            raise ValueError(
+                "Contradicting values for `enable` and `disable` passed."
+            )
+        disable = not enable
+
+    if disable is not None:
+        kwargs["disable"] = disable
+    return _tqdm(*args, **kwargs)
```

### Comparing `pypesto-0.4.1/pypesto/visualize/__init__.py` & `pypesto-0.4.2/pypesto/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/clust_color.py` & `pypesto-0.4.2/pypesto/visualize/clust_color.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/dimension_reduction.py` & `pypesto-0.4.2/pypesto/visualize/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/ensemble.py` & `pypesto-0.4.2/pypesto/visualize/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     ax: Optional[plt.Axes] = None,
     size: Optional[Tuple[float]] = (12, 6),
 ):
     """
     Visualize identifiablity of parameter ensemble.
 
     Plot an overview about how many parameters hit the parameter bounds based
-    on a ensemble of parameters. confidence intervals/credible ranges are
+    on an ensemble of parameters. confidence intervals/credible ranges are
     computed via the ensemble mean plus/minus 1 standard deviation.
-    This highlevel routine expects a ensemble object as input.
+    This highlevel routine expects an ensemble object as input.
 
     Parameters
     ----------
     ensemble:
         ensemble of parameter vectors (from pypesto.ensemble)
     ax:
         Axes object to use.
@@ -40,15 +40,15 @@
     """
     # first get the data to check identifiability
     id_df = ensemble.check_identifiability()
 
     # check how many bounds are actually hit and which ones
     none_hit, lb_hit, ub_hit, both_hit = _prepare_identifiability_plot(id_df)
 
-    # call lowlevel routine whick works with np arrays only
+    # call lowlevel routine which works with np arrays only
     ax = ensemble_identifiability_lowlevel(
         none_hit, lb_hit, ub_hit, both_hit, ax, size
     )
 
     return ax
```

### Comparing `pypesto-0.4.1/pypesto/visualize/misc.py` & `pypesto-0.4.2/pypesto/visualize/misc.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/model_fit.py` & `pypesto-0.4.2/pypesto/visualize/model_fit.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Visualization of the model fit after optimization.
 
 Currently only for PEtab problems.
 """
+
+import copy
 from typing import Sequence, Union
 
 import amici
 import amici.plotting
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 import petab
 from amici.petab_objective import rdatas_to_simulation_df
 from petab.visualize import plot_problem
 
-from ..C import CENSORED, NONLINEAR_MONOTONE, ORDINAL, RDATAS
+from ..C import CENSORED, ORDINAL, RDATAS, SEMIQUANTITATIVE
+from ..hierarchical.relative.calculator import RelativeAmiciCalculator
 from ..petab.importer import get_petab_non_quantitative_data_types
 from ..problem import Problem
 from ..result import Result
 from .ordinal_categories import plot_categories_from_pypesto_result
 from .spline_approximation import _add_spline_mapped_simulations_to_model_fit
 
 AmiciModel = Union['amici.Model', 'amici.ModelPtr']
@@ -95,25 +98,25 @@
         **kwargs,
     )
 
     non_quantitative_data_types = get_petab_non_quantitative_data_types(
         petab_problem
     )
 
-    if non_quantitative_data_types:
+    if non_quantitative_data_types is not None:
         if (
             ORDINAL in non_quantitative_data_types
             or CENSORED in non_quantitative_data_types
         ):
             axes = plot_categories_from_pypesto_result(
                 result,
                 start_index=start_index,
                 axes=axes,
             )
-        if NONLINEAR_MONOTONE in non_quantitative_data_types:
+        if SEMIQUANTITATIVE in non_quantitative_data_types:
             axes = _add_spline_mapped_simulations_to_model_fit(
                 result=result,
                 pypesto_problem=pypesto_problem,
                 start_index=start_index,
                 axes=axes,
             )
 
@@ -170,40 +173,132 @@
     """
     if problem is None:
         problem = result.problem
     # add timepoints as needed
     if timepoints is None:
         end_time = max(problem.objective.edatas[0].getTimepoints())
         timepoints = np.linspace(start=0, stop=end_time, num=n_timepoints)
-    obj = problem.objective.set_custom_timepoints(timepoints_global=timepoints)
 
-    # evaluate objective with return dic = True to get data
-    parameters = result.optimize_result.list[start_index]['x']
-    # reduce vector to only include free indices. Needed downstream.
-    parameters = problem.get_reduced_vector(parameters)
-    ret = obj(parameters, mode='mode_fun', sensi_orders=(0,), return_dict=True)
+    # get rdatas
+    rdatas = _get_simulation_rdatas(
+        result=result,
+        problem=problem,
+        start_index=start_index,
+        simulation_timepoints=timepoints,
+    )
 
     if state_ids == [] and state_names == []:
         axes = _time_trajectory_model_without_states(
             model=problem.objective.amici_model,
-            rdatas=ret['rdatas'],
+            rdatas=rdatas,
             observable_ids=observable_ids,
         )
     else:
         axes = _time_trajectory_model_with_states(
             model=problem.objective.amici_model,
-            rdatas=ret['rdatas'],
+            rdatas=rdatas,
             state_ids=state_ids,
             state_names=state_names,
             observable_ids=observable_ids,
         )
 
     return axes
 
 
+def _get_simulation_rdatas(
+    result: Union[Result, Sequence[Result]],
+    problem: Problem,
+    start_index: int = 0,
+    simulation_timepoints: np.ndarray = None,
+) -> list[amici.ReturnData]:
+    """
+    Get simulation results for a given optimization result and timepoints.
+
+    Parameters
+    ----------
+    result:
+        The result object from optimization.
+    problem:
+        A pypesto problem.
+    timepoints:
+        Array of timepoints, at which the trajectory will be stored..
+
+    start_index:
+        Index of Optimization run to be plotted. Default is best start.
+    Returns
+    -------
+    rdatas:
+        List of amici.ReturnData objects containing the simulation results.
+    """
+    # add timepoints as needed
+    if simulation_timepoints is None:
+        end_time = max(problem.objective.edatas[0].getTimepoints())
+        simulation_timepoints = np.linspace(start=0, stop=end_time, num=1000)
+
+    # get optimization result
+    parameters = result.optimize_result.list[start_index]['x']
+
+    # reduce vector to only include free indices. Needed downstream.
+    parameters = problem.get_reduced_vector(parameters)
+
+    # simulate with custom timepoints for hierarchical model
+    if isinstance(problem.objective.calculator, RelativeAmiciCalculator):
+        # get parameter dictionary
+        x_dct = dict(
+            zip(problem.x_names, result.optimize_result.list[start_index].x)
+        )
+
+        # evaluate objective with return dict = True to get inner parameters
+        ret = problem.objective(
+            parameters, mode='mode_fun', sensi_orders=(0,), return_dict=True
+        )
+
+        # update parameter dictionary with inner parameters
+        inner_parameters = ret['inner_parameters']
+        x_dct.update(inner_parameters)
+
+        parameter_mapping = problem.objective.parameter_mapping
+        edatas = copy.deepcopy(problem.objective.edatas)
+        amici_model = problem.objective.amici_model
+
+        # disable sensitivities to improve computation time
+        amici_solver = copy.deepcopy(problem.objective.amici_solver)
+        amici_solver.setSensitivityOrder(amici.SensitivityOrder.none)
+
+        for j in range(len(edatas)):
+            edatas[j].setTimepoints(simulation_timepoints)
+
+        amici.parameter_mapping.fill_in_parameters(
+            edatas=edatas,
+            problem_parameters=x_dct,
+            scaled_parameters=True,
+            parameter_mapping=parameter_mapping,
+            amici_model=amici_model,
+        )
+
+        rdatas = amici.runAmiciSimulations(
+            amici_model,
+            amici_solver,
+            edatas,
+        )
+    else:
+        # set custom timepoints
+        obj = problem.objective.set_custom_timepoints(
+            timepoints_global=simulation_timepoints
+        )
+
+        # evaluate objective with return dict = True to get data
+        ret = obj(
+            parameters, mode='mode_fun', sensi_orders=(0,), return_dict=True
+        )
+        rdatas = ret['rdatas']
+
+    return rdatas
+
+
 def _time_trajectory_model_with_states(
     model: AmiciModel,
     rdatas: Union['amici.ReturnData', Sequence['amici.ReturnData']],
     state_ids: Sequence[str],
     state_names: Sequence[str],
     observable_ids: Union[str, Sequence[str]],
 ):
```

### Comparing `pypesto-0.4.1/pypesto/visualize/optimization_stats.py` & `pypesto-0.4.2/pypesto/visualize/optimization_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 
     Returns
     -------
     ax:
         The plot axes.
     """
     fvals = result.optimize_result.fval
-    values = [res[property_name] for res in result.optimize_result.list]
+    values = [[res[property_name]] for res in result.optimize_result.list]
     values, fvals = delete_nan_inf(fvals, values)
 
     if start_indices is not None:
         start_indices = process_start_indices(result, start_indices)
         values = values[start_indices]
         fvals = fvals[start_indices]
```

### Comparing `pypesto-0.4.1/pypesto/visualize/optimizer_convergence.py` & `pypesto-0.4.2/pypesto/visualize/optimizer_convergence.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,22 +48,24 @@
     import seaborn as sns
 
     if ax is None:
         ax = plt.subplots(figsize=size)[1]
 
     fvals = result.optimize_result.fval
     grad_norms = [
-        np.linalg.norm(
-            result.problem.get_reduced_vector(
-                grad, result.problem.x_free_indices
-            ),
-            2,
+        (
+            np.linalg.norm(
+                result.problem.get_reduced_vector(
+                    grad, result.problem.x_free_indices
+                ),
+                2,
+            )
+            if grad is not None
+            else np.NaN
         )
-        if grad is not None
-        else np.NaN
         for grad in result.optimize_result.grad
     ]
     msgs = result.optimize_result.message
     conv_data = pd.DataFrame(
         {'fval': fvals, 'gradient norm': grad_norms, 'exit message': msgs}
     )
     sns.scatterplot(
```

### Comparing `pypesto-0.4.1/pypesto/visualize/optimizer_history.py` & `pypesto-0.4.2/pypesto/visualize/optimizer_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -472,7 +472,78 @@
     else:
         logger.warning(
             f'Reference point is currently only implemented for trace_y == '
             f'{TRACE_Y_FVAL} and will not be plotted for trace_y == {trace_y}.'
         )
 
     return ax
+
+
+def sacess_history(
+    histories: list[HistoryBase],
+    ax: Optional[plt.Axes] = None,
+) -> plt.Axes:
+    """Plot `SacessOptimizer` history.
+
+    Plot the history of the best objective values for each
+    :class:`pypesto.optimize.ess.sacess.SacessOptimizer`
+    worker over computation time as step splot.
+
+    Parameters
+    ----------
+    histories:
+        List of histories from different workers as obtained from
+        :attr:`pypesto.optimize.ess.sacess.SacessOptimizer.histories`.
+    ax:
+        Axes object to use.
+
+    Returns
+    -------
+    The plot axes. `ax` or a new axes if `ax` was `None`.
+    """
+    ax = ax or plt.subplot()
+
+    # plot overall minimum
+    # merge results
+    t = np.hstack([history.get_time_trace() for history in histories])
+    fx = np.hstack([history.get_fval_trace() for history in histories])
+    time_order = np.argsort(t)
+    t = t[time_order]
+    fx = fx[time_order]
+
+    # get the monotonously decreasing sequence
+    monotone = np.where(fx <= np.fmin.accumulate(fx))[0]
+    x, y = t[monotone], fx[monotone]
+
+    # extend from last decrease to last timepoint
+    x = np.append(x, [t.max()])
+    y = np.append(y, [y.min()])
+    ax.step(
+        x,
+        y,
+        linestyle="dotted",
+        color="grey",
+        where="post",
+        label="overall",
+        alpha=0.8,
+    )
+
+    # plot steps of individual workers
+    for worker_idx, history in enumerate(histories):
+        x, y = history.get_time_trace(), history.get_fval_trace()
+        # extend from last decrease to last timepoint
+        x = np.append(x, [np.max(t)])
+        y = np.append(y, [np.min(y)])
+        lines = ax.step(
+            x, y, ".-", where="post", label=f"worker {worker_idx}", alpha=0.8
+        )
+        # Plot last point without marker, unless we actually had an improvement there.
+        # The time point of the overall last improvement is appended to all histories,
+        # even if redundant, so we can just skip the marker for the last point.
+        for line in lines:
+            line.set_markevery([True] * (len(x) - 1) + [False])
+
+    ax.legend()
+    ax.set_xlabel("time (s)")
+    ax.set_ylabel("fval")
+    ax.set_title("SacessOptimizer convergence")
+    return ax
```

### Comparing `pypesto-0.4.1/pypesto/visualize/ordinal_categories.py` & `pypesto-0.4.2/pypesto/visualize/ordinal_categories.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 import warnings
-from typing import TYPE_CHECKING, Dict, List, Optional
+from typing import TYPE_CHECKING, Optional
 
 if TYPE_CHECKING:
     import pypesto
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 try:
     import amici
     from petab.C import OBSERVABLE_ID
 
-    from ..hierarchical.optimal_scaling.calculator import (
-        OptimalScalingAmiciCalculator,
-    )
-    from ..hierarchical.optimal_scaling.parameter import (
-        OptimalScalingParameter,
-    )
-    from ..hierarchical.optimal_scaling.solver import (
+    from ..hierarchical.ordinal.calculator import OrdinalCalculator
+    from ..hierarchical.ordinal.parameter import OrdinalParameter
+    from ..hierarchical.ordinal.solver import (
         compute_interval_constraints,
         get_bounds_for_category,
         undo_inner_parameter_reparameterization,
     )
 except ImportError:
     pass
 
@@ -72,15 +68,15 @@
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
             pypesto_result.optimize_result.list[start_index]['x'],
         )
     )
     x_dct.update(
-        pypesto_result.problem.objective.calculator.noise_dummy_values
+        pypesto_result.problem.objective.calculator.necessary_par_dummy_values
     )
 
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_result.problem.objective.edatas
     parameter_mapping = pypesto_result.problem.objective.parameter_mapping
     amici_model = pypesto_result.problem.objective.amici_model
     amici_solver = pypesto_result.problem.objective.amici_solver
@@ -126,15 +122,15 @@
         petab_problem.measurement_df[OBSERVABLE_ID].unique()
     )
 
     optimal_scaling_calculator = None
     for (
         calculator
     ) in pypesto_result.problem.objective.calculator.inner_calculators:
-        if isinstance(calculator, OptimalScalingAmiciCalculator):
+        if isinstance(calculator, OrdinalCalculator):
             optimal_scaling_calculator = calculator
             break
 
     # Get the inner solver and problem.
     inner_solver = optimal_scaling_calculator.inner_solver
     inner_problem = optimal_scaling_calculator.inner_problem
 
@@ -152,23 +148,23 @@
         measurement_df_observable_ordering,
         axes,
         **kwargs,
     )
 
 
 def plot_categories_from_inner_result(
-    inner_problem: 'pypesto.hierarchical.optimal_scaling.problem.OptimalScalingProblem',
-    inner_solver: 'pypesto.hierarchical.optimal_scaling.solver.OptimalScalingInnerSolver',
-    results: List[Dict],
-    simulation: List[np.ndarray],
-    timepoints: List[np.ndarray],
-    observable_ids: List[str] = None,
-    condition_ids: List[str] = None,
-    petab_condition_ordering: List[str] = None,
-    measurement_df_observable_ordering: List[str] = None,
+    inner_problem: 'pypesto.hierarchical.ordinal.problem.OrdinalProblem',
+    inner_solver: 'pypesto.hierarchical.ordinal.solver.OrdinalInnerSolver',
+    results: list[dict],
+    simulation: list[np.ndarray],
+    timepoints: list[np.ndarray],
+    observable_ids: list[str] = None,
+    condition_ids: list[str] = None,
+    petab_condition_ordering: list[str] = None,
+    measurement_df_observable_ordering: list[str] = None,
     axes: Optional[plt.Axes] = None,
     **kwargs,
 ):
     """Plot the inner solutions.
 
     Parameters
     ----------
@@ -498,21 +494,21 @@
             color='gray',
             alpha=0.5,
             label='Censoring areas',
         )
 
 
 def _get_data_for_plotting(
-    inner_parameters: List['OptimalScalingParameter'],
-    optimal_scaling_bounds: List,
-    sim: List[np.ndarray],
-    timepoints: List[np.ndarray],
+    inner_parameters: list['OrdinalParameter'],
+    optimal_scaling_bounds: list,
+    sim: list[np.ndarray],
+    timepoints: list[np.ndarray],
     interval_range: float,
     interval_gap: float,
-    options: Dict,
+    options: dict,
     measurement_type: str,
 ):
     """Return data in the form suited for plotting."""
     if options[REPARAMETERIZED] and measurement_type == ORDINAL:
         optimal_scaling_bounds = undo_inner_parameter_reparameterization(
             optimal_scaling_bounds,
             inner_parameters,
```

### Comparing `pypesto-0.4.1/pypesto/visualize/parameters.py` & `pypesto-0.4.2/pypesto/visualize/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,25 @@
             result=result,
             lb=lb,
             ub=ub,
             parameter_indices=parameter_indices,
             start_indices=start_indices,
             plot_inner_parameters=plot_inner_parameters,
         )
+
+        # parse fvals and parameters
+        fvals = np.array(fvals)
+        # remove nan or inf values
+        xs, fvals = delete_nan_inf(
+            fvals=fvals,
+            x=xs,
+            xdim=len(ub) if ub is not None else 1,
+            magnitude_bound=WATERFALL_MAX_VALUE,
+        )
+
         lb, ub, xs = map(scale_parameters, (lb, ub, xs))
 
         # call lowlevel routine
         ax = parameters_lowlevel(
             xs=xs,
             fvals=fvals,
             lb=lb,
@@ -219,16 +230,16 @@
     ax.set_ylabel("counts")
     ax.set_title(f"{parameter_name}")
 
     return ax
 
 
 def parameters_lowlevel(
-    xs: Sequence[Union[np.ndarray, List[float]]],
-    fvals: Union[np.ndarray, List[float]],
+    xs: np.ndarray,
+    fvals: np.ndarray,
     lb: Optional[Union[np.ndarray, List[float]]] = None,
     ub: Optional[Union[np.ndarray, List[float]]] = None,
     x_labels: Optional[Iterable[str]] = None,
     ax: Optional[matplotlib.axes.Axes] = None,
     size: Optional[Tuple[float, float]] = None,
     colors: Optional[Sequence[Union[np.ndarray, List[float]]]] = None,
     linestyle: str = '-',
@@ -237,16 +248,16 @@
 ) -> matplotlib.axes.Axes:
     """
     Plot parameters plot using list of parameters.
 
     Parameters
     ----------
     xs:
-        Including optimized parameters for each startpoint.
-        Shape: (n_starts, dim).
+        Including optimized parameters for each start that did not result in an infinite fval.
+        Shape: (n_starts_successful, dim).
     fvals:
         Function values. Needed to assign cluster colors.
     lb, ub:
         The lower and upper bounds.
     x_labels:
         Labels to be used for the parameters.
     ax:
@@ -264,24 +275,14 @@
         avoid overplotting (default: True)
 
     Returns
     -------
     ax:
         The plot axes.
     """
-    # parse input
-    xs = np.array(xs)
-    fvals = np.array(fvals)
-    # remove nan or inf values in fvals and xs
-    xs, fvals = delete_nan_inf(
-        fvals=fvals,
-        x=xs,
-        xdim=len(ub) if ub is not None else 1,
-        magnitude_bound=WATERFALL_MAX_VALUE,
-    )
 
     if size is None:
         # 0.5 inch height per parameter
         size = (18.5, max(xs.shape[1], 1) / 2)
 
     if ax is None:
         ax = plt.subplots()[1]
@@ -372,36 +373,18 @@
         objective function values which are needed for plotting later
     xs:
         parameter values which will be plotted later
     """
     # retrieve results
     fvals = result.optimize_result.fval
     xs = result.optimize_result.x
-    # retrieve inner parameters if available
-    inner_xs = [
-        res.get(INNER_PARAMETERS, None) for res in result.optimize_result.list
-    ]
-    if any(inner_xs):
-        # search for first non-empty inner_xs to obtain inner_xs_names
-        for inner_xs_idx in inner_xs:
-            if inner_xs_idx is not None:
-                inner_xs_names = list(inner_xs_idx.keys())
-                break
-        # fill inner_xs with nan if no inner_xs are available
-        inner_xs = [
-            np.full(len(inner_xs_names), np.nan)
-            if inner_xs_idx is None
-            else list(inner_xs_idx.values())
-            for inner_xs_idx in inner_xs
-        ]
-        # set bounds for inner parameters
-        inner_lb = np.full(len(inner_xs_names), -np.inf)
-        inner_ub = np.full(len(inner_xs_names), np.inf)
-    else:
-        inner_xs = None
+
+    # retrieve inner parameters in case of hierarchical optimization
+    inner_xs, inner_xs_names, inner_lb, inner_ub = _handle_inner_inputs(result)
+
     # parse indices which should be plotted
     if start_indices is not None:
         start_indices = process_start_indices(result, start_indices)
 
         # reduce number of displayed results
         xs_out = [xs[ind] for ind in start_indices]
         fvals_out = [fvals[ind] for ind in start_indices]
@@ -444,14 +427,70 @@
             np.concatenate([x, inner_x]) if x is not None else None
             for x, inner_x in zip(xs_out, inner_xs_out)
         ]
 
     return lb, ub, x_labels, fvals_out, xs_out
 
 
+def _handle_inner_inputs(
+    result: Result,
+) -> Union[
+    Tuple[None, None, None, None],
+    Tuple[list[np.ndarray], list[str], np.ndarray, np.ndarray],
+]:
+    """Handle inner parameters from hierarchical optimization, if available.
+
+    Parameters
+    ----------
+    result:
+        Optimization result obtained by 'optimize.py'.
+
+    Returns
+    -------
+    inner_xs:
+        Inner parameter values which will be appended to xs.
+    inner_xs_names:
+        Inner parameter names.
+    inner_lb:
+        Inner parameter lower bounds.
+    inner_ub:
+        Inner parameter upper bounds.
+    """
+    inner_xs = [
+        res.get(INNER_PARAMETERS, None) for res in result.optimize_result.list
+    ]
+    inner_xs_names = None
+    inner_lb = None
+    inner_ub = None
+
+    from ..problem import HierarchicalProblem
+
+    if any(inner_x is not None for inner_x in inner_xs) and isinstance(
+        result.problem, HierarchicalProblem
+    ):
+        inner_xs_names = result.problem.inner_x_names
+        # replace None with a list of nans
+        inner_xs = [
+            (
+                np.full(len(inner_xs_names), np.nan)
+                if inner_xs_idx is None
+                else np.asarray(inner_xs_idx)
+            )
+            for inner_xs_idx in inner_xs
+        ]
+        # set bounds for inner parameters
+        inner_lb = result.problem.inner_lb
+        inner_ub = result.problem.inner_ub
+
+    if inner_xs_names is None:
+        inner_xs = None
+
+    return inner_xs, inner_xs_names, inner_lb, inner_ub
+
+
 def parameters_correlation_matrix(
     result: Result,
     parameter_indices: Union[str, Sequence[int]] = 'free_only',
     start_indices: Optional[Union[int, Iterable[int]]] = None,
     method: Union[str, Callable] = 'pearson',
     cluster: bool = True,
     cmap: Union[Colormap, str] = 'bwr',
```

### Comparing `pypesto-0.4.1/pypesto/visualize/profile_cis.py` & `pypesto-0.4.2/pypesto/visualize/profile_cis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/profiles.py` & `pypesto-0.4.2/pypesto/visualize/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -489,19 +489,19 @@
                 # profile_indices should contain all parameter indices,
                 # for which in at least one of the results a profile exists
                 plottable_indices.update(tmp_indices)
     plottable_indices = sorted(plottable_indices)
 
     # get the profiles, which should be plotted and sanitize, if not plottable
     if profile_indices is None:
-        profile_indices = list(plottable_indices)
+        profile_indices_ret = list(plottable_indices)
     else:
+        profile_indices_ret = list(profile_indices)
         for ind in profile_indices:
             if ind not in plottable_indices:
-                profile_indices = list(profile_indices)
-                profile_indices.remove(ind)
+                profile_indices_ret.remove(ind)
                 warn(
                     'Requested to plot profile for parameter index %i, '
                     'but profile has not been computed.' % ind
                 )
 
-    return profile_indices
+    return profile_indices_ret
```

### Comparing `pypesto-0.4.1/pypesto/visualize/reference_points.py` & `pypesto-0.4.2/pypesto/visualize/reference_points.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/sampling.py` & `pypesto-0.4.2/pypesto/visualize/sampling.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.4.1/pypesto/visualize/select.py` & `pypesto-0.4.2/pypesto/visualize/select.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Visualization routines for model selection with pyPESTO."""
+
 from typing import Dict, List, Tuple
 
 import matplotlib.pyplot as plt
 import networkx as nx
 from petab_select import Model
 from petab_select.constants import VIRTUAL_INITIAL_MODEL, Criterion
```

### Comparing `pypesto-0.4.1/pypesto/visualize/spline_approximation.py` & `pypesto-0.4.2/pypesto/visualize/spline_approximation.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import warnings
-from typing import Dict, List, Optional, Sequence, Union
+from typing import Optional, Sequence, Union
 
 import matplotlib.axes
 import matplotlib.pyplot as plt
 import numpy as np
 
 import pypesto
 
-from ..C import AMICI_SIGMAY, AMICI_Y, CURRENT_SIMULATION, DATAPOINTS, SCIPY_X
+from ..C import (
+    AMICI_SIGMAY,
+    AMICI_Y,
+    CURRENT_SIMULATION,
+    DATAPOINTS,
+    REGULARIZE_SPLINE,
+    SCIPY_X,
+)
 from ..problem import Problem
 from ..result import Result
 
 try:
     import amici
 
-    from ..hierarchical.spline_approximation.calculator import (
-        SplineAmiciCalculator,
-    )
-    from ..hierarchical.spline_approximation.solver import (
-        SplineInnerSolver,
+    from ..hierarchical import InnerCalculatorCollector
+    from ..hierarchical.semiquantitative.calculator import SemiquantCalculator
+    from ..hierarchical.semiquantitative.solver import (
+        SemiquantInnerSolver,
+        _calculate_regularization_for_group,
         get_spline_mapped_simulations,
     )
 except ImportError:
     pass
 
 
 def plot_splines_from_pypesto_result(
@@ -42,25 +49,32 @@
     Returns
     -------
     fig:
         The figure.
     ax:
         The axes.
     """
+    # Check the calculator is the InnerCalculatorCollector.
+    if not isinstance(
+        pypesto_result.problem.objective.calculator, InnerCalculatorCollector
+    ):
+        raise ValueError(
+            'The calculator must be an instance of the InnerCalculatorCollector.'
+        )
 
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
             pypesto_result.optimize_result.list[start_index]['x'],
         )
     )
 
     x_dct.update(
-        pypesto_result.problem.objective.calculator.noise_dummy_values
+        pypesto_result.problem.objective.calculator.necessary_par_dummy_values
     )
 
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_result.problem.objective.edatas
     parameter_mapping = pypesto_result.problem.objective.parameter_mapping
     amici_model = pypesto_result.problem.objective.amici_model
     amici_solver = pypesto_result.problem.objective.amici_solver
@@ -95,41 +109,44 @@
     sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
     sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
 
     spline_calculator = None
     for (
         calculator
     ) in pypesto_result.problem.objective.calculator.inner_calculators:
-        if isinstance(calculator, SplineAmiciCalculator):
+        if isinstance(calculator, SemiquantCalculator):
             spline_calculator = calculator
             break
 
     # Get the inner solver and problem.
     inner_solver = spline_calculator.inner_solver
     inner_problem = spline_calculator.inner_problem
 
     inner_results = inner_solver.solve(inner_problem, sim, sigma)
 
     return plot_splines_from_inner_result(
-        inner_problem, inner_results, observable_ids, **kwargs
+        inner_problem, inner_solver, inner_results, observable_ids, **kwargs
     )
 
 
 def plot_splines_from_inner_result(
     inner_problem: 'pypesto.hierarchical.spline_approximation.problem.SplineInnerProblem',
-    results: List[Dict],
+    inner_solver: 'pypesto.hierarchical.spline_approximation.solver.SplineInnerSolver',
+    results: list[dict],
     observable_ids=None,
     **kwargs,
 ):
     """Plot the inner solutions.
 
     Parameters
     ----------
     inner_problem:
         The inner problem.
+    inner_solver:
+        The inner solver.
     results:
         The results from the inner solver.
     kwargs:
         Additional arguments to pass to the plotting function.
 
     Returns
     -------
@@ -173,15 +190,19 @@
         s = result[SCIPY_X]
 
         inner_parameters = np.array([x.value for x in xs])
         measurements = inner_problem.groups[group][DATAPOINTS]
         simulation = inner_problem.groups[group][CURRENT_SIMULATION]
 
         # For the simulation, get the spline bases
-        delta_c, spline_bases, n = SplineInnerSolver._rescale_spline_bases(
+        (
+            delta_c,
+            spline_bases,
+            n,
+        ) = SemiquantInnerSolver._rescale_spline_bases(
             self=None,
             sim_all=simulation,
             N=len(inner_parameters),
             K=len(simulation),
         )
         mapped_simulations = get_spline_mapped_simulations(
             s, simulation, len(inner_parameters), delta_c, spline_bases, n
@@ -196,14 +217,28 @@
         axs[group_idx].plot(
             spline_bases,
             inner_parameters,
             linestyle='-',
             color='g',
             label='Spline function',
         )
+        if inner_solver.options[REGULARIZE_SPLINE]:
+            alpha_opt, beta_opt = _calculate_optimal_regularization(
+                s=s,
+                N=len(inner_parameters),
+                c=spline_bases,
+            )
+            axs[group_idx].plot(
+                spline_bases,
+                alpha_opt * spline_bases + beta_opt,
+                linestyle='--',
+                color='orange',
+                label='Regularization line',
+            )
+
         axs[group_idx].plot(
             simulation, mapped_simulations, 'r^', label='Mapped simulation'
         )
         axs[group_idx].legend()
         if observable_ids is not None:
             axs[group_idx].set_title(f'{observable_ids[group-1]}')
         else:
@@ -214,14 +249,63 @@
 
     for ax in axs[len(results) :]:
         ax.remove()
 
     return fig, axs
 
 
+def _calculate_optimal_regularization(
+    s: np.ndarray,
+    N: int,
+    c: np.ndarray,
+):
+    """Calculate the optimal linear regularization for the spline approximation.
+
+    Parameters
+    ----------
+    s:
+        The spline parameters.
+    N:
+        The number of inner parameters.
+    c:
+        The spline bases.
+
+    Returns
+    -------
+    alpha_opt:
+        The optimal slope of the linear function.
+    beta_opt:
+        The optimal offset of the linear function.
+    """
+    lower_trian = np.tril(np.ones((N, N)))
+    xi = np.dot(lower_trian, s)
+
+    # Calculate auxiliary values
+    c_sum = np.sum(c)
+    xi_sum = np.sum(xi)
+    c_squares_sum = np.sum(c**2)
+    c_dot_xi = np.dot(c, xi)
+    # Calculate the optimal linear function offset
+    if np.isclose(N * c_squares_sum - c_sum**2, 0):
+        beta_opt = xi_sum / N
+    else:
+        beta_opt = (xi_sum * c_squares_sum - c_dot_xi * c_sum) / (
+            N * c_squares_sum - c_sum**2
+        )
+
+    # If the offset is smaller than 0, we set it to 0
+    if beta_opt < 0:
+        beta_opt = 0
+
+    # Calculate the slope of the optimal linear function
+    alpha_opt = (c_dot_xi - beta_opt * c_sum) / c_squares_sum
+
+    return alpha_opt, beta_opt
+
+
 def _add_spline_mapped_simulations_to_model_fit(
     result: Union[Result, Sequence[Result]],
     pypesto_problem: Problem,
     start_index: int = 0,
     axes: Optional[plt.Axes] = None,
 ) -> Union[matplotlib.axes.Axes, None]:
     """Visualize the spline optimized model fit.
@@ -240,15 +324,17 @@
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_problem.objective.x_ids,
             result.optimize_result.list[start_index]['x'],
         )
     )
-    x_dct.update(pypesto_problem.objective.calculator.noise_dummy_values)
+    x_dct.update(
+        pypesto_problem.objective.calculator.necessary_par_dummy_values
+    )
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_problem.objective.edatas
     parameter_mapping = pypesto_problem.objective.parameter_mapping
     amici_model = pypesto_problem.objective.amici_model
     amici_solver = pypesto_problem.objective.amici_solver
     n_threads = pypesto_problem.objective.n_threads
 
@@ -278,15 +364,15 @@
 
     # Get simulation and sigma.
     sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
     sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
 
     spline_calculator = None
     for calculator in pypesto_problem.objective.calculator.inner_calculators:
-        if isinstance(calculator, SplineAmiciCalculator):
+        if isinstance(calculator, SemiquantCalculator):
             spline_calculator = calculator
             break
 
     # Get the inner solver and problem.
     inner_solver = spline_calculator.inner_solver
     inner_problem = spline_calculator.inner_problem
 
@@ -309,15 +395,19 @@
         xs = inner_problem.get_xs_for_group(group)
         s = inner_result[SCIPY_X]
 
         inner_parameters = np.array([x.value for x in xs])
         simulation = inner_problem.groups[group][CURRENT_SIMULATION]
 
         # For the simulation, get the spline bases
-        delta_c, spline_bases, n = SplineInnerSolver._rescale_spline_bases(
+        (
+            delta_c,
+            spline_bases,
+            n,
+        ) = SemiquantInnerSolver._rescale_spline_bases(
             self=None,
             sim_all=simulation,
             N=len(inner_parameters),
             K=len(simulation),
         )
         # and the spline-mapped simulations.
         mapped_simulations = get_spline_mapped_simulations(
@@ -355,7 +445,125 @@
         )
 
     # Reset the legend.
     for ax in axes.values():
         ax.legend()
 
     return axes
+
+
+def _obtain_regularization_for_start(
+    pypesto_result: Result, start_index=0
+) -> Optional[float]:
+    """Obtain the regularization for the start index.
+
+    Calculates and returns the spline linear regularization
+    term of the objective function for the start index.
+
+    Parameters
+    ----------
+    pypesto_result:
+        The pypesto result.
+    start_index:
+        The start index for which to calculate the regularization.
+
+    Returns
+    -------
+    The regularization term of the objective function for the start index.
+    """
+    # Get the parameters from the pypesto result for the start_index.
+    x_dct = dict(
+        zip(
+            pypesto_result.problem.objective.x_ids,
+            pypesto_result.optimize_result.list[start_index]['x'],
+        )
+    )
+
+    x_dct.update(
+        pypesto_result.problem.objective.calculator.necessary_par_dummy_values
+    )
+
+    # Get the needed objects from the pypesto problem.
+    edatas = pypesto_result.problem.objective.edatas
+    parameter_mapping = pypesto_result.problem.objective.parameter_mapping
+    amici_model = pypesto_result.problem.objective.amici_model
+    amici_solver = pypesto_result.problem.objective.amici_solver
+    n_threads = pypesto_result.problem.objective.n_threads
+
+    # Fill in the parameters.
+    amici.parameter_mapping.fill_in_parameters(
+        edatas=edatas,
+        problem_parameters=x_dct,
+        scaled_parameters=True,
+        parameter_mapping=parameter_mapping,
+        amici_model=amici_model,
+    )
+
+    # Simulate the model with the parameters from the pypesto result.
+    inner_rdatas = amici.runAmiciSimulations(
+        amici_model,
+        amici_solver,
+        edatas,
+        num_threads=min(n_threads, len(edatas)),
+    )
+
+    # If any amici simulation failed, raise warning and return None.
+    if any(rdata.status != amici.AMICI_SUCCESS for rdata in inner_rdatas):
+        warnings.warn(
+            'Warning: Some AMICI simulations failed. Cannot plot inner solutions.'
+        )
+        return None
+
+    # Get simulation and sigma.
+    sim = [rdata[AMICI_Y] for rdata in inner_rdatas]
+    sigma = [rdata[AMICI_SIGMAY] for rdata in inner_rdatas]
+
+    spline_calculator = None
+    for (
+        calculator
+    ) in pypesto_result.problem.objective.calculator.inner_calculators:
+        if isinstance(calculator, SemiquantCalculator):
+            spline_calculator = calculator
+            break
+
+    # Get the inner solver and problem.
+    inner_solver = spline_calculator.inner_solver
+    inner_problem = spline_calculator.inner_problem
+
+    inner_results = inner_solver.solve(inner_problem, sim, sigma)
+
+    reg_term_sum = 0
+
+    # for each result and group, plot the inner solution
+    for result, group in zip(inner_results, inner_problem.groups):
+        # For each group get the inner parameters and simulation
+        xs = inner_problem.get_xs_for_group(group)
+
+        s = result[SCIPY_X]
+
+        inner_parameters = np.array([x.value for x in xs])
+        simulation = inner_problem.groups[group][CURRENT_SIMULATION]
+
+        # For the simulation, get the spline bases
+        (
+            delta_c,
+            spline_bases,
+            n,
+        ) = SemiquantInnerSolver._rescale_spline_bases(
+            self=None,
+            sim_all=simulation,
+            N=len(inner_parameters),
+            K=len(simulation),
+        )
+
+        if inner_solver.options[REGULARIZE_SPLINE]:
+            reg_term = _calculate_regularization_for_group(
+                s=s,
+                N=len(inner_parameters),
+                c=spline_bases,
+                regularization_factor=inner_solver.options[
+                    'regularization_factor'
+                ],
+            )
+            reg_term_sum += reg_term
+
+    return reg_term_sum
```

### Comparing `pypesto-0.4.1/pypesto/visualize/waterfall.py` & `pypesto-0.4.2/pypesto/visualize/waterfall.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 )
 from .reference_points import ReferencePoint, create_references
 
 
 def waterfall(
     results: Union[Result, Sequence[Result]],
     ax: Optional[plt.Axes] = None,
-    size: Optional[Tuple[float]] = (18.5, 10.5),
+    size: Optional[tuple[float, float]] = (18.5, 10.5),
     y_limits: Optional[Tuple[float]] = None,
     scale_y: Optional[str] = 'log10',
     offset_y: Optional[float] = None,
     start_indices: Optional[Union[Sequence[int], int]] = None,
     n_starts_to_zoom: int = 0,
     reference: Optional[Sequence[ReferencePoint]] = None,
     colors: Optional[Union[RGBA, Sequence[RGBA]]] = None,
```

### Comparing `pypesto-0.4.1/pypesto.egg-info/SOURCES.txt` & `pypesto-0.4.2/pypesto.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,32 +23,36 @@
 pypesto/ensemble/__init__.py
 pypesto/ensemble/covariance_analysis.py
 pypesto/ensemble/dimension_reduction.py
 pypesto/ensemble/ensemble.py
 pypesto/ensemble/task.py
 pypesto/ensemble/util.py
 pypesto/hierarchical/__init__.py
-pypesto/hierarchical/calculator.py
+pypesto/hierarchical/base_parameter.py
+pypesto/hierarchical/base_problem.py
+pypesto/hierarchical/base_solver.py
 pypesto/hierarchical/inner_calculator_collector.py
-pypesto/hierarchical/parameter.py
 pypesto/hierarchical/petab.py
-pypesto/hierarchical/problem.py
-pypesto/hierarchical/solver.py
-pypesto/hierarchical/util.py
-pypesto/hierarchical/optimal_scaling/__init__.py
-pypesto/hierarchical/optimal_scaling/calculator.py
-pypesto/hierarchical/optimal_scaling/parameter.py
-pypesto/hierarchical/optimal_scaling/problem.py
-pypesto/hierarchical/optimal_scaling/solver.py
-pypesto/hierarchical/spline_approximation/__init__.py
-pypesto/hierarchical/spline_approximation/calculator.py
-pypesto/hierarchical/spline_approximation/parameter.py
-pypesto/hierarchical/spline_approximation/problem.py
-pypesto/hierarchical/spline_approximation/solver.py
+pypesto/hierarchical/ordinal/__init__.py
+pypesto/hierarchical/ordinal/calculator.py
+pypesto/hierarchical/ordinal/parameter.py
+pypesto/hierarchical/ordinal/problem.py
+pypesto/hierarchical/ordinal/solver.py
+pypesto/hierarchical/relative/__init__.py
+pypesto/hierarchical/relative/calculator.py
+pypesto/hierarchical/relative/problem.py
+pypesto/hierarchical/relative/solver.py
+pypesto/hierarchical/relative/util.py
+pypesto/hierarchical/semiquantitative/__init__.py
+pypesto/hierarchical/semiquantitative/calculator.py
+pypesto/hierarchical/semiquantitative/parameter.py
+pypesto/hierarchical/semiquantitative/problem.py
+pypesto/hierarchical/semiquantitative/solver.py
 pypesto/history/__init__.py
+pypesto/history/amici.py
 pypesto/history/base.py
 pypesto/history/csv.py
 pypesto/history/generate.py
 pypesto/history/hdf5.py
 pypesto/history/memory.py
 pypesto/history/optimizer.py
 pypesto/history/options.py
@@ -88,14 +92,15 @@
 pypesto/petab/__init__.py
 pypesto/petab/importer.py
 pypesto/predict/__init__.py
 pypesto/predict/amici_predictor.py
 pypesto/predict/task.py
 pypesto/problem/__init__.py
 pypesto/problem/base.py
+pypesto/problem/hierarchical.py
 pypesto/profile/__init__.py
 pypesto/profile/approximate.py
 pypesto/profile/options.py
 pypesto/profile/profile.py
 pypesto/profile/profile_next_guess.py
 pypesto/profile/task.py
 pypesto/profile/util.py
```

### Comparing `pypesto-0.4.1/pypesto.egg-info/requires.txt` & `pypesto-0.4.2/pypesto.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -38,28 +38,19 @@
 scikit-learn>=0.24.1
 sphinx>=6.2.1
 nbsphinx>=0.8.9
 nbconvert>=6.5.0
 sphinx-rtd-theme>=1.2.0
 sphinx-autodoc-typehints>=1.18.3
 sphinxcontrib-bibtex>=2.5.0
-ipython>=8.4.0
 myst-parser>=0.18.0
-ipykernel>=6.15.1
-networkx>=2.5.1
-petab-select>=0.1.8
-fides>=0.6.1
-amici>=0.18.0
-petab>=0.2.0
-aesara>=2.0.5
-jax>=0.4.1
-jaxlib>=0.4.1
+ipykernel==6.23.1
 notebook>=6.1.4
 networkx>=2.5.1
-petab-select>=0.1.8
+petab-select>=0.1.12
 pytest>=5.4.3
 pytest-cov>=2.10.0
 gitpython>=3.1.7
 pytest-rerunfailures>=9.1.1
 autograd>=1.3
 
 [all_optimizers]
@@ -85,31 +76,51 @@
 nbsphinx>=0.8.9
 nbconvert>=6.5.0
 sphinx-rtd-theme>=1.2.0
 sphinx-autodoc-typehints>=1.18.3
 sphinxcontrib-bibtex>=2.5.0
 ipython>=8.4.0
 myst-parser>=0.18.0
-ipykernel>=6.15.1
+ipykernel==6.23.1
+julia>=0.5.7
+pygments>=2.12.0
+arviz>=0.12.1
+aesara>=2.8.6
+pymc>=4.2.1
+emcee>=3.0.2
+dynesty>=2.0.3
+nlopt>=2.6.2
+pyswarm>=0.6
+notebook>=6.1.4
 networkx>=2.5.1
-petab-select>=0.1.8
+petab-select>=0.1.12
 fides>=0.6.1
 amici>=0.18.0
 petab>=0.2.0
 aesara>=2.0.5
 jax>=0.4.1
 jaxlib>=0.4.1
 
 [dynesty]
 dynesty>=2.0.3
 
 [emcee]
 emcee>=3.0.2
 
 [example]
+julia>=0.5.7
+ipython>=8.4.0
+pygments>=2.12.0
+arviz>=0.12.1
+aesara>=2.8.6
+pymc>=4.2.1
+emcee>=3.0.2
+dynesty>=2.0.3
+nlopt>=2.6.2
+pyswarm>=0.6
 notebook>=6.1.4
 
 [fides]
 fides>=0.6.1
 
 [ipopt]
 cyipopt>=1.3.0
@@ -145,15 +156,15 @@
 pyswarm>=0.6
 
 [pyswarms]
 pyswarms>=1.3.0
 
 [select]
 networkx>=2.5.1
-petab-select>=0.1.8
+petab-select>=0.1.12
 
 [test]
 pytest>=5.4.3
 pytest-cov>=2.10.0
 gitpython>=3.1.7
 pytest-rerunfailures>=9.1.1
 autograd>=1.3
```

### Comparing `pypesto-0.4.1/setup.cfg` & `pypesto-0.4.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -122,26 +122,33 @@
 	nbsphinx >= 0.8.9
 	nbconvert >= 6.5.0
 	sphinx-rtd-theme >= 1.2.0
 	sphinx-autodoc-typehints >= 1.18.3
 	sphinxcontrib-bibtex >= 2.5.0
 	ipython >= 8.4.0
 	myst-parser >= 0.18.0
-	ipykernel >= 6.15.1
+	ipykernel == 6.23.1
+	%(example)s
 	%(select)s
 	%(fides)s
 	%(amici)s
 	%(petab)s
 	%(aesara)s
 	%(jax)s
 example = 
+	%(julia)s
+	%(pymc)s
+	%(emcee)s
+	%(dynesty)s
+	%(nlopt)s
+	%(pyswarm)s
 	notebook >= 6.1.4
 select = 
 	networkx >= 2.5.1
-	petab-select >= 0.1.8
+	petab-select >= 0.1.12
 test = 
 	pytest >= 5.4.3
 	pytest-cov >= 2.10.0
 	gitpython >= 3.1.7
 	pytest-rerunfailures >= 9.1.1
 	autograd >= 1.3
```

