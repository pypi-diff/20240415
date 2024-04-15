# Comparing `tmp/mri-nufft-0.6.1.tar.gz` & `tmp/mri_nufft-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mri-nufft-0.6.1.tar", last modified: Wed Feb 21 15:16:54 2024, max compression
+gzip compressed data, was "mri_nufft-0.6.2.tar", last modified: Mon Apr 15 13:26:44 2024, max compression
```

## Comparing `mri-nufft-0.6.1.tar` & `mri_nufft-0.6.2.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.555469 mri-nufft-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.531469 mri-nufft-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.535469 mri-nufft-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-21 15:16:54.555469 mri-nufft-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.539469 mri-nufft-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.531469 mri-nufft-0.6.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.539469 mri-nufft-0.6.1/docs/_static/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/_static/logos/mri-nufft-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    42804 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/_static/logos/mri-nufft.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.531469 mri-nufft-0.6.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.539469 mri-nufft-0.6.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.539469 mri-nufft-0.6.1/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/misc/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/misc/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/misc/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/misc/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/misc/related.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/nufft.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/docs/trajectory_gradspec.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.543469 mri-nufft-0.6.1/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_2D_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_3D_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/examples/example_trajectory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 15:16:54.555469 mri-nufft-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.535469 mri-nufft-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.551469 mri-nufft-0.6.1/src/mri_nufft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-21 15:16:54.000000 mri-nufft-0.6.1/src/mri_nufft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-21 15:16:54.000000 mri-nufft-0.6.1/src/mri_nufft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 15:16:54.000000 mri-nufft-0.6.1/src/mri_nufft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-21 15:16:54.000000 mri-nufft-0.6.1/src/mri_nufft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-21 15:16:54.000000 mri-nufft-0.6.1/src/mri_nufft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.543469 mri-nufft-0.6.1/src/mrinufft/
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-21 15:16:54.000000 mri-nufft-0.6.1/src/mrinufft/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.543469 mri-nufft-0.6.1/src/mrinufft/density/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/density/geometry_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/density/nufft_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/density/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.543469 mri-nufft-0.6.1/src/mrinufft/io/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/io/cfl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/io/nsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.547469 mri-nufft-0.6.1/src/mrinufft/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.547469 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/_cupy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/bart.py
--rw-r--r--   0 runner    (1001) docker     (127)    28594 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/finufft.py
--rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/gpunufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/nfft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/nudft_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/pynufft_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/sigpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/tfnufft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.547469 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/css_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/off_resonnance.py
--rw-r--r--   0 runner    (1001) docker     (127)    27992 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/operators/stacked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.547469 mri-nufft-0.6.1/src/mrinufft/trajectories/
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/trajectories/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/trajectories/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/trajectories/trajectory2D.py
--rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/trajectories/trajectory3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/src/mrinufft/trajectories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.551469 mri-nufft-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/case_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:16:54.551469 mri-nufft-0.6.1/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/helpers/asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/helpers/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_ndft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-02-21 15:16:29.000000 mri-nufft-0.6.1/tests/test_stacked_gpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.367490 mri_nufft-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.343490 mri_nufft-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 13:26:44.367490 mri_nufft-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.347490 mri_nufft-0.6.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/_static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_static/logos/mri-nufft-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42804 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_static/logos/mri-nufft.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.347490 mri_nufft-0.6.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.351490 mri_nufft-0.6.2/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/misc/related.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/nufft.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/docs/trajectory_gradspec.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.355490 mri_nufft-0.6.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_2D_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25495 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_3D_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20986 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/examples/example_trajectory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:26:44.367490 mri_nufft-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.347490 mri_nufft-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/src/mri_nufft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mri_nufft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.355490 mri_nufft-0.6.2/src/mrinufft/
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 13:26:44.000000 mri_nufft-0.6.2/src/mrinufft/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.355490 mri_nufft-0.6.2/src/mrinufft/density/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/geometry_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/nufft_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/density/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/io/cfl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/io/nsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/_cupy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28594 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/finufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/gpunufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nudft_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/pynufft_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/sigpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/tfnufft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.359490 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/css_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/off_resonnance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27992 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/operators/stacked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/src/mrinufft/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17067 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22207 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17188 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/src/mrinufft/trajectories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/case_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/helpers/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/helpers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:26:44.363490 mri_nufft-0.6.2/tests/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_gpunufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/operators/test_stacked_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-15 13:26:24.000000 mri_nufft-0.6.2/tests/test_ndft.py
```

### Comparing `mri-nufft-0.6.1/.github/workflows/master-cd.yml` & `mri_nufft-0.6.2/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/.github/workflows/style.yml` & `mri_nufft-0.6.2/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/.github/workflows/tags-release.yml` & `mri_nufft-0.6.2/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/.github/workflows/test-ci.yml` & `mri_nufft-0.6.2/.github/workflows/test-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,15 @@
           make
           echo $PWD >> $GITHUB_PATH
 
       - name: Run Tests
         shell: bash
         run: |
           export COVERAGE_FILE=coverage_${{ matrix.backend }}
-          pytest --backend ${{ matrix.backend }} --ref ${{ env.ref_backend }} --cov --disable-pytest-warnings --cov-branch --cov-report=term
+          pytest -k='operators' --backend ${{ matrix.backend }} --ref ${{ env.ref_backend }} --cov --disable-pytest-warnings --cov-branch --cov-report=term
       - name: Upload coverage
         uses: actions/upload-artifact@v3
         with:
           name: coverage_data
           path: coverage_${{ matrix.backend}}
 
   test-gpu:
@@ -107,30 +107,39 @@
           source $RUNNER_WORKSPACE/venv/bin/activate
           pip install --upgrade pip wheel
           pip install -e mri-nufft[test]
           pip install cupy-cuda11x
           pip install torch --index-url https://download.pytorch.org/whl/cu118
           pip install finufft
 
+
       - name: Install backend
+        if: ${{ matrix.backend == 'gpunufft' || matrix.backend == 'cufinufft' }}
         shell: bash
         run: |
           source $RUNNER_WORKSPACE/venv/bin/activate
           export CUDA_BIN_PATH=/usr/local/cuda-11.8/
           export PATH=/usr/local/cuda-11.8/bin/${PATH:+:${PATH}}
           export LD_LIBRARY_PATH=/usr/local/cuda-11.8/lib/{LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}
           pip install ${{ matrix.backend }}
 
+      - name: Install pynfft
+        if: ${{ matrix.backend == 'pynfft' }}
+        shell: bash
+        run: |
+          source $RUNNER_WORKSPACE/venv/bin/activate
+          pip install pynfft2
+
       - name: Run Tests
         shell: bash
         run: |
           cd $RUNNER_WORKSPACE/mri-nufft
           source $RUNNER_WORKSPACE/venv/bin/activate
           export COVERAGE_FILE=coverage_${{ matrix.backend }}
-          python -m pytest --ref ${{ env.ref_backend }} --backend ${{ matrix.backend }} --disable-pytest-warnings --cov --cov-branch --cov-report=term
+          python -m pytest -k='operators' --ref ${{ env.ref_backend }} --backend ${{ matrix.backend }} --disable-pytest-warnings --cov --cov-branch --cov-report=term
 
       - name: Upload coverage
         if: success()
         uses: actions/upload-artifact@v3
         with:
           name: coverage_data
           path: coverage_${{ matrix.backend }}
@@ -164,15 +173,15 @@
           python -m pip install -e .[test,dev]
           python -m pip install finufft pooch brainweb-dl
 
       - name: Run examples
         shell: bash
         run: |
           export COVERAGE_FILE=coverage_plots
-          pytest examples --cov --cov-branch --cov-report=term
+          pytest examples tests -k="not operators" --cov --cov-branch --cov-report=term
 
       - name: Upload coverage
         if: success()
         uses: actions/upload-artifact@v3
         with:
           name: coverage_data
           path: coverage_plots
```

### Comparing `mri-nufft-0.6.1/LICENSE.txt` & `mri_nufft-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/PKG-INFO` & `mri_nufft-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mri-nufft
-Version: 0.6.1
+Version: 0.6.2
 Summary: MRI Non-Cartesian Fourier Operators with multiple computation backends.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `mri-nufft-0.6.1/README.rst` & `mri_nufft-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/Makefile` & `mri_nufft-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/_static/logos/mri-nufft-icon.png` & `mri_nufft-0.6.2/docs/_static/logos/mri-nufft-icon.png`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/_static/logos/mri-nufft.png` & `mri_nufft-0.6.2/docs/_static/logos/mri-nufft.png`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/_templates/autosummary/class.rst` & `mri_nufft-0.6.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/_templates/autosummary/module.rst` & `mri_nufft-0.6.2/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/conf.py` & `mri_nufft-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/getting_started.rst` & `mri_nufft-0.6.2/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/index.rst` & `mri_nufft-0.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/misc/code_of_conduct.rst` & `mri_nufft-0.6.2/docs/misc/code_of_conduct.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/misc/development.rst` & `mri_nufft-0.6.2/docs/misc/development.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/nufft.rst` & `mri_nufft-0.6.2/docs/nufft.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/docs/trajectory_gradspec.rst` & `mri_nufft-0.6.2/docs/trajectory_gradspec.rst`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/conftest.py` & `mri_nufft-0.6.2/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_2D_trajectories.py` & `mri_nufft-0.6.2/examples/example_2D_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_3D_trajectories.py` & `mri_nufft-0.6.2/examples/example_3D_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_density.py` & `mri_nufft-0.6.2/examples/example_density.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_display_config.py` & `mri_nufft-0.6.2/examples/example_display_config.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_readme.py` & `mri_nufft-0.6.2/examples/example_readme.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_stacked.py` & `mri_nufft-0.6.2/examples/example_stacked.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/examples/example_trajectory_tools.py` & `mri_nufft-0.6.2/examples/example_trajectory_tools.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/pyproject.toml` & `mri_nufft-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mri_nufft.egg-info/PKG-INFO` & `mri_nufft-0.6.2/src/mri_nufft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mri-nufft
-Version: 0.6.1
+Version: 0.6.2
 Summary: MRI Non-Cartesian Fourier Operators with multiple computation backends.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
```

### Comparing `mri-nufft-0.6.1/src/mri_nufft.egg-info/SOURCES.txt` & `mri_nufft-0.6.2/src/mri_nufft.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -72,18 +72,19 @@
 src/mrinufft/trajectories/display.py
 src/mrinufft/trajectories/tools.py
 src/mrinufft/trajectories/trajectory2D.py
 src/mrinufft/trajectories/trajectory3D.py
 src/mrinufft/trajectories/utils.py
 tests/case_trajectories.py
 tests/conftest.py
-tests/test_batch.py
-tests/test_bindings.py
 tests/test_density.py
-tests/test_interfaces.py
 tests/test_io.py
 tests/test_ndft.py
-tests/test_stacked.py
-tests/test_stacked_gpu.py
 tests/helpers/__init__.py
 tests/helpers/asserts.py
-tests/helpers/factories.py
+tests/helpers/factories.py
+tests/operators/test_batch.py
+tests/operators/test_bindings.py
+tests/operators/test_gpunufft.py
+tests/operators/test_interfaces.py
+tests/operators/test_stacked.py
+tests/operators/test_stacked_gpu.py
```

### Comparing `mri-nufft-0.6.1/src/mrinufft/__init__.py` & `mri_nufft-0.6.2/src/mrinufft/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/_utils.py` & `mri_nufft-0.6.2/src/mrinufft/_utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/density/geometry_based.py` & `mri_nufft-0.6.2/src/mrinufft/density/geometry_based.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/density/nufft_based.py` & `mri_nufft-0.6.2/src/mrinufft/density/nufft_based.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/density/utils.py` & `mri_nufft-0.6.2/src/mrinufft/density/utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/io/cfl.py` & `mri_nufft-0.6.2/src/mrinufft/io/cfl.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/io/nsp.py` & `mri_nufft-0.6.2/src/mrinufft/io/nsp.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/__init__.py` & `mri_nufft-0.6.2/src/mrinufft/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/base.py` & `mri_nufft-0.6.2/src/mrinufft/operators/base.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/_cupy_kernels.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/_cupy_kernels.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/bart.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/bart.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 from mrinufft._utils import proper_trajectory
 from mrinufft.operators.base import FourierOperatorCPU
 
 import numpy as np
 from mrinufft.io.cfl import traj2cfl, _writecfl, _readcfl
 
 # available if return code is 0
-BART_AVAILABLE = not subp.call(
-    ["which", "bart"], stdout=subp.DEVNULL, stderr=subp.DEVNULL
-)
+try:
+    BART_AVAILABLE = not subp.call(
+        ["which", "bart"], stdout=subp.DEVNULL, stderr=subp.DEVNULL
+    )
+except Exception:
+    BART_AVAILABLE = False
 
 
 class RawBartNUFFT:
     """Wrapper around BART NUFFT CLI."""
 
     def __init__(self, samples, shape, extra_op_args=None, extra_adj_op_args=None):
         self.samples = samples  # To normalize and send to file
```

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/cufinufft.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/finufft.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/finufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/gpunufft.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/gpunufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/nfft.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nfft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/nudft_numpy.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/nudft_numpy.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/pynufft_cpu.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/pynufft_cpu.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/sigpy.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/sigpy.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/tfnufft.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/tfnufft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/css_color.txt` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/css_color.txt`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/gpu_utils.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/interfaces/utils/utils.py` & `mri_nufft-0.6.2/src/mrinufft/operators/interfaces/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/off_resonnance.py` & `mri_nufft-0.6.2/src/mrinufft/operators/off_resonnance.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/operators/stacked.py` & `mri_nufft-0.6.2/src/mrinufft/operators/stacked.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/trajectories/__init__.py` & `mri_nufft-0.6.2/src/mrinufft/trajectories/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/trajectories/display.py` & `mri_nufft-0.6.2/src/mrinufft/trajectories/display.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/trajectories/tools.py` & `mri_nufft-0.6.2/src/mrinufft/trajectories/tools.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/trajectories/trajectory2D.py` & `mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory2D.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/trajectories/trajectory3D.py` & `mri_nufft-0.6.2/src/mrinufft/trajectories/trajectory3D.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/src/mrinufft/trajectories/utils.py` & `mri_nufft-0.6.2/src/mrinufft/trajectories/utils.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/case_trajectories.py` & `mri_nufft-0.6.2/tests/case_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/conftest.py` & `mri_nufft-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/helpers/__init__.py` & `mri_nufft-0.6.2/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/helpers/asserts.py` & `mri_nufft-0.6.2/tests/helpers/asserts.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/helpers/factories.py` & `mri_nufft-0.6.2/tests/helpers/factories.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/test_batch.py` & `mri_nufft-0.6.2/tests/operators/test_batch.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/test_bindings.py` & `mri_nufft-0.6.2/tests/operators/test_bindings.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/test_density.py` & `mri_nufft-0.6.2/tests/test_density.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,29 +57,7 @@
 def test_voronoi(traj, shape):
     """Test the voronoi method."""
     result = voronoi(traj)
     distance = radial_distance(traj, shape)
     result = result / np.mean(result)
     distance = distance / np.mean(distance)
     assert_correlate(result, distance, slope=1)
-
-
-@parametrize("osf", [1, 1.25, 2])
-@parametrize_with_cases(
-    "traj, shape",
-    cases=[
-        CasesTrajectories.case_nyquist_radial2D,
-        CasesTrajectories.case_nyquist_radial3D,
-    ],
-)
-@parametrize(backend=["gpunufft"])
-def test_pipe(backend, traj, shape, osf):
-    """Test the pipe method."""
-    distance = radial_distance(traj, shape)
-    result = pipe(traj, shape, osf=osf, num_iterations=10)
-    result = result / np.mean(result)
-    distance = distance / np.mean(distance)
-    if osf != 2:
-        # If OSF < 2, we dont perfectly estimate
-        assert_correlate(result, distance, slope=1, slope_err=None, r_value_err=0.2)
-    else:
-        assert_correlate(result, distance, slope=1, slope_err=0.1, r_value_err=0.1)
```

### Comparing `mri-nufft-0.6.1/tests/test_interfaces.py` & `mri_nufft-0.6.2/tests/operators/test_interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test the interfaces module."""
 
 import numpy as np
+import pytest
 from pytest_cases import parametrize_with_cases, parametrize, fixture
 from mrinufft import get_operator
 from case_trajectories import CasesTrajectories
 
 from helpers import (
     kspace_from_op,
     image_from_op,
@@ -39,14 +40,16 @@
     request,
     backend="pynfft",
     kspace_locs=None,
     shape=None,
     n_coils=1,
 ):
     """Generate an operator."""
+    if backend in ["pynfft", "sigpy"] and kspace_locs.shape[-1] == 3:
+        pytest.skip("3D for slow cpu is not tested")
     return get_operator(backend)(kspace_locs, shape, n_coils=n_coils, smaps=None)
 
 
 @fixture(scope="session", autouse=True)
 def ref_backend(request):
     """Get the reference backend from the CLI."""
     return request.config.getoption("ref")
```

### Comparing `mri-nufft-0.6.1/tests/test_io.py` & `mri_nufft-0.6.2/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/test_ndft.py` & `mri_nufft-0.6.2/tests/test_ndft.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/test_stacked.py` & `mri_nufft-0.6.2/tests/operators/test_stacked.py`

 * *Files identical despite different names*

### Comparing `mri-nufft-0.6.1/tests/test_stacked_gpu.py` & `mri_nufft-0.6.2/tests/operators/test_stacked_gpu.py`

 * *Files identical despite different names*

