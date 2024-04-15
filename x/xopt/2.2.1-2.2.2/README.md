# Comparing `tmp/xopt-2.2.1.tar.gz` & `tmp/xopt-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-yekks0dj/xopt-2.2.1.tar", last modified: Fri Feb  9 00:25:27 2024, max compression
+gzip compressed data, was "/home/runner/work/Xopt/Xopt/dist/.tmp-6mpyfq9i/xopt-2.2.2.tar", last modified: Mon Apr 15 19:26:55 2024, max compression
```

## Comparing `xopt-2.2.1.tar` & `xopt-2.2.2.tar`

### file list

```diff
@@ -1,139 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-09 00:25:17.000000 xopt-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-09 00:25:17.000000 xopt-2.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-02-09 00:25:27.000000 xopt-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-02-09 00:25:17.000000 xopt-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-02-09 00:25:17.000000 xopt-2.2.1/benchmarks/test_mo.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-09 00:25:17.000000 xopt-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-09 00:25:27.000000 xopt-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-09 00:25:17.000000 xopt-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/tests/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/tests/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_bax.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_bayesian_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_custom_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_hessian_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_high_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_mggpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_mobo.py
--rw-r--r--   0 runner    (1001) docker     (127)    18358 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_model_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_time_dependent_bo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_turbo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/bayesian/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/test_extremum_seeking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/test_latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/test_neldermead.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/generators/test_rcds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_numerical_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9345 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_vocs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-02-09 00:25:17.000000 xopt-2.2.1/tests/test_xopt.py
--rw-r--r--   0 runner    (1001) docker     (127)    78325 2024-02-09 00:25:17.000000 xopt-2.2.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/asynchronous.py
--rw-r--r--   0 runner    (1001) docker     (127)    18139 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/bayesian/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/bayesian/bax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/bax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/bax/acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/bax/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/bax_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/bayesian_exploration.py
--rw-r--r--   0 runner    (1001) docker     (127)    27951 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/bayesian_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/hessian_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/heteroskedastic.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/custom_botorch/proximal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/expected_improvement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/mggpo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/mobo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/bayesian/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/models/prior_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/models/standard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/models/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/multi_fidelity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/objectives.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/time_dependent.py
--rw-r--r--   0 runner    (1001) docker     (127)     8507 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/turbo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/upper_confidence_bound.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16618 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/bayesian/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/es/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/es/extremumseeking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/ga/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/ga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/ga/cnsga.py
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/ga/deap_creator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/ga/deap_fitness_with_constraints.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3138 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/ga/fitness_with_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/rcds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/rcds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/rcds/rcds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/generators/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/scipy/latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (127)    17535 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/scipy/neldermead.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/mpi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/mpi/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/numerical_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26114 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/pydantic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/benchmarking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt/resources/test_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/ackley_20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/modified_tnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/multi_objective.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/sinusoid_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/sphere_20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/test_functions/tnk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/resources/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    23128 2024-02-09 00:25:17.000000 xopt-2.2.1/xopt/vocs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 00:25:27.000000 xopt-2.2.1/xopt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 19:26:51.000000 xopt-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 19:26:51.000000 xopt-2.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-15 19:26:55.000000 xopt-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8594 2024-04-15 19:26:51.000000 xopt-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:54.000000 xopt-2.2.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-15 19:26:51.000000 xopt-2.2.2/benchmarks/test_mo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 19:26:51.000000 xopt-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-15 19:26:55.000000 xopt-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 19:26:51.000000 xopt-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/tests/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/tests/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_bax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_bayesian_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_custom_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_hessian_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_high_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_mobo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19856 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_model_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_time_dependent_bo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_turbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/bayesian/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_extremum_seeking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/generators/test_rcds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_numerical_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10859 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_vocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-15 19:26:51.000000 xopt-2.2.2/tests/test_xopt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78325 2024-04-15 19:26:51.000000 xopt-2.2.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/asynchronous.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18279 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8344 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/bax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax/acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bayesian_exploration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27951 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/bayesian_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/hessian_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/heteroskedastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/custom_botorch/proximal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/expected_improvement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/mggpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/mobo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/bayesian/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/prior_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10944 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/standard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/models/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/multi_fidelity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/time_dependent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/upper_confidence_bound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17222 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/bayesian/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/es/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/es/extremumseeking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/ga/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/cnsga.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/deap_creator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3137 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/deap_fitness_with_constraints.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3138 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/ga/fitness_with_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/rcds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/rcds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14100 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/rcds/rcds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/generators/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/scipy/latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17535 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/scipy/neldermead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/mpi/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/numerical_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26153 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/benchmarking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt/resources/test_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/ackley_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/modified_tnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/multi_objective.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sinusoid_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sphere_100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sphere_20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/sphere_50.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/test_functions/tnk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/resources/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9610 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-04-15 19:26:51.000000 xopt-2.2.2/xopt/vocs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 19:26:55.000000 xopt-2.2.2/xopt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 19:26:54.000000 xopt-2.2.2/xopt.egg-info/top_level.txt
```

### Comparing `xopt-2.2.1/LICENSE` & `xopt-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/PKG-INFO` & `xopt-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 2.2.1
+Version: 2.2.2
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-2.2.1/README.md` & `xopt-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/benchmarks/test_mo.py` & `xopt-2.2.2/benchmarks/test_mo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/setup.py` & `xopt-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_bayesian_exploration.py` & `xopt-2.2.2/tests/generators/bayesian/test_bayesian_exploration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from copy import deepcopy
 
+import pytest
+
+from pydantic import ValidationError
+
 from xopt.base import Xopt
 from xopt.evaluator import Evaluator
 from xopt.generators.bayesian.bayesian_exploration import BayesianExplorationGenerator
 from xopt.resources.testing import TEST_VOCS_BASE, TEST_VOCS_DATA, xtest_callable
 
 
 class TestBayesianExplorationGenerator:
@@ -72,7 +76,13 @@
         X = Xopt(generator=gen, evaluator=evaluator, vocs=TEST_VOCS_BASE)
         X.add_data(TEST_VOCS_DATA)
 
         # now use bayes opt
         X.step()
         X.step()
         assert len(X.data) == 20
+
+    def test_vocs_validation(self):
+        test_vocs = deepcopy(TEST_VOCS_BASE)
+
+        with pytest.raises(ValidationError):
+            BayesianExplorationGenerator(vocs=test_vocs)
```

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_bayesian_generator.py` & `xopt-2.2.2/tests/generators/bayesian/test_bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_constraints.py` & `xopt-2.2.2/tests/generators/bayesian/test_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_custom_model.py` & `xopt-2.2.2/tests/generators/bayesian/test_custom_model.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_expected_improvement.py` & `xopt-2.2.2/tests/generators/bayesian/test_expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_hessian_kernel.py` & `xopt-2.2.2/tests/generators/bayesian/test_hessian_kernel.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_high_level.py` & `xopt-2.2.2/tests/generators/bayesian/test_high_level.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_mggpo.py` & `xopt-2.2.2/tests/generators/bayesian/test_mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_mobo.py` & `xopt-2.2.2/tests/generators/bayesian/test_mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_model_constructor.py` & `xopt-2.2.2/tests/generators/bayesian/test_model_constructor.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import yaml
 from botorch import fit_gpytorch_mll
 from botorch.models import HeteroskedasticSingleTaskGP, SingleTaskGP
 from botorch.models.transforms import Normalize, Standardize
 from gpytorch import ExactMarginalLogLikelihood
 from gpytorch.kernels import PeriodicKernel, PolynomialKernel, ScaleKernel
 from gpytorch.likelihoods import GaussianLikelihood
+from gpytorch.means import ConstantMean
 from gpytorch.priors import GammaPrior
 from pydantic import ValidationError
 
 from xopt.generators.bayesian.custom_botorch.heteroskedastic import (
     XoptHeteroskedasticSingleTaskGP,
 )
 from xopt.generators.bayesian.expected_improvement import ExpectedImprovementGenerator
@@ -433,14 +434,31 @@
         with torch.no_grad():
             generated_pred = generated_model.posterior(test_pts).mean[..., 0]
             benchmark_pred = benchmark_model.posterior(test_pts).mean[..., 0]
 
             assert torch.allclose(generated_pred, benchmark_pred, rtol=1e-3)
             assert ~torch.allclose(generated_pred, old_prediction, rtol=1e-3)
 
+    def test_unused_modules_warning(self):
+        test_vocs = deepcopy(TEST_VOCS_BASE)
+        test_data = deepcopy(TEST_VOCS_DATA)
+
+        # test unused covariance or mean module
+        kwargs_covar = {"covar_modules": {"faulty_output_name": PeriodicKernel()}}
+        kwargs_mean = {"mean_modules": {"faulty_output_name": ConstantMean()}}
+
+        for kwargs in [kwargs_covar, kwargs_mean]:
+            gp_constructor = StandardModelConstructor(**kwargs)
+            generator = ExpectedImprovementGenerator(
+                vocs=test_vocs, gp_constructor=gp_constructor
+            )
+            generator.add_data(test_data)
+            with pytest.warns(UserWarning):
+                _ = generator.train_model()
+
     def test_heteroskedastic(self):
         test_data = deepcopy(TEST_VOCS_DATA)
         test_vocs = deepcopy(TEST_VOCS_BASE)
 
         gp_constructor = StandardModelConstructor()
         model = gp_constructor.build_model_from_vocs(test_vocs, test_data)
         assert isinstance(model.models[0], SingleTaskGP)
@@ -483,14 +501,30 @@
         assert torch.allclose(
             posterior.mean[..., 0].flatten(), bposterior.mean.flatten()
         )
         assert torch.allclose(
             posterior.variance[..., 0].flatten(), bposterior.variance.flatten()
         )
 
+    def test_custom_noise_prior(self):
+        test_data = deepcopy(TEST_VOCS_DATA)
+        test_vocs = deepcopy(TEST_VOCS_BASE)
+
+        noise_prior = GammaPrior(1.0, 1000.0)
+
+        gp_constructor = StandardModelConstructor(custom_noise_prior=noise_prior)
+        model = gp_constructor.build_model_from_vocs(test_vocs, test_data)
+
+        # check if created models have the correct noise priors
+        assert model.models[0].likelihood.noise_covar.noise_prior.rate == 1000.0
+        assert model.models[0].likelihood.noise_covar.noise_prior.concentration == 1.0
+
+        assert model.models[1].likelihood.noise_covar.noise_prior.rate == 1000.0
+        assert model.models[1].likelihood.noise_covar.noise_prior.concentration == 1.0
+
     @pytest.fixture(autouse=True)
     def clean_up(self):
         yield
         files = ["test.yml", "covar_modules_y.pt", "covar_modules_c.pt"]
         for f in files:
             if os.path.exists(f):
                 os.remove(f)
```

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_multi_fidelity.py` & `xopt-2.2.2/tests/generators/bayesian/test_multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_time_dependent_bo.py` & `xopt-2.2.2/tests/generators/bayesian/test_time_dependent_bo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_turbo.py` & `xopt-2.2.2/tests/generators/bayesian/test_turbo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_upper_confidence_bound.py` & `xopt-2.2.2/tests/generators/bayesian/test_upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/bayesian/test_utils.py` & `xopt-2.2.2/tests/generators/bayesian/test_utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/test_extremum_seeking.py` & `xopt-2.2.2/tests/generators/test_extremum_seeking.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/test_latin_hypercube.py` & `xopt-2.2.2/tests/generators/test_latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/test_neldermead.py` & `xopt-2.2.2/tests/generators/test_neldermead.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             data = X.vocs.variable_data(X.data).to_numpy()
             if not np.array_equal(data, scipy_data[: i + 1, :]):
                 raise Exception
 
         data = X.vocs.variable_data(X.data).to_numpy()
         assert np.array_equal(data, scipy_data)
 
-        idx, best = X.vocs.select_best(X.data)
+        idx, best, _ = X.vocs.select_best(X.data)
         xbest = X.vocs.variable_data(X.data.loc[idx, :]).to_numpy().flatten()
         assert np.array_equal(
             xbest, result.x
         ), "Xopt Simplex does not match the vanilla one"
 
     @pytest.mark.parametrize(
         "fun,fstring,x0,v,cstep",
@@ -212,12 +212,12 @@
         # Numerical precision issues with using strings for floats, need tolerance
         assert np.allclose(data, scipy_data, rtol=0, atol=1e-10)
 
         data = X3.vocs.variable_data(X3.data).to_numpy()
         assert data.shape == scipy_data.shape
         assert np.allclose(data, scipy_data, rtol=0, atol=1e-10)
 
-        idx, best = X.vocs.select_best(X.data)
+        idx, best, _ = X.vocs.select_best(X.data)
         xbest = X.vocs.variable_data(X.data.loc[idx, :]).to_numpy().flatten()
         assert np.array_equal(
             xbest, result.x
         ), "Xopt Simplex does not match the vanilla one"
```

### Comparing `xopt-2.2.1/tests/generators/test_random.py` & `xopt-2.2.2/tests/generators/test_random.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/generators/test_rcds.py` & `xopt-2.2.2/tests/generators/test_rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_evaluator.py` & `xopt-2.2.2/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_generator.py` & `xopt-2.2.2/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_io.py` & `xopt-2.2.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_mpi.py` & `xopt-2.2.2/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_numerical_optimizer.py` & `xopt-2.2.2/tests/test_numerical_optimizer.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_perf.py` & `xopt-2.2.2/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_pydantic.py` & `xopt-2.2.2/tests/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_utils.py` & `xopt-2.2.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/tests/test_vocs.py` & `xopt-2.2.2/tests/test_vocs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from copy import deepcopy
 
 import numpy as np
 import pandas as pd
 import pytest
+from pydantic import ValidationError
 
 from xopt.resources.testing import TEST_VOCS_BASE, TEST_VOCS_DATA
 from xopt.vocs import ObjectiveEnum, VOCS
 
 
 class TestVOCS(object):
     def test_init(self):
@@ -22,14 +23,36 @@
         assert vocs.n_constraints == 0
 
     def test_empty_objectives(self):
         VOCS(
             variables={"x": [0, 1]},
         )
 
+    def test_constraint_specification(self):
+        good_constraint_list = [
+            ["LESS_THAN", 0],
+            ["GREATER_THAN", 0],
+            ["less_than", 0],
+            ["greater_than", 0],
+        ]
+
+        for ele in good_constraint_list:
+            VOCS(variables={"x": [0, 1]}, constraints={"c": ele})
+
+        bad_constraint_list = [
+            ["LESS_THAN"],
+            ["GREATER_TAN", 0],
+            [0, "less_than"],
+            ["greater_than", "ahc"],
+        ]
+
+        for ele in bad_constraint_list:
+            with pytest.raises(ValidationError):
+                VOCS(variables={"x": [0, 1]}, constraints={"c": ele})
+
     def test_from_yaml(self):
         Y = """
         variables:
           a: [0, 1e3] # Note that 1e3 usually parses as a str with YAML.
           b: [-1, 1]
         objectives:
           c: maximize
@@ -59,15 +82,19 @@
 
     def test_random_inputs(self):
         vocs = deepcopy(TEST_VOCS_BASE)
         n_samples = 10
         data = pd.DataFrame(vocs.random_inputs(n_samples))
         assert data.shape == (n_samples, vocs.n_inputs)
 
-        TEST_VOCS_BASE.random_inputs(5, include_constants=False)
+        test_inputs = TEST_VOCS_BASE.random_inputs(5, include_constants=False)
+        assert len(test_inputs) == 5
+
+        test_inputs = TEST_VOCS_BASE.random_inputs()
+        assert isinstance(test_inputs[0]["x1"], float)
 
     def test_serialization(self):
         vocs = deepcopy(TEST_VOCS_BASE)
         vocs.model_dump_json()
 
         vocs.variables["a"] = np.array([1, 2])
         vocs.model_dump_json()
@@ -177,37 +204,37 @@
                 "c1": [1.0, 0.0, 1.0, 0.0],
                 "y1": [0.5, 0.1, 1.0, 1.5],
             }
         )
 
         # test maximization
         vocs.objectives[vocs.objective_names[0]] = "MAXIMIZE"
-        idx, val = vocs.select_best(test_data)
+        idx, val, _ = vocs.select_best(test_data)
         assert idx == [2]
         assert val == [1.0]
 
         vocs.constraints = {}
-        idx, val = vocs.select_best(test_data)
+        idx, val, _ = vocs.select_best(test_data)
         assert idx == [3]
         assert val == [1.5]
 
         # test returning multiple best values -- sorted by best value
-        idx, val = vocs.select_best(test_data, 2)
+        idx, val, _ = vocs.select_best(test_data, 2)
         assert np.allclose(idx, np.array([3, 2]))
         assert np.allclose(val, np.array([1.5, 1.0]))
 
         # test minimization
         vocs.objectives[vocs.objective_names[0]] = "MINIMIZE"
         vocs.constraints = {"c1": ["GREATER_THAN", 0.5]}
-        idx, val = vocs.select_best(test_data)
+        idx, val, _ = vocs.select_best(test_data)
         assert idx == [0]
         assert val == [0.5]
 
         vocs.constraints = {}
-        idx, val = vocs.select_best(test_data)
+        idx, val, _ = vocs.select_best(test_data)
         assert idx == 1
         assert val == 0.1
 
     @pytest.mark.filterwarnings("ignore: All-NaN axis encountered")
     def test_cumulative_optimum(self):
         vocs = deepcopy(TEST_VOCS_BASE)
         obj_name = vocs.objective_names[0]
```

### Comparing `xopt-2.2.1/tests/test_xopt.py` & `xopt-2.2.2/tests/test_xopt.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/versioneer.py` & `xopt-2.2.2/versioneer.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/__init__.py` & `xopt-2.2.2/xopt/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/asynchronous.py` & `xopt-2.2.2/xopt/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
             Dict[str, List[float]],
             Dict[str, float],
         ],
     ):
         """
         Submit data to evaluator and return futures indexed to internal futures list.
 
-        Args:
+        Parameters
+        ----------
             input_data: dataframe containing input data
 
         """
 
         if not isinstance(input_data, DataFrame):
             try:
                 input_data = DataFrame(input_data)
```

### Comparing `xopt-2.2.1/xopt/base.py` & `xopt-2.2.2/xopt/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,38 +401,46 @@
         new_data.index = np.arange(len(new_data), dtype=np.int64)
         if inplace:
             self.data = new_data
             self.generator.data = new_data
         else:
             return new_data
 
-    def random_evaluate(self, n_samples=1, seed=None, **kwargs):
+    def random_evaluate(
+        self,
+        n_samples=None,
+        seed=None,
+        custom_bounds: dict = None,
+    ):
         """
         Convenience method to generate random inputs using VOCs and evaluate them.
 
         This method generates random inputs using the Variables, Objectives,
         Constraints, and Statics (VOCS) and evaluates them, adding the data to the
         Xopt object and generator.
 
         Parameters
         ----------
         n_samples : int, optional
             The number of random samples to generate.
         seed : int, optional
             The random seed for reproducibility.
-        **kwargs
-            Additional keyword arguments for generating random inputs.
+        custom_bounds : dict, optional
+            Dictionary of vocs-like ranges for random sampling
+
 
         Returns
         -------
         pd.DataFrame
             The results of the evaluations added to the internal DataFrame.
 
         """
-        random_inputs = self.vocs.random_inputs(n_samples, seed=seed, **kwargs)
+        random_inputs = self.vocs.random_inputs(
+            n_samples, seed=seed, custom_bounds=custom_bounds, include_constants=True
+        )
         result = self.evaluate_data(random_inputs)
         return result
 
     def yaml(self, **kwargs):
         """
         Serialize the Xopt configuration to a YAML string.
```

### Comparing `xopt-2.2.1/xopt/evaluator.py` & `xopt-2.2.2/xopt/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,17 @@
     function_kwargs : dict, default={}
         Any kwargs to pass on to this function.
     max_workers : int, default=1
         Maximum number of workers.
     executor : NormalExecutor
         NormalExecutor or any instantiated Executor object
     vectorized : bool, default=False
-        If true,
+        If true, lists of evaluation points will be sent to the evaluator
+        function to be processed in parallel instead of evaluated seperately via
+        mapping.
     """
 
     function: Callable
     max_workers: int = Field(1, ge=1)
     executor: NormalExecutor = Field(exclude=True)  # Do not serialize
     function_kwargs: dict = Field({})
     vectorized: bool = Field(False)
```

### Comparing `xopt-2.2.1/xopt/generator.py` & `xopt-2.2.2/xopt/generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/__init__.py` & `xopt-2.2.2/xopt/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/__init__.py` & `xopt-2.2.2/xopt/generators/bayesian/__init__.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/base_model.py` & `xopt-2.2.2/xopt/generators/bayesian/base_model.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/bax/acquisition.py` & `xopt-2.2.2/xopt/generators/bayesian/bax/acquisition.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     Example:
         >>> model1 = SingleTaskGP(train_X, train_Y1)
         >>> model2 = SingleTaskGP(train_X, train_Y2)
         >>> model = ModelList(model1, model2)
         >>> EIG = ExpectedInformationGain(model, algo)
         >>> eig = EIG(test_X)
 
-        Args:
+        Parameters
+        ----------
             model: A fitted independent multi-output (ModelList) model.
     """
 
     def __init__(self, model: Model, algorithm: Algorithm, bounds: Tensor) -> None:
         super().__init__(model=model)
         self.algorithm = algorithm
 
@@ -58,21 +59,23 @@
         ]
         self.fantasy_models = ModelList(*fantasy_models)
 
     @t_batch_mode_transform(expected_q=1, assert_output_shape=False)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate Expected Information Gain on the candidate set X.
 
-        Args:
+        Parameters
+        ----------
             X: A `(b1 x ... bk) x 1 x d`-dim batched tensor of `d`-dim design points.
                 Expected Information Gain is computed for each point individually,
                 i.e., what is considered are the marginal posteriors, not the
                 joint.
 
-        Returns:
+        Returns
+        -------
             A `(b1 x ... bk)`-dim tensor of Expected Information Gain values at the
             given design points `X`.
         """
 
         # Use the current & fantasy models to compute a
         # Monte-Carlo estimate of the Expected Information Gain:
         # see https://arxiv.org/pdf/2104.09460.pdf:
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/bax/algorithms.py` & `xopt-2.2.2/xopt/generators/bayesian/bax/algorithms.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         xx = torch.meshgrid(*linspace_list, indexing="ij")
         mesh_pts = torch.stack(xx).flatten(start_dim=1).T
 
         return mesh_pts
 
 
 class GridMinimize(GridScanAlgorithm):
-    model_names_ordered: List[str] = Field(
+    observable_names_ordered: List[str] = Field(
         default=["y1"],
         description="names of observable/objective models used in this algorithm",
     )
 
     def get_execution_paths(
         self, model: Model, bounds: Tensor
     ) -> Tuple[Tensor, Tensor, Dict]:
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/bax_generator.py` & `xopt-2.2.2/xopt/generators/bayesian/bax_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import pickle
 from copy import deepcopy
 from typing import Dict
 
-from pydantic import Field
+from pydantic import Field, field_validator
+from pydantic_core.core_schema import ValidationInfo
 
 from xopt.generators.bayesian.bax.acquisition import ModelListExpectedInformationGain
 from xopt.generators.bayesian.bax.algorithms import Algorithm
 from xopt.generators.bayesian.bayesian_generator import BayesianGenerator
 
 logger = logging.getLogger()
 
@@ -20,22 +21,28 @@
     )
     algorithm_results_file: str = Field(
         None, description="file name to save algorithm results at every step"
     )
 
     _n_calls: int = 0
 
+    @field_validator("vocs", mode="after")
+    def validate_vocs(cls, v, info: ValidationInfo):
+        if v.n_objectives != 0:
+            raise ValueError("this generator only supports observables")
+        return v
+
     def generate(self, n_candidates: int) -> list[dict]:
         self._n_calls += 1
         return super().generate(n_candidates)
 
     def _get_acquisition(self, model):
         bax_model_ids = [
             self.vocs.output_names.index(name)
-            for name in self.algorithm.model_names_ordered
+            for name in self.algorithm.observable_names_ordered
         ]
         bax_model = model.subset_output(bax_model_ids)
         eig = ModelListExpectedInformationGain(
             bax_model, self.algorithm, self._get_optimization_bounds()
         )
         self.algorithm_results = eig.algorithm_results
         if self.algorithm_results_file is not None:
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/bayesian_exploration.py` & `xopt-2.2.2/xopt/generators/bayesian/bayesian_exploration.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     supports_batch_generation: bool = True
 
     __doc__ = "Bayesian exploration generator\n" + formatted_base_docstring()
 
     @field_validator("vocs", mode="after")
     def validate_vocs(cls, v, info: ValidationInfo):
         if v.n_objectives != 0:
-            raise ValueError("this generator only supports zero objectives only")
+            raise ValueError("this generator only supports observables")
         return v
 
     def _get_acquisition(self, model):
         sampler = self._get_sampler(model)
         qPV = qPosteriorVariance(
             model,
             sampler=sampler,
@@ -51,15 +51,16 @@
         model: Model,
         sampler: Optional[MCSampler] = None,
         objective: Optional[MCAcquisitionObjective] = None,
         posterior_transform: Optional[PosteriorTransform] = None,
         X_pending: Optional[Tensor] = None,
     ) -> None:
         r"""q-Upper Confidence Bound.
-        Args:
+        Parameters
+        ----------
             model: A fitted model.
             sampler: The sampler used to draw base samples. Defaults to
                 `SobolQMCNormalSampler(num_samples=512, collapse_batch_dims=True)`
             objective: The MCAcquisitionObjective under which the samples are
                 evaluated. Defaults to `IdentityMCObjective()`.
             posterior_transform: A PosteriorTransform (optional).
             X_pending: A `batch_shape x m x d`-dim Tensor of `m` design points that have
@@ -75,18 +76,21 @@
             X_pending=X_pending,
         )
 
     @concatenate_pending_points
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate qUpperConfidenceBound on the candidate set `X`.
-        Args:
+        Parameters
+        ----------
             X: A `batch_sahpe x q x d`-dim Tensor of t-batches with `q` `d`-dim design
                 points each.
-        Returns:
+
+        Returns
+        -------
             A `batch_shape'`-dim Tensor of Upper Confidence Bound values at the given
             design points `X`, where `batch_shape'` is the broadcasted batch shape of
             model and input `X`.
         """
         posterior = self.model.posterior(
             X=X, posterior_transform=self.posterior_transform
         )
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/bayesian_generator.py` & `xopt-2.2.2/xopt/generators/bayesian/bayesian_generator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/constrained_acquisition.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 class FeasibilityObjective(GenericMCObjective):
     def __init__(
         self,
         constraints: List[Callable[[Tensor], Tensor]],
         infeasible_cost: float = 0.0,
         eta: float = 1e-3,
     ) -> None:
-        def ones_callable(X):
-            return torch.ones(X.shape[:-1])
+        def ones_callable(Z, X=None):
+            return torch.ones(Z.shape[:-1])
 
         super().__init__(objective=ones_callable)
         self.constraints = constraints
         self.eta = eta
         self.register_buffer("infeasible_cost", torch.as_tensor(infeasible_cost))
 
     def forward(self, samples: Tensor, X: Optional[Tensor] = None) -> Tensor:
         r"""Evaluate the feasibility-weighted objective on the samples.
 
-        Args:
+        Parameters
+        ----------
             samples: A `sample_shape x batch_shape x q x m`-dim Tensors of
                 samples from a model posterior.
             X: A `batch_shape x q x d`-dim tensor of inputs. Relevant only if
                 the objective depends on the inputs explicitly.
 
         Returns:
             A `sample_shape x batch_shape x q`-dim Tensor of objective values
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/hessian_kernel.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/hessian_kernel.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/heteroskedastic.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/heteroskedastic.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
         covar_module: Optional[Module] = None,
     ) -> None:
         r"""
         Xopt copy of HeteroskedasticSingleTaskGP from botorch which allows for a user
         to specify mean and covariance modules.
 
 
-        Args:
+        Parameters
+        ----------
             train_X: A `batch_shape x n x d` tensor of training features.
             train_Y: A `batch_shape x n x m` tensor of training observations.
             train_Yvar: A `batch_shape x n x m` tensor of observed measurement
                 noise.
             outcome_transform: An outcome transform that is applied to the
                 training data during instantiation and to the posterior during
                 inference (that is, the `Posterior` obtained by calling
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/identity.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/identity.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 class Identity(AcquisitionFunction):
     def __init__(self, model) -> None:
         super().__init__(model)
 
     @t_batch_mode_transform()
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate qUpperConfidenceBound on the candidate set `X`.
-        Args:
+        Parameters
+        ----------
             X: A `batch_sahpe x q x d`-dim Tensor of t-batches with `q` `d`-dim design
                 points each.
-        Returns:
+
+        Returns
+        -------
             A `batch_shape'`-dim Tensor of Upper Confidence Bound values at the given
             design points `X`, where `batch_shape'` is the broadcasted batch shape of
             model and input `X`.
         """
 
         return torch.ones(X.shape[:-2])
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/log_acquisition_function.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/multi_fidelity.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/multi_fidelity.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/custom_botorch/proximal.py` & `xopt-2.2.2/xopt/generators/bayesian/custom_botorch/proximal.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         proximal_weights: Tensor,
         transformed_weighting: bool = True,
         beta: float = 1.0,
     ) -> None:
         r"""Derived Acquisition Function weighted by proximity to recently
         observed point.
 
-        Args:
+        Parameters
+        ----------
             acq_function: The base acquisition function, operating on input tensors
                 of feature dimension `d`.
             proximal_weights: A `d` dim tensor used to bias locality
                 along each axis.
             transformed_weighting: If True, the proximal weights are applied in
                 the transformed input space given by
                 `acq_function.model.input_transform` (if available), otherwise
@@ -85,18 +86,20 @@
         self.register_buffer("beta", torch.tensor(beta))
         _validate_model(model, proximal_weights)
 
     @t_batch_mode_transform(expected_q=1, assert_output_shape=False)
     def forward(self, X: Tensor) -> Tensor:
         r"""Evaluate base acquisition function with proximal weighting.
 
-        Args:
+        Parameters
+        ----------
             X: Input tensor of feature dimension `d` .
 
-        Returns:
+        Returns
+        -------
             Base acquisition function evaluated on tensor `X` multiplied by proximal
             weighting.
         """
         model = self.acq_func.model
 
         train_inputs = model.train_inputs[0]
 
@@ -139,15 +142,16 @@
 
 def _validate_model(model: Model, proximal_weights: Tensor) -> None:
     r"""Validate model
 
     Perform vaidation checks on model used in base acquisition function to make sure
     it is compatible with proximal weighting.
 
-    Args:
+    Parameters
+    ----------
         model: Model associated with base acquisition function to be validated.
         proximal_weights: A `d` dim tensor used to bias locality
                 along each axis.
     """
 
     # check model for train_inputs and single batch
     if not hasattr(model, "train_inputs"):
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/expected_improvement.py` & `xopt-2.2.2/xopt/generators/bayesian/expected_improvement.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/mggpo.py` & `xopt-2.2.2/xopt/generators/bayesian/mggpo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/mobo.py` & `xopt-2.2.2/xopt/generators/bayesian/mobo.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/models/prior_mean.py` & `xopt-2.2.2/xopt/generators/bayesian/models/prior_mean.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
         model: torch.nn.Module,
         input_transformer: InputTransform,
         outcome_transformer: OutcomeTransform,
         fixed_model: bool = True,
     ):
         """Custom prior mean for a GP based on an arbitrary model.
 
-        Args:
+        Parameters
+        ----------
             model: Representation of the model.
             input_transformer: Module used to transform inputs in the GP.
             outcome_transformer: Module used to transform outcomes in the GP.
             fixed_model: If true, the model is put in evaluation mode and
               gradient computation is deactivated. Note that, even if this is
               set to false, model inference will always happen in evaluation
               mode unless training mode is reactivated in the base model.
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/models/standard.py` & `xopt-2.2.2/xopt/generators/bayesian/models/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os.path
+import warnings
 from copy import deepcopy
 from typing import Dict, List, Optional, Union
 
 import botorch.settings
 import pandas as pd
 import torch
 from botorch.models import ModelListGP
 from botorch.models.transforms import Normalize, Standardize
 from gpytorch.constraints import GreaterThan
 from gpytorch.kernels import Kernel
-from gpytorch.likelihoods import GaussianLikelihood
-from gpytorch.priors import GammaPrior
+from gpytorch.likelihoods import GaussianLikelihood, Likelihood
+from gpytorch.priors import GammaPrior, Prior
 from pydantic import ConfigDict, Field, field_validator
 from pydantic_core.core_schema import ValidationInfo
 from torch.nn import Module
 
 from xopt.generators.bayesian.base_model import ModelConstructor
 from xopt.generators.bayesian.models.prior_mean import CustomMean
 from xopt.generators.bayesian.utils import get_training_data
@@ -73,14 +74,19 @@
         [], description="list of prior mean modules that can be trained"
     )
     transform_inputs: Union[Dict[str, bool], bool] = Field(
         True,
         description="specify if inputs should be transformed inside the gp "
         "model, can optionally specify a dict of specifications",
     )
+    custom_noise_prior: Optional[Prior] = Field(
+        None,
+        description="specify custom noise prior for the GP likelihood, "
+        "overwrites value specified by use_low_noise_prior",
+    )
 
     model_config = ConfigDict(arbitrary_types_allowed=True, validate_assignment=True)
 
     @field_validator("covar_modules", "mean_modules", mode="before")
     def validate_torch_modules(cls, v):
         if not isinstance(v, dict):
             raise ValueError("must be dict")
@@ -97,24 +103,30 @@
     @field_validator("trainable_mean_keys")
     def validate_trainable_mean_keys(cls, v, info: ValidationInfo):
         for name in v:
             assert name in info.data["mean_modules"]
         return v
 
     @property
-    def likelihood(self):
+    def likelihood(self) -> Likelihood:
         """
-        Get the likelihood for the model, considering the low noise prior.
+        Get the likelihood for the model, considering the low noise prior and or a
+        custom noise prior.
 
         Returns
         -------
-        GaussianLikelihood
+        Likelihood
             The likelihood for the model.
 
         """
+        if self.custom_noise_prior is not None:
+            return GaussianLikelihood(
+                noise_prior=self.custom_noise_prior,
+            )
+
         if self.use_low_noise_prior:
             return GaussianLikelihood(
                 noise_prior=GammaPrior(1.0, 100.0),
             )
         else:
             noise_prior = GammaPrior(1.1, 0.05)
             noise_prior_mode = (noise_prior.concentration - 1) / noise_prior.rate
@@ -161,22 +173,24 @@
             A list of trained botorch models.
 
         """
         # build model
         tkwargs = {"dtype": dtype, "device": device}
         models = []
 
+        covar_modules = deepcopy(self.covar_modules)
+        mean_modules = deepcopy(self.mean_modules)
         for outcome_name in outcome_names:
             input_transform = self._get_input_transform(
                 outcome_name, input_names, input_bounds, tkwargs
             )
             outcome_transform = Standardize(1)
-            covar_module = self._get_module(self.covar_modules, outcome_name)
+            covar_module = self._get_module(covar_modules, outcome_name)
             mean_module = self.build_mean_module(
-                outcome_name, input_transform, outcome_transform
+                outcome_name, mean_modules, input_transform, outcome_transform
             )
 
             # get training data
             train_X, train_Y, train_Yvar = get_training_data(
                 input_names, outcome_name, data
             )
             # collect arguments into a single dict
@@ -190,53 +204,66 @@
             if train_Yvar is None:
                 # train basic single-task-gp model
                 models.append(
                     self.build_single_task_gp(
                         train_X.to(**tkwargs),
                         train_Y.to(**tkwargs),
                         likelihood=self.likelihood,
-                        **kwargs
+                        **kwargs,
                     )
                 )
             else:
                 # train heteroskedastic single-task-gp model
                 # turn off warnings
                 models.append(
                     self.build_heteroskedastic_gp(
                         train_X.to(**tkwargs),
                         train_Y.to(**tkwargs),
                         train_Yvar.to(**tkwargs),
-                        **kwargs
+                        **kwargs,
                     )
                 )
+        # check all specified modules were added to the model
+        if covar_modules:
+            warnings.warn(
+                f"Covariance modules for output names {[k for k, v in self.covar_modules.items()]} "
+                f"could not be added to the model."
+            )
+        if mean_modules:
+            warnings.warn(
+                f"Mean modules for output names {[k for k, v in self.mean_modules.items()]} "
+                f"could not be added to the model."
+            )
 
         return ModelListGP(*models)
 
     def build_mean_module(
-        self, name, input_transform, outcome_transform
+        self, name, mean_modules, input_transform, outcome_transform
     ) -> Optional[CustomMean]:
         """
         Build the mean module for the output specified by name.
 
         Parameters
         ----------
         name : str
             The name of the output.
+        mean_modules: dict
+            The dictionary of mean modules.
         input_transform : InputTransform
             Transform for input variables.
         outcome_transform : OutcomeTransform
             Transform for outcome variables.
 
         Returns
         -------
         Optional[CustomMean]
             The mean module for the output, or None if not specified.
 
         """
-        mean_module = self._get_module(self.mean_modules, name)
+        mean_module = self._get_module(mean_modules, name)
         if mean_module is not None:
             fixed_model = False if name in self.trainable_mean_keys else True
             mean_module = CustomMean(
                 mean_module, input_transform, outcome_transform, fixed_model=fixed_model
             )
         return mean_module
 
@@ -257,15 +284,15 @@
         Module
             The retrieved module.
 
         """
         if isinstance(base, Module):
             return deepcopy(base)
         elif isinstance(base, dict):
-            return deepcopy(base.get(name))
+            return deepcopy(base.pop(name, None))
         else:
             return None
 
     def _get_input_transform(self, outcome_name, input_names, input_bounds, tkwargs):
         """get input transform based on the supplied bounds and attributes"""
         # get input bounds
         if input_bounds is None:
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/models/time_dependent.py` & `xopt-2.2.2/xopt/generators/bayesian/models/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/multi_fidelity.py` & `xopt-2.2.2/xopt/generators/bayesian/multi_fidelity.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         weights = torch.zeros(self.vocs.n_outputs, **self._tkwargs)
         for idx, ele in enumerate(self.vocs.objective_names):
             if self.vocs.objectives[ele] == "MINIMIZE":
                 weights[idx] = -1.0
             elif self.vocs.objectives[ele] == "MAXIMIZE":
                 weights[idx] = 1.0
 
-        def obj_callable(Z):
+        def obj_callable(Z, X=None):
             return torch.matmul(Z, weights.reshape(-1, 1)).squeeze(-1)
 
         c_posterior_mean = ConstrainedMCAcquisitionFunction(
             self.model,
             qUpperConfidenceBound(
                 model=self.model, beta=0.0, objective=GenericMCObjective(obj_callable)
             ),
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/objectives.py` & `xopt-2.2.2/xopt/generators/bayesian/objectives.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,26 +63,26 @@
 
     """
     n_outputs = vocs.n_outputs
     weights = torch.zeros(n_outputs).to(**tkwargs)
 
     weights = set_botorch_weights(weights, vocs)
 
-    def obj_callable(Z):
+    def obj_callable(Z, X=None):
         return torch.matmul(Z, weights.reshape(-1, 1)).squeeze(-1)
 
     return GenericMCObjective(obj_callable)
 
 
 def create_exploration_objective(vocs, tkwargs):
     n_outputs = vocs.n_outputs
     weights = torch.zeros(n_outputs).to(**tkwargs)
     weights[0] = 1.0
 
-    def obj_callable(Z):
+    def obj_callable(Z, X=None):
         return torch.matmul(Z, weights.reshape(-1, 1)).squeeze(-1)
 
     return GenericMCObjective(obj_callable)
 
 
 def create_mobo_objective(vocs, tkwargs):
     """
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/time_dependent.py` & `xopt-2.2.2/xopt/generators/bayesian/time_dependent.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/turbo.py` & `xopt-2.2.2/xopt/generators/bayesian/turbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         self.center_x = (
             variable_data.loc[best_idx][self.vocs.variable_names].iloc[0].to_dict()
         )
 
     def update_state(self, data: DataFrame, previous_batch_size: int = 1) -> None:
         """
         Update turbo state class using min of data points that are feasible.
-        Otherwise raise an error
+        If no points in the data set are feasible raise an error.
 
         NOTE: this is the opposite of botorch which assumes maximization, xopt assumes
         minimization
 
         Parameters
         ----------
         data : DataFrame
@@ -160,15 +160,15 @@
 
         """
         # get locations of valid data samples
         feas_data = self.vocs.feasibility_data(data)
 
         if len(data[feas_data["feasible"]]) == 0:
             raise RuntimeError(
-                "turbo requires at least one valid point in training " "dataset"
+                "turbo requires at least one valid point in the training dataset"
             )
         else:
             self._set_best_point(data[feas_data["feasible"]])
 
         # get feasibility of last `n_candidates`
         recent_data = data.iloc[-previous_batch_size:]
         f_data = self.vocs.feasibility_data(recent_data)
```

### Comparing `xopt-2.2.1/xopt/generators/bayesian/upper_confidence_bound.py` & `xopt-2.2.2/xopt/generators/bayesian/upper_confidence_bound.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/utils.py` & `xopt-2.2.2/xopt/generators/bayesian/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/bayesian/visualize.py` & `xopt-2.2.2/xopt/generators/bayesian/visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,42 +18,59 @@
     """Displays GP model predictions for the selected output(s).
 
     The GP models are displayed with respect to the named variables. If None are given, the list of variables in
     generator.vocs is used. Feasible samples are indicated with a filled orange "o", infeasible samples with a
     hollow red "o". Feasibility is calculated with respect to all constraints unless the selected output is a
     constraint itself, in which case only that one is considered.
 
-    Args:
-        generator: Bayesian generator object.
-        output_names: Outputs for which the GP models are displayed. Defaults to all outputs in generator.vocs.
-        variable_names: The variables with respect to which the GP models are displayed (maximum of 2).
-          Defaults to generator.vocs.variable_names.
-        idx: Index of the last sample to use. This also selects the point of reference in higher dimensions unless
-          an explicit reference_point is given.
-        reference_point: Reference point determining the value of variables in generator.vocs.variable_names,
-          but not in variable_names (slice plots in higher dimensions). Defaults to last used sample.
-        show_samples: Whether samples are shown.
-        show_prior_mean: Whether the prior mean is shown.
-        show_feasibility: Whether the feasibility region is shown.
-        show_acquisition: Whether the acquisition function is computed and shown.
-        n_grid: Number of grid points per dimension used to display the model predictions.
+    Parameters
+    ----------
+        generator : Generator
+            Bayesian generator object.
+        output_names : List[str]
+            Outputs for which the GP models are displayed. Defaults to all outputs in
+            generator.vocs.
+        variable_names : List[str]
+            The variables with respect to which the GP models are displayed (maximum
+            of 2). Defaults to generator.vocs.variable_names.
+        idx : int
+            Index of the last sample to use. This also selects the point of reference in
+            higher dimensions unless an explicit reference_point is given.
+        reference_point : dict
+            Reference point determining the value of variables in
+            generator.vocs.variable_names, but not in variable_names (slice plots in
+            higher dimensions). Defaults to last used sample.
+        show_samples : bool, optional
+            Whether samples are shown.
+        show_prior_mean : bool, optional
+            Whether the prior mean is shown.
+        show_feasibility : bool, optional
+            Whether the feasibility region is shown.
+        show_acquisition : bool, optional
+            Whether the acquisition function is computed and shown.
+        n_grid : int, optional
+        Number of grid points per dimension used to display the model predictions.
 
     Returns:
+    --------
         The matplotlib figure and axes objects.
     """
 
     # define output and variable names
     vocs, data = generator.vocs, generator.data
     if output_names is None:
         output_names = vocs.output_names
     if variable_names is None:
         variable_names = vocs.variable_names
     dim_x, dim_y = len(variable_names), len(output_names)
     if dim_x not in [1, 2]:
-        raise ValueError(f"Number of variables should be 1 or 2, not {dim_x}.")
+        raise ValueError(
+            f"Visualization is only supported with respect to 1 or 2 variables, not {dim_x}. "
+            f"Provide a compatible list of variable names to create slice plots at higher dimensions."
+        )
 
     # check names exist in vocs
     for names, s in zip(
         [output_names, variable_names], ["output_names", "variable_names"]
     ):
         invalid = [name not in getattr(vocs, s) for name in names]
         if any(invalid):
@@ -280,14 +297,15 @@
             for j in range(ncols):
                 ax_ij = ax[i, j] if nrows > 1 else ax[j]
                 # model predictions
                 pcm = ax_ij.pcolormesh(
                     x_mesh[0].numpy(),
                     x_mesh[1].numpy(),
                     predictions[output_name][j].reshape(n_grid, n_grid),
+                    rasterized=True,
                 )
                 divider = make_axes_locatable(ax_ij)
                 cax = divider.append_axes("right", size="5%", pad=0.1)
                 cbar = fig.colorbar(pcm, cax=cax)
                 if j == 0:
                     ax_ij.set_title(f"Posterior Mean [{output_name}]")
                     cbar.set_label(output_name)
@@ -344,27 +362,29 @@
             pass
         else:
             if predictions["acq"][0] is None:
                 pcm = ax[len(output_names), 0].pcolormesh(
                     x_mesh[0].numpy(),
                     x_mesh[1].numpy(),
                     predictions["acq"][1].reshape(n_grid, n_grid),
+                    rasterized=True,
                 )
                 divider = make_axes_locatable(ax[len(output_names), 0])
                 cax = divider.append_axes("right", size="5%", pad=0.1)
                 cbar = fig.colorbar(pcm, cax=cax)
                 cbar.set_label(r"$\alpha\,$[{}]".format(vocs.output_names[0]))
                 ax[len(output_names), 0].set_title("Acq. Function")
                 ax[len(output_names), 1].axis("off")
             else:
                 for j in range(2):
                     pcm = ax[len(output_names), j].pcolormesh(
                         x_mesh[0].numpy(),
                         x_mesh[1].numpy(),
                         predictions["acq"][j].reshape(n_grid, n_grid),
+                        rasterized=True,
                     )
                     divider = make_axes_locatable(ax[len(output_names), j])
                     cax = divider.append_axes("right", size="5%", pad=0.1)
                     cbar = fig.colorbar(pcm, cax=cax)
                     cbar.set_label(r"$\alpha\,$[{}]".format(vocs.output_names[0]))
                 ax[len(output_names), 0].set_title("Base Acq. Function")
                 ax[len(output_names), 1].set_title("Constrained Acq. Function")
@@ -379,14 +399,15 @@
             else:
                 ax_feasibility = ax[-1, 0]
                 ax[-1, 1].axis("off")
             pcm = ax_feasibility.pcolormesh(
                 x_mesh[0].numpy(),
                 x_mesh[1].numpy(),
                 predictions["feasibility"].reshape(n_grid, n_grid),
+                rasterized=True,
             )
             divider = make_axes_locatable(ax_feasibility)
             cax = divider.append_axes("right", size="5%", pad=0.1)
             cbar = fig.colorbar(pcm, cax=cax)
             cbar.set_label("Feasibility")
             ax_feasibility.set_title("Feasibility")
         else:
```

### Comparing `xopt-2.2.1/xopt/generators/es/extremumseeking.py` & `xopt-2.2.2/xopt/generators/es/extremumseeking.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/ga/cnsga.py` & `xopt-2.2.2/xopt/generators/ga/cnsga.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/ga/deap_creator.py` & `xopt-2.2.2/xopt/generators/ga/deap_creator.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/ga/deap_fitness_with_constraints.py` & `xopt-2.2.2/xopt/generators/ga/deap_fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/ga/fitness_with_constraints.py` & `xopt-2.2.2/xopt/generators/ga/fitness_with_constraints.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/rcds/rcds.py` & `xopt-2.2.2/xopt/generators/rcds/rcds.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/scipy/latin_hypercube.py` & `xopt-2.2.2/xopt/generators/scipy/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/scipy/neldermead.py` & `xopt-2.2.2/xopt/generators/scipy/neldermead.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/generators/utils.py` & `xopt-2.2.2/xopt/generators/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/log.py` & `xopt-2.2.2/xopt/log.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/mpi/run.py` & `xopt-2.2.2/xopt/mpi/run.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/numerical_optimizer.py` & `xopt-2.2.2/xopt/numerical_optimizer.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/pydantic.py` & `xopt-2.2.2/xopt/pydantic.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,20 +596,22 @@
         return map_fn(fn, *iter, **kwargs)
 
 
 def get_callable_from_string(callable: str, bind: Any = None) -> Callable:
     """Get callable from a string. In the case that the callable points to a bound method,
     the function returns a callable taking the bind instance as the first arg.
 
-    Args:
+        Parameters
+        ----------
         callable: String representation of callable abiding convention
              __module__:callable
         bind: Class to bind as self
 
-    Returns:
+    Returns
+    -------
         Callable
     """
     callable_split = callable.rsplit(".", 1)
 
     if len(callable_split) != 2:
         raise ValueError(f"Improperly formatted callable string: {callable_split}")
```

### Comparing `xopt-2.2.1/xopt/resources/benchmarking.py` & `xopt-2.2.2/xopt/resources/benchmarking.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/test_functions/ackley_20.py` & `xopt-2.2.2/xopt/resources/test_functions/ackley_20.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/test_functions/modified_tnk.py` & `xopt-2.2.2/xopt/resources/test_functions/modified_tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/test_functions/multi_objective.py` & `xopt-2.2.2/xopt/resources/test_functions/multi_objective.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/test_functions/problem.py` & `xopt-2.2.2/xopt/resources/test_functions/problem.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/test_functions/rosenbrock.py` & `xopt-2.2.2/xopt/resources/test_functions/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/test_functions/tnk.py` & `xopt-2.2.2/xopt/resources/test_functions/tnk.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/resources/testing.py` & `xopt-2.2.2/xopt/resources/testing.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/utils.py` & `xopt-2.2.2/xopt/utils.py`

 * *Files identical despite different names*

### Comparing `xopt-2.2.1/xopt/vocs.py` & `xopt-2.2.2/xopt/vocs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import Any, Dict, List, Union
 
 import numpy as np
 import pandas as pd
 import yaml
 from pandas import DataFrame
-from pydantic import ConfigDict, conlist, Field
+from pydantic import ConfigDict, conlist, Field, field_validator
 
 from xopt.pydantic import XoptBaseModel
 
 
 # Enums for objectives and constraints
 class ObjectiveEnum(str, Enum):
     MINIMIZE = "MINIMIZE"
@@ -26,17 +26,18 @@
 class ConstraintEnum(str, Enum):
     LESS_THAN = "LESS_THAN"
     GREATER_THAN = "GREATER_THAN"
 
     # Allow any case
     @classmethod
     def _missing_(cls, name):
-        for member in cls:
-            if member.name.lower() == name.lower():
-                return member
+        if isinstance(name, str):
+            for member in cls:
+                if member.name.lower() == name.lower():
+                    return member
 
 
 class VOCS(XoptBaseModel):
     """
     Variables, Objectives, Constraints, and other Settings (VOCS) data structure
     to describe optimization problems.
     """
@@ -62,14 +63,32 @@
         description="observation names tracked alongside objectives and constraints",
     )
 
     model_config = ConfigDict(
         validate_assignment=True, use_enum_values=True, extra="forbid"
     )
 
+    @field_validator("constraints")
+    def coorect_list_types(cls, v):
+        """make sure that constraint list types are correct"""
+        for _, item in v.items():
+            if not isinstance(item[0], str):
+                raise ValueError(
+                    "constraint specification list must have the first "
+                    "element as a string`"
+                )
+
+            if not isinstance(item[1], float):
+                raise ValueError(
+                    "constraint specification list must have the second "
+                    "element as a float"
+                )
+
+        return v
+
     @classmethod
     def from_yaml(cls, yaml_text):
         loaded = yaml.safe_load(yaml_text)
         return cls(**loaded)
 
     def as_yaml(self):
         return yaml.dump(self.model_dump(), default_flow_style=None, sort_keys=False)
@@ -211,23 +230,22 @@
             )
             bounds = custom_bounds.to_dict()
             for k in bounds.keys():
                 bounds[k] = [bounds[k][i] for i in range(2)]
 
         for key, val in bounds.items():  # No need to sort here
             a, b = val
-            n = n if n is not None else 1
             x = rng_sample_function(n)
             inputs[key] = x * a + (1 - x) * b
 
         # Constants
         if include_constants and self.constants is not None:
             inputs.update(self.constants)
 
-        if n == 1:
+        if n is None:
             return [inputs]
         else:
             return pd.DataFrame(inputs).to_dict("records")
 
     def convert_dataframe_to_inputs(
         self, data: pd.DataFrame, include_constants=True
     ) -> pd.DataFrame:
@@ -271,93 +289,118 @@
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "variable_",
     ) -> pd.DataFrame:
         """
         Returns a dataframe containing variables according to `vocs.variables` in sorted
         order
 
-        Args:
-            data: Data to be processed.
-            prefix: Prefix added to column names.
+        Parameters
+        ----------
+            data: DataFrame
+                Data to be processed.
+            prefix: str, optional
+                Prefix added to column names.
 
-        Returns:
-            result: processed Dataframe
+        Returns
+        -------
+            result: DataFrame
+                Processed Dataframe
         """
         return form_variable_data(self.variables, data, prefix=prefix)
 
     def objective_data(
         self,
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "objective_",
         return_raw=False,
     ) -> pd.DataFrame:
         """
         Returns a dataframe containing objective data transformed according to
         `vocs.objectives` such that we always assume minimization.
 
-        Args:
-            data: data to be processed.
-            prefix: prefix added to column names.
+        Parameters
+        ----------
+            data: DataFrame
+                Data to be processed.
+            prefix: str, optional
+                Prefix added to column names.
 
-        Returns:
-            result: processed Dataframe
+        Returns
+        -------
+            result: DataFrame
+                Processed Dataframe
         """
         return form_objective_data(self.objectives, data, prefix, return_raw)
 
     def constraint_data(
         self,
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "constraint_",
     ) -> pd.DataFrame:
         """
         Returns a dataframe containing constraint data transformed according to
         `vocs.constraints` such that values that satisfy each constraint are negative.
 
-        Args:
-            data: data to be processed.
-            prefix: prefix added to column names.
+        Parameters
+        ----------
+            data: DataFrame
+                Data to be processed.
+            prefix: str, optional
+                Prefix added to column names.
 
-        Returns:
-            result: processed Dataframe
+        Returns
+        -------
+            result: DataFrame
+                Processed Dataframe
         """
         return form_constraint_data(self.constraints, data, prefix)
 
     def observable_data(
         self,
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "observable_",
     ) -> pd.DataFrame:
         """
         Returns a dataframe containing observable data
 
-        Args:
-            data: data to be processed.
-            prefix: prefix added to column names.
+        Parameters
+        ----------
+            data: DataFrame
+                Data to be processed.
+            prefix: str, optional
+                Prefix added to column names.
 
-        Returns:
-            result: processed Dataframe
+        Returns
+        -------
+            result: DataFrame
+                Processed Dataframe
         """
         return form_observable_data(self.observable_names, data, prefix)
 
     def feasibility_data(
         self,
         data: Union[pd.DataFrame, List[Dict], List[Dict]],
         prefix: str = "feasible_",
     ) -> pd.DataFrame:
         """
         Returns a dataframe containing booleans denoting if a constraint is satisfied or
         not. Returned dataframe also contains a column `feasible` which denotes if
         all constraints are satisfied.
 
-        Args:
-            data: data to be processed.
-            prefix: prefix added to column names.
+        Parameters
+        ----------
+            data: DataFrame
+                Data to be processed.
+            prefix: str, optional
+                Prefix added to column names.
 
-        Returns:
-            result: processed Dataframe
+        Returns
+        -------
+            result: DataFrame
+                Processed Dataframe
         """
         return form_feasibility_data(self.constraints, data, prefix)
 
     def normalize_inputs(self, input_points: pd.DataFrame) -> pd.DataFrame:
         """
         Normalize input data (transform data into the range [0,1]) based on the
         variable ranges defined in the VOCS.
@@ -365,15 +408,15 @@
         Parameters
         ----------
         input_points : pd.DataFrame
             A DataFrame containing input data to be normalized.
 
         Returns
         -------
-        pd.DataFrame
+        result : pd.DataFrame
             A DataFrame with input data in the range [0,1] corresponding to the
             specified variable ranges. Contains columns equal to the intersection
             between `input_points` and `vocs.variable_names`.
 
         Notes
         -----
 
@@ -402,15 +445,15 @@
         Parameters
         ----------
         input_points : pd.DataFrame
             A DataFrame containing normalized input data in the range [0,1].
 
         Returns
         -------
-        pd.DataFrame
+        result : pd.DataFrame
             A DataFrame with denormalized input data corresponding to the
             specified variable ranges. Contains columns equal to the intersection
             between `input_points` and `vocs.variable_names`.
 
         Notes
         -----
 
@@ -432,86 +475,106 @@
             return pd.DataFrame([])
 
     def validate_input_data(self, input_points: pd.DataFrame) -> None:
         """
         Validates input data. Raises an error if the input data does not satisfy
         requirements given by vocs.
 
-        Args:
-            input_points: input data to be validated.
+        Parameters
+        ----------
+            input_points : DataFrame
+                Input data to be validated.
 
-        Returns:
+        Returns
+        -------
             None
 
-        Raises:
+        Raises
+        ------
             ValueError: if input data does not satisfy requirements.
         """
         validate_input_data(self, input_points)
 
     def extract_data(self, data: pd.DataFrame, return_raw=False):
         """
         split dataframe into seperate dataframes for variables, objectives and
         constraints based on vocs - objective data is transformed based on
         `vocs.objectives` properties
 
-        Args:
-            data: dataframe to be split
-            return_raw: if True, return untransformed objective data
-
-        Returns:
-            variable_data: dataframe containing variable data
-            objective_data: dataframe containing objective data
-            constraint_data: dataframe containing constraint data
+        Parameters
+        ----------
+            data: DataFrame
+                Dataframe to be split
+            return_raw : bool, optional
+                If True, return untransformed objective data
+
+        Returns
+        -------
+            variable_data : DataFrame
+                Dataframe containing variable data
+            objective_data : DataFrame
+                Dataframe containing objective data
+            constraint_data : DataFrame
+                Dataframe containing constraint data
         """
         variable_data = self.variable_data(data, "")
         objective_data = self.objective_data(data, "", return_raw)
         constraint_data = self.constraint_data(data, "")
         return variable_data, objective_data, constraint_data
 
-    def select_best(self, data: pd.DataFrame, n=1):
+    def select_best(self, data: pd.DataFrame, n: int = 1):
         """
         get the best value and point for a given data set based on vocs
         - does not work for multi-objective problems
         - data that violates any constraints is ignored
 
-        Args:
-            data: dataframe to select best point from
-            n: number of best points to return
+        Parameters
+        ----------
+            data: DataFrame
+                Dataframe to select best point from
+            n: int, optional
+                Number of best points to return
 
-        Returns:
+        Returns
+        -------
             index: index of best point
             value: value of best point
+            params: input parameters that give the best point
         """
         if self.n_objectives != 1:
             raise NotImplementedError(
                 "cannot select best point when n_objectives is not 1"
             )
 
         feasible_data = self.feasibility_data(data)
         ascending_flag = {"MINIMIZE": True, "MAXIMIZE": False}
         obj = self.objectives[self.objective_names[0]]
         obj_name = self.objective_names[0]
         res = data[feasible_data["feasible"]].sort_values(
             obj_name, ascending=ascending_flag[obj]
         )[obj_name][:n]
 
-        return res.index.to_numpy(), res.to_numpy()
+        params = data.iloc[res.index.to_numpy()][self.variable_names].to_dict(
+            orient="records"
+        )[0]
+
+        return res.index.to_numpy(), res.to_numpy(), params
 
     def cumulative_optimum(self, data: pd.DataFrame) -> pd.DataFrame:
         """
         Returns the cumulative optimum for the given DataFrame.
 
         Parameters
         ----------
-        data: pd.DataFrame
+        data: DataFrame
             Data for which the cumulative optimum shall be calculated.
 
         Returns
         -------
-        pd.DataFrame
+        DataFrame
             Cumulative optimum for the given DataFrame.
 
         """
         if not self.objectives:
             raise RuntimeError("No objectives defined.")
         if data.empty:
             return pd.DataFrame()
@@ -618,18 +681,22 @@
 
 
 def form_constraint_data(constraints: Dict, data: pd.DataFrame, prefix="constraint_"):
     """
     Use constraint dict and data (dataframe) to generate constraint data (dataframe). A
     constraint is satisfied if the evaluation is < 0.
 
-    Args:
-        constraints: Dictionary of constraints
-        data: Dataframe with the data to be evaluated
-        prefix: Prefix to use for the transformed data in the dataframe
+    Parameters
+    ----------
+        constraints: dict
+            Dictionary of constraints
+        data: DataFrame
+            Dataframe with the data to be evaluated
+        prefix: str, optional
+            Prefix to use for the transformed data in the dataframe
 
     Returns a dataframe with the constraint data.
 
     Missing or nan values will be filled with: np.inf
 
     """
     if not constraints:
@@ -661,18 +728,22 @@
 
 
 def form_observable_data(observables: List, data: pd.DataFrame, prefix="observable_"):
     """
     Use constraint dict and data (dataframe) to generate constraint data (dataframe). A
     constraint is satisfied if the evaluation is < 0.
 
-    Args:
-        observables: Dictonary of constraints
-        data: Dataframe with the data to be evaluated
-        prefix: Prefix to use for the transformed data in the dataframe
+    Parameters
+    ----------
+        observables: dict
+            Dictionary of observables
+        data: DataFrame
+            Dataframe with the data to be evaluated
+        prefix: str, optional
+            Prefix to use for the transformed data in the dataframe
 
     Returns a dataframe with the constraint data.
 
     Missing or nan values will be filled with: np.inf
 
     """
     if not observables:
```

### Comparing `xopt-2.2.1/xopt.egg-info/PKG-INFO` & `xopt-2.2.2/xopt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xopt
-Version: 2.2.1
+Version: 2.2.2
 Home-page: https://github.com/ChristopherMayes/xopt
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align="center">
   <img src="docs/assets/Xopt-logo.png", width="200">
```

### Comparing `xopt-2.2.1/xopt.egg-info/SOURCES.txt` & `xopt-2.2.2/xopt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -111,9 +111,11 @@
 xopt/resources/test_functions/__init__.py
 xopt/resources/test_functions/ackley_20.py
 xopt/resources/test_functions/modified_tnk.py
 xopt/resources/test_functions/multi_objective.py
 xopt/resources/test_functions/problem.py
 xopt/resources/test_functions/rosenbrock.py
 xopt/resources/test_functions/sinusoid_1d.py
+xopt/resources/test_functions/sphere_100.py
 xopt/resources/test_functions/sphere_20.py
+xopt/resources/test_functions/sphere_50.py
 xopt/resources/test_functions/tnk.py
```

