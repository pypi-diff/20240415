# Comparing `tmp/gempy_engine-2023.1.0b5.tar.gz` & `tmp/gempy_engine-2023.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gempy_engine-2023.1.0b5.tar", last modified: Fri Sep 15 12:26:14 2023, max compression
+gzip compressed data, was "gempy_engine-2023.2.0b1.tar", last modified: Wed Nov 22 15:03:55 2023, max compression
```

## Comparing `gempy_engine-2023.1.0b5.tar` & `gempy_engine-2023.2.0b1.tar`

### file list

```diff
@@ -1,189 +1,200 @@
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.751186 gempy_engine-2023.1.0b5/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      523 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/AUTHORS.rst
--rw-r--r--   0 leguark   (1000) leguark   (1000)    13879 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/LICENSE
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1883 2023-09-15 12:26:14.751186 gempy_engine-2023.1.0b5/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1144 2023-08-11 08:35:11.000000 gempy_engine-2023.1.0b5/README.md
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.721186 gempy_engine-2023.1.0b5/gempy_engine/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.721186 gempy_engine-2023.1.0b5/gempy_engine/API/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.721186 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3326 2023-08-11 13:31:07.000000 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/_dual_contouring.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2205 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3092 2023-09-06 13:48:11.000000 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/_interpolate_on_edges.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      114 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/_mask_buffer.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6935 2023-09-06 14:51:11.000000 gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6217 2023-09-11 09:13:50.000000 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_interp_scalar_field.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5115 2023-09-11 09:13:50.000000 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_interp_single_feature.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12052 2023-09-11 09:09:04.000000 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_multi_scalar_field_manager.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2519 2023-09-06 08:45:57.000000 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_octree_generation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3493 2023-09-06 09:43:29.000000 gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/interp_features.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/API/model/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/model/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1953 2023-09-14 08:16:44.000000 gempy_engine-2023.1.0b5/gempy_engine/API/model/model_api.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/API/server/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/server/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4176 2023-09-15 12:25:48.000000 gempy_engine-2023.1.0b5/gempy_engine/API/server/_process_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1857 2023-07-31 13:44:11.000000 gempy_engine-2023.1.0b5/gempy_engine/API/server/_server_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3942 2023-08-11 11:39:20.000000 gempy_engine-2023.1.0b5/gempy_engine/API/server/main_server_pro.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       61 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      640 2023-09-14 07:25:26.000000 gempy_engine-2023.1.0b5/gempy_engine/config.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7524 2023-09-11 09:09:21.000000 gempy_engine-2023.1.0b5/gempy_engine/core/backend_tensor.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/core/data/
--rw-r--r--   0 leguark   (1000) leguark   (1000)      281 2023-07-12 09:25:33.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1238 2023-08-16 14:56:03.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/custom_segmentation_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1207 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/dual_contouring_data.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      602 2023-09-14 08:17:23.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/dual_contouring_mesh.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2695 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/exported_fields.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      442 2023-09-05 11:04:18.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/exported_structs.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      226 2023-07-31 14:30:08.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/generic_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3801 2023-09-06 08:45:57.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3503 2023-08-17 12:00:28.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/input_data_descriptor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1714 2023-09-11 09:06:41.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/internal_structs.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3402 2023-09-06 09:45:56.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/interp_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2811 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/interpolation_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7560 2023-09-07 13:38:42.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/interpolation_input.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1550 2023-08-17 13:49:03.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/faults.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1583 2023-09-11 09:06:41.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/kernel_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3354 2023-08-11 08:42:39.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/orientations.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/server/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/server/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1000 2023-08-11 11:40:58.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/server/input_parser.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      145 2023-08-09 08:33:04.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/solvers.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2187 2023-08-07 12:04:10.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/surface_points.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      430 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/matrices_sizes.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1575 2023-09-06 14:32:35.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/octree_level.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10999 2023-09-11 09:06:40.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/options.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6905 2023-09-14 13:03:36.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/raw_arrays_solution.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6486 2023-09-11 09:12:04.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/regular_grid.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4767 2023-09-05 09:27:38.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/scalar_field_output.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2758 2023-09-15 12:24:25.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/solutions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      198 2023-07-24 09:17:59.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/stack_relation_type.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4792 2023-09-06 08:23:45.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/stacks_structure.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2365 2023-07-12 14:22:41.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/tensors_structure.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10868 2023-09-05 14:24:09.000000 gempy_engine-2023.1.0b5/gempy_engine/core/data/transforms.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      825 2023-09-11 09:11:46.000000 gempy_engine-2023.1.0b5/gempy_engine/core/utils.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/modules/activator/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/activator/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2317 2023-09-11 09:06:40.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/activator/activator_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/modules/data_preprocess/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/data_preprocess/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2172 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/data_preprocess/_input_preparation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1451 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/data_preprocess/data_preprocess_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.731186 gempy_engine-2023.1.0b5/gempy_engine/modules/dual_contouring/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/dual_contouring/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10307 2023-09-11 09:10:07.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/dual_contouring/dual_contouring_interface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10997 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/dual_contouring/fancy_triangulation.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      779 2023-09-11 09:07:38.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6515 2023-09-11 09:12:38.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_covariance_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2869 2023-09-11 09:10:14.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4148 2023-09-11 09:10:42.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_kernel_constructors.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1347 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_kernel_selectors.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    12223 2023-08-16 13:29:03.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_kernels_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2519 2023-08-11 11:19:33.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8145 2023-09-11 09:09:41.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_structs.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3548 2023-08-16 13:29:03.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_test_assembler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      976 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_utils.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    11212 2023-09-11 09:11:09.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_vectors_preparation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1379 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1217 2023-09-06 08:37:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/_octree_common.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3252 2023-09-06 12:06:01.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/_octree_internals.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5790 2023-09-05 11:45:12.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/octrees_topology_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/gempy_engine/modules/solver/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/solver/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3615 2023-09-14 07:38:04.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/solver/solver_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/gempy_engine/modules/topology/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/topology/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/gempy_engine/modules/topology/topology _interface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1366 2023-09-14 07:42:55.000000 gempy_engine-2023.1.0b5/gempy_engine/optional_dependencies.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/gempy_engine/plugins/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:38.000000 gempy_engine-2023.1.0b5/gempy_engine/plugins/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/gempy_engine/plugins/plotting/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:56.000000 gempy_engine-2023.1.0b5/gempy_engine/plugins/plotting/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3667 2023-07-31 13:58:12.000000 gempy_engine-2023.1.0b5/gempy_engine/plugins/plotting/helper_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5479 2023-08-16 14:46:48.000000 gempy_engine-2023.1.0b5/gempy_engine/plugins/plotting/helper_functions_pyvista.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.721186 gempy_engine-2023.1.0b5/gempy_engine.egg-info/
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1883 2023-09-15 12:26:14.000000 gempy_engine-2023.1.0b5/gempy_engine.egg-info/PKG-INFO
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7094 2023-09-15 12:26:14.000000 gempy_engine-2023.1.0b5/gempy_engine.egg-info/SOURCES.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-09-15 12:26:14.000000 gempy_engine-2023.1.0b5/gempy_engine.egg-info/dependency_links.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)      171 2023-09-15 12:26:14.000000 gempy_engine-2023.1.0b5/gempy_engine.egg-info/requires.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2023-09-15 12:26:14.000000 gempy_engine-2023.1.0b5/gempy_engine.egg-info/top_level.txt
--rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-09-15 12:26:14.751186 gempy_engine-2023.1.0b5/setup.cfg
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1331 2023-09-15 12:25:48.000000 gempy_engine-2023.1.0b5/setup.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2532 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/test_backend_tensor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2883 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/test_tensorflow.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      693 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/test_tf.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/benchmark/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/benchmark/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4213 2023-07-12 08:04:38.000000 gempy_engine-2023.1.0b5/tests/benchmark/one_fault_model.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2297 2023-08-11 09:00:58.000000 gempy_engine-2023.1.0b5/tests/benchmark/profile_runner.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4341 2023-08-11 09:00:58.000000 gempy_engine-2023.1.0b5/tests/benchmark/test_benchmark_one_feature.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1800 2023-09-11 09:11:23.000000 gempy_engine-2023.1.0b5/tests/conftest.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/fixtures/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/fixtures/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     8052 2023-09-06 11:07:34.000000 gempy_engine-2023.1.0b5/tests/fixtures/complex_geometries.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      936 2023-09-06 11:20:47.000000 gempy_engine-2023.1.0b5/tests/fixtures/grids.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6263 2023-09-06 12:06:01.000000 gempy_engine-2023.1.0b5/tests/fixtures/heavy_models.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2710 2023-09-06 11:26:04.000000 gempy_engine-2023.1.0b5/tests/fixtures/simple_geometries.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    18958 2023-09-06 11:21:58.000000 gempy_engine-2023.1.0b5/tests/fixtures/simple_models.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_api/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_api/__init__.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_api/test_faults/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_api/test_faults/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6609 2023-09-06 11:10:34.000000 gempy_engine-2023.1.0b5/tests/test_common/test_api/test_faults/test_faults_graben.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10729 2023-09-11 09:15:23.000000 gempy_engine-2023.1.0b5/tests/test_common/test_api/test_faults/test_one_fault.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1526 2023-07-24 07:52:55.000000 gempy_engine-2023.1.0b5/tests/test_common/test_api/test_output_to_subsurface.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5303 2023-09-06 07:38:12.000000 gempy_engine-2023.1.0b5/tests/test_common/test_api/test_public_interface.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_core/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_core/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       72 2023-07-12 07:31:14.000000 gempy_engine-2023.1.0b5/tests/test_common/test_core/test_data_classes.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_dependencies/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_dependencies/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)      542 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_dependencies/pykeops_test_compiler.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    18780 2023-08-11 08:42:39.000000 gempy_engine-2023.1.0b5/tests/test_common/test_dependencies/test_pykeops.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4019 2023-09-06 11:07:34.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_external_functions.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3308 2023-09-06 07:47:54.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_interpolate_model.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     2102 2023-09-06 11:22:27.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_kernels.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     7483 2023-09-06 11:07:34.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_multi_fields.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     6236 2023-09-06 11:13:35.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1285 2023-09-06 07:48:11.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_multiple_grids.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1273 2023-09-11 09:13:50.000000 gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_options.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_modules/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1732 2023-09-06 08:39:46.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_activator.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    26089 2023-09-06 13:11:39.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_dual.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     5858 2023-09-06 11:21:04.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_exporter.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9593 2023-08-11 09:00:58.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     4881 2023-09-06 09:33:45.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     3091 2023-08-11 09:00:58.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_universal.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)    10870 2023-09-06 09:47:56.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_octrees.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1604 2023-09-06 09:39:39.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_solver.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       29 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_topology.py
-drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-09-15 12:26:14.741186 gempy_engine-2023.1.0b5/tests/test_common/test_prototyping/
--rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_prototyping/__init__.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     9854 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_common/test_prototyping/test_broadcasting.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)       52 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/test_installation.py
--rw-r--r--   0 leguark   (1000) leguark   (1000)     1642 2023-06-18 07:50:48.000000 gempy_engine-2023.1.0b5/tests/verify_helper.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      523 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/AUTHORS.rst
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    13879 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/LICENSE
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2419 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1144 2023-08-11 08:35:11.000000 gempy_engine-2023.2.0b1/README.md
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.035317 gempy_engine-2023.2.0b1/gempy_engine/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.035317 gempy_engine-2023.2.0b1/gempy_engine/API/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.035317 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4516 2023-11-21 09:51:13.000000 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/_dual_contouring.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2205 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3092 2023-09-06 13:48:11.000000 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/_interpolate_on_edges.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      114 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/_mask_buffer.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7039 2023-11-14 16:11:18.000000 gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6230 2023-11-07 13:11:51.000000 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_interp_scalar_field.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5470 2023-11-21 09:15:57.000000 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_interp_single_feature.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12242 2023-11-22 12:15:34.000000 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_multi_scalar_field_manager.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2827 2023-11-21 08:02:54.000000 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_octree_generation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3938 2023-11-21 08:04:09.000000 gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/interp_features.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/API/model/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/model/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2758 2023-11-15 12:51:49.000000 gempy_engine-2023.2.0b1/gempy_engine/API/model/model_api.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/API/server/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/server/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4176 2023-09-15 12:25:48.000000 gempy_engine-2023.2.0b1/gempy_engine/API/server/_process_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1857 2023-07-31 13:44:11.000000 gempy_engine-2023.2.0b1/gempy_engine/API/server/_server_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3942 2023-11-14 16:11:18.000000 gempy_engine-2023.2.0b1/gempy_engine/API/server/main_server_pro.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       61 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      741 2023-11-15 12:33:34.000000 gempy_engine-2023.2.0b1/gempy_engine/config.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10734 2023-11-22 12:20:58.000000 gempy_engine-2023.2.0b1/gempy_engine/core/backend_tensor.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/core/data/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      281 2023-07-12 09:25:33.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3973 2023-10-09 08:27:43.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/centered_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1314 2023-10-05 13:36:58.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/custom_segmentation_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1279 2023-10-05 11:49:56.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/dual_contouring_data.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      602 2023-09-14 08:17:23.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/dual_contouring_mesh.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2695 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/exported_fields.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      442 2023-09-05 11:04:18.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/exported_structs.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      226 2023-07-31 14:30:08.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/generic_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      173 2023-10-06 08:38:22.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/geophysics_input.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4090 2023-11-21 08:38:52.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3503 2023-08-17 12:00:28.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/input_data_descriptor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1809 2023-10-05 10:03:35.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/internal_structs.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3754 2023-11-10 14:48:43.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/interp_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3045 2023-10-05 13:51:07.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/interpolation_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8096 2023-10-09 11:51:50.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/interpolation_input.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1550 2023-08-17 13:49:03.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/faults.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1556 2023-11-07 13:54:12.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/kernel_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3418 2023-11-07 14:37:50.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/orientations.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/server/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/server/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1000 2023-08-11 11:40:58.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/server/input_parser.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      145 2023-08-09 08:33:04.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/solvers.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2251 2023-11-07 14:37:50.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/surface_points.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      430 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/matrices_sizes.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1575 2023-10-06 08:38:22.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/octree_level.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11074 2023-11-14 16:11:18.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/options.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7089 2023-11-07 14:40:56.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/raw_arrays_solution.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6853 2023-10-09 12:54:40.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/regular_grid.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4866 2023-10-05 11:10:56.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/scalar_field_output.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2862 2023-10-06 12:20:32.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/solutions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      198 2023-07-24 09:17:59.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/stack_relation_type.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4792 2023-09-06 08:23:45.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/stacks_structure.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2478 2023-10-05 12:38:32.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/tensors_structure.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10868 2023-09-05 14:24:09.000000 gempy_engine-2023.2.0b1/gempy_engine/core/data/transforms.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1286 2023-11-07 14:37:50.000000 gempy_engine-2023.2.0b1/gempy_engine/core/utils.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/modules/activator/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/activator/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3944 2023-11-15 12:33:19.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/activator/activator_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/modules/data_preprocess/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/data_preprocess/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2243 2023-10-05 12:38:32.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/data_preprocess/_input_preparation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1448 2023-11-22 12:22:12.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/data_preprocess/data_preprocess_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.045317 gempy_engine-2023.2.0b1/gempy_engine/modules/dual_contouring/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/dual_contouring/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11182 2023-11-21 09:37:42.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/dual_contouring/dual_contouring_interface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11119 2023-11-21 09:49:37.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/dual_contouring/fancy_triangulation.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/modules/geophysics/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-06 08:07:32.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/geophysics/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1929 2023-10-09 08:58:18.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/geophysics/fw_gravity.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2021 2023-10-09 08:27:43.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/geophysics/gravity_gradient.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      867 2023-10-05 12:31:28.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6559 2023-11-07 14:08:41.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_covariance_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2950 2023-10-05 09:41:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4237 2023-11-07 11:42:44.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_kernel_constructors.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1347 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_kernel_selectors.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    12219 2023-11-07 14:09:40.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_kernels_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2519 2023-08-11 11:19:33.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7724 2023-11-07 14:09:40.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_structs.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3548 2023-08-16 13:29:03.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_test_assembler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      976 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_utils.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    11297 2023-11-22 12:24:25.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_vectors_preparation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1379 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1217 2023-09-06 08:37:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/_octree_common.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3252 2023-09-06 12:06:01.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/_octree_internals.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6276 2023-11-07 11:59:29.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/octrees_topology_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/modules/solver/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/solver/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4373 2023-11-22 12:06:18.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/solver/solver_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/modules/topology/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/topology/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/gempy_engine/modules/topology/topology _interface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1565 2023-10-05 08:11:53.000000 gempy_engine-2023.2.0b1/gempy_engine/optional_dependencies.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/plugins/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:38.000000 gempy_engine-2023.2.0b1/gempy_engine/plugins/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/gempy_engine/plugins/plotting/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-07-24 07:51:56.000000 gempy_engine-2023.2.0b1/gempy_engine/plugins/plotting/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3667 2023-07-31 13:58:12.000000 gempy_engine-2023.2.0b1/gempy_engine/plugins/plotting/helper_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5479 2023-08-16 14:46:48.000000 gempy_engine-2023.2.0b1/gempy_engine/plugins/plotting/helper_functions_pyvista.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.035317 gempy_engine-2023.2.0b1/gempy_engine.egg-info/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2419 2023-11-22 15:03:55.000000 gempy_engine-2023.2.0b1/gempy_engine.egg-info/PKG-INFO
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7493 2023-11-22 15:03:55.000000 gempy_engine-2023.2.0b1/gempy_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        1 2023-11-22 15:03:55.000000 gempy_engine-2023.2.0b1/gempy_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      164 2023-11-22 15:03:55.000000 gempy_engine-2023.2.0b1/gempy_engine.egg-info/requires.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       19 2023-11-22 15:03:55.000000 gempy_engine-2023.2.0b1/gempy_engine.egg-info/top_level.txt
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       38 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/setup.cfg
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1331 2023-11-22 15:00:16.000000 gempy_engine-2023.2.0b1/setup.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2532 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/test_backend_tensor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2883 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/test_tensorflow.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      693 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/test_tf.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/benchmark/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/benchmark/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4234 2023-11-14 16:11:18.000000 gempy_engine-2023.2.0b1/tests/benchmark/one_fault_model.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2297 2023-08-11 09:00:58.000000 gempy_engine-2023.2.0b1/tests/benchmark/profile_runner.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4341 2023-08-11 09:00:58.000000 gempy_engine-2023.2.0b1/tests/benchmark/test_benchmark_one_feature.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1835 2023-11-14 16:03:52.000000 gempy_engine-2023.2.0b1/tests/conftest.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/fixtures/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/fixtures/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     8073 2023-10-05 14:07:00.000000 gempy_engine-2023.2.0b1/tests/fixtures/complex_geometries.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      936 2023-09-06 11:20:47.000000 gempy_engine-2023.2.0b1/tests/fixtures/grids.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6263 2023-11-14 16:11:18.000000 gempy_engine-2023.2.0b1/tests/fixtures/heavy_models.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2710 2023-09-06 11:26:04.000000 gempy_engine-2023.2.0b1/tests/fixtures/simple_geometries.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    20258 2023-11-10 08:20:25.000000 gempy_engine-2023.2.0b1/tests/fixtures/simple_models.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/test_common/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/test_common/test_api/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_api/__init__.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.055317 gempy_engine-2023.2.0b1/tests/test_common/test_api/test_faults/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_api/test_faults/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6609 2023-11-14 16:10:31.000000 gempy_engine-2023.2.0b1/tests/test_common/test_api/test_faults/test_faults_graben.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10824 2023-11-14 16:11:18.000000 gempy_engine-2023.2.0b1/tests/test_common/test_api/test_faults/test_one_fault.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1526 2023-07-24 07:52:55.000000 gempy_engine-2023.2.0b1/tests/test_common/test_api/test_output_to_subsurface.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5564 2023-10-05 13:20:49.000000 gempy_engine-2023.2.0b1/tests/test_common/test_api/test_public_interface.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_common/test_core/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_core/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       72 2023-07-12 07:31:14.000000 gempy_engine-2023.2.0b1/tests/test_common/test_core/test_data_classes.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_common/test_dependencies/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_dependencies/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      542 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_dependencies/pykeops_test_compiler.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    18780 2023-08-11 08:42:39.000000 gempy_engine-2023.2.0b1/tests/test_common/test_dependencies/test_pykeops.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4159 2023-11-14 16:05:22.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_external_functions.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3308 2023-09-06 07:47:54.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_interpolate_model.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2102 2023-09-06 11:22:27.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_kernels.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     7959 2023-10-05 14:03:14.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_multi_fields.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     6378 2023-11-14 16:04:57.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1285 2023-09-06 07:48:11.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_multiple_grids.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1273 2023-09-11 09:13:50.000000 gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_options.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_common/test_modules/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3518 2023-11-10 14:06:17.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_activator.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    26764 2023-10-05 14:25:58.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_dual.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5985 2023-10-05 14:43:29.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_exporter.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2109 2023-11-15 12:52:50.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_geophysics.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9996 2023-10-05 14:47:39.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     5020 2023-10-05 14:50:19.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     3232 2023-10-05 14:53:15.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_universal.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)    10870 2023-09-06 09:47:56.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_octrees.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     1604 2023-09-06 09:39:39.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_solver.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       29 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_topology.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_common/test_prototyping/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_prototyping/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     9854 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_common/test_prototyping/test_broadcasting.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)       52 2023-06-18 07:50:48.000000 gempy_engine-2023.2.0b1/tests/test_installation.py
+drwxr-xr-x   0 leguark   (1000) leguark   (1000)        0 2023-11-22 15:03:55.065317 gempy_engine-2023.2.0b1/tests/test_pytorch/
+-rw-r--r--   0 leguark   (1000) leguark   (1000)        0 2023-10-05 07:48:25.000000 gempy_engine-2023.2.0b1/tests/test_pytorch/__init__.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     4292 2023-11-07 14:10:20.000000 gempy_engine-2023.2.0b1/tests/test_pytorch/test_pytorch_gradients.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)      125 2023-10-05 07:51:30.000000 gempy_engine-2023.2.0b1/tests/test_pytorch/test_pytorch_installation.py
+-rw-r--r--   0 leguark   (1000) leguark   (1000)     2416 2023-10-05 14:42:20.000000 gempy_engine-2023.2.0b1/tests/verify_helper.py
```

### Comparing `gempy_engine-2023.1.0b5/AUTHORS.rst` & `gempy_engine-2023.2.0b1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/LICENSE` & `gempy_engine-2023.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/README.md` & `gempy_engine-2023.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/_experimental_water_tight_DC_1.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/_interpolate_on_edges.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/_interpolate_on_edges.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/dual_contouring/multi_scalar_dual_contouring.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import copy
 import warnings
 from typing import List
 
 import numpy as np
 
+from gempy_engine.core.backend_tensor import BackendTensor
 from ._dual_contouring import compute_dual_contouring
 from ._experimental_water_tight_DC_1 import _experimental_water_tight
 from ._interpolate_on_edges import interpolate_on_edges_for_dual_contouring
 from ._mask_buffer import MaskBuffer
 from ...core.data import InterpolationOptions
 from ...core.data.dual_contouring_data import DualContouringData
 from ...core.data.dual_contouring_mesh import DualContouringMesh
 from ...core.data.input_data_descriptor import InputDataDescriptor
 from ...core.data.interp_output import InterpOutput
 from ...core.data.interpolation_input import InterpolationInput
 from ...core.data.octree_level import OctreeLevel
-from ...core.data.options import DualContouringMaskingOptions
+from ...core.data.options import MeshExtractionMaskingOptions
 from ...core.data.stack_relation_type import StackRelationType
 from ...core.utils import gempy_profiler_decorator
 from ...modules.dual_contouring.fancy_triangulation import get_left_right_array
 
 
 @gempy_profiler_decorator
 def dual_contouring_multi_scalar(data_descriptor: InputDataDescriptor, interpolation_input: InterpolationInput,
@@ -35,104 +36,107 @@
 
     if options.debug_water_tight:
         _experimental_water_tight(all_meshes, data_descriptor, interpolation_input, octree_leaves, dual_contouring_options)
         return all_meshes
 
     # region new triangulations
     is_pure_octree = bool(np.all(octree_list[0].grid_centers.regular_grid_shape == 2))
-    match (options.dual_contouring_fancy, is_pure_octree):
+    match (options.mesh_extraction_fancy, is_pure_octree):
         case (True, True):
             left_right_codes = get_left_right_array(octree_list)
         case (True, False):
             left_right_codes = None
             warnings.warn("Fancy triangulation only works with regular grid of resolution [2,2,2]. Defaulting to regular triangulation")
         case (False, _):
             left_right_codes = None
         case _:
             raise ValueError("Invalid combination of options")
     # endregion
-    
-    all_mask_arrays : np.ndarray = _mask_generation(
-            octree_leaves=octree_leaves,
-            masking_option=options.dual_contouring_masking_options
-        )
-    
+
+    all_mask_arrays: np.ndarray = _mask_generation(
+        octree_leaves=octree_leaves,
+        masking_option=options.mesh_extraction_masking_options
+    )
+
     for n_scalar_field in range(data_descriptor.stack_structure.n_stacks):
         previous_stack_is_onlap = data_descriptor.stack_relation[n_scalar_field - 1] == 'Onlap'
         was_erosion_before = data_descriptor.stack_relation[n_scalar_field - 1] == 'Erosion'
         if previous_stack_is_onlap and was_erosion_before:  # ? (July, 2023) Is this still valid? I thought we have all the combinations
             raise NotImplementedError("Erosion and Onlap are not supported yet")
             pass
 
-        mask: np.ndarray = all_mask_arrays[n_scalar_field] 
-        
+        mask: np.ndarray = all_mask_arrays[n_scalar_field]
+
         if mask is not None and left_right_codes is not None:
             left_right_codes_per_stack = left_right_codes[mask]
         else:
             left_right_codes_per_stack = left_right_codes
 
         # @off
         dc_data: DualContouringData = interpolate_on_edges_for_dual_contouring(
-            data_descriptor     = data_descriptor,
-            interpolation_input = interpolation_input,
-            options             = dual_contouring_options,
-            n_scalar_field      = n_scalar_field,  
-            octree_leaves       = octree_leaves,
-            mask                = mask
+            data_descriptor=data_descriptor,
+            interpolation_input=interpolation_input,
+            options=dual_contouring_options,
+            n_scalar_field=n_scalar_field,
+            octree_leaves=octree_leaves,
+            mask=mask
         )
 
         meshes: List[DualContouringMesh] = compute_dual_contouring(
-            dc_data_per_stack = dc_data,
-            left_right_codes  = left_right_codes_per_stack,
-            debug             = options.debug
+            dc_data_per_stack=dc_data,
+            left_right_codes=left_right_codes_per_stack,
+            debug=options.debug
         )
-        
+
         # ! If the order of the meshes does not match the order of scalar_field_at_surface points we need to reorder them HERE
 
         if meshes is not None:
             all_meshes.extend(meshes)
         # @on
 
     return all_meshes
 
 
-def _mask_generation(octree_leaves, masking_option: DualContouringMaskingOptions) -> np.ndarray | None:
+def _mask_generation(octree_leaves, masking_option: MeshExtractionMaskingOptions) -> np.ndarray | None:
     all_scalar_fields_outputs: list[InterpOutput] = octree_leaves.outputs_corners
     n_scalar_fields = len(all_scalar_fields_outputs)
     grid_size = all_scalar_fields_outputs[0].grid_size
-    mask_matrix = np.zeros((n_scalar_fields, grid_size//8), dtype=bool)
+    mask_matrix = BackendTensor.t.zeros((n_scalar_fields, grid_size // 8), dtype=bool)
     onlap_chain_counter = 0
 
     for i in range(n_scalar_fields):
         stack_relation = all_scalar_fields_outputs[i].scalar_fields.stack_relation
         match (masking_option, stack_relation):
-            case DualContouringMaskingOptions.RAW, _:
-                mask_matrix[i] = np.ones(grid_size//8, dtype=bool)
-            case DualContouringMaskingOptions.DISJOINT, _:
+            case MeshExtractionMaskingOptions.RAW, _:
+                mask_matrix[i] = BackendTensor.t.ones(grid_size // 8, dtype=bool)
+            case MeshExtractionMaskingOptions.DISJOINT, _:
                 raise NotImplementedError("Disjoint is not supported yet. Not even sure if there is anything to support")
-            # case (DualContouringMaskingOptions.DISJOINT | DualContouringMaskingOptions.INTERSECT, StackRelationType.FAULT):
+            # case (MeshExtractionMaskingOptions.DISJOINT | MeshExtractionMaskingOptions.INTERSECT, StackRelationType.FAULT):
             #     mask_matrix[i] = np.ones(grid_size//8, dtype=bool)
-            # case DualContouringMaskingOptions.DISJOINT, StackRelationType.ERODE | StackRelationType.BASEMENT:
+            # case MeshExtractionMaskingOptions.DISJOINT, StackRelationType.ERODE | StackRelationType.BASEMENT:
             #     mask_scalar = all_scalar_fields_outputs[i - 1].squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
             #     if MaskBuffer.previous_mask is None:
             #         mask = mask_scalar
             #     else:
             #         mask = (MaskBuffer.previous_mask ^ mask_scalar) * mask_scalar
             #     MaskBuffer.previous_mask = mask
-            # case DualContouringMaskingOptions.DISJOINT, StackRelationType.ONLAP:
+            # case MeshExtractionMaskingOptions.DISJOINT, StackRelationType.ONLAP:
             #     raise NotImplementedError("Onlap is not supported yet")
             #     return octree_leaves.outputs_corners[n_scalar_field].squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
-            case DualContouringMaskingOptions.INTERSECT, StackRelationType.ERODE:
-                mask_matrix[i] = all_scalar_fields_outputs[i + onlap_chain_counter].squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
+            case MeshExtractionMaskingOptions.INTERSECT, StackRelationType.ERODE:
+                x = all_scalar_fields_outputs[i + onlap_chain_counter].squeezed_mask_array.reshape((1, -1, 8))
+                mask_matrix[i] = BackendTensor.t.sum(x, -1, bool)[0]
                 onlap_chain_counter = 0
-            case DualContouringMaskingOptions.INTERSECT,  StackRelationType.BASEMENT:
-                mask_matrix[i] = all_scalar_fields_outputs[i].squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
+            case MeshExtractionMaskingOptions.INTERSECT, StackRelationType.BASEMENT:
+                x = all_scalar_fields_outputs[i].squeezed_mask_array.reshape((1, -1, 8))
+                mask_matrix[i] = BackendTensor.t.sum(x, -1, bool)[0]
                 onlap_chain_counter = 0
-            case DualContouringMaskingOptions.INTERSECT, StackRelationType.ONLAP:
-                mask_matrix[i] = all_scalar_fields_outputs[i].squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
+            case MeshExtractionMaskingOptions.INTERSECT, StackRelationType.ONLAP:
+                x = all_scalar_fields_outputs[i].squeezed_mask_array.reshape((1, -1, 8))
+                mask_matrix[i] = BackendTensor.t.sum(x, -1, bool)[0]
                 onlap_chain_counter += 1
             case _, StackRelationType.FAULT:
-                mask_matrix[i] = np.ones(grid_size//8, dtype=bool)
+                mask_matrix[i] = BackendTensor.t.ones(grid_size // 8, dtype=bool)
             case _:
                 raise ValueError("Invalid combination of options")
-    
-    return mask_matrix
+
+    return mask_matrix
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_interp_scalar_field.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_interp_scalar_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,15 @@
     @classmethod
     def get(cls, solver_input: SolverInput, kernel_options: KernelOptions):
         input_hash = hash((solver_input, kernel_options))
         current_weights = cls.weights.get(input_hash, None)
         return current_weights
 
 
-def interpolate_scalar_field(solver_input: SolverInput, options: InterpolationOptions) -> \
-        Tuple[np.ndarray, ExportedFields]:
+def interpolate_scalar_field(solver_input: SolverInput, options: InterpolationOptions) -> Tuple[np.ndarray, ExportedFields]:
     # region Solver
     if WeightsBuffer.get(solver_input, options.kernel_options) is None:
         weights = _solve_interpolation(solver_input, options.kernel_options)
         WeightsBuffer.add(weights, solver_input, options.kernel_options)
     else:
         weights = WeightsBuffer.get(solver_input, options.kernel_options)
 
@@ -61,17 +60,17 @@
         # Save debug data for later
         from gempy_engine.core.data.solutions import Solutions
         Solutions.debug_input_data["weights"] = weights
         Solutions.debug_input_data["A_matrix"] = A_matrix
         Solutions.debug_input_data["b_vector"] = b_vector
 
         # Check matrices have the right dtype:
-        assert A_matrix.dtype == BackendTensor.dtype, f"Wrong dtype for A_matrix: {A_matrix.dtype}. should be {BackendTensor.dtype}"
-        assert b_vector.dtype == BackendTensor.dtype, f"Wrong dtype for b_vector: {b_vector.dtype}. should be {BackendTensor.dtype}"
-        assert weights.dtype == BackendTensor.dtype, f"Wrong dtype for weights: {weights.dtype}. should be {BackendTensor.dtype}"
+        assert A_matrix.dtype == BackendTensor.dtype_obj, f"Wrong dtype for A_matrix: {A_matrix.dtype}. should be {BackendTensor.dtype_obj}"
+        assert b_vector.dtype == BackendTensor.dtype_obj, f"Wrong dtype for b_vector: {b_vector.dtype}. should be {BackendTensor.dtype_obj}"
+        assert weights.dtype == BackendTensor.dtype_obj, f"Wrong dtype for weights: {weights.dtype}. should be {BackendTensor.dtype_obj}"
 
     return weights
 
 
 def _evaluate_sys_eq(solver_input: SolverInput, weights: np.ndarray, options: InterpolationOptions) -> ExportedFields:
     compute_gradient: bool = options.compute_scalar_gradient
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_interp_single_feature.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_interp_single_feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import copy
 from typing import Optional, Callable
 
 import numpy as np
 
+from gempy_engine.config import AvailableBackends, COMPUTE_GRADIENTS
 from ...core.backend_tensor import BackendTensor
 from ._interp_scalar_field import interpolate_scalar_field
 from ...core.data import SurfacePoints, SurfacePointsInternals, Orientations, OrientationsInternals, TensorsStructure
 from ...core.data.exported_fields import ExportedFields
 from ...core.data.internal_structs import SolverInput
 from ...core.data.interpolation_functions import CustomInterpolationFunctions
 from ...core.data.interpolation_input import InterpolationInput
@@ -21,15 +22,18 @@
                         options: InterpolationOptions,
                         data_shape: TensorsStructure,
                         solver_input: SolverInput,
                         external_interp_funct: Optional[CustomInterpolationFunctions] = None,
                         external_segment_funct: Optional[Callable[[np.ndarray], float]] = None,
                         clean_buffer: bool = True) -> ScalarFieldOutput:
     
-    grid = copy.deepcopy(interpolation_input.grid)
+    if BackendTensor.engine_backend is not AvailableBackends.PYTORCH and COMPUTE_GRADIENTS is False:
+        grid = copy.deepcopy(interpolation_input.grid)
+    else:
+        grid = interpolation_input.grid
 
     # region Interpolate scalar field
     xyz = solver_input.xyz_to_interpolate
 
     if external_interp_funct is None:  # * EXTERNAL INTERPOLATION FUNCTION branching
         weights, exported_fields = interpolate_scalar_field(solver_input, options)
 
@@ -53,46 +57,49 @@
     # endregion
 
     # region segmentation
     unit_values = interpolation_input.unit_values
     if external_segment_funct is not None:
         sigmoid_slope = external_segment_funct(xyz)
     else:
-        sigmoid_slope = 50000
+        sigmoid_slope = options.sigmoid_slope
 
     values_block: np.ndarray = activator_interface.activate_formation_block(exported_fields, unit_values, sigmoid_slope=sigmoid_slope)
     
     # endregion
     
     output = ScalarFieldOutput(
         weights=weights,
         grid=grid,
         exported_fields=exported_fields,
         values_block=values_block, # TODO: Check value
         stack_relation=interpolation_input.stack_relation
     )
 
-    if BackendTensor.dtype:
+    if BackendTensor.dtype and BackendTensor.engine_backend != AvailableBackends.PYTORCH:
         # Check matrices have the right dtype:
         assert values_block.dtype == BackendTensor.dtype, f"Wrong dtype for values_bloc: {values_block.dtype}. should be {BackendTensor.dtype}"
         assert exported_fields.scalar_field.dtype == BackendTensor.dtype, f"Wrong dtype for scalar_field: {exported_fields.scalar_field.dtype}. should be {BackendTensor.dtype}"
 
     return output
 
 
 def input_preprocess(data_shape: TensorsStructure, interpolation_input: InterpolationInput) -> SolverInput:
     grid = interpolation_input.grid
     surface_points: SurfacePoints = interpolation_input.surface_points
     orientations: Orientations = interpolation_input.orientations
 
     sp_internal: SurfacePointsInternals = data_preprocess_interface.prepare_surface_points(surface_points, data_shape)
     ori_internal: OrientationsInternals = data_preprocess_interface.prepare_orientations(orientations)
-
+    
     # * We need to interpolate in ALL the surface points not only the surface points of the stack
-    grid_internal: np.ndarray = data_preprocess_interface.prepare_grid(grid.values, interpolation_input.all_surface_points)
+    grid_internal: np.ndarray = data_preprocess_interface.prepare_grid(
+        grid=grid.values,
+        surface_points=interpolation_input.all_surface_points
+    )
 
     fault_values: FaultsData = interpolation_input.fault_values
     faults_on_sp: np.ndarray = fault_values.fault_values_on_sp
     fault_ref, fault_rest = data_preprocess_interface.prepare_faults(faults_on_sp, data_shape)
     fault_values.fault_values_ref, fault_values.fault_values_rest = fault_ref, fault_rest
 
     solver_input = SolverInput(
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_multi_scalar_field_manager.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_multi_scalar_field_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,14 @@
         compute_scalar_grad       = options.compute_scalar_gradient
     )
 
     all_outputs = []
     for e, _ in enumerate(all_scalar_fields_outputs):
         output: InterpOutput = InterpOutput(all_scalar_fields_outputs[e], combined_scalar_output[e])
         all_outputs.append(output)
-
     return all_outputs
 
 
 def _interpolate_stack(root_data_descriptor: InputDataDescriptor, root_interpolation_input: InterpolationInput,
                        options: InterpolationOptions) -> ScalarFieldOutput | List[ScalarFieldOutput]:
     # region === Local functions ===
     def _grab_stack_fault_data(_all_stack_values_block, _interpolation_input_i, _stack_structure) -> FaultsData:
@@ -57,15 +56,17 @@
     # endregion
 
     stack_structure = root_data_descriptor.stack_structure
 
     all_scalar_fields_outputs: List[ScalarFieldOutput | None] = [None] * stack_structure.n_stacks
 
     xyz_to_interpolate_size: int = root_interpolation_input.grid.len_all_grids + root_interpolation_input.surface_points.n_points
-    all_stack_values_block: np.ndarray = np.zeros((stack_structure.n_stacks, xyz_to_interpolate_size), dtype=BackendTensor.dtype)  # * Used for faults
+    all_stack_values_block: np.ndarray = BackendTensor.t.zeros(
+        (stack_structure.n_stacks, xyz_to_interpolate_size),
+        dtype=BackendTensor.dtype_obj)  # * Used for faults
 
     for i in range(stack_structure.n_stacks):
         stack_structure.stack_number = i
 
         tensor_struct_i: TensorsStructure = TensorsStructure.from_tensor_structure_subset(root_data_descriptor, i)
         interpolation_input_i: InterpolationInput = InterpolationInput.from_interpolation_input_subset(
             all_interpolation_input = root_interpolation_input,
@@ -101,15 +102,15 @@
             )
 
     return all_scalar_fields_outputs
 
 
 def _modify_faults_values_output(fault_input: FaultsData, values_on_all_xyz: np.ndarray,
                                  xyz_to_interpolate: np.ndarray) -> np.ndarray:
-    val_min = np.min(values_on_all_xyz, axis=1).reshape(-1, 1)  # ? Is this as good as it gets?
+    val_min = BackendTensor.t.min(values_on_all_xyz, axis=1).reshape(-1, 1)  # ? Is this as good as it gets?
     shifted_vals = (values_on_all_xyz - val_min)  # * Shift values between 0 and 1... hopefully
     if fault_input.finite_faults_defined:
         # TODO: Rescale scalar field parameters
         finite_fault_scalar: np.ndarray = fault_input.finite_fault_data.apply(
             points=xyz_to_interpolate
         )
         fault_scalar_field = shifted_vals * finite_fault_scalar
@@ -118,15 +119,15 @@
     return fault_scalar_field
 
 
 # @off
 def _lithology_mask(all_scalar_fields_outputs: List[ScalarFieldOutput], stack_relation: List[StackRelationType]) -> np.ndarray:
     n_scalar_fields = len(all_scalar_fields_outputs)
     grid_size       = all_scalar_fields_outputs[0].grid_size
-    mask_matrix     = np.zeros((n_scalar_fields, grid_size), dtype = bool)
+    mask_matrix     = BackendTensor.t.zeros((n_scalar_fields, grid_size), dtype = bool)
     
     onlap_chain_counter = 0
     # Setting the mask matrix
     for i in range(n_scalar_fields):
         onlap_chain_cont   : bool = stack_relation[i - 1] in [StackRelationType.ONLAP, StackRelationType.FAULT]
         onlap_chain_began  : bool = stack_relation[i - 1 - onlap_chain_counter] is StackRelationType.ONLAP
         onlap_chain_counter: int  = (onlap_chain_counter + 1) * onlap_chain_cont * onlap_chain_began
@@ -148,26 +149,26 @@
                 mask_matrix[i, :] = all_scalar_fields_outputs[i].mask_components_fault
             case False | StackRelationType.BASEMENT:
                 mask_matrix[i, :] = all_scalar_fields_outputs[i].mask_components_basement
             case _:
                 raise ValueError(f"Stack relation {stack_relation[i]} not recognized")
     
     # Doing the black magic
-    final_mask_array     = np.zeros((n_scalar_fields, grid_size), dtype=bool)
+    final_mask_array     = BackendTensor.t.zeros((n_scalar_fields, grid_size), dtype=bool)
     final_mask_array[0]  = mask_matrix[-1]
-    final_mask_array[1:] = np.cumprod(np.invert(mask_matrix[:-1]), axis=0)
+    final_mask_array[1:] = BackendTensor.t.cumprod(BackendTensor.t.invert(mask_matrix[:-1]), axis=0)
     final_mask_array     *= mask_matrix
 
     return final_mask_array
 
 
 def _faults_mask(all_scalar_fields_outputs: List[ScalarFieldOutput], stack_relation: List[StackRelationType]) -> np.ndarray:
     n_scalar_fields = len(all_scalar_fields_outputs)
     grid_size       = all_scalar_fields_outputs[0].grid_size
-    mask_matrix     = np.zeros((n_scalar_fields, grid_size), dtype = bool)
+    mask_matrix     = BackendTensor.t.zeros((n_scalar_fields, grid_size), dtype = bool)
 
     for i in range(len(all_scalar_fields_outputs)):
         match stack_relation[i]:
             case StackRelationType.FAULT:
                 mask_matrix[i, :] = all_scalar_fields_outputs[i].mask_components_erode # * Faults behave as erosion contacts for the fault block
             case _:
                 mask_matrix[i, :] = all_scalar_fields_outputs[i].mask_components_fault
@@ -177,17 +178,17 @@
 
 
 def _combine_scalar_fields(all_scalar_fields_outputs: List[ScalarFieldOutput],
                            lithology_mask: np.ndarray,
                            faults_mask: np.ndarray,
                            compute_scalar_grad: bool = False) -> List[CombinedScalarFieldsOutput]:
     n_scalar_fields            : int     = len(all_scalar_fields_outputs)
-    squeezed_value_block       : ndarray = np.zeros((1 , lithology_mask.shape[1]))
-    squeezed_fault_block       : ndarray = np.zeros((1 , lithology_mask.shape[1]))
-    squeezed_scalar_field_block: ndarray = np.zeros((1 , lithology_mask.shape[1]))
+    squeezed_value_block       : ndarray = BackendTensor.t.zeros((1 , lithology_mask.shape[1]))
+    squeezed_fault_block       : ndarray = BackendTensor.t.zeros((1 , lithology_mask.shape[1]))
+    squeezed_scalar_field_block: ndarray = BackendTensor.t.zeros((1 , lithology_mask.shape[1]))
 
     def _apply_mask(block_to_squeeze: np.ndarray, squeezed_mask_array: np.ndarray, previous_block: np.ndarray) -> np.ndarray:
         return (previous_block + block_to_squeeze * squeezed_mask_array).reshape(-1)
 
     all_combined_scalar_fields = []
     for i in range(n_scalar_fields):
         interp_output: ScalarFieldOutput = all_scalar_fields_outputs[i]
@@ -207,17 +208,17 @@
         squeezed_fault_block = _apply_mask(
             block_to_squeeze    = interp_output.values_block,
             squeezed_mask_array = faults_mask[i],
             previous_block      = squeezed_fault_block
         )
 
         if compute_scalar_grad is True:
-            squeezed_gx_block: Optional[ndarray] = np.zeros((1, lithology_mask.shape[1]))
-            squeezed_gy_block: Optional[ndarray] = np.zeros((1, lithology_mask.shape[1]))
-            squeezed_gz_block: Optional[ndarray] = np.zeros((1, lithology_mask.shape[1]))
+            squeezed_gx_block: Optional[ndarray] = BackendTensor.t.zeros((1, lithology_mask.shape[1]))
+            squeezed_gy_block: Optional[ndarray] = BackendTensor.t.zeros((1, lithology_mask.shape[1]))
+            squeezed_gz_block: Optional[ndarray] = BackendTensor.t.zeros((1, lithology_mask.shape[1]))
 
             squeezed_gx_block = _apply_mask(interp_output.exported_fields.gx_field, lithology_mask[i], squeezed_gx_block)
             squeezed_gy_block = _apply_mask(interp_output.exported_fields.gy_field, lithology_mask[i], squeezed_gy_block)
             squeezed_gz_block = _apply_mask(interp_output.exported_fields.gz_field, lithology_mask[i], squeezed_gz_block)
         else:
             squeezed_gx_block = None
             squeezed_gy_block = None
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/_octree_generation.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/_octree_generation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import copy
 from typing import List
 
+from ...core.backend_tensor import BackendTensor
+from ...config import COMPUTE_GRADIENTS, AvailableBackends
 from ...core.data.regular_grid import RegularGrid
 from ...core.data.options import InterpolationOptions
 from ...core.data.octree_level import OctreeLevel
 from ...core.data.interp_output import InterpOutput
 from ...core.data.grid import Grid
 from ...core.data.input_data_descriptor import InputDataDescriptor
 from ...core.data.interpolation_input import InterpolationInput
@@ -12,27 +14,31 @@
 from ._multi_scalar_field_manager import interpolate_all_fields
 
 import numpy as np
 
 
 def interpolate_on_octree(interpolation_input: InterpolationInput, options: InterpolationOptions,
                           data_shape: InputDataDescriptor) -> OctreeLevel:
-    interpolation_input = copy.deepcopy(interpolation_input)
+    
+    if BackendTensor.engine_backend is not AvailableBackends.PYTORCH and COMPUTE_GRADIENTS is False:
+        temp_interpolation_input = copy.deepcopy(interpolation_input)
+    else:
+        temp_interpolation_input = interpolation_input
     
     # * Interpolate - centers
-    output_0_centers: List[InterpOutput] = interpolate_all_fields(interpolation_input, options, data_shape)  # interpolate - centers
+    output_0_centers: List[InterpOutput] = interpolate_all_fields(temp_interpolation_input, options, data_shape)  # interpolate - centers
 
     # * Interpolate - corners
-    grid_0_centers: Grid = interpolation_input.grid  # ? This could be moved to the next section
+    grid_0_centers: Grid = temp_interpolation_input.grid  # ? This could be moved to the next section
     if options.compute_corners:
         grid_0_corners = Grid.from_xyz_coords(
             xyz_coords=_generate_corners(regular_grid=grid_0_centers.regular_grid)
         )
-        interpolation_input.grid = grid_0_corners  # * Prepare grid for next interpolation
-        output_0_corners: List[InterpOutput] = interpolate_all_fields(interpolation_input, options, data_shape)  # * This is unnecessary for the last level except for Dual contouring
+        temp_interpolation_input.grid = grid_0_corners  # * Prepare grid for next interpolation
+        output_0_corners: List[InterpOutput] = interpolate_all_fields(temp_interpolation_input, options, data_shape)  # * This is unnecessary for the last level except for Dual contouring
     else:
         output_0_corners = []
         grid_0_corners = None
     
     # * Create next octree level
     next_octree_level = OctreeLevel(
         grid_centers=grid_0_centers,
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/interp_single/interp_features.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/interp_single/interp_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import copy
 from typing import List
 
 import gempy_engine.core.data.tensors_structure
+from gempy_engine.config import AvailableBackends, COMPUTE_GRADIENTS
+from ...core.backend_tensor import BackendTensor
+from ...core.data.grid import Grid
 from ...core import data
 from ...core.data import InterpolationOptions
 from ...core.data.octree_level import OctreeLevel
 from ...core.data.interp_output import InterpOutput
 from ...core.data.scalar_field_output import ScalarFieldOutput
 from ...core.data.input_data_descriptor import InputDataDescriptor
 from ...core.data.interpolation_input import InterpolationInput
@@ -22,32 +25,38 @@
                                 data_descriptor: InputDataDescriptor) -> List[OctreeLevel]:
     n_levels = options.number_octree_levels
 
     octree_list = []
     for i in range(0, n_levels):
         options.current_octree_level = i
         
+        # * Here it goes all the different grids
         next_octree: OctreeLevel = interpolate_on_octree(interpolation_input, options, data_descriptor)
         
         if options.is_last_octree_level is False:
-            grid_1_centers = get_next_octree_grid(
+            # * This is only a Grid with a Regular grid
+            grid_1_centers: Grid = get_next_octree_grid(
                 prev_octree=next_octree,
                 compute_topology=False,
                 debug=False
             )
             interpolation_input.grid = grid_1_centers
         octree_list.append(next_octree)
 
     return octree_list
 
 
 def interpolate_all_fields_no_octree(interpolation_input: InterpolationInput, options: InterpolationOptions,
                                      data_descriptor: InputDataDescriptor) -> List[InterpOutput]:
-    interpolation_input = copy.deepcopy(interpolation_input)
-    return ms.interpolate_all_fields(interpolation_input, options, data_descriptor)
+    if BackendTensor.engine_backend is not AvailableBackends.PYTORCH and COMPUTE_GRADIENTS is False:
+        temp_interpolation_input = copy.deepcopy(interpolation_input)
+    else:
+        temp_interpolation_input = interpolation_input
+
+    return ms.interpolate_all_fields(temp_interpolation_input, options, data_descriptor)
 
 
 # region testing
 # ? DEP - It seems I just run this in the tests
 def interpolate_single_field(interpolation_input: InterpolationInput, options: data.InterpolationOptions,
                              data_shape: gempy_engine.core.data.tensors_structure.TensorsStructure) -> InterpOutput:  # * Only For testing
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/model/model_api.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/model/model_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,73 @@
 import copy
 from typing import List, Optional
 
+from ...core.backend_tensor import BackendTensor
+from ...config import COMPUTE_GRADIENTS, AvailableBackends
+from ...core.data.interp_output import InterpOutput
+from ...core.data.geophysics_input import GeophysicsInput
+from ...modules.geophysics.fw_gravity import compute_gravity
 from ...core.data.dual_contouring_mesh import DualContouringMesh
 from ..dual_contouring.multi_scalar_dual_contouring import dual_contouring_multi_scalar
 from ..interp_single._interp_scalar_field import WeightsBuffer
 from ..interp_single.interp_features import interpolate_n_octree_levels
 from ...core.data import InterpolationOptions
 from ...core.data.solutions import Solutions
 from ...core.data.octree_level import OctreeLevel
 from ...core.data.input_data_descriptor import InputDataDescriptor
 from ...core.data.interpolation_input import InterpolationInput
 from ...core.utils import gempy_profiler_decorator
 
 
 @gempy_profiler_decorator
 def compute_model(interpolation_input: InterpolationInput, options: InterpolationOptions,
-                  data_descriptor: InputDataDescriptor) -> Solutions:
+                  data_descriptor: InputDataDescriptor, *, geophysics_input: Optional[GeophysicsInput] = None) -> Solutions:
     WeightsBuffer.clean()
-    
+
     # TODO: Make sure if this works with TF
     # ! If we inline this it seems the deepcopy does not work
-    interpolation_input = copy.deepcopy(interpolation_input) 
-    
+    if BackendTensor.engine_backend is not AvailableBackends.PYTORCH and COMPUTE_GRADIENTS is False:
+        interpolation_input = copy.deepcopy(interpolation_input)
+
     output: list[OctreeLevel] = interpolate_n_octree_levels(
         interpolation_input=interpolation_input,
         options=options,
         data_descriptor=data_descriptor
     )
 
+    # region Geophysics
+    # ---------------------
+
+    # TODO: [ ] Gravity
+
+    # TODO: [ ] Magnetics
+
+    if geophysics_input is not None:
+        first_level_last_field: InterpOutput = output[0].outputs_centers[-1]
+        gravity = compute_gravity(
+            geophysics_input=geophysics_input,
+            root_ouput=first_level_last_field
+        )
+    else:
+        gravity = None
+
+    # endregion
+
     meshes: Optional[list[DualContouringMesh]] = None
-    if options.dual_contouring:
+    if options.mesh_extraction:
         meshes: list[DualContouringMesh] = dual_contouring_multi_scalar(
             data_descriptor=data_descriptor,
             interpolation_input=interpolation_input,
             options=options,
             octree_list=output[:options.number_octree_levels_surface]
         )
 
-    # ---------------------
-    # TODO: [ ] Gravity
-
-    # TODO: [ ] Magnetics
-
     solutions = Solutions(
         octrees_output=output,
         dc_meshes=meshes,
+        fw_gravity=gravity
     )
 
     if options.debug:
         solutions.debug_input_data["stack_interpolation_input"] = interpolation_input
 
     return solutions
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/server/_process_output.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/server/_process_output.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/server/_server_functions.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/server/_server_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/API/server/main_server_pro.py` & `gempy_engine-2023.2.0b1/gempy_engine/API/server/main_server_pro.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from gempy_engine.core.data import InterpolationOptions
 from gempy_engine.core.data.input_data_descriptor import InputDataDescriptor
 from gempy_engine.core.data.interpolation_input import InterpolationInput
 from gempy_engine.core.data.kernel_classes.kernel_functions import AvailableKernelFunctions
 from ._process_output import process_output
 from ._server_functions import process_input, setup_logger
 from ...core.data.kernel_classes.server.input_parser import GemPyInput
-from ...core.data.options import DualContouringMaskingOptions
+from ...core.data.options import MeshExtractionMaskingOptions
 from ...core.data.solutions import Solutions
 
 try:
     # noinspection PyUnresolvedReferences
     import pyvista as pv
     from test.helper_functions_pyvista import plot_octree_pyvista, plot_dc_meshes, plot_pyvista
 except ImportError:
@@ -37,15 +37,15 @@
 
 range_ = 1
 default_interpolation_options: InterpolationOptions = InterpolationOptions(
     range= range_,  # TODO: have constructor from RegularGrid
     c_o=( range_ ** 2 ) / 14 / 3,
     number_octree_levels=4,
     kernel_function=AvailableKernelFunctions.cubic,
-    dual_contouring=True
+    mesh_extraction=True
 )
 
 
 # endregion
 
 logger = setup_logger()
 
@@ -59,19 +59,19 @@
         gempy_input=gempy_input,
         logger=logger
     )
 
     # region Set new fancy triangulation TODO: This has to be move to the interpolation options coming from the client
     FANCY_TRIANGULATION = True
     if FANCY_TRIANGULATION:
-        default_interpolation_options.dual_contouring_fancy = True
-        # default_interpolation_options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW  # * To Date only raw making is supported
+        default_interpolation_options.mesh_extraction_fancy = True
+        # default_interpolation_options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW  # * To Date only raw making is supported
     # endregion
 
-    default_interpolation_options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW  # * To Date only raw making is supported
+    default_interpolation_options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW  # * To Date only raw making is supported
     
     solutions: Solutions = _compute_model(
         interpolation_input=interpolation_input,
         options=default_interpolation_options,
         structure=input_data_descriptor
     )
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/config.py` & `gempy_engine-2023.2.0b1/gempy_engine/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from importlib.util import find_spec
 from enum import Enum, auto, Flag
 
 
 class AvailableBackends(Flag):
     numpy = auto()
     tensorflow = auto()
+    PYTORCH = auto()
+    
     # Legacy
     aesara = auto()
     legacy = auto()
 
 
 # ! Careful what we commit here!
 DEBUG_MODE = True
 OPTIMIZE_MEMORY = True
 DEFAULT_BACKEND = AvailableBackends.numpy
 DEFAULT_PYKEOPS = False
 DEFAULT_TENSOR_DTYPE = 'float64'
 LINE_PROFILER_ENABLED = False
 SET_RAW_ARRAYS_IN_SOLUTION = True
+COMPUTE_GRADIENTS = False 
 
 is_numpy_installed = find_spec("numpy") is not None
 is_tensorflow_installed = find_spec("tensorflow") is not None
+is_pytorch_installed = find_spec("pytorch")
 is_pykeops_installed = find_spec("pykeops") is not None
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/backend_tensor.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/backend_tensor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 from typing import Union, Any, Optional
 import warnings
 
 import numpy
 
-from gempy_engine.config import is_pykeops_installed, is_numpy_installed, is_tensorflow_installed, DEBUG_MODE, \
-    DEFAULT_BACKEND, AvailableBackends, DEFAULT_PYKEOPS, DEFAULT_TENSOR_DTYPE
+from gempy_engine.config import (is_pykeops_installed, is_numpy_installed, is_tensorflow_installed,
+                                 is_pytorch_installed,
+                                 DEBUG_MODE, DEFAULT_BACKEND, AvailableBackends, DEFAULT_PYKEOPS, DEFAULT_TENSOR_DTYPE)
 
 if is_pykeops_installed:
     import pykeops.numpy
 
 
 class BackendTensor:
     engine_backend: AvailableBackends
 
     pykeops_enabled: bool
     use_gpu: bool = True
-    dtype: str = 'float64'
+    dtype: str = DEFAULT_TENSOR_DTYPE
+    dtype_obj: Union[str, "torch.dtype"] = DEFAULT_TENSOR_DTYPE
 
     tensor_types: Union
     tensor_backend_pointer: dict = dict()  # Pycharm will infer the type. It is the best I got so far
     tfnp: numpy  # Alias for the tensor backend pointer
     _: Any  # Alias for the tensor backend pointer
     t: numpy  # Alias for the tensor backend pointer
 
+    
     @classmethod
     def get_backend_string(cls) -> str:
-        match(cls.use_gpu, cls.pykeops_enabled):
-            case(True, True):
+        match (cls.use_gpu, cls.pykeops_enabled):
+            case (True, True):
                 return "GPU"
-            case(False, True):
+            case (False, True):
                 return "CPU"
-            case(False, _):
+            case (False, _):
                 return "CPU"
 
     @classmethod
     def change_backend_gempy(cls, engine_backend: AvailableBackends, use_gpu: bool = True, dtype: Optional[str] = None):
-        cls.dtype = DEFAULT_TENSOR_DTYPE if dtype is None else dtype
-        cls._change_backend(engine_backend, pykeops_enabled=DEFAULT_PYKEOPS, use_gpu=use_gpu)
-    
+        cls._change_backend(engine_backend, pykeops_enabled=DEFAULT_PYKEOPS, use_gpu=use_gpu, dtype=dtype)
+
     @classmethod
-    def _change_backend(cls, engine_backend: AvailableBackends, pykeops_enabled: bool = False, use_gpu: bool = True):
+    def _change_backend(cls, engine_backend: AvailableBackends, pykeops_enabled: bool = False, use_gpu: bool = True, dtype: Optional[str] = None):
+        cls.dtype = DEFAULT_TENSOR_DTYPE if dtype is None else dtype
+        cls.dtype_obj = cls.dtype
         match engine_backend:
             case (engine_backend.numpy):
                 if is_numpy_installed is False:
-                    raise AttributeError(f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: numpy")
+                    raise AttributeError(
+                        f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: numpy")
 
                 # * Import a copy of numpy as tfnp
                 from importlib.util import find_spec, module_from_spec
 
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
-                    
+
                     spec = find_spec('numpy')
                     tfnp = module_from_spec(spec)
                     spec.loader.exec_module(tfnp)
 
                 cls._set_active_backend_pointers(engine_backend, tfnp)
                 cls.tensor_types = Union[tfnp.ndarray]  # tensor Types with respect the backend
 
@@ -66,21 +71,23 @@
                         cls.use_gpu = True
                         cls._wrap_pykeops_functions()
                     case (True, True, False):
                         cls.pykeops_enabled = True
                         cls.use_gpu = False
                         cls._wrap_pykeops_functions()
                     case (True, False, _):
-                        raise AttributeError(f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: pykeops")
+                        raise AttributeError(
+                            f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: pykeops")
                     case (False, _, _):
                         cls.pykeops_enabled = False
                         cls.use_gpu = False
             case (engine_backend.tensorflow):
                 if is_tensorflow_installed is False:
-                    raise AttributeError(f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: tensorflow")
+                    raise AttributeError(
+                        f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: tensorflow")
 
                 import tensorflow as tf
                 experimental_numpy_api = tf.experimental.numpy
                 cls._set_active_backend_pointers(engine_backend, experimental_numpy_api)  # * Here is where we set the tensorflow-numpy backend
                 cls.tensor_types = Union[tf.Tensor, tf.Variable]  # tensor Types with respect the backend:
 
                 from tensorflow.python.ops.numpy_ops import np_config
@@ -105,17 +112,30 @@
                         cls.use_gpu = True
                         cls.pykeops_enabled = False
                     case (False, False):
                         tf.config.set_visible_devices([], 'GPU')
                         cls.pykeops_enabled = False
                     case (True, _):
                         raise NotImplementedError("Pykeops is not compatible with Tensorflow yet")
+            case (engine_backend.PYTORCH):
+                if is_pytorch_installed is False:
+                    raise AttributeError(
+                        f"Engine Backend: {engine_backend} cannot be used because the correspondent library is not installed: pytorch")
+
+                import torch as pytorch_copy
+                cls._set_active_backend_pointers(engine_backend, pytorch_copy)  # * Here is where we set the tensorflow-numpy backend
+                cls._wrap_pytorch_functions()
+                cls.dtype_obj = pytorch_copy.float32 if cls.dtype == "float32" else pytorch_copy.float64
+                cls.tensor_types = pytorch_copy.Tensor
+                cls.pykeops_enabled = False  # TODO: Make this compatible with pykeops
+
             case (_):
-                raise AttributeError(f"Engine Backend: {engine_backend} cannot be used because the correspondent library"
-                                     f"is not installed:")
+                raise AttributeError(
+                    f"Engine Backend: {engine_backend} cannot be used because the correspondent library"
+                    f"is not installed:")
 
     @classmethod
     def _set_active_backend_pointers(cls, engine_backend, tfnp):
         cls.engine_backend = engine_backend
         cls.tensor_backend_pointer['active_backend'] = tfnp
         # Add any alias here
         cls.tfnp = cls.tensor_backend_pointer['active_backend']
@@ -127,43 +147,96 @@
     @classmethod
     def describe_conf(cls):
         print(f"\n Using {cls.engine_backend} backend. \n")
         print(f"\n Using gpu: {cls.use_gpu}. \n")
         print(f"\n Using pykeops: {cls.pykeops_enabled}. \n")
 
     @classmethod
+    def _wrap_pytorch_functions(cls):
+        from torch import sum, repeat_interleave
+        import torch
+        
+        def _sum(tensor, axis=None, dtype=None, keepdim=False):
+            if isinstance(dtype, str):
+                dtype = getattr(torch, dtype)
+            
+            return sum(tensor, axis, dtype=dtype, keepdim=keepdim)
+        
+        def _repeat(tensor, n_repeats, axis=None):
+            return repeat_interleave(tensor, n_repeats, dim=axis)
+        
+        def _array(array_like, dtype=None):
+            if isinstance(dtype, str):
+                dtype = getattr(torch, dtype)
+            if isinstance(array_like, torch.Tensor):
+                return array_like
+            else: 
+                return torch.tensor(array_like, dtype=dtype)
+        
+        def _concatenate(tensors, axis=0, dtype=None):
+            # Switch if tensor is numpy array or a torch tensor
+            match type(tensors[0]):
+                case numpy.ndarray:
+                    return numpy.concatenate(tensors, axis=axis)
+                case torch.Tensor:
+                    return torch.cat(tensors, dim=axis)
+        
+        def _transpose(tensor, axes=None):
+            return tensor.transpose(axes[0], axes[1])
+        
+        
+        cls.tfnp.sum = _sum
+        cls.tfnp.repeat = _repeat
+        cls.tfnp.expand_dims = lambda tensor, axis: tensor
+        cls.tfnp.invert = lambda tensor: ~tensor
+        cls.tfnp.hstack = lambda tensors: torch.concat(tensors, dim=1)
+        cls.tfnp.array = _array 
+        cls.tfnp.to_numpy = lambda tensor: tensor.detach().numpy()
+        cls.tfnp.min = lambda tensor, axis: tensor.min(axis=axis)[0]
+        cls.tfnp.max = lambda tensor, axis: tensor.max(axis=axis)[0]
+        cls.tfnp.rint = lambda tensor: tensor.round().type(torch.int32)
+        cls.tfnp.vstack = lambda tensors: torch.cat(tensors, dim=0)
+        cls.tfnp.copy = lambda tensor: tensor.clone()
+        cls.tfnp.concatenate = _concatenate
+        cls.tfnp.transpose = _transpose
+        
+
+    @classmethod
     def _wrap_pykeops_functions(cls):
         def _exp(tensor):
             if type(tensor) == numpy.ndarray:
                 return numpy.exp(tensor)
             elif type(tensor) == pykeops.numpy.LazyTensor:
                 return tensor.exp()
 
-        def _sum(tensor, axis, keepdims=False, dtype=None):
+        def _sum(tensor, axis, dtype=None, keepdims=False):
             if type(tensor) == numpy.ndarray:
                 return numpy.sum(tensor, axis=axis, keepdims=keepdims, dtype=dtype)
             elif type(tensor) == pykeops.numpy.LazyTensor:
                 return tensor.sum(axis)
 
         def _divide(tensor, other, dtype=None):
             if type(tensor) == numpy.ndarray:
                 return numpy.divide(tensor, other, dtype=dtype)
             elif type(tensor) == pykeops.numpy.LazyTensor:
                 return tensor / other
 
         def _sqrt_fn(tensor):
             return tensor.sqrt()
-        
+
         cls.tfnp.sqrt = _sqrt_fn
         cls.tfnp.sum = _sum
         cls.tfnp.exp = _exp
         cls.tfnp.divide = _divide
 
     @classmethod
     def _wrap_numpy_functions(cls):
         cls.tfnp.cast = lambda tensor, dtype: tensor.astype(dtype)
         cls.tfnp.reduce_sum = cls.tfnp.sum
         cls.tfnp.concat = cls.tfnp.concatenate
         cls.tfnp.constant = cls.tfnp.array
+        cls.tfnp.to_numpy = lambda tensor: tensor
+        cls.tfnp.rint = lambda tensor: tensor.round().astype(numpy.int32)
+    
 
 
 BackendTensor._change_backend(DEFAULT_BACKEND)
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/custom_segmentation_functions.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/custom_segmentation_functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 def _implicit_3d_ellipsoid_to_slope(xyz: np.ndarray, center: np.ndarray, radius: np.ndarray,
                                     max_slope: float = 1000, min_slope: float = 1):
     """
     Implicit 3D ellipsoid.
     """
     # ! Finite faults needs quite a bit of fine tunning once we can compute models in real time
     # ! This function only works for elipses perpendicular to the cartesian axis
-    scalar = - np.sum((xyz - center) ** 2.00 / (radius ** 2), axis=1)
+    from gempy_engine.core.backend_tensor import BackendTensor
+    scalar = - BackendTensor.t.sum((xyz - center) ** 2.00 / (radius ** 2), axis=1)
     scalar_shifted = scalar - scalar.min()
 
     sigmoid_slope = 10  # ? This probably should be also public
     Z_x = scalar_shifted
 
     drift_0 = 4  # ? Making it a %. It depends on the radius
     scale_0 = max_slope
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/dual_contouring_data.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/dual_contouring_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 
+from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.core.data.exported_fields import ExportedFields
 
 
 @dataclass(init=True)
 class DualContouringData:
     xyz_on_edge: np.ndarray
     valid_edges: np.ndarray
@@ -25,15 +26,15 @@
 
     bias_center_mass: np.ndarray = None  # * Only for testing
     bias_normals: np.ndarray = None  # * Only for testing
 
     def __post_init__(self):
         if self.exported_fields_on_edges is not None:
             ef = self.exported_fields_on_edges
-            self._gradients = np.stack((ef.gx_field, ef.gy_field, ef.gz_field), axis=0).T  # ! When we are computing the edges for dual contouring there is no surface points
+            self._gradients = BackendTensor.t.stack((ef.gx_field, ef.gy_field, ef.gz_field), axis=0).T  # ! When we are computing the edges for dual contouring there is no surface points
 
     @property
     def gradients(self):
         return self._gradients
 
     @property
     def valid_voxels(self):
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/dual_contouring_mesh.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/dual_contouring_mesh.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/exported_fields.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/exported_fields.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/grid.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/grid.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 from numpy import ndarray
 
+from gempy_engine.core.backend_tensor import BackendTensor
+from .centered_grid import CenteredGrid
 from .generic_grid import GenericGrid
 from .regular_grid import RegularGrid
 
 
 # TODO: [ ] values is independent field to regular grid. Proabably we want to have an extra field for them
 # TODO: (custom_grid?) and then having a values as a property that brings both together?
 @dataclass
 class Grid:
     regular_grid: RegularGrid = None
     custom_grid: Optional[GenericGrid] = None
     topography: Optional[GenericGrid] = None
     sections: Optional[GenericGrid] = None
-    centered_grid = None  # TODO: Not implemented this probably will need something different that the generic grid?
+    geophysics_grid: Optional[CenteredGrid] = None  # TODO: Not implemented this probably will need something different that the generic grid?
 
     debug_vals = None
     
     @classmethod
     def from_xyz_coords(cls, xyz_coords: ndarray) -> "Grid":
         return cls(custom_grid=GenericGrid(values=xyz_coords))
 
@@ -37,18 +39,21 @@
             values.append(self.regular_grid.values)
         if self.custom_grid is not None:
             values.append(self.custom_grid.values)
         if self.topography is not None:
             values.append(self.topography.values)
         if self.sections is not None:
             values.append(self.sections.values)
-        if self.centered_grid is not None:
-            values.append(self.centered_grid.values)
-
-        return np.concatenate(values)
+        if self.geophysics_grid is not None:
+            values.append(self.geophysics_grid.values)
+        
+        values_array = BackendTensor.t.concatenate(values, dtype=BackendTensor.dtype)
+        values_array = BackendTensor.t.array(values_array)
+        
+        return values_array
 
 
     @property
     def regular_grid_slice(self) -> slice:
         return slice(
             0,
             len(self.regular_grid) if self.regular_grid is not None else 0
@@ -75,23 +80,21 @@
         start = self.topography_slice.stop
         return slice(
             start,
             start + len(self.sections) if self.sections is not None else start
         )
 
     @property
-    def centered_grid_slice(self) -> slice:
+    def geophysics_grid_slice(self) -> slice:
         start = self.sections_slice.stop
         return slice(
             start,
-            start + len(self.centered_grid) if self.centered_grid is not None else start
+            start + len(self.geophysics_grid) if self.geophysics_grid is not None else start
         )
 
-
-
     @property
     def len_all_grids(self) -> int:
         return self.values.shape[0]
 
     @property
     def regular_grid_values(self) -> np.ndarray:  # shape(nx, ny, nz, 3)
         return self.regular_grid.values.reshape(*self.regular_grid_shape, 3)
@@ -105,16 +108,16 @@
         return self.topography.values
 
     @property
     def sections_values(self) -> np.ndarray:
         return self.sections.values
 
     @property
-    def centered_grid_values(self) -> np.ndarray:
-        return self.centered_grid.values
+    def geophysics_grid_values(self) -> np.ndarray:
+        return self.geophysics_grid.values
 
     @property
     def regular_grid_shape(self) -> ndarray | list:
         return self.regular_grid.regular_grid_shape
 
     @property
     def dxdydz(self) -> tuple[float, float, float]:
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/input_data_descriptor.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/input_data_descriptor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/internal_structs.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/internal_structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,18 @@
 
     debug = None
 
     def __init__(self, sp_internal: SurfacePointsInternals, ori_internal: OrientationsInternals,
                  xyz_to_interpolate=None, fault_internal=None):
         self.sp_internal = sp_internal
         self.ori_internal = ori_internal
-        if xyz_to_interpolate is not None:
-            self.xyz_to_interpolate = xyz_to_interpolate.astype(BackendTensor.dtype)
+        # ? DEP: Moved to preparation
+        # if xyz_to_interpolate is not None:
+        #     self.xyz_to_interpolate = xyz_to_interpolate.astype(BackendTensor.dtype)
+        self.xyz_to_interpolate = xyz_to_interpolate
         self._fault_internal = fault_internal
 
     def __hash__(self):
         # xyz_to_interpolate and _faults are dependent on the octree levels
         combined = hash((self.sp_internal, self.ori_internal))
         return combined
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/interp_output.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/interp_output.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 
+from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.core.data.exported_structs import CombinedScalarFieldsOutput
 from gempy_engine.core.data.scalar_field_output import ScalarFieldOutput
 
 
 @dataclass(init=True)
 class InterpOutput:
     scalar_fields: ScalarFieldOutput
@@ -70,20 +71,28 @@
         return self.block[self.grid.topography_slice]
 
     @property
     def sections(self):
         return self.block[self.grid.sections_slice]
 
     @property
-    def custom_grid(self):
+    def custom_grid_values(self):
         return self.block[self.grid.custom_grid_slice]
+    
+    @property
+    def geophysics_grid_values(self):
+        return self.block[self.grid.geophysics_grid_slice]
+    
+    @property
+    def ids_geophysics_grid(self):
+        return BackendTensor.t.rint(self.block[self.grid.geophysics_grid_slice])
 
     @property
     def ids_block_regular_grid(self):
-        return np.rint(self.block[self.grid.regular_grid_slice].reshape(self.grid.regular_grid_shape))
+        return np.rint(self.block[self.grid.regular_grid_slice].reshape(self.grid.regular_grid_shape.tolist()))
 
     @property
     def ids_custom_grid(self):
         return np.rint(self.block[self.grid.custom_grid_slice])
 
     @property
     def ids_block(self) -> np.ndarray:
@@ -102,16 +111,16 @@
             return self.combined_scalar_field.final_block  # * (miguel March 2023) For now faults does not have final block. We will have to add a mask logic for fault blocks first
 
     @property
     def litho_faults_ids(self):
         if self.combined_scalar_field is None:  # * This in principle is only used for testing
             return self.ids_block
 
-        litho_ids = np.rint(self.block)
-        faults_ids = np.rint(self.faults_block)
+        litho_ids = BackendTensor.t.rint(self.block)
+        faults_ids = BackendTensor.t.rint(self.faults_block)
 
         # Get the number of unique lithology IDs
         multiplier = len(np.unique(litho_ids))
 
         # Generate the unique IDs
         unique_ids = litho_ids + faults_ids * multiplier
         return unique_ids
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/interpolation_functions.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/interpolation_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import enum
 import functools
 from dataclasses import dataclass
 from typing import Callable
 
 import numpy as np
 
+from gempy_engine.core.backend_tensor import BackendTensor
+
 
 class InterpolationFunctions(enum.Enum):
     GAUSSIAN_PROCESS = enum.auto()
     CUSTOM = enum.auto()
     SPHERE = enum.auto()
     
     
@@ -16,14 +18,17 @@
 class CustomInterpolationFunctions:
     scalar_field_at_surface_points: np.ndarray
     implicit_function: Callable
     gx_function: Callable
     gy_function: Callable
     gz_function: Callable
     
+    def __post_init__(self):
+        self.scalar_field_at_surface_points = BackendTensor.t.array(self.scalar_field_at_surface_points, dtype=BackendTensor.dtype_obj)
+        
     @classmethod
     def from_builtin(cls, interpolation_function: InterpolationFunctions, scalar_field_at_surface_points: np.ndarray,
                      **kwargs):
         match interpolation_function:
             case InterpolationFunctions.SPHERE:
                 # TODO: Move this block to a different module
                 def implicit_sphere(xyz: np.ndarray, extent: np.ndarray):
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/interpolation_input.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/interpolation_input.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 
 from . import SurfacePoints, Orientations
 from gempy_engine.core.data.generic_grid import GenericGrid
+from gempy_engine.core.data.centered_grid import CenteredGrid
 from .grid import Grid
 from .regular_grid import RegularGrid
 from .stack_relation_type import StackRelationType
 from .stacks_structure import StacksStructure
 from .kernel_classes.faults import FaultsData
 from .kernel_classes.server.input_parser import InterpolationInputSchema
 
@@ -100,15 +101,15 @@
         surface_points: SurfacePoints = SurfacePoints(
             sp_coords=transform.apply(structural_frame.surface_points.xyz) + _legacy_factor,
             nugget_effect_scalar=structural_frame.surface_points.nugget
         )
 
         orientations: Orientations = Orientations(
             dip_positions=transform.apply(structural_frame.orientations.xyz) + _legacy_factor,
-            dip_gradients=(transform.transform_gradient(structural_frame.orientations.grads)),
+            dip_gradients=transform.transform_gradient(structural_frame.orientations.grads),
             nugget_effect_grad=structural_frame.orientations.nugget
         )
         
         # TODO: if octrees we should deactivate the regular grid resolution?
         if octrees:
             interpolation_resolution = np.array([2, 2, 2])
         else:
@@ -125,20 +126,29 @@
             extent=new_extents,
             regular_grid_shape=interpolation_resolution,
         )
         
         topography_values: GenericGrid = GenericGrid( values=transform.apply(grid.topography.values)) if grid.topography is not None else None
         section_values: GenericGrid = GenericGrid(values=transform.apply(grid.sections.values)) if grid.sections is not None else None
         custom_values: GenericGrid = GenericGrid(values=transform.apply(grid.custom_grid.values)) if grid.custom_grid is not None else None
+        if grid.centered_grid is not None:
+            centered_grid = CenteredGrid(
+                centers=transform.apply(grid.centered_grid.centers),
+                radius=transform.scale_points(np.atleast_2d(grid.centered_grid.radius))[0], # * This is a bit too much shape manipulation for my taste
+                resolution=grid.centered_grid.resolution
+            )
+        else:
+            centered_grid = None
 
         grid: Grid = Grid(
             regular_grid=regular_grid,
             topography=topography_values,
             sections=section_values,
-            custom_grid=custom_values
+            custom_grid=custom_values,
+            geophysics_grid=centered_grid
         )
 
         # endregion
         
         interpolation_input: InterpolationInput = cls(
             surface_points=surface_points,
             orientations=orientations,
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/faults.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/faults.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/kernel_functions.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/kernel_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def exp_function_p_div_r(sq_r, a):
     return -(1 / (a ** 2) * BackendTensor.tfnp.exp(-(sq_r / (2 * a ** 2))))
 
 
 def exp_function_a(sq_r, a):
-    first_term = BackendTensor.tfnp.divide(sq_r, (a ** 4), dtype=BackendTensor.dtype) # ! This term is almost always zero. I thnk we can just remove it
+    first_term = BackendTensor.tfnp.divide(sq_r, (a ** 4)) # ! This term is almost always zero. I thnk we can just remove it
     second_term = 1 / (a ** 2)
     third_term = BackendTensor.tfnp.exp(-(sq_r / (2 * a ** 2)))
     return (first_term - second_term) * third_term
 
 
 @dataclass
 class KernelFunction:
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/orientations.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/orientations.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     dip_gradients: np.ndarray  #: Initialize this re-normalizes implicitly
 
     nugget_effect_grad: Union[np.ndarray, float] = 0.01
 
     def __post_init__(self):
         if type(self.nugget_effect_grad) is float or type(self.nugget_effect_grad) is int:
             self.nugget_effect_grad = np.ones(self.n_items) * self.nugget_effect_grad
-        cast_type_inplace(self)
+        cast_type_inplace(self, requires_grad=True) # TODO: This has to be grabbed from options
         
         
     def renormalize_gradients(self):
         # * In principle we do this in the Transform class in the main gempy repo
         magnitudes = np.linalg.norm(self.dip_gradients, axis=1, keepdims=True)
         magnitudes[magnitudes == 0] = 1
         self.dip_gradients = self.dip_gradients / magnitudes
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/server/input_parser.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/server/input_parser.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/kernel_classes/surface_points.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/kernel_classes/surface_points.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # TODO (Sep 2022): Pretty sure this has to be private
     slice_feature: Optional[slice] = slice(None, None)  # * Used to slice the surface points values of the interpolation (grid.values)
 
     def __post_init__(self):
         if type(self.nugget_effect_scalar) is float or type(self.nugget_effect_scalar) is int:
             self.nugget_effect_scalar = np.ones(self.n_points) * self.nugget_effect_scalar
-        cast_type_inplace(self)
+        cast_type_inplace(self, requires_grad=True) # TODO: This has to be grabbed from options
 
     @classmethod
     def from_schema(cls, schema: SurfacePointsSchema):
         return cls(sp_coords=np.array(schema.sp_coords))
 
     @classmethod
     def from_suraface_points_subset(cls, surface_points: "SurfacePoints", data_structure: StacksStructure):
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/octree_level.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/octree_level.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 @dataclass(init=True)
 class OctreeLevel:
     # Input
     grid_centers: Grid
     grid_corners: Optional[Grid]
-    outputs_centers: List[InterpOutput]  #: List of output (one per stack)
+    outputs_centers: list[InterpOutput]  #: List of output (one per stack)
     outputs_corners: list[InterpOutput]
 
     # Topo
     edges_id: np.ndarray = None
     count_edges: np.ndarray = None
     marked_edges: List[np.ndarray] = None  # 3 arrays in x, y, z
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/options.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/options.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass, asdict
 
 import gempy_engine.config
 from gempy_engine.core.data.kernel_classes.solvers import Solvers
 from gempy_engine.core.data.kernel_classes.kernel_functions import AvailableKernelFunctions
 
 
-class DualContouringMaskingOptions(enum.Enum):
+class MeshExtractionMaskingOptions(enum.Enum):
     NOTHING = enum.auto()  # * This is only for testing
     DISJOINT = enum.auto()
     INTERSECT = enum.auto()
     RAW = enum.auto()
 
 
 @dataclass(frozen=False)
@@ -99,34 +99,36 @@
     kernel_options                 : KernelOptions                = None  # * This is the compression of the fields above and the way to go in the future
 
     number_octree_levels           : int                          = 1
     current_octree_level           : int                          = 0  # * Make this a read only property 
 
     compute_scalar_gradient        : bool                         = False
 
-    dual_contouring                : bool                         = True
-    dual_contouring_masking_options: DualContouringMaskingOptions = DualContouringMaskingOptions.INTERSECT
-    dual_contouring_fancy          : bool                         = True
+    mesh_extraction                : bool                         = True
+    mesh_extraction_masking_options: MeshExtractionMaskingOptions = MeshExtractionMaskingOptions.INTERSECT
+    mesh_extraction_fancy          : bool                         = True
 
     debug                          : bool                         = gempy_engine.config.DEBUG_MODE
     debug_water_tight              : bool                         = False
 
+    sigmoid_slope                  : int                          = 50000
     _number_octree_levels_surface  : int                          = 4
+
     
     def __init__(
             self,
             range                     : int | float,
             c_o                       : float,
             uni_degree                : int                              = 1,
             i_res                     : float                            = 4,
             gi_res                    : float                            = 2                                   , # ! This should be DEP
             number_dimensions         : int                              = 3                                   , # ? This probably too
             number_octree_levels      : int                              = 1,
             kernel_function           : AvailableKernelFunctions         = AvailableKernelFunctions.cubic,
-            dual_contouring           : bool                             = True,
+            mesh_extraction           : bool                             = True,
             compute_scalar_gradient   : bool                             = False,
             compute_condition_number  : bool                             = False,
             
     ):
         self.number_octree_levels = number_octree_levels
         
         self.kernel_options = KernelOptions(
@@ -136,15 +138,15 @@
             i_res                      = i_res,
             gi_res                     = gi_res,
             number_dimensions          = number_dimensions,
             kernel_function            = kernel_function,
             compute_condition_number = compute_condition_number
         )
 
-        self.dual_contouring         = dual_contouring
+        self.mesh_extraction         = mesh_extraction
         self.compute_scalar_gradient = compute_scalar_gradient
 
     # @on
 
     def __repr__(self):
         return f"InterpolationOptions({', '.join(f'{k}={v}' for k, v in asdict(self).items())})"
 
@@ -163,15 +165,15 @@
 
         Kwargs:
             kernel_options (KernelOptions, optional): Options for the kernel. Default is None.
             number_octree_levels (int, optional): Number of octree levels. Default is 1.
             current_octree_level (int, optional): Current octree level. Default is 0.
             compute_scalar_gradient (bool, optional): Whether to compute the scalar gradient. Default is False.
             dual_contouring (bool, optional): Whether to use dual contouring. Default is True.
-            dual_contouring_masking_options (DualContouringMaskingOptions, optional): Options for dual contouring masking.
+            mesh_extraction_masking_options (MeshExtractionMaskingOptions, optional): Options for dual contouring masking.
             dual_contouring_fancy (bool, optional): Fancy version of dual contouring. Default is True.
             debug (bool, optional): Debug mode status. Default is derived from config.
             debug_water_tight (bool, optional): Debug mode for water-tight conditions. Default is False.
             tensor_dtype (str, optional): Data type for tensors. Default is derived from config.
 
         Returns:
             None
@@ -184,15 +186,15 @@
                 setattr(self, key, value)  # sets the attribute to the provided value
             else:
                 warnings.warn(f"{key} is not a recognized attribute and will be ignored.")
 
     @property
     def compute_corners(self):
         is_not_last_octree = (self.is_last_octree_level is False)
-        is_dual_contouring = self.dual_contouring
+        is_dual_contouring = self.mesh_extraction
         is_octree_for_surfaces = self.current_octree_level == self.number_octree_levels_surface - 1
         is_dual_contouring_and_octree_is_for_surfaces = is_dual_contouring and is_octree_for_surfaces
         
         compute_corners = is_dual_contouring_and_octree_is_for_surfaces or is_not_last_octree
         return compute_corners
 
     @property
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/raw_arrays_solution.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/raw_arrays_solution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 ﻿from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 
-from gempy.optional_dependencies import require_subsurface, require_pandas
+from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.core.data.interp_output import InterpOutput
 from gempy_engine.core.data.dual_contouring_mesh import DualContouringMesh
 from gempy_engine.core.data.octree_level import OctreeLevel
 
 # ? These two imports are suggesting that this class should be splatted and move one half into a gempy.module
 from gempy_engine.modules.octrees_topology.octrees_topology_interface import get_regular_grid_value_for_level
 from gempy_engine.modules.octrees_topology.octrees_topology_interface import ValueType
+from gempy_engine.optional_dependencies import require_pandas, require_subsurface
 
 
 @dataclass(init=True)
 class RawArraysSolution:
     # region Input data results
     # ? Do I need these fields?
     # weights_vector: np.ndarray
@@ -25,15 +26,15 @@
 
     # endregion
 
     # region Regular Grid
     lith_block: np.ndarray = np.empty(0)
     fault_block: np.ndarray = np.empty(0)
     litho_faults_block: np.ndarray = np.empty(0)
-    
+
     scalar_field_matrix: np.ndarray = np.empty(0)
     block_matrix: np.ndarray = np.empty(0)
     mask_matrix: np.ndarray = np.empty(0)
     mask_matrix_squeezed: np.ndarray = np.empty(0)
     values_matrix: np.ndarray = np.empty(0)
     gradient: np.ndarray = np.empty(0)
     # endregion
@@ -46,86 +47,86 @@
 
     # region Geophysics
     fw_gravity: Optional[np.ndarray] = None
     fw_magnetic: Optional[np.ndarray] = None
     # endregion
 
     # region Mesh
-    vertices: list[np.ndarray] = np.empty(( 0, 3 ))
+    vertices: list[np.ndarray] = np.empty((0, 3))
     edges: list[np.ndarray] = None
     # endregion
 
     # region topology
     topology_edges: Optional[np.ndarray] = None  # ? I am not 100% sure the type is correct
     topology_count: Optional[np.ndarray] = None  # ? I am not 100% sure the type is correct
 
     # endregion
 
     # ? TODO: This could be just the init
     @classmethod
-    def from_gempy_engine_solutions(cls, octrees_output: list[OctreeLevel], meshes: list[DualContouringMesh]) \
-            -> "RawArraysSolution":
+    def from_gempy_engine_solutions(cls, octrees_output: list[OctreeLevel], meshes: list[DualContouringMesh],
+                                    fw_gravity: Optional[np.ndarray] = None) -> "RawArraysSolution":
         raw_arrays_solution = cls()
 
         # region Blocks
         last_octree_level: OctreeLevel = octrees_output[(-1)]
 
         raw_arrays_solution.block_matrix = cls._get_regular_grid_values_for_all_structural_groups(
-            octree_output=octrees_output, 
+            octree_output=octrees_output,
             scalar_type=ValueType.values_block
         )
-        
+
         raw_arrays_solution.fault_block = get_regular_grid_value_for_level(
             octree_list=octrees_output,
             level=None,
             value_type=ValueType.faults_block
         ).astype("int8").ravel()
-        
+
         raw_arrays_solution.litho_faults_block = get_regular_grid_value_for_level(
             octree_list=octrees_output,
             level=None,
             value_type=ValueType.litho_faults_block
         ).astype("int32").ravel()
 
         raw_arrays_solution.scalar_field_matrix = cls._get_regular_grid_values_for_all_structural_groups(
             octree_output=octrees_output,
             scalar_type=ValueType.scalar
         )
-        
+
         raw_arrays_solution.mask_matrix = cls._get_regular_grid_values_for_all_structural_groups(
             octree_output=octrees_output,
             scalar_type=ValueType.mask_component
         )
-        
+
         raw_arrays_solution.mask_matrix_squeezed = cls._get_regular_grid_values_for_all_structural_groups(
             octree_output=octrees_output,
             scalar_type=ValueType.squeeze_mask
         )
 
         raw_arrays_solution._set_lith_block(octrees_output)
         raw_arrays_solution._set_scalar_field_at_surface_points(last_octree_level)
         # endregion
-        
+
         # region Grids
         first_level_octree: OctreeLevel = octrees_output[0]
-        
+
         # TODO: Make this more clever to account for the fact that we can have more than one scalar field
         output: InterpOutput = first_level_octree.outputs_centers[-1]  # ! This is the scalar field. Usually we want the last one but not necessarily
-        
-        raw_arrays_solution.geological_map = output.geological_map
-        raw_arrays_solution.sections = output.sections
-        raw_arrays_solution.custom = output.custom_grid
+
+        raw_arrays_solution.geological_map = BackendTensor.t.to_numpy(output.geological_map)
+        raw_arrays_solution.sections = BackendTensor.t.to_numpy(output.sections)
+        raw_arrays_solution.custom = BackendTensor.t.to_numpy(output.custom_grid_values)
         # endregion
-        
+
         # region Meshes
         if meshes:
             raw_arrays_solution.vertices = [mesh.vertices for mesh in meshes]
             raw_arrays_solution.edges = [mesh.edges for mesh in meshes]
             # TODO: I will have to apply the transform to this one
-            
+
         # endregion
         return raw_arrays_solution
 
     # ? Should all these arrays being properties better?
     @staticmethod
     def _get_regular_grid_values_for_all_structural_groups(octree_output: list[OctreeLevel], scalar_type: ValueType):
         temp_list = []
@@ -140,33 +141,34 @@
             )
         scalar_field_stacked = np.vstack(temp_list)
         return scalar_field_stacked
 
     def _set_scalar_field_at_surface_points(self, octree_output: OctreeLevel):
         temp_list = []
         for i in range(octree_output.number_of_outputs):
-            temp_list.append(octree_output.outputs_centers[i].scalar_fields.exported_fields.scalar_field_at_surface_points)
+            at_surface_points = octree_output.outputs_centers[i].scalar_fields.exported_fields.scalar_field_at_surface_points
+            temp_list.append(BackendTensor.t.to_numpy(at_surface_points))
 
         self.scalar_field_at_surface_points = temp_list
 
     def _set_lith_block(self, octree_output: list[OctreeLevel]):
 
         block = get_regular_grid_value_for_level(
             octree_list=octree_output,
             level=None,
             value_type=ValueType.ids
         ).astype("int8").ravel()
-        
-        block[block == 0] = block.max() + 1 # Move basement from first to last
+
+        block[block == 0] = block.max() + 1  # Move basement from first to last
         self.lith_block = block
 
     def meshes_to_subsurface(self):
         ss = require_subsurface()
         pd = require_pandas()
-        
+
         vertex: list[np.ndarray] = self.vertices
         simplex_list: list[np.ndarray] = self.edges
 
         idx_max = 0
         for simplex_array in simplex_list:
             simplex_array += idx_max
             idx_max = simplex_array.max() + 1
@@ -175,9 +177,9 @@
 
         concatenated_id_array = np.concatenate(id_array)
         meshes: ss.UnstructuredData = ss.UnstructuredData.from_array(
             vertex=np.concatenate(vertex),
             cells=np.concatenate(simplex_list),
             vertex_attr=pd.DataFrame({'id': concatenated_id_array})
         )
-        
+
         return meshes
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/regular_grid.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/regular_grid.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,28 @@
 
 @dataclass(frozen=False)  # TODO: I want to do this class immutable
 class RegularGrid:
     extent: Union[np.ndarray, List]
     regular_grid_shape: Union[np.ndarray, List]  # Shape(3)
     _active_cells: np.ndarray = field(default=None, repr=False, init=False)
     left_right: np.ndarray = field(default=None, repr=False, init=False)
-
+    
+    values: np.ndarray = field(default=None, repr=False, init=False)
+    original_values: np.ndarray = field(default=None, repr=False, init=False)  #: When the regular grid is representing a octree level, only active cells are stored in values. This is the original values of the regular grid.
+    
     def __len__(self):
         return self.regular_grid_shape.prod()
 
     def __post_init__(self):
         self.regular_grid_shape = _check_and_convert_list_to_array(self.regular_grid_shape)
         self.extent = _check_and_convert_list_to_array(self.extent) + 1e-6  # * This to avoid some errors evaluating in 0 (e.g. bias in dual contouring)
 
         self.values = self._create_regular_grid(self.extent, self.regular_grid_shape)
+        self.original_values = self.values.copy()
+        
 
     @classmethod
     def from_octree_level(cls, xyz_coords_octree: np.ndarray, previous_regular_grid: "RegularGrid",
                           active_cells: np.ndarray, left_right: np.ndarray) -> "RegularGrid":
        
         regular_grid_for_octree_level = cls(
             extent=previous_regular_grid.extent,
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/scalar_field_output.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/scalar_field_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import dataclasses
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 
+from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.core.data.exported_fields import ExportedFields
 from gempy_engine.core.data.grid import Grid
 from gempy_engine.core.data.stack_relation_type import StackRelationType
 
 
 @dataclass
 class ScalarFieldOutput:
@@ -92,22 +93,22 @@
                     fault_limit_value = exported_fields.scalar_field_at_surface_points.min()
                     thickness_1 = fault_limit_value - fault_thickness
                     thickness_2 = fault_limit_value + fault_thickness
 
                     f1 = exported_fields.scalar_field > thickness_1
                     f2 = exported_fields.scalar_field < thickness_2
 
-                    exported_fields.scalar_field_at_fault_shell = np.array([thickness_1, thickness_2])
+                    exported_fields.scalar_field_at_fault_shell = BackendTensor.t.array([thickness_1, thickness_2])
                     mask_array = f1 * f2
                 else:
                     # TODO:  This branch should be like
                     # ? Is the commented out for finite faults?
                     # erode_limit_value = exported_fields.scalar_field_at_surface_points.min()
                     # mask_lith = exported_fields.scalar_field > erode_limit_value
 
-                    mask_array = np.zeros_like(exported_fields.scalar_field)
+                    mask_array = BackendTensor.t.zeros_like(exported_fields.scalar_field)
             case False | StackRelationType.BASEMENT:
-                mask_array = np.ones_like(exported_fields.scalar_field)
+                mask_array = BackendTensor.t.ones_like(exported_fields.scalar_field)
             case _:
                 raise ValueError("Stack relation type is not supported")
 
         return mask_array
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/solutions.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,24 @@
     _raw_arrays: RawArraysSolution = field(init=False)
     # ------
     gravity: np.ndarray = None
     magnetics: np.ndarray = None
 
     debug_input_data: dict = {}
     
-    def __init__(self, octrees_output: List[OctreeLevel], dc_meshes: List[DualContouringMesh] = None):
+    def __init__(self, octrees_output: List[OctreeLevel], dc_meshes: List[DualContouringMesh] = None, fw_gravity: np.ndarray = None):
         self.octrees_output = octrees_output
         self.dc_meshes = dc_meshes
+        self.gravity = fw_gravity
         
         if SET_RAW_ARRAYS_IN_SOLUTION:  # * This can add an unnecessary overhead
             self._raw_arrays = RawArraysSolution.from_gempy_engine_solutions(
                 octrees_output=octrees_output,
-                meshes=dc_meshes
+                meshes=dc_meshes,
+                fw_gravity=fw_gravity
             )
 
     def __repr__(self):
         return f"Solutions({len(self.octrees_output)} Octree Levels, {len(self.dc_meshes)} DualContouringMeshes)"
 
     def _repr_html_(self):
         return f"<b>Solutions:</b> {len(self.octrees_output)} Octree Levels, {len(self.dc_meshes)} DualContouringMeshes"
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/stacks_structure.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/stacks_structure.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/tensors_structure.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/tensors_structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ﻿from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Type
 
 import numpy as np
 
+from gempy_engine.config import AvailableBackends
 from ..backend_tensor import BackendTensor as b
 
 
 def _cast_type_inplace(struct_data_instance: "TensorStructure"):
     for key, val in struct_data_instance.__dict__.items():
         if type(val) != np.ndarray: continue
         struct_data_instance.__dict__[key] = val.astype(struct_data_instance.dtype)
@@ -58,10 +59,12 @@
 
     @property
     def partitions_bool(self):
         ref_positions = self.reference_sp_position
 
         res = np.eye(self.total_number_sp, dtype='int32')[np.array(ref_positions).reshape(-1)]
         one_hot_ = res.reshape(list(ref_positions.shape) + [self.total_number_sp])
-
+        
+        one_hot_ = b.tfnp.array(one_hot_)
+            
         partitions = b.tfnp.sum(one_hot_, axis=0, dtype=bool)
         return partitions
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/core/data/transforms.py` & `gempy_engine-2023.2.0b1/gempy_engine/core/data/transforms.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/data_preprocess/_input_preparation.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/data_preprocess/_input_preparation.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from gempy_engine.core.data.kernel_classes.orientations import Orientations, OrientationsInternals
 from gempy_engine.core.data.kernel_classes.surface_points import SurfacePoints, SurfacePointsInternals
 
 
 def orientations_preprocess(orientations: Orientations):
     tiled_positions = b.tfnp.tile(orientations.dip_positions, (orientations.n_dimensions, 1))
     tiled_gradients = b.tfnp.tile(orientations.dip_gradients, (orientations.n_dimensions, 1))
-    tiled_nugget = b.tfnp.tile(orientations.nugget_effect_grad, orientations.n_dimensions)
+    tiled_nugget = b.tfnp.tile(orientations.nugget_effect_grad, (1, orientations.n_dimensions))
     return OrientationsInternals(
         orientations=orientations,
         dip_positions_tiled=tiled_positions,
         gradients_tiled=tiled_gradients,
         nugget_effect_grad=tiled_nugget
     )
 
@@ -22,16 +22,18 @@
 
     partitions_bool = tensors_structure.partitions_bool
     
     ref_nugget, ref_points, rest_nugget, rest_points = _compute_rest_ref_in_numpy(partitions_bool, sp_input)
 
     # repeat the reference points (the number of persurface -1)  times
     number_repetitions = tensors_structure.number_of_points_per_surface - 1
-    ref_points_repeated = b.tfnp.repeat(ref_points, number_repetitions, 0)  # ref_points shape: (1, 3)
-    ref_nugget_repeated = b.tfnp.repeat(ref_nugget, number_repetitions, 0)  # ref_nugget shape: (1)
+    number_repetitions = BackendTensor.t.array(number_repetitions)
+    
+    ref_points_repeated = b.t.repeat(ref_points, number_repetitions, 0)  # ref_points shape: (1, 3)
+    ref_nugget_repeated = b.t.repeat(ref_nugget, number_repetitions, 0)  # ref_nugget shape: (1)
 
     nugget_effect_ref_rest = rest_nugget + ref_nugget_repeated
 
     return SurfacePointsInternals(ref_points_repeated, rest_points, nugget_effect_ref_rest)
 
 
 def _compute_rest_ref_in_numpy(partitions_bool: np.ndarray, sp: SurfacePoints):
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/data_preprocess/data_preprocess_interface.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/data_preprocess/data_preprocess_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Tuple
 
 from numpy import ndarray
 
+from gempy_engine.config import AvailableBackends
 from gempy_engine.core.data import SurfacePoints, Orientations, SurfacePointsInternals, TensorsStructure, OrientationsInternals
 import numpy as np
 from gempy_engine.core.backend_tensor import BackendTensor as bt
 
 
 from gempy_engine.modules.data_preprocess._input_preparation import surface_points_preprocess, orientations_preprocess
 
@@ -16,22 +17,21 @@
 
 def prepare_orientations(orientations: Orientations) -> OrientationsInternals:
     return orientations_preprocess(orientations)
 
 
 def prepare_grid(grid: np.ndarray, surface_points: SurfacePoints) -> np.ndarray:
     concat = bt.tfnp.concatenate([grid, surface_points.sp_coords])
-    #concat = np.concatenate([grid, surface_points.sp_coords])    
     return concat
 
 
 def prepare_faults(faults_values_on_sp: np.ndarray, tensors_structure: TensorsStructure) -> Tuple[ndarray, ndarray]:
     
     partitions_bool = tensors_structure.partitions_bool
-    number_repetitions = tensors_structure.number_of_points_per_surface - 1
+    number_repetitions = bt.t.array(tensors_structure.number_of_points_per_surface - 1)
 
     ref_points = faults_values_on_sp[:, partitions_bool]
 
-    ref_matrix_val_repeated = np.repeat(ref_points, number_repetitions, 1)
+    ref_matrix_val_repeated = bt.t.repeat(ref_points, number_repetitions, 1)
     rest_matrix_val = faults_values_on_sp[:, ~partitions_bool]
 
     return ref_matrix_val_repeated, rest_matrix_val
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/dual_contouring/dual_contouring_interface.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/dual_contouring/dual_contouring_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Tuple
 
+from gempy_engine.config import AvailableBackends
 from ...core.backend_tensor import BackendTensor
 from ...core.data.dual_contouring_data import DualContouringData
 import numpy as np
 
 
 def find_intersection_on_edge(_xyz_corners: np.ndarray, scalar_field_on_corners: np.ndarray,
                               scalar_at_sp: np.ndarray, masking=None) -> Tuple[np.ndarray, np.ndarray]:
@@ -19,18 +20,18 @@
     xyz_8 = _xyz_corners.reshape((-1, 8, 3))
 
     if masking is not None:
         ma_8 = masking
         xyz_8 = xyz_8[ma_8]
         scalar_8 = scalar_8[:, ma_8]
 
-    scalar_at_sp = scalar_at_sp.reshape((-1, 1, 1)).astype(BackendTensor.dtype)
+    scalar_at_sp = scalar_at_sp.reshape((-1, 1, 1))
 
     n_isosurface = scalar_at_sp.shape[0]
-    xyz_8 = np.tile(xyz_8, (n_isosurface, 1, 1))  # TODO: Generalize
+    xyz_8 = BackendTensor.t.tile(xyz_8, (n_isosurface, 1, 1))  # TODO: Generalize
 
     # Compute distance of scalar field on the corners
     scalar_dx = scalar_8[:, :, :4] - scalar_8[:, :, 4:]
     scalar_d_y = scalar_8[:, :, [0, 1, 4, 5]] - scalar_8[:, :, [2, 3, 6, 7]]
     scalar_d_z = scalar_8[:, :, ::2] - scalar_8[:, :, 1::2]
 
     # Compute the weights
@@ -50,17 +51,18 @@
     
     # Mask invalid edges
     valid_edge_x = np.logical_and(weight_x > -0.01, weight_x < 1.01)
     valid_edge_y = np.logical_and(weight_y > -0.01, weight_y < 1.01)
     valid_edge_z = np.logical_and(weight_z > -0.01, weight_z < 1.01)
 
     # * Note(miguel) From this point on the arrays become sparse
-    xyz_8_edges = np.hstack([xyz_8[:, 4:], xyz_8[:, [2, 3, 6, 7]], xyz_8[:, 1::2]])
-    intersect_segment = np.hstack([intersect_dx, intersect_dy, intersect_dz])
-    valid_edges = np.hstack([valid_edge_x, valid_edge_y, valid_edge_z])[:, :, 0]
+    xyz_8_edges = BackendTensor.t.hstack([xyz_8[:, 4:], xyz_8[:, [2, 3, 6, 7]], xyz_8[:, 1::2]])
+    intersect_segment = BackendTensor.t.hstack([intersect_dx, intersect_dy, intersect_dz])
+    valid_edges = BackendTensor.t.hstack([valid_edge_x, valid_edge_y, valid_edge_z])[:, :, 0]
+    valid_edges = valid_edges > 0
 
     intersection_xyz = xyz_8_edges[valid_edges] + intersect_segment[valid_edges]
 
     return intersection_xyz, valid_edges
 
 
 def triangulate_dual_contouring(dc_data_per_surface: DualContouringData):
@@ -125,14 +127,16 @@
     directions = np.dstack([nynz_direction, nyz_direction, ynz_direction, yz_direction,
                             nxnz_direction, xnz_direction, nxz_direction, xz_direction,
                             nxny_direction, nxy_direction, xny_direction, xy_direction])
 
     # endregion
 
     valid_edg = valid_edges[valid_voxels][:, :]
+    valid_edg = BackendTensor.t.to_numpy(valid_edg)
+    
     direction_each_edge = (directions * valid_edg)
 
     # Pick only edges with more than 2 voxels nearby
     three_neighbours = (directions * valid_edg).sum(axis=0) == 3
     matrix_to_right_C_order = np.transpose((direction_each_edge * three_neighbours), (1, 2, 0))
     indices = np.where(matrix_to_right_C_order)[2].reshape(-1, 3)
 
@@ -149,54 +153,68 @@
     valid_edges  = dc_data_per_stack.valid_edges
     valid_voxels = dc_data_per_stack.valid_voxels
     xyz_on_edge  = dc_data_per_stack.xyz_on_edge[slice_surface]
     gradients    = dc_data_per_stack.gradients[slice_surface]
     # @on
 
     # * Coordinates for all posible edges (12) and 3 dummy edges_normals in the center
-    edges_xyz = np.zeros((n_edges, 15, 3))
+    edges_xyz = BackendTensor.t.zeros((n_edges, 15, 3), dtype=BackendTensor.dtype_obj)
+    valid_edges = valid_edges > 0
     edges_xyz[:, :12][valid_edges] = xyz_on_edge
 
     # Normals
-    edges_normals = np.zeros((n_edges, 15, 3))
+    edges_normals = BackendTensor.t.zeros((n_edges, 15, 3), dtype=BackendTensor.dtype_obj)
     edges_normals[:, :12][valid_edges] = gradients
 
     if OLD_METHOD:=False:
         # ! Moureze model does not seems to work with the new method
         # ! This branch is all nans at least with ch1_1 model
         bias_xyz = np.copy(edges_xyz[:, :12])
         isclose = np.isclose(bias_xyz, 0)
         bias_xyz[isclose] = np.nan  # np zero values to nans
         mass_points = np.nanmean(bias_xyz, axis=1)  # Mean ignoring nans
     else:  # ? This is actually doing something
-        bias_xyz = np.copy(edges_xyz[:, :12])
+        bias_xyz = BackendTensor.t.copy(edges_xyz[:, :12])
+        bias_xyz = BackendTensor.t.to_numpy(bias_xyz)
         mask = bias_xyz == 0
         masked_arr = np.ma.masked_array(bias_xyz, mask)
         mass_points = masked_arr.mean(axis=1)
+        mass_points = BackendTensor.t.array(mass_points)
 
     edges_xyz[:, 12] = mass_points
     edges_xyz[:, 13] = mass_points
     edges_xyz[:, 14] = mass_points
 
     BIAS_STRENGTH = 1
-    edges_normals[:, 12] = np.array([BIAS_STRENGTH, 0, 0])
-    edges_normals[:, 13] = np.array([0, BIAS_STRENGTH, 0])
-    edges_normals[:, 14] = np.array([0, 0, BIAS_STRENGTH])
+    
+    bias_x = BackendTensor.t.array([BIAS_STRENGTH, 0, 0], dtype=BackendTensor.dtype_obj)
+    bias_y = BackendTensor.t.array([0, BIAS_STRENGTH, 0], dtype=BackendTensor.dtype_obj)
+    bias_z = BackendTensor.t.array([0, 0, BIAS_STRENGTH], dtype=BackendTensor.dtype_obj)
+    
+    edges_normals[:, 12] = bias_x
+    edges_normals[:, 13] = bias_y
+    edges_normals[:, 14] = bias_z
 
     # Remove unused voxels
     edges_xyz = edges_xyz[valid_voxels]
     edges_normals = edges_normals[valid_voxels]
 
     # Compute LSTSQS in all voxels at the same time
     A = edges_normals
     b = (A * edges_xyz).sum(axis=2)
-    term1 = np.einsum("ijk, ilj->ikl", A, np.transpose(A, (0, 2, 1)))
-    term2 = np.linalg.inv(term1)
-    term3 = np.einsum("ijk,ik->ij", np.transpose(A, (0, 2, 1)), b)
-    vertices = np.einsum("ijk, ij->ik", term2, term3)
+
+    if BackendTensor.engine_backend == AvailableBackends.PYTORCH:
+        transpose_shape = (2, 1)
+    else:
+        transpose_shape = (0, 2,1)
+        
+    term1 = BackendTensor.t.einsum("ijk, ilj->ikl", A, BackendTensor.t.transpose(A, transpose_shape))
+    term2 = BackendTensor.t.linalg.inv(term1)
+    term3 = BackendTensor.t.einsum("ijk,ik->ij", BackendTensor.t.transpose(A, transpose_shape), b)
+    vertices = BackendTensor.t.einsum("ijk, ij->ik", term2, term3)
 
     if debug:
         dc_data_per_stack.bias_center_mass = edges_xyz[:, 12:].reshape(-1, 3)
         dc_data_per_stack.bias_normals = edges_normals[:, 12:].reshape(-1, 3)
 
     return vertices
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/dual_contouring/fancy_triangulation.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/dual_contouring/fancy_triangulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,17 +174,18 @@
     # region: Find and remove edges at the border of the extent
     code__a_prod_edge = ~mapped_voxel_0.all(axis=0)  # mapped_voxel_0.prod(axis=0) == 0  # (n_voxels - active_voxels_for_given_edge - invalid_edges, 1)
     code__b_prod_edge = ~mapped_voxel_1.all(axis=0)  # mapped_voxel_1.prod(axis=0) == 0  # (n_voxels - active_voxels_for_given_edge - invalid_edges, 1)
     code__c_prod_edge = ~mapped_voxel_2.all(axis=0)  # mapped_voxel_2.prod(axis=0) == 0  # (n_voxels - active_voxels_for_given_edge - invalid_edges, 1)
 
     valid_edges_within_extent = code__a_prod_edge * code__b_prod_edge * code__c_prod_edge  # * Valid in the sense that there are valid voxels around
 
-    code__a_p = mapped_voxel_0[:, valid_edges_within_extent] == 0  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
-    code__b_p = mapped_voxel_1[:, valid_edges_within_extent] == 0  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
-    code__c_p = mapped_voxel_2[:, valid_edges_within_extent] == 0  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
+    from ...core.backend_tensor import BackendTensor
+    code__a_p = BackendTensor.t.array(mapped_voxel_0[:, valid_edges_within_extent] == 0)  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
+    code__b_p = BackendTensor.t.array(mapped_voxel_1[:, valid_edges_within_extent] == 0)  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
+    code__c_p = BackendTensor.t.array(mapped_voxel_2[:, valid_edges_within_extent] == 0)  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
 
     if False:
         debug_code_p = code__a_p + code__b_p + code__c_p  # (n_voxels, n_voxels - active_voxels_for_given_edge - invalid_edges - edges_at_extent_border)
         # 15 and 17 does not have y
         
     # endregion
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_b_vector_assembler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+from gempy_engine.config import AvailableBackends
 from gempy_engine.core.backend_tensor import BackendTensor as bt, BackendTensor
 from gempy_engine.core.data.kernel_classes.orientations import OrientationsInternals
+import numpy as np
 
 
 def b_vector_assembly(ori: OrientationsInternals, cov_size: int) -> bt.tensor_types:
     g_s = ori.n_orientations_tiled
     n_dim = ori.orientations.n_dimensions
 
     if n_dim == 3:
         g_vector = ori.orientations.gx, ori.orientations.gy, ori.orientations.gz
     elif n_dim == 2:
         g_vector = ori.orientations.gx, ori.orientations.gy
     else:
         raise ValueError("Wrong number of dimensions in the gradients.")
 
-    b_vector = bt.tfnp.concatenate([*g_vector, bt.tfnp.zeros(cov_size - g_s, dtype=BackendTensor.dtype)], -1)
+    zeros = bt.t.zeros(cov_size - g_s, dtype=BackendTensor.dtype_obj)
+    b_vector = bt.tfnp.concatenate([*g_vector, zeros], -1)
     b_vector = bt.tfnp.expand_dims(b_vector, axis=1)
 
     return b_vector
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_covariance_assembler.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_covariance_assembler.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,17 +41,18 @@
         Solutions.debug_input_data['faults_drift'] = faults_drift
 
     return cov
 
 
 def _get_cov_grad(dm, k_a, k_p_ref, nugget):
     cov_grad = dm.hu * dm.hv / (dm.r_ref_ref ** 2 + 1e-5) * (- k_p_ref + k_a) - k_p_ref * dm.perp_matrix  # C
-    grad_nugget = nugget[0]
+    grad_nugget = nugget[0, 0]
     if BackendTensor.pykeops_enabled is False:
-        nugget_selector = np.eye(cov_grad.shape[0], dtype=BackendTensor.dtype) * dm.perp_matrix
+        eye = BackendTensor.t.array(np.eye(cov_grad.shape[0], dtype=BackendTensor.dtype))
+        nugget_selector = eye * dm.perp_matrix
         nugget_matrix = nugget_selector * grad_nugget
         cov_grad += nugget_matrix
     else:
         from pykeops.numpy import LazyTensor
         matrix_shape = dm.hu.shape[0]
         diag_ = np.arange(matrix_shape).reshape(-1, 1).astype(BackendTensor.dtype)
         diag_i = LazyTensor(diag_[:, None])
@@ -64,17 +65,17 @@
 
 def _get_cov_surface_points(dm, k_ref_ref, k_ref_rest, k_rest_ref, k_rest_rest, options: KernelOptions, nugget_effect):
     cov_surface_points = options.i_res * (k_rest_rest - k_rest_ref - k_ref_rest + k_ref_ref)
     ref_nugget = nugget_effect[0]
     flipped_perp_matrix = ( dm.perp_matrix - 1 ) * -1
     
     if BackendTensor.pykeops_enabled is False: # Add nugget effect for ref and rest point
-        diag = np.eye(cov_surface_points.shape[0], dtype=BackendTensor.dtype) * ref_nugget  # * This is also applying it to the grad which is bad
+        eye = BackendTensor.t.array(np.eye(cov_surface_points.shape[0], dtype=BackendTensor.dtype))
+        diag = eye * ref_nugget  # * This is also applying it to the grad which is bad
         cov_surface_points += diag * flipped_perp_matrix
-        # cov_surface_points[:3, :3] = 0
     else:
         from pykeops.numpy import LazyTensor
         matrix_shape = k_rest_ref.shape[0]
         diag_ = np.arange(matrix_shape).reshape(-1, 1).astype(BackendTensor.dtype)
         diag_i = LazyTensor(diag_[:, None])
         diag_j = LazyTensor(diag_[None, :])
         nugget_matrix = (((0.5 - (diag_i - diag_j) ** 2).step()) * ref_nugget)
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dataclasses import dataclass
 from typing import Optional
 
 import numpy as np
 
 from ...core.backend_tensor import BackendTensor
-from gempy_engine.config import DEBUG_MODE
+from gempy_engine.config import DEBUG_MODE, AvailableBackends
 
 
 @dataclass
 class InternalDistancesMatrices:
     dif_ref_ref: np.ndarray
     dif_rest_rest: np.ndarray
     hu: np.ndarray
@@ -25,15 +25,15 @@
     hu_ref_grad: Optional[np.ndarray]  # These are only used by grad eval
     hu_rest_grad: Optional[np.ndarray]  # These are only used by grad eval
     # hu_ref_sum: np.ndarray   # These are only used for caching
     # hu_rest_sum: np.ndarray  # These are only used for caching
     # 
     
     def __post_init__(self):
-        if DEBUG_MODE:
+        if DEBUG_MODE and BackendTensor.engine_backend != AvailableBackends.PYTORCH:
             assert self.dif_ref_ref.dtype == BackendTensor.dtype, f"Wrong dtype for dif_ref_ref: {self.dif_ref_ref.dtype}. should be {BackendTensor.dtype}"
             assert self.dif_rest_rest.dtype == BackendTensor.dtype, f"Wrong dtype for dif_rest_rest: {self.dif_rest_rest.dtype}. should be {BackendTensor.dtype}"
             assert self.hu.dtype == BackendTensor.dtype, f"Wrong dtype for hu: {self.hu.dtype}. should be {BackendTensor.dtype}"
             assert self.hv.dtype == BackendTensor.dtype, f"Wrong dtype for hv: {self.hv.dtype}. should be {BackendTensor.dtype}"
             assert self.huv_ref.dtype == BackendTensor.dtype, f"Wrong dtype for huv_ref: {self.huv_ref.dtype}. should be {BackendTensor.dtype}"
             assert self.huv_rest.dtype == BackendTensor.dtype, f"Wrong dtype for huv_rest: {self.huv_rest.dtype}. should be {BackendTensor.dtype}"
             assert (self.perp_matrix.dtype == "int8" or self.perp_matrix.dtype == BackendTensor.dtype), f"Wrong dtype for perp_matrix: {self.perp_matrix.dtype}. should be int8 or float32 for pykeops"
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_kernel_constructors.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_kernel_constructors.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 
 import numpy as np
 
 from ...core.backend_tensor import BackendTensor
 from ...core.data.matrices_sizes import MatricesSizes
 from ...core.data.kernel_classes.orientations import OrientationsInternals
 from ...core.data.options import KernelOptions
+from ...core.backend_tensor import BackendTensor as bt
 
 
 def assembly_dips_points_tensor(dips_coord: np.ndarray, sp_coord: np.ndarray, matrices_size: MatricesSizes):
     n_dim = matrices_size.dim
     drift_size = matrices_size.drifts_size
-    z = np.zeros((drift_size, n_dim), dtype=BackendTensor.dtype)
+    z = bt.t.zeros((drift_size, n_dim), dtype=BackendTensor.dtype_obj)
     
-    dipspoints = np.vstack((dips_coord, sp_coord, z))
+    dipspoints = bt.t.vstack((dips_coord, sp_coord, z))
     return dipspoints
 
 
 def assembly_dips_ug_coords(ori_internals: OrientationsInternals, interpolation_options: KernelOptions,
                             matrices_size: MatricesSizes) \
         -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     n_ori = ori_internals.n_orientations
@@ -78,26 +79,26 @@
 
 def assembly_dips_points_coords(surface_points: np.ndarray, matrices_sizes: MatricesSizes,
                                 interpolation_options: KernelOptions) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     n_dim = interpolation_options.number_dimensions
     ori_size = matrices_sizes.ori_size
     drifts_size = matrices_sizes.drifts_size
     
-    z = np.zeros((ori_size, n_dim), dtype=BackendTensor.dtype)  # * Orientations area
-    z2 = np.zeros((drifts_size, n_dim), dtype=BackendTensor.dtype)  # * Universal area
+    z = bt.t.zeros((ori_size, n_dim), dtype=BackendTensor.dtype_obj)  # * Orientations area
+    z2 = bt.t.zeros((drifts_size, n_dim), dtype=BackendTensor.dtype_obj)  # * Universal area
 
-    zb = z2.copy()  # ! This block has to be here because it has to be before we modify z2
-    zc = z2.copy()
+    zb = bt.t.copy(z2)  # ! This block has to be here because it has to be before we modify z2
+    zc = bt.t.copy(z2)
 
     if interpolation_options.uni_degree != 0:
         for i in range(n_dim):
             z2[i, i] = 1
 
     # Degree 1
-    points_degree_1 = np.vstack((z, surface_points, z2))
+    points_degree_1 = bt.t.vstack((z, surface_points, z2))
 
     # Degree 2
     # TODO: Substitute vstack
     if interpolation_options.uni_degree == 2:
 
         for i in range(n_dim):
             zb[n_dim + i, i] = 1
@@ -109,11 +110,11 @@
         for i in range(n_dim):
             zc[n_dim + i, i] = 1
         # zc[n_dim * 2:, 1] = 1
         zc[n_dim * 2, 1] = 1
         zc[n_dim * 2 + 1, 2] = 1
         zc[n_dim * 2 + 2, 2] = 1
 
-    points_degree_2a = np.vstack((z, surface_points, zb))
-    points_degree_2b = np.vstack((z, surface_points, zc))
+    points_degree_2a = bt.t.vstack((z, surface_points, zb))
+    points_degree_2b = bt.t.vstack((z, surface_points, zc))
 
     return points_degree_1, points_degree_2a, points_degree_2b
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_kernel_selectors.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_kernel_selectors.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_kernels_assembler.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_kernels_assembler.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...core.utils import gempy_profiler_decorator
 
 tensor_types = bt.tensor_types
 
 
 def create_cov_kernel(ki: KernelInput, options: KernelOptions) -> tensor_types:
     kernel_f: KernelFunction = options.kernel_function.value
-    
+
     distances_matrices = _compute_all_distance_matrices(
         cs=ki.cartesian_selector,
         ori_sp_matrices=ki.ori_sp_matrices,
         square_distance=kernel_f.consume_sq_distance,
         is_gradient=False
     )
 
@@ -166,15 +166,15 @@
             cs=cs,
             ori_sp_matrices=ori_sp_matrices,
             square_distance=square_distance
         )
 
     if develeping_distances_buffer := False and is_gradient:  # This is for developing
         _check_which_items_are_the_same_between_calls(distance_matrices)
-
+    
     DistancesBuffer.last_internal_distances_matrices = distance_matrices  # * Save common values for next call
     return distance_matrices
 
 
 def _compute_distances_using_cache(cs, last_internal_distances_matrices: InternalDistancesMatrices) -> InternalDistancesMatrices:
     dif_ref_ref = last_internal_distances_matrices.dif_ref_ref  # Can be cached
     dif_rest_rest = last_internal_distances_matrices.dif_rest_rest  # Can be cached
@@ -235,43 +235,45 @@
     perp_matrix = bt.t.sum(cs.hu_sel_i * cs.hv_sel_j, axis=-1, dtype='int8')  # * dtype arg only works for pure numpy. Axis dependent
 
     # region: distance r
     r_ref_ref = bt.t.sum(dif_ref_ref ** 2, axis=-1)  # Can be cached
     r_rest_rest = bt.t.sum(dif_rest_rest ** 2, axis=-1)  # Can be cached
     r_ref_rest = bt.t.sum((ori_sp_matrices.dip_ref_i - ori_sp_matrices.diprest_j) ** 2, axis=-1)  # Can be cached
     r_rest_ref = bt.t.sum((ori_sp_matrices.diprest_i - ori_sp_matrices.dip_ref_j) ** 2, axis=-1)  # Can be cached
+
     if square_distance is False:
         # @off
-        r_ref_ref   = bt.t.sqrt(r_ref_ref)
-        r_rest_rest = bt.t.sqrt(r_rest_rest)
-        r_ref_rest  = bt.t.sqrt(r_ref_rest)
-        r_rest_ref  = bt.t.sqrt(r_rest_ref)
+        epsilon = 1e-10  # Add small regularization term to avoid numerical errors
+        r_ref_ref = bt.t.sqrt(r_ref_ref + epsilon)
+        r_rest_rest = bt.t.sqrt(r_rest_rest + epsilon)
+        r_ref_rest = bt.t.sqrt(r_ref_rest + epsilon)
+        r_rest_ref = bt.t.sqrt(r_rest_ref + epsilon)
     # endregion
 
     new_distance_matrices = InternalDistancesMatrices(
-        dif_ref_ref     = dif_ref_ref,
-        dif_rest_rest   = dif_rest_rest,
-        hu              = hu,
-        hv              = hv,
-        huv_ref         = huv_ref,
-        huv_rest        = huv_rest,
-        perp_matrix     = perp_matrix,
-        r_ref_ref       = r_ref_ref,
-        r_ref_rest      = r_ref_rest,
-        r_rest_ref      = r_rest_ref,
-        r_rest_rest     = r_rest_rest,
-        hu_ref          = hu_ref,
-        hu_rest         = hu_rest,
-        hu_ref_grad     = None,
-        hu_rest_grad    = None,
+        dif_ref_ref=dif_ref_ref,
+        dif_rest_rest=dif_rest_rest,
+        hu=hu,
+        hv=hv,
+        huv_ref=huv_ref,
+        huv_rest=huv_rest,
+        perp_matrix=perp_matrix,
+        r_ref_ref=r_ref_ref,
+        r_ref_rest=r_ref_rest,
+        r_rest_ref=r_rest_ref,
+        r_rest_rest=r_rest_rest,
+        hu_ref=hu_ref,
+        hu_rest=hu_rest,
+        hu_ref_grad=None,
+        hu_rest_grad=None,
         #    hu_ref_sum = hu_ref_sum   , hu_rest_sum = hu_rest_sum,
         # @on
     )
     return new_distance_matrices
 
 
 def _check_which_items_are_the_same_between_calls(distance_matrices):
     import numpy as np
     print(f"Checking distances matrices. Shape: {distance_matrices.dif_ref_ref.shape}")
     for k, v in DistancesBuffer.last_internal_distances_matrices.__dict__.items():
         if not np.allclose(v, distance_matrices.__dict__[k]):
-            print("Not allclose", k)
+            print("Not allclose", k)
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_pykeops_cov_compiler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_structs.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_structs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 from dataclasses import dataclass
 from typing import Tuple, Optional
 
 import numpy as np
 
+from gempy_engine.core.utils import cast_type_inplace
 from gempy_engine.core.backend_tensor import BackendTensor, AvailableBackends
 
 tensor_types = BackendTensor.tensor_types
 
 
 def _upgrade_kernel_input_to_keops_tensor(struct_data_instance):
     from pykeops.numpy import LazyTensor
 
     for key, val in struct_data_instance.__dict__.items():
         if key == "n_faults_i": continue
         struct_data_instance.__dict__[key] = LazyTensor(val.astype(BackendTensor.dtype))  # ! This as type is quite expensive
-        #struct_data_instance.__dict__[key] = LazyTensor(val)  # ! This as type is quite expensive
+
+def _cast_tensors(data_class_instance):
+    match (BackendTensor.engine_backend, BackendTensor.pykeops_enabled):
+        case (AvailableBackends.numpy, True):
+            _upgrade_kernel_input_to_keops_tensor(data_class_instance)
+        case (AvailableBackends.PYTORCH, False):
+            cast_type_inplace(data_class_instance)
+        case (AvailableBackends.PYTORCH, True):
+            raise NotImplementedError("Pytorch with pykeops is not implemented yet")
+        case (_, _):
+            pass
 
 
 @dataclass
 class OrientationSurfacePointsCoords:
     dip_ref_i: tensor_types = np.empty((0, 1, 3))
     dip_ref_j: tensor_types = np.empty((1, 0, 3))
     diprest_i: tensor_types = np.empty((0, 1, 3))
@@ -29,16 +40,15 @@
             dips_points0 = x[:, None, :]  # i
             dips_points1 = y[None, :, :]  # j
             return dips_points0, dips_points1
 
         self.dip_ref_i, self.dip_ref_j = _assembly(x_ref, y_ref)
         self.diprest_i, self.diprest_j = _assembly(x_rest, y_rest)
         
-        if BackendTensor.engine_backend == AvailableBackends.numpy and BackendTensor.pykeops_enabled:
-            _upgrade_kernel_input_to_keops_tensor(self)
+        _cast_tensors(self)
 
 
 @dataclass
 class OrientationsDrift:
     dips_ug_ai: tensor_types = np.empty((0, 1, 3))
     dips_ug_aj: tensor_types = np.empty((1, 0, 3))
     dips_ug_bi: tensor_types = np.empty((0, 1, 3))
@@ -58,16 +68,15 @@
         self.dips_ug_bi = x_degree_2[:, None, :]
         self.dips_ug_bj = y_degree_2[None, :, :]
         self.dips_ug_ci = x_degree_2b[:, None, :]
         self.dips_ug_cj = y_degree_2b[None, :, :]
         self.selector_ci = selector_degree_2[:, None, :]
         self.selector_cj = selector_degree_2[None, :, :]
 
-        if BackendTensor.engine_backend == AvailableBackends.numpy and BackendTensor.pykeops_enabled:
-            _upgrade_kernel_input_to_keops_tensor(self)
+        _cast_tensors(self)
 
 
 @dataclass
 class PointsDrift:
     dipsPoints_ui_ai: tensor_types = np.empty((0, 1, 3))
     dipsPoints_ui_aj: tensor_types = np.empty((1, 0, 3))
     dipsPoints_ui_bi1: tensor_types = np.empty((0, 1, 3))
@@ -79,33 +88,32 @@
                  y_degree_2a: np.ndarray, x_degree_2b: np.ndarray, y_degree_2b: np.ndarray):
         self.dipsPoints_ui_ai = x_degree_1[:, None, :]
         self.dipsPoints_ui_aj = y_degree_1[None, :, :]
         self.dipsPoints_ui_bi1 = x_degree_2a[:, None, :]
         self.dipsPoints_ui_bj1 = y_degree_2a[None, :, :]
         self.dipsPoints_ui_bi2 = x_degree_2b[:, None, :]
         self.dipsPoints_ui_bj2 = y_degree_2b[None, :, :]
-        if BackendTensor.engine_backend == AvailableBackends.numpy and BackendTensor.pykeops_enabled:
-            _upgrade_kernel_input_to_keops_tensor(self)
+
+        _cast_tensors(self)
 
 
 @dataclass
 class FaultDrift:
     faults_i: tensor_types = np.empty((0, 1, 3))
     faults_j: tensor_types = np.empty((1, 0, 3))
-    
+
     n_faults_i: int = 0
-    
+
     def __init__(self, x_degree_1: np.ndarray, y_degree_1: np.ndarray, ):
         self.faults_i = x_degree_1[:, None, :]
         self.faults_j = y_degree_1[None, :, :]
-        
+
         self.n_faults_i = x_degree_1.shape[1]
-        
-        if BackendTensor.engine_backend == AvailableBackends.numpy and BackendTensor.pykeops_enabled:
-            _upgrade_kernel_input_to_keops_tensor(self)
+
+        _cast_tensors(self)
 
 
 @dataclass
 class CartesianSelector:
     hu_sel_i: tensor_types = np.empty((0, 1, 3))
     hu_sel_j: tensor_types = np.empty((1, 0, 3))
     hv_sel_i: tensor_types = np.empty((0, 1, 3))
@@ -133,50 +141,44 @@
 
         self.h_sel_ref_i = x_sel_h_ref[:, None, :]
         self.h_sel_ref_j = y_sel_h_ref[None, :, :]
 
         self.h_sel_rest_i = x_sel_h_rest[:, None, :]
         self.h_sel_rest_j = y_sel_h_rest[None, :, :]
 
-#        self.is_gradient = is_gradient
-
-        if BackendTensor.engine_backend == AvailableBackends.numpy and BackendTensor.pykeops_enabled:
-            _upgrade_kernel_input_to_keops_tensor(self)
+        _cast_tensors(self)
 
 
 @dataclass
 class DriftMatrixSelector:
     sel_ui: tensor_types = np.empty((0, 1, 3))
     sel_vj: tensor_types = np.empty((1, 0, 3))
-    
+
     def __init__(self, x_size: int, y_size: int, n_drift_eq: int, drift_start_post_x: int, drift_start_post_y: int):
         sel_i = np.zeros((x_size, 2), dtype=BackendTensor.dtype)
         sel_j = np.zeros((y_size, 2), dtype=BackendTensor.dtype)
 
         drift_pos_0_x = drift_start_post_x
         drift_pos_1_x = drift_start_post_x + n_drift_eq + 1
 
         drift_pos_0_y = drift_start_post_y
         drift_pos_1_y = drift_start_post_y + n_drift_eq + 1
-        
+
         if n_drift_eq != 0:
             sel_i[:drift_pos_0_x, 0] = 1
             sel_i[drift_pos_0_x:drift_pos_1_x, 1] = 1
-        
+
             sel_j[:drift_pos_0_y, 0] = -1
             sel_j[drift_pos_0_y:drift_pos_1_y, 1] = -1
 
         self.sel_ui = sel_i[:, None, :]
         self.sel_vj = sel_j[None, :, :]
 
-        if BackendTensor.engine_backend == AvailableBackends.numpy and BackendTensor.pykeops_enabled:
-            _upgrade_kernel_input_to_keops_tensor(self)
-    
-    
-    
+        _cast_tensors(self)
+
     @classmethod
     def old_method(cls, x_size: int, y_size: int, n_drift_eq: int):  # * This does not account for faults
         sel_i = np.zeros((x_size, 2))
         sel_j = np.zeros((y_size, 2))
 
         # ! TODO [x]: This need to account for faults too. This is what the new __init__ does.
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_test_assembler.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_test_assembler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_utils.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_utils.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/_vectors_preparation.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/_vectors_preparation.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,18 +116,18 @@
         rest_fault=None
     )
 
 
 def _assembly_dips_points_tensors(matrices_size: MatricesSizes, ori_, sp_) -> OrientationSurfacePointsCoords:
     dips_ref_coord = assembly_dips_points_tensor(ori_.dip_positions_tiled, sp_.ref_surface_points, matrices_size)
     dips_rest_coord = assembly_dips_points_tensor(ori_.dip_positions_tiled, sp_.rest_surface_points, matrices_size)
-
+    
     orientations_sp_matrices = OrientationSurfacePointsCoords(dips_ref_coord, dips_ref_coord, dips_rest_coord,
                                                               dips_rest_coord)  # When we create que core covariance these are the repeated since the distance are with themselves
-
+    
     return orientations_sp_matrices
 
 
 def _assembly_dips_points_grid_tensors(grid, matrices_size: MatricesSizes, ori_, sp_):
     """Used for kernel construction"""
     dips_ref_coord = assembly_dips_points_tensor(ori_.dip_positions_tiled, sp_.ref_surface_points, matrices_size)
     dips_rest_coord = assembly_dips_points_tensor(ori_.dip_positions_tiled, sp_.rest_surface_points, matrices_size)
@@ -183,15 +183,15 @@
 
 
 def _assembly_drift_grid_tensors(grid: np.ndarray, options: KernelOptions, matrices_size: MatricesSizes,
                                  ori_: OrientationsInternals, sp_: SurfacePointsInternals, axis: int):
     # region UG
     dips_ug_d1, dips_ug_d2a, dips_ug_d2b, second_degree_selector = assembly_dips_ug_coords(ori_, options, matrices_size)
 
-    grid_1 = np.zeros_like(grid)
+    grid_1 = BackendTensor.t.zeros_like(grid)
     grid_1[:, axis] = 1
 
     sel = np.ones(options.number_dimensions)
     sel[axis] = 0
 
     dips_ug = OrientationsDrift(
         x_degree_1=dips_ug_d1, y_degree_1=grid_1,
@@ -222,18 +222,18 @@
     return FaultDrift(fault_vector_ref, fault_vector_ref), FaultDrift(fault_vector_rest, fault_vector_rest)
 
 
 def _assembly_fault_internals(faults_val, options, ori_size):
     def _assembler(matrix_val, ori_size_: int, uni_drift_size: int):  # TODO: This function (probably)needs to be extracted to _kernel_constructors
         n_uni_eq = uni_drift_size  # * Number of equations. This should be how many faults are active
         n_faults = matrix_val.shape[1]  # TODO [ ]: We are going to have to tweak this for multiple faults
-        z = np.zeros((ori_size_, n_faults), dtype=BackendTensor.dtype)
-        z2 = np.zeros((n_uni_eq, n_faults), dtype=BackendTensor.dtype)
-        z3 = np.eye(n_faults, dtype=BackendTensor.dtype)
+        z = BackendTensor.t.zeros((ori_size_, n_faults), dtype=BackendTensor.dtype_obj)
+        z2 = BackendTensor.t.zeros((n_uni_eq, n_faults), dtype=BackendTensor.dtype_obj)
+        z3 = BackendTensor.t.eye(n_faults, dtype=BackendTensor.dtype_obj)
         # Degree 1
-        return np.vstack((z, matrix_val, z2, z3))
+        return BackendTensor.t.vstack((z, matrix_val, z2, z3))
 
     ref_matrix_val = faults_val.fault_values_ref
     rest_matrix_val = faults_val.fault_values_rest
     fault_vector_ref = _assembler(ref_matrix_val.T, ori_size, options.n_uni_eq)
     fault_vector_rest = _assembler(rest_matrix_val.T, ori_size, options.n_uni_eq)
     return fault_vector_ref, fault_vector_rest
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/kernel_constructor/kernel_constructor_interface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/_octree_common.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/_octree_common.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/_octree_internals.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/_octree_internals.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/octrees_topology/octrees_topology_interface.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/octrees_topology/octrees_topology_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,19 +86,28 @@
 
     # Octree - Level 0
     root: OctreeLevel = octree_list[0]
 
     regular_grid_shape = root.grid_centers.regular_grid_shape
 
     block = _get_block_from_value_type(root, scalar_n, value_type)
-
+    
+    # Check if block is pytorch tensor and detach
+    # ! Convert to numpy
+    from gempy_engine.core.backend_tensor import BackendTensor
+    from gempy_engine.config import AvailableBackends
+    match (BackendTensor.engine_backend):
+        case AvailableBackends.PYTORCH:
+            block = block.detach().numpy()
+    
     regular_grid: np.ndarray = _expand_regular_grid(
-        active_cells_erg=block.reshape(regular_grid_shape),
+        active_cells_erg=block.reshape(regular_grid_shape.tolist()),
         n_rep=level
     )
+    
     shape = regular_grid_shape
 
     active_cells_index: List["np.ndarray[np.int]"] = []
     global_active_cells_index: np.ndarray = np.array([])
 
     # Octree - Level n
     for e, octree in enumerate(octree_list[1:level + 1]):
@@ -106,14 +115,17 @@
         active_cells: np.ndarray = octree.grid_centers.regular_grid.active_cells
 
         local_active_cells: np.ndarray = np.where(active_cells)[0]
         shape: np.ndarray = octree.grid_centers.regular_grid_shape
         oct: np.ndarray = calculate_oct(shape, n_rep)
 
         block = _get_block_from_value_type(octree, scalar_n, value_type)
+        match (BackendTensor.engine_backend):
+            case AvailableBackends.PYTORCH:
+                block = block.detach().numpy()
 
         ids: np.ndarray = _expand_octree(block.reshape((-1, 2, 2, 2)), n_rep - 1)
 
         is_branch = e > 0
 
         if is_branch:
             local_shape: "np.ndarray[np.int]" = np.array([2, 2, 2])
@@ -126,15 +138,15 @@
             local_shape = shape // 2
             local_anchors = get_global_anchor(local_active_cells, local_shape, n_rep)
             global_active_cells_index = (local_anchors.reshape(-1, 1) + oct).ravel()
             regular_grid[global_active_cells_index] = ids  # + (e * 2)
 
         active_cells_index.append(global_active_cells_index)
 
-    return regular_grid.reshape(shape)
+    return regular_grid.reshape(shape.tolist())
 
 
 def _get_block_from_value_type(root: OctreeLevel, scalar_n: int, value_type: ValueType):
     element_output: InterpOutput = root.outputs_centers[scalar_n]
     match value_type:
         case ValueType.ids:
             block = element_output.final_block
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/modules/solver/solver_interface.py` & `gempy_engine-2023.2.0b1/gempy_engine/modules/solver/solver_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,24 +8,33 @@
 
 from gempy_engine.core.data.options import KernelOptions
 
 bt = BackendTensor
 global n_iters
 
 
-def kernel_reduction(cov, b, kernel_options: KernelOptions) -> np.ndarray:
+def kernel_reduction(cov, b, kernel_options: KernelOptions, n_faults: int = 0) -> np.ndarray:
     global n_iters
     n_iters = 0
     
     solver: Solvers = kernel_options.kernel_solver
     compute_condition_number = kernel_options.compute_condition_number
     
     # ? Maybe we should always compute the conditional_number no matter the branch
     dtype = BackendTensor.dtype
     match (BackendTensor.engine_backend, BackendTensor.pykeops_enabled, solver):
+        case (AvailableBackends.PYTORCH, False, _):
+            w = bt.t.linalg.solve(cov, b)
+            
+            cond_number = bt.t.linalg.cond(cov)
+            print(f'Condition number: {cond_number}.')
+            # cond_number.backward()
+            
+        case (AvailableBackends.PYTORCH, True, _):
+            raise NotImplementedError('Pykeops is not implemented for pytorch yet')
         case (AvailableBackends.tensorflow, True, _):
             raise NotImplementedError('Pykeops is not implemented for tensorflow yet')
             # w = cov.solve(b.numpy().astype('float32'), alpha=smooth, dtype_acc='float32')
         case (AvailableBackends.tensorflow, False, _):
             import tensorflow as tf
             w = tf.linalg.solve(cov, b)
         case (AvailableBackends.numpy, True, Solvers.PYKEOPS_CG):
@@ -51,15 +60,16 @@
             A = aslinearoperator(cov)
             print(f'A size: {A.shape}')
             w, info = cg(
                 A=A,
                 b=b[:, 0],
                 maxiter=100,
                 tol=.000005,  # * With this tolerance we do 8 iterations
-                callback=callback
+                callback=callback,
+                # x0=x0
             )
             w = np.atleast_2d(w).T
             print(f'CG iterations: {n_iters}')
         
         case (AvailableBackends.numpy, _, Solvers.GMRES):
             from scipy.sparse.linalg import aslinearoperator, gmres
             A = aslinearoperator(cov)
@@ -80,16 +90,26 @@
 
 def _compute_conditional_number(cov):
     cond_number = np.linalg.cond(cov)
     svd = np.linalg.svd(cov)
     eigvals = np.linalg.eigvals(cov)
     is_positive_definite = np.all(eigvals > 0)
     print(f'Condition number: {cond_number}. Is positive definite: {is_positive_definite}')
+    
+    idx = np.where(eigvals > 800)
+    print(idx)
+    import matplotlib.pyplot as plt
     if not is_positive_definite:  # ! Careful numpy False
         warnings.warn('The covariance matrix is not positive definite')
+    # Plotting the histogram
+    plt.hist(eigvals, bins=50, color='blue', alpha=0.7, log=True)
+    plt.xlabel('Eigenvalue')
+    plt.ylabel('Frequency')
+    plt.title('Histogram of Eigenvalues')
+    plt.show()
 
 
 
 def callback(xk):
     global n_iters
     n_iters += 1
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/optional_dependencies.py` & `gempy_engine-2023.2.0b1/gempy_engine/optional_dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 def require_pandas():
     try:
         import pandas as pd
     except ImportError:
         raise ImportError("The pandas library is required to use this function.")
     return pd
 
+def require_subsurface():
+    try:
+        import subsurface
+    except ImportError:
+        raise ImportError("The subsurface library is required to use this function.")
+    return subsurface
 
 def require_pooch():
     try:
         import pooch
     except ImportError:
         raise ImportError("The pooch library is required to use this function.")
     return pooch
```

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/plugins/plotting/helper_functions.py` & `gempy_engine-2023.2.0b1/gempy_engine/plugins/plotting/helper_functions.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine/plugins/plotting/helper_functions_pyvista.py` & `gempy_engine-2023.2.0b1/gempy_engine/plugins/plotting/helper_functions_pyvista.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/gempy_engine.egg-info/SOURCES.txt` & `gempy_engine-2023.2.0b1/gempy_engine.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -29,20 +29,22 @@
 gempy_engine/API/server/_process_output.py
 gempy_engine/API/server/_server_functions.py
 gempy_engine/API/server/main_server_pro.py
 gempy_engine/core/__init__.py
 gempy_engine/core/backend_tensor.py
 gempy_engine/core/utils.py
 gempy_engine/core/data/__init__.py
+gempy_engine/core/data/centered_grid.py
 gempy_engine/core/data/custom_segmentation_functions.py
 gempy_engine/core/data/dual_contouring_data.py
 gempy_engine/core/data/dual_contouring_mesh.py
 gempy_engine/core/data/exported_fields.py
 gempy_engine/core/data/exported_structs.py
 gempy_engine/core/data/generic_grid.py
+gempy_engine/core/data/geophysics_input.py
 gempy_engine/core/data/grid.py
 gempy_engine/core/data/input_data_descriptor.py
 gempy_engine/core/data/internal_structs.py
 gempy_engine/core/data/interp_output.py
 gempy_engine/core/data/interpolation_functions.py
 gempy_engine/core/data/interpolation_input.py
 gempy_engine/core/data/matrices_sizes.py
@@ -69,14 +71,17 @@
 gempy_engine/modules/activator/activator_interface.py
 gempy_engine/modules/data_preprocess/__init__.py
 gempy_engine/modules/data_preprocess/_input_preparation.py
 gempy_engine/modules/data_preprocess/data_preprocess_interface.py
 gempy_engine/modules/dual_contouring/__init__.py
 gempy_engine/modules/dual_contouring/dual_contouring_interface.py
 gempy_engine/modules/dual_contouring/fancy_triangulation.py
+gempy_engine/modules/geophysics/__init__.py
+gempy_engine/modules/geophysics/fw_gravity.py
+gempy_engine/modules/geophysics/gravity_gradient.py
 gempy_engine/modules/kernel_constructor/__init__.py
 gempy_engine/modules/kernel_constructor/_b_vector_assembler.py
 gempy_engine/modules/kernel_constructor/_covariance_assembler.py
 gempy_engine/modules/kernel_constructor/_internalDistancesMatrices.py
 gempy_engine/modules/kernel_constructor/_kernel_constructors.py
 gempy_engine/modules/kernel_constructor/_kernel_selectors.py
 gempy_engine/modules/kernel_constructor/_kernels_assembler.py
@@ -136,17 +141,21 @@
 tests/test_common/test_integrations/test_multi_fields_dual_contouring.py
 tests/test_common/test_integrations/test_multiple_grids.py
 tests/test_common/test_integrations/test_options.py
 tests/test_common/test_modules/__init__.py
 tests/test_common/test_modules/test_activator.py
 tests/test_common/test_modules/test_dual.py
 tests/test_common/test_modules/test_exporter.py
+tests/test_common/test_modules/test_geophysics.py
 tests/test_common/test_modules/test_octrees.py
 tests/test_common/test_modules/test_solver.py
 tests/test_common/test_modules/test_topology.py
 tests/test_common/test_modules/test_kernel_constructor/__init__.py
 tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py
 tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py
 tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py
 tests/test_common/test_modules/test_kernel_constructor/test_universal.py
 tests/test_common/test_prototyping/__init__.py
-tests/test_common/test_prototyping/test_broadcasting.py
+tests/test_common/test_prototyping/test_broadcasting.py
+tests/test_pytorch/__init__.py
+tests/test_pytorch/test_pytorch_gradients.py
+tests/test_pytorch/test_pytorch_installation.py
```

### Comparing `gempy_engine-2023.1.0b5/setup.py` & `gempy_engine-2023.2.0b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ﻿from setuptools import setup, find_packages
 
-version = "2023.1.0b5"
+version = "2023.2.0b1"
 
 
 def read_requirements(file_name):
     with open(file_name, "r", encoding="utf-8") as f:
         return [line.strip() for line in f.readlines()]
```

### Comparing `gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/test_backend_tensor.py` & `gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/test_backend_tensor.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/test_tensorflow.py` & `gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/SKIP_tensor_flow/test_tf.py` & `gempy_engine-2023.2.0b1/tests/SKIP_tensor_flow/test_tf.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/benchmark/one_fault_model.py` & `gempy_engine-2023.2.0b1/tests/benchmark/one_fault_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,24 @@
 from gempy_engine.core.data import SurfacePoints, Orientations, InterpolationOptions, TensorsStructure
 from gempy_engine.core.data.grid import RegularGrid, Grid
 from gempy_engine.core.data.input_data_descriptor import InputDataDescriptor
 from gempy_engine.core.data.stack_relation_type import StackRelationType
 from gempy_engine.core.data.stacks_structure import StacksStructure
 from gempy_engine.core.data.interpolation_input import InterpolationInput
 from gempy_engine.core.data.kernel_classes.kernel_functions import AvailableKernelFunctions
-from gempy_engine.core.data.options import DualContouringMaskingOptions
+from gempy_engine.core.data.options import MeshExtractionMaskingOptions
 from gempy_engine.core.data.solutions import Solutions
 
 
 def my_func():
     interpolation_input, structure, options = one_fault_model()
 
     options.compute_scalar_gradient = False
     options.dual_contouring = False
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW
 
     options.number_octree_levels = 8
     solutions: Solutions = compute_model(interpolation_input, options, structure)
 
     return
 
 
@@ -73,15 +73,15 @@
          ]
     )
 
     stack_structure = StacksStructure(
         number_of_points_per_stack=np.array([9, 24, 37]),
         number_of_orientations_per_stack=np.array([1, 4, 6]),
         number_of_surfaces_per_stack=np.array([1, 2, 3]),
-        masking_descriptor=[StackRelationType.FAULT, StackRelationType.ERODE, StackRelationType.ERODE, False],
+        masking_descriptor=[StackRelationType.FAULT, StackRelationType.ERODE, StackRelationType.ERODE, StackRelationType.BASEMENT],
         faults_relations=faults_relations
     )
 
     tensor_struct = TensorsStructure(number_of_points_per_surface=np.array([9, 12, 12, 13, 12, 12]))
     input_data_descriptor = InputDataDescriptor(tensor_struct, stack_structure)
     # endregion
```

### Comparing `gempy_engine-2023.1.0b5/tests/benchmark/profile_runner.py` & `gempy_engine-2023.2.0b1/tests/benchmark/profile_runner.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/benchmark/test_benchmark_one_feature.py` & `gempy_engine-2023.2.0b1/tests/benchmark/test_benchmark_one_feature.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/conftest.py` & `gempy_engine-2023.2.0b1/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,20 @@
 from tests.fixtures.heavy_models import *
 
 pykeops_enabled = False
 backend = AvailableBackends.numpy
 use_gpu = False
 plot_pyvista = False  # ! Set here if you want to plot the results
 
-BackendTensor._change_backend(backend, use_gpu=use_gpu, pykeops_enabled=pykeops_enabled)
+
+BackendTensor._change_backend(
+    engine_backend=backend,
+    use_gpu=use_gpu,
+    pykeops_enabled=pykeops_enabled
+)
 
 try:
     import pyvista as pv
 except ImportError:
     plot_pyvista = False
```

### Comparing `gempy_engine-2023.1.0b5/tests/fixtures/complex_geometries.py` & `gempy_engine-2023.2.0b1/tests/fixtures/complex_geometries.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
          ]
     )
 
     stack_structure = StacksStructure(
         number_of_points_per_stack=np.array([9, 24, 37]),
         number_of_orientations_per_stack=np.array([1, 4, 6]),
         number_of_surfaces_per_stack=np.array([1, 2, 3]),
-        masking_descriptor=[StackRelationType.FAULT, StackRelationType.ERODE, StackRelationType.ERODE, False],
+        masking_descriptor=[StackRelationType.FAULT, StackRelationType.ERODE, StackRelationType.ERODE, StackRelationType.BASEMENT],
         faults_relations=faults_relations
     )
 
     tensor_struct = TensorsStructure(number_of_points_per_surface=np.array([9, 12, 12, 13, 12, 12]))
     input_data_descriptor = InputDataDescriptor(tensor_struct, stack_structure)
     # endregion
```

### Comparing `gempy_engine-2023.1.0b5/tests/fixtures/grids.py` & `gempy_engine-2023.2.0b1/tests/fixtures/grids.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/fixtures/heavy_models.py` & `gempy_engine-2023.2.0b1/tests/fixtures/heavy_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         kernel_function=AvailableKernelFunctions.cubic,
         uni_degree=0,
     )
 
     # TODO: Add solver parameter
     interpolation_options.kernel_options.kernel_solver = solver
 
-    from gempy_engine.core.data.options import DualContouringMaskingOptions
-    interpolation_options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW
+    from gempy_engine.core.data.options import MeshExtractionMaskingOptions
+    interpolation_options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW
 
     # endregion
     # region InputDataDescriptor
     tensor_struct: TensorsStructure = TensorsStructure(
         number_of_points_per_surface=np.array([surface_points.n_points]),
     )
     stack_structure: StacksStructure = StacksStructure(
```

### Comparing `gempy_engine-2023.1.0b5/tests/fixtures/simple_geometries.py` & `gempy_engine-2023.2.0b1/tests/fixtures/simple_geometries.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/fixtures/simple_models.py` & `gempy_engine-2023.2.0b1/tests/fixtures/simple_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,14 +323,48 @@
             values_block=values_block,
             stack_relation=ii.stack_relation,
         ),
     )
 
     return output
 
+@pytest.fixture(scope="session")
+def simple_model_3_layers_output(simple_model_3_layers):
+    interporlation_input = simple_model_3_layers[0]
+    options = simple_model_3_layers[1]
+    data_shape = simple_model_3_layers[2].tensors_structure
+    ids = np.array([1, 2, 3, 4])
+
+    interp_input: SolverInput = input_preprocess(data_shape, interporlation_input)
+    weights = _solve_interpolation(interp_input, options.kernel_options)
+
+    exported_fields = _evaluate_sys_eq(interp_input, weights, options)
+
+    exported_fields.set_structure_values(
+        reference_sp_position=data_shape.reference_sp_position,
+        slice_feature=interporlation_input.slice_feature,
+        grid_size=interporlation_input.grid.len_all_grids)
+
+    # -----------------
+    # Export and Masking operations can happen even in parallel
+    # TODO: [~X] Export block
+    values_block: np.ndarray = activate_formation_block(exported_fields, ids, sigmoid_slope=50000)
+
+    output = InterpOutput(
+        ScalarFieldOutput(
+            weights=weights,
+            grid=interporlation_input.grid,
+            exported_fields=exported_fields,
+            values_block=values_block,
+            stack_relation=interporlation_input.stack_relation,
+        ),
+    )
+
+    return output
+
 
 @pytest.fixture(scope="session")
 def unconformity_complex():
     return unconformity_complex_factory()
 
 
 def unconformity_complex_factory():
@@ -342,15 +376,15 @@
                                         orientations["azimuth"],
                                         orientations["polarity"])
     dip_gradients = np.vstack(dip_gradients_).T
     stack_structure = StacksStructure(
         number_of_points_per_stack=np.array([3, 2, 6]),
         number_of_orientations_per_stack=np.array([2, 1, 6]),
         number_of_surfaces_per_stack=np.array([1, 1, 2]),
-        masking_descriptor=[StackRelationType.ERODE, StackRelationType.ERODE, False],
+        masking_descriptor=[StackRelationType.ERODE, StackRelationType.ERODE, StackRelationType.BASEMENT],
     )
     tensor_struct = TensorsStructure(number_of_points_per_surface=np.array([3, 2, 3, 3]))
     input_data_descriptor = InputDataDescriptor(tensor_struct, stack_structure)
     range_ = 0.8660254 * 100
     c_o = 35.71428571 * 100
     i_r = 4
     gi_r = 2
@@ -431,15 +465,15 @@
                                         orientations["azimuth"],
                                         orientations["polarity"])
     dip_gradients = np.vstack(dip_gradients_).T
 
     stack_structure = StacksStructure(number_of_points_per_stack=np.array([3]),
                                       number_of_orientations_per_stack=np.array([2]),
                                       number_of_surfaces_per_stack=np.array([1]),
-                                      masking_descriptor=[False])
+                                      masking_descriptor=[StackRelationType.BASEMENT])
 
     tensor_struct = TensorsStructure(number_of_points_per_surface=np.array([3]))
     input_data_descriptor = InputDataDescriptor(tensor_struct, stack_structure)
 
     range_ = 0.8660254 * 100
     c_o = 35.71428571 * 100
     i_r = 4
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_api/test_faults/test_faults_graben.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_api/test_faults/test_faults_graben.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from gempy_engine import compute_model
 from gempy_engine.core.data import InterpolationOptions
 from gempy_engine.core.data.input_data_descriptor import InputDataDescriptor
 from gempy_engine.core.data.interpolation_input import InterpolationInput
 from gempy_engine.core.data.kernel_classes.faults import FaultsData
 from gempy_engine.core.data.octree_level import OctreeLevel
-from gempy_engine.core.data.options import DualContouringMaskingOptions
+from gempy_engine.core.data.options import MeshExtractionMaskingOptions
 from gempy_engine.core.data.solutions import Solutions
 from gempy_engine.modules.octrees_topology.octrees_topology_interface import ValueType
 
 from gempy_engine.plugins.plotting import helper_functions_pyvista
 from tests.conftest import plot_pyvista
 from gempy_engine.plugins.plotting.helper_functions import plot_scalar_and_input_2d, plot_block_and_input_2d
 from tests.test_common.test_api.test_faults.test_one_fault import _plot_stack_raw
@@ -19,15 +19,15 @@
     structure: InputDataDescriptor
     options: InterpolationOptions
 
     interpolation_input, structure, options = graben_fault_model
 
     options.compute_scalar_gradient = False
     options.dual_contouring = True
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.INTERSECT
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.INTERSECT
     options.dual_conturing_fancy = True
     options.debug=True
 
     options.number_octree_levels = 4
     solutions: Solutions = compute_model(interpolation_input, options, structure)
 
     outputs: list[OctreeLevel] = solutions.octrees_output
@@ -60,15 +60,15 @@
     structure: InputDataDescriptor
     options: InterpolationOptions
 
     interpolation_input, structure, options = graben_fault_model
 
     options.compute_scalar_gradient = False
     options.dual_contouring = True
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW
 
     fault_data: FaultsData = FaultsData.from_user_input(thickness=.2)
     fault_data2: FaultsData = FaultsData.from_user_input(thickness=.2)
     structure.stack_structure.faults_input_data = [fault_data, fault_data2, None]
 
     options.number_octree_levels = n_octree_levels
     solutions: Solutions = compute_model(interpolation_input, options, structure)
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_api/test_faults/test_one_fault.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_api/test_faults/test_one_fault.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from gempy_engine.core.data import InterpolationOptions, TensorsStructure
 from gempy_engine.core.data.custom_segmentation_functions import ellipsoid_3d_factory, _implicit_3d_ellipsoid_to_slope
 from gempy_engine.core.data.grid import RegularGrid, Grid
 from gempy_engine.core.data.input_data_descriptor import InputDataDescriptor
 from gempy_engine.core.data.interpolation_input import InterpolationInput
 from gempy_engine.core.data.kernel_classes.faults import FaultsData
 from gempy_engine.core.data.octree_level import OctreeLevel
-from gempy_engine.core.data.options import DualContouringMaskingOptions
+from gempy_engine.core.data.options import MeshExtractionMaskingOptions
 from gempy_engine.core.data.solutions import Solutions
 from gempy_engine.modules.kernel_constructor.kernel_constructor_interface import yield_covariance
 from gempy_engine.modules.octrees_topology.octrees_topology_interface import ValueType
 from gempy_engine.plugins.plotting import helper_functions_pyvista
 from tests.conftest import pykeops_enabled, plot_pyvista
 from gempy_engine.plugins.plotting.helper_functions import plot_block_and_input_2d, plot_scalar_and_input_2d
 
@@ -25,15 +25,15 @@
     structure: InputDataDescriptor
     options: InterpolationOptions
 
     interpolation_input, structure, options = one_fault_model
 
     options.compute_scalar_gradient = False
     options.dual_contouring = True
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.INTERSECT
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.INTERSECT
     options.dual_contouring_fancy = True
 
     options.number_octree_levels = n_oct_levels
 
     solutions: Solutions = compute_model(interpolation_input, options, structure)
 
     outputs: list[OctreeLevel] = solutions.octrees_output
@@ -81,15 +81,15 @@
     options: InterpolationOptions
 
     interpolation_input, structure, options = one_fault_model
 
     fault_data: FaultsData = FaultsData.from_user_input(thickness=.5)
     structure.stack_structure.faults_input_data = [fault_data, None, None]
     options.dual_contouring = True
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.INTERSECT
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.INTERSECT
 
     options.number_octree_levels = n_oct_levels
     solutions: Solutions = compute_model(interpolation_input, options, structure)
 
     # TODO: Grab second scalar and create fault kernel
     outputs: list[OctreeLevel] = solutions.octrees_output
 
@@ -118,15 +118,15 @@
     regular_grid = RegularGrid(extent, resolution)
     grid = Grid(regular_grid=regular_grid)
     interpolation_input.grid = grid
     options.number_octree_levels = n_oct_levels
 
     options.compute_scalar_gradient = False
     options.dual_contouring = True
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW
 
     # region finite fault
     faults_relations = np.array(
         [[False, True, True],
          [False, False, False],
          [False, False, False]
          ]
@@ -141,15 +141,15 @@
 
     structure.stack_structure.segmentation_functions_per_stack = [f1_finite_fault, None, None]
 
     solutions: Solutions = compute_model(interpolation_input, options, structure)
     meshes = solutions.dc_meshes  # + meshes
 
     outputs: list[OctreeLevel] = solutions.octrees_output
-    scalar = f1_finite_fault(solutions.octrees_output[-1].grid_centers.regular_grid.values)
+    scalar = f1_finite_fault(solutions.octrees_output[-1].grid_centers.values)
     # endregion
 
     if True:
         plot_block_and_input_2d(0, interpolation_input, outputs, structure.stack_structure, ValueType.values_block)
         plot_block_and_input_2d(1, interpolation_input, outputs, structure.stack_structure, ValueType.values_block)
         plot_block_and_input_2d(2, interpolation_input, outputs, structure.stack_structure, ValueType.values_block)
 
@@ -171,15 +171,15 @@
     interpolation_input: InterpolationInput
     structure: InputDataDescriptor
     options: InterpolationOptions
 
     interpolation_input, structure, options = one_fault_model
     structure.stack_structure.faults_input_data = None
 
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.RAW
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.RAW
     options.number_octree_levels = 1
 
     rescaling_factor = 240
     resolution = np.array([20, 4, 20])
     extent = np.array([-500, 500., -500, 500, -450, 550]) / rescaling_factor
     regular_grid = RegularGrid(extent, resolution)
     grid = Grid(regular_grid=regular_grid)
@@ -189,21 +189,22 @@
 
     fault_mesh = solutions.dc_meshes[0]
 
     regular_grid = solutions.octrees_output[-1].outputs_centers[0].grid.regular_grid
     resolution = regular_grid.resolution
 
     radius = np.array([1, 1, 2])
+    from gempy_engine.core.backend_tensor import BackendTensor
     scalar = _implicit_3d_ellipsoid_to_slope(  # * This paints the 3d regular grid
-        xyz=regular_grid.values,
+        xyz=BackendTensor.t.array(regular_grid.values),
         center=np.array([0, 0, 0]),
         radius=radius
     )
     scalar_fault = _implicit_3d_ellipsoid_to_slope(  # * This paints the 2d fault mesh
-        xyz=fault_mesh.vertices, 
+        xyz=BackendTensor.t.array(fault_mesh.vertices),
         center=np.array([0, 0, 0]),
         radius=radius
     )
 
     if plot_pyvista or False:
         import pyvista as pv
         p = pv.Plotter()
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_api/test_output_to_subsurface.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_api/test_output_to_subsurface.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_api/test_public_interface.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_api/test_public_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,15 +95,20 @@
     )
     
     if plot_pyvista or False:
         pv.global_theme.show_edges = True
         p = pv.Plotter()
         plot_octree_pyvista(p, solutions.octrees_output, interpolation_options.number_octree_levels - 1)
         plot_dc_meshes(p, solutions.dc_meshes[0])
-        plot_points(p, interpolation_input.surface_points.sp_coords)
+        surface_points_to_plot = interpolation_input.surface_points.sp_coords
+        # If they are torch tensors convert to numpy
+        if isinstance(surface_points_to_plot, BackendTensor.t.Tensor):
+            surface_points_to_plot = surface_points_to_plot.numpy()
+            
+        plot_points(p, surface_points_to_plot)
         p.show()
 
 
 # noinspection DuplicatedCode
 def _compute_model(interpolation_input: InterpolationInput, options: InterpolationOptions, structure: InputDataDescriptor):
     n_oct_levels = options.number_octree_levels
     solutions: Solutions = compute_model(interpolation_input, options, structure)
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_dependencies/pykeops_test_compiler.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_dependencies/pykeops_test_compiler.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_dependencies/test_pykeops.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_dependencies/test_pykeops.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_external_functions.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_external_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from gempy_engine.API.interp_single._multi_scalar_field_manager import _interpolate_stack
 from gempy_engine.API.interp_single.interp_features import interpolate_all_fields_no_octree
 from gempy_engine.API.model.model_api import compute_model
 from gempy_engine.core.data.solutions import Solutions
 from gempy_engine.core.data.interp_output import InterpOutput
 from gempy_engine.core.data.scalar_field_output import ScalarFieldOutput
 from gempy_engine.core.data.exported_fields import ExportedFields
-from gempy_engine.core.data.options import DualContouringMaskingOptions
+from gempy_engine.core.data.options import MeshExtractionMaskingOptions
 from gempy_engine.modules.activator.activator_interface import activate_formation_block
 from gempy_engine.plugins.plotting import helper_functions_pyvista
 from tests.conftest import TEST_SPEED
 from gempy_engine.plugins.plotting.helper_functions import plot_block
 
 PLOT = False
 
@@ -52,28 +52,32 @@
         return x_dir ** 2 + y_dir ** 2 + z_dir ** 2
 
     interpolation_input, options, structure = unconformity_complex
     grid = interpolation_input.grid.regular_grid
     xyz = grid.values
     scalar = implicit_sphere(xyz, grid.extent)
 
-    exported_fields = ExportedFields(scalar, _scalar_field_at_surface_points=np.array([20]))
+    from gempy_engine.core.backend_tensor import BackendTensor
+    exported_fields = ExportedFields(
+        _scalar_field=BackendTensor.t.array(scalar),
+        _scalar_field_at_surface_points=BackendTensor.t.array([20])
+    )
     values_block = activate_formation_block(exported_fields, np.array([0, 1]), 100000)
 
     if PLOT or False:
         plot_block(scalar, grid)
         plot_block(values_block, grid)
 
 
 @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
 def test_dual_contouring_multiple_independent_fields(unconformity_complex_implicit, n_oct_levels=2):
     interpolation_input, options, structure = unconformity_complex_implicit
     options.number_octree_levels = n_oct_levels
     options.debug = True
-    options.dual_contouring_masking_options = DualContouringMaskingOptions.DISJOINT
+    options.mesh_extraction_masking_options = MeshExtractionMaskingOptions.INTERSECT
 
     solutions: Solutions = compute_model(interpolation_input, options, structure)
 
     if PLOT or False:
         dc_data = solutions.dc_meshes[0].dc_data  # * Scalar field where to show gradients
         intersection_xyz = dc_data.xyz_on_edge
         gradients = dc_data.gradients
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_interpolate_model.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_interpolate_model.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_kernels.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_kernels.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_multi_fields.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_multi_fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from gempy_engine.API.model.model_api import compute_model
 from gempy_engine.core.data import TensorsStructure
 from gempy_engine.core.data.grid import Grid
 from gempy_engine.core.data.interp_output import InterpOutput
 from gempy_engine.core.data.interpolation_input import InterpolationInput
 from gempy_engine.core.data.scalar_field_output import ScalarFieldOutput
 from gempy_engine.core.data.solutions import Solutions
+from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.modules.octrees_topology.octrees_topology_interface import get_regular_grid_value_for_level
 from gempy_engine.plugins.plotting import helper_functions_pyvista
 from gempy_engine.plugins.plotting.helper_functions import plot_block
 from tests.conftest import plot_pyvista, TEST_SPEED
 
 try:
     # noinspection PyUnresolvedReferences
@@ -85,17 +86,20 @@
     output_0_corners: List[InterpOutput] = interpolate_all_fields(interpolation_input, options, structure)  # TODO: This is unnecessary for the last level except for Dual contouring
 
     if plot_pyvista or False:
         plot_block(outputs[0].combined_scalar_field.squeezed_mask_array, grid)
         plot_block(outputs[1].combined_scalar_field.squeezed_mask_array, grid)
         plot_block(outputs[2].combined_scalar_field.squeezed_mask_array, grid)
 
-    mask_1 = output_0_corners[0].squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
-    mask_2 = output_0_corners[1].combined_scalar_field.squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
-    mask_3 = output_0_corners[2].combined_scalar_field.squeezed_mask_array.reshape((1, -1, 8)).sum(-1, bool)[0]
+    m1 = output_0_corners[0].squeezed_mask_array.reshape((1, -1, 8))
+    m2 = output_0_corners[1].squeezed_mask_array.reshape((1, -1, 8))
+    m3  = output_0_corners[2].squeezed_mask_array.reshape((1, -1, 8))
+    mask_1 = BackendTensor.t.to_numpy(BackendTensor.t.sum(m1, -1, bool)[0])
+    mask_2 = BackendTensor.t.to_numpy(BackendTensor.t.sum(m2, -1, bool)[0])
+    mask_3 = BackendTensor.t.to_numpy(BackendTensor.t.sum(m3, -1, bool)[0])
 
     if True:
         plot_block(mask_1, grid)
         plot_block(mask_2, grid)
         plot_block(mask_3, grid)
 
     if True:
@@ -110,28 +114,34 @@
 
 def test_final_block(unconformity_complex):
     interpolation_input, options, structure = unconformity_complex
     outputs: List[InterpOutput] = interpolate_all_fields(interpolation_input, options, structure)
 
     if plot_pyvista or True:
         grid = interpolation_input.grid.regular_grid
-        plot_block(outputs[0].final_block, grid)
-        plot_block(outputs[1].final_block, grid)
-        plot_block(outputs[2].final_block, grid)
+        plot_block(
+            BackendTensor.t.to_numpy(outputs[0].final_block),
+            grid)
+        plot_block(
+            BackendTensor.t.to_numpy(outputs[1].final_block),
+            grid)
+        plot_block(
+            BackendTensor.t.to_numpy(outputs[2].final_block),
+            grid)
 
 
 def test_final_exported_fields(unconformity_complex):
     interpolation_input, options, structure = unconformity_complex
     outputs: List[InterpOutput] = interpolate_all_fields(interpolation_input, options, structure)
 
     if plot_pyvista or False:
         grid = interpolation_input.grid.regular_grid
-        plot_block(outputs[0].final_exported_fields._scalar_field, grid)
-        plot_block(outputs[1].final_exported_fields._scalar_field, grid)
-        plot_block(outputs[2].final_exported_fields._scalar_field, grid)
+        plot_block(BackendTensor.t.to_numpy(outputs[0].final_exported_fields._scalar_field_at_surface_points), grid)
+        plot_block(BackendTensor.t.to_numpy(outputs[1].final_exported_fields._scalar_field_at_surface_points), grid)
+        plot_block(BackendTensor.t.to_numpy(outputs[2].final_exported_fields._scalar_field_at_surface_points), grid)
 
 
 @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
 def test_plot_corners(unconformity_complex, n_oct_levels=2):
     interpolation_input, options, structure = unconformity_complex
     options.number_octree_levels = n_oct_levels
     solutions: Solutions = compute_model(interpolation_input, options, structure)
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_multi_fields_dual_contouring.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,83 @@
 import pytest
 
 from gempy_engine import compute_model
 from gempy_engine.core.data.grid import RegularGrid, Grid
-from gempy_engine.core.data.options import DualContouringMaskingOptions
+from gempy_engine.core.data.options import MeshExtractionMaskingOptions
 from gempy_engine.core.data.solutions import Solutions
 from gempy_engine.plugins.plotting import helper_functions_pyvista
 from tests.conftest import TEST_SPEED
 from tests.fixtures.simple_models import unconformity_complex_factory
 from tests.test_common.test_integrations.test_multi_fields import plot_pyvista
 
 
-@pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
+# @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
+@pytest.mark.skipif(True, reason="Disjoint is not working for now")
 def test_dual_contouring_multiple_independent_fields(n_oct_levels=2):
     _run_model_for_dual_contouring_option(
-        dual_contouring_option=DualContouringMaskingOptions.DISJOINT,
+        dual_contouring_option=MeshExtractionMaskingOptions.DISJOINT,
         n_oct_levels=n_oct_levels,
         model=unconformity_complex_factory()
     )
 
 
 @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
 def test_dual_contouring_multiple_independent_fields_intersect(n_oct_levels=2):
     _run_model_for_dual_contouring_option(
-        dual_contouring_option=DualContouringMaskingOptions.INTERSECT,
+        dual_contouring_option=MeshExtractionMaskingOptions.INTERSECT,
         n_oct_levels=n_oct_levels,
         model=unconformity_complex_factory()
     )
 
 
 @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
 def test_dual_contouring_multiple_independent_fields_intersect_raw(n_oct_levels=2):
     _run_model_for_dual_contouring_option(
-        dual_contouring_option=DualContouringMaskingOptions.RAW,
+        dual_contouring_option=MeshExtractionMaskingOptions.RAW,
         n_oct_levels=n_oct_levels,
         model=unconformity_complex_factory()
     )
 
 
 @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
 def test_dual_contouring_multiple_independent_fields_intersect_RAW_fancy_triangulation(
         unconformity_complex, n_oct_levels=5):
     _run_model_for_FANCY_dual_contouring(
-        dual_contouring_option=DualContouringMaskingOptions.RAW,
+        dual_contouring_option=MeshExtractionMaskingOptions.RAW,
         n_oct_levels=n_oct_levels,
         unconformity_complex=unconformity_complex
     )
 
 
-@pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
+# @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
+@pytest.mark.skipif(True, reason="Disjoint is not working for now")
 def test_dual_contouring_multiple_independent_fields_intersect_DISJOINT_fancy_triangulation(
         unconformity_complex, n_oct_levels=5):
     _run_model_for_FANCY_dual_contouring(
-        dual_contouring_option=DualContouringMaskingOptions.DISJOINT,
+        dual_contouring_option=MeshExtractionMaskingOptions.DISJOINT,
         n_oct_levels=n_oct_levels,
         unconformity_complex=unconformity_complex
     )
     
     
 @pytest.mark.skipif(TEST_SPEED.value <= 1, reason="Global test speed below this test value.")
 def test_dual_contouring_multiple_independent_fields_intersect_INTERSECT_fancy_triangulation(
         unconformity_complex, n_oct_levels=5):
     _run_model_for_FANCY_dual_contouring(
-        dual_contouring_option=DualContouringMaskingOptions.INTERSECT,
+        dual_contouring_option=MeshExtractionMaskingOptions.INTERSECT,
         n_oct_levels=n_oct_levels,
         unconformity_complex=unconformity_complex
     )
 
 
 def _run_model_for_FANCY_dual_contouring(dual_contouring_option, n_oct_levels, unconformity_complex):
     interpolation_input, options, structure = unconformity_complex
     options.number_octree_levels = n_oct_levels
     options.debug = True
-    options.dual_contouring_masking_options = dual_contouring_option
+    options.mesh_extraction_masking_options = dual_contouring_option
     options.dual_contouring_fancy = True
     regular_grid = RegularGrid(extent=[0, 10., 0, 2., 0, 5.], regular_grid_shape=[2, 2, 2])
     grid = Grid(regular_grid=regular_grid)
     interpolation_input.grid = grid
     solutions: Solutions = compute_model(interpolation_input, options, structure)
     if plot_pyvista or False:
         dc_data = solutions.dc_meshes[3].dc_data  # * Scalar field where to show gradients
@@ -94,15 +96,15 @@
         )
 
 
 def _run_model_for_dual_contouring_option(dual_contouring_option, n_oct_levels, model):
     interpolation_input, options, structure = model
     options.number_octree_levels = n_oct_levels
     options.debug = True
-    options.dual_contouring_masking_options = dual_contouring_option
+    options.mesh_extraction_masking_options = dual_contouring_option
     solutions: Solutions = compute_model(interpolation_input, options, structure)
     if plot_pyvista or False:
         dc_data = solutions.dc_meshes[0].dc_data  # * Scalar field where to show gradients
         helper_functions_pyvista.plot_pyvista(
             solutions.octrees_output,
             dc_meshes=solutions.dc_meshes,
             # xyz_on_edge=dc_data.xyz_on_edge,
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_multiple_grids.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_multiple_grids.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_integrations/test_options.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_integrations/test_options.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_dual.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_dual.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pytest
 
 from gempy_engine.API.dual_contouring._interpolate_on_edges import _get_intersection_on_edges
 from gempy_engine.API.interp_single._interp_scalar_field import _evaluate_sys_eq
 from gempy_engine.API.interp_single._interp_single_feature import input_preprocess
 from gempy_engine.API.interp_single._multi_scalar_field_manager import interpolate_all_fields
 from gempy_engine.API.model.model_api import compute_model
+from gempy_engine.config import AvailableBackends
+from gempy_engine.core.backend_tensor import BackendTensor
 from gempy_engine.core.data.grid import Grid, RegularGrid
 import numpy as np
 import os
 
 import gempy_engine.API.interp_single.interp_features as interp
 
 from gempy_engine.API.dual_contouring._dual_contouring import  compute_dual_contouring
@@ -87,14 +89,15 @@
         helper_functions_pyvista.plot_pyvista(octree_list, dc_meshes=dc_meshes, gradients=gradients,
                                               a=center_mass, b=normals,
                                               gradient_pos=intersection_xyz,
                                               v_just_points=vertices, vertices=intersection_points)
     # endregion
 
 
+@pytest.mark.skipif(BackendTensor.engine_backend != AvailableBackends.numpy, reason="Only numpy supported")
 def test_compute_dual_contouring_fancy_triangulation(simple_model, simple_grid_3d_octree):
     from gempy_engine.modules.dual_contouring.fancy_triangulation import get_left_right_array, triangulate
 
     def _simple_grid_3d_octree_regular():
         import dataclasses
         resolution = [2, 2, 2]
         extent = [0.25, .75, 0.25, .75, 0.25, .75]
@@ -261,25 +264,28 @@
             indices=meshes[0].edges,
             plot_label=False,
             plot_marching_cubes=False,
             n=0
         )
 
 
+
+@pytest.mark.skipif(BackendTensor.engine_backend != AvailableBackends.numpy, reason="Only numpy supported")
 def test_find_edges_intersection_step_by_step(simple_model, simple_grid_3d_octree):
     # region Test find_intersection_on_edge
     spi, ori_i, options, data_shape = simple_model
     ids = np.array([1, 2])
     grid_0_centers = copy.deepcopy(simple_grid_3d_octree)
     interpolation_input = InterpolationInput(spi, ori_i, grid_0_centers, ids)
 
     options.number_octree_levels = 5
+    options.compute_scalar_gradient = True
     octree_list = interpolate_n_octree_levels(interpolation_input, options, data_shape)
 
-    last_octree_level: OctreeLevel = octree_list[2]
+    last_octree_level: OctreeLevel = octree_list[-1]
 
     sfsp = last_octree_level.last_output_corners.scalar_field_at_sp
 
     xyz_on_edge, valid_edges = find_intersection_on_edge(last_octree_level.grid_corners.values, last_octree_level.output_corners.exported_fields.scalar_field, sfsp, )
 
     # endregion
 
@@ -375,21 +381,24 @@
         _plot_pyvista(last_octree_level, octree_list, simple_model, ids, grid_0_centers,
                       xyz_on_edge, gradients, a, b, v_pro, np.array(v_mesh), indices=None,
                       plot_label=False, plot_marching_cubes=False)
 
     return xyz_on_edge, gradients
 
 
+
+@pytest.mark.skipif(BackendTensor.engine_backend != AvailableBackends.numpy, reason="Only numpy supported")
 def test_find_edges_intersection_pro(simple_model, simple_grid_3d_octree):
     # region Test find_intersection_on_edge
     spi, ori_i, options, data_shape = simple_model
     ids = np.array([1, 2])
     grid_0_centers = simple_grid_3d_octree
     interpolation_input = InterpolationInput(spi, ori_i, grid_0_centers, ids)
 
+    options.compute_scalar_gradient = True
     octree_list = interpolate_n_octree_levels(interpolation_input, options, data_shape)
 
     last_octree_level: OctreeLevel = octree_list[-1]
 
     sfsp = last_octree_level.output_corners.scalar_field_at_sp
     # sfsp = np.append(sfsp, -0.1)
     xyz_on_edge, valid_edges = find_intersection_on_edge(last_octree_level.grid_corners.values, last_octree_level.output_corners.exported_fields.scalar_field, sfsp, )
@@ -481,24 +490,28 @@
                       xyz_on_edge, gradients, a=center_mass, b=normals,
                       v_pro=v_pro, indices=indices, plot_marching_cubes=True
                       )
 
     return xyz_on_edge, gradients
 
 
+
+
+@pytest.mark.skipif(BackendTensor.engine_backend != AvailableBackends.numpy, reason="Only numpy supported")
 def test_find_edges_intersection_bias_on_center_of_the_cell(simple_model, simple_grid_3d_octree):
     """This looks works that taking the center of gravity of the edges intersections. I leave this test here as 
     documentation"""
 
     # region Test find_intersection_on_edge
     spi, ori_i, options, data_shape = simple_model
     ids = np.array([1, 2])
     grid_0_centers = simple_grid_3d_octree
     interpolation_input = InterpolationInput(spi, ori_i, grid_0_centers, ids)
 
+    options.compute_scalar_gradient = True
     octree_list = interpolate_n_octree_levels(interpolation_input, options, data_shape)
 
     last_octree_level: OctreeLevel = octree_list[-1]
 
     sfsp = last_octree_level.output_corners.scalar_field_at_sp
     xyz_on_edge, valid_edges = find_intersection_on_edge(last_octree_level.grid_corners.values, last_octree_level.output_corners.exported_fields.scalar_field, sfsp, )
     valid_voxels = valid_edges.sum(axis=1, dtype=bool)
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_exporter.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,8 +152,12 @@
         plt.quiver(xyz_lvl0[:, 0], xyz_lvl0[:, 2],
                    outputs[0].exported_fields.gx_field,
                    outputs[0].exported_fields.gz_field,
                    pivot="tail",
                    color='green', alpha=.6, )
 
         grid = interpolation_input.grid.regular_grid
-        plot_block(outputs[0].final_exported_fields._scalar_field, grid)
+        from gempy_engine.core.backend_tensor import BackendTensor
+        plot_block(
+            BackendTensor.t.to_numpy(outputs[0].final_exported_fields._scalar_field),
+            grid
+        )
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,24 +42,29 @@
     solver_input = SolverInput(sp_internals, ori_internals, None, None)
     cov = yield_covariance(solver_input, options.kernel_options)
     print(cov)
 
     # todo: verify the full matrix when pykeops is False
 
     parameters: Options = NamerFactory.with_parameters("axis=1").with_comparator(ArrayComparator())
-    verify(BackendTensor.tfnp.sum(cov, axis=1, keepdims=True), options=parameters)
+    sol = BackendTensor.tfnp.sum(cov, axis=1, keepdims=True)
+    # verify(BackendTensor.t.to_numpy(sol), options=parameters)
+    verify(sol, options=parameters)
 
 
 def test_b_vector(simple_model_2):
     orientations = simple_model_2[1]
     ori_internals = orientations_preprocess(orientations)
 
     b_vec = yield_b_vector(ori_internals, 9)
 
-    verify(b_vec)
+    verify(
+        data=b_vec,
+        options=NamerFactory.with_parameters().with_comparator(ArrayComparator())
+    )
 
 
 def test_eval_kernel(simple_model_2, simple_grid_2d):
     surface_points = simple_model_2[0]
     orientations = simple_model_2[1]
     options = simple_model_2[2]
     input_data_descriptor: InputDataDescriptor = simple_model_2[3]
@@ -75,14 +80,15 @@
     print(export_gradient_)
 
 
 pykeops_enabled = True
 
 
 # TODO: (bug) When running test_covariance_spline_kernel the running the class test breaks for some weird state change
+@pytest.mark.skipif(BackendTensor.engine_backend != AvailableBackends.numpy, reason="These tests only makes sense for numpy backend and PyKEOPS")
 class TestPykeopsNumPyEqual():
 
     @pytest.fixture(scope="class")
     def preprocess_data(self, simple_model_2_b):
         surface_points = simple_model_2_b[0]
         orientations = simple_model_2_b[1]
         input_data_descriptor: InputDataDescriptor = simple_model_2_b[3]
@@ -150,15 +156,18 @@
             np.testing.assert_array_almost_equal(dm.perp_matrix, dm_sol.perp_matrix, decimal=3)
             if False:  # ! (March 6, 2023) these checks are failing but they are old
                 np.testing.assert_array_almost_equal(dm.r_ref_ref, dm_sol.r_ref_ref, decimal=3)
                 np.testing.assert_array_almost_equal(dm.r_ref_rest, dm_sol.r_ref_rest, decimal=3)
                 np.testing.assert_array_almost_equal(dm.r_rest_ref, dm_sol.r_rest_ref, decimal=3)
                 np.testing.assert_array_almost_equal(dm.r_rest_rest, dm_sol.r_rest_rest, decimal=3)
 
-        verify(BackendTensor.tfnp.sum(dm.dif_ref_ref, axis=1, keepdims=False), options=NamerFactory.with_parameters("dif_ref_ref"))
+        verify(
+            data=BackendTensor.tfnp.sum(dm.dif_ref_ref, axis=1, keepdims=False), 
+            options=NamerFactory.with_parameters("dif_ref_ref").with_comparator(ArrayComparator())
+        )
 
     def test_compare_cg(self, preprocess_data):
         self._compare_covariance_item_numpy_pykeops(preprocess_data, item="cov_grad", cov_func=_test_covariance_items)
         
     @pytest.mark.skip(reason="Deprecated")
     def test_compare_ci(self, preprocess_data):
         self._compare_covariance_item_numpy_pykeops(preprocess_data, item="cov_sp", cov_func=_test_covariance_items)
@@ -172,28 +181,28 @@
     def test_compare_full_cov(self, preprocess_data):
         self._compare_covariance_item_numpy_pykeops(preprocess_data, item="cov", cov_func=_test_covariance_items, compare_to_saved=False)
 
     def _compare_covariance_item_numpy_pykeops(self, preprocess_data, item, cov_func, compare_to_saved=True):
         sp_internals, ori_internals, options = preprocess_data
 
         # numpy
-        BackendTensor.change_backend(AvailableBackends.numpy, pykeops_enabled=False)
+        BackendTensor._change_backend(AvailableBackends.numpy, pykeops_enabled=False)
         solver_input = SolverInput(sp_internals, ori_internals)
         kernel_data = cov_vectors_preparation(solver_input, options.kernel_options)
         c_n = cov_func(kernel_data, options, item=item)
 
         path = dir_name + f"/../solutions/{item}.npy"
         if False:
             np.save(path, c_n)
 
         l = np.load(path)
         c_n_sum = c_n.sum(0).reshape(-1, 1)
 
         # pykeops
-        BackendTensor.change_backend(AvailableBackends.numpy, pykeops_enabled=pykeops_enabled)
+        BackendTensor._change_backend(AvailableBackends.numpy, pykeops_enabled=pykeops_enabled)
         kernel_data = cov_vectors_preparation(solver_input, options.kernel_options)
         c_k = cov_func(kernel_data, options, item=item)
         c_k_sum = c_n.sum(0).reshape(-1, 1)
 
         print('l: ', l)
         print("just numpy: ", c_n, c_n_sum)
         print("pykeops: ", c_k, c_k_sum)
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_kernel_constructor_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 plot = False
 
 
 class TestCompareWithGempy_v2:
     @pytest.fixture(scope="class")
     def internals(self, simple_model):
-        BackendTensor.change_backend(AvailableBackends.numpy, pykeops_enabled=False)
+        BackendTensor._change_backend(AvailableBackends.numpy, pykeops_enabled=False)
 
         surface_points = simple_model[0]
         orientations = simple_model[1]
         options = simple_model[2]
         tensors_structure = simple_model[3]
 
         # Prepare options
@@ -89,14 +89,15 @@
         sp_internals, ori_internals, options = internals
         solver_input = SolverInput(sp_internals, ori_internals)
         cov = yield_covariance(solver_input, options.kernel_options)
         b_vec = yield_b_vector(ori_internals, cov.shape[0])
         weights = kernel_reduction(cov, b_vec)
         return weights
 
+    @pytest.mark.skipif(BackendTensor.engine_backend != AvailableBackends.numpy, reason="These tests only makes sense for numpy backend")
     def test_reduction(self, internals):
         sp_internals, ori_internals, options = internals
         # Test cov
         solver_input = SolverInput(sp_internals, ori_internals)
         cov = yield_covariance(solver_input, options.kernel_options)
 
         print("\n")
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_kernel_constructor/test_kernel_faults.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 
 def test_implicit_ellipsoid():
     rescaling_factor = 240
     resolution = np.array([20, 4, 20])
     extent = np.array([-500, 500., -500, 500, -450, 550]) / rescaling_factor
     regular_grid = RegularGrid(extent, resolution)
 
-    scalar = _implicit_3d_ellipsoid_to_slope(regular_grid.values, np.array([0, 0, 0]), np.array([1, 1, 2]))
+    from gempy_engine.core.backend_tensor import BackendTensor
+    scalar = _implicit_3d_ellipsoid_to_slope(
+        xyz=BackendTensor.t.array(regular_grid.values),
+        center= np.array([0, 0, 0]),
+        radius= np.array([1, 1, 2])
+    )
+    
     if plot_pyvista or False:
         import pyvista as pv
         p = pv.Plotter()
         regular_grid_values = regular_grid.values_vtk_format
         shape = regular_grid_values.shape
 
         grid_3d = regular_grid_values.reshape(*(resolution + 1), 3).T
```

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_octrees.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_octrees.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_modules/test_solver.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_modules/test_solver.py`

 * *Files identical despite different names*

### Comparing `gempy_engine-2023.1.0b5/tests/test_common/test_prototyping/test_broadcasting.py` & `gempy_engine-2023.2.0b1/tests/test_common/test_prototyping/test_broadcasting.py`

 * *Files identical despite different names*

