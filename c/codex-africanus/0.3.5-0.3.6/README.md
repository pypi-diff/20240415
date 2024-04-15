# Comparing `tmp/codex-africanus-0.3.5.tar.gz` & `tmp/codex_africanus-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codex-africanus-0.3.5.tar", last modified: Tue Jan 30 15:45:48 2024, max compression
+gzip compressed data, was "codex_africanus-0.3.6.tar", last modified: Mon Apr 15 09:31:22 2024, max compression
```

## Comparing `codex-africanus-0.3.5.tar` & `codex_africanus-0.3.6.tar`

### file list

```diff
@@ -1,305 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.966735 codex-africanus-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-01-30 15:45:48.966735 codex-africanus-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.918734 codex-africanus-0.3.5/africanus/
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.922734 codex-africanus-0.3.5/africanus/averaging/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27819 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/bda_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/bda_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    28978 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/splines.py
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.922734 codex-africanus-0.3.5/africanus/averaging/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/test_bda_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/test_bda_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/test_splines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    16618 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/tests/test_time_and_channel_averaging.py
--rw-r--r--   0 runner    (1001) docker     (127)    30665 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/time_and_channel_avg.py
--rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/averaging/time_and_channel_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.922734 codex-africanus-0.3.5/africanus/calibration/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.922734 codex-africanus-0.3.5/africanus/calibration/phase_only/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/phase_only/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/phase_only/dask.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15462 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/phase_only/phase_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.922734 codex-africanus-0.3.5/africanus/calibration/phase_only/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/phase_only/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/phase_only/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/phase_only/tests/test_phase_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.922734 codex-africanus-0.3.5/africanus/calibration/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/calibration/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/compute_and_corrupt_vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/correct_vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/corrupt_vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/residual_vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/calibration/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10464 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/calibration/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/constants/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/coordinates/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/coordinates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/coordinates/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/coordinates/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/deconv/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/deconv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/deconv/hogbom/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/deconv/hogbom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/deconv/hogbom/clean.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/dft/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/dft/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/dft/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.926734 codex-africanus-0.3.5/africanus/experimental/rime/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.930734 codex-africanus-0.3.5/africanus/experimental/rime/fused/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/specification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.930734 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/cube_dde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/feed_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/phase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.930734 codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/test_rime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/test_structref_setter.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.930734 codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/parangle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.930734 codex-africanus-0.3.5/africanus/gps/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gps/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gps/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.934734 codex-africanus-0.3.5/africanus/gridding/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.934734 codex-africanus-0.3.5/africanus/gridding/nifty/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/nifty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16802 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/nifty/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.934734 codex-africanus-0.3.5/africanus/gridding/nifty/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/nifty/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/nifty/tests/test_nifty_gridder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.934734 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/degridder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/gridder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.934734 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/baseline_transform_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/convolution_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/phase_transform_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/stokes_conversion_policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.934734 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/tests/test_daskintrf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25516 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/tests/test_ppgridder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/gridding/wgridder/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/hessian.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/im2residim.py
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/im2vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/gridding/wgridder/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/tests/test_wgridder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/gridding/wgridder/vis2im.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/install/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/install/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/install/extras_require.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/linalg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27692 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/linalg/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/linalg/kronecker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/model/coherency/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/model/coherency/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/cuda/conversion.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/cuda/conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.938734 codex-africanus-0.3.5/africanus/model/coherency/cuda/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/cuda/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/cuda/tests/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/coherency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/coherency/tests/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/shape/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/gaussian_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/shapelets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/shape/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/tests/test_gaussian_shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    39008 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/shape/tests/test_shapelets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/spectral/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spectral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spectral/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spectral/spec_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/spectral/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spectral/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spectral/tests/test_spectral_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/spi/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spi/component_spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spi/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.942734 codex-africanus-0.3.5/africanus/model/spi/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spi/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18549 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/spi/examples/simple_spi_fitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.946734 codex-africanus-0.3.5/africanus/model/wsclean/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/file_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/spec_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.946734 codex-africanus-0.3.5/africanus/model/wsclean/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/tests/test_spectral_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/model/wsclean/tests/test_wsclean_model_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.946734 codex-africanus-0.3.5/africanus/rime/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.950734 codex-africanus-0.3.5/africanus/rime/cuda/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/beam.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/beam_freq_interp.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/feeds.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/macros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/phase.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/predict.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/test_shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.950734 codex-africanus-0.3.5/africanus/rime/cuda/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/cuda/tests/test_warp_transpose.cu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/dask.py
--rw-r--r--   0 runner    (1001) docker     (127)    21247 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/dask_predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.950734 codex-africanus-0.3.5/africanus/rime/examples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/examples/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/examples/predict_shapelet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/fast_beam_cubes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/feeds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.950734 codex-africanus-0.3.5/africanus/rime/jax/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/jax/phase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.950734 codex-africanus-0.3.5/africanus/rime/jax/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/jax/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/jax/tests/test_jax_phase_delay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/parangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/parangles_astropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/parangles_casa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/phase.py
--rw-r--r--   0 runner    (1001) docker     (127)    24615 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/predict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.954734 codex-africanus-0.3.5/africanus/rime/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/test_fast_beams.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/test_parangles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/test_rime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/test_wsclean_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)    71957 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/tests/test_zernike.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/wsclean_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/rime/zernike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.954734 codex-africanus-0.3.5/africanus/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/testing/beam_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.954734 codex-africanus-0.3.5/africanus/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/testing/tests/test_beam_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.958734 codex-africanus-0.3.5/africanus/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/appdirs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/beams.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/casa_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/cub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/cuda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/dask_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/jax_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/numba.py
--rw-r--r--   0 runner    (1001) docker     (127)    15953 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/nvcc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/trove.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/africanus/util/type_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.962734 codex-africanus-0.3.5/codex_africanus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/codex_africanus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/codex_africanus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/codex_africanus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/codex_africanus.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/codex_africanus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/codex_africanus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 15:45:48.962734 codex-africanus-0.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/averaging-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/calibration-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/cmdline-utils.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5722 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/coordinates-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/deconv-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/dft-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/experimental.rst
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/gps-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/gridding-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/linalg-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/model-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/rime-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/docs/util-api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-01-30 15:45:48.970734 codex-africanus-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-01-30 15:45:48.000000 codex-africanus-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.597040 codex_africanus-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-15 09:31:22.597040 codex_africanus-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.553040 codex_africanus-0.3.6/africanus/
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.553040 codex_africanus-0.3.6/africanus/averaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27819 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/bda_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20547 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/bda_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28978 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.553040 codex_africanus-0.3.6/africanus/averaging/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13469 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/test_bda_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/test_bda_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/test_splines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16618 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/tests/test_time_and_channel_averaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30665 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/time_and_channel_avg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/averaging/time_and_channel_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.553040 codex_africanus-0.3.6/africanus/calibration/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.553040 codex_africanus-0.3.6/africanus/calibration/phase_only/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/phase_only/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/phase_only/dask.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15462 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/phase_only/phase_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/calibration/phase_only/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/phase_only/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/phase_only/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/phase_only/tests/test_phase_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/calibration/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/calibration/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/compute_and_corrupt_vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/correct_vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/corrupt_vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/residual_vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/calibration/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10464 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/calibration/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/constants/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/coordinates/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/coordinates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/coordinates/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/coordinates/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.557040 codex_africanus-0.3.6/africanus/deconv/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/deconv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.561040 codex_africanus-0.3.6/africanus/deconv/hogbom/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/deconv/hogbom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/deconv/hogbom/clean.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.561040 codex_africanus-0.3.6/africanus/dft/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/dft/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/dft/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.561040 codex_africanus-0.3.6/africanus/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.561040 codex_africanus-0.3.6/africanus/experimental/rime/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.561040 codex_africanus-0.3.6/africanus/experimental/rime/fused/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7880 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29643 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15567 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/specification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.561040 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8329 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10825 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/cube_dde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/feed_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/phase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14600 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/test_rime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/test_structref_setter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3863 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/parangle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/gps/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gps/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gps/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/gridding/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/gridding/nifty/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/nifty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16802 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/nifty/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/gridding/nifty/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/nifty/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/nifty/tests/test_nifty_gridder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.565040 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12182 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9525 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/degridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/gridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/kernels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.569040 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/baseline_transform_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13152 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/convolution_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/phase_transform_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/stokes_conversion_policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.569040 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12466 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/tests/test_daskintrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25516 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/tests/test_ppgridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.569040 codex_africanus-0.3.6/africanus/gridding/wgridder/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/hessian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/im2residim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/im2vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.569040 codex_africanus-0.3.6/africanus/gridding/wgridder/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20326 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/tests/test_wgridder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/gridding/wgridder/vis2im.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.569040 codex_africanus-0.3.6/africanus/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/install/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/install/extras_require.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.569040 codex_africanus-0.3.6/africanus/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/linalg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27692 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/linalg/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/linalg/kronecker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/coherency/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7943 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/coherency/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/cuda/conversion.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     7354 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/cuda/conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/coherency/cuda/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/cuda/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/cuda/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/coherency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/coherency/tests/test_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/shape/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/gaussian_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/shapelets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/shape/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/tests/test_gaussian_shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39008 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/shape/tests/test_shapelets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.573040 codex_africanus-0.3.6/africanus/model/spectral/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spectral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spectral/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8503 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spectral/spec_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.577040 codex_africanus-0.3.6/africanus/model/spectral/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spectral/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spectral/tests/test_spectral_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.577040 codex_africanus-0.3.6/africanus/model/spi/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spi/component_spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spi/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.577040 codex_africanus-0.3.6/africanus/model/spi/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spi/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18549 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/spi/examples/simple_spi_fitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.577040 codex_africanus-0.3.6/africanus/model/wsclean/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/file_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/spec_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.577040 codex_africanus-0.3.6/africanus/model/wsclean/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/tests/test_spectral_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/model/wsclean/tests/test_wsclean_model_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.581040 codex_africanus-0.3.6/africanus/rime/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.581040 codex_africanus-0.3.6/africanus/rime/cuda/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/beam.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/beam_freq_interp.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/feeds.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/macros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/phase.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11117 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/predict.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6709 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10720 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/test_shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.581040 codex_africanus-0.3.6/africanus/rime/cuda/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/cuda/tests/test_warp_transpose.cu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/dask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21247 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/dask_predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.581040 codex_africanus-0.3.6/africanus/rime/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/examples/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17501 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/examples/predict_shapelet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/fast_beam_cubes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/feeds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.585040 codex_africanus-0.3.6/africanus/rime/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/jax/phase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.585040 codex_africanus-0.3.6/africanus/rime/jax/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/jax/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/jax/tests/test_jax_phase_delay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/parangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/parangles_astropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/parangles_casa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24615 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/predict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.585040 codex_africanus-0.3.6/africanus/rime/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/test_fast_beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/test_parangles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/test_rime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/test_wsclean_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71957 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/tests/test_zernike.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/wsclean_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/rime/zernike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.585040 codex_africanus-0.3.6/africanus/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/testing/beam_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.585040 codex_africanus-0.3.6/africanus/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/testing/tests/test_beam_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.589040 codex_africanus-0.3.6/africanus/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/appdirs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/casa_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/cub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/dask_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/jax_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15953 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/nvcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13169 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/trove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/africanus/util/type_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.593040 codex_africanus-0.3.6/codex_africanus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/codex_africanus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/codex_africanus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/codex_africanus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/codex_africanus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/codex_africanus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/codex_africanus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 09:31:22.593040 codex_africanus-0.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/averaging-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/calibration-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/cmdline-utils.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5722 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/coordinates-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/deconv-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/dft-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22392 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/experimental.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/gps-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/gridding-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/linalg-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/model-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/rime-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/docs/util-api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-15 09:31:22.597040 codex_africanus-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-15 09:31:22.000000 codex_africanus-0.3.6/setup.py
```

### Comparing `codex-africanus-0.3.5/CONTRIBUTING.rst` & `codex_africanus-0.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/HISTORY.rst` & `codex_africanus-0.3.6/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =======
 History
 =======
 
+0.3.6 (2024-04-15)
+------------------
+* Fix jax configuration (:pr:`301`)
+* Configure dependabot for github actions (:pr:`296`)
+* Cache numba kernels between CI runs (:pr:`294`)
+
 0.3.5 (2024-01-30)
 ------------------
 * Update setup.py metadata (:pr:`293`)
 * Address warnings (:pr:`292`)
 * Update github action versions (:pr:`291`)
 * Deprecate python 3.8 support (:pr:`290`)
 * Use pre-commit hooks for auto-linting (:pr:`290`)
```

### Comparing `codex-africanus-0.3.5/LICENSE` & `codex_africanus-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/PKG-INFO` & `codex_africanus-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codex-africanus
-Version: 0.3.5
+Version: 0.3.6
 Summary: Radio Astronomy Building Blocks
 Home-page: https://github.com/ska-sa/codex-africanus
 Author: Simon Perkins
 Author-email: sperkins@sarao.ac.za
 License: BSD-3-Clause
 Keywords: codex-africanus
 Classifier: Development Status :: 4 - Beta
```

### Comparing `codex-africanus-0.3.5/README.rst` & `codex_africanus-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/bda_avg.py` & `codex_africanus-0.3.6/africanus/averaging/bda_avg.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/bda_mapping.py` & `codex_africanus-0.3.6/africanus/averaging/bda_mapping.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/dask.py` & `codex_africanus-0.3.6/africanus/averaging/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/shared.py` & `codex_africanus-0.3.6/africanus/averaging/shared.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/splines.py` & `codex_africanus-0.3.6/africanus/averaging/splines.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/support.py` & `codex_africanus-0.3.6/africanus/averaging/support.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/tests/test_bda_averaging.py` & `codex_africanus-0.3.6/africanus/averaging/tests/test_bda_averaging.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/tests/test_bda_mapping.py` & `codex_africanus-0.3.6/africanus/averaging/tests/test_bda_mapping.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/tests/test_mapping.py` & `codex_africanus-0.3.6/africanus/averaging/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/tests/test_splines.py` & `codex_africanus-0.3.6/africanus/averaging/tests/test_splines.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/tests/test_support.py` & `codex_africanus-0.3.6/africanus/averaging/tests/test_support.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/tests/test_time_and_channel_averaging.py` & `codex_africanus-0.3.6/africanus/averaging/tests/test_time_and_channel_averaging.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/time_and_channel_avg.py` & `codex_africanus-0.3.6/africanus/averaging/time_and_channel_avg.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/averaging/time_and_channel_mapping.py` & `codex_africanus-0.3.6/africanus/averaging/time_and_channel_mapping.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/phase_only/dask.py` & `codex_africanus-0.3.6/africanus/calibration/phase_only/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/phase_only/phase_only.py` & `codex_africanus-0.3.6/africanus/calibration/phase_only/phase_only.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/phase_only/tests/conftest.py` & `codex_africanus-0.3.6/africanus/calibration/phase_only/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/phase_only/tests/test_phase_only.py` & `codex_africanus-0.3.6/africanus/calibration/phase_only/tests/test_phase_only.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/tests/conftest.py` & `codex_africanus-0.3.6/africanus/calibration/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/compute_and_corrupt_vis.py` & `codex_africanus-0.3.6/africanus/calibration/utils/compute_and_corrupt_vis.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/correct_vis.py` & `codex_africanus-0.3.6/africanus/calibration/utils/correct_vis.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/corrupt_vis.py` & `codex_africanus-0.3.6/africanus/calibration/utils/corrupt_vis.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/dask.py` & `codex_africanus-0.3.6/africanus/calibration/utils/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/residual_vis.py` & `codex_africanus-0.3.6/africanus/calibration/utils/residual_vis.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/tests/conftest.py` & `codex_africanus-0.3.6/africanus/calibration/utils/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/tests/test_utils.py` & `codex_africanus-0.3.6/africanus/calibration/utils/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/calibration/utils/utils.py` & `codex_africanus-0.3.6/africanus/calibration/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/conftest.py` & `codex_africanus-0.3.6/africanus/conftest.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/coordinates/coordinates.py` & `codex_africanus-0.3.6/africanus/coordinates/coordinates.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/coordinates/dask.py` & `codex_africanus-0.3.6/africanus/coordinates/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/deconv/hogbom/clean.py` & `codex_africanus-0.3.6/africanus/deconv/hogbom/clean.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/dft/dask.py` & `codex_africanus-0.3.6/africanus/dft/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/dft/kernels.py` & `codex_africanus-0.3.6/africanus/dft/kernels.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/arguments.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/arguments.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/core.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/core.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/dask.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/intrinsics.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/intrinsics.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/specification.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/specification.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/brightness.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/brightness.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/core.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/core.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/cube_dde.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/cube_dde.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/feed_rotation.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/feed_rotation.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/gaussian.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/gaussian.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/terms/phase.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/terms/phase.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/test_rime.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/test_rime.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/tests/test_structref_setter.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/tests/test_structref_setter.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/core.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/core.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/lm.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/lm.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/experimental/rime/fused/transformers/parangle.py` & `codex_africanus-0.3.6/africanus/experimental/rime/fused/transformers/parangle.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gps/kernels.py` & `codex_africanus-0.3.6/africanus/gps/kernels.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gps/utils.py` & `codex_africanus-0.3.6/africanus/gps/utils.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/nifty/dask.py` & `codex_africanus-0.3.6/africanus/gridding/nifty/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/nifty/tests/test_nifty_gridder.py` & `codex_africanus-0.3.6/africanus/gridding/nifty/tests/test_nifty_gridder.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/dask.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/degridder.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/degridder.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/gridder.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/gridder.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/kernels.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/kernels.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/baseline_transform_policies.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/baseline_transform_policies.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/convolution_policies.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/convolution_policies.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/phase_transform_policies.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/phase_transform_policies.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/policies/stokes_conversion_policies.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/policies/stokes_conversion_policies.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/tests/test_daskintrf.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/tests/test_daskintrf.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/perleypolyhedron/tests/test_ppgridder.py` & `codex_africanus-0.3.6/africanus/gridding/perleypolyhedron/tests/test_ppgridder.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/util.py` & `codex_africanus-0.3.6/africanus/gridding/util.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/wgridder/dask.py` & `codex_africanus-0.3.6/africanus/gridding/wgridder/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/wgridder/hessian.py` & `codex_africanus-0.3.6/africanus/gridding/wgridder/hessian.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/wgridder/im2residim.py` & `codex_africanus-0.3.6/africanus/gridding/wgridder/im2residim.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/wgridder/im2vis.py` & `codex_africanus-0.3.6/africanus/gridding/wgridder/im2vis.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/wgridder/tests/test_wgridder.py` & `codex_africanus-0.3.6/africanus/gridding/wgridder/tests/test_wgridder.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/gridding/wgridder/vis2im.py` & `codex_africanus-0.3.6/africanus/gridding/wgridder/vis2im.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/linalg/geometry.py` & `codex_africanus-0.3.6/africanus/linalg/geometry.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/linalg/kronecker_tools.py` & `codex_africanus-0.3.6/africanus/linalg/kronecker_tools.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/coherency/conversion.py` & `codex_africanus-0.3.6/africanus/model/coherency/conversion.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/coherency/cuda/conversion.cu.j2` & `codex_africanus-0.3.6/africanus/model/coherency/cuda/conversion.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/coherency/cuda/conversion.py` & `codex_africanus-0.3.6/africanus/model/coherency/cuda/conversion.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/coherency/cuda/tests/test_convert.py` & `codex_africanus-0.3.6/africanus/model/coherency/cuda/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/coherency/dask.py` & `codex_africanus-0.3.6/africanus/model/coherency/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/coherency/tests/test_convert.py` & `codex_africanus-0.3.6/africanus/model/coherency/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/shape/dask.py` & `codex_africanus-0.3.6/africanus/model/shape/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/shape/gaussian_shape.py` & `codex_africanus-0.3.6/africanus/model/shape/gaussian_shape.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/shape/shapelets.py` & `codex_africanus-0.3.6/africanus/model/shape/shapelets.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/shape/tests/test_gaussian_shape.py` & `codex_africanus-0.3.6/africanus/model/shape/tests/test_gaussian_shape.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/shape/tests/test_shapelets.py` & `codex_africanus-0.3.6/africanus/model/shape/tests/test_shapelets.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/spectral/dask.py` & `codex_africanus-0.3.6/africanus/model/spectral/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/spectral/spec_model.py` & `codex_africanus-0.3.6/africanus/model/spectral/spec_model.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/spectral/tests/test_spectral_model.py` & `codex_africanus-0.3.6/africanus/model/spectral/tests/test_spectral_model.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/spi/component_spi.py` & `codex_africanus-0.3.6/africanus/model/spi/component_spi.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/spi/dask.py` & `codex_africanus-0.3.6/africanus/model/spi/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/spi/examples/simple_spi_fitter.py` & `codex_africanus-0.3.6/africanus/model/spi/examples/simple_spi_fitter.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/wsclean/dask.py` & `codex_africanus-0.3.6/africanus/model/wsclean/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/wsclean/file_model.py` & `codex_africanus-0.3.6/africanus/model/wsclean/file_model.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/wsclean/spec_model.py` & `codex_africanus-0.3.6/africanus/model/wsclean/spec_model.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/wsclean/tests/conftest.py` & `codex_africanus-0.3.6/africanus/model/wsclean/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/wsclean/tests/test_spectral_model.py` & `codex_africanus-0.3.6/africanus/model/wsclean/tests/test_spectral_model.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/model/wsclean/tests/test_wsclean_model_file.py` & `codex_africanus-0.3.6/africanus/model/wsclean/tests/test_wsclean_model_file.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/beam.cu.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/beam.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/beam.py` & `codex_africanus-0.3.6/africanus/rime/cuda/beam.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/beam_freq_interp.cu.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/beam_freq_interp.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/feeds.cu.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/feeds.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/feeds.py` & `codex_africanus-0.3.6/africanus/rime/cuda/feeds.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/macros.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/macros.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/phase.cu.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/phase.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/phase.py` & `codex_africanus-0.3.6/africanus/rime/cuda/phase.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/predict.cu.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/predict.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/predict.py` & `codex_africanus-0.3.6/africanus/rime/cuda/predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/test_shuffle.py` & `codex_africanus-0.3.6/africanus/rime/cuda/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/cuda/tests/test_warp_transpose.cu.j2` & `codex_africanus-0.3.6/africanus/rime/cuda/tests/test_warp_transpose.cu.j2`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/dask.py` & `codex_africanus-0.3.6/africanus/rime/dask.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/dask_predict.py` & `codex_africanus-0.3.6/africanus/rime/dask_predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/examples/predict.py` & `codex_africanus-0.3.6/africanus/rime/examples/predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/examples/predict_shapelet.py` & `codex_africanus-0.3.6/africanus/rime/examples/predict_shapelet.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/fast_beam_cubes.py` & `codex_africanus-0.3.6/africanus/rime/fast_beam_cubes.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/feeds.py` & `codex_africanus-0.3.6/africanus/rime/feeds.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/jax/phase.py` & `codex_africanus-0.3.6/africanus/rime/jax/phase.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/jax/tests/test_jax_phase_delay.py` & `codex_africanus-0.3.6/africanus/rime/jax/tests/test_jax_phase_delay.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/parangles.py` & `codex_africanus-0.3.6/africanus/rime/parangles.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/parangles_astropy.py` & `codex_africanus-0.3.6/africanus/rime/parangles_astropy.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/parangles_casa.py` & `codex_africanus-0.3.6/africanus/rime/parangles_casa.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/phase.py` & `codex_africanus-0.3.6/africanus/rime/phase.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/predict.py` & `codex_africanus-0.3.6/africanus/rime/predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/conftest.py` & `codex_africanus-0.3.6/africanus/rime/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/test_fast_beams.py` & `codex_africanus-0.3.6/africanus/rime/tests/test_fast_beams.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/test_parangles.py` & `codex_africanus-0.3.6/africanus/rime/tests/test_parangles.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/test_predict.py` & `codex_africanus-0.3.6/africanus/rime/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/test_rime.py` & `codex_africanus-0.3.6/africanus/rime/tests/test_rime.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/test_wsclean_predict.py` & `codex_africanus-0.3.6/africanus/rime/tests/test_wsclean_predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/tests/test_zernike.py` & `codex_africanus-0.3.6/africanus/rime/tests/test_zernike.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/transform.py` & `codex_africanus-0.3.6/africanus/rime/transform.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/wsclean_predict.py` & `codex_africanus-0.3.6/africanus/rime/wsclean_predict.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/rime/zernike.py` & `codex_africanus-0.3.6/africanus/rime/zernike.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/testing/beam_factory.py` & `codex_africanus-0.3.6/africanus/testing/beam_factory.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/testing/tests/test_beam_factory.py` & `codex_africanus-0.3.6/africanus/testing/tests/test_beam_factory.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/beams.py` & `codex_africanus-0.3.6/africanus/util/beams.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/casa_types.py` & `codex_africanus-0.3.6/africanus/util/casa_types.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/cmdline.py` & `codex_africanus-0.3.6/africanus/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/code.py` & `codex_africanus-0.3.6/africanus/util/code.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/cub.py` & `codex_africanus-0.3.6/africanus/util/cub.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/cuda.py` & `codex_africanus-0.3.6/africanus/util/cuda.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/dask_util.py` & `codex_africanus-0.3.6/africanus/util/dask_util.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/docs.py` & `codex_africanus-0.3.6/africanus/util/docs.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/jinja2.py` & `codex_africanus-0.3.6/africanus/util/jinja2.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/numba.py` & `codex_africanus-0.3.6/africanus/util/numba.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/nvcc.py` & `codex_africanus-0.3.6/africanus/util/nvcc.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/patterns.py` & `codex_africanus-0.3.6/africanus/util/patterns.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/requirements.py` & `codex_africanus-0.3.6/africanus/util/requirements.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/shapes.py` & `codex_africanus-0.3.6/africanus/util/shapes.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/testing.py` & `codex_africanus-0.3.6/africanus/util/testing.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/trove.py` & `codex_africanus-0.3.6/africanus/util/trove.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/africanus/util/type_inference.py` & `codex_africanus-0.3.6/africanus/util/type_inference.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/codex_africanus.egg-info/PKG-INFO` & `codex_africanus-0.3.6/codex_africanus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codex-africanus
-Version: 0.3.5
+Version: 0.3.6
 Summary: Radio Astronomy Building Blocks
 Home-page: https://github.com/ska-sa/codex-africanus
 Author: Simon Perkins
 Author-email: sperkins@sarao.ac.za
 License: BSD-3-Clause
 Keywords: codex-africanus
 Classifier: Development Status :: 4 - Beta
```

### Comparing `codex-africanus-0.3.5/codex_africanus.egg-info/SOURCES.txt` & `codex_africanus-0.3.6/codex_africanus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/codex_africanus.egg-info/requires.txt` & `codex_africanus-0.3.6/codex_africanus.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/Makefile` & `codex_africanus-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/averaging-api.rst` & `codex_africanus-0.3.6/docs/averaging-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/calibration-api.rst` & `codex_africanus-0.3.6/docs/calibration-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/conf.py` & `codex_africanus-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/coordinates-api.rst` & `codex_africanus-0.3.6/docs/coordinates-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/dft-api.rst` & `codex_africanus-0.3.6/docs/dft-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/experimental.rst` & `codex_africanus-0.3.6/docs/experimental.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/gridding-api.rst` & `codex_africanus-0.3.6/docs/gridding-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/installation.rst` & `codex_africanus-0.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/linalg-api.rst` & `codex_africanus-0.3.6/docs/linalg-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/make.bat` & `codex_africanus-0.3.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/model-api.rst` & `codex_africanus-0.3.6/docs/model-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/rime-api.rst` & `codex_africanus-0.3.6/docs/rime-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/docs/util-api.rst` & `codex_africanus-0.3.6/docs/util-api.rst`

 * *Files identical despite different names*

### Comparing `codex-africanus-0.3.5/setup.cfg` & `codex_africanus-0.3.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.5
+current_version = 0.3.6
 commit = True
 tag = True
 tag_name = {new_version}
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `codex-africanus-0.3.5/setup.py` & `codex_africanus-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,10 +86,10 @@
     name="codex-africanus",
     packages=find_packages(),
     python_requires=">=3.9",
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/ska-sa/codex-africanus",
-    version="0.3.5",
+    version="0.3.6",
     zip_safe=False,
 )
```

